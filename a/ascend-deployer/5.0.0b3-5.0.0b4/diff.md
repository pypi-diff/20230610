# Comparing `tmp/ascend_deployer-5.0.0b3-py3-none-any.whl.zip` & `tmp/ascend_deployer-5.0.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,264 +1,402 @@
-Zip file size: 369195 bytes, number of entries: 262
--rw-r--r--  2.0 unx    11558 b- defN 23-Apr-08 02:25 ascend_deployer/LICENSE
--rw-r--r--  2.0 unx    67023 b- defN 23-Apr-08 02:25 ascend_deployer/README.en.rst
--rw-r--r--  2.0 unx     4129 b- defN 23-Apr-08 02:25 ascend_deployer/README.rst
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-08 02:25 ascend_deployer/__init__.py
--rw-r--r--  2.0 unx      244 b- defN 23-Apr-08 02:25 ascend_deployer/ansible.cfg
--rwxr-x---  2.0 unx    61429 b- defN 23-Apr-08 02:25 ascend_deployer/install.sh
--rw-r--r--  2.0 unx      125 b- defN 23-Apr-08 02:25 ascend_deployer/inventory_file
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-08 02:25 ascend_deployer/start_download.bat
--rwxr-x---  2.0 unx    10751 b- defN 23-Apr-08 02:25 ascend_deployer/start_download.sh
--rw-r--r--  2.0 unx      112 b- defN 23-Apr-08 02:25 ascend_deployer/start_download_ui.bat
--rw-r--r--  2.0 unx     2104 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/__init__.py
--rw-r--r--  2.0 unx      325 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/config.ini
--rw-r--r--  2.0 unx    11164 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/deb_downloader.py
--rw-r--r--  2.0 unx    21026 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/download_util.py
--rw-r--r--  2.0 unx     8717 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/downloader.py
--rw-r--r--  2.0 unx     7914 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/downloader_ui.py
--rw-r--r--  2.0 unx     4552 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/logger_config.py
--rw-r--r--  2.0 unx     4470 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/os_dep_downloader.py
--rw-r--r--  2.0 unx    12509 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/other_downloader.py
--rw-r-----  2.0 unx     2258 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/other_resources.json
--rw-r--r--  2.0 unx    11816 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/pip_downloader.py
--rw-r-----  2.0 unx     8754 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/python_version.json
--rw-r-----  2.0 unx     1783 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/requirements.txt
--rw-r--r--  2.0 unx    21007 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/rpm_downloader.py
--rw-r--r--  2.0 unx     7161 b- defN 22-Dec-07 12:00 ascend_deployer/downloader/software_mgr.py
--rw-r-----  2.0 unx      284 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/support_url.json
--rw-r--r--  2.0 unx     9087 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/deb_downloader.cpython-36.pyc
--rw-r--r--  2.0 unx    18614 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/download_util.cpython-36.pyc
--rw-r--r--  2.0 unx     6124 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/downloader.cpython-36.pyc
--rw-r--r--  2.0 unx     3190 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/logger_config.cpython-36.pyc
--rw-r--r--  2.0 unx     3350 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/os_dep_downloader.cpython-36.pyc
--rw-r--r--  2.0 unx     8456 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/other_downloader.cpython-36.pyc
--rw-r--r--  2.0 unx     9460 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/pip_downloader.cpython-36.pyc
--rw-r--r--  2.0 unx    15637 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/rpm_downloader.cpython-36.pyc
--rw-r--r--  2.0 unx     6264 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/__pycache__/software_mgr.cpython-36.pyc
--rw-r-----  2.0 unx     6926 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.6_aarch64/pkg_info.json
--rw-r-----  2.0 unx      378 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.6_aarch64/source.repo
--rw-r-----  2.0 unx     6287 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.6_x86_64/pkg_info.json
--rw-r-----  2.0 unx      391 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.6_x86_64/source.repo
--rw-r-----  2.0 unx     6926 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.7_aarch64/pkg_info.json
--rw-r-----  2.0 unx      378 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/BCLinux_7.7_aarch64/source.repo
--rw-r-----  2.0 unx     8690 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
--rw-r-----  2.0 unx      234 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
--rw-r-----  2.0 unx     8475 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
--rw-r-----  2.0 unx      223 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
--rw-r--r--  2.0 unx    12171 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/config/CentOS_8.2_aarch64/pkg_info.json
--rw-r-----  2.0 unx      457 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_8.2_aarch64/source.repo
--rw-r--r--  2.0 unx    11193 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/config/CentOS_8.2_x86_64/pkg_info.json
--rw-r-----  2.0 unx      452 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/CentOS_8.2_x86_64/source.repo
--rw-r-----  2.0 unx    12274 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_10.0_x86_64/pkg_info.json
--rw-r-----  2.0 unx      131 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_10.0_x86_64/source.list
--rw-r-----  2.0 unx     9007 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_9.9_aarch64/pkg_info.json
--rw-r-----  2.0 unx      129 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_9.9_aarch64/source.list
--rw-r-----  2.0 unx     9447 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_9.9_x86_64/pkg_info.json
--rw-r-----  2.0 unx      129 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Debian_9.9_x86_64/source.list
--rw-r-----  2.0 unx    65900 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
--rw-r-----  2.0 unx     6028 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
--rw-r-----  2.0 unx      130 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
--rw-r-----  2.0 unx    42840 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
--rw-r-----  2.0 unx     4518 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
--rw-r-----  2.0 unx      130 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
--rw-r-----  2.0 unx    42208 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
--rw-r-----  2.0 unx     3827 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
--rw-r-----  2.0 unx       65 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
--rw-r-----  2.0 unx    60396 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
--rw-r-----  2.0 unx     2490 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
--rw-r-----  2.0 unx      187 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
--rw-r-----  2.0 unx    60964 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
--rw-r-----  2.0 unx     2156 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
--rw-r-----  2.0 unx      180 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
--rw-r-----  2.0 unx     3831 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/pkg_info.json
--rw-r-----  2.0 unx      222 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/source.list
--rw-r--r--  2.0 unx     5526 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/Linx_6.0.100_aarch64/pkg_info.json
--rw-r--r--  2.0 unx      127 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/Linx_6.0.100_aarch64/source.list
--rw-r-----  2.0 unx     8000 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Linx_6_aarch64/pkg_info.json
--rw-r-----  2.0 unx      129 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Linx_6_aarch64/source.list
--rw-r-----  2.0 unx    51454 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
--rw-r-----  2.0 unx     2549 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
--rw-r-----  2.0 unx      182 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
--rw-r-----  2.0 unx    51932 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
--rw-r-----  2.0 unx     2209 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
--rw-r-----  2.0 unx      180 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
--rw-r--r--  2.0 unx    51351 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
--rw-r--r--  2.0 unx     2424 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
--rw-r--r--  2.0 unx      182 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
--rw-r--r--  2.0 unx    43010 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
--rw-r--r--  2.0 unx     2422 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
--rw-r--r--  2.0 unx      180 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
--rw-r-----  2.0 unx     7930 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Tlinux_2.4_aarch64/pkg_info.json
--rw-r-----  2.0 unx      587 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Tlinux_2.4_aarch64/source.repo
--rw-r-----  2.0 unx     8101 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Tlinux_2.4_x86_64/pkg_info.json
--rw-r-----  2.0 unx      473 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Tlinux_2.4_x86_64/source.repo
--rw-r-----  2.0 unx    57488 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
--rw-r-----  2.0 unx     2460 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
--rw-r-----  2.0 unx      186 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
--rw-r-----  2.0 unx    57488 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1021e_aarch64/installed.txt
--rw-r-----  2.0 unx     2460 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1021e_aarch64/pkg_info.json
--rw-r-----  2.0 unx      186 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20-1021e_aarch64/source.repo
--rw-r-----  2.0 unx     4884 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20SP1_aarch64/pkg_info.json
--rw-r-----  2.0 unx      131 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20SP1_aarch64/source.list
--rw-r-----  2.0 unx     4610 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20SP1_x86_64/pkg_info.json
--rw-r-----  2.0 unx      131 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20SP1_x86_64/source.list
--rw-r-----  2.0 unx     4884 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20_aarch64/pkg_info.json
--rw-r-----  2.0 unx      131 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20_aarch64/source.list
--rw-r-----  2.0 unx     4610 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20_x86_64/pkg_info.json
--rw-r-----  2.0 unx      131 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/UOS_20_x86_64/source.list
--rw-r-----  2.0 unx     4177 b- defN 22-Dec-07 12:08 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
--rw-r-----  2.0 unx      370 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
--rw-r-----  2.0 unx     5004 b- defN 22-Dec-07 12:09 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
--rw-r-----  2.0 unx      352 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
--rw-r-----  2.0 unx     5145 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
--rw-r-----  2.0 unx      366 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
--rw-r-----  2.0 unx     5563 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
--rw-r-----  2.0 unx      348 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
--rw-r--r--  2.0 unx     5864 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
--rw-r--r--  2.0 unx      366 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
--rw-r--r--  2.0 unx     5604 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
--rw-r--r--  2.0 unx      348 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
--rw-r-----  2.0 unx     5041 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/software/CANN_5.0.4.json
--rw-r-----  2.0 unx     3983 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/software/CANN_5.1.RC1.1.json
--rw-r--r--  2.0 unx     5626 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/software/CANN_5.1.RC2.json
--rw-r--r--  2.0 unx     5201 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/software/CANN_6.0.1.json
--rw-r--r--  2.0 unx     5525 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/software/CANN_6.0.RC1.json
--rw-r--r--  2.0 unx     5340 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.10.0.json
--rw-r--r--  2.0 unx     3660 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.5.0.json
--rw-r--r--  2.0 unx     3660 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.6.2.json
--rw-r--r--  2.0 unx     5304 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.7.0.json
--rw-r--r--  2.0 unx     5304 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.8.0.json
--rw-r--r--  2.0 unx     5304 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindSpore_1.9.0.json
--rw-r-----  2.0 unx    26018 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/software/MindStudio_3.0.3.json
--rw-r-----  2.0 unx    26018 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/software/MindStudio_3.0.4.json
--rw-r--r--  2.0 unx    48360 b- defN 23-Mar-31 08:24 ascend_deployer/downloader/software/MindStudio_5.0.0.json
--rw-r-----  2.0 unx    25492 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/software/MindStudio_5.0.RC1.json
--rw-r--r--  2.0 unx    25492 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/software/MindStudio_5.0.RC2.json
--rw-r--r--  2.0 unx    25492 b- defN 23-Mar-31 08:19 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
--rw-r-----  2.0 unx        0 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/yum_metadata/__init__.py
--rw-r-----  2.0 unx     1772 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
--rw-r-----  2.0 unx    11322 b- defN 22-Oct-29 06:06 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
--rw-r-----  2.0 unx      140 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/yum_metadata/__pycache__/__init__.cpython-36.pyc
--rw-r-----  2.0 unx     9172 b- defN 22-Dec-07 12:01 ascend_deployer/downloader/yum_metadata/__pycache__/gen_yum_metadata.cpython-36.pyc
--rw-r--r--  2.0 unx     1136 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/create_user.yml
--rw-r-----  2.0 unx      835 b- defN 22-Nov-18 08:44 ascend_deployer/playbooks/distribution.yml
--rw-r-----  2.0 unx     1061 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/gather_app_info.yml
--rw-r--r--  2.0 unx      938 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/gather_npu_fact.yml
--rw-r-----  2.0 unx      491 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/modify_user_group.yml
--rw-r--r--  2.0 unx     1311 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/os_map.yml
--rw-r-----  2.0 unx     1073 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
--rw-r-----  2.0 unx     1073 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
--rw-r--r--  2.0 unx     1076 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
--rw-r--r--  2.0 unx     1076 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
--rw-r-----  2.0 unx      139 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/set_facts_cache_permission.yml
--rw-r-----  2.0 unx     4459 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/task_set_custom_fact.yml
--rw-r-----  2.0 unx     6621 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/facts/app_info.fact.j2
--rw-r--r--  2.0 unx    10259 b- defN 23-Apr-08 02:22 ascend_deployer/playbooks/facts/npu_info.fact.j2
--rw-r-----  2.0 unx      409 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_atlasedge.yml
--rw-r-----  2.0 unx      323 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_docker_images.yml
--rw-r--r--  2.0 unx     1128 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/install_driver.yml
--rw-r-----  2.0 unx     1151 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_firmware.yml
--rw-r-----  2.0 unx      888 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_gcc.yml
--rw-r-----  2.0 unx      388 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_ha.yml
--rw-r-----  2.0 unx      293 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_ief.yml
--rw-r-----  2.0 unx      216 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_kernels.yml
--rw-r--r--  2.0 unx     1223 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/install_mindspore.yml
--rw-r--r--  2.0 unx     9015 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/install_mindstudio.yml
--rw-r-----  2.0 unx       96 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_nnae.yml
--rw-r-----  2.0 unx      210 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_nnrt.yml
--rw-r--r--  2.0 unx     1398 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/install_npu.yml
--rw-r-----  2.0 unx      108 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_python375.yml
--rw-r-----  2.0 unx     2499 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_pytorch.yml
--rw-r-----  2.0 unx      313 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_sys_pkg.yml
--rw-r-----  2.0 unx     3007 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_tensorflow.yml
--rw-r-----  2.0 unx      104 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_tfplugin.yml
--rw-r-----  2.0 unx      102 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_toolbox.yml
--rw-r-----  2.0 unx      216 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/install_toolkit.yml
--rw-r-----  2.0 unx     1263 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_atlasedge.yml
--rw-r-----  2.0 unx      663 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_cmake.yml
--rw-r-----  2.0 unx      810 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_docker_images.yml
--rw-r-----  2.0 unx      239 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_driver.yml
--rw-r--r--  2.0 unx     5640 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_driver_bcinux.yml
--rw-r--r--  2.0 unx     5723 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_driver_common.yml
--rw-r--r--  2.0 unx     4840 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_firmware.yml
--rw-r--r--  2.0 unx     2210 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_gcc.yml
--rw-r--r--  2.0 unx     3055 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_get_npu_scene.yml
--rw-r-----  2.0 unx     1056 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_ha.yml
--rw-r-----  2.0 unx      662 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_ief.yml
--rw-r-----  2.0 unx     2777 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_ief_a500.yml
--rw-r-----  2.0 unx     1665 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_ief_a500pro.yml
--rw-r-----  2.0 unx     1395 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_kernel.yml
--rw-r--r--  2.0 unx     1317 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_kernel_euleros.yml
--rw-r--r--  2.0 unx     3933 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_kernels.yml
--rw-r--r--  2.0 unx     2805 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_mindspore.yml
--rw-r--r--  2.0 unx     3270 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_nnae.yml
--rw-r--r--  2.0 unx     2992 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_nnrt.yml
--rw-r-----  2.0 unx      709 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_protobuf.yml
--rw-r-----  2.0 unx     3209 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_python375.yml
--rw-r-----  2.0 unx     1265 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_pytorch.yml
--rw-r-----  2.0 unx      785 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_sys_apt.yml
--rw-r-----  2.0 unx      496 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_sys_dnf.yml
--rw-r--r--  2.0 unx     1226 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_sys_pkg.yml
--rw-r-----  2.0 unx      456 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_sys_yum.yml
--rw-r-----  2.0 unx     1556 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/task_tensorflow.yml
--rw-r--r--  2.0 unx     3449 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_tfplugin.yml
--rw-r--r--  2.0 unx     3298 b- defN 23-Mar-31 08:19 ascend_deployer/playbooks/install/task_toolbox.yml
--rw-r--r--  2.0 unx     6307 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/install/task_toolkit.yml
--rw-r-----  2.0 unx      102 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/install_nnae.yml
--rw-r-----  2.0 unx      219 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/install_nnrt.yml
--rw-r-----  2.0 unx      110 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
--rw-r-----  2.0 unx      225 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/install_toolkit.yml
--rw-r-----  2.0 unx      106 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
--rw-r-----  2.0 unx      106 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
--rw-r-----  2.0 unx      114 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
--rw-r-----  2.0 unx      112 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
--rw-r-----  2.0 unx     1255 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_nnae.yml
--rw-r-----  2.0 unx     1255 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_nnrt.yml
--rw-r-----  2.0 unx      555 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
--rw-r-----  2.0 unx     1468 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
--rw-r-----  2.0 unx      606 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
--rw-r-----  2.0 unx     1563 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
--rw-r-----  2.0 unx     1310 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_tfplugin.yml
--rw-r-----  2.0 unx     1303 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/install/patch/task_toolkit.yml
--rw-r-----  2.0 unx      963 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_auto.yml
--rw-r-----  2.0 unx      259 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_edge.yml
--rw-r-----  2.0 unx      442 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_mindspore.yml
--rw-r-----  2.0 unx      363 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_offline_dev.yml
--rw-r-----  2.0 unx      357 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_offline_run.yml
--rw-r-----  2.0 unx      438 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
--rw-r-----  2.0 unx      432 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
--rw-r-----  2.0 unx      521 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
--rw-r-----  2.0 unx      515 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
--rw-r-----  2.0 unx      273 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/scene/scene_vmhost.yml
--rw-r-----  2.0 unx     2180 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/case_driver.yml
--rw-r-----  2.0 unx      567 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/case_firmware.yml
--rw-r-----  2.0 unx     4679 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/case_mindspore.yml
--rw-r--r--  2.0 unx     1466 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/case_nnae.yml
--rw-r--r--  2.0 unx     1466 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/case_nnrt.yml
--rw-r-----  2.0 unx     3095 b- defN 22-Nov-18 08:44 ascend_deployer/playbooks/test/case_pytorch.yml
--rw-r-----  2.0 unx     6827 b- defN 22-Nov-18 08:44 ascend_deployer/playbooks/test/case_tensorflow.yml
--rw-r--r--  2.0 unx     1514 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/case_tfplugin.yml
--rw-r-----  2.0 unx     1149 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/case_toolbox.yml
--rw-r--r--  2.0 unx     1509 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/case_toolkit.yml
--rw-r--r--  2.0 unx      608 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/test_all.yml
--rw-r-----  2.0 unx      284 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_driver.yml
--rw-r-----  2.0 unx      284 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_firmware.yml
--rw-r-----  2.0 unx       99 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_mindspore.yml
--rw-r--r--  2.0 unx       90 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/test_nnae.yml
--rw-r--r--  2.0 unx       89 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/test_nnrt.yml
--rw-r-----  2.0 unx       96 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_pytorch.yml
--rw-r-----  2.0 unx      101 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_tensorflow.yml
--rw-r--r--  2.0 unx       97 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/test_tfplugin.yml
--rw-r-----  2.0 unx      104 b- defN 22-Oct-29 06:06 ascend_deployer/playbooks/test/test_toolbox.yml
--rw-r--r--  2.0 unx       95 b- defN 23-Mar-31 08:24 ascend_deployer/playbooks/test/test_toolkit.yml
--rwxr-x---  2.0 unx    10900 b- defN 22-Oct-29 06:06 ascend_deployer/tools/DeviceIP-conf.sh
--rwxr-xr-x  2.0 unx     1409 b- defN 22-Dec-07 12:00 ascend_deployer/tools/ascend-deployer
--rw-r--r--  2.0 unx     9930 b- defN 22-Dec-07 12:00 ascend_deployer/tools/update_crl.sh
--rwxr-xr-x  2.0 unx     1409 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.data/scripts/ascend-deployer
--rw-r--r--  2.0 unx     4131 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx       80 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      789 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/WHEEL
--rw-r--r--  2.0 unx     4575 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx    29665 b- defN 23-Apr-08 02:25 ascend_deployer-5.0.0b3.dist-info/RECORD
-262 files, 1645347 bytes uncompressed, 320039 bytes compressed:  80.5%
+Zip file size: 473028 bytes, number of entries: 400
+-rw-r--r--  2.0 unx      797 b- defN 23-Jun-10 09:54 ascend_deployer/Inventory_Template.CSV
+-rw-------  2.0 unx      769 b- defN 23-Jun-10 09:54 ascend_deployer/__init__.py
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-10 09:54 ascend_deployer/ansible.cfg
+-rw-------  2.0 unx     6434 b- defN 23-Jun-10 09:54 ascend_deployer/ascend_deployer.py
+-rw-------  2.0 unx     2076 b- defN 23-Jun-10 09:54 ascend_deployer/ascend_download.py
+-rw-------  2.0 unx     5986 b- defN 23-Jun-10 09:54 ascend_deployer/downloader_ui.py
+-rwxr-x---  2.0 unx    16597 b- defN 23-Jun-10 09:54 ascend_deployer/install.sh
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-10 09:54 ascend_deployer/inventory_file
+-rw-------  2.0 unx     3379 b- defN 23-Jun-10 09:54 ascend_deployer/jobs.py
+-rwxr-x---  2.0 unx     3367 b- defN 23-Jun-10 09:54 ascend_deployer/start_download.sh
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-10 09:54 ascend_deployer/start_download_ui.bat
+-rw-------  2.0 unx     4507 b- defN 23-Jun-10 09:54 ascend_deployer/utils.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-10 09:54 ascend_deployer/version.json
+-rw-r--r--  2.0 unx    13617 b- defN 23-Jun-10 09:54 ascend_deployer/ansible_plugin/ansible_log.py
+-rw-r--r--  2.0 unx     1123 b- defN 23-Jun-10 09:54 ascend_deployer/ansible_plugin/install_info.yaml
+-rw-r--r--  2.0 unx     2218 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/__init__.py
+-rw-r--r--  2.0 unx      137 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config.ini
+-rw-r--r--  2.0 unx    11014 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/deb_downloader.py
+-rw-r--r--  2.0 unx     3811 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dl_mef_dependency_downloader.py
+-rw-r--r--  2.0 unx    17797 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/download_util.py
+-rw-r--r--  2.0 unx    15709 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/downloader.py
+-rw-r--r--  2.0 unx     4552 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/logger_config.py
+-rw-r--r--  2.0 unx     2730 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/obs_resources.json
+-rw-r--r--  2.0 unx     4562 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/os_dep_downloader.py
+-rw-r--r--  2.0 unx    14390 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/other_downloader.py
+-rw-r--r--  2.0 unx     2870 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/other_resources.json
+-rw-r--r--  2.0 unx    13377 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/pip_downloader.py
+-rw-r--r--  2.0 unx     8754 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/python_version.json
+-rw-r--r--  2.0 unx     1775 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/requirements.txt
+-rw-r--r--  2.0 unx    20876 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/rpm_downloader.py
+-rw-r--r--  2.0 unx     8430 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software_mgr.py
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/support_url.json
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/version_match.json
+-rw-r--r--  2.0 unx     8690 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
+-rw-r--r--  2.0 unx    10223 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      371 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
+-rw-r--r--  2.0 unx    43257 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
+-rw-r--r--  2.0 unx     4596 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
+-rw-r--r--  2.0 unx    42707 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
+-rw-r--r--  2.0 unx     3668 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
+-rw-r--r--  2.0 unx    65900 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
+-rw-r--r--  2.0 unx     6028 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo
+-rw-r--r--  2.0 unx    42840 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      130 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo
+-rw-r--r--  2.0 unx    42208 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt
+-rw-r--r--  2.0 unx     3827 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx       65 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo
+-rw-r--r--  2.0 unx    60396 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt
+-rw-r--r--  2.0 unx     2490 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo
+-rw-r--r--  2.0 unx    60964 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt
+-rw-r--r--  2.0 unx     2156 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      180 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
+-rw-r--r--  2.0 unx    51454 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
+-rw-r--r--  2.0 unx     2549 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      182 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
+-rw-r--r--  2.0 unx    51932 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt
+-rw-r--r--  2.0 unx     3651 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo
+-rw-r--r--  2.0 unx    51351 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt
+-rw-r--r--  2.0 unx     5439 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      458 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo
+-rw-r--r--  2.0 unx    43010 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt
+-rw-r--r--  2.0 unx     3220 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
+-rw-r--r--  2.0 unx    57488 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
+-rw-r--r--  2.0 unx     2460 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      186 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
+-rw-r--r--  2.0 unx     4177 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      370 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
+-rw-r--r--  2.0 unx     5691 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
+-rw-r--r--  2.0 unx     5145 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
+-rw-r--r--  2.0 unx     6229 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
+-rw-r--r--  2.0 unx     5864 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
+-rw-r--r--  2.0 unx     6617 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
+-rw-r--r--  2.0 unx      348 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
+-rw-r--r--  2.0 unx     3336 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
+-rw-r--r--  2.0 unx     3344 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json
+-rw-r--r--  2.0 unx     3328 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json
+-rw-r--r--  2.0 unx     3424 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
+-rw-r--r--  2.0 unx     3408 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
+-rw-r--r--  2.0 unx     3424 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
+-rw-r--r--  2.0 unx     3408 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
+-rw-r--r--  2.0 unx     3368 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
+-rw-r--r--  2.0 unx     3368 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
+-rw-r--r--  2.0 unx     3368 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
+-rw-r--r--  2.0 unx     3352 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
+-rw-r--r--  2.0 unx     2948 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
+-rw-r--r--  2.0 unx     2920 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
+-rw-r--r--  2.0 unx      853 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
+-rw-r--r--  2.0 unx     5822 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/CANN_6.0.1.json
+-rw-r--r--  2.0 unx     5438 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/CANN_6.0.RC1.json
+-rw-r--r--  2.0 unx     5287 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/CANN_6.3.RC1.json
+-rw-r--r--  2.0 unx       84 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/DL_5.0.RC1.json
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MEF_5.0.RC1.json
+-rw-r--r--  2.0 unx     5341 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.10.0.json
+-rw-r--r--  2.0 unx     3660 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.5.0.json
+-rw-r--r--  2.0 unx     3660 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.6.2.json
+-rw-r--r--  2.0 unx     5304 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.7.0.json
+-rw-r--r--  2.0 unx     5304 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.8.0.json
+-rw-r--r--  2.0 unx     5304 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_1.9.0.json
+-rw-r--r--  2.0 unx     5360 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
+-rw-r--r--  2.0 unx    26018 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_3.0.3.json
+-rw-r--r--  2.0 unx    26018 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_3.0.4.json
+-rw-r--r--  2.0 unx    48361 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_5.0.0.json
+-rw-r--r--  2.0 unx    25492 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_5.0.RC1.json
+-rw-r--r--  2.0 unx    25492 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_5.0.RC2.json
+-rw-r--r--  2.0 unx    25492 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
+-rw-r--r--  2.0 unx    48368 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
+-rw-r--r--  2.0 unx     2890 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/Torch-npu_1.11.0.json
+-rw-r--r--  2.0 unx     2906 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
+-rw-r--r--  2.0 unx     2895 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/Torch-npu_1.8.1.json
+-rw-r--r--  2.0 unx     2920 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/yum_metadata/__init__.py
+-rw-r--r--  2.0 unx     1772 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
+-rw-r--r--  2.0 unx    11330 b- defN 23-Jun-10 09:54 ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
+-rw-r--r--  2.0 unx     1572 b- defN 23-Jun-10 09:54 ascend_deployer/group_vars/all.yaml
+-rw-r--r--  2.0 unx      807 b- defN 23-Jun-10 09:54 ascend_deployer/patch/selenium_firefox.patch
+-rw-r--r--  2.0 unx     1127 b- defN 23-Jun-10 09:54 ascend_deployer/patch/selenium_firefox_profile.patch
+-rw-r--r--  2.0 unx      236 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/basic.yaml
+-rw-r--r--  2.0 unx      479 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/check.yaml
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/check_pkgs.yml
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/create_user.yml
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/distribution.yml
+-rw-r--r--  2.0 unx      672 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/docker.yaml
+-rw-r--r--  2.0 unx     1021 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/gather_app_info.yml
+-rw-r--r--  2.0 unx     3487 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/gather_facts.yaml
+-rw-r--r--  2.0 unx     1162 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/gather_npu_fact.yml
+-rw-r--r--  2.0 unx      121 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/harbor.yaml
+-rw-r--r--  2.0 unx      122 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/hccn.yaml
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/image_load.yaml
+-rw-r--r--  2.0 unx     2213 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/k8s.yaml
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/kubeedge.yaml
+-rw-r--r--  2.0 unx     1654 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/mindxdl.yaml
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/modify_user_group.yml
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/os_map.yaml
+-rw-r--r--  2.0 unx     2065 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/os_map.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
+-rw-r--r--  2.0 unx     1076 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/report.yaml
+-rw-r--r--  2.0 unx      139 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/set_facts_cache_permission.yml
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/sync_time.yml
+-rw-r--r--  2.0 unx     6051 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/task_set_custom_fact.yml
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/uninstall_mef_releate.yaml
+-rw-r--r--  2.0 unx     5199 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/facts/app_info.fact.j2
+-rw-r--r--  2.0 unx     6149 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/facts/npu_info.fact.j2
+-rw-r--r--  2.0 unx      409 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_atlasedge.yml
+-rw-r--r--  2.0 unx      323 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_docker_images.yml
+-rw-r--r--  2.0 unx     1128 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_driver.yml
+-rw-r--r--  2.0 unx     1151 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_firmware.yml
+-rw-r--r--  2.0 unx      888 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_gcc.yml
+-rw-r--r--  2.0 unx      388 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_ha.yml
+-rw-r--r--  2.0 unx      293 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_ief.yml
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_kernels.yml
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_mindspore.yml
+-rw-r--r--  2.0 unx     9015 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_mindstudio.yml
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_nnae.yml
+-rw-r--r--  2.0 unx      210 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_nnrt.yml
+-rw-r--r--  2.0 unx     1398 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_npu.yml
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_python.yml
+-rw-r--r--  2.0 unx     2499 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_pytorch.yml
+-rw-r--r--  2.0 unx      313 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_sys_pkg.yml
+-rw-r--r--  2.0 unx     3007 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_tensorflow.yml
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_tfplugin.yml
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_toolbox.yml
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/install_toolkit.yml
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_atlasedge.yml
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_cmake.yml
+-rw-r--r--  2.0 unx      769 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_dl.yml
+-rw-r--r--  2.0 unx      810 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_docker_images.yml
+-rw-r--r--  2.0 unx      239 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_driver.yml
+-rw-r--r--  2.0 unx     6047 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_driver_bcinux.yml
+-rw-r--r--  2.0 unx     6130 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_driver_common.yml
+-rw-r--r--  2.0 unx     5295 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_firmware.yml
+-rw-r--r--  2.0 unx     2210 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_gcc.yml
+-rw-r--r--  2.0 unx     3055 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_get_npu_scene.yml
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_ha.yml
+-rw-r--r--  2.0 unx      662 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_ief.yml
+-rw-r--r--  2.0 unx     2777 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_ief_a500.yml
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_ief_a500pro.yml
+-rw-r--r--  2.0 unx     1395 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_kernel.yml
+-rw-r--r--  2.0 unx     1317 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_kernel_euleros.yml
+-rw-r--r--  2.0 unx     6030 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_kernels.yml
+-rw-r--r--  2.0 unx     1879 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_mindspore.yml
+-rw-r--r--  2.0 unx     3270 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_nnae.yml
+-rw-r--r--  2.0 unx     2992 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_nnrt.yml
+-rw-r--r--  2.0 unx      709 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_protobuf.yml
+-rw-r--r--  2.0 unx     3209 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_python.yml
+-rw-r--r--  2.0 unx     1265 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_pytorch.yml
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_sys_apt.yml
+-rw-r--r--  2.0 unx     1794 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_sys_dnf.yml
+-rw-r--r--  2.0 unx     3230 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_sys_pkg.yml
+-rw-r--r--  2.0 unx     1798 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_sys_yum.yml
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_tensorflow.yml
+-rw-r--r--  2.0 unx     3449 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_tfplugin.yml
+-rw-r--r--  2.0 unx     3298 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_toolbox.yml
+-rw-r--r--  2.0 unx     6307 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/task_toolkit.yml
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/install_nnae.yml
+-rw-r--r--  2.0 unx      219 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/install_nnrt.yml
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/install_tfplugin.yml
+-rw-r--r--  2.0 unx      225 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/install_toolkit.yml
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/rollback_nnae.yml
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/rollback_nnrt.yml
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/rollback_tfplugin.yml
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/rollback_toolkit.yml
+-rw-r--r--  2.0 unx     1255 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_nnae.yml
+-rw-r--r--  2.0 unx     1255 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_nnrt.yml
+-rw-r--r--  2.0 unx      555 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml
+-rw-r--r--  2.0 unx     1468 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml
+-rw-r--r--  2.0 unx      606 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml
+-rw-r--r--  2.0 unx     1563 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml
+-rw-r--r--  2.0 unx     1310 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_tfplugin.yml
+-rw-r--r--  2.0 unx     1303 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/install/patch/task_toolkit.yml
+-rw-r--r--  2.0 unx      369 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_check.yml
+-rw-r--r--  2.0 unx     2169 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_install.yml
+-rw-r--r--  2.0 unx      711 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_patch.yml
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_patch_rollback.yml
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_scene.yml
+-rw-r--r--  2.0 unx      967 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/process/process_test.yml
+-rw-r--r--  2.0 unx      310 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
+-rw-r--r--  2.0 unx     1258 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
+-rw-r--r--  2.0 unx     4146 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
+-rw-r--r--  2.0 unx     1437 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
+-rw-r--r--  2.0 unx     4504 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
+-rw-r--r--  2.0 unx     4892 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
+-rw-r--r--  2.0 unx    10079 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
+-rw-r--r--  2.0 unx      341 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/README.md
+-rw-r--r--  2.0 unx     1296 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
+-rw-r--r--  2.0 unx      181 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
+-rw-r--r--  2.0 unx     9911 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
+-rw-r--r--  2.0 unx      675 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
+-rw-r--r--  2.0 unx    12803 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
+-rw-r--r--  2.0 unx     7226 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
+-rw-r--r--  2.0 unx      646 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
+-rw-r--r--  2.0 unx     1517 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
+-rw-r--r--  2.0 unx     5651 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
+-rw-r--r--  2.0 unx     5906 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
+-rw-r--r--  2.0 unx     5550 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
+-rw-r--r--  2.0 unx     4386 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
+-rw-r--r--  2.0 unx     7418 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
+-rw-r--r--  2.0 unx       67 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/README.md
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
+-rw-r--r--  2.0 unx      500 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
+-rw-r--r--  2.0 unx      418 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
+-rw-r--r--  2.0 unx      892 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
+-rw-r--r--  2.0 unx     1160 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
+-rw-r--r--  2.0 unx     1314 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
+-rw-r--r--  2.0 unx     1158 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
+-rw-r--r--  2.0 unx      346 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
+-rw-r--r--  2.0 unx     1157 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
+-rw-r--r--  2.0 unx       42 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
+-rw-r--r--  2.0 unx     1707 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
+-rw-r--r--  2.0 unx      536 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/README.md
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
+-rw-r--r--  2.0 unx      929 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
+-rw-r--r--  2.0 unx     1169 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
+-rw-r--r--  2.0 unx      417 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml
+-rw-r--r--  2.0 unx      869 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
+-rw-r--r--  2.0 unx     1401 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
+-rw-r--r--  2.0 unx      897 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
+-rw-r--r--  2.0 unx     4442 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
+-rw-r--r--  2.0 unx     1797 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
+-rw-r--r--  2.0 unx     3518 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
+-rw-r--r--  2.0 unx     1596 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
+-rw-r--r--  2.0 unx   202740 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
+-rw-r--r--  2.0 unx       37 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
+-rw-r--r--  2.0 unx      485 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
+-rw-r--r--  2.0 unx       78 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
+-rw-r--r--  2.0 unx     3498 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
+-rw-r--r--  2.0 unx     1896 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
+-rw-r--r--  2.0 unx     8715 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
+-rw-r--r--  2.0 unx    10576 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
+-rw-r--r--  2.0 unx     1877 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
+-rw-r--r--  2.0 unx     2443 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
+-rw-r--r--  2.0 unx     1355 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
+-rw-r--r--  2.0 unx      176 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
+-rw-r--r--  2.0 unx     5145 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
+-rw-r--r--  2.0 unx      144 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
+-rw-r--r--  2.0 unx      528 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
+-rw-r--r--  2.0 unx     1732 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
+-rw-r--r--  2.0 unx     6312 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
+-rw-r--r--  2.0 unx     1011 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
+-rw-r--r--  2.0 unx      786 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
+-rw-r--r--  2.0 unx     1666 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
+-rw-r--r--  2.0 unx      389 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
+-rw-r--r--  2.0 unx      960 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_auto.yml
+-rw-r--r--  2.0 unx      660 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_dl.yml
+-rw-r--r--  2.0 unx      259 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_edge.yml
+-rw-r--r--  2.0 unx      491 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_mef.yml
+-rw-r--r--  2.0 unx      514 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_mindspore.yml
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_offline_dev.yml
+-rw-r--r--  2.0 unx      354 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_offline_run.yml
+-rw-r--r--  2.0 unx      510 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_pytorch_dev.yml
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_pytorch_run.yml
+-rw-r--r--  2.0 unx      593 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml
+-rw-r--r--  2.0 unx      587 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_tensorflow_run.yml
+-rw-r--r--  2.0 unx      273 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/scene/scene_vmhost.yml
+-rw-r--r--  2.0 unx     2180 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_driver.yml
+-rw-r--r--  2.0 unx      567 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_firmware.yml
+-rw-r--r--  2.0 unx     4679 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_mindspore.yml
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_nnae.yml
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_nnrt.yml
+-rw-r--r--  2.0 unx     3095 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_pytorch.yml
+-rw-r--r--  2.0 unx     6827 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_tensorflow.yml
+-rw-r--r--  2.0 unx     1514 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_tfplugin.yml
+-rw-r--r--  2.0 unx     1149 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_toolbox.yml
+-rw-r--r--  2.0 unx     1509 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/case_toolkit.yml
+-rw-r--r--  2.0 unx      608 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_all.yml
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_driver.yml
+-rw-r--r--  2.0 unx      284 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_firmware.yml
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_mindspore.yml
+-rw-r--r--  2.0 unx       90 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_nnae.yml
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_nnrt.yml
+-rw-r--r--  2.0 unx       96 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_pytorch.yml
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_tensorflow.yml
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_tfplugin.yml
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_toolbox.yml
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-10 09:54 ascend_deployer/playbooks/test/test_toolkit.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/__init__.py
+-rw-r--r--  2.0 unx    19112 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/ascend_deploy.py
+-rw-r--r--  2.0 unx      870 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/backup.sh
+-rw-r--r--  2.0 unx      368 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/check.sh
+-rw-r--r--  2.0 unx    20699 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/check_pkgs.sh
+-rw-r--r--  2.0 unx      249 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/hccn_set.sh
+-rw-r--r--  2.0 unx     1142 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/image_load.sh
+-rw-r--r--  2.0 unx      969 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/install.sh
+-rw-r--r--  2.0 unx     3587 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/install_ansible.sh
+-rw-r--r--  2.0 unx      272 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/install_kubeedge.sh
+-rw-r--r--  2.0 unx      248 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/machine_report.sh
+-rw-r--r--  2.0 unx    14207 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/nexus.py
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/nexus_config.json
+-rw-r--r--  2.0 unx      535 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/uninstall_k8s_docker.sh
+-rw-r--r--  2.0 unx      643 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/uninstall_mef_kubeedge.sh
+-rw-r--r--  2.0 unx      679 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/uninstall_mef_related.sh
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/upgrade.sh
+-rw-r--r--  2.0 unx     5723 b- defN 23-Jun-10 09:54 ascend_deployer/scripts/utils.sh
+-rw-r--r--  2.0 unx    10900 b- defN 23-Jun-10 09:54 ascend_deployer/tools/DeviceIP-conf.sh
+-rw-r--r--  2.0 unx     1409 b- defN 23-Jun-10 09:54 ascend_deployer/tools/ascend-deployer
+-rw-r--r--  2.0 unx     4049 b- defN 23-Jun-10 09:54 ascend_deployer/tools/check.py
+-rw-r--r--  2.0 unx     7085 b- defN 23-Jun-10 09:54 ascend_deployer/tools/hccn.py
+-rw-r--r--  2.0 unx     9930 b- defN 23-Jun-10 09:54 ascend_deployer/tools/update_crl.sh
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-10 09:54 ascend_deployer/tools/hccn/main/go.mod
+-rw-r--r--  2.0 unx     6863 b- defN 23-Jun-10 09:54 ascend_deployer/tools/hccn/main/hccn.go
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-10 09:54 ascend_deployer/tools/report/main/go.mod
+-rw-r--r--  2.0 unx    18729 b- defN 23-Jun-10 09:54 ascend_deployer/tools/report/main/main.go
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-10 09:54 ascend_deployer/tools/unzip/main/go.mod
+-rw-r--r--  2.0 unx     1587 b- defN 23-Jun-10 09:54 ascend_deployer/tools/unzip/main/unzip.go
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/basic.yaml
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/check.yaml
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/docker.yaml
+-rw-r--r--  2.0 unx       53 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/gather_facts.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/harbor.yaml
+-rw-r--r--  2.0 unx       45 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/hccn.yaml
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/image_load.yaml
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/k8s.yaml
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/k8s_reset.yaml
+-rw-r--r--  2.0 unx       74 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/mindxdl.yaml
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-10 09:54 ascend_deployer/yamls/report.yaml
+-rwxr-xr-x  2.0 unx     1409 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.data/scripts/ascend-deployer
+-rw-------  2.0 unx     4131 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/DESCRIPTION.rst
+-rw-------  2.0 unx       74 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/entry_points.txt
+-rw-------  2.0 unx      777 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/metadata.json
+-rw-------  2.0 unx       16 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/top_level.txt
+-rw-------  2.0 unx       92 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/WHEEL
+-rw-------  2.0 unx     4575 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/METADATA
+-rw-------  2.0 unx    44959 b- defN 23-Jun-10 09:56 ascend_deployer-5.0.0b4.dist-info/RECORD
+400 files, 2022988 bytes uncompressed, 398618 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -1,56 +1,74 @@
-Filename: ascend_deployer/LICENSE
+Filename: ascend_deployer/Inventory_Template.CSV
 Comment: 
 
-Filename: ascend_deployer/README.en.rst
+Filename: ascend_deployer/__init__.py
 Comment: 
 
-Filename: ascend_deployer/README.rst
+Filename: ascend_deployer/ansible.cfg
 Comment: 
 
-Filename: ascend_deployer/__init__.py
+Filename: ascend_deployer/ascend_deployer.py
 Comment: 
 
-Filename: ascend_deployer/ansible.cfg
+Filename: ascend_deployer/ascend_download.py
+Comment: 
+
+Filename: ascend_deployer/downloader_ui.py
 Comment: 
 
 Filename: ascend_deployer/install.sh
 Comment: 
 
 Filename: ascend_deployer/inventory_file
 Comment: 
 
-Filename: ascend_deployer/start_download.bat
+Filename: ascend_deployer/jobs.py
 Comment: 
 
 Filename: ascend_deployer/start_download.sh
 Comment: 
 
 Filename: ascend_deployer/start_download_ui.bat
 Comment: 
 
+Filename: ascend_deployer/utils.py
+Comment: 
+
+Filename: ascend_deployer/version.json
+Comment: 
+
+Filename: ascend_deployer/ansible_plugin/ansible_log.py
+Comment: 
+
+Filename: ascend_deployer/ansible_plugin/install_info.yaml
+Comment: 
+
 Filename: ascend_deployer/downloader/__init__.py
 Comment: 
 
 Filename: ascend_deployer/downloader/config.ini
 Comment: 
 
 Filename: ascend_deployer/downloader/deb_downloader.py
 Comment: 
 
+Filename: ascend_deployer/downloader/dl_mef_dependency_downloader.py
+Comment: 
+
 Filename: ascend_deployer/downloader/download_util.py
 Comment: 
 
 Filename: ascend_deployer/downloader/downloader.py
 Comment: 
 
-Filename: ascend_deployer/downloader/downloader_ui.py
+Filename: ascend_deployer/downloader/logger_config.py
 Comment: 
 
-Filename: ascend_deployer/downloader/logger_config.py
+Filename: ascend_deployer/downloader/obs_resources.json
 Comment: 
 
 Filename: ascend_deployer/downloader/os_dep_downloader.py
 Comment: 
 
 Filename: ascend_deployer/downloader/other_downloader.py
 Comment: 
@@ -72,99 +90,45 @@
 
 Filename: ascend_deployer/downloader/software_mgr.py
 Comment: 
 
 Filename: ascend_deployer/downloader/support_url.json
 Comment: 
 
-Filename: ascend_deployer/downloader/__pycache__/deb_downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/download_util.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/logger_config.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/os_dep_downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/other_downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/pip_downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/rpm_downloader.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/__pycache__/software_mgr.cpython-36.pyc
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.6_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.6_aarch64/source.repo
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.6_x86_64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.6_x86_64/source.repo
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.7_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/BCLinux_7.7_aarch64/source.repo
+Filename: ascend_deployer/downloader/version_match.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/CentOS_8.2_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/CentOS_8.2_aarch64/source.repo
-Comment: 
-
-Filename: ascend_deployer/downloader/config/CentOS_8.2_x86_64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/CentOS_8.2_x86_64/source.repo
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Debian_10.0_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Debian_10.0_x86_64/source.list
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Debian_9.9_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Debian_9.9_aarch64/source.list
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Debian_9.9_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Debian_9.9_x86_64/source.list
+Filename: ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo
 Comment: 
 
 Filename: ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt
 Comment: 
 
 Filename: ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json
 Comment: 
@@ -204,32 +168,14 @@
 
 Filename: ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/source.list
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Linx_6.0.100_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Linx_6.0.100_aarch64/source.list
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Linx_6_aarch64/pkg_info.json
-Comment: 
-
-Filename: ascend_deployer/downloader/config/Linx_6_aarch64/source.list
-Comment: 
-
 Filename: ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt
 Comment: 
 
 Filename: ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo
@@ -258,119 +204,128 @@
 
 Filename: ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json
 Comment: 
 
 Filename: ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Tlinux_2.4_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Tlinux_2.4_aarch64/source.repo
+Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Tlinux_2.4_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Tlinux_2.4_x86_64/source.repo
+Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt
+Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo
+Filename: ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1021e_aarch64/installed.txt
+Filename: ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1021e_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20-1021e_aarch64/source.repo
+Filename: ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20SP1_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20SP1_aarch64/source.list
+Filename: ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20SP1_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20SP1_x86_64/source.list
+Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20_aarch64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/UOS_20_x86_64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/software/CANN_5.0.4.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/software/CANN_5.1.RC1.1.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json
 Comment: 
 
-Filename: ascend_deployer/downloader/software/CANN_5.1.RC2.json
+Filename: ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.0.1.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/CANN_6.0.RC1.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/CANN_6.3.RC1.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/DL_5.0.RC1.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/MEF_5.0.RC1.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/MindSpore_1.10.0.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindSpore_1.5.0.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindSpore_1.6.2.json
@@ -381,14 +336,17 @@
 
 Filename: ascend_deployer/downloader/software/MindSpore_1.8.0.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindSpore_1.9.0.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json
+Comment: 
+
 Filename: ascend_deployer/downloader/software/MindStudio_3.0.3.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_3.0.4.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_5.0.0.json
@@ -399,44 +357,98 @@
 
 Filename: ascend_deployer/downloader/software/MindStudio_5.0.RC2.json
 Comment: 
 
 Filename: ascend_deployer/downloader/software/MindStudio_5.0.RC3.json
 Comment: 
 
+Filename: ascend_deployer/downloader/software/MindStudio_6.0.RC1.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/Torch-npu_1.8.1.json
+Comment: 
+
+Filename: ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json
+Comment: 
+
 Filename: ascend_deployer/downloader/yum_metadata/__init__.py
 Comment: 
 
 Filename: ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql
 Comment: 
 
 Filename: ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py
 Comment: 
 
-Filename: ascend_deployer/downloader/yum_metadata/__pycache__/__init__.cpython-36.pyc
+Filename: ascend_deployer/group_vars/all.yaml
+Comment: 
+
+Filename: ascend_deployer/patch/selenium_firefox.patch
+Comment: 
+
+Filename: ascend_deployer/patch/selenium_firefox_profile.patch
+Comment: 
+
+Filename: ascend_deployer/playbooks/basic.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/check.yaml
 Comment: 
 
-Filename: ascend_deployer/downloader/yum_metadata/__pycache__/gen_yum_metadata.cpython-36.pyc
+Filename: ascend_deployer/playbooks/check_pkgs.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/create_user.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/distribution.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/docker.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/gather_app_info.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/gather_facts.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/gather_npu_fact.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/harbor.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/hccn.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/image_load.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/k8s.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/kubeedge.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/mindxdl.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/modify_user_group.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/os_map.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/os_map.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml
@@ -444,20 +456,32 @@
 
 Filename: ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/report.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/set_facts_cache_permission.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/sync_time.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/task_set_custom_fact.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/uninstall_mef_releate.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/facts/app_info.fact.j2
 Comment: 
 
 Filename: ascend_deployer/playbooks/facts/npu_info.fact.j2
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_atlasedge.yml
@@ -495,15 +519,15 @@
 
 Filename: ascend_deployer/playbooks/install/install_nnrt.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_npu.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/install_python375.yml
+Filename: ascend_deployer/playbooks/install/install_python.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_pytorch.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/install_sys_pkg.yml
 Comment: 
@@ -522,14 +546,17 @@
 
 Filename: ascend_deployer/playbooks/install/task_atlasedge.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_cmake.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/install/task_dl.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/install/task_docker_images.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_driver.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_driver_bcinux.yml
@@ -576,15 +603,15 @@
 
 Filename: ascend_deployer/playbooks/install/task_nnrt.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_protobuf.yml
 Comment: 
 
-Filename: ascend_deployer/playbooks/install/task_python375.yml
+Filename: ascend_deployer/playbooks/install/task_python.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_pytorch.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/task_sys_apt.yml
 Comment: 
@@ -654,20 +681,296 @@
 
 Filename: ascend_deployer/playbooks/install/patch/task_tfplugin.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/install/patch/task_toolkit.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/process/process_check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/process/process_install.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/process/process_patch.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/process/process_patch_rollback.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/process/process_scene.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/process/process_test.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/files/space.sh
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/README.md
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/README.md
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tests/inventory
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/README.md
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/README.md
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml
+Comment: 
+
+Filename: ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml
+Comment: 
+
 Filename: ascend_deployer/playbooks/scene/scene_auto.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/scene/scene_dl.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/scene/scene_edge.yml
 Comment: 
 
+Filename: ascend_deployer/playbooks/scene/scene_mef.yml
+Comment: 
+
 Filename: ascend_deployer/playbooks/scene/scene_mindspore.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/scene/scene_offline_dev.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/scene/scene_offline_run.yml
@@ -747,41 +1050,152 @@
 
 Filename: ascend_deployer/playbooks/test/test_toolbox.yml
 Comment: 
 
 Filename: ascend_deployer/playbooks/test/test_toolkit.yml
 Comment: 
 
+Filename: ascend_deployer/scripts/__init__.py
+Comment: 
+
+Filename: ascend_deployer/scripts/ascend_deploy.py
+Comment: 
+
+Filename: ascend_deployer/scripts/backup.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/check.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/check_pkgs.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/hccn_set.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/image_load.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/install.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/install_ansible.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/install_kubeedge.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/machine_report.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/nexus.py
+Comment: 
+
+Filename: ascend_deployer/scripts/nexus_config.json
+Comment: 
+
+Filename: ascend_deployer/scripts/uninstall_k8s_docker.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/uninstall_mef_kubeedge.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/uninstall_mef_related.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/upgrade.sh
+Comment: 
+
+Filename: ascend_deployer/scripts/utils.sh
+Comment: 
+
 Filename: ascend_deployer/tools/DeviceIP-conf.sh
 Comment: 
 
 Filename: ascend_deployer/tools/ascend-deployer
 Comment: 
 
+Filename: ascend_deployer/tools/check.py
+Comment: 
+
+Filename: ascend_deployer/tools/hccn.py
+Comment: 
+
 Filename: ascend_deployer/tools/update_crl.sh
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.data/scripts/ascend-deployer
+Filename: ascend_deployer/tools/hccn/main/go.mod
+Comment: 
+
+Filename: ascend_deployer/tools/hccn/main/hccn.go
+Comment: 
+
+Filename: ascend_deployer/tools/report/main/go.mod
+Comment: 
+
+Filename: ascend_deployer/tools/report/main/main.go
+Comment: 
+
+Filename: ascend_deployer/tools/unzip/main/go.mod
+Comment: 
+
+Filename: ascend_deployer/tools/unzip/main/unzip.go
+Comment: 
+
+Filename: ascend_deployer/yamls/basic.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/check.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/docker.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/gather_facts.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/harbor.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/hccn.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/image_load.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/k8s.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/k8s_reset.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/mindxdl.yaml
+Comment: 
+
+Filename: ascend_deployer/yamls/report.yaml
+Comment: 
+
+Filename: ascend_deployer-5.0.0b4.data/scripts/ascend-deployer
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/DESCRIPTION.rst
+Filename: ascend_deployer-5.0.0b4.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/entry_points.txt
+Filename: ascend_deployer-5.0.0b4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/metadata.json
+Filename: ascend_deployer-5.0.0b4.dist-info/metadata.json
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/top_level.txt
+Filename: ascend_deployer-5.0.0b4.dist-info/top_level.txt
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/WHEEL
+Filename: ascend_deployer-5.0.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/METADATA
+Filename: ascend_deployer-5.0.0b4.dist-info/METADATA
 Comment: 
 
-Filename: ascend_deployer-5.0.0b3.dist-info/RECORD
+Filename: ascend_deployer-5.0.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ascend_deployer/__init__.py

```diff
@@ -0,0 +1,49 @@
+00000000: 2321 2f75 7372 2f62 696e 2f65 6e76 2070  #!/usr/bin/env p
+00000010: 7974 686f 6e33 0a23 2063 6f64 696e 673a  ython3.# coding:
+00000020: 2075 7466 2d38 0a23 2043 6f70 7972 6967   utf-8.# Copyrig
+00000030: 6874 2032 3032 3320 4875 6177 6569 2054  ht 2023 Huawei T
+00000040: 6563 686e 6f6c 6f67 6965 7320 436f 2e2c  echnologies Co.,
+00000050: 204c 7464 0a23 0a23 204c 6963 656e 7365   Ltd.#.# License
+00000060: 6420 756e 6465 7220 7468 6520 4170 6163  d under the Apac
+00000070: 6865 204c 6963 656e 7365 2c20 5665 7273  he License, Vers
+00000080: 696f 6e20 322e 3020 2874 6865 2022 4c69  ion 2.0 (the "Li
+00000090: 6365 6e73 6522 293b 0a23 2079 6f75 206d  cense");.# you m
+000000a0: 6179 206e 6f74 2075 7365 2074 6869 7320  ay not use this 
+000000b0: 6669 6c65 2065 7863 6570 7420 696e 2063  file except in c
+000000c0: 6f6d 706c 6961 6e63 6520 7769 7468 2074  ompliance with t
+000000d0: 6865 204c 6963 656e 7365 2e0a 2320 596f  he License..# Yo
+000000e0: 7520 6d61 7920 6f62 7461 696e 2061 2063  u may obtain a c
+000000f0: 6f70 7920 6f66 2074 6865 204c 6963 656e  opy of the Licen
+00000100: 7365 2061 740a 230a 2320 6874 7470 3a2f  se at.#.# http:/
+00000110: 2f77 7777 2e61 7061 6368 652e 6f72 672f  /www.apache.org/
+00000120: 6c69 6365 6e73 6573 2f4c 4943 454e 5345  licenses/LICENSE
+00000130: 2d32 2e30 0a23 0a23 2055 6e6c 6573 7320  -2.0.#.# Unless 
+00000140: 7265 7175 6972 6564 2062 7920 6170 706c  required by appl
+00000150: 6963 6162 6c65 206c 6177 206f 7220 6167  icable law or ag
+00000160: 7265 6564 2074 6f20 696e 2077 7269 7469  reed to in writi
+00000170: 6e67 2c20 736f 6674 7761 7265 0a23 2064  ng, software.# d
+00000180: 6973 7472 6962 7574 6564 2075 6e64 6572  istributed under
+00000190: 2074 6865 204c 6963 656e 7365 2069 7320   the License is 
+000001a0: 6469 7374 7269 6275 7465 6420 6f6e 2061  distributed on a
+000001b0: 6e20 2241 5320 4953 2220 4241 5349 532c  n "AS IS" BASIS,
+000001c0: 0a23 2057 4954 484f 5554 2057 4152 5241  .# WITHOUT WARRA
+000001d0: 4e54 4945 5320 4f52 2043 4f4e 4449 5449  NTIES OR CONDITI
+000001e0: 4f4e 5320 4f46 2041 4e59 204b 494e 442c  ONS OF ANY KIND,
+000001f0: 2065 6974 6865 7220 6578 7072 6573 7320   either express 
+00000200: 6f72 2069 6d70 6c69 6564 2e0a 2320 5365  or implied..# Se
+00000210: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
+00000220: 7220 7468 6520 7370 6563 6966 6963 206c  r the specific l
+00000230: 616e 6775 6167 6520 676f 7665 726e 696e  anguage governin
+00000240: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
+00000250: 640a 2320 6c69 6d69 7461 7469 6f6e 7320  d.# limitations 
+00000260: 756e 6465 7220 7468 6520 4c69 6365 6e73  under the Licens
+00000270: 652e 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d  e..# ===========
+00000280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000002a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000002b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000002c0: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
+000002d0: 7420 7379 730a 7379 732e 7061 7468 2e61  t sys.sys.path.a
+000002e0: 7070 656e 6428 6f73 2e70 6174 682e 6469  ppend(os.path.di
+000002f0: 726e 616d 6528 5f5f 6669 6c65 5f5f 2929  rname(__file__))
+00000300: 0a                                       .
```

## ascend_deployer/ansible.cfg

```diff
@@ -1,15 +1,18 @@
 [defaults]
 forks=50
 command_warnings=False
-host_key_checking=True
+host_key_checking=False
+callback_plugins   = ./ansible_plugin
+bin_ansible_callbacks=True
 
 gathering=explicit
 fact_caching=jsonfile
 deprecation_warnings=False
 interpreter_python=auto_legacy_silent
+fact_caching_connection=./facts-cache
 
 [inventory]
 unparsed_is_failed=True
 
 [ssh_connection]
 scp_if_ssh=True
```

## ascend_deployer/install.sh

```diff
@@ -1,217 +1,41 @@
 #!/bin/bash
 unset LD_LIBRARY_PATH
 declare -x PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:"${ASCENDPATH}""
 readonly TRUE=1
 readonly FALSE=0
 readonly SIZE_THRESHOLD=$((5 * 1024 * 1024 * 1024))
-readonly ZIP_COUNT_THRESHOLD=3000
-readonly TAR_COUNT_THRESHOLD=100000
 readonly LOG_SIZE_THRESHOLD=$((20 * 1024 * 1024))
 readonly LOG_COUNT_THRESHOLD=5
 readonly kernel_version=$(uname -r)
 readonly arch=$(uname -m)
 readonly BASE_DIR=$(
     cd "$(dirname $0)" >/dev/null 2>&1
     pwd -P
 )
 readonly PYLIB_PATH=${BASE_DIR}/resources/pylibs
-readonly A310P_SOC_PRODUCT_LIST="Ascend-hdk-310p-npu-soc,Ascend-hdk-310p-npu-driver-soc,Ascend-hdk-310p-npu-firmware-soc"
-readonly A300I_PRODUCT_LIST="A300i-pro,Atlas-300i-pro"
-readonly A300V_PRO_PRODUCT_LIST="A300v-pro,Atlas-300v-pro"
-readonly A300V_PRODUCT_LIST="Atlas-300v"
-readonly A300IDUO_PRODOUCT_LIST="A300i-duo,Atlas-300i-duo"
-readonly A310P_PRODUCT_LIST="Ascend-hdk-310p,Ascend310P"
-readonly INFER_PRODUCT_LIST="Ascend-hdk-310,Ascend310,A300-3000,A300-3010,Atlas-200"
-readonly NORMALIZE_910_PRODUCT_LSIT="Ascend-hdk-910,Ascend910"
-readonly TRAIN_910B_PRODUCT_LIST="Ascend-hdk-910b,Ascend910B-hdk"
-readonly TRAIN_PRODUCT_LIST="A300t-9000,A800-9000,A800-9010,A900-9000"
-readonly TRAIN_PRO_PRODUCT_LIST="Atlas-300t-pro"
-readonly CANN_PRODUCT_LIST="Ascend-cann,Ascend-mindx"
-readonly APP_NAME_LIST=(all npu driver firmware nnrt nnae tfplugin toolbox toolkit atlasedge ha)
-
-readonly ROOT_CA=$(
-    cat <<EOF
------BEGIN CERTIFICATE-----
-MIIFTzCCAzegAwIBAgIIRbYUczgwtHkwDQYJKoZIhvcNAQELBQAwNzELMAkGA1UE
-BhMCQ04xDzANBgNVBAoTBkh1YXdlaTEXMBUGA1UEAxMOSHVhd2VpIFJvb3QgQ0Ew
-IBcNMTUxMDE1MDgwODUwWhgPMjA1MDEwMTUwODA4NTBaMDcxCzAJBgNVBAYTAkNO
-MQ8wDQYDVQQKEwZIdWF3ZWkxFzAVBgNVBAMTDkh1YXdlaSBSb290IENBMIICIjAN
-BgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA7kxjA5g73QH7nvrTI/ZEJP2Da3Q0
-Mg00q8/mM5DAmFkS5/9ru1ZQnKXN5zoq53e4f1r9eUhwjoakWIPjoTdC27hhBoKb
-ZbZODbS/uPFu8aXrcDnAnCe+02Dsh5ClHm+Dp37mIe56Nhw/fMVOqZf00cY4GyfJ
-KyBRC1cdecg1i2mCApLBe9WZh4/xlmmhCurkl6RyWrXqz6Xmi9glZhlR67g0Y0CU
-qtTvyv+GoJyTuH0zq1DUh6VRamKkmoHAMKpDgDfmFkH33UFwgU2X/ef6mJGpYsHu
-jlcvon5NZKAYBHmOof2e9mxDyIZH0mZnDsneMF5EDK4jO+qBdFn5KdXy8lOGiVVJ
-aeGtux3zG/LgGfil6881mylj3jHszyT0CyIRoQn9HwD5Pn6Punkp5BcyWdzdZ1TF
-cBKuIWOGUhbzcFoXnkyz6iDe4gxtH4D3ZQ3x0lpxIHeWUxKl1H0FeoEJx6PL0Koc
-/iJ+eMSzoxHx4J5CyTYgF99zpfS7nYXsRhr8y1asXcp7ubLoI8yLkMbBYrg+XFL0
-3gOHmkttdX67xKnCxcpYFVWs+nPwyvOCm81SH1YYnJnGP5csjH8hH2xbZpMpwrCZ
-n6lZf7tzafmezFgJ6f/A8NZPmzhXe+LXgfWaiE3dBTPFy6ubzBKlWT53BQpP4u11
-YvdVxNxSwrKhE4UCAwEAAaNdMFswHwYDVR0jBBgwFoAUcnaWww+QnNRVuK6bSe73
-31zJArQwDAYDVR0TBAUwAwEB/zALBgNVHQ8EBAMCAQYwHQYDVR0OBBYEFHJ2lsMP
-kJzUVbium0nu999cyQK0MA0GCSqGSIb3DQEBCwUAA4ICAQBwV1EEsMrEarDE0hEq
-EyA/N0YpBcUjNWO8UmLYWSzBpv4ePXNtV6PQ8RrGNthcisa56nbb+OfwclPpii01
-j89QVI4SlU8BFJUyU/FIRIudlSXWJzAVJcjHatU6Sqi7OdGDoZOIkx0jmyJ5rKoY
-oCj4hOjYHeYJIF/CEIF+OnZmj5P6e/MxxC0FvExgJrJyqgIGmRRRkoVEOxjpIHIt
-nIFaEa7y8cX9wnvjhYICR6CRmm0jzNsfd0lwdtOedlh3F7nIk8Ot1p3wUMKg1HcM
-cxzygWv4CjVTZy6E1/+s6KTEGwX0p/2ISJhfjtlREzvQ6mfwBPbI6NZmD0ymRsy7
-mlEEPnkweoEFN9y8P8GITupl20n5C/RD8J+I3ABysW4J57FY6moJawjYvpqGQi+R
-4viJ3QWyW+AyMO8hQim924uGNuxij8Avna2K5Mc4Tb/HjSBMJ9glsfTLNqN0xDT7
-b7/4o2Fkk5Szt/rKTiSVVbH22US2ri5SV8A+gbH/41NjFNZlAxsxLSN0gHeStDih
-kFs9liaQICKYpJToZKHS6hP0paYU61wSqy4lUEyka5KzQZIr7h/BZ8elVI6xGKHg
-v2VSpgYKuxC59I+syXRsN6AslVRq8/2Zo1IPcU3k01VsZAlvARrxS+lYfztdiss0
-gdNojAmDZwk73Vwty4KrPanEhw==
------END CERTIFICATE-----
-EOF
-)
-
-readonly ROOT_CA_G2=$(
-    cat <<EOF
------BEGIN CERTIFICATE-----
-MIIGQjCCA/agAwIBAgIDPDrbMEEGCSqGSIb3DQEBCjA0oA8wDQYJYIZIAWUDBAIB
-BQChHDAaBgkqhkiG9w0BAQgwDQYJYIZIAWUDBAIBBQCiAwIBIDB8MQswCQYDVQQG
-EwJDTjEcMBoGA1UEChMTSHVhd2VpIFRlY2hub2xvZ2llczEnMCUGA1UECxMeSHVh
-d2VpIENlcnRpZmljYXRpb24gQXV0aG9yaXR5MSYwJAYDVQQDEx1IdWF3ZWkgSW50
-ZWdyaXR5IFJvb3QgQ0EgLSBHMjAgFw0yMTAyMDcwOTM2NDZaGA8yMDUxMDUwNzA5
-MzY0NlowfDELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE0h1YXdlaSBUZWNobm9sb2dp
-ZXMxJzAlBgNVBAsTHkh1YXdlaSBDZXJ0aWZpY2F0aW9uIEF1dGhvcml0eTEmMCQG
-A1UEAxMdSHVhd2VpIEludGVncml0eSBSb290IENBIC0gRzIwggIiMA0GCSqGSIb3
-DQEBAQUAA4ICDwAwggIKAoICAQDdiU8j/HUtpiSLjsmr1t1P/nBDTbxuun0OVcia
-Q6Oc+E6y1YXCUmFn+p1WwKEJQetkKbCWlcZch8I2G/f86J/Z4m4ZwZJSV04B/uKQ
-GAy35FW5bNBtvYH3xN4ne0oGW6qWkgJQsDHG6iFZqRBKLx1O7yOhwvEdG5jfJwg2
-6NK5ad75vM6LHA6tEPG9ttMhcmj9VgzUdAFOHOt1IlAkZ+odFn6Prte4i/M0bYZg
-D/LShlgtBp+iDrWD+zHfcWADEGEsEzxyX7CJviJBTnoUwKM0/CQGLzaUTcGKfmVR
-qvlxCuSGRYsZWlOyoGomiSzmHxCMKzshrHW+RTO6YidFvbt/eKM0TRl3sXm6S1+C
-+FRY25es4lrXBm1/7VIcYy8CAmBAzYscFkaJqDiOqZ2wH3nDmonZeLgL0gfhSN5X
-ofsOa3+K0FwLGMSs8S6znSyFdmgsdAu53EzQQ/CDolyDKza38sqRMxa2FSvIrbji
-lypuUg6QH4p8XZdLac/D63s69rVbDgct9Yt39e7PCx51XLkQZevzW0wacuylvzyW
-TCHqvNHo3zVLvfhtfB70LkhTTnZIcJFSi/Qz62BfQwBriMLEtNaFDyVA1/ZyJLPa
-O0NvQ7T2tkkfsopSjGq8U9bcirLLyIJT3PW5j+zr96cO4nnO6TK2esXnBC6m/tqr
-NhKnQwIDAQABo2MwYTAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAd
-BgNVHQ4EFgQUDjkBfSbLAmrgyjRlUCChRGzsf54wHwYDVR0jBBgwFoAUDjkBfSbL
-AmrgyjRlUCChRGzsf54wQQYJKoZIhvcNAQEKMDSgDzANBglghkgBZQMEAgEFAKEc
-MBoGCSqGSIb3DQEBCDANBglghkgBZQMEAgEFAKIDAgEgA4ICAQBhnanpVOz0exdF
-fSyv8VxBZKL0XIYDue5nmeo0CJ2770Tj6NZawOJPkOAluzSAJpGKZdZgTfZdjKgR
-UmGAzL0IBdOf2lbmRyz4Qm1e6nTqB6TvveyeksnxfxDAQq0t2zbIv41OS3RObf5C
-T56TKR7mp7t6QR83Er8zaK8WbehFMx0puRTt+kST7b32Nzp2jI7jxlugi7+/oJoR
-dwYd7NKTdkpjLSBz3dfigt2Gp8U5BTXxAvO6hsVkb4OHbJ5n+h5avY8q/Hzzd2xc
-7bJFHVy5pL4nh/vM1z8/MRZUpxGLKOozNarYESVSzIZc9ovA08WKmaSqXkCgNwEv
-7K/cDCnKAp73aknUAGJg6zAN3BZikSLYM+V+Tmc4FR/UQG/+GSkdvg0kmxKt3izw
-oVctj/Je350VQLOgYkmOTQXdBCtMo8T5q/ZWq8mct1DtS4KaLxgLQQN214QS5MqY
-68mFyuU3eKN7sD7BUzhG6t+phVhFJ6mslPOpaxOSaUFwBXW1nZ4afoKrk7EFXVQ1
-xr37Fsc+a2P7DF9GD4liyzLc+0xOJZRVrM7fNPbdID0a2gp65qyTK4wrD/xsS7c6
-NtAPvl8SX/H76yV7/XFtqmmfRj3YyGj2DctWZ8qUVTsxHQxVMWkeFzf7G4au6jqn
-UCrZxwwkrbPM3H6LA3VdrF1oWN0hjg==
------END CERTIFICATE-----
-EOF
-)
 
 DEBUG_CMD=""
-STDOUT_CALLBACK=""
 
 declare -A OS_MAP=(["ubuntu"]="Ubuntu")
 OS_MAP["ubuntu"]="Ubuntu"
 OS_MAP["centos"]="CentOS"
 OS_MAP["euleros"]="EulerOS"
 OS_MAP["debian"]="Debian"
 OS_MAP["kylin"]="Kylin"
 OS_MAP["bclinux"]="BCLinux"
 OS_MAP["Linx"]="Linx"
 OS_MAP["UOS"]="UOS"
 OS_MAP["uos"]="UOS"
 OS_MAP["tlinux"]="Tlinux"
 OS_MAP["openEuler"]="OpenEuler"
 
-if [ -z ${ASNIBLE_CONFIG} ]; then
-    export ANSIBLE_CONFIG=$BASE_DIR/ansible.cfg
-fi
-if [ -z ${ASNIBLE_LOG_PATH} ]; then
-    export ANSIBLE_LOG_PATH=$BASE_DIR/install.log
-fi
-if [ -z ${ASNIBLE_INVENTORY} ]; then
-    export ANSIBLE_INVENTORY=$BASE_DIR/inventory_file
-fi
-if [ -z ${ANSIBLE_CACHE_PLUGIN_CONNECTION} ]; then
-    export ANSIBLE_CACHE_PLUGIN_CONNECTION=$BASE_DIR/facts_cache
-fi
-
-function is_safe_owned_file() {
-    local path=$1
-    local user_id=$(stat -c %u ${path})
-    local group_id=$(stat -c %g ${path})
-    if [ ! -n "${user_id}" ] || [ ! -n "${group_id}" ]; then
-        echo "user or group not exist"
-        return 1
-    fi
-    if [ $(stat -c '%A' ${path} | cut -c6) == w ] || [ $(stat -c '%A' ${path} | cut -c9) == w ]; then
-        echo "${path} does not comply with security rules."
-        return 1
-    fi
-    if [ ${user_id} != "0" ] && [ ${user_id} != ${UID} ]; then
-        echo "The path is not owned by root or current user"
-        return 1
-    fi
-    return 0
-}
-
-function is_safe_owned_dir() {
-    local path=$1
-    local user_id=$(stat -c %u ${path})
-    local group_id=$(stat -c %g ${path})
-    if [ ! -n "${user_id}" ] || [ ! -n "${group_id}" ]; then
-        echo "user or group not exist"
-        return 1
-    fi
-    if [ $(stat -c '%A' ${path} | cut -c6) == w ] || [ $(stat -c '%A' ${path} | cut -c9) == w ]; then
-        echo "${path} does not comply with security rules."
-        return 1
-    fi
-    if [ ${user_id} != "0" ] && [ ${user_id} != ${UID} ]; then
-        echo "The path is not owned by root or current user"
-        return 1
-    fi
-    return 0
-}
-
-function safe_file() {
-    local cur_path=$(realpath "$1")
-    is_safe_owned_file ${cur_path}
-    if [ $? -eq 1 ]; then
-        exit 1
-    fi
-    cur_path=$(dirname "$cur_path")
-    safe_dir ${cur_path}
-    if [ $? -eq 1 ]; then
-        exit 1
-    fi
-    return 0
-}
-
-function safe_dir() {
-    local cur_path=$1
-    while [ "${cur_path}" != "/" ]; do
-        is_safe_owned_dir ${cur_path}
-        if [ $? -eq 1 ]; then
-            exit 1
-        fi
-        cur_path=$(dirname "$cur_path")
-    done
-    return 0
-}
-
-function check_exec_file() {
-    local exec_files=(cat date whoami who awk sed grep bash ls mkdir tar chmod make find unzip openssl cp rm basename dirname mv touch which pwd uname sort stat cut realpath rpm dpkg python3 python)
-    for j in ${exec_files[@]}; do
-        which $j &>/dev/null
-        if [ $? -eq 0 ]; then
-            safe_file $(which $j)
-        fi
-    done
-}
+export ANSIBLE_CONFIG=$BASE_DIR/ansible.cfg
+export ANSIBLE_LOG_PATH=$BASE_DIR/install.log
+export ANSIBLE_CACHE_PLUGIN_CONNECTION=$BASE_DIR/facts_cache
 
 function log_info() {
     local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
     local USER_N=$(whoami)
     local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
     echo "[INFO] $*"
     echo "${DATE_N} ${USER_N}@${IP_N} [INFO] $*" >>${BASE_DIR}/install.log
@@ -259,76 +83,69 @@
 
 readonly PYTHON_TAR=${specified_python}
 
 readonly PYTHON_VERSION=$(echo ${specified_python} | sed 's/P/p/;s/-//')
 
 readonly PYTHON_MINOR=$(echo ${PYTHON_VERSION%.*})
 
-if [ ${UID} == 0 ]; then
-    readonly PYTHON_PREFIX=/usr/local/${PYTHON_VERSION}
-else
-    readonly PYTHON_PREFIX=${HOME}/.local/${PYTHON_VERSION}
-fi
+readonly PYTHON_PREFIX=${HOME}/.local/${PYTHON_VERSION}
 
 function get_os_version() {
     local id=${1}
     local ver=${2}
     local codename=${3}
     local version=${ver}
 
-    # Ubuntu, bclinux no need specific handle
+    # Ubuntu
+    if [ "${id}" == "Ubuntu" ]; then
+        ubuntu_version=$(grep -oP "^PRETTY_NAME=\K.*" /etc/os-release|awk '{print $2}')
+        if [[ $ubuntu_version =~ 18.04 ]] && [[ $ubuntu_version != 18.04.1 ]] && [[ $ubuntu_version != 18.04.5 ]];then
+            version=$ubuntu_version
+        fi
+    fi
 
     # CentOS
     if [ "${id}" == "CentOS" ]; then
-        if [ "${ver}" == "7" ]; then
-            version="7.6"
-        fi
-        if [ "${ver}" == "8" ]; then
-            version="8.2"
-        fi
+        version=$(cat /etc/centos-release|awk '{print $4}'|awk -v FS="." -v OFS="." '{print $1,$2}')
     fi
 
     # EulerOS
     if [ "${id}" == "EulerOS" ]; then
         if [ "${ver}" == "2.0" ] && [ "${codename}" == "SP8" ]; then
             version="2.8"
         elif [ "${ver}" == "2.0" ] && [[ "${codename}" =~ SP9 ]]; then
             version="2.9"
+        elif [ "${ver}" == "2.0" ] && [[ "${codename}" =~ SP10 ]]; then
+            version="2.10"
         fi
     fi
 
     # Debian
     if [ "${id}" == "Debian" ]; then
-        if [ "${ver}" == "9" ]; then
-            version="9.9"
-        elif [ "${ver}" == "10" ]; then
-            version="10.0"
-        fi
+        version=$(cat /etc/debian_version)
     fi
 
     # Kylin
     if [ "${id}" == "Kylin" ]; then
         version=${ver}${codename}
     fi
 
     # Linx 6 is almost same with debian 9
     if [ "${id}" == "Linx" ]; then
         if [ "${ver}" == "9" ]; then
-            version="6"
+            version="6.0.90"
         fi
         if [ "${ver}" == "10" ]; then
             version="6.0.100"
         fi
     fi
 
     # OpenEuler
     if [ "${id}" == "OpenEuler" ]; then
-        if [[ "${codename}" =~ "LTS" ]] || [[ "${codename}" == "" ]]; then
-            codename="LTS"
-        fi
+        codename=$(grep -oP "^VERSION=.*\KLTS[-\w]*" /etc/os-release)
         version=${ver}${codename}
     fi
 
     # UOS 20 SP1
     if [ "${id}" == "UOS" ] && [[ "$(grep -oP "^VERSION=\"?\K[\w\ ]+" /etc/os-release | awk '{print $2}')" == "SP1" ]]; then
         version="${ver}SP1"
     fi
@@ -371,16 +188,18 @@
     local os_name=$(get_os_name)
     if [ "${os_name}" != "EulerOS" ]; then
         return
     fi
     local euler=""
     if [[ "${g_os_ver_arch}" =~ 2.8 ]]; then
         euler="eulerosv2r8.${arch}"
-    else
+    elif [[ "${g_os_ver_arch}" =~ 2.9 ]]; then
         euler="eulerosv2r9.${arch}"
+    else
+        euler="eulerosv2r10.${arch}"
     fi
     local kh=$(rpm -qa kernel-headers | wc -l)
     local kd=$(rpm -qa kernel-devel | wc -l)
     local kh_rpm=$(find ${BASE_DIR}/resources/kernel/ -name "kernel-headers*" | sort -r | grep -m1 ${euler})
     local kd_rpm=$(find ${BASE_DIR}/resources/kernel/ -name "kernel-devel*" | sort -r | grep -m1 ${euler})
     if [ ${kh} -eq 0 ] && [ -f "${kh_rpm}" ]; then
         echo "install ${kh_rpm} when installing system packages" >>${BASE_DIR}/install.log
@@ -428,20 +247,16 @@
 }
 
 # check if resource of specific os is exists
 function check_resources() {
     if [ -d ${BASE_DIR}/resources/${g_os_ver_arch} ]; then
         return
     fi
-    log_warning "no resources founded for os ${g_os_ver_arch}, start downloading"
-    bash ${BASE_DIR}/start_download.sh --os-list=${g_os_ver_arch}
-    if [[ $? != 0 ]]; then
-        log_error "download ${g_os_ver_arch} fail"
-        return 1
-    fi
+    log_error "Resources missing detected, please run download operation firstly"
+    return 1
 }
 
 function install_sys_packages() {
     check_resources
     local check_resources_status=$?
     if [[ ${check_resources_status} != 0 ]]; then
         return ${check_resources_status}
@@ -485,19 +300,30 @@
     fi
 
     echo "install system packages are listed as follows:" >>${BASE_DIR}/install.log
     echo "$(ls ${BASE_DIR}/resources/${g_os_ver_arch} | grep -E "\.(rpm|deb)$")" >>${BASE_DIR}/install.log
     if [ $(command -v docker | wc -l) -eq 1 ];then
         log_warning "Docker is already installed on the system, and errors may occur when installing system dependencies"
     fi
-    if [ ${have_rpm} -eq 1 ]; then
+    if [[ "${g_os_ver_arch}" =~ OpenEuler_22.03LTS ]]; then
+      yum install --skip-broken --disablerepo="*" -y ${BASE_DIR}/resources/${g_os_ver_arch}/*.rpm
+      if [ $(command -v docker | wc -l) -eq 0 ];then
+        yum install --skip-broken --disablerepo="*" -y ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.rpm
+        systemctl restart docker
+      fi
+    elif [ ${have_rpm} -eq 1 ]; then
         rpm -ivh --force --nodeps --replacepkgs ${BASE_DIR}/resources/${g_os_ver_arch}/*.rpm
-    else
+        rpm -ivh --force --nodeps --replacepkgs ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.rpm
+        systemctl restart docker
+    fi
+    if [ ${have_rpm} -ne 1 ]; then
         export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical
         dpkg --force-all -i ${BASE_DIR}/resources/${g_os_ver_arch}/*.deb
+        dpkg --force-all -i ${BASE_DIR}/resources/${g_os_ver_arch}/docker/*.deb
+        systemctl restart docker
     fi
     if [[ $? != 0 ]]; then
         log_error "install system packages fail"
         return 1
     fi
 }
 
@@ -524,20 +350,16 @@
 }
 
 # check if resource of specific os is exists
 function check_python_resource() {
     if [ -f ${BASE_DIR}/resources/sources/${PYTHON_TAR}.tar.xz ]; then
         return
     fi
-    log_warning "can't find ${PYTHON_TAR}.tar.xz, start downloading"
-    bash ${BASE_DIR}/start_download.sh --os-list=${g_os_ver_arch}
-    if [[ $? != 0 ]]; then
-        log_error "download ${PYTHON_TAR}.tar.xz fail"
-        return 1
-    fi
+    log_error "Resources missing detected, please run download operation firstly"
+    return 1
 }
 
 function install_python375() {
     check_python_resource
     local check_python_resource_status=$?
     if [[ ${check_python_resource_status} != 0 ]]; then
         return ${check_python_resource_status}
@@ -561,794 +383,15 @@
         ${PYTHON_MINOR} -m pip install selinux --no-index --find-links ${PYLIB_PATH}
     fi
     echo "export PATH=${PYTHON_PREFIX}/bin:\$PATH" >${PYTHON_PREFIX}/../ascendrc 2>/dev/null
     echo "export LD_LIBRARY_PATH=${PYTHON_PREFIX}/lib:\$LD_LIBRARY_PATH" >>${PYTHON_PREFIX}/../ascendrc 2>/dev/null
     chmod 640 ${PYTHON_PREFIX}/../ascendrc
 }
 
-function install_ansible() {
-    log_info "install ansible"
-    local ansible_path=${PYTHON_PREFIX}/lib/${PYTHON_MINOR}/site-packages/ansible
-    ${PYTHON_MINOR} -m ensurepip
-    ${PYTHON_MINOR} -m pip install --upgrade pip --no-index --find-links ${PYLIB_PATH}
-    ${PYTHON_MINOR} -m pip install ansible-core --no-index --find-links ${PYLIB_PATH}
-    # patch the INTERPRETER_PYTHON_DISTRO_MAP, make it support EulerOS
-    if [ -f ${ansible_path}/config/base.yml ]; then
-        eulercnt=$(grep euleros ${ansible_path}/config/base.yml | wc -l)
-        if [ ${eulercnt} == 0 ]; then
-            # euler os 2 is recoginized as centos 2
-            sed -i "1501 i\      '2': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # ubuntu 18.04 is recoginized as debian buster/sid due tu /etc/debian_release
-            sed -i "1506 i\      'buster/sid': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # euler os use python3 as default python interpreter
-            sed -i "1516 i\    euleros:" ${ansible_path}/config/base.yml
-            sed -i "1517 i\      '2': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # kylin should use python3. if selinux enalbed, the default python have no selinux
-            sed -i "1518 i\    kylin:" ${ansible_path}/config/base.yml
-            sed -i "1519 i\      '10': /usr/bin/python3" ${ansible_path}/config/base.yml
-            sed -i "1520 i\      'V10': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # debian 10.0
-            sed -i "1506 i\      '10.0': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # ubuntu 20.04 is recoginized as debian bullseye/sid due to /etc/debian_version
-            sed -i "1508 i\      'bullseye/sid': /usr/bin/python3" ${ansible_path}/config/base.yml
-            # openeuler os use python3 as default python interpreter
-            sed -i "1523 i\    openeuler:" ${ansible_path}/config/base.yml
-            sed -i "1524 i\      '20.03': /usr/bin/python3" ${ansible_path}/config/base.yml
-            sed -i "1525 i\    uos:" ${ansible_path}/config/base.yml
-            sed -i "1526 i\      '20': /usr/bin/python3" ${ansible_path}/config/base.yml
-            sed -i "1527 i\    uniontech:" ${ansible_path}/config/base.yml
-            sed -i "1528 i\      '20': /usr/bin/python3" ${ansible_path}/config/base.yml
-        fi
-    fi
-}
-
-function check_extracted_size() {
-    local IFS_OLD=$IFS
-    unset IFS
-    for zip_package in $(find ${BASE_DIR}/resources/ -name "*.zip" 2>/dev/null); do
-        unzip -l ${zip_package} >/dev/null 2>&1
-        if [[ $? != 0 ]]; then
-            log_error "$(basename ${zip_package}) does not look like a zip compressed file"
-            return 1
-        fi
-        local check_zip=$(unzip -l ${zip_package} | awk -v size_threshold="${SIZE_THRESHOLD}" -v count_threshold="${ZIP_COUNT_THRESHOLD}" 'END {print ($1 <= size_threshold && $2 <= count_threshold)}')
-        if [[ ${check_zip} == 0 ]]; then
-            log_error "$(basename ${zip_package}) extracted size over 5G or extracted files count over ${ZIP_COUNT_THRESHOLD}"
-            return 1
-        fi
-        unzip -l ${zip_package} | grep -F "../" >/dev/null 2>&1
-        if [[ $? == 0 ]]; then
-            log_error "The name of $(basename ${zip_package}) contains ../"
-            return 1
-        fi
-        unzip -l ${zip_package} | grep -F '..\' >/dev/null 2>&1
-        if [[ $? == 0 ]]; then
-            log_error "The name of $(basename ${zip_package}) contains ..\\"
-            return 1
-        fi
-    done
-    for tar_package in $(find ${BASE_DIR}/resources/ -type f -name "*.tar" -o -name "*.tar.*z*" 2>/dev/null); do
-        tar tvf ${tar_package} >/dev/null 2>&1
-        if [[ $? != 0 ]]; then
-            log_error "$(basename ${tar_package}) does not look like a tar compressed file"
-            return 1
-        fi
-        local check_tar=$(tar tvf ${tar_package} | awk -v size_threshold="${SIZE_THRESHOLD}" -v count_threshold="${TAR_COUNT_THRESHOLD}" '{sum += $3} END {print (sum <= size_threshold && NR <= count_threshold)}')
-        if [[ ${check_tar} == 0 ]]; then
-            log_error "$(basename ${tar_package}) extracted size over 5G or extracted files count over ${TAR_COUNT_THRESHOLD}"
-            return 1
-        fi
-        tar tf ${tar_package} | grep -F "../" >/dev/null 2>&1
-        if [[ $? == 0 ]]; then
-            log_error "The name of $(basename ${tar_package}) contains ../"
-            return 1
-        fi
-        tar tf ${tar_package} | grep -F '..\' >/dev/null 2>&1
-        if [[ $? == 0 ]]; then
-            log_error "The name of $(basename ${tar_package}) contains ..\\"
-            return 1
-        fi
-    done
-    IFS=${IFS_OLD}
-}
-
-function check_npu_scene() {
-    IFS=","
-    for product in $1; do
-        if [[ "$2" =~ ${product} ]]; then
-            echo 1
-            unset IFS
-            return 0
-        fi
-    done
-    echo 0
-    unset IFS
-    return 0
-}
-
-function compare_crl() {
-    openssl crl -verify -in $1 -inform DER -CAfile $3 -noout 2>/dev/null
-    if [[ $? != 0 ]]; then
-        echo "$(basename $3) check $(basename $1) validation not pass" >>${BASE_DIR}/install.log
-        return 2
-    fi
-    if [[ -f $2 ]]; then
-        openssl crl -verify -in $2 -inform DER -CAfile $3 -noout 2>/dev/null
-        if [[ $? != 0 ]]; then
-            echo "$(basename $3) check $(basename $2) validation not pass" >>${BASE_DIR}/install.log
-            return 3
-        fi
-        local zip_crl_lastupdate_time=$(date +%s -d "$(openssl crl -in $1 -inform DER -noout -lastupdate | awk -F'lastUpdate=' '{print $2}')")
-        local sys_crl_lastupdate_time=$(date +%s -d "$(openssl crl -in $2 -inform DER -noout -lastupdate | awk -F'lastUpdate=' '{print $2}')")
-        if [[ ${zip_crl_lastupdate_time} -gt ${sys_crl_lastupdate_time} ]]; then
-            echo "$(basename $2) system crl update success" >>${BASE_DIR}/install.log
-            mkdir -p -m 700 $(dirname $2) && cp $1 $2 && chmod 600 $2
-            return 0
-        elif [[ ${zip_crl_lastupdate_time} -eq ${sys_crl_lastupdate_time} ]]; then
-            return 0
-        else
-            echo "$(basename $2) is newer than $(basename $1), no need to update system crl" >>${BASE_DIR}/install.log
-            return 1
-        fi
-    else
-        echo "$(basename $2) system crl update success" >>${BASE_DIR}/install.log
-        mkdir -p -m 700 $(dirname $2) && cp $1 $2 && chmod 600 $2
-    fi
-    return 0
-}
-
-function check_file_version() {
-    local file_version=$(basename $2 | cut -d '_' -f2)
-    IFS=","
-    for version in $1; do
-        if [[ "$file_version" =~ ${version} ]]; then
-            echo 1
-            unset IFS
-            return 0
-        fi
-    done
-    echo 0
-    unset IFS
-    return 0
-}
-
-function zip_extract() {
-    if [[ "$(basename ${zip_file})" =~ zip ]]; then
-        if [[ $(check_npu_scene ${CANN_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_cann_zip
-        elif [[ $(check_npu_scene ${A310P_SOC_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_soc_zip
-        elif [[ $(check_npu_scene ${A300I_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_a300i_zip
-        elif [[ $(check_npu_scene ${A300V_PRO_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_a300v_pro_zip
-        elif [[ $(check_npu_scene ${A300V_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_a300v_zip
-        elif [[ $(check_npu_scene ${A300IDUO_PRODOUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_a300iduo_zip
-        elif [[ $(check_npu_scene ${A310P_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_a310p_zip
-        elif [[ $(check_npu_scene ${INFER_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_infer_zip
-        elif [[ $(check_npu_scene ${TRAIN_910B_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_910b_zip
-        elif [[ $(check_npu_scene ${TRAIN_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_train_zip
-        elif [[ $(check_npu_scene ${TRAIN_PRO_PRODUCT_LIST} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_train_pro_zip
-        elif [[ $(check_npu_scene ${NORMALIZE_910_PRODUCT_LSIT} $(basename ${zip_file})) == 1 ]]; then
-            local run_from_zip=${BASE_DIR}/resources/run_from_910_zip
-        else
-            echo "not support $(basename ${zip_file}), please check" >>${BASE_DIR}/install.log
-            return 1
-        fi
-        mkdir -p -m 750 ${run_from_zip} && unzip -oq ${zip_file} -d ${run_from_zip}
-    else
-        if [[ "$(basename ${zip_file})" =~ atlasedge.*aarch64 ]]; then
-            local atlasedge_dir=${BASE_DIR}/resources/run_from_cann_zip/atlasedge_aarch64
-        elif [[ "$(basename ${zip_file})" =~ ha.*aarch64 ]]; then
-            local atlasedge_dir=${BASE_DIR}/resources/run_from_cann_zip/ha_aarch64
-        elif [[ "$(basename ${zip_file})" =~ atlasedge.*x86_64 ]]; then
-            local atlasedge_dir=${BASE_DIR}/resources/run_from_cann_zip/atlasedge_x86_64
-        elif [[ "$(basename ${zip_file})" =~ ha.*x86_64 ]]; then
-            local atlasedge_dir=${BASE_DIR}/resources/run_from_cann_zip/ha_x86_64
-        fi
-        mkdir -p -m 750 ${atlasedge_dir}
-        cp ${zip_file} ${cms_file} ${crl_file} ${atlasedge_dir}
-        tar --no-same-owner -xf ${zip_file} -C ${atlasedge_dir}
-    fi
-}
-
-function hmac_check() {
-    local sys_crl=$1
-    local ca_file=$2
-    compare_crl ${crl_file} ${sys_crl} ${ca_file}
-    local verify_crl=$?
-    if [[ ${verify_crl} == 0 ]]; then
-        local updated_crl=${crl_file}
-    elif [[ ${verify_crl} == 1 ]]; then
-        local updated_crl=${sys_crl}
-    else
-        return 1
-    fi
-    [[ ! "$(openssl crl -in ${updated_crl} -inform DER -noout -text)" =~ "$(openssl x509 -in ${ca_file} -serial -noout | awk -F'serial=' '{print $2}')" ]] &&
-        openssl cms -verify --no_check_time -in ${cms_file} -inform DER -CAfile ${ca_file} -binary -content ${zip_file} -purpose any -out /dev/null 2>/dev/null
-    local verify_success=$?
-    if [[ ${verify_success} -ne 0 ]]; then
-        echo "$(basename ${updated_crl}) or $(basename ${cms_file}) check cms validation not pass for $(basename ${ca_file})" >>${BASE_DIR}/install.log
-        return 1
-    fi
-}
-
-function verify_zip() {
-    unset IFS
-    local hmac_check_result=0
-    if [[ ${UID} == 0 ]]; then
-        local sys_crl_file=/etc/hwsipcrl/ascendsip.crl
-        local sys_g2_crl_file=/etc/hwsipcrl/ascendsip_g2.crl
-        local ascend_cert_path=/usr/local/Ascend/toolbox/latest/Ascend-DMI/bin/ascend-cert
-    else
-        local sys_crl_file=~/.local/hwsipcrl/ascendsip.crl
-        local sys_g2_crl_file=~/.local/hwsipcrl/ascendsip_g2.crl
-        local ascend_cert_path=~/Ascend/toolbox/latest/Ascend-DMI/bin/ascend-cert
-    fi
-    local root_ca_g2_file=${BASE_DIR}/playbooks/rootca_g2.pem
-    echo -e "${ROOT_CA_G2}" >${root_ca_g2_file}
-    local root_ca_file=${BASE_DIR}/playbooks/rootca.pem
-    echo -e "${ROOT_CA}" >${root_ca_file}
-    chmod 600 $2 ${root_ca_g2_file} ${root_ca_file}
-    for zip_package in $(
-        find ${BASE_DIR}/resources/CANN_* 2>/dev/null | grep ".zip$"
-        find ${BASE_DIR}/resources/*.zip 2>/dev/null
-        find ${BASE_DIR}/resources/patch/*.zip 2>/dev/null
-    ); do
-        rm -rf ${BASE_DIR}/resources/zip_tmp && unzip -q ${zip_package} -d ${BASE_DIR}/resources/zip_tmp
-        local cms_file=$(find ${BASE_DIR}/resources/zip_tmp/*.zip.cms 2>/dev/null || find ${BASE_DIR}/resources/zip_tmp/*.tar.gz.cms 2>/dev/null)
-        local zip_file=$(find ${BASE_DIR}/resources/zip_tmp/*.zip 2>/dev/null || find ${BASE_DIR}/resources/zip_tmp/*.tar.gz 2>/dev/null)
-        local crl_file=$(find ${BASE_DIR}/resources/zip_tmp/*.zip.crl 2>/dev/null || find ${BASE_DIR}/resources/zip_tmp/*.tar.gz.crl 2>/dev/null)
-        if [ -f ${ascend_cert_path} ]; then
-            echo "ascend-cert check $(basename ${zip_file})" >>${BASE_DIR}/install.log
-            ${ascend_cert_path} -u ${crl_file} >/dev/null 2>&1
-            if [[ $? != 0 ]]; then
-                echo "ascend-cert update $(basename ${crl_file}) to system failed" >>${BASE_DIR}/install.log
-                hmac_check_result=1
-            else
-                ${ascend_cert_path} ${cms_file} ${zip_file} ${crl_file} >/dev/null 2>&1
-                hmac_check_result=$?
-            fi
-        else
-            echo "openssl check $(basename ${zip_file})" >>${BASE_DIR}/install.log
-            hmac_check ${sys_g2_crl_file} ${root_ca_g2_file} || hmac_check ${sys_crl_file} ${root_ca_file}
-            hmac_check_result=$?
-        fi
-        if [[ ${hmac_check_result} == 0 ]]; then
-            zip_extract
-            rm -rf ${BASE_DIR}/resources/zip_tmp
-        else
-            rm -rf ${BASE_DIR}/resources/zip_tmp
-            break
-        fi
-    done
-    rm -rf ${root_ca_g2_file} ${root_ca_file}
-    chmod -R 750 $(find ${BASE_DIR}/resources/run_from_*_zip -type d 2>/dev/null) 2>/dev/null
-    chmod -R 640 $(find ${BASE_DIR}/resources/run_from_*_zip -type f 2>/dev/null) 2>/dev/null
-    return ${hmac_check_result}
-}
-
-function verify_zip_redirect() {
-    log_info "The system is busy with checking compressed files, Please wait for a moment..."
-    rm -rf ${BASE_DIR}/resources/zip_tmp
-    check_extracted_size
-    local check_extracted_size_status=$?
-    if [[ ${check_extracted_size_status} != 0 ]]; then
-        return ${check_extracted_size_status}
-    fi
-    verify_zip >${BASE_DIR}/tmp.log 2>&1
-    local verify_result=$?
-    cat ${BASE_DIR}/tmp.log >>${BASE_DIR}/install.log
-    cat ${BASE_DIR}/tmp.log && rm -rf ${BASE_DIR}/tmp.log
-    if [ ${verify_result} -ne 0 ]; then
-        log_error "check validation fail"
-        return 1
-    fi
-    if [[ $(find ${BASE_DIR}/resources -type f | wc -L) -gt 1023 ]] || [[ $(find ${BASE_DIR}/resources -type l | wc -L) -gt 1023 ]]; then
-        log_error "The file name contains more than 1023 characters"
-        return 1
-    fi
-}
-
-function check_run_pkg() {
-    if [[ "$(basename ${run_file})" =~ run ]]; then
-        if [[ $(check_npu_scene ${CANN_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_cann_zip
-        elif [[ $(check_npu_scene ${A310P_SOC_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_soc_zip
-        elif [[ $(check_npu_scene ${A300I_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_a300i_zip
-        elif [[ $(check_npu_scene ${A300V_PRO_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_a300v_pro_zip
-        elif [[ $(check_npu_scene ${A300V_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_a300v_zip
-        elif [[ $(check_npu_scene ${A300IDUO_PRODOUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_a300iduo_zip
-        elif [[ $(check_npu_scene ${A310P_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_a310p_zip
-        elif [[ $(check_npu_scene ${INFER_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_infer_zip
-        elif [[ $(check_npu_scene ${TRAIN_910B_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_910b_zip
-        elif [[ $(check_npu_scene ${TRAIN_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_train_zip
-        elif [[ $(check_npu_scene ${TRAIN_PRO_PRODUCT_LIST} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_train_pro_zip
-        elif [[ $(check_npu_scene ${NORMALIZE_910_PRODUCT_LSIT} $(basename ${run_file})) == 1 ]]; then
-            local run_pkg_dir=${BASE_DIR}/resources/run_from_910_zip
-        else
-            echo "not support $(basename ${run_file}), please check" >>${BASE_DIR}/install.log
-            return 1
-        fi
-        mkdir -p -m 750 ${run_pkg_dir} && cp ${run_file} ${run_pkg_dir}
-    fi
-}
-
-function check_run_pkgs() {
-    unset IFS
-    rm -rf ${BASE_DIR}/resources/run_from_*_zip
-    for run_file in $(find ${BASE_DIR}/resources -name '*.run'); do
-        check_run_pkg
-    done
-}
-
-function process_install() {
-    check_run_pkgs
-    verify_zip_redirect
-    local verify_zip_redirect_status=$?
-    if [[ ${verify_zip_redirect_status} != 0 ]]; then
-        return ${verify_zip_redirect_status}
-    fi
-    local tmp_install_play=${BASE_DIR}/playbooks/tmp_install.yml
-    echo "- import_playbook: gather_npu_fact.yml" >${tmp_install_play}
-    if [ "x${nocopy_flag}" != "xy" ]; then
-        echo "- import_playbook: distribution.yml" >>${tmp_install_play}
-    fi
-    IFS=','
-    if [[ ${install_target} =~ "driver" && ${install_target} =~ "firmware" ]]; then
-        echo "- import_playbook: install/install_npu.yml" >>${tmp_install_play}
-    fi
-    for target in ${install_target}; do
-        if [ ${target} == "python" ]; then
-            new_target="python375"
-        else
-            new_target=${target}
-        fi
-        if [[ ${target} == "driver" || ${target} == "firmware" ]] && [[ ${install_target} =~ "driver" && ${install_target} =~ "firmware" ]]; then
-            continue
-        fi
-        echo "- import_playbook: install/install_${new_target}.yml" >>${tmp_install_play}
-    done
-    unset IFS
-    echo "ansible-playbook -i ./inventory_file $(basename ${tmp_install_play}) -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} -e tensorflow_version=${TENSORFLOW_VERSION} -e kernels_type=${KERNELS_TYPE} -e force_upgrade_npu=${FORCE_UPGRADE_NPU} ${DEBUG_CMD}"
-    cat ${tmp_install_play}
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${tmp_install_play} -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} -e tensorflow_version=${TENSORFLOW_VERSION} -e kernels_type=${KERNELS_TYPE} -e force_upgrade_npu=${FORCE_UPGRADE_NPU} ${DEBUG_CMD}
-    local process_install_ansible_playbook_status=$?
-    if [ -f ${tmp_install_play} ]; then
-        rm -f ${tmp_install_play}
-    fi
-    if [[ ${process_install_ansible_playbook_status} != 0 ]]; then
-        return ${process_install_ansible_playbook_status}
-    fi
-}
-
-function process_scene() {
-    check_run_pkgs
-    verify_zip_redirect
-    local verify_zip_redirect_status_1=$?
-    if [[ ${verify_zip_redirect_status_1} != 0 ]]; then
-        return ${verify_zip_redirect_status_1}
-    fi
-    local tmp_scene_play=${BASE_DIR}/playbooks/tmp_scene.yml
-    echo "- import_playbook: gather_npu_fact.yml" >${tmp_scene_play}
-    if [ "x${nocopy_flag}" != "xy" ]; then
-        echo "- import_playbook: distribution.yml" >>${tmp_scene_play}
-    fi
-    echo "- import_playbook: scene/scene_${install_scene}.yml" >>${tmp_scene_play}
-    echo "ansible-playbook -i ./inventory_file $(basename ${tmp_scene_play}) -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} -e tensorflow_version=${TENSORFLOW_VERSION} -e kernels_type=${KERNELS_TYPE} -e force_upgrade_npu=${FORCE_UPGRADE_NPU} ${DEBUG_CMD}"
-    cat ${tmp_scene_play}
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${tmp_scene_play} -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} -e tensorflow_version=${TENSORFLOW_VERSION} -e kernels_type=${KERNELS_TYPE} -e force_upgrade_npu=${FORCE_UPGRADE_NPU} ${DEBUG_CMD}
-    local process_scene_ansible_playbook_status=$?
-    if [ -f ${tmp_scene_play} ]; then
-        rm -f ${tmp_scene_play}
-    fi
-    if [[ ${process_scene_ansible_playbook_status} != 0 ]]; then
-        return ${process_scene_ansible_playbook_status}
-    fi
-}
-
-function process_patch() {
-    rm -rf ${BASE_DIR}/resources/run_from_*_zip
-    verify_zip_redirect
-    local verify_zip_redirect_status_2=$?
-    if [[ ${verify_zip_redirect_status_2} != 0 ]]; then
-        return ${verify_zip_redirect_status_2}
-    fi
-    local tmp_patch_play=${BASE_DIR}/playbooks/tmp_patch.yml
-    echo "- import_playbook: gather_npu_fact.yml" >${tmp_patch_play}
-    if [ "x${nocopy_flag}" != "xy" ]; then
-        echo "- import_playbook: distribution.yml" >>${tmp_patch_play}
-    fi
-    IFS=','
-    for target in ${patch_target}; do
-        echo "- import_playbook: install/patch/install_${target}.yml" >>${tmp_patch_play}
-    done
-    unset IFS
-    echo "ansible-playbook -i ./inventory_file $(basename ${tmp_patch_play}) -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}"
-    cat ${tmp_patch_play}
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${tmp_patch_play} -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}
-    local process_patch_ansible_playbook_status=$?
-    if [ -f ${tmp_patch_play} ]; then
-        rm -f ${tmp_patch_play}
-    fi
-    if [[ ${process_patch_ansible_playbook_status} != 0 ]]; then
-        return ${process_patch_ansible_playbook_status}
-    fi
-}
-
-function process_patch_rollback() {
-    rm -rf ${BASE_DIR}/resources/run_from_*_zip
-    verify_zip_redirect
-    local verify_zip_redirect_status=$?
-    if [[ ${verify_zip_redirect_status} != 0 ]]; then
-        return ${verify_zip_redirect_status}
-    fi
-    local tmp_patch_rollback_play=${BASE_DIR}/playbooks/tmp_patch_rollback.yml
-    echo "- import_playbook: gather_npu_fact.yml" >${tmp_patch_rollback_play}
-    IFS=','
-    for target in ${patch_rollback_target}; do
-        echo "- import_playbook: install/patch/rollback_${target}.yml" >>${tmp_patch_rollback_play}
-    done
-    unset IFS
-    echo "ansible-playbook -i ./inventory_file $(basename ${tmp_patch_rollback_play}) -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}"
-    cat ${tmp_patch_rollback_play}
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${tmp_patch_rollback_play} -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}
-    local process_patch_rollback_ansible_playbook_status=$?
-    if [ -f ${tmp_patch_rollback_play} ]; then
-        rm -f ${tmp_patch_rollback_play}
-    fi
-    if [[ ${process_patch_rollback_ansible_playbook_status} != 0 ]]; then
-        return ${process_patch_rollback_ansible_playbook_status}
-    fi
-}
-
-function process_test() {
-    local tmp_test_play=${BASE_DIR}/playbooks/tmp_test.yml
-    echo "- import_playbook: gather_npu_fact.yml" >${tmp_test_play}
-    IFS=','
-    for target in ${test_target}; do
-        echo "- import_playbook: test/test_${target}.yml" >>${tmp_test_play}
-    done
-    unset IFS
-    echo "ansible-playbook -i ./inventory_file $(basename ${tmp_test_play}) -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}"
-    cat ${tmp_test_play}
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${tmp_test_play} -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION} ${DEBUG_CMD}
-    local process_test_ansible_playbook_status=$?
-    if [ -f ${tmp_test_play} ]; then
-        rm -f ${tmp_test_play}
-    fi
-    if [[ ${process_test_ansible_playbook_status} != 0 ]]; then
-        return ${process_test_ansible_playbook_status}
-    fi
-}
-
-function process_check() {
-    echo "ansible-playbook -i ./inventory_file playbooks/gather_npu_fact.yml -e hosts_name=ascend -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION}"
-    ansible_playbook -i ${BASE_DIR}/inventory_file ${BASE_DIR}/playbooks/gather_npu_fact.yml -e "hosts_name=ascend" -e python_tar=${PYTHON_TAR} -e python_version=${PYTHON_VERSION}
-    local process_check_ansible_playbook_status=$?
-    if [[ ${process_check_ansible_playbook_status} != 0 ]]; then
-        return ${process_check_ansible_playbook_status}
-    fi
-}
-
-function process_chean() {
-    ansible -i ${BASE_DIR}/inventory_file all -m shell -a "rm -rf ~/resources.tar ~/resources"
-    local process_chean_ansible_status=$?
-    if [[ ${process_chean_ansible_status} != 0 ]]; then
-        return ${process_chean_ansible_status}
-    fi
-}
-
-function print_usage() {
-    unset IFS
-    echo "Usage: ./install.sh [options]"
-    echo " Options:"
-    echo "--help  -h                     show this help message and exit"
-    echo "--check                        check environment"
-    echo "--clean                        clean resources on remote servers"
-    echo "--nocopy                       do not copy resources to remote servers when install for remote"
-    echo "--force_upgrade_npu            can force upgrade NPU when not all devices have exception"
-    echo "--kernels_type                 Appoint kernels package type,must be nnae or toolkit,default is nnae"
-    echo "--tensorflow_version           Appoint tensorflow version,must be 1.15.0 or 2.6.5,default is 1.15.0"
-    echo "--verbose                      Print verbose"
-    echo "--output-file=<output_file>    Redirect the output of ansible execution results to a file"
-    echo "--stdout_callback=<callback_name> set stdout_callback for ansible"
-    echo "                               avaiable callback could be listed by: ansible-doc -t callback -l"
-    echo "--install=<package_name>       Install specific package:"
-    for target in $(find ${BASE_DIR}/playbooks/install/install_*.yml); do
-        target=$(basename ${target})
-        if [ ${target} == "install_python375.yml" ]; then
-            target="install_python.yml"
-        fi
-        tmp=${target#*_}
-        echo "                               ${tmp%.*}"
-    done
-    echo "The \"npu\" will install driver and firmware together"
-    echo "--install-scene=<scene_name>   Install specific scene:"
-    for scene in $(find ${BASE_DIR}/playbooks/scene/scene_*.yml); do
-        scene=$(basename ${scene})
-        tmp=${scene#*_}
-        echo "                               ${tmp%.*}"
-    done
-    echo "--patch=<package_name>         Patching specific package:"
-    for target in $(find ${BASE_DIR}/playbooks/install/patch/install_*.yml); do
-        target=$(basename ${target})
-        tmp=${target#*_}
-        echo "                               ${tmp%.*}"
-    done
-    echo "--patch-rollback=<package_name> Rollback specific package:"
-    for target in $(find ${BASE_DIR}/playbooks/install/patch/install_*.yml); do
-        target=$(basename ${target})
-        tmp=${target#*_}
-        echo "                               ${tmp%.*}"
-    done
-    echo "--test=<target>                test the functions:"
-    for test in $(find ${BASE_DIR}/playbooks/test/test_*.yml); do
-        test=$(basename ${test})
-        tmp=${test#*_}
-        echo "                               ${tmp%.*}"
-    done
-}
-
-FORCE_UPGRADE_NPU=false
-KERNELS_TYPE=nnae
-TENSORFLOW_VERSION=1.15.0
-
-function parse_script_args() {
-    if [ $# = 0 ]; then
-        print_usage
-        return 6
-    fi
-    while true; do
-        case "$1" in
-        --help | -h)
-            print_usage
-            return 6
-            ;;
-        --install=*)
-            install_target=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${install_target}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--install parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --install-scene=*)
-            install_scene=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${install_scene}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--install-scene parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --patch=*)
-            patch_target=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${patch_target}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--patch parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --patch-rollback=*)
-            patch_rollback_target=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${patch_rollback_target}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--patch_rollback parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --test=*)
-            test_target=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${test_target}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--test parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --output-file=*)
-            output_file=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${output_file}" | grep -Evq '^[a-zA-Z0-9._,/-]*$'); then
-                log_error "--output-file parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --stdout_callback=*)
-            STDOUT_CALLBACK=$(echo $1 | cut -d"=" -f2)
-            if $(echo "${STDOUT_CALLBACK}" | grep -Evq '^[a-zA-Z0-9._,]*$'); then
-                log_error "--stdout_callback parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --nocopy)
-            nocopy_flag=y
-            shift
-            ;;
-        --force_upgrade_npu)
-            FORCE_UPGRADE_NPU=true
-            shift
-            ;;
-        --kernels_type=*)
-            KERNELS_TYPE=$(echo $1 | cut -d"=" -f2)
-            if [[ "${KERNELS_TYPE}" != "nnae" ]] && [[ "${KERNELS_TYPE}" != "toolkit" ]]; then
-                log_error "--kernels_type parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --tensorflow_version=*)
-            TENSORFLOW_VERSION=$(echo $1 | cut -d"=" -f2)
-            if [[ "${TENSORFLOW_VERSION}" != "1.15.0" ]] && [[ "${TENSORFLOW_VERSION}" != "2.6.5" ]]; then
-                log_error "--tensorflow_version parameter is invalid"
-                print_usage
-                return 1
-            fi
-            shift
-            ;;
-        --verbose)
-            DEBUG_CMD="-v"
-            shift
-            ;;
-        --check)
-            check_flag=y
-            shift
-            ;;
-        --clean)
-            clean_flag=y
-            shift
-            ;;
-        *)
-            if [ "x$1" != "x" ]; then
-                log_error "Unsupported parameters: $1"
-                print_usage
-                return 1
-            fi
-            break
-            ;;
-        esac
-    done
-}
-
-function check_script_args() {
-    if [ -z ${install_target} ] && [ -z ${install_scene} ] && [ -z ${patch_target} ] && [ -z ${patch_rollback_target} ] && [ -z ${test_target} ] && [[ ${check_flag} != "y" ]] && [[ ${clean_flag} != "y" ]]; then
-        log_error "expected one valid argument at least"
-        print_usage
-        return 1
-    fi
-
-    # --install
-    IFS=','
-    local unsupport=${FALSE}
-    for target in ${install_target}; do
-        if [ ${target} == 'python' ]; then
-            continue
-        fi
-        if [ ! -z ${target} ] && [ ! -f ${BASE_DIR}/playbooks/install/install_${target}.yml ]; then
-            log_error "not support install for ${target}"
-            unsupport=${TRUE}
-        fi
-    done
-    if [ ${unsupport} == ${TRUE} ]; then
-        print_usage
-        return 1
-    fi
-    unset IFS
-
-    # --install-scene
-    local unsupport=${FALSE}
-    if [ ! -z ${install_scene} ] && [ ! -f ${BASE_DIR}/playbooks/scene/scene_${install_scene}.yml ]; then
-        log_error "not support install scene for ${install_scene}"
-        unsupport=${TRUE}
-    fi
-    if [ ${unsupport} == ${TRUE} ]; then
-        print_usage
-        return 1
-    fi
-
-    # --patch
-    IFS=','
-    local unsupport=${FALSE}
-    for target in ${patch_target}; do
-        if [ ! -z ${target} ] && [ ! -f ${BASE_DIR}/playbooks/install/patch/install_${target}.yml ]; then
-            log_error "not support install patch for ${target}"
-            unsupport=${TRUE}
-        fi
-    done
-    if [ ${unsupport} == ${TRUE} ]; then
-        print_usage
-        return 1
-    fi
-    unset IFS
-
-    # --patch-rollback
-    IFS=','
-    local unsupport=${FALSE}
-    for target in ${patch_rollback_target}; do
-        if [ ! -z ${target} ] && [ ! -f ${BASE_DIR}/playbooks/install/patch/install_${target}.yml ]; then
-            log_error "not support rollback for ${target}"
-            unsupport=${TRUE}
-        fi
-    done
-    if [ ${unsupport} == ${TRUE} ]; then
-        print_usage
-        return 1
-    fi
-    unset IFS
-
-    # --test
-    IFS=','
-    local unsupport=${FALSE}
-    for target in ${test_target}; do
-        if [ ! -z ${target} ] && [ ! -f ${BASE_DIR}/playbooks/test/test_${target}.yml ]; then
-            log_error "not support test for ${target}"
-            unsupport=${TRUE}
-        fi
-    done
-    if [ ${unsupport} == ${TRUE} ]; then
-        print_usage
-        return 1
-    fi
-    unset IFS
-
-    # --custom
-    if [ "x${install_target}" != "x" ] && [ "x${install_scene}" != "x" ]; then
-        log_error "Unsupported --install and --install-scene at same time"
-        print_usage
-        return 1
-    fi
-}
-
-function ansible_playbook() {
-    if [ -z "${output_file}" ]; then
-        ansible-playbook $*
-    elif [ -f "${output_file}" ]; then
-        log_error "${output_file} already exists, please specify another output file name"
-        return 1
-    else
-        ansible-playbook $* >"${output_file}"
-    fi
-}
 
-function check_inventory() {
-    local pass1=$(grep ansible_ssh_pass ${BASE_DIR}/inventory_file | wc -l)
-    local pass2=$(grep ansible_sudo_pass ${BASE_DIR}/inventory_file | wc -l)
-    local pass3=$(grep ansible_become_pass ${BASE_DIR}/inventory_file | wc -l)
-    local pass_cnt=$((pass1 + pass2 + pass3))
-    if [ ${pass_cnt} == 0 ]; then
-        return
-    fi
-    log_error "The inventory_file contains password, please use the SSH key instead"
-    return 1
-}
 
 function bootstrap() {
     export PATH=${PYTHON_PREFIX}/bin:$PATH
     export LD_LIBRARY_PATH=${PYTHON_PREFIX}/lib:$LD_LIBRARY_PATH
     unset PYTHONPATH
 
     check_python375
@@ -1368,20 +411,15 @@
         install_python375
         local install_python375_status_1=$?
         if [[ ${install_python375_status_1} != 0 ]]; then
             return ${install_python375_status_1}
         fi
     fi
 
-    local have_ansible_cmd=$(command -v ansible | wc -l)
-    have_no_python_module "ansible"
-    if [[ $? == ${TRUE} ]] || [[ ${have_ansible_cmd} == 0 ]]; then
-        log_warning "no ansible"
-        install_ansible
-    fi
+    bash ${BASE_DIR}/scripts/install_ansible.sh
 }
 
 function rotate_log() {
     local log_list=$(ls $1* | sort -r)
     for item in $log_list; do
         local suffix=${item##*.}
         local prefix=${item%.*}
@@ -1417,150 +455,37 @@
         fi
     done
     chmod 750 $BASE_DIR/ $BASE_DIR/playbooks/install
     chmod 600 ${BASE_DIR}/*.log ${BASE_DIR}/tools/*.log ${BASE_DIR}/inventory_file $BASE_DIR/ansible.cfg ${BASE_DIR}/downloader/config.ini 2>/dev/null
     chmod 400 ${BASE_DIR}/*.log.? ${BASE_DIR}/tools/*.log.? 2>/dev/null
 }
 
-function prepare_environment() {
-    if [ -z ${ANSIBLE_STDOUT_CALLBACK} ] && [ ! -z ${STDOUT_CALLBACK} ]; then
-        export ANSIBLE_STDOUT_CALLBACK=${STDOUT_CALLBACK}
-    fi
-}
 main() {
     local os_name=$(grep -oP "^ID=\"?\K\w+" /etc/os-release)
-    if type python >/dev/null 2>&1; then
-        local python='python'
-    elif type python3 >/dev/null 2>&1; then
-        local python='python3'
-    else
-        echo "python or python3 must be installed"
-        exit 1
-    fi
-    case ${os_name} in
-    ubuntu)
-        dpkg -l >previous_dpkg.txt
-        ;;
-    openEuler)
-        rpm -qa >previous_rpm.txt
-        ;;
-    centos)
-        rpm -qa >previous_rpm.txt
-        ;;
-    esac
-    check_exec_file
     check_log ${BASE_DIR}/install.log
     check_log ${BASE_DIR}/install_operation.log
     set_permission
 
     check_python_version
     local check_python_version_status=$?
     if [[ ${check_python_version_status} != 0 ]]; then
         return ${check_python_version_status}
     fi
 
-    parse_script_args $*
-    local parse_script_args_status=$?
-    if [[ ${parse_script_args_status} != 0 ]]; then
-        return ${parse_script_args_status}
-    fi
-
-    check_script_args
-    local check_script_args_status=$?
-    if [[ ${check_script_args_status} != 0 ]]; then
-        return ${check_script_args_status}
-    fi
-
     if [ -d ${BASE_DIR}/facts_cache ]; then
         rm -rf ${BASE_DIR}/facts_cache && mkdir -p -m 750 ${BASE_DIR}/facts_cache
     fi
 
     bootstrap
     local bootstrap_status=$?
     if [[ ${bootstrap_status} != 0 ]]; then
         return ${bootstrap_status}
     fi
 
-    check_inventory
-    local check_inventory_status=$?
-    if [[ ${check_inventory_status} != 0 ]]; then
-        return ${check_inventory_status}
-    fi
-
-    prepare_environment
-
-    if [ "x${install_target}" != "x" ]; then
-        process_install ${install_target}
-        local process_install_status=$?
-        if [[ ${process_install_status} != 0 ]]; then
-            return ${process_install_status}
-        fi
-    fi
-
-    if [ "x${install_scene}" != "x" ]; then
-        process_scene ${install_scene}
-        local process_scene_status=$?
-        if [[ ${process_scene_status} != 0 ]]; then
-            return ${process_scene_status}
-        fi
-    fi
-
-    if [ "x${patch_target}" != "x" ]; then
-        process_patch ${patch_target}
-        local process_patch_status=$?
-        if [[ ${process_patch_status} != 0 ]]; then
-            return ${process_patch_status}
-        fi
-    fi
-
-    if [ "x${patch_rollback_target}" != "x" ]; then
-        process_patch_rollback ${patch_rollback_target}
-        local process_patch_rollback_status=$?
-        if [[ ${process_patch_rollback_status} != 0 ]]; then
-            return ${process_patch_rollback_status}
-        fi
-    fi
-
-    if [ "x${test_target}" != "x" ]; then
-        process_test ${test_target}
-        local process_test_status=$?
-        if [[ ${process_test_status} != 0 ]]; then
-            return ${process_test_status}
-        fi
-    fi
-
-    if [ "x${check_flag}" == "xy" ]; then
-        process_check
-        local process_check_status=$?
-        if [[ ${process_check_status} != 0 ]]; then
-            return ${process_check_status}
-        fi
-    fi
-
-    if [ "x${clean_flag}" == "xy" ]; then
-        process_chean
-        local process_chean_status=$?
-        if [[ ${process_chean_status} != 0 ]]; then
-            return ${process_chean_status}
-        fi
-    fi
-    case ${os_name} in
-    ubuntu)
-        dpkg -l >current_dpkg.txt
-        ${python} report.py dpkg
-        ;;
-    openEuler)
-        rpm -qa >current_rpm.txt
-        ${python} report.py rpm
-        ;;
-    centos)
-        rpm -qa >current_rpm.txt
-        ${python} report.py rpm
-        ;;
-    esac
+    $PYTHON_MINOR ${BASE_DIR}/ascend_deployer.py $*
 }
 
 main $*
 main_status=$?
 if [[ ${main_status} != 0 ]] && [[ ${main_status} != 6 ]]; then
     operation_log_info "parameter error,run failed"
 else
```

## ascend_deployer/inventory_file

```diff
@@ -1,7 +1,28 @@
-[ascend]
+[hccn]
+
+[hccn:vars]
+gateways=""
+netmask="255.255.255.0"
+roce_port=4791
+bitmap=""
+dscp_tc=""
+common_network="0.0.0.0/0"
+
+[master]
+#10.10.10.10 ansible_ssh_user="root" ansible_ssh_pass="test1234" k8s_api_server_ip=10.10.10.10
+
+[worker]
 localhost ansible_connection='local'
 
-[ascend:vars]
-user=HwHiAiUser
-group=HwHiAiUser
-install_path=/usr/local/Ascend
+[other_build_image]
+
+[all:vars]
+SCENE_NUM=1
+EXTRA_COMPONENT=""
+POD_NETWORK_CIDR="192.168.0.0/16"
+KUBE_VIP=""
+HARBOR_SERVER=""
+HARBOR_ADMIN_USER=""
+HARBOR_ADMIN_PASSWORD=""
+HARBOR_PUBLIC_PROJECT="false"
+HARBOR_CA_FILE=""
```

## ascend_deployer/start_download.sh

```diff
@@ -2,95 +2,14 @@
 unset LD_LIBRARY_PATH
 declare -x PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:"${ASCENDPATH}""
 readonly TRUE=1
 readonly FALSE=0
 readonly BASE_DIR=$(cd "$(dirname $0)" > /dev/null 2>&1; pwd -P)
 readonly LOG_SIZE_THRESHOLD=$((20*1024*1024))
 readonly LOG_COUNT_THRESHOLD=5
-OS_LIST=""
-PKG_LIST=""
-
-function is_safe_owned_file()
-{
-    local path=$1
-    local user_id=$(stat -c %u ${path})
-    local group_id=$(stat -c %g ${path})
-    if [ ! -n "${user_id}" ] || [ ! -n "${group_id}" ];then
-        echo "user or group not exist"
-        return 1
-    fi
-    if [ $(stat -c '%A' ${path}|cut -c6) == w ] || [ $(stat -c '%A' ${path}|cut -c9) == w ];then
-        echo "${path} does not comply with security rules."
-        return 1
-    fi
-    if [ ${user_id} != "0" ] && [ ${user_id} != ${UID} ];then
-        echo "The path is not owned by root or current user"
-        return 1
-    fi
-    return 0
-}
-
-function is_safe_owned_dir()
-{
-    local path=$1
-    local user_id=$(stat -c %u ${path})
-    local group_id=$(stat -c %g ${path})
-    if [ ! -n "${user_id}" ] || [ ! -n "${group_id}" ];then
-        echo "user or group not exist"
-        return 1
-    fi
-    if [ $(stat -c '%A' ${path}|cut -c6) == w ] || [ $(stat -c '%A' ${path}|cut -c9) == w ];then
-        echo "${path} does not comply with security rules."
-        return 1
-    fi
-    if [ ${user_id} != "0" ] && [ ${user_id} != ${UID} ];then
-        echo "The path is not owned by root or current user"
-        return 1
-    fi
-    return 0
-}
-
-function safe_file()
-{
-    local cur_path=$(realpath "$1")
-    is_safe_owned_file ${cur_path}
-    if [ $? -eq 1 ];then
-        exit 1
-    fi
-    cur_path=$(dirname "$cur_path")
-    safe_dir ${cur_path}
-    if [ $? -eq 1 ];then
-        exit 1
-    fi
-    return 0
-}
-
-function safe_dir()
-{
-    local cur_path=$1
-    while [ "${cur_path}" != "/" ];do
-        is_safe_owned_dir ${cur_path}
-        if [ $? -eq 1 ];then
-            exit 1
-        fi
-        cur_path=$(dirname "$cur_path")
-    done
-    return 0
-}
-
-function check_exec_file()
-{
-    local files=(cat date whoami who awk sed grep ls chmod find rm basename dirname mv touch which pwd sort stat cut realpath yum apt python3 python)
-    for j in ${files[@]};do
-    which $j &> /dev/null
-    if [ $? -eq 0 ];then
-        safe_file $(which $j)
-    fi
-    done
-}
 
 function operation_log_info()
 {
     local DATE_N=$(date "+%Y-%m-%d %H:%M:%S")
     local USER_N=$(whoami)
     local IP_N=$(who am i | awk '{print $NF}' | sed 's/[()]//g')
     echo "${DATE_N} ${USER_N}@${IP_N} [INFO] $*" >> ${BASE_DIR}/downloader_operation.log
@@ -163,227 +82,40 @@
     # centos 8.2
     platform_python="/usr/libexec/platform-python3.6"
     if [ -f ${platform_python} ];then
         echo ${platform_python}
         return 0
     fi
 
-    # this python3 mybe replace by user and have no lzma or other module
+    # this python3 maybe replace by user and have no lzma or other module
     have_python3=$(command -v python3 | wc -l)
     if [ ${have_python3} -eq 1 ];then
         echo python3
         return 0
     fi
 
     return 1
 }
 
-function install_python3()
-{
-
-    if [ $(id -u) -ne 0 ];then
-        log_error "you are not root user and python3 is not available, please install python3 first by yourself"
-        return 1
-    fi
-
-    have_yum=$(command -v yum | wc -l)
-    if [ ${have_yum} -eq 1 ];then
-        log_info "yum install -y python3"
-        yum install -y python3 > ${BASE_DIR}/tmp.log 2>&1
-        local install_result=$?
-        cat ${BASE_DIR}/tmp.log >> ${BASE_DIR}/downloader.log
-        cat ${BASE_DIR}/tmp.log && rm -rf ${BASE_DIR}/tmp.log
-        if [[ ${install_result} != 0 ]];then
-            log_error "python3 is not available and yum install -y python3 failed, please check network or yum"
-            return 1
-        fi
-
-    fi
-
-    have_apt=$(command -v apt | wc -l)
-    if [ ${have_apt} -eq 1 ];then
-        log_info "apt install -y python3"
-        apt install -y python3 > ${BASE_DIR}/tmp.log 2>&1
-        local install_result=$?
-        cat ${BASE_DIR}/tmp.log >> ${BASE_DIR}/downloader.log
-        cat ${BASE_DIR}/tmp.log && rm -rf ${BASE_DIR}/tmp.log
-        if [[ ${install_result} != 0 ]];then
-            log_error "python3 is not available and apt install -y python3 failed, please check network or apt"
-            return 1
-        fi
-    fi
-
-    have_python3=$(command -v python3 | wc -l)
-    if [ ${have_python3} -eq 0 ];then
-        log_error "python3 is not available, please check python3"
-        return 1
-    fi
-}
-
-function print_usage()
-{
-    echo "Usage: ./start_download.sh [-h] [--os-list=OS_LIST] [--download=PACKAGES]]"
-    echo ""
-    echo " optional arguments:"
-    echo "--help  -h               show this help message and exit"
-    echo "--os-list=<OS1>,<OS2>    Specific OS list to download, supported os are:"
-    for os in $(find ${BASE_DIR}/downloader/config -maxdepth 1 -mindepth 1 -type d | sort -V)
-    do
-        os_name=$(basename ${os})
-        echo "                         ${os_name}"
-    done
-    echo "--download=<PK1>,<PK2>==<Version>"
-    echo "                         Specific package list to download, supported packages are:"
-    for package_json in $(find ${BASE_DIR}/downloader/software -maxdepth 1 -type f -name "*.json" | sort -V)
-    do
-        package=$(basename ${package_json} .json | sed "s/_/==/g")
-        echo "                         ${package}"
-    done
-    echo -e "\n  notes: When <Version> is missing, <PK> is the latest.\n"
-}
-
-function parse_script_args() {
-    if [ $# = 0 ];then
-        print_usage
-        return 2
-    fi
-    while true; do
-        case "$1" in
-        --help | -h)
-            print_usage
-            return 2
-            ;;
-        --os-list=*)
-            OS_LIST=$(echo $1 | cut -d"=" -f2)
-            shift
-            ;;
-        --download=*)
-            PKG_LIST=$(echo $1| cut -d"=" -f2-)
-            shift
-            ;;
-        *)
-            if [ "x$1" != "x" ]; then
-                log_error "Unsupported parameters: $1"
-                print_usage
-                return 1
-            fi
-            break
-            ;;
-        esac
-    done
-}
-
-function check_script_args()
-{
-    if [ -z "${OS_LIST}" ] && [ -z "${PKG_LIST}" ];then
-        log_error "--os-list or --download expected one argument at least"
-        print_usage
-        return 1
-    fi
-
-    if [ -z "${OS_LIST}" ] && [[ "${PKG_LIST}" =~ "MindSpore" ]];then
-        log_error "os_list can not be none when downloading mindspore"
-        print_usage
-        return 1
-    fi
-
-    if [ -z "${OS_LIST}" ] && [[ "${PKG_LIST}" =~ "MindStudio" ]];then
-        log_error "os_list can not be none when downloading MindStudio"
-        print_usage
-        return 1
-    fi
-
-    # --os-list
-    if $(echo "${OS_LIST}" | grep -Evq '^[a-zA-Z0-9._,-]*$');then
-        log_error "--os-list ${OS_LIST} is invalid"
-        print_usage
-        return 1
-    fi
-    local unsupport=${FALSE}
-    IFS=','
-    for os in ${OS_LIST}
-    do
-        if [ "${os}" = "." ] || [ ! -d ${BASE_DIR}/downloader/config/${os} ];then
-            log_error "not support download for ${os}"
-            unsupport=${TRUE}
-        fi
-    done
-    unset IFS
-    if [ ${unsupport} == ${TRUE} ];then
-        print_usage
-        return 1
-    fi
-
-    # --download
-    if $(echo "${PKG_LIST}" | grep -Evq '^[a-zA-Z0-9._,=]*$');then
-        log_error "--download ${PKG_LIST} is invalid"
-        print_usage
-        return 1
-    fi
-    local unsupport=${FALSE}
-    IFS=','
-    for package in ${PKG_LIST}
-    do
-        case "${package}" in
-        CANN|MindStudio|MindSpore)
-            continue
-            ;;
-        *)
-        local name_version=$(echo ${package} | awk -F== '{print $1"_"$2}')
-            if [ ! -f ${BASE_DIR}/downloader/software/${name_version}.json ];then
-                log_error "not support download for ${package}"
-                unsupport=${TRUE}
-            fi
-            ;;
-        esac
-    done
-    unset IFS
-    if [ ${unsupport} == ${TRUE} ];then
-        print_usage
-        return 1
-    fi
-}
-
 function main()
 {
-    check_exec_file
     check_log ${BASE_DIR}/downloader.log
     check_log ${BASE_DIR}/downloader_operation.log
     set_permission
-    parse_script_args $*
-    parse_status=$?
-    if [[ ${parse_status} != 0 ]];then
-        return ${parse_status}
-    fi
-
-    check_script_args
-    if [[ $? != 0 ]];then
-        return 1
-    fi
 
     get_python3 >/dev/null 2>&1
     if [[ $? == 0 ]];then
         local pycmd=$(get_python3)
     else
-        install_python3
-        if [[ $? != 0 ]];then
-            return 1
-        fi
-        local pycmd="python3"
-    fi
-    local os_cmd=""
-    if [ ! -z "${OS_LIST}" ];then
-        os_cmd="--os-list ${OS_LIST}"
-    fi
-    local download_cmd=""
-    if [ ! -z "${PKG_LIST}" ];then
-        download_cmd="--download ${PKG_LIST}"
+        log_error "python3 is not available, install it first by running 'apt install -y python3' or 'yum install -y python3' with root permission and available repo accessing"
+        return 1
     fi
-    log_info "${pycmd} $(basename ${BASE_DIR})/downloader/downloader.py ${os_cmd} ${download_cmd}"
-    ${pycmd} ${BASE_DIR}/downloader/downloader.py ${os_cmd} ${download_cmd}
+
+    log_info "${pycmd} $(basename ${BASE_DIR})/ascend_download.py $@"
+    ${pycmd} ${BASE_DIR}/ascend_download.py $@
 }
 
 main $*
 main_status=$?
 if [[ ${main_status} != 0 ]] && [[ ${main_status} != 2 ]];then
     operation_log_info "parameter error,run failed"
 else
```

## ascend_deployer/start_download_ui.bat

```diff
@@ -1,6 +1,3 @@
-python downloader/downloader_ui.py
-if errorlevel 1 (
-    exit 0
-)
-python downloader/downloader.py
-TIMEOUT /T 20
+mode con cols=180 lines=40
+python downloader_ui.py
+pause
```

## ascend_deployer/downloader/__init__.py

```diff
@@ -19,19 +19,18 @@
 """
 
 import os
 import shutil
 import platform
 
 
-dir_list = ['downloader', 'playbooks', 'docs', 'tools']
-file_list = ['install.sh', 'start_download.sh',
-             'inventory_file', 'ansible.cfg',
-             'README.md', 'README.en.md',
-             'start_download_ui.bat', 'start_download.bat']
+dir_list = ['downloader', 'playbooks', 'tools', 'ansible_plugin', 'group_vars', 'patch', 'scripts', 'yamls']
+file_list = ['install.sh', 'inventory_file', 'ansible.cfg',
+             'README.md', 'README.en.md', '__init__.py', 'ascend_deployer.py', 'jobs.py', 'utils.py',
+             'hccn_inventory_file', 'Inventory_Template.CSV', 'MEF_README.md', 'version.json']
 CUR_DIR = os.path.dirname(__file__)
 
 
 def copy_scripts():
     """
     copy scripts from library to ASCEND_DEPLOY_HOME
     the default ASCEND_DEPLOYER_HOME is HOME
```

## ascend_deployer/downloader/config.ini

```diff
@@ -1,15 +1,9 @@
 [pypi]
 index_url=https://repo.huaweicloud.com/repository/pypi/simple
 
 [proxy]
 verify=false
 
-[download]
-os_list=CentOS_7.6_aarch64,CentOS_7.6_x86_64,CentOS_8.2_aarch64,CentOS_8.2_x86_64,Ubuntu_18.04_aarch64,Ubuntu_18.04_x86_64
-
-[software]
-pkg_list=CANN_5.1.RC2,MindStudio_5.0.RC2
-
 [python]
 ascend_python_version=Python-3.7.5
```

## ascend_deployer/downloader/deb_downloader.py

```diff
@@ -12,26 +12,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 
 import os
-import sys
 import gzip
 import re
 import sqlite3 as sqlite
-import urllib.request
-import configparser
-from urllib.error import HTTPError
-import logger_config
-from download_util import DOWNLOAD_INST
-from download_util import calc_sha256
-from downloader import get_download_path
-
+from . import logger_config
+from .download_util import DOWNLOAD_INST
+from .download_util import calc_sha256, get_download_path, CH, DownloadCheckError
 
 DOC = r"""
 ubuntu的子仓
 main:完全的自由软件。
 restricted:不完全的自由软件。
 universe:ubuntu官方不提供支持与补丁，全靠社区支持。
 muitiverse：非自由软件，完全不提供支持和补丁。
@@ -40,14 +34,15 @@
 LOG = logger_config.LOG
 
 
 class DebianSource(object):
     """
     source
     """
+
     def __init__(self, line):
         tmp = line.split(' ')
         self.url = tmp[1].strip()
         self.distro = tmp[2].strip()
         self.repoList = [i.strip() for i in tmp[3:]]
 
     def get_url(self):
@@ -66,14 +61,15 @@
             yield repo, repo_url
 
 
 class Package(object):
     """
     Package
     """
+
     def __init__(self, package, filename, sha256=None):
         self.package = package
         self.filename = filename
         self.sha256 = sha256
 
     def get_packagename(self):
         """
@@ -94,34 +90,35 @@
         return self.sha256
 
 
 class Apt(object):
     """
     downloader for apt
     """
+
     def __init__(self, source_file, arch):
         self.arch = arch
         self.binary_path = 'binary-amd64' \
             if 'x86' in self.arch else 'binary-arm64'
         # 读取源配置
         self.source_list = []
         self.base_dir = get_download_path()
         self.repo_file = os.path.join(self.base_dir, source_file)
         self.resources_dir = os.path.join(self.base_dir, 'resources')
+        self.primary_connection = sqlite.Connection(':memory:')
+        self.primary_cur = self.primary_connection.cursor()
         with open(self.repo_file) as file:
             for line in file.readlines():
                 source = DebianSource(line)
                 self.source_list.append(source)
 
     def make_cache(self):
         """
         make_cache
         """
-        self.primary_connection = sqlite.Connection(':memory:')
-        self.primary_cur = self.primary_connection.cursor()
         try:
             self.primary_cur.executescript("CREATE TABLE packages \
                     (name TEXT, version TEXT, source TEXT, repo TEXT, \
                     url TEXT, sha256 TEXT);")
         except sqlite.OperationalError as e:
             pass
         finally:
@@ -215,19 +212,19 @@
                 sha256 = line.split(': ')[1]
 
             if line.startswith("Filename:"):
                 filename = line.split(': ')[1]
 
             if len(line.strip()) == 0:
                 params = {'name': package,
-                    'version': version,
-                    'source': source_url,
-                    'repo': repo,
-                    'url': filename,
-                    'sha256': sha256}
+                          'version': version,
+                          'source': source_url,
+                          'repo': repo,
+                          'url': filename,
+                          'sha256': sha256}
                 self.primary_cur.execute("INSERT INTO \
                         PACKAGES (name, version, source, repo, url, sha256) \
                         VALUES (:name, :version, :source, :repo, :url, \
                         :sha256);", params)
 
     def download_by_url(self, pkg, dst_dir):
         """
@@ -246,23 +243,22 @@
         dst_file = os.path.join(download_dir, file_name)
 
         checksum = pkg['sha256'] if 'sha256' in pkg else None
         if checksum and not self.need_download_again(checksum, dst_file):
             print(file_name.ljust(60), 'exists')
             return True
 
-        try:
-            LOG.info('download from [%s]', url)
-            return DOWNLOAD_INST.download(url, dst_file)
-        except HTTPError as http_error:
-            print('[{0}]->{1}'.format(url, http_error))
-            LOG.error('[%s]->[%s]', url, http_error)
-            return False
-        finally:
-            pass
+        LOG.info('download from [%s]', url)
+        if DOWNLOAD_INST.download(url, dst_file):
+            if checksum and not CH.check_hash(dst_file, checksum):
+                raise DownloadCheckError(dst_file)
+            else:
+                print(file_name.ljust(60), 'download success')
+                return True
+        return False
 
     def download_by_name(self, pkg, dst_dir):
         """
         download
 
         :param name:
         :param dst_dir:
@@ -289,45 +285,41 @@
             print("can't find package {0}".format(name))
             LOG.error("can't find package %s", name)
             return False
 
         pkg_sha256 = ''
         version = results[0][0]
         url = results[0][3] + results[0][1]
-        pkg_sha256 =  results[0][2]
+        pkg_sha256 = results[0][2]
         for item in results:
             [cur_ver, cur_url, cur_sha256, cur_source, cur_repo] = item
             if not self.version_compare(version, cur_ver):
                 version = cur_ver
-                url =  cur_source + cur_url
-                pkg_sha256 =  cur_sha256
+                url = cur_source + cur_url
+                pkg_sha256 = cur_sha256
             if 'version' in pkg and pkg['version'] in cur_ver:
-                url =  cur_source + cur_url
-                pkg_sha256 =  cur_sha256
+                url = cur_source + cur_url
+                pkg_sha256 = cur_sha256
                 break
 
-        try:
-            LOG.info('[%s] download from [%s]', name, url)
-            file_name = os.path.basename(url)
-            dst_file = os.path.join(dst_dir, file_name)
-            if not self.need_download_again(pkg_sha256, dst_file):
-                LOG.info("%s no need download again", name)
-                print(name.ljust(60), 'exists')
-                return True
-            if DOWNLOAD_INST.download(url, dst_file):
-                print(name.ljust(60), 'download success')
+        LOG.info('[%s] download from [%s]', name, url)
+        file_name = os.path.basename(url)
+        dst_file = os.path.join(dst_dir, file_name)
+        if not self.need_download_again(pkg_sha256, dst_file):
+            LOG.info("%s no need download again", name)
+            print(name.ljust(60), 'exists')
+            return True
+        if DOWNLOAD_INST.download(url, dst_file):
+            if pkg_sha256 and not CH.check_hash(dst_file, pkg_sha256):
+                raise DownloadCheckError(dst_file)
+            else:
+                print(file_name.ljust(60), 'download success')
                 return True
-            print(name.ljust(60), 'download failed')
-            return False
-        except HTTPError as http_error:
-            print('[{0}]->{1}'.format(url, http_error))
-            LOG.error('[%s]->[%s]', url, http_error)
-            return False
-        finally:
-            pass
+        print(name.ljust(60), 'download failed')
+        return False
 
     def download(self, pkg, dst_dir):
         """
         download
         """
         if 'url' in pkg:
             return self.download_by_url(pkg, dst_dir)
```

## ascend_deployer/downloader/download_util.py

```diff
@@ -10,32 +10,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
-
+import ctypes
 import os
+import collections
 import configparser
 import json
 import socket
 import time
 import sys
 import hashlib
 import ssl
 import platform
 from urllib import request
-from urllib import parse
 from urllib.error import ContentTooShortError, URLError
 
-import logger_config
+from . import logger_config
+from . import software_mgr
 
 
-def get_ascend_path():
+def get_download_path():
     """
     get download path
     """
     cur_dir = os.path.dirname(__file__)
     if 'site-packages' not in cur_dir and 'dist-packages' not in cur_dir:
         cur = os.path.dirname(cur_dir)
         return cur
@@ -48,77 +49,53 @@
     else:
         deployer_home = os.getcwd()
 
     return os.path.join(deployer_home, 'ascend-deployer')
 
 
 LOG = logger_config.LOG
-CUR_DIR = get_ascend_path()
+CUR_DIR = get_download_path()
 ROOT_DIR = os.path.dirname(CUR_DIR)
 
 
 def get_support_url():
     """
     get support url
     """
     resources_json = os.path.join(CUR_DIR, 'downloader', 'support_url.json')
     with open(resources_json, 'r', encoding='utf-8') as json_file:
         data = json.load(json_file)
     return data
 
+
 class ConfigUtil:
     config_file = os.path.join(CUR_DIR, 'downloader/config.ini')
 
     def __init__(self) -> None:
         self.config = configparser.RawConfigParser()
         self.config.read(self.config_file)
 
     def get_pypi_url(self):
         return self.config.get('pypi', 'index_url')
 
     def get_proxy_verify(self):
         return self.config.getboolean('proxy', 'verify')
 
-    def get_download_os_list(self):
-        os_list = self.config.get('download', 'os_list')
-        return [x.strip() for x in os_list.split(',') if len(x.strip()) != 0]
-
-    def get_download_pkg_list(self):
-        pkg_list = self.config.get('software', 'pkg_list')
-        return [x.strip() for x in pkg_list.split(',') if len(x.strip()) != 0]
-
     def get_python_version(self):
         return self.config.get('python', 'ascend_python_version')
 
+
 CONFIG_INST = ConfigUtil()
 
 
 class ProxyUtil:
     def __init__(self) -> None:
         self.verify = CONFIG_INST.get_proxy_verify()
         self.proxy_handler = self._init_proxy_handler()
         self.https_handler = self._init_https_handler()
-    
-    @staticmethod
-    def _init_proxy_handler():
-        return request.ProxyHandler()
-
-
-    def _init_https_handler(self):
-        if not self.verify:
-            context = self.create_unverified_context()
-        else:
-            context = self.create_verified_context()
-
-        return request.HTTPSHandler(context=context)
-
-    def build_proxy_handler(self):
-        opener = request.build_opener(self.proxy_handler,
-                                      self.https_handler)
-        request.install_opener(opener)
 
     @staticmethod
     def create_unverified_context():
         context = ssl.SSLContext(ssl.PROTOCOL_TLSv1_2)
         context.verify_mode = ssl.CERT_NONE
         context.check_hostname = False
         return context
@@ -140,84 +117,130 @@
         context.options |= ssl.OP_NO_SSLv2
         context.options |= ssl.OP_NO_SSLv3
         context.options |= ssl.OP_NO_TLSv1
         context.options |= ssl.OP_NO_TLSv1_1
         context.set_ciphers(':'.join(safe_ciphers))
         return context
 
-def schedule(blocknum, blocksize, totalsize):
-    try:
-        speed = (blocknum * blocksize) / (time.time() - DownloadUtil.start_time)
-    except ZeroDivisionError as err:
-        print(err)
-        LOG.error(err)
-        raise
-    speed = float(speed) / 1024
-    speed_str = r" {:.2f} KB/s".format(speed)
-    if speed >= 1024:
-        speed_str = r" {:.2f} MB/s".format(speed / 1024)
-    recv_size = blocknum * blocksize
-    # config scheduler
-    f = sys.stdout
-    pervent = recv_size / totalsize
-    if pervent > 1:
-        pervent = 1
-    percent_str = "{:.2f}%".format(pervent * 100)
-    n = round(pervent * 50)
-    s = ('=' * (n - 1) + '>').ljust(50, '-')
-    if pervent == 1:
-        s = ('=' * n).ljust(50, '-')
-    f.write('\r' + percent_str.ljust(7, ' ') + '[' + s + ']' + speed_str.ljust(20))
-    f.flush()
+    @staticmethod
+    def _init_proxy_handler():
+        return request.ProxyHandler()
+
+    def build_proxy_handler(self):
+        opener = request.build_opener(self.proxy_handler,
+                                      self.https_handler)
+        request.install_opener(opener)
+
+    def _init_https_handler(self):
+        if not self.verify:
+            context = self.create_unverified_context()
+        else:
+            context = self.create_verified_context()
+
+        return request.HTTPSHandler(context=context)
+
+
+class DownloadError(Exception):
+    def __init__(self, url, dst_file):
+        self.url, self.dst_file = url, dst_file
+
+
+class DownloadCheckError(Exception):
+    def __init__(self, dst_file):
+        self.dst_file = dst_file
+
+
+class UrlOpenError(Exception):
+    def __init__(self, msg):
+        self.err_msg = msg
 
 
 class DownloadUtil:
     proxy_inst = ProxyUtil()
     start_time = time.time()
 
+    @staticmethod
+    def call_schedule(pkg):
+        def schedule(blocknum, blocksize, totalsize):
+            try:
+                speed = (blocknum * blocksize) / (time.time() - DownloadUtil.start_time)
+            except ZeroDivisionError as err:
+                print(err)
+                LOG.error(err)
+                raise
+            speed = float(speed) / 1024
+            speed_str = r" {:.2f} KB/s".format(speed)
+            if speed >= 1024:
+                speed_str = r" {:.2f} MB/s".format(speed / 1024)
+            recv_size = blocknum * blocksize
+            # config scheduler
+            f = sys.stdout
+            pervent = recv_size / totalsize
+            if pervent > 1:
+                pervent = 1
+            percent_str = "{:.2f}%".format(pervent * 100)
+            n = round(pervent * 50)
+            s = ('=' * (n - 1) + '>').ljust(50, '-')
+            if len(pkg) > 24:
+                pkg_str = "".join(list(pkg)[:21]) + "..."
+            elif len(pkg) < 24:
+                pkg_str = "".join(list(pkg)) + (24 - len(pkg)) * ""
+            else:
+                pkg_str = pkg
+
+            if pervent == 1:
+                s = ('=' * n).ljust(50, '-')
+            print_str = '\r' + Color.CLEAR + Color.info("start downloading ") \
+                        + pkg_str.ljust(33, ' ') + ' ' \
+                        + percent_str.ljust(7, ' ') + '[' + s + ']' + speed_str.ljust(20)
+            f.write(print_str)
+            f.flush()
+
+        return schedule
+
     @classmethod
     def download(cls, url: str, dst_file_name: str):
         parent_dir = os.path.dirname(dst_file_name)
         if not os.path.exists(parent_dir):
             LOG.info("mkdir : %s", os.path.basename(parent_dir))
             os.makedirs(parent_dir, mode=0o750, exist_ok=True)
 
         res = cls.download_with_retry(url, dst_file_name)
         if not res:
             print(url.ljust(60), 'download failed')
             LOG.error('download %s failed', url)
-            raise RuntimeError
+            raise DownloadError(url, dst_file_name)
         else:
             LOG.info('download %s successfully', url)
             return True
 
     @classmethod
     def download_with_retry(cls, url: str, dst_file_name: str, retry_times=5):
         for retry in range(1, retry_times + 1):
             try:
                 LOG.info('downloading try: %s from %s', retry, url)
                 delete_if_exist(dst_file_name)
                 cls.proxy_inst.build_proxy_handler()
                 DownloadUtil.start_time = time.time()
-                print("start downloading {}".format(url.split('/')[-1].split('#')[0]))
-                local_file, _ = request.urlretrieve(url, dst_file_name, schedule)
-                sys.stdout.write('\n')
+                pkg_name = url.split('/')[-1].split('#')[0]
+                local_file, _ = request.urlretrieve(url, dst_file_name, cls.call_schedule(pkg_name))
                 return is_exists(local_file)
-            except ContentTooShortError as ex:
+            except (ContentTooShortError, URLError, ssl.SSLError) as ex:
                 print(ex)
                 LOG.error(ex)
-            except URLError as err:
-                print(err)
-                LOG.error(err)
             except socket.timeout as timeout:
                 socket.setdefaulttimeout(retry * 60)
                 print(timeout)
                 LOG.error(timeout)
-            except ConnectionResetError as rest:
+            except ConnectionResetError as reset:
                 print('connection reset by peer, retry...')
+                LOG.error('connection reset by peer:{}, retry...'.format(reset))
+            except Exception as ex:
+                print('download failed, retry...')
+                LOG.error('download failed with err:{}, retry...'.format(ex))
             finally:
                 pass
             print('please wait for a moment...')
             LOG.info('please wait for a moment...')
             time.sleep(retry * 2)
         return False
 
@@ -264,213 +287,47 @@
             finally:
                 pass
             print('please wait for a moment...')
             LOG.info('please wait for a moment...')
             time.sleep(retry * 2)
         return False
 
-DOWNLOAD_INST = DownloadUtil()
-
-class Cann_Download:
-    browser = None
-
-    def __init__(self):
-        self.download_dir = None
 
-    @classmethod
-    def quit(cls):
-        if cls.browser:
-            cls.browser.quit()
-            cls.browser = None
-
-    def download(self, url: str, dst_file_name: str):
-        if "support.huawei" not in url:
-            return DOWNLOAD_INST.download(url, dst_file_name)
-        file_name = os.path.basename(dst_file_name)
-
-        try:
-            import selenium
-        except ImportError:
-            print("[ERROR] import selenium error, please install selenium first")
-            print(file_name.ljust(60), 'download failed')
-            LOG.error('import selenium error, download %s failed', file_name)
-            return False
-
-        try:
-            res = self.download_with_selenium(url, dst_file_name)
-        except selenium.common.exceptions.WebDriverException as err:
-            print("[ERROR] some problem has occured when runing selenium")
-            LOG.error('selenium.common.exceptions.WebDriverException: %s', err)
-            res = False
-
-        if not res:
-            print(file_name.ljust(60), 'download failed')
-            LOG.error('download %s failed', file_name)
-            return False
-        else:
-            LOG.info('download %s successfully', file_name)
-            return True
-
-    def get_firefox_driver(self):
-        import selenium
-        from selenium import webdriver
-
-        fp = webdriver.FirefoxProfile()
-        fp.set_preference("browser.download.folderList", 2)
-        fp.set_preference("browser.helperApps.alwaysAsk.force", False)
-        fp.set_preference("browser.download.manager.showAlertOnComplete", True)
-        fp.set_preference('browser.helperApps.neverAsk.saveToDisk',
-                          'application/zip,application/octet-stream,'
-                          'application/x-zip-compressed,multipart/x-zip,'
-                          'application/x-rar-com'
-                          'pressed, application/octet-stream')
-        fp.set_preference("security.ssl3.ecdhe_ecdsa_aes_128_gcm_sha256", True)
-        fp.set_preference("security.ssl3.ecdhe_ecdsa_aes_256_gcm_sha384", True)
-        fp.set_preference("security.ssl3.ecdhe_rsa_aes_128_gcm_sha256", True)
-        fp.set_preference("security.ssl3.ecdhe_rsa_aes_256_gcm_sha384", True)
-        forbiddens = [
-            'dhe_dss_aes_128_sha', 'dhe_dss_aes_256_sha', 'dhe_dss_camellia_128_sha',
-            'dhe_dss_camellia_256_sha', 'dhe_dss_des_ede3_sha', 'dhe_dss_des_sha',
-            'dhe_rsa_aes_128_sha', 'dhe_rsa_aes_256_sha', 'dhe_rsa_camellia_128_sha',
-            'dhe_rsa_camellia_256_sha', 'dhe_rsa_des_ede3_sha', 'dhe_rsa_des_sha',
-            'ecdhe_ecdsa_aes_128_sha', 'ecdhe_ecdsa_aes_256_sha', 'ecdhe_ecdsa_chacha20_poly1305_sha256',
-            'ecdhe_ecdsa_des_ede3_sha', 'ecdhe_ecdsa_null_sha', 'ecdhe_ecdsa_rc4_128_sha',
-            'ecdhe_rsa_aes_128_sha', 'ecdhe_rsa_aes_256_sha', 'ecdhe_rsa_chacha20_poly1305_sha256',
-            'ecdhe_rsa_des_ede3_sha', 'ecdhe_rsa_null_sha', 'ecdhe_rsa_rc4_128_sha',
-            'ecdh_ecdsa_aes_128_sha', 'ecdh_ecdsa_aes_256_sha', 'ecdh_ecdsa_des_ede3_sha',
-            'ecdh_ecdsa_null_sha', 'ecdh_ecdsa_rc4_128_sha', 'ecdh_rsa_aes_128_sha', 'ecdh_rsa_aes_256_sha',
-            'ecdh_rsa_des_ede3_sha', 'ecdh_rsa_null_sha', 'ecdh_rsa_rc4_128_sha', 'rsa_1024_des_cbc_sha',
-            'rsa_1024_rc4_56_sha', 'rsa_aes_128_sha', 'rsa_aes_256_sha', 'rsa_camellia_128_sha',
-            'rsa_camellia_256_sha', 'rsa_des_ede3_sha', 'rsa_des_sha', 'rsa_fips_des_ede3_sha',
-            'rsa_fips_des_sha', 'rsa_null_md5', 'rsa_null_sha', 'rsa_rc2_40_md5',
-            'rsa_rc4_40_md5', 'rsa_rc4_128_md5', 'rsa_rc4_128_sha']
-        for value in forbiddens:
-            fp.set_preference("security.ssl3.{}".format(value), False)
-
-        fp.set_preference("browser.download.dir", self.download_dir)
-        if platform.system() == 'Linux':
-            driver_path = os.path.join(ROOT_DIR, 'geckodriver')
-            if not os.path.exists(driver_path):
-                print("[ERROR] {} not exists, please check the file".format(os.path.basename(driver_path)))
-                LOG.error("{} not exists, please check the file".format(os.path.basename(driver_path)))
-                raise FileNotFoundError
-            try:
-                os.chmod(driver_path, mode=0o500)
-            except PermissionError as err:
-                print("[ERROR] {} no permission to be chmod to 500, please chown the file to the current user".format(os.path.basename(driver_path)))
-                LOG.error("{} no permission to be chmod to 500, please chown the file to the current user: {}".format(os.path.basename(driver_path), err))
-                raise PermissionError
-            try:
-                browser = webdriver.Firefox(firefox_profile=fp,
-                                            port=56003,
-                                            service_args=['--marionette-port',
-                                                          '56004'],
-                                            service_log_path='/dev/null',
-                                            executable_path=driver_path)
-            except TypeError as err:
-                print("[ERROR] mybey you should patch selenium first")
-                LOG.error("mybey you should patch selenium first: %s", err)
-                raise PermissionError
-            except selenium.common.exceptions.SessionNotCreatedException as err:
-                print("[ERROR] firefox or geckodriver is not available, please check")
-                LOG.error("firefox or geckodriver is not available: %s", err)
-                raise
-        else:
-            driver_path = os.path.join(ROOT_DIR, 'geckodriver.exe')
-            if not os.path.exists(driver_path):
-                print("[ERROR] {} not exists, please check the file".format(os.path.basename(driver_path)))
-                LOG.error("{} not exists, please check the file".format(os.path.basename(driver_path)))
-                raise FileNotFoundError
-            try:
-                browser = webdriver.Firefox(firefox_profile=fp,
-                                            service_log_path='NUL',
-                                            executable_path=driver_path)
-            except selenium.common.exceptions.SessionNotCreatedException as err:
-                print("[ERROR] firefox or geckodriver is not available, please check")
-                LOG.error("firefox or geckodriver is not available: %s", err)
-                raise
-        return browser
-
-    def login(self):
-        login_url = get_support_url().get('login_url')
-        Cann_Download.browser = self.get_firefox_driver()
-        self.browser.get(login_url)
-        count = 0
-        while Cann_Download.browser.current_url != \
-                get_support_url().get('support_site'):
-            count += 1
-            if count > 300:
-                print("[ERROR] login timeout or not logged in, please try again")
-                LOG.error("login timeout or not logged in")
-                raise ConnectionRefusedError()
-            time.sleep(1)
-
-    def download_with_selenium(self, url: str, dst_file_name: str):
-        from selenium import webdriver
-
-        file_name = os.path.basename(dst_file_name)
-        self.download_dir = os.path.dirname(dst_file_name)
-
-        if self.browser is None:
-            try:
-                self.login()
-            except (ConnectionRefusedError, FileNotFoundError, PermissionError):
-                LOG.error('download %s failed', file_name)
-                return False
-
-        delete_if_exist(dst_file_name)
-        delete_if_exist(dst_file_name + '.asc')
-        print("start downloading {}".format(file_name))
-
-        self.browser.get(url)
-        webdriver.support.wait.WebDriverWait(self.browser, 30).until(
-            lambda _driver:
-            _driver.find_element_by_partial_link_text('直接下载'))
-        self.browser.find_element_by_partial_link_text('直接下载').click()
-        if get_support_url().get('apply_right') in \
-                self.browser.current_url:
-            print("[ERROR] no permission to download, please apply for permission first")
-            LOG.error('no permission to download, download %s failed', file_name)
-            return False
-        wait_count = 1
-        for _ in range(5):
-            time.sleep(5)
-            if not os.path.exists(dst_file_name) and wait_count == 5:
-                print('[ERROR] The current network is abnormal, please ensure that the network is normal.')
-                LOG.error('[ERROR] The current network is abnormal, please ensure that the network is normal.')
-                return False
-            self.wait_download_complete(file_name)
-            if os.path.exists(dst_file_name):
-                break
-            else:
-                wait_count += 1
-        self.browser.find_element_by_partial_link_text('pgp').click()
-        self.wait_download_complete(file_name + '.asc')
-
-        return is_exists(dst_file_name) and is_exists(dst_file_name + '.asc')
-
-    def wait_download_complete(self, file_name):
-        while file_name + '.part' in \
-                [_file_name for _file_name in os.listdir(self.download_dir)]:
-            time.sleep(1)
-
-
-CANN_DOWNLOAD_INST = Cann_Download()
+DOWNLOAD_INST = DownloadUtil()
+BLOCKSIZE = 1024 * 1024 * 100
 
 
 def calc_sha256(file_path):
     hash_val = None
     if file_path is None or not os.path.exists(file_path):
         return hash_val
     with open(file_path, 'rb') as hash_file:
         sha256_obj = hashlib.sha256()
-        sha256_obj.update(hash_file.read())
+        buf = hash_file.read(BLOCKSIZE)
+        while len(buf) > 0:
+            sha256_obj.update(buf)
+            buf = hash_file.read(BLOCKSIZE)
         hash_val = sha256_obj.hexdigest()
     return hash_val
 
+
+def calc_md5(file_path):
+    md5_val = None
+    if file_path is None or not os.path.exists(file_path):
+        return md5_val
+    with open(file_path, 'rb') as md5_file:
+        md5_obj = hashlib.md5()
+        buf = md5_file.read(BLOCKSIZE)
+        while len(buf) > 0:
+            md5_obj.update(buf)
+            buf = md5_file.read(BLOCKSIZE)
+        hash_val = md5_obj.hexdigest()
+    return hash_val
+
+
 def get_specified_python():
     if os.environ.get("ASCEND_PYTHON_VERSION"):
         specified_python = os.environ.get("ASCEND_PYTHON_VERSION")
     else:
         specified_python = CONFIG_INST.get_python_version()
     resources_json = os.path.join(CUR_DIR, 'downloader', 'python_version.json')
     with open(resources_json, 'r', encoding='utf-8') as json_file:
@@ -479,29 +336,32 @@
         if specified_python not in available_python_list:
             tips = "[ERROR] ascend_python_version is not available, available Python-x.x.x is in 3.7.0~3.7.11 and 3.8.0~3.8.11 and 3.9.0~3.9.9"
             print(tips)
             LOG.error(tips)
             sys.exit(1)
     return specified_python
 
+
 def delete_if_exist(dst_file_name: str):
     if os.path.exists(dst_file_name):
         LOG.info('{} already exists'.format(os.path.basename(dst_file_name)))
         os.remove(dst_file_name)
         LOG.info('{} already deleted'.format(os.path.basename(dst_file_name)))
 
+
 def is_exists(dst_file_name: str):
     if os.path.exists(dst_file_name):
         LOG.info('{} exists after downloading, success'.format(os.path.basename(dst_file_name)))
         return True
     else:
         print('[ERROR] {} not exists after downloading, failed'.format(os.path.basename(dst_file_name)))
         LOG.info('{} not exists after downloading, failed'.format(os.path.basename(dst_file_name)))
         return False
 
+
 def get_arch(os_list):
     """
     根据os_list判断需要下载哪些架构的包
     """
     arm, x86 = 0, 0
     for os_item in os_list:
         if not arm and "aarch64" in os_item:
@@ -515,7 +375,146 @@
         arch = "aarch64"
     elif not arm and x86:
         arch = "x86_64"
     else:
         arch = ("x86_64", "aarch64")
 
     return arch
+
+
+class CheckHash:
+    @classmethod
+    def check_hash(cls, dst_file, sha256):
+        """
+        check_hash
+        校验下载文件的hash值与给定hash值是否相等
+
+        :param dst_file: 下载文件文件
+        :param sha256:  hash
+        :return:
+        """
+        file_hash = calc_sha256(dst_file)
+        return sha256 == file_hash
+
+    @classmethod
+    def check_download_hash(cls, dst_file, url_with_hash):
+        """
+        check_download_hash
+        校验下载文件的hash值与url中的hash值是否相等
+
+        :param dst_file: 下载文件文件
+        :param url_with_hash:  带hash值的URL
+        :return:
+        """
+        if 'sha256=' in url_with_hash:
+            key_word = 'sha256='
+            file_hash = calc_sha256(dst_file)
+        else:
+            key_word = 'md5='
+            file_hash = calc_md5(dst_file)
+        index_of_hash = str(url_with_hash).index(key_word) + len(key_word)
+        target_hash = url_with_hash[index_of_hash:]
+        return target_hash == file_hash
+
+
+CH = CheckHash()
+
+
+class State(object):
+    NONE = 0
+    EXIT = 1
+    ASK = 2
+
+
+class Color:
+    RED = '\033[31m'
+    BLUE = '\033[32m'
+    END = '\033[0m'
+    YELLOW = '\033[93m'
+    CLEAR = '\033[K'
+
+    @classmethod
+    def info(cls, msg):
+        return cls.BLUE + msg + cls.END
+
+    @classmethod
+    def warn(cls, msg):
+        return cls.YELLOW + msg + cls.END
+
+    @classmethod
+    def error(cls, msg):
+        return cls.RED + msg + cls.END
+
+
+def check_version_matched(os_list, pkg_list):
+    """
+    check version matched between CANN and MindSpore
+    :param pkg_list:download package list
+    :return:err_with_exit msg, err_with_ask msg
+    """
+    item_counter = collections.defaultdict(int)
+    version_dict = collections.defaultdict(lambda: "")
+    for pkg_item in pkg_list:
+        for item in ("DL", "MindSpore", "MindStudio", "Torch-npu", "CANN", "MEF"):
+            if item not in pkg_item:
+                continue
+            name_version = get_name_version(pkg_item)
+            item_counter[item] += 1
+            version_dict[item] = name_version
+            if item_counter.get(item, 0) > 1:
+                return State.EXIT, "Only one {} is allowed, Please reselect and try again".format(item)
+
+    warning_messages = ''
+    for name, version in version_dict.items():
+        if "CANN" not in version:
+            warning_messages += check_cann_matching(version_dict.get("CANN", ""), version)
+    versions = [v.split("_")[1] for k, v in version_dict.items() if k in ["DL", "MEF"]]
+    for version in versions:
+        support_os_list = os.listdir(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), f'dependency/{version}/COMMON'))
+
+        not_support_list = [i for i in os_list if i.replace('==', '_') not in support_os_list]
+        if not_support_list:
+            if item_counter.get('DL', 0) > 0:
+                return State.EXIT, "ascend-deployer do not support install DL on {}".format(not_support_list)
+            elif item_counter.get('MEF', 0) > 0:
+                return State.EXIT, "ascend-deployer do not support install MEF on {}".format(not_support_list)
+    if warning_messages:
+        return State.ASK, warning_messages
+
+    return State.NONE, ""
+
+
+def check_cann_matching(cann_version, name_version):
+    warning_message = ""
+    version_match_json = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'version_match.json')
+    with open(version_match_json, 'r', encoding='utf-8') as json_file:
+        version_match_data = json.load(json_file)
+    matching_cann = version_match_data.get(name_version)
+    if matching_cann != cann_version and name_version not in version_match_data.get("NoneMatched", []):
+        warning_message = "{} need matching {}".format(name_version, matching_cann)
+    return warning_message
+
+
+def get_name_version(pkg_item):
+    name_version = pkg_item
+    if pkg_item and '==' not in pkg_item and '_' not in pkg_item:
+        name, version = software_mgr.get_software_name_version(pkg_item)
+        name_version = name + '_' + version
+        print('version of {} not selected, use {} as default'.format(pkg_item, name_version))
+    return name_version.replace('==', '_')
+
+
+def get_free_space_b(folder):
+    """
+    get the free space of 'folder' in windows or linux
+    :param folder:the path to get space
+    :return:bites of space size
+    """
+    if platform.system().lower() == 'windows':
+        free_bytes = ctypes.c_ulonglong(0)
+        ctypes.windll.kernel32.GetDiskFreeSpaceExW(ctypes.c_wchar_p(folder), None, None, ctypes.pointer(free_bytes))
+        return free_bytes.value
+    else:
+        st = os.statvfs(folder)
+        return st.f_bavail * st.f_frsize
+
```

## ascend_deployer/downloader/downloader.py

```diff
@@ -14,101 +14,275 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 """downloader"""
 import glob
 import os
 import sys
-import shutil
 import argparse
-import platform
+from functools import wraps
+from io import StringIO
+
+from . import download_util
+from . import logger_config
+from . import pip_downloader
+from . import os_dep_downloader
+from . import other_downloader
+from . import software_mgr
+from . import dl_mef_dependency_downloader
+from . import deb_downloader
+from . import rpm_downloader
+from .download_util import get_download_path, State, Color, get_free_space_b
 
 FILE_PATH = os.path.realpath(__file__)
 CUR_DIR = os.path.dirname(__file__)
 
-sys.path.append(CUR_DIR)
-
-import download_util
-import logger_config
-import pip_downloader
-import os_dep_downloader
-import other_downloader
-import software_mgr
-
-
 LOG = logger_config.LOG
 LOG_OPERATION = logger_config.LOG_OPERATION
+MAX_DOWNLOAD_SIZE = 20 * (2 ** 30)
 
 
-def download_other_packages(dst=None):
-    """
-    download other resources, such as source code tar ball
-    """
-    return other_downloader.download_other_packages(dst)
-
-
-def download_specified_python(dst=None):
-    """
-    download ascend_python_version=Python-3.7.5
-    """
-    return other_downloader.download_specified_python(dst)
-
-
-def download_other_software(os_list=None, software_list=None, dst=None):
-    """
-    download other resources, such as CANN and MindStudio
-    """
-    if software_list is None and dst is None:
-        return other_downloader.download_pkg_from_json()
-    else:
+class DependencyDownload(object):
+    def __init__(self, os_list, software_list, download_path, check):
+        self.origin_download = None
+        self.origin_cann_download = None
+        self.progress = 0
+        self.download_items = []
+        self.dst = download_util.get_download_path()
+        self.res_dir = os.path.join(self.dst, "resources")
+        self.finished_items = []
+        self.extra_schedule = None
+        self.origin_check_download_hash = None
+        self.origin_check_hash = None
+        self.origin_print = print
+        self.software_list = software_list
+        self.download_path = download_path
+        if check:
+            self.check_software_list(os_list, software_list)
+        if os.name == 'nt':
+            os.system('chcp 65001')
+            os.system('cls')
+
+    @staticmethod
+    def check_space(download_path):
+        free_size = get_free_space_b(download_path)
+        if free_size < MAX_DOWNLOAD_SIZE:
+            print(Color.warn("[WARN] the disk space of {} is less than {:.2f}GB".format(download_path,
+                                                                                        MAX_DOWNLOAD_SIZE / (
+                                                                                                1024 ** 3))))
+
+    @staticmethod
+    def check_software_list(os_list, software_list):
+        """
+        check the download software list
+        :param os_list: download os list
+        :param software_list: download software list
+        """
+        check_stat, msg = download_util.check_version_matched(os_list, software_list)
+        if check_stat == State.EXIT:
+            print("[ERROR] {}".format(msg))
+            LOG.error("[ERROR] {}".format(msg))
+            sys.exit(1)
+        if check_stat == State.ASK:
+            print("[WARN] {}".format(msg))
+            while True:
+                answer = input("need to force download or not?(y/n)")
+                if answer in {'y', 'yes'}:
+                    print("Versions do not match, force download.")
+                    LOG.info("Versions do not match, force download.")
+                    break
+                elif answer in {'n', 'no'}:
+                    print("Versions do not match, exit.")
+                    LOG.info("Versions do not match, exit.")
+                    sys.exit(0)
+                else:
+                    print("Invalid input, please re-enter!")
+
+    @staticmethod
+    def process_bar(blocknum, blocksize, totalsize):
+        recv_size = blocknum * blocksize
+        # config scheduler
+        f = sys.stdout
+        pervent = recv_size / totalsize
+        if pervent > 1:
+            pervent = 1
+        percent_str = "{:.2f}%".format(pervent * 100)
+        n = round(pervent * 50)
+        s = ('=' * (n - 1) + '>').ljust(50, '-')
+        if pervent == 1:
+            s = ('=' * n).ljust(50, '-')
+        f.write('\r' + Color.info('All Download Progress:').ljust(61, ' ') +
+                percent_str.ljust(7, ' ') + '[' + s + ']')
+        f.flush()
+
+    @staticmethod
+    def download_other_packages(os_list, dst=None):
+        """
+        download other resources, such as source code tar ball
+        """
+        return other_downloader.download_other_packages(os_list, dst)
+
+    @staticmethod
+    def download_specified_python(dst=None):
+        """
+        download ascend_python_version=Python-3.7.5
+        """
+        return other_downloader.download_specified_python(dst)
+
+    @staticmethod
+    def download_other_software(os_list, software_list, dst):
+        """
+        download other resources, such as CANN and MindStudio
+        """
         return other_downloader.download(os_list, software_list, dst)
 
-
-def download_python_packages(os_list=None, res_dir=None):
-    """
-    download_python_packages
-    """
-    if os_list is None and res_dir is None:
-        return pip_downloader.download_from_json()
-    else:
+    @staticmethod
+    def download_python_packages(os_list, res_dir):
+        """
+        download_python_packages
+        """
         return pip_downloader.download(os_list, res_dir)
 
-
-def download_mindspore(os_list=None, software_list=None, dst=None):
-    """
-    download_mindspore
-    """
-    if software_list is None and dst is None:
-        return other_downloader.download_ms_from_json()
-    else:
+    @staticmethod
+    def download_mindspore(os_list, software_list, dst):
+        """
+        download_mindspore
+        """
         return other_downloader.download_ms(os_list, software_list, dst)
 
-
-def download_os_packages(os_list=None, software_list=None, dst=None):
-    """
-    download_os_packages
-    """
-    os_dep = os_dep_downloader.OsDepDownloader()
-    if os_list is None and dst is None:
-        return os_dep.download_pkg_from_json()
-    else:
+    @staticmethod
+    def download_torch_npu(os_list, software_list, dst):
+        """
+        download_torch_npu
+        """
+        return other_downloader.download_torch_npu(os_list, software_list, dst)
+
+    @staticmethod
+    def download_os_packages(os_list, software_list, dst):
+        """
+        download_os_packages
+        """
+        os_dep = os_dep_downloader.OsDepDownloader()
         return os_dep.download(os_list, software_list, dst)
 
-
-def download_all(os_list, software_list, dst):
-    """
-    download all resources for specific os list
-    """
-    res_dir = os.path.join(dst, "resources")
-    download_specified_python(dst)
-    download_python_packages(os_list, res_dir)
-    download_mindspore(os_list, software_list, dst)
-    download_os_packages(os_list, software_list, res_dir)
-    download_other_packages(dst)
-    download_other_software(os_list, software_list, dst)
+    @staticmethod
+    def download_dl_mef_resources(os_list, software_list, dst):
+        """
+        download_dl_mef_resources
+        """
+        for pkg_name in software_list:
+            if "DL" in pkg_name or "MEF" in pkg_name:
+                return dl_mef_dependency_downloader.download_dl_mef_dependency(os_list, software_list, dst)
+        return {'ok': [], 'failed': []}
+
+    @staticmethod
+    def cursor_down():
+        sys.stdout.write('\n')
+        sys.stdout.flush()
+
+    @staticmethod
+    def cursor_up():
+        sys.stdout.write('\x1b[1A')
+        sys.stdout.flush()
+
+    def mock_print(self, *args, **kwargs):
+        # deal args with xxxErr
+        if len(args) == 1 and not isinstance(*args, str):
+            return print("\r", *args, **kwargs, end='')
+        str_args = '\r' + Color.CLEAR + ''.join(list(args))
+        return print(str_args, **kwargs, end='')
+
+    def mock_download(self, *args, **kwargs):
+        # mock other_downloader.DOWNLOAD_INST.download
+        if args[1].endswith(".xml") or args[1].endswith("sqlite.bz2") or args[1].endswith("sqlite.xz"):
+            self.download_items.append(args[0])
+            return self.origin_download(*args, **kwargs)
+        self.download_items.append(args[0])
+        return True
+
+    def mock_check_hash(self, *args, **kwargs):
+        return True
+
+    def collect_info(self, *args):
+        self.check_space(self.download_path)
+        msg = Color.info('start analyzing the amount of packages to be downloaded ...')
+        self.origin_print(msg)
+        LOG.info(msg, extra=logger_config.LOG_CONF.EXTRA)
+        self.origin_download = other_downloader.DOWNLOAD_INST.download
+        other_downloader.DOWNLOAD_INST.download = self.mock_download
+        self.origin_check_download_hash = download_util.CH.check_download_hash
+        download_util.CH.check_download_hash = self.mock_check_hash
+        self.origin_check_hash = download_util.CH.check_hash
+        download_util.CH.check_hash = self.mock_check_hash
+
+        other_downloader.print = self.mock_print
+        pip_downloader.print = self.mock_print
+        download_util.print = self.mock_print
+        os_dep_downloader.print = self.mock_print
+        deb_downloader.print = self.mock_print
+        rpm_downloader.print = self.mock_print
+        dl_mef_dependency_downloader.print = self.mock_print
+        origin_output = sys.stdout
+        sys.stdout = StringIO()
+        LOG.disabled = True
+        pip_downloader.LOG.disabled = True
+        os_dep_downloader.LOG.disabled = True
+        deb_downloader.LOG.disabled = True
+        rpm_downloader.LOG.disabled = True
+        other_downloader.LOG.disabled = True
+        dl_mef_dependency_downloader.LOG.disabled = True
+        try:
+            self.download_all(*args)
+        except Exception as e:
+            raise e
+        finally:
+            sys.stdout = origin_output
+            LOG.disabled = False
+            pip_downloader.LOG.disabled = False
+            os_dep_downloader.LOG.disabled = False
+            deb_downloader.LOG.disabled = False
+            rpm_downloader.LOG.disabled = False
+            other_downloader.LOG.disabled = False
+            dl_mef_dependency_downloader.LOG.disabled = False
+
+            print = self.origin_print
+            download_util.CH.check_download_hash = self.origin_check_download_hash
+            download_util.CH.check_hash = self.origin_check_hash
+            pip_downloader.my_pip.downloaded = []
+            other_downloader.DOWNLOAD_INST.download = self.counter(self.origin_download)
+        msg = f'finish analyzing ...'
+        print(msg)
+        LOG.info(msg, extra=logger_config.LOG_CONF.EXTRA)
+
+    def counter(self, f):
+        @wraps(f)
+        def wrap(*args, **kwargs):
+            try:
+                return f(*args, **kwargs)
+            finally:
+                self.finished_items.append(args[0])
+                self.cursor_down()
+                self.process_bar(len(set(self.finished_items)), 1, len(set(self.download_items)))
+                self.cursor_up()
+
+        return wrap
+
+    def download_all(self, os_list, software_list, dst):
+        """
+        download all resources
+        """
+        res_dir = os.path.join(dst, "resources")
+        self.download_specified_python(dst)
+        self.download_python_packages(os_list, res_dir)
+        self.download_mindspore(os_list, software_list, dst)
+        self.download_torch_npu(os_list, software_list, dst)
+        self.download_os_packages(os_list, software_list, res_dir)
+        self.download_other_packages(os_list, dst)
+        self.download_other_software(os_list, software_list, dst)
+        self.download_dl_mef_resources(os_list, software_list, dst)
 
 
 def parse_argument(download_path):
     """
     解析参数
     """
     support_os_list = os.listdir(os.path.join(download_path, 'downloader', 'config'))
@@ -122,37 +296,32 @@
         pkg_name, version = pkg.split('_')
         download_help += '{}=={}\n'.format(pkg_name, version[:-5])
 
     parser = argparse.ArgumentParser(
         epilog="  notes: When <Version> is missing, <PK> is the latest.\r\n",
         formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('--os-list', action='store', dest='os_list',
-            help=os_list_help)
+                        help=os_list_help)
     parser.add_argument('--download', action='store', dest='packages',
-            help=download_help)
+                        help=download_help)
 
     try:
         args = parser.parse_args()
     except SystemExit as e:
         if e.code == 0:
             sys.exit(0)
         else:
             sys.exit(1)
 
     if args.os_list is None and args.packages is None:
         parser.print_help()
         sys.exit(0)
 
-    if args.os_list is None and "MindSpore" in args.packages:
-        print("os_list can not be none when downloading mindspore")
-        parser.print_help()
-        sys.exit(0)
-    
-    if args.os_list is None and "MindStudio" in args.packages:
-        print("os_list can not be none when downloading MindStudio")
+    if args.os_list is None or args.packages is None:
+        print("os_list or packages can not be none")
         parser.print_help()
         sys.exit(0)
 
     if args.os_list is not None:
         for os_item in args.os_list.split(','):
             if os_item not in support_os_list:
                 print('os {} is not supported'.format(os_item))
@@ -164,32 +333,14 @@
                 print('software {} is not supported'.format(soft))
                 parser.print_help()
                 sys.exit(1)
 
     return args
 
 
-def get_download_path():
-    """
-    get download path
-    """
-    if 'site-packages' not in CUR_DIR and 'dist-packages' not in CUR_DIR:
-        cur = os.path.dirname(FILE_PATH)
-        return os.path.dirname(cur)
-
-    deployer_home = ''
-    if platform.system() == 'Linux':
-        deployer_home = os.getenv('HOME')
-        if os.getenv('ASCEND_DEPLOYER_HOME') is not None:
-            deployer_home = os.getenv('ASCEND_DEPLOYER_HOME')
-    else:
-        deployer_home = os.getcwd()
-    return os.path.join(deployer_home, 'ascend-deployer')
-
-
 def delete_glibc(os_list, download_path):
     delete_os_list = ['Kylin_V10Tercel_aarch64', 'Kylin_V10Tercel_x86_64']
     for i in delete_os_list:
         if i in os_list:
             os_dir = os.path.join(download_path, 'resources', i)
             glibc = glob.glob('{}/glibc-[0-9]*'.format(os_dir))
             try:
@@ -219,51 +370,47 @@
 
     os_list = []
     if args.os_list is not None:
         os_list = args.os_list.split(',')
     software_list = []
     if args.packages is not None:
         software_list = args.packages.split(',')
+    download_dependency(os_list, software_list, download_path, args.force_download)
+
+
+def download_dependency(os_list, software_list, download_path, check):
+    download_status = "Failed"
+    err_log = ""
+    dependency_download = DependencyDownload(os_list, software_list, download_path, check)
     try:
-        download_all(os_list, software_list, download_path)
+        dependency_download.collect_info(os_list, software_list, download_path)
+        dependency_download.download_all(os_list, software_list, download_path)
     except (KeyboardInterrupt, SystemExit):
         download_status = "Failed"
-        exit_status = 1
-    except Exception:
+        err_log = Color.error("download failed,keyboard interrupt or system exit,please check.")
+    except download_util.DownloadError as e:
+        download_status = "Failed"
+        err_log = Color.error("download failed,download from {} to {} failed".format(e.url, e.dst_file))
+    except download_util.DownloadCheckError as e:
+        download_status = "Failed"
+        err_log = Color.error("{} download verification failed".format(e.dst_file))
+    except Exception as e:
         download_status = "Failed"
-        exit_status = 1
+        err_log = Color.error("download failed with error {} ,please retry.".format(e))
     else:
         download_status = "Success"
-        exit_status = 0
+        err_log = ""
     finally:
-        log_msg = "downloading --os-list={} --download={}: {}".format(
-            args.os_list, args.packages, download_status)
+        download_result = "\ndownload and check --os_list={} --download={}:{}".format(",".join(os_list),
+                                                                                      ",".join(software_list),
+                                                                                      download_status)
+        if download_status == "Success":
+            log_msg = "\n" + err_log + download_result
+        else:
+            log_msg = "\n\n" + err_log + download_result
+        print(log_msg)
         LOG_OPERATION.info(log_msg, extra=logger_config.LOG_CONF.EXTRA)
         delete_glibc(os_list, download_path)
-        sys.exit(exit_status)
 
 
 if __name__ == "__main__":
-    if len(sys.argv) == 1:
-        _download_status = "Failed"
-        try:
-            download_specified_python()
-            download_python_packages()
-            download_mindspore()
-            download_os_packages()
-            download_other_packages()
-            download_other_software()
-        except (KeyboardInterrupt, SystemExit):
-            _download_status = "Failed"
-        except Exception:
-            _download_status = "Failed"
-        else:
-            _download_status = "Success"
-        finally:
-            _log_msg = "downloading --os-list={} --download={}: {}".format(
-                ",".join(download_util.CONFIG_INST.get_download_os_list()),
-                ",".join(download_util.CONFIG_INST.get_download_pkg_list()),
-                _download_status)
-            LOG_OPERATION.info(_log_msg, extra=logger_config.LOG_CONF.EXTRA)
-            delete_glibc(download_util.CONFIG_INST.get_download_os_list(), get_download_path())
-    else:
-        main()
+    main()
```

## ascend_deployer/downloader/os_dep_downloader.py

```diff
@@ -11,58 +11,56 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 """download os dependencies"""
 import json
 import os
-import sys
-import time
 
-from deb_downloader import Apt
-from rpm_downloader import Yum
-from download_util import CONFIG_INST
-import logger_config
-import software_mgr
-from downloader import get_download_path
+from .deb_downloader import Apt
+from .rpm_downloader import Yum
+from . import logger_config
+from . import software_mgr
+from .download_util import get_download_path
 
 LOG = logger_config.LOG
 
 
 class OsDepDownloader:
     def __init__(self):
-        self.os_list = CONFIG_INST.get_download_os_list()
-        self.pkg_list = CONFIG_INST.get_download_pkg_list()
         self.project_dir = get_download_path()
         self.resources_dir = os.path.join(self.project_dir, 'resources')
 
     def download(self, os_list, software_list, dst):
         results = {}
         mindstudio_list = [software for software in software_list if "MindStudio" in software]
         for os_item in os_list:
             res = self.download_os(os_item, mindstudio_list, dst)
             results[os_item] = res
         return results
 
-    def download_pkg_from_json(self):
-        results = {}
-        software_list = [software.replace("_", "==") for software in self.pkg_list if "MindStudio" in software]
-        for os_item in self.os_list:
-            res = self.download_os(os_item, software_list, self.resources_dir)
-            results[os_item] = res
-        return results
-
     def download_os(self, os_item, software_list, dst):
         """
         download os packages. debs or rpms
         :param os_itme:  Ubuntu_18.04_aarch64, CentOS_8.2_x86_64..
         """
+        docker_pkg_list = [
+            "docker-ce-cli",
+            "containerd.io",
+            "docker-ce",
+            "docker-ce-rootless-extras",
+            "docker-scan-plugin",
+            "docker-engine",
+        ]
         dst_dir = os.path.join(dst, os_item)
         if not os.path.exists(dst_dir):
             os.makedirs(dst_dir, mode=0o750, exist_ok=True)
+        docker_dir = os.path.join(dst_dir, 'docker')
+        if not os.path.exists(docker_dir):
+            os.makedirs(docker_dir, mode=0o750, exist_ok=True)
         LOG.info('item:{} save dir: {}'.format(os_item, os.path.basename(dst_dir)))
 
         config_file = os.path.join(self.project_dir, 'downloader/config/{0}/pkg_info.json'.format(os_item))
         source_list_file = os.path.join(self.project_dir, 'downloader/config/{0}/source.list'.format(os_item))
         downloader = None
 
         if os.path.exists(source_list_file):
@@ -73,38 +71,42 @@
         else:
             source_repo_file = os.path.join(self.project_dir, 'downloader/config/{0}/source.repo'.format(os_item))
             if 'aarch64' in os_item:
                 downloader = Yum(source_repo_file, 'aarch64')
             else:
                 downloader = Yum(source_repo_file, 'x86_64')
 
-        res = {'ok': [], 'failed':[]}
+        res = {'ok': [], 'failed': []}
         if downloader is not None:
             if downloader.make_cache() is False:
                 LOG.error('downloader make_cache failed')
-                res['failed'].append(os_item)
+                res.get('failed', []).append(os_item)
                 raise RuntimeError
 
         with open(config_file, 'r', encoding='utf-8') as f:
             data = json.load(f)
             for item in data:
+                if item['name'] in docker_pkg_list:
+                    dst_dir = docker_dir
+                else:
+                    dst_dir = os.path.join(dst, os_item)
                 if downloader.download(item, dst_dir):
-                    res['ok'].append(item['name'])
+                    res.get('ok', []).append(item['name'])
                     continue
                 print('download failed', item['name'])
-                res['failed'].append(item['name'])
+                res.get('failed', []).append(item['name'])
                 raise RuntimeError
 
         for software in software_list:
             formal_name, version = software_mgr.get_software_name_version(software)
             pkg_list = software_mgr.get_software_sys(formal_name, os_item, version)
             soft_dst_dir = os.path.join(dst, "{0}_{1}".format(formal_name, version), os_item)
             for pkg in pkg_list:
                 if downloader.download(pkg, soft_dst_dir):
-                    res['ok'].append(pkg['name'])
+                    res.get('ok', []).append(pkg['name'])
                     continue
                 print('download failed', pkg['name'])
-                res['failed'].append(pkg['name'])
+                res.get('failed', []).append(pkg['name'])
                 raise RuntimeError
         if downloader is not None:
             downloader.clean_cache()
         return res
```

## ascend_deployer/downloader/other_downloader.py

```diff
@@ -11,73 +11,80 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 
-import configparser
 import json
 import os
-import shutil
 import time
-from download_util import calc_sha256, get_arch, get_specified_python, CONFIG_INST, DOWNLOAD_INST, CANN_DOWNLOAD_INST
-import logger_config
-from software_mgr import get_software_name_version, get_software_other, get_software_mindspore
+from .download_util import calc_sha256, get_arch, get_specified_python,\
+    DOWNLOAD_INST, CH, DownloadCheckError
+from . import logger_config
+from .software_mgr import get_software_name_version, get_software_other, get_software_mindspore, get_software_torch_npu
 
 LOG = logger_config.LOG
 CUR_DIR = os.path.dirname(os.path.realpath(__file__))
 PROJECT_DIR = os.path.dirname(CUR_DIR)
-PKG_LIST = CONFIG_INST.get_download_pkg_list()
-OS_LIST = CONFIG_INST.get_download_os_list()
 
 
 def download_software(software, dst, arch):
     """
     下载软件的其他资源
     """
     formal_name, version = get_software_name_version(software)
     others = get_software_other(formal_name, version)
     download_dir = os.path.join(dst, "resources", "{0}_{1}".format(formal_name, version))
-
-    if not os.path.exists(download_dir):
-        os.makedirs(download_dir, mode=0o750, exist_ok=True)
-    LOG.info('item:{} save dir: {}'.format(software, os.path.basename(download_dir)))
+    if "DL" not in download_dir and "MEF" not in download_dir:
+        if not os.path.exists(download_dir):
+            os.makedirs(download_dir, mode=0o750, exist_ok=True)
+        LOG.info('item:{} save dir: {}'.format(software, os.path.basename(download_dir)))
     results = []
     if formal_name == "CANN":
         if arch == "x86_64" or arch == "aarch64":
-            others = (item for item in others if arch in item['filename'].replace('-','_'))
+            others = (
+                item
+                for item in others
+                if arch in item["filename"].replace("-", "_")
+                   or "kernels" in item["filename"]
+            )
         try:
             for item in others:
                 dest_file = os.path.join(download_dir, item['filename'])
                 if os.path.exists(dest_file) and 'sha256' in item:
                     file_hash = calc_sha256(dest_file)
                     if file_hash == item['sha256']:
                         print(item['filename'].ljust(60), 'exists')
                         LOG.info('{0} no need download again'.format(item['filename']))
                         continue
-                ret = CANN_DOWNLOAD_INST.download(item['url'], dest_file)
+                ret = DOWNLOAD_INST.download(item['url'], dest_file)
                 if ret:
+                    if 'sha256' in item and not CH.check_hash(dest_file, item['sha256']):
+                        LOG.info('the downloaded file：{} hash is not equal to the hash in file'.format(dest_file))
+                        raise DownloadCheckError(dest_file)
                     print(item['filename'].ljust(60), 'download success')
                 results.append(ret)
         finally:
             while '.part' in ','.join(os.listdir(download_dir)):
                 time.sleep(1)
-            CANN_DOWNLOAD_INST.quit()
     else:
         for item in others:
             dest_file = os.path.join(download_dir, item['filename'])
             if os.path.exists(dest_file) and 'sha256' in item:
                 file_hash = calc_sha256(dest_file)
                 if file_hash == item['sha256']:
                     print(item['filename'].ljust(60), 'exists')
                     LOG.info('{0} no need download again'.format(item['filename']))
                     continue
             ret = DOWNLOAD_INST.download(item['url'], dest_file)
             if ret:
+                if 'sha256' in item and not CH.check_hash(dest_file, item['sha256']):
+                    LOG.info('the downloaded file：{} hash is not equal to the hash in file'.format(dest_file))
+                    raise DownloadCheckError(dest_file)
                 print(item['filename'].ljust(60), 'download success')
             results.append(ret)
     return all(results)
 
 
 def download(os_list, software_list, dst):
     """
@@ -85,71 +92,66 @@
     """
     if os_list is None:
         os_list = []
     arch = get_arch(os_list)
     LOG.info('software arch is {0}'.format(arch))
 
     results = {'ok': [], 'failed': []}
-    no_mindspore_list = [software for software in software_list if "MindSpore" not in software]
-    for software in no_mindspore_list:
-        res = download_software(software, dst, arch)
-        if res:
-            results['ok'].append(software)
-            continue
-        results['failed'].append(software)
-    return results
-
-
-def download_pkg_from_json():
-    """
-    按config.ini下载其他部分
-    """
-    arch = get_arch(OS_LIST)
-    LOG.info('software arch is {0}'.format(arch))
-
-    results = {'ok': [], 'failed': []}
-    software_list = [software.replace("_", "==") for software in PKG_LIST if "MindSpore" not in software]
+    no_frame_list = []
     for software in software_list:
-        res = download_software(software, PROJECT_DIR, arch)
+        if "MindSpore" not in software and "Torch-npu" not in software:
+            no_frame_list.append(software)
+    for software in no_frame_list:
+        res = download_software(software, dst, arch)
         if res:
-            results['ok'].append(software)
+            results.get('ok', []).append(software)
             continue
-        results['failed'].append(software)
+        results.get('failed', []).append(software)
     return results
 
 
-def download_other_packages(dst=None):
+def download_other_packages(os_list, dst=None):
     """
     download_other_packages
 
     :return:
     """
     if dst is None:
         base_dir = PROJECT_DIR
     else:
         base_dir = dst
+    arch = get_arch(os_list)
     resources_json = os.path.join(CUR_DIR, 'other_resources.json')
     results = {'ok': [], 'failed': []}
     with open(resources_json, 'r', encoding='utf-8') as json_file:
         data = json.load(json_file)
         for item in data:
             dest_file = os.path.join(base_dir, item['dest'], item['filename'])
             if os.path.exists(dest_file) and 'sha256' in item:
                 file_hash = calc_sha256(dest_file)
                 url_hash = item['sha256']
                 if file_hash == url_hash:
                     print(item['filename'].ljust(60), 'exists')
                     LOG.info('{0} no need download again'.format(item['filename']))
                     continue
+            if 'nexus' in item['filename']:
+                if arch == "x86_64" and arch not in item['filename']:
+                    continue
+                if arch == "aarch64" and arch not in item['filename']:
+                    continue
             LOG.info('download[{0}] -> [{1}]'.format(item['url'], os.path.basename(dest_file)))
             if DOWNLOAD_INST.download(item['url'], dest_file):
-                results['ok'].append(item['filename'])
-                print(item['filename'].ljust(60), 'download success')
-                continue
-            results['failed'].append(item['filename'])
+                if not CH.check_hash(dest_file, item['sha256']):
+                    results.get('failed', []).append(item['filename'])
+                    raise DownloadCheckError(dest_file)
+                else:
+                    results.get('ok', []).append(item['filename'])
+                    print(item['filename'].ljust(60), 'download success')
+                    continue
+            results.get('failed', []).append(item['filename'])
     return results
 
 
 def download_specified_python(dst=None):
     """
     download ascend_python_version=Python-3.7.5
 
@@ -172,28 +174,32 @@
                     url_hash = item['sha256']
                     if file_hash == url_hash:
                         print(item['filename'].ljust(60), 'exists')
                         LOG.info('{0} no need download again'.format(item['filename']))
                         break
                 LOG.info('download[{0}] -> [{1}]'.format(item['url'], os.path.basename(dest_file)))
                 if DOWNLOAD_INST.download(item['url'], dest_file):
-                    results['ok'].append(item['filename'])
-                    print(item['filename'].ljust(60), 'download success')
-                    break
-                results['failed'].append(item['filename'])
+                    if not CH.check_hash(dest_file, item['sha256']):
+                        results.get('failed', []).append(item['filename'])
+                        raise DownloadCheckError(dest_file)
+                    else:
+                        results.get('ok', []).append(item['filename'])
+                        print(item['filename'].ljust(60), 'download success')
+                        break
+                results.get('failed', []).append(item['filename'])
                 break
         return results
 
 
 def download_ms_whl(os_item, software, dst):
     """
     下载软件的其他资源
     """
     formal_name, version = get_software_name_version(software)
-    download_dir = os.path.join(dst, "resources", "{}".format(os_item))
+    download_dir = os.path.join(dst, "resources", "pylibs")
     results = []
     os_item_split = os_item.split("_")
     os_name, arch = "_".join(os_item_split[:2]), "_".join(os_item_split[2:])
     specified_python = get_specified_python()
     implement_flag = "cp37"
     if "Python-3.7" in specified_python:
         implement_flag = "cp37"
@@ -202,101 +208,129 @@
     if "Python-3.9" in specified_python:
         implement_flag = "cp39"
 
     whl_list = get_software_mindspore(formal_name, "linux_cpu_{}".format(arch), version)
     for item in whl_list:
         if item.get('python', 'cp37') != implement_flag:
             print("Try to get {} on {}, but it does not match {}".format
-            (item['filename'], item.get('python'), implement_flag))
+                  (item['filename'], item.get('python'), implement_flag))
             continue
         dest_file = os.path.join(download_dir, "CPU", os.path.basename(item['url']))
         if os.path.exists(dest_file) and 'sha256' in item:
             file_hash = calc_sha256(dest_file)
             url_hash = item['sha256']
             if file_hash == url_hash:
                 print(item['filename'].ljust(60), 'exists')
                 LOG.info('{0} no need download again'.format(item['filename']))
                 continue
             else:
                 LOG.info('{0} need download again'.format(item['filename']))
         ret = DOWNLOAD_INST.download(item['url'], dest_file)
         if ret:
+            if 'sha256' in item and not CH.check_hash(dest_file, item['sha256']):
+                LOG.info('the downloaded file：{} hash is not equal to the hash in file'.format(dest_file))
+                raise DownloadCheckError(dest_file)
             print(item['filename'].ljust(60), 'download success')
         results.append(ret)
-    
+
     whl_list = get_software_mindspore(formal_name, "linux_{}".format(arch), version)
     for item in whl_list:
         if item.get('python', 'cp37') != implement_flag:
             print("Try to get {} on {}, but it does not match {}".format
-            (item['filename'], item.get('python'), implement_flag))
+                  (item['filename'], item.get('python'), implement_flag))
             continue
-        dest_file = os.path.join(download_dir, "Ascend910", os.path.basename(item['url']))
+        dest_file = os.path.join(download_dir, "Ascend", os.path.basename(item['url']))
         if os.path.exists(dest_file) and 'sha256' in item:
             file_hash = calc_sha256(dest_file)
             url_hash = item['sha256']
             if file_hash == url_hash:
                 print(item['filename'].ljust(60), 'exists')
                 LOG.info('{0} no need download again'.format(item['filename']))
                 continue
             else:
                 LOG.info('{0} need download again'.format(item['filename']))
         ret = DOWNLOAD_INST.download(item['url'], dest_file)
         if ret:
+            if 'sha256' in item and not CH.check_hash(dest_file, item['sha256']):
+                LOG.info('the downloaded file：{} hash is not equal to the hash in file'.format(dest_file))
+                raise DownloadCheckError(dest_file)
             print(item['filename'].ljust(60), 'download success')
         results.append(ret)
-    
+
+    return all(results)
+
+
+def download_torch_npu_whl(os_item, software, dst):
+    """
+    下载软件的其他资源
+    """
+    formal_name, version = get_software_name_version(software)
+    download_dir = os.path.join(dst, "resources", "pylibs")
+    results = []
+    os_item_split = os_item.split("_")
+    os_name, arch = "_".join(os_item_split[:2]), "_".join(os_item_split[2:])
+    specified_python = get_specified_python()
+    implement_flag = "cp37"
+    if "Python-3.7" in specified_python:
+        implement_flag = "cp37"
+    if "Python-3.8" in specified_python:
+        implement_flag = "cp38"
+    if "Python-3.9" in specified_python:
+        implement_flag = "cp39"
+
+    whl_list = get_software_torch_npu(formal_name, "linux_{}".format(arch), version)
     for item in whl_list:
         if item.get('python', 'cp37') != implement_flag:
             print("Try to get {} on {}, but it does not match {}".format
-            (item['filename'], item.get('python'), implement_flag))
+                  (item['filename'], item.get('python'), implement_flag))
             continue
-        A910_dest_file = os.path.join(download_dir, "Ascend910", os.path.basename(item['url']))
-        if os.path.exists(A910_dest_file) and os_name in ["Ubuntu_18.04","Ubuntu_22.04", "CentOS_7.6", "EulerOS_2.8", "EulerOS_2.10", "OpenEuler_22.03LTS"]:
-            dest_file = os.path.join(download_dir, "Ascend310", os.path.basename(item['url']))
-            if os.path.exists(dest_file) and 'sha256' in item:
-                file_hash = calc_sha256(dest_file)
-                url_hash = item['sha256']
-                if file_hash == url_hash:
-                    LOG.info('{0} exist, no need copy again'.format(os.path.basename(dest_file)))
-                else:
-                    LOG.info('{0} exist but not completed, need copy again'.format(os.path.basename(dest_file)))
-                    os.remove(dest_file)
-                    shutil.copy(A910_dest_file, dest_file)
+        dest_file = os.path.join(download_dir, os.path.basename(item['url']))
+        if os.path.exists(dest_file) and 'sha256' in item:
+            file_hash = calc_sha256(dest_file)
+            url_hash = item['sha256']
+            if file_hash == url_hash:
+                print(item['filename'].ljust(60), 'exists')
+                LOG.info('{0} no need download again'.format(item['filename']))
+                continue
             else:
-                parent_dir = os.path.dirname(dest_file)
-                if not os.path.exists(parent_dir):
-                    os.makedirs(parent_dir, mode=0o750, exist_ok=True)
-                LOG.info('{0} not exist, copy from Ascend910'.format(os.path.basename(dest_file)))
-                shutil.copy(A910_dest_file, dest_file)
+                LOG.info('{0} need download again'.format(item['filename']))
+        ret = DOWNLOAD_INST.download(item['url'], dest_file)
+        if ret:
+            if 'sha256' in item and not CH.check_hash(dest_file, item['sha256']):
+                LOG.info('the downloaded file：{} hash is not equal to the hash in file'.format(dest_file))
+                raise DownloadCheckError(dest_file)
+            print(item['filename'].ljust(60), 'download success')
+        results.append(ret)
+
     return all(results)
 
 
 def download_ms(os_list, software_list, dst):
     """
     按传参下载mindspore
     """
     results = {'ok': [], 'failed': []}
     mindspore_list = [software for software in software_list if "MindSpore" in software]
     for os_item in os_list:
         for software in mindspore_list:
             res = download_ms_whl(os_item, software, dst)
             if res:
-                results['ok'].append(software)
+                results.get('ok', []).append(software)
                 continue
-            results['failed'].append(software)
+            results.get('failed', []).append(software)
     return results
 
 
-def download_ms_from_json():
+def download_torch_npu(os_list, software_list, dst):
     """
-    按config.ini下载mindspore
+    按传参下载torch_npu
     """
     results = {'ok': [], 'failed': []}
-    software_list = [software.replace("_", "==") for software in PKG_LIST if "MindSpore" in software]
-    for os_item in OS_LIST:
-        for software in software_list:
-            res = download_ms_whl(os_item, software, PROJECT_DIR)
+    torch_npu_list = [software for software in software_list if "Torch-npu" in software]
+    for os_item in os_list:
+        for software in torch_npu_list:
+            res = download_torch_npu_whl(os_item, software, dst)
             if res:
-                results['ok'].append(software)
+                results.get('ok', []).append(software)
                 continue
-            results['failed'].append(software)
+            results.get('failed', []).append(software)
     return results
```

## ascend_deployer/downloader/other_resources.json

### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {'insert': "[(1, OrderedDict([('filename', 'nexus_3.53.1_aarch64.tar'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.cn-east-2.myhuaweicloud.com/MindXDL/5.0.RC1/resources/nexus_3.53.1_aarch64.tar'), "*

 * *           "('sha256', '37d2b5c5acd46454528a769fba9e6c4cc6bc459bc3127d75cd0c9c35fc70af6c'), "*

 * *           "('dest', 'resources/nexus')])), (2, OrderedDict([('filename', "*

 * *           "'nexus_3.53.1_x86_64.tar'), ('url', "*

 * *           "'https://ascend-repo-modelzoo.obs.cn-east-2.myhuaweicloud.com/MindXD […]*

```diff
@@ -2,14 +2,26 @@
     {
         "dest": "resources/sources",
         "filename": "protobuf-python-3.13.0.tar.gz",
         "sha256": "9c4d2ad449d27da5ac1db1ad5ecc4a642dedd6bbe59219d61d7b655b6b12be89",
         "url": "https://mindx.obs.cn-south-1.myhuaweicloud.com/opensource/protobuf-python-3.13.0.tar.gz"
     },
     {
+        "dest": "resources/nexus",
+        "filename": "nexus_3.53.1_aarch64.tar",
+        "sha256": "37d2b5c5acd46454528a769fba9e6c4cc6bc459bc3127d75cd0c9c35fc70af6c",
+        "url": "https://ascend-repo-modelzoo.obs.cn-east-2.myhuaweicloud.com/MindXDL/5.0.RC1/resources/nexus_3.53.1_aarch64.tar"
+    },
+    {
+        "dest": "resources/nexus",
+        "filename": "nexus_3.53.1_x86_64.tar",
+        "sha256": "0251113556c924ffca3b14711c5b866202d78df9c3301da824ff0bf99c9d5424",
+        "url": "https://ascend-repo-modelzoo.obs.cn-east-2.myhuaweicloud.com/MindXDL/5.0.RC1/resources/nexus_3.53.1_x86_64.tar"
+    },
+    {
         "dest": "resources/sources",
         "filename": "gcc-7.3.0.tar.gz",
         "sha256": "fa06e455ca198ddc11ea4ddf2a394cf7cfb66aa7e0ab98cc1184189f1d405870",
         "url": "https://mirrors.huaweicloud.com/gnu/gcc/gcc-7.3.0/gcc-7.3.0.tar.gz"
     },
     {
         "dest": "resources/sources",
```

## ascend_deployer/downloader/pip_downloader.py

```diff
@@ -11,31 +11,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 
-import os
-import urllib.request
 import http.client
+import os
+import json
 import time
 from html.parser import HTMLParser
-from download_util import CONFIG_INST, DOWNLOAD_INST
-from download_util import calc_sha256, get_arch, get_specified_python
-import logger_config
 
+from . import logger_config
+from .download_util import CONFIG_INST, DOWNLOAD_INST
+from .download_util import calc_sha256, get_arch, get_specified_python, CH, DownloadCheckError, UrlOpenError
 
 LOG = logger_config.LOG
 
 
 class SimpleIndexParser(HTMLParser):
     """
     解析simple index
     """
+
     def __init__(self):
         super().__init__()
         self.index = {}
         self.tmp_attrs = None
 
     def get_index(self):
         """
@@ -60,21 +61,23 @@
             self.index[data] = self.tmp_attrs[0][1]
 
 
 class MyPip(object):
     """
     downloader for pip
     """
+
     def __init__(self):
         self.cache = {}
         self.downloaded = []
         # 读取配置
         script = os.path.realpath(__file__)
         self.pypi_url = CONFIG_INST.get_pypi_url()
         self.require_file = os.path.join(os.path.dirname(script), 'requirements.txt')
+        self.obs_resources_file = os.path.join(os.path.dirname(script), 'obs_resources.json')
         self.repo_path = os.path.join(os.path.dirname(script), '../resources/pylibs')
 
     @staticmethod
     def file_download(url, dest):
         """
         file_download
 
@@ -131,28 +134,29 @@
         """
         if distribution in self.cache.keys():
             index = self.cache.get(distribution)
         else:
             url = '{0}/{1}/'.format(self.pypi_url, distribution.lower())
             LOG.info('pypi URL = [{0}]'.format(url))
             index = ''
+            resp = None
             for retry in [x + 1 for x in range(5)]:
-                success = False
                 try:
                     resp = DOWNLOAD_INST.urlopen(url)
-                    index = resp.read()
-                    success = True
                 except http.client.HTTPException as e:
                     print(e)
                     LOG.error(e)
                     time.sleep(2 * retry)
                 finally:
                     pass
-                if success:
+                if resp:
                     break
+            if not resp:
+                raise UrlOpenError("url open failed,please check the network")
+            index = resp.read()
             self.cache[distribution] = index
 
         parser = SimpleIndexParser()
         parser.feed(index.decode())
         idx = parser.get_index()
         return idx
 
@@ -193,35 +197,71 @@
                 if version in name:
                     pkg = name
                     url = href
             else:
                 continue
         return pkg, url
 
+    def get_url_from_obs(self, name, platform, implement):
+        if platform == 'none':
+            return "", ""
+        distribution, version = name.split('==')
+        with open(self.obs_resources_file) as file_content:
+            index = json.load(file_content)
+            for file_name, href in index.items():
+                elements = file_name.split('-')
+                try:
+                    wheel_name = elements[0]
+                    wheel_version = elements[1].split('+')[0]
+                    wheel_impl = elements[2]
+                    wheel_platform = elements[4].split('.')[0]
+                except IndexError as err:
+                    print(err)
+                    LOG.error(err)
+                if wheel_name != distribution:
+                    continue
+                if wheel_version != version:
+                    continue
+                if wheel_impl not in ('py3', 'py2.py3', implement):
+                    continue
+                if wheel_platform not in ('any', platform):
+                    continue
+                return file_name, href
+            return "", ""
+
     def download_wheel(self, name, platform, implement, dest_path):
         """
         下载软件包
         """
+        # get url from pypi
         distribution, version = name.split('==')
         index = self.get_simple_index(distribution)
         file_name, url = self.wheel_filter(index, version, platform, implement)
         if len(url) == 0:
-            LOG.info('can not find {0} for {1} {2}'.format(name, platform, implement))
-            return False
+            # get url from obs
+            file_name, download_url = self.get_url_from_obs(name, platform, implement)
+            if not download_url:
+                LOG.info('can not find {0} for {1} {2}'.format(name, platform, implement))
+                return False
+        else:
+            download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
+
         if file_name in self.downloaded:
             return
-        download_url = '{0}/{1}/{2}'.format(self.pypi_url, distribution, url)
         LOG.info("Download {0} from [{1}]".format(file_name, download_url))
         file_path = os.path.join(dest_path, file_name)
-        if not self.need_download_again(file_path, url):
+        if not self.need_download_again(file_path, download_url):
             print(file_name.ljust(60), "exists")
             LOG.info('{0} no need download again'.format(file_name))
             self.downloaded.append(file_name)
             return True
         self.file_download(download_url, file_path)
+        if not CH.check_download_hash(file_path, download_url):
+            LOG.info('the downloaded file：{} hash is not equal to the hash in the url'.format(file_path))
+            raise DownloadCheckError(file_path)
         print(file_name.ljust(60), "download success")
         self.downloaded.append(file_name)
         return True
 
     def download_source(self, name, dest_path):
         """
         下载源码包
@@ -238,14 +278,17 @@
         file_path = os.path.join(dest_path, file_name)
         if not self.need_download_again(file_path, url):
             print(file_name.ljust(60), "exists")
             LOG.info('{0} no need download again'.format(file_name))
             self.downloaded.append(file_name)
             return True
         self.file_download(download_url, file_path)
+        if not CH.check_download_hash(file_path, url):
+            LOG.info('the downloaded file：{} hash is not equal to the hash in the url'.format(file_path))
+            raise DownloadCheckError(file_path)
         print(file_name.ljust(60), "download success")
         self.downloaded.append(file_name)
         return True
 
     @staticmethod
     def need_download_again(dst_file, url_with_hash):
         """
@@ -269,27 +312,27 @@
         else:
             return True
 
         index_of_hash = str(url_with_hash).index(key_word) + len(key_word)
         target_hash = url_with_hash[index_of_hash:]
         if target_hash != file_hash:
             LOG.info('hash {0} in url: {1} != file: {2}'.format(key_word,
-                target_hash, file_hash))
+                                                                target_hash, file_hash))
         return target_hash != file_hash
 
     def download_x86(self, name, implement_flag, dest_path):
         """
         download_x86
 
         :param name:
         :param implement_flag:
         :param dest_path:
         :return:
         """
-        platform_list = ('manylinux1_x86_64', 'manylinux2010_x86_64',
+        platform_list = ('linux_x86_64', 'manylinux1_x86_64', 'manylinux2010_x86_64',
                          'manylinux2014_x86_64')
         for platform in platform_list:
             if self.download_wheel(name, platform, implement_flag, dest_path):
                 return True
         return False
 
     def download_arm(self, name, implement_flag, dest_path):
@@ -297,16 +340,19 @@
         download_arm
 
         :param name:
         :param implement_flag:
         :param dest_path:
         :return:
         """
-        platform = 'manylinux2014_aarch64'
-        return self.download_wheel(name, platform, implement_flag, dest_path)
+        platform_list = ('linux_aarch64', 'manylinux_2_17_aarch64', 'manylinux2014_aarch64')
+        for platform in platform_list:
+            if self.download_wheel(name, platform, implement_flag, dest_path):
+                return True
+        return False
 
     def download(self, name, dest_path, arch):
         """
         download
 
         :param name:
         :param dest_path:
@@ -354,30 +400,11 @@
     LOG.info('pip arch is {0}'.format(arch))
 
     results = {'ok': [], 'failed': []}
     with open(my_pip.require_file) as file_content:
         for line in file_content:
             LOG.info('[{0}]'.format(line.strip()))
             if my_pip.download(line.strip(), repo_path, arch):
-                results['ok'].append(line.strip())
-                continue
-            results['failed'].append(line.strip())
-    return results
-
-
-def download_from_json():
-    """
-    按config.ini下载其他部分
-    """
-    arch = get_arch(CONFIG_INST.get_download_os_list())
-    repo_path = my_pip.repo_path
-    LOG.info('pip arch is {0}'.format(arch))
-
-    results = {'ok': [], 'failed': []}
-    with open(my_pip.require_file) as file_content:
-        for line in file_content:
-            LOG.info('[{0}]'.format(line.strip()))
-            if my_pip.download(line.strip(), repo_path, arch):
-                results['ok'].append(line.strip())
+                results.get('ok', []).append(line.strip())
                 continue
-            results['failed'].append(line.strip())
+            results.get('failed', []).append(line.strip())
     return results
```

## ascend_deployer/downloader/requirements.txt

```diff
@@ -55,15 +55,15 @@
 packaging==20.9
 pandas==1.1.5
 pathlib2==2.3.5
 Pillow==8.0.1
 pip==20.3.3
 pkgconfig==1.5.1
 protobuf==3.13.0
-psutil==5.8.0
+psutil==5.9.4
 pyasn1-modules==0.2.8
 pyasn1==0.4.8
 pycparser==2.20
 pylint==2.7.2
 pyparsing==2.4.7
 PyQt5-sip==12.8.1
 PyQt5==5.14.0
@@ -79,16 +79,16 @@
 setuptools==50.3.2
 six==1.15.0
 sympy==1.4
 tensorboard-plugin-wit==1.8.0
 tensorboard==1.15.0
 tensorboard==2.6.0
 tensorboard-data-server==0.6.1
-tensorflow-cpu==1.15.0
-tensorflow-cpu==2.6.5
+tensorflow==1.15.0
+tensorflow==2.6.5
 tensorflow-estimator==1.15.1
 tensorflow-estimator==2.6.0
 termcolor==1.1.0
 toml==0.10.2
 typed-ast==1.4.2
 typing-extensions==3.7.4.3
 urllib3==1.25.11
```

## ascend_deployer/downloader/rpm_downloader.py

```diff
@@ -11,34 +11,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 
-import urllib.request
 import configparser
 import os
 import gzip
 import bz2
 import shutil
 import sqlite3
 import lzma
 import xml.sax
 from xml.dom import minidom
 from urllib.error import HTTPError
 
-import logger_config
-from download_util import DOWNLOAD_INST
-from download_util import calc_sha256
-from yum_metadata.gen_yum_metadata import YumMetadataSqlite
-from yum_metadata.gen_yum_metadata import YumPackageHandler
-from yum_metadata.gen_yum_metadata import Require
-from yum_metadata.gen_yum_metadata import Provide
-from downloader import get_download_path
+from . import logger_config
+from .download_util import DOWNLOAD_INST
+from .download_util import calc_sha256
+from .yum_metadata.gen_yum_metadata import YumMetadataSqlite
+from .yum_metadata.gen_yum_metadata import YumPackageHandler
+from .yum_metadata.gen_yum_metadata import Require
+from .download_util import get_download_path
 
 LOG = logger_config.LOG
 
 try:
     from urlparse import urljoin
 except ImportError:
     from urllib.parse import urljoin
@@ -93,15 +91,14 @@
         config.read(self.repo_file)
 
 
         self.config_dir = os.path.join(self.base_dir,
                                       os.path.dirname(source_file))
         self.db_tmps = os.path.join(self.config_dir, "db_tmps")
         self.installed_file = os.path.join(self.config_dir, 'installed.txt')
-        print('repofile={} cache={}'.format(self.repo_file, self.db_tmps))
         LOG.info('repofile={} cache={}'.format(self.repo_file, self.db_tmps))
         self.clean_cache()
         self.sources = {}
         for item in config.keys():
             if 'DEFAULT' == item:
                 continue
             self.sources[item] = config.get(item, 'baseurl')
```

## ascend_deployer/downloader/software_mgr.py

```diff
@@ -16,27 +16,28 @@
 # ===========================================================================
 """software manager,管理可选下载的软件"""
 import json
 import os
 
 CUR_DIR = os.path.dirname(__file__)
 g_software_list = set()
-sys_software_list, ms_software_list, other_software_list = ([] for _ in range(3))
+sys_software_list, ms_software_list, torch_npu_software_list, other_software_list = ([] for _ in range(4))
 
 
 class Software(object):
     """
     软件类，用于存储软件信息
     """
     def __init__(self, name, default=False):
         self.name = name
         self.default = default
         self.sys_pkgs = {}
         self.other_pkgs = {}
         self.mindspore = {}
+        self.torch_npu = {}
         self.version = ""
 
     def __lt__(self, other):
         return self.version < other.version
 
     def get_name(self):
         """
@@ -79,21 +80,33 @@
     def get_mindspore(self, sys_name):
         """
         get mindspore
         """
         if sys_name not in self.mindspore:
             return []
         return self.mindspore[sys_name]
+    
+    def get_torch_npu(self, sys_name):
+        """
+        get torch_npu
+        """
+        return self.torch_npu.get(sys_name, [])
 
     def set_mindspore(self, sys_name, pkg_list):
         """
         set mindspore
         """
         self.mindspore[sys_name] = pkg_list
 
+    def set_torch_npu(self, sys_name, pkg_list):
+        """
+        set torch_npu
+        """
+        self.torch_npu[sys_name] = pkg_list
+
     def get_other_pkgs(self):
         """
         get other dependencies
         """
         return self.other_pkgs
 
     def set_other_pkgs(self, pkg_list):
@@ -115,14 +128,18 @@
             for sys_obj in json_obj['systems']:
                 soft.set_sys_pkgs(sys_obj['system'], sys_obj['sys'])
             sys_software_list.append(soft)
         if 'mindspore' in json_obj:
             for sys_obj in json_obj['mindspore']:
                 soft.set_mindspore(sys_obj['system'], sys_obj['whl'])
             ms_software_list.append(soft)
+        if 'torch-npu' in json_obj:
+            for sys_obj in json_obj['torch-npu']:
+                soft.set_torch_npu(sys_obj['system'], sys_obj['whl'])
+            torch_npu_software_list.append(soft)
         if 'other' in json_obj:
             soft.set_other_pkgs(json_obj['other'])
             other_software_list.append(soft)
 
 
 def software_init():
     """
@@ -130,15 +147,15 @@
     """
     soft_dir = os.path.join(CUR_DIR, 'software')
     for _, _, files in os.walk(soft_dir):
         for file_name in files:
             if file_name.endswith('json'):
                 load_software(os.path.join(CUR_DIR, 'software', file_name))
     global g_software_list
-    g_software_list = set(sys_software_list + ms_software_list + other_software_list)
+    g_software_list = set(sys_software_list + ms_software_list + torch_npu_software_list + other_software_list)
 
 
 def get_software_name_version(software):
     """
     获取软件依包的正式名和版本号
     :param in:  software      软件名,可能带==<version>
     :return:   正式名和版本号。例如 CANN==20.2.RC1->CANN,20.2.RC1; MindStudio==2.0.0->MindStudio,2.0.0
@@ -194,14 +211,34 @@
                 return soft.get_mindspore(sys_name)
         else:
             if soft.get_name().lower() == name.lower() and soft.get_version() == version:
                 return soft.get_mindspore(sys_name)
     return []
 
 
+def get_software_torch_npu(name, sys_name, version=None):
+    """
+    获取软件依赖的操作系统依赖
+    :param in:  name      软件名
+    :param in:  sys_name  操作系统
+    :param in:  version   软件版本
+    :return:   软件name在操作系统sys_name下的mindspore whl
+    """
+    if len(g_software_list) == 0:
+        software_init()
+    for soft in torch_npu_software_list:
+        if version is None:
+            if soft.get_name().lower() == name.lower():
+                return soft.get_torch_npu(sys_name)
+        else:
+            if soft.get_name().lower() == name.lower() and soft.get_version() == version:
+                return soft.get_torch_npu(sys_name)
+    return []
+
+
 def get_software_other(name, version=None):
     """
     获取软件的其他依赖项
     :param in:  name      软件名
     :param in:  version   软件版本
     :return:   安装软件name所需要下载的其他内容列表
     """
```

## ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8040123456790125%*

 * *Differences: {'0': "{'name': 'kernel-headers'}",*

 * * 'insert': "[(83, OrderedDict([('name', 'e2fsprogs'), ('used_by', ['driver', 'cann', "*

 * *           "'framework'])])), (84, OrderedDict([('name', 'e2fsprogs-libs'), ('used_by', ['driver', "*

 * *           "'cann', 'framework'])])), (85, OrderedDict([('name', 'libselinux-utils'), ('used_by', "*

 * *           "['driver', 'cann', 'framework'])])), (86, OrderedDict([('name', 'libss'), ('used_by', "*

 * *           "['driver', 'cann', 'framework'])])), (87, OrderedDict([('name', 'xz'), ('use […]*

```diff
@@ -1,10 +1,10 @@
 [
     {
-        "name": "kernel-headers-3.10.0-957.el7.x86_64.rpm",
+        "name": "kernel-headers",
         "sha256": "26a4011aec80fb6cd37fec1817db1fe58697286e7f23cb839e8877a0a5771207",
         "url": "https://mirrors.bfsu.edu.cn/centos-vault/7.6.1810/os/x86_64/Packages/kernel-headers-3.10.0-957.el7.x86_64.rpm"
     },
     {
         "name": "openssl",
         "sha256": "0ea161cbcbbf5db609bb4d7524750c0a6e57dc279282aa021aabf63a7cc63e79",
         "url": "https://mirrors.huaweicloud.com/centos-vault/8.2.2004/BaseOS/x86_64/os/Packages/openssl-1.1.1c-15.el8.x86_64.rpm"
@@ -648,14 +648,145 @@
         "used_by": [
             "driver",
             "cann",
             "framework"
         ]
     },
     {
+        "name": "e2fsprogs",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "e2fsprogs-libs",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "libselinux-utils",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "libss",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "xz",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "xz-libs",
+        "used_by": [
+            "driver",
+            "cann",
+            "framework"
+        ]
+    },
+    {
+        "name": "audit-libs-python",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "checkpolicy",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "container-selinux",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "fuse-overlayfs",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "fuse3-libs",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "libsemanage-python",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "policycoreutils-python",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "python-IPy",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "setools-libs",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "audit",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "audit-libs",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "policycoreutils",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "libcgroup",
+        "used_by": [
+            "docker"
+        ]
+    },
+    {
+        "name": "slirp4netns",
+        "sha256": "b98eb2c09940f8fb40405c0fd310bfa2ebc8f2e5e2711df564b35db06d027286",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/slirp4netns-0.4.3-4.el7_8.x86_64.rpm"
+    },
+    {
         "name": "docker-ce-cli",
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "containerd.io",
         "release": "3.1.el7",
@@ -666,9 +797,14 @@
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "docker-ce",
         "release": "3.el7",
         "version": "20.10.8"
+    },
+    {
+        "name": "docker-scan-plugin",
+        "release": "3.el7",
+        "version": "0.23.0"
     }
 ]
```

## ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo

```diff
@@ -1,8 +1,14 @@
+[extra]
+baseurl=https://mirrors.huaweicloud.com/centos/7/extras/x86_64/
+
 [base]
 baseurl=https://mirrors.huaweicloud.com/centos/7/os/x86_64/
 
 [epel]
 baseurl=https://mirrors.huaweicloud.com/epel/7/x86_64/
 
+[update]
+baseurl=https://mirrors.huaweicloud.com/centos/7/updates/x86_64/
+
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/x86_64/stable/
```

## ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-[base]
-baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/
-
-[docker-ce]
-baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/aarch64/stable/
+[base]
+baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/aarch64/
+
+[docker-ce]
+baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/aarch64/stable/
```

## ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.6578947368421053%*

 * *Differences: {'insert': "[(20, OrderedDict([('name', 'container-selinux'), ('autodependency', 'true'), ('info', "*

 * *           "'docker need')])), (21, OrderedDict([('name', 'python2-audit'), ('autodependency', "*

 * *           "'true'), ('info', 'docker need')])), (22, OrderedDict([('name', 'python2-enum34'), "*

 * *           "('autodependency', 'true'), ('info', 'docker need')])), (23, OrderedDict([('name', "*

 * *           "'python2-libselinux'), ('autodependency', 'true'), ('info', 'docker need')])), (24, "*

 * *           "OrderedDic […]*

```diff
@@ -88,19 +88,79 @@
     },
     {
         "autodependency": "true",
         "info": "used for mindspore",
         "name": "gmp-c++"
     },
     {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "container-selinux"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-audit"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-enum34"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-libselinux"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-libsemanage"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-policycoreutils"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "checkpolicy"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-IPy"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "python2-setools"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "libcgroup"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "fuse-overlayfs"
+    },
+    {
         "name": "sshpass",
         "sha256": "d30541c4470226e2e6708198692f6e62e9435d5b48d0240f089dce7230fc5a49",
         "url": "https://dl.fedoraproject.org/pub/archive/epel/8.5.2022-05-10/Everything/x86_64/Packages/s/sshpass-1.06-9.el8.x86_64.rpm"
     },
     {
+        "name": "slirp4netns",
+        "sha256": "b98eb2c09940f8fb40405c0fd310bfa2ebc8f2e5e2711df564b35db06d027286",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/slirp4netns-0.4.3-4.el7_8.x86_64.rpm"
+    },
+    {
         "name": "docker-ce-cli",
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "containerd.io",
         "release": "3.1.el7",
@@ -111,9 +171,14 @@
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "docker-ce-rootless-extras",
         "release": "3.el7",
         "version": "20.10.8"
+    },
+    {
+        "name": "docker-scan-plugin",
+        "release": "3.el7",
+        "version": "0.23.0"
     }
 ]
```

## ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo

```diff
@@ -1,5 +1,14 @@
+[extra]
+baseurl=https://mirrors.huaweicloud.com/centos/7/extras/x86_64/
+
 [base]
 baseurl = https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/OS/x86_64/
 
+[everything]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/everything/x86_64/
+
+[update]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-20.03-LTS/update/x86_64/
+
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/x86_64/stable/
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.4067796610169492%*

 * *Differences: {'insert': "[(20, OrderedDict([('name', 'bzip2'), ('autodependency', 'true')])), (21, "*

 * *           "OrderedDict([('name', 'cpp'), ('autodependency', 'true')])), (22, "*

 * *           "OrderedDict([('name', 'libgcc'), ('autodependency', 'true')])), (23, "*

 * *           "OrderedDict([('name', 'libgomp'), ('autodependency', 'true')])), (24, "*

 * *           "OrderedDict([('name', 'libstdc++'), ('autodependency', 'true')])), (25, "*

 * *           "OrderedDict([('name', 'openssh-clients'), ('autodependency', 'true')])), (26, " […]*

```diff
@@ -89,14 +89,134 @@
     },
     {
         "name": "sshpass",
         "sha256": "cbab3b56cd6ba1cc6608fd5a4fb15360be879602fc8c6d79cac195c752c95188",
         "url": "https://repo.openeuler.org/openEuler-22.03-LTS/everything/aarch64/Packages/sshpass-1.09-1.oe2203.aarch64.rpm"
     },
     {
+        "autodependency": "true",
+        "name": "bzip2"
+    },
+    {
+        "autodependency": "true",
+        "name": "cpp"
+    },
+    {
+        "autodependency": "true",
+        "name": "libgcc"
+    },
+    {
+        "autodependency": "true",
+        "name": "libgomp"
+    },
+    {
+        "autodependency": "true",
+        "name": "libstdc++"
+    },
+    {
+        "autodependency": "true",
+        "name": "openssh-clients"
+    },
+    {
+        "autodependency": "true",
+        "name": "openssh-server"
+    },
+    {
+        "autodependency": "true",
+        "name": "openssl"
+    },
+    {
+        "autodependency": "true",
+        "name": "openssl-libs"
+    },
+    {
+        "autodependency": "true",
+        "name": "sqlite"
+    },
+    {
+        "autodependency": "true",
+        "name": "xz"
+    },
+    {
+        "autodependency": "true",
+        "name": "zlib"
+    },
+    {
+        "autodependency": "true",
+        "name": "cmake-data"
+    },
+    {
+        "autodependency": "true",
+        "name": "cmake-filesystem"
+    },
+    {
+        "autodependency": "true",
+        "name": "cmake-rpm-macros"
+    },
+    {
+        "autodependency": "true",
+        "name": "e2fsprogs-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "emacs-filesystem"
+    },
+    {
+        "autodependency": "true",
+        "name": "gcc-gfortran"
+    },
+    {
+        "autodependency": "true",
+        "name": "jsoncpp"
+    },
+    {
+        "autodependency": "true",
+        "name": "keyutils-libs-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "krb5-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libaec-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libgfortran"
+    },
+    {
+        "autodependency": "true",
+        "name": "libquadmath"
+    },
+    {
+        "autodependency": "true",
+        "name": "libquadmath-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libselinux-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libsepol-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libstdc++-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "libverto-devel"
+    },
+    {
+        "autodependency": "true",
+        "name": "pcre2-devel"
+    },
+    {
         "name": "docker-ce-cli",
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "containerd.io",
         "release": "3.1.el7",
@@ -107,9 +227,33 @@
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "docker-ce-rootless-extras",
         "release": "3.el7",
         "version": "20.10.8"
+    },
+    {
+        "autodependency": "true",
+        "name": "fuse-overlayfs"
+    },
+    {
+        "name": "slirp4netns",
+        "sha256": "c3d964fa9cb020cee2efdce3688ef075734b14bf1dd6fde036117d1914d23c3a",
+        "url": "https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/Packages/slirp4netns-0.4.3-4.el7_8.aarch64.rpm"
+    },
+    {
+        "name": "container-selinux",
+        "sha256": "48de427ad3fb67f3b6998701340eafe1f610fbd587e8bd4e639124fe4d3f86d4",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/everything/x86_64/Packages/container-selinux-2.138-4.oe2203.noarch.rpm"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "fuse3"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "libcgroup"
     }
 ]
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo

```diff
@@ -1,5 +1,14 @@
+[extra]
+baseurl=https://mirrors.huaweicloud.com/centos-altarch/7/extras/aarch64/
+
 [base]
 baseurl = https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/OS/aarch64/
 
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/aarch64/stable/
+
+[everything]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/everything/aarch64/
+
+[update]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/update/aarch64/
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8275862068965517%*

 * *Differences: {'insert': "[(19, OrderedDict([('name', 'fuse-overlayfs'), ('autodependency', 'true'), ('info', "*

 * *           "'docker need')])), (20, OrderedDict([('name', 'libcgroup'), ('autodependency', "*

 * *           "'true'), ('info', 'docker need')])), (21, OrderedDict([('name', 'slirp4netns'), "*

 * *           "('url', "*

 * *           "'https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/slirp4netns-0.4.3-4.el7_8.x86_64.rpm'), "*

 * *           "('sha256', 'b98eb2c09940f8fb40405c0fd310bfa2ebc8f2e5e2711df564b35db06d0272 […]*

```diff
@@ -84,14 +84,34 @@
     },
     {
         "autodependency": "true",
         "info": "used for mindspore",
         "name": "gmp-c++"
     },
     {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "fuse-overlayfs"
+    },
+    {
+        "autodependency": "true",
+        "info": "docker need",
+        "name": "libcgroup"
+    },
+    {
+        "name": "slirp4netns",
+        "sha256": "b98eb2c09940f8fb40405c0fd310bfa2ebc8f2e5e2711df564b35db06d027286",
+        "url": "https://mirrors.huaweicloud.com/centos/7/extras/x86_64/Packages/slirp4netns-0.4.3-4.el7_8.x86_64.rpm"
+    },
+    {
+        "name": "container-selinux",
+        "sha256": "48de427ad3fb67f3b6998701340eafe1f610fbd587e8bd4e639124fe4d3f86d4",
+        "url": "https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/OS/x86_64/Packages/container-selinux-2.138-4.oe2203.noarch.rpm"
+    },
+    {
         "name": "sshpass",
         "sha256": "11ce47f53bebfc51054e49fbce324c1abf346169b28d47cd2ce6040df9799a7a",
         "url": "https://repo.openeuler.org/openEuler-22.03-LTS/everything/x86_64/Packages/sshpass-1.09-1.oe2203.x86_64.rpm"
     },
     {
         "name": "docker-ce-cli",
         "release": "3.el7",
@@ -107,9 +127,14 @@
         "release": "3.el7",
         "version": "20.10.8"
     },
     {
         "name": "docker-ce-rootless-extras",
         "release": "3.el7",
         "version": "20.10.8"
+    },
+    {
+        "name": "docker-scan-plugin",
+        "release": "3.el7",
+        "version": "0.23.0"
     }
 ]
```

## ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo

```diff
@@ -1,5 +1,14 @@
+[extra]
+baseurl=https://mirrors.huaweicloud.com/centos/7/extras/x86_64/
+
 [base]
 baseurl = https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/OS/x86_64/
 
+[everything]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/everything/x86_64/
+
+[update]
+baseurl=https://repo.huaweicloud.com/openeuler/openEuler-22.03-LTS/update/x86_64/
+
 [docker-ce]
 baseurl=https://mirrors.huaweicloud.com/docker-ce/linux/centos/7/x86_64/stable/
```

## ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.874251497005988%*

 * *Differences: {'insert': "[(146, OrderedDict([('name', 'build-essential')])), (147, OrderedDict([('name', "*

 * *           "'bzip2-doc')])), (148, OrderedDict([('name', 'fakeroot')])), (149, "*

 * *           "OrderedDict([('name', 'libalgorithm-diff-perl')])), (150, OrderedDict([('name', "*

 * *           "'libalgorithm-diff-xs-perl')])), (151, OrderedDict([('name', "*

 * *           "'libalgorithm-merge-perl')])), (152, OrderedDict([('name', 'libfakeroot')])), (153, "*

 * *           "OrderedDict([('name', 'libfile-fcntllock-perl')])), (154,  […]*

```diff
@@ -440,9 +440,72 @@
     {
         "info": "cross compiler ends",
         "name": "linux-libc-dev-arm64-cross"
     },
     {
         "info": "used by mindspore",
         "name": "libgmpxx4ldbl"
+    },
+    {
+        "name": "build-essential"
+    },
+    {
+        "name": "bzip2-doc"
+    },
+    {
+        "name": "fakeroot"
+    },
+    {
+        "name": "libalgorithm-diff-perl"
+    },
+    {
+        "name": "libalgorithm-diff-xs-perl"
+    },
+    {
+        "name": "libalgorithm-merge-perl"
+    },
+    {
+        "name": "libfakeroot"
+    },
+    {
+        "name": "libfile-fcntllock-perl"
+    },
+    {
+        "name": "manpages-dev"
+    },
+    {
+        "name": "bzip2"
+    },
+    {
+        "name": "liblzma5"
+    },
+    {
+        "name": "libncursesw5"
+    },
+    {
+        "name": "libpcre3"
+    },
+    {
+        "name": "libsasl2-modules"
+    },
+    {
+        "name": "libsepol1"
+    },
+    {
+        "name": "dbus-user-session"
+    },
+    {
+        "name": "docker-scan-plugin"
+    },
+    {
+        "name": "libltdl7"
+    },
+    {
+        "name": "pigz"
+    },
+    {
+        "name": "dbus"
+    },
+    {
+        "name": "libdbus-1-3"
     }
 ]
```

## ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8907103825136612%*

 * *Differences: {'insert': "[(163, OrderedDict([('name', 'build-essential')])), (164, OrderedDict([('name', "*

 * *           "'bzip2-doc')])), (165, OrderedDict([('name', 'fakeroot')])), (166, "*

 * *           "OrderedDict([('name', 'libalgorithm-diff-perl')])), (167, OrderedDict([('name', "*

 * *           "'libalgorithm-diff-xs-perl')])), (168, OrderedDict([('name', "*

 * *           "'libalgorithm-merge-perl')])), (169, OrderedDict([('name', 'libfakeroot')])), (170, "*

 * *           "OrderedDict([('name', 'libfile-fcntllock-perl')])), (171,  […]*

```diff
@@ -490,9 +490,69 @@
     },
     {
         "name": "libubsan1-arm64-cross"
     },
     {
         "info": "cross compiler ends",
         "name": "linux-libc-dev-arm64-cross"
+    },
+    {
+        "name": "build-essential"
+    },
+    {
+        "name": "bzip2-doc"
+    },
+    {
+        "name": "fakeroot"
+    },
+    {
+        "name": "libalgorithm-diff-perl"
+    },
+    {
+        "name": "libalgorithm-diff-xs-perl"
+    },
+    {
+        "name": "libalgorithm-merge-perl"
+    },
+    {
+        "name": "libfakeroot"
+    },
+    {
+        "name": "libfile-fcntllock-perl"
+    },
+    {
+        "name": "manpages-dev"
+    },
+    {
+        "name": "libgcc-s1"
+    },
+    {
+        "name": "libncurses6"
+    },
+    {
+        "name": "libncursesw6"
+    },
+    {
+        "name": "libpcre2-8-0"
+    },
+    {
+        "name": "libpcre3"
+    },
+    {
+        "name": "libsasl2-modules"
+    },
+    {
+        "name": "libsepol1"
+    },
+    {
+        "name": "libtinfo6"
+    },
+    {
+        "name": "docker-scan-plugin"
+    },
+    {
+        "name": "pigz"
+    },
+    {
+        "name": "slirp4netns"
     }
 ]
```

## ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json

### Pretty-printed

 * *Similarity: 0.8541666666666666%*

 * *Differences: {'insert': "[(135, OrderedDict([('name', 'docker-scan-plugin'), ('version', '0.23.0')])), (144, "*

 * *           "OrderedDict([('name', 'libasan6-arm64-cross')])), (145, OrderedDict([('name', "*

 * *           "'libhwasan0-arm64-cross')])), (146, OrderedDict([('name', 'gcc-12-cross-base')])), "*

 * *           "(147, OrderedDict([('name', 'libhdf5-hl-cpp-100')])), (148, OrderedDict([('name', "*

 * *           "'gcc-12')])), (149, OrderedDict([('name', 'dh-elpa-helper')])), (150, "*

 * *           "OrderedDict([('name', 'libcurl4-o […]*

```diff
@@ -405,14 +405,18 @@
         "version": "23.0.1"
     },
     {
         "name": "containerd.io",
         "version": "1.6.18"
     },
     {
+        "name": "docker-scan-plugin",
+        "version": "0.23.0"
+    },
+    {
         "name": "libquadmath0"
     },
     {
         "name": "libseccomp2"
     },
     {
         "info": "gcc cross compiler",
@@ -431,14 +435,95 @@
     {
         "name": "cpp-12"
     },
     {
         "name": "cpp-9"
     },
     {
+        "name": "libasan6-arm64-cross"
+    },
+    {
+        "name": "libhwasan0-arm64-cross"
+    },
+    {
+        "name": "gcc-12-cross-base"
+    },
+    {
+        "name": "libhdf5-hl-cpp-100"
+    },
+    {
+        "name": "gcc-12"
+    },
+    {
+        "name": "dh-elpa-helper"
+    },
+    {
+        "name": "libcurl4-openssl-dev"
+    },
+    {
+        "name": "emacsen-common"
+    },
+    {
+        "name": "libgcc-10-dev-arm64-cross"
+    },
+    {
+        "name": "libhdf5-103-1"
+    },
+    {
+        "name": "libnsl-dev"
+    },
+    {
+        "name": "libhdf5-hl-100"
+    },
+    {
+        "name": "libasan8"
+    },
+    {
+        "name": "libtsan2"
+    },
+    {
+        "name": "libtinfo5"
+    },
+    {
+        "name": "libgcc-12-dev"
+    },
+    {
+        "name": "libstdc++-11-dev-arm64-cross"
+    },
+    {
+        "name": "libasan5"
+    },
+    {
+        "name": "libgcc-9-dev"
+    },
+    {
+        "name": "libtirpc-dev"
+    },
+    {
+        "name": "libhdf5-cpp-103-1"
+    },
+    {
+        "name": "lto-disabled-list"
+    },
+    {
+        "name": "rpcsvc-proto"
+    },
+    {
+        "name": "libhdf5-fortran-102"
+    },
+    {
+        "name": "gcc-9"
+    },
+    {
+        "name": "libgcc-11-dev-arm64-cross"
+    },
+    {
+        "name": "libhdf5-hl-fortran-100"
+    },
+    {
         "name": "cpp-aarch64-linux-gnu"
     },
     {
         "name": "gcc-11-aarch64-linux-gnu"
     },
     {
         "name": "g++-11-aarch64-linux-gnu"
```

## ascend_deployer/downloader/software/CANN_6.0.1.json

### Pretty-printed

 * *Similarity: 0.8611111111111112%*

 * *Differences: {"'default'": 'False',*

 * * "'other'": "{insert: [(4, OrderedDict([('filename', 'Ascend-cann-kernels-310p_6.0.1_linux.zip'), "*

 * *            "('url', "*

 * *            "'https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-kernels-310p_6.0.1_linux.zip'), "*

 * *            "('sha256', '4cf05205bf69feb213eb800fcb1caf6921d17b22a5c8fa1c5de351591c7166fe')])), "*

 * *            "(5, OrderedDict([('filename', 'Ascend-cann-kernels-910_6.0.1_linux.zip'), ('url', "*

 * *            "'https://ascend-repo.obs.cn- […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "name": "CANN",
     "other": [
         {
             "filename": "Ascend-cann-toolkit_6.0.1_linux-aarch64.zip",
             "sha256": "500db9fbe8b6848b464e667483d4b6864ae5a991fa718f60433ad37a38c0edec",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-toolkit_6.0.1_linux-aarch64.zip"
         },
@@ -19,14 +19,24 @@
         },
         {
             "filename": "Ascend-cann-nnae_6.0.1_linux-x86_64.zip",
             "sha256": "29ac639fd1614a7b027b99eb609f08e44a16c4348f88532a0fce7bb1734c3d22",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-nnae_6.0.1_linux-x86_64.zip"
         },
         {
+            "filename": "Ascend-cann-kernels-310p_6.0.1_linux.zip",
+            "sha256": "4cf05205bf69feb213eb800fcb1caf6921d17b22a5c8fa1c5de351591c7166fe",
+            "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-kernels-310p_6.0.1_linux.zip"
+        },
+        {
+            "filename": "Ascend-cann-kernels-910_6.0.1_linux.zip",
+            "sha256": "b3fe79d017fbe0190bdbf9fb38b69cf4a3528dd17f5c5d92e2b43e92d3095670",
+            "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-kernels-910_6.0.1_linux.zip"
+        },
+        {
             "filename": "Ascend-cann-nnrt_6.0.1_linux-aarch64.zip",
             "sha256": "2eb6701230551d58704bd9201958f819c58e3096e61bfa4a0362d99c6660bedb",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.1/Ascend-cann-nnrt_6.0.1_linux-aarch64.zip"
         },
         {
             "filename": "Ascend-cann-nnrt_6.0.1_linux-x86_64.zip",
             "sha256": "0ae2b4894e93b01d541a5b390befa0954509bb8fcf45e3c7619c0e9e776d060a",
```

## ascend_deployer/downloader/software/CANN_6.0.RC1.json

### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'other'": "{0: {'sha256': '9c91f115792949a0a1a6c31f27960953f68d0aabaee50c1020893c0363c6cbd0'}, "*

 * *            "1: {'sha256': '0db899eeca0a91428bee4e889082b28251ef5405349541fe5659bd48055340cc'}, 2: "*

 * *            "{'sha256': 'c28277554e45917812006e229b88aababebf95590385c173288f4dc34125e2af'}, 3: "*

 * *            "{'sha256': 'b747cfbb6182fe7f7582abc5ae151a7393a29cd14bde47f0d7272290e74c01ea'}, 4: "*

 * *            "{'sha256': '3afa742063a387cc1b612f9c15f1a02ca86d0bcab3c524e88b9acc812884d0e4'}, 5: "*

 * *            "{'sha […]*

```diff
@@ -1,39 +1,39 @@
 {
     "default": false,
     "name": "CANN",
     "other": [
         {
             "filename": "Ascend-cann-toolkit_6.0.RC1_linux-aarch64.zip",
-            "sha256": "",
+            "sha256": "9c91f115792949a0a1a6c31f27960953f68d0aabaee50c1020893c0363c6cbd0",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-toolkit_6.0.RC1_linux-aarch64.zip"
         },
         {
             "filename": "Ascend-cann-toolkit_6.0.RC1_linux-x86_64.zip",
-            "sha256": "",
+            "sha256": "0db899eeca0a91428bee4e889082b28251ef5405349541fe5659bd48055340cc",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-toolkit_6.0.RC1_linux-x86_64.zip"
         },
         {
             "filename": "Ascend-cann-nnae_6.0.RC1_linux-aarch64.zip",
-            "sha256": "",
+            "sha256": "c28277554e45917812006e229b88aababebf95590385c173288f4dc34125e2af",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-nnae_6.0.RC1_linux-aarch64.zip"
         },
         {
             "filename": "Ascend-cann-nnae_6.0.RC1_linux-x86_64.zip",
-            "sha256": "",
+            "sha256": "b747cfbb6182fe7f7582abc5ae151a7393a29cd14bde47f0d7272290e74c01ea",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-nnae_6.0.RC1_linux-x86_64.zip"
         },
         {
             "filename": "Ascend-cann-nnrt_6.0.RC1_linux-aarch64.zip",
-            "sha256": "",
+            "sha256": "3afa742063a387cc1b612f9c15f1a02ca86d0bcab3c524e88b9acc812884d0e4",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-nnrt_6.0.RC1_linux-aarch64.zip"
         },
         {
             "filename": "Ascend-cann-nnrt_6.0.RC1_linux-x86_64.zip",
-            "sha256": "",
+            "sha256": "e295129daed0bc46f5457e5d73f43979b63e3ad218c16448d4d83af52313b960",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/CANN/CANN%206.0.RC1/Ascend-cann-nnrt_6.0.RC1_linux-x86_64.zip"
         },
         {
             "filename": "A800-9000-npu_6.0.rc1_linux-aarch64.zip",
             "sha256": "d03f23394b691f92ac11db066c16fac789e66a8434bf4a29b7ea10517b76ecb5",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/Ascend%20HDK/Ascend%20HDK%2022.0.RC3.1/A800-9000-npu_6.0.rc1_linux-aarch64.zip"
         },
```

## ascend_deployer/downloader/software/MindSpore_1.10.0.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "mindspore": [
         {
             "system": "linux_aarch64",
             "whl": [
                 {
                     "dest": "",
                     "filename": "mindspore_ascend-1.10.0-cp39-cp39-linux_aarch64.whl",
```

## ascend_deployer/downloader/software/MindStudio_5.0.0.json

### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'default'": 'False'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "default": true,
+    "default": false,
     "name": "MindStudio",
     "other": [
         {
             "filename": "MindStudio_5.0.0_linux.tar.gz",
             "sha256": "6958f7b26bab65d9552c8cc6fb4d89b80c46d78a3743887343c40477aae9cc46",
             "url": "https://ascend-repo.obs.cn-east-2.myhuaweicloud.com/MindStudio/MindStudio%205.0.0/MindStudio_5.0.0_linux.tar.gz"
         }
```

## ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 import os
 import sqlite3 as sqlite
 import xml.sax
 
-import logger_config
+from .. import logger_config
 
 LOG = logger_config.LOG
 
 try:
     import defusedxml
     defusedxml.defuse_stdlib()
 except ImportError:
```

## ascend_deployer/playbooks/gather_app_info.yml

 * *Ordering differences only*

```diff
@@ -1,40 +1,40 @@
-- name: gather app install info for all
-  hosts: all
-  gather_facts: False
-  vars:
-    need_test: yes
-    temp: "{{ ansible_distribution_version | regex_findall('[0-9]+.[0-9]+') }}"
-    os_version: "{{ temp[0] }}"
-    os_and_arch: "{{ansible_distribution}}_{{os_version}}_{{ansible_architecture}}"
-
-  tasks:
-    - name: gather facts first
-      setup:
-        fact_path: /notexist
-
-    - name: set custom fact tasks
-      import_tasks: task_set_custom_fact.yml
-
-    - name: create facts.d folder
-      file:
-        path: ~/ansible/facts.d/
-        state: directory
-        mode: 0750
-        recurse: yes
-
-    - name: copy app_info.fact to host
-      template:
-        src: facts/app_info.fact.j2
-        dest: ~/ansible/facts.d/app_info.fact
-        mode: "0550"
-
-    - name: gather facts again
-      setup:
-        fact_path: ~/ansible/facts.d/
-
-    - name: show app install info
-      debug:
-        var=ansible_local.app_info
-
-- name: set facts_cache dir permission
-  import_playbook: set_facts_cache_permission.yml
+- name: gather app install info for all
+  hosts: all
+  gather_facts: False
+  vars:
+    need_test: yes
+    temp: "{{ ansible_distribution_version | regex_findall('[0-9]+.[0-9]+') }}"
+    os_version: "{{ temp[0] }}"
+    os_and_arch: "{{ansible_distribution}}_{{os_version}}_{{ansible_architecture}}"
+
+  tasks:
+    - name: gather facts first
+      setup:
+        fact_path: /notexist
+
+    - name: set custom fact tasks
+      import_tasks: task_set_custom_fact.yml
+
+    - name: create facts.d folder
+      file:
+        path: ~/ansible/facts.d/
+        state: directory
+        mode: 0750
+        recurse: yes
+
+    - name: copy app_info.fact to host
+      template:
+        src: facts/app_info.fact.j2
+        dest: ~/ansible/facts.d/app_info.fact
+        mode: "0550"
+
+    - name: gather facts again
+      setup:
+        fact_path: ~/ansible/facts.d/
+
+    - name: show app install info
+      debug:
+        var=ansible_local.app_info
+
+- name: set facts_cache dir permission
+  import_playbook: set_facts_cache_permission.yml
```

## ascend_deployer/playbooks/gather_npu_fact.yml

```diff
@@ -2,24 +2,28 @@
   hosts: all
   gather_facts: False
 
   tasks:
     - name: gather facts first
       setup:
         fact_path: /notexist
-    
+
+    - name: sync time
+      import_tasks: sync_time.yml
+      when: ansible_user_uid == 0
+
     - name: create user if not exist
       import_tasks: create_user.yml
       when: ansible_user_uid == 0
 
     - set_fact: python_minor={{python_version[:-2]}}
 
     - name: get python version
       debug: var=python_minor
-      
+
     - name: set custom fact tasks
       import_tasks: task_set_custom_fact.yml
 
     - name: create facts.d folder
       file:
         path: ~/ansible/facts.d/
         state: directory
@@ -32,9 +36,14 @@
         dest: ~/ansible/facts.d/npu_info.fact
         mode: "0550"
 
     - name: gather facts again
       setup:
         fact_path: ~/ansible/facts.d/
 
+    - name: create nexus repository
+      shell: python3 {{inventory_dir}}/scripts/nexus.py
+      delegate_to: localhost
+      run_once: true
+
 - name: set facts_cache dir permission
   import_playbook: set_facts_cache_permission.yml
```

## ascend_deployer/playbooks/os_map.yml

```diff
@@ -9,39 +9,27 @@
   UOS: "UOS"
   uos: "UOS"
   tlinux: "Tlinux"
   openEuler: "OpenEuler"
 os_version_dict:
   euleros:
     "2.0": "2"
-  centos:
-    "7": "7.6"
-    "8": "8.2"
-  debian:
-    "9": "9.9"
-    "10": "10.0"
   kylin:
     "V10": "V10"
     "v10": "v10"
   Linx:
-    "9": "6"
+    "9": "6.0.90"
     "10": "6.0.100"
 code_name_dict:
   euleros:
     "SP8": ".8"
     "SP9": ".9"
     "SP9x86": ".9"
-  kylin:
-    "Tercel": "Tercel"
-    "juniper": "juniper"
-  openEuler:
-    "LTS-SP1": "LTS"
-    "LTS-SP3": "LTS"
-    "LTS": "LTS"
-    "": "LTS"
+    "SP10": ".10"
+    "SP10x86": ".10"
 code_name: ""
 scene_dict:
   normalize310p:
     - "{{ resources_dir }}/run_from_a310p_zip"
   normalize910:
     - "{{ resources_dir }}/run_from_910_zip"
   a910b:
@@ -58,7 +46,46 @@
     - "{{ resources_dir }}/run_from_a300v_pro_zip"
   a300iduo:
     - "{{ resources_dir }}/run_from_a300iduo_zip"
   train:
     - "{{ resources_dir }}/run_from_train_zip"
   trainpro:
     - "{{ resources_dir }}/run_from_train_pro_zip"
+os_list:
+  - BCLinux_7.6_aarch64
+  - BCLinux_7.6_x86_64
+  - BCLinux_7.7_aarch64
+  - CentOS_7.6_aarch64
+  - CentOS_7.6_x86_64
+  - CentOS_8.2_aarch64
+  - CentOS_8.2_x86_64
+  - Debian_9.9_aarch64
+  - Debian_9.9_x86_64
+  - Debian_10.0_x86_64
+  - EulerOS_2.8_aarch64
+  - EulerOS_2.9_aarch64
+  - EulerOS_2.9_x86_64
+  - EulerOS_2.10_aarch64
+  - EulerOS_2.10_x86_64
+  - Kylin_v10juniper_aarch64
+  - Kylin_V10Tercel_aarch64
+  - Kylin_V10Tercel_x86_64
+  - Linx_6.0.90_aarch64
+  - Linx_6.0.100_aarch64
+  - OpenEuler_20.03LTS_aarch64
+  - OpenEuler_20.03LTS_x86_64
+  - OpenEuler_22.03LTS_aarch64
+  - OpenEuler_22.03LTS_x86_64
+  - Tlinux_2.4_aarch64
+  - Tlinux_2.4_x86_64
+  - Ubuntu_18.04_aarch64
+  - Ubuntu_18.04_x86_64
+  - Ubuntu_20.04_aarch64
+  - Ubuntu_20.04_x86_64
+  - Ubuntu_22.04_aarch64
+  - Ubuntu_22.04_x86_64
+  - UOS_20_aarch64
+  - UOS_20_x86_64
+  - UOS_20-1020e_aarch64
+  - UOS_20-1021e_aarch64
+  - UOS_20SP1_aarch64
+  - UOS_20SP1_x86_64
```

## ascend_deployer/playbooks/task_set_custom_fact.yml

```diff
@@ -2,55 +2,108 @@
   include_vars: os_map.yml
 
 - name: get OS ID
   shell: grep -oP "^ID=\"?\K\w+" /etc/os-release
   changed_when: false
   register: os_id
 
-- name: get OS VERSION
-  shell: grep -oP "^VERSION_ID=\"?\K\w+\.?\w*" /etc/os-release
-  changed_when: false
-  register: os_ver
-
-- name: get OS code name
-  shell: grep -oP "^VERSION=(.*?)\(\K[\w\.\ -]+" /etc/os-release | awk -F_ '{print $1}'
-  changed_when: false
-  register: os_codename
-  failed_when: false
-  ignore_errors: yes
+- name: message
+  debug:
+    msg: "os {{ os_id.stdout}} is not supported"
+  failed_when: true
+  when: os_id.stdout not in os_dict
 
 - name: set os_name
   set_fact:
     os_name: "{{ os_dict[os_id.stdout] }}"
     cacheable: yes
   when: os_id.stdout in os_dict
 
-- name: message
-  debug:
-    msg: "os {{ os_id.stdout}} is not supportted"
-  failed_when: true
-  when: os_id.stdout not in os_dict
+- name: get OS VERSION
+  shell: grep -oP "^VERSION_ID=\"?\K\w+\.?\w*" /etc/os-release
+  changed_when: false
+  register: os_ver
 
 - name: set os_version first
   set_fact:
     os_version: "{{ os_ver.stdout }}"
     cacheable: yes
 
 - name: set os_version second
   set_fact:
     os_version: "{{ os_version_dict[os_id.stdout][os_ver.stdout] }}"
     cacheable: yes
   when: os_id.stdout in os_version_dict
 
+- name: get centos version
+  shell: cat /etc/centos-release|awk '{print $4}'|awk -v FS="." -v OFS="." '{print $1,$2}'
+  changed_when: false
+  register: os_ver
+  when: os_id.stdout == "centos"
+
+- name: set centos version
+  set_fact:
+    os_version: "{{ os_ver.stdout }}"
+    cacheable: yes
+  when: os_id.stdout == "centos"
+
+- name: get debian version
+  shell: cat /etc/debian_version
+  changed_when: false
+  register: os_ver
+  when: os_id.stdout == "debian"
+
+- name: set debian version
+  set_fact:
+    os_version: "{{ os_ver.stdout }}"
+    cacheable: yes
+  when: os_id.stdout == "debian"
+
+- name: get ubuntu version
+  shell: grep -oP "^PRETTY_NAME=\K.*" /etc/os-release|awk '{print $2}'
+  changed_when: false
+  register: ubuntu_ver
+  when: os_id.stdout == "ubuntu"
+
+- name: set ubuntu version
+  set_fact:
+    os_version: "{{ ubuntu_ver.stdout }}"
+    cacheable: yes
+  when: os_id.stdout == "ubuntu" and "18.04" in ubuntu_ver.stdout and ubuntu_ver.stdout != "18.04.1" and ubuntu_ver.stdout != "18.04.5"
+
+- name: get OS code name
+  shell: grep -oP "^VERSION=(.*?)\(\K[\w\.\ -]+" /etc/os-release | awk -F_ '{print $1}'
+  changed_when: false
+  register: os_codename
+  failed_when: false
+  ignore_errors: yes
+
 - name: set os code name
   set_fact:
     code_name: "{{ code_name_dict[os_id.stdout][os_codename.stdout] }}"
     cacheable: yes
   when: os_id.stdout in code_name_dict
 
+- name: get openEuler code name
+  shell: grep -oP "^VERSION=.*\KLTS[-\w]*" /etc/os-release
+  register: openEuler_codename
+  when: os_id.stdout == "openEuler"
+
+- name: set os code name for openEuler
+  set_fact:
+    code_name: "{{openEuler_codename.stdout}}"
+    cacheable: yes
+  when: os_id.stdout == "openEuler"
+
+- name: set os code name for kylin
+  set_fact:
+    code_name: "{{os_codename.stdout}}"
+    cacheable: yes
+  when: os_id.stdout == "kylin"
+
 - name: set euleros kernel flag
   set_fact:
     euleros_kernel_flag: "eulerosv2r{{code_name[1]}}.{{ansible_architecture}}"
     cacheable: yes
   when: os_name == "EulerOS"
 
 - name: get UOS_20SP1 code name
@@ -90,17 +143,23 @@
     os_and_arch: "{{os_name}}_{{os_version}}{{code_name}}_{{ansible_architecture}}"
     cacheable: yes
 
 - name: print current os
   debug:
     msg: "current os is {{ os_and_arch }}"
 
+- name: message
+  debug:
+    msg: "os {{os_and_arch}} is not supported"
+  failed_when: true
+  when: os_and_arch not in os_list
+
 - name: set resources_dir local
   set_fact:
-    resources_dir: "{{ inventory_dir }}/resources"
+    resources_dir: "{{ ascend_deployer_work_dir }}/resources"
     cacheable: yes
   when: ansible_connection == "local"
 
 - name: set resources_dir remote
   set_fact:
     resources_dir: "{{ ansible_user_dir }}/resources"
     cacheable: yes
```

## ascend_deployer/playbooks/facts/app_info.fact.j2

```diff
@@ -1,212 +1,166 @@
-#!{{ ansible_python.executable }}
-#!/usr/bin/env python
-import json
-import os
-import platform
-import sys
-import re
-
-
-def get_info_from_config(pkg_name, config_file='/etc/ascend_install.info'):
-    if not os.path.exists(config_file):
-        return None
-    if pkg_name not in ['driver', 'firmware']:
-        return None
-    info_dict = {"name": pkg_name, "install_arch": platform.machine()}
-    install_path_pattern = pkg_name + "_install_path"
-    install_path = ''
-    with open(config_file) as config_f:
-        for line in config_f:
-            if install_path_pattern in line.lower():
-                install_path = line.strip().split('=')[-1]
-                break
-    if not install_path or len(install_path) == 0:
-        return None
-    info_dict['install_path'] = install_path
-
-    pkg_version = ''
-    version_file = os.path.join(install_path, pkg_name, 'version.info')
-    with open(version_file) as version_f:
-        for line in version_f:
-            if 'Version' in line.strip():
-                pkg_version = line.strip().split('=')[-1]
-
-                break
-    info_dict['version'] = pkg_version
-    return info_dict
-
-
-def get_info_dict_list(pkg_name, target_paths, target_file):
-    info_dict_list = []
-    for target_path in target_paths:
-        install_config_file = os.path.join(target_path, target_file)
-        info_dict = {"name": pkg_name}
-        install_arch = platform.machine()
-        pkg_version = ''
-        install_path = target_path
-        with open(install_config_file) as config_f:
-            for line in config_f:
-                if line.lower().startswith('version'):
-                    pkg_version = line.strip().split('=')[-1]
-                if line.lower().startswith('arch'):
-                    install_arch = line.strip().split('=')[-1]
-                if line.lower().startswith('path'):
-                    install_path = line.strip().split('=')[-1]
-
-        info_dict['install_path'] = install_path
-        info_dict['install_arch'] = install_arch
-        info_dict['version'] = pkg_version
-        info_dict_list.append(info_dict)
-
-    return info_dict_list
-
-
-def getinfo_from_xml(file_path, root_path):
-    if not os.path.exists(file_path):
-        return {}
-    with open(file_path, 'r') as f:
-        lines = f.readlines()
-    archs = {'ARM': 'aarch64', 'x86': 'x86_64'}
-    info_dict = {}
-    for line in lines:
-        if 'OutterName' in line:
-            info_dict['name'] = re.findall('>(.*)<', line)[0]
-        if 'ProcessorArchitecture' in line:
-            arch = re.findall('>(.*)<', line)[0]
-            info_dict['install_arch'] = archs.get(arch, arch)
-        if 'Version' in line:
-            info_dict['version'] = re.findall('>(.*)<', line)[0]
-    info_dict['install_path'] = root_path
-    return info_dict
-
-
-def get_edge_install_info(pkg_name, root_path='/usr/local'):
-    info_dict_list = []
-    if pkg_name == 'atlasedge':
-        xml_file = os.path.join(root_path, 'AtlasEdge/version.xml')
-    elif pkg_name == 'ha':
-        xml_file = os.path.join(root_path, 'ha/version.xml')
-    else:
-        return info_dict_list
-    res = getinfo_from_xml(xml_file, root_path)
-    if res:
-        info_dict_list.append(res)
-    return info_dict_list
-
-
-def get_cann_info_from_config(pkg_name, root_path='/usr/local/Ascend'):
-    if os.getuid() != 0:
-        root_path = os.path.expanduser('~/Ascend')
-    if not os.path.exists(root_path):
-        return None
-    if pkg_name not in ['nnrt', 'toolkit', 'nnae', 'tfplugin', 'toolbox']:
-        return None
-    first_path = os.path.join(root_path, pkg_name)
-    if pkg_name == 'toolkit':
-        first_path = os.path.join(root_path, 'ascend-toolkit')
-    target_file = "ascend_" + pkg_name + "_install.info"
-    target_paths = set()
-    for top, dirs, nodirs in os.walk(first_path):
-        for file_name in nodirs:
-            if file_name == target_file:
-                target_paths.add(top)
-                break
-    return get_info_dict_list(pkg_name, target_paths, target_file)
-
-
-def get_firmware_install_info():
-    try:
-        return get_info_from_config("firmware")
-    except:
-        return None
-
-
-def get_driver_install_info():
-    try:
-        return get_info_from_config("driver")
-    except:
-        return None
-
-
-def get_nnrt_install_info():
-    try:
-        return get_cann_info_from_config('nnrt')
-    except:
-        return None
-
-
-def get_nnae_install_info():
-    try:
-        return get_cann_info_from_config('nnae')
-    except:
-        return None
-
-
-def get_tfplugin_install_info():
-    try:
-        return get_cann_info_from_config('tfplugin')
-    except:
-        return None
-
-
-def get_toolbox_install_info():
-    try:
-        return get_cann_info_from_config('toolbox')
-    except:
-        return None
-
-
-def get_toolkit_install_info():
-    try:
-        return get_cann_info_from_config('toolkit')
-    except:
-        return None
-
-
-def get_app_install_info(app_name='all'):
-    app_install_info = []
-    firmware = get_firmware_install_info()
-    if app_name in ['all', 'npu', 'firmware'] and firmware:
-        app_install_info.append(firmware)
-    driver = get_driver_install_info()
-    if app_name in ['all', 'npu', 'driver'] and driver:
-        app_install_info.append(driver)
-    nnrt = get_nnrt_install_info()
-    if app_name in ['all', 'nnrt'] and nnrt:
-        app_install_info.extend(nnrt)
-    nnae = get_nnae_install_info()
-    if app_name in ['all', 'nnae'] and nnae:
-        app_install_info.extend(nnae)
-    tfplugin = get_tfplugin_install_info()
-    if app_name in ['all', 'tfplugin'] and tfplugin:
-        app_install_info.extend(tfplugin)
-    toolbox = get_toolbox_install_info()
-    if app_name in ['all', 'toolbox'] and toolbox:
-        app_install_info.extend(toolbox)
-    toolkit = get_toolkit_install_info()
-    if app_name in ['all', 'toolkit'] and toolkit:
-        app_install_info.extend(toolkit)
-    if app_name in ['all', 'atlasedge']:
-        edge = get_edge_install_info('atlasedge')
-        if edge:
-            app_install_info.extend(edge)
-    if app_name in ['all', 'ha']:
-        ha = get_edge_install_info('ha')
-        if ha:
-            app_install_info.extend(ha)
-    return app_install_info
-
-
-def main():
-    ret = {
-        "progress": "1.0",
-        "operation": "app display",
-        "result": []
-    }
-
-    result = get_app_install_info("{{ app_name }}")
-    ret['result'] = result
-    json.dump(ret, sys.stdout, indent=4)
-
-
-main()
+#!{{ ansible_python.executable }}
+#!/usr/bin/env python
+import json
+import os
+import platform
+import re
+
+
+def get_info_from_config(pkg_name, config_file='/etc/ascend_install.info'):
+    if not os.path.exists(config_file):
+        return None
+    if pkg_name not in ['driver', 'firmware']:
+        return None
+    info_dict = {"name": pkg_name, "install_arch": platform.machine()}
+    install_path_pattern = pkg_name + "_install_path"
+    install_path = ''
+    with open(config_file) as config_f:
+        for line in config_f:
+            if install_path_pattern in line.lower():
+                install_path = line.strip().split('=')[-1]
+                break
+    if not install_path or len(install_path) == 0:
+        return None
+    info_dict['install_path'] = install_path
+
+    pkg_version = ''
+    version_file = os.path.join(install_path, pkg_name, 'version.info')
+    with open(version_file) as version_f:
+        for line in version_f:
+            if 'Version' in line.strip():
+                pkg_version = line.strip().split('=')[-1]
+
+                break
+    info_dict['version'] = pkg_version
+    return info_dict
+
+
+def get_info_dict_list(pkg_name, target_paths, target_file):
+    info_dict_list = []
+    for target_path in target_paths:
+        install_config_file = os.path.join(target_path, target_file)
+        info_dict = {"name": pkg_name}
+        install_arch = platform.machine()
+        pkg_version = ''
+        install_path = target_path
+        with open(install_config_file) as config_f:
+            for line in config_f:
+                if line.lower().startswith('version'):
+                    pkg_version = line.strip().split('=')[-1]
+                if line.lower().startswith('arch'):
+                    install_arch = line.strip().split('=')[-1]
+                if line.lower().startswith('path'):
+                    install_path = line.strip().split('=')[-1]
+
+        info_dict['install_path'] = install_path
+        info_dict['install_arch'] = install_arch
+        info_dict['version'] = pkg_version
+        info_dict_list.append(info_dict)
+
+    return info_dict_list
+
+
+def getinfo_from_xml(file_path, root_path):
+    if not os.path.exists(file_path):
+        return {}
+    with open(file_path, 'r') as f:
+        lines = f.readlines()
+    archs = {'ARM': 'aarch64', 'x86': 'x86_64'}
+    info_dict = {}
+    for line in lines:
+        if 'OutterName' in line:
+            info_dict['name'] = re.findall('>(.*)<', line)[0]
+        if 'ProcessorArchitecture' in line:
+            arch = re.findall('>(.*)<', line)[0]
+            info_dict['install_arch'] = archs.get(arch, arch)
+        if 'Version' in line:
+            info_dict['version'] = re.findall('>(.*)<', line)[0]
+    info_dict['install_path'] = root_path
+    return info_dict
+
+
+def get_edge_install_info(pkg_name, root_path='/usr/local'):
+    info_dict_list = []
+    if pkg_name == 'atlasedge':
+        xml_file = os.path.join(root_path, 'AtlasEdge/version.xml')
+    elif pkg_name == 'ha':
+        xml_file = os.path.join(root_path, 'ha/version.xml')
+    else:
+        return info_dict_list
+    res = getinfo_from_xml(xml_file, root_path)
+    if res:
+        info_dict_list.append(res)
+    return info_dict_list
+
+
+def get_cann_info_from_config(pkg_name, root_path='/usr/local/Ascend'):
+    if os.getuid() != 0:
+        root_path = os.path.expanduser('~/Ascend')
+    if not os.path.exists(root_path):
+        return None
+    if pkg_name not in ['nnrt', 'toolkit', 'nnae', 'tfplugin', 'toolbox']:
+        return None
+    first_path = os.path.join(root_path, pkg_name, 'latest')
+    if pkg_name == 'toolkit':
+        first_path = os.path.join(root_path, 'ascend-toolkit', 'latest')
+    target_file = "ascend_" + pkg_name + "_install.info"
+    target_paths = set()
+    for top, dirs, nodirs in os.walk(first_path):
+        for file_name in nodirs:
+            if file_name == target_file:
+                target_paths.add(top)
+                break
+    return get_info_dict_list(pkg_name, target_paths, target_file)
+
+
+def get_basic_install_info(app):
+    try:
+        return get_info_from_config(app)
+    except:
+        return None
+
+
+def get_cann_install_info(cann):
+    try:
+        return get_cann_info_from_config(cann)
+    except:
+        return None
+
+
+def get_app_install_info():
+    app_install_info = []
+    basic_list = ['firmware', 'driver']
+    for app_name in basic_list:
+        app_info = get_basic_install_info(app_name)
+        if app_info:
+            app_install_info.append(app_info)
+
+    cann_list = ['nnrt', 'nnae', 'tfplugin', 'toolbox', 'toolkit']
+    for app_name in cann_list:
+        app_info = get_cann_install_info(app_name)
+        if app_info:
+            app_install_info.extend(app_info)
+
+    edge_list = ['atlasedge', 'ha']
+    for app_name in edge_list:
+        app_info = get_edge_install_info(app_name)
+        if app_name:
+            app_install_info.extend(app_info)
+
+    return app_install_info
+
+
+def main():
+    ret = {
+        "progress": "1.0",
+        "operation": "app display",
+        "result": []
+    }
+
+    result = get_app_install_info()
+    ret['result'] = result
+    with open('smartkit/display.json', 'w') as f:
+        json.dump(ret, f, indent=4)
+
+
+main()
```

## ascend_deployer/playbooks/facts/npu_info.fact.j2

```diff
@@ -1,327 +1,172 @@
 #!{{ ansible_python.executable }}
-import glob
 import json
 import os
 import platform
 import shlex
 import subprocess
 import sys
 
+ID_LEN = 6  # read 6 chars in /sys/bus/pci/devices/*/{class,vendor,device,subsystem_vendor,subsystem_device}
+ARCH = platform.machine()
+FIND_PRODUCT_CMD = 'dmidecode -t 1'
+FIND_SOC_PRODUCT_CMD = 'dmidecode -t 2'
 
-class ChipMetaData():
-    "metadata includes vid, did, svid, sdid, arch"
+card_map = {
+    ('0x19e5', '0xd100', '0x0200', '0x0100'): {'x86_64': 'A300-3010', 'aarch64': 'A300-3000'},
+    ('0x19e5', '0xd801', '0x0200', '0x0100'): 'A300T-9000',
+    ('0x19e5', '0xd802', '0x0200', '0x0100'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3000'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3001'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3002'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3003'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3004'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3400'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3401'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3402'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x3403'): 'A900T',
+    ('0x19e5', '0xd802', '0x19e5', '0x6000'): 'A900T',
+    ('0x19e5', '0xd500', '0x0200', '0x0100'): 'A300i-pro',
+    ('0x19e5', '0xd500', '0x0200', '0x0110'): 'A300i-duo',
+}
 
-    def __init__(self, vid, did, svid, sdid, arch):
-        self.vid = vid
-        self.did = did
-        self.svid = svid
-        self.sdid = sdid
-        self.arch = arch
-
-    def __hash__(self):
-        return hash((self.vid, self.did, self.svid, self.sdid, self.arch))
-
-    def __eq__(self, other):
-        return (self.vid, self.did, self.svid, self.sdid, self.arch) == (
-            other.vid, other.did, other.svid, other.sdid, other.arch)
-
-
-CHIPS_DICT = {
-    ChipMetaData('0x19e5', '0xd100', '0x0200', '0x0100',
-                 'x86_64'): 'A300-3010',
-    ChipMetaData('0x19e5', '0xd100', '0x0200', '0x0100',
-                 'aarch64'): 'A300-3000',
-    ChipMetaData('0x19e5', '0xd801', '0x0200', '0x0100',
-                 'aarch64'): 'A300T-9000',
-    ChipMetaData('0x19e5', '0xd801', '0x0200', '0x0100',
-                 'x86_64'): 'A300T-9000',
-    ChipMetaData('0x19e5', '0xd802', '0x0200', '0x0100',
-                 'aarch64'): 'A900T',
-    ChipMetaData('0x19e5', '0xd802', '0x0200', '0x0100',
-                 'x86_64'): 'A900T',
-    ChipMetaData('0x19e5', '0xd500', '0x0200', '0x0100',
-                 'aarch64'): 'A300i-pro',
-    ChipMetaData('0x19e5', '0xd500', '0x0200', '0x0100',
-                 'x86_64'): 'A300i-pro',
-    ChipMetaData('0x19e5', '0xd500', '0x0200', '0x0110',
-                 'x86_64'): 'A300i-duo',
-    ChipMetaData('0x19e5', '0xd500', '0x0200', '0x0110',
-                 'aarch64'): 'A300i-duo',
+product_model_dict = {
+    'Atlas 800 (Model 9000)': {'product': 'A800', 'model': '9000', 'name': 'A800-9000'},
+    'Atlas 800 (Model 9010)': {'product': 'A800', 'model': '9010', 'name': 'A800-9010'},
+    'Atlas 900 (Model 9000)': {'product': 'A900', 'model': '9000'},
+    'Atlas 900 Compute Node': {'product': 'A900', 'model': '9000'},
+    'A300T-9000': {'product': 'A300t', 'model': '9000', 'name': 'A300t-9000'},
+    'Atlas 800 (Model 3000)': {'product': 'A300', 'model': '3000', 'name': 'A300-3000'},
+    'Atlas 800 (Model 3010)': {'product': 'A300', 'model': '3010', 'name': 'A300-3010'},
+    'Atlas 500 Pro (Model 3000)': {'product': 'A300', 'model': '3000', 'name': 'A300-3000'},
+    'Atlas 500 Pro(Model 3000)': {'product': 'A300', 'model': '3000', 'name': 'A300-3000'},
+    'A300-3010': {'product': 'A300', 'model': '3010', 'name': 'A300-3010'},
+    'A300-3000': {'product': 'A300', 'model': '3000', 'name': 'A300-3000'},
+    'Atlas 500 (Model 3000)': {'product': 'A300', 'model': '3000', 'name': 'A300-3000'},
+    'A300i-pro': {'product': 'A300i', 'model': 'pro', 'name': 'A300i-pro'},
+    'A200-3000': {'product': 'A300', 'model': '3000'},
+    'A300i-duo': {'product': 'Atlas-300i-duo', 'model': 'duo', 'name': 'A300i-duo'},
+}
+
+scene_dict = {
+    'A300i-pro': 'a300i',
+    'A300-3000': 'infer',
+    'A300-3010': 'infer',
+    'A200-3000': 'infer',
+    'A800-9000': 'train',
+    'A800-9010': 'train',
+    'Atlas 900 Compute Node': 'train',
+    'A900T': 'a910b',
+    'A300i-duo': 'a300iduo',
 }
-FIND_METADATA = 'grep 0x1200 /sys/bus/pci/devices/*/class | awk -F \/ \'{print $6}\''
-FIND_PRODUCT_CMD = 'dmidecode -t 1'
-FIND_SOC_PRODUCT_CMD = 'dmidecode -t 2'
-FIND_PRODUCT = 'dmidecode -t 1 | grep Product | awk -F: \'{print $2}\''
 
 
-def get_profile_model(arch, model):
+def get_profile_model(model):
     if model == '--':
         return 'unknown'
 
     if 'Atlas' in model and 'Model' in model:
         model = "A" + model.split("(")[0].split()[1].strip() + \
                 "-" + model.split(")")[0].split("Model")[1].strip()
 
     if model == 'A300T-9000':
-        if arch == 'aarch64':
+        if ARCH == 'aarch64':
             model = 'A800-9000'
         else:
             model = 'A800-9010'
 
     if model in ['A500-3000', 'A800-3000']:
         model = 'A300-3000'
     if model == 'A800-3010':
         model = 'A300-3010'
 
     return model
 
 
-def get_scene(profile_model):
-    scene = ''
-    if profile_model in ['A300i-pro']:
-        scene = 'a300i'
-    if profile_model in ['A300-3000', 'A300-3010', 'A200-3000']:
-        scene = 'infer'
-    if profile_model in ['A800-9000', 'A800-9010', 'Atlas 900 Compute Node']:
-        scene = 'train'
-    if profile_model in ['A900T']:
-        scene = 'a910b'
-    if profile_model in ['A300i-duo']:
-        scene = 'a300iduo'
-
-    return scene
-
-
-def get_chip_info(vid, did, svid, sdid, arch):
-    if did == '0xd802':
-        return 'A900T'
-    chip_meta_data = ChipMetaData(vid.lower(), did.lower(), svid, sdid, arch)
-    return CHIPS_DICT.get(chip_meta_data, '--')
-
-
-def check_metadata_file_existance(bdf_path):
-    metadata_file = os.path.join(bdf_path, 'vendor')
-    ret = os.path.exists(metadata_file)
-    if not ret:
-        return False
-
-    metadata_file = os.path.join(bdf_path, 'device')
-    ret = os.path.exists(metadata_file)
-    if not ret:
-        return False
-
-    metadata_file = os.path.join(bdf_path, 'subsystem_device')
-    ret = os.path.exists(metadata_file)
-    if not ret:
-        return False
-
-    metadata_file = os.path.join(bdf_path, 'subsystem_vendor')
-    ret = os.path.exists(metadata_file)
-    if not ret:
-        return False
-
-    return True
-
-
-def get_metadatas(bdf_path):
-    metadata_file = os.path.join(bdf_path, 'device')
-    with open(metadata_file) as f:
-        did = f.read().replace('\t', '').replace('\n', '')
-        if not did:
-            return {}
-
-    metadata_file = os.path.join(bdf_path, 'vendor')
-    with open(metadata_file) as f:
-        vid = f.read().replace('\t', '').replace('\n', '')
-        if not vid:
-            return {}
-
-    metadata_file = os.path.join(bdf_path, 'subsystem_device')
-    with open(metadata_file) as f:
-        sdid = f.read().replace('\t', '').replace('\n', '')
-        if not sdid:
-            return {}
-
-    metadata_file = os.path.join(bdf_path, 'subsystem_vendor')
-    with open(metadata_file) as f:
-        svid = f.read().replace('\t', '').replace('\n', '')
-        if not svid:
-            return {}
-
-    return dict(did=did, vid=vid, sdid=sdid, svid=svid)
-
-
-def get_model():
-    bdf_file_paths = []
-    DEVNULL = open(os.devnull, 'w')
-    for candidate_dir in glob.glob('/sys/bus/pci/devices/*'):
-        find_metadata_cmd = ["grep", "0x1200",
-                             os.path.join(candidate_dir, "class")]
-        return_code = subprocess.call(find_metadata_cmd, shell=False,
-                                      stdout=DEVNULL, stderr=subprocess.STDOUT)
-        if return_code == 0:
-            bdf_file_paths.append(candidate_dir)
-    for bdf_file_path in bdf_file_paths:
-        model = _get_model(bdf_file_path, DEVNULL)
-        if model != '--':
-            return model
-    try:
-        cp = subprocess.Popen(args=shlex.split(FIND_SOC_PRODUCT_CMD),
-                              shell=False,
-                              universal_newlines=True,
-                              stdin=subprocess.PIPE,
-                              stdout=subprocess.PIPE,
-                              stderr=subprocess.PIPE)
-    except Exception:
-        return '--'
-    dmi_info_lines = cp.stdout.readlines()
-    raw_product = ""
-    for i in dmi_info_lines:
-        if 'Product' in i:
-            product_infos = i.split(':')
-            if len(product_infos) < 2:
-                return '--'
-            raw_product = product_infos[1]
-            break
-    product = raw_product.replace('\t', '').replace('\n', '').strip()
-    if product == 'Atlas 200I SoC A1':
-        return product
+def parse_item(dir_path):
+    """
+    parse device to tuple
+
+    @rtype: tuple
+    """
+    id_list = []
+    name_order = ('vendor', 'device', 'subsystem_vendor', 'subsystem_device')
+    for file_name in name_order:
+        full_file_path = os.path.join(dir_path, file_name)
+        if not os.path.exists(full_file_path):
+            continue
+        with open(os.path.join(full_file_path)) as f:
+            id_list.append(f.read(ID_LEN))
+    return tuple(id_list)
+
+
+def parse_card():
+    devices_path = '/sys/bus/pci/devices/'
+    for dir_name in os.listdir(devices_path):
+        full_dir = os.path.join(devices_path, dir_name)
+        class_file = os.path.join(full_dir, 'class')
+        if not os.path.exists(class_file):
+            continue
+        with open(class_file) as f:
+            if not f.read(ID_LEN).startswith('0x1200'):
+                continue
+        item = parse_item(full_dir)
+        value = card_map.get(item, '--')
+        if isinstance(value, dict):
+            return value.get(ARCH, '--')
+        return value
     return '--'
 
-def _get_model(bdf_file_path, DEVNULL):
-    ret = check_metadata_file_existance(bdf_file_path)
-    if not ret:
-        return '--'
-
-    metadata_dict = get_metadatas(bdf_file_path)
-    if not metadata_dict:
-        return '--'
-
-    arch = platform.machine()
-
-    chip_info = get_chip_info(
-        metadata_dict['vid'], metadata_dict['did'], metadata_dict['svid'],
-        metadata_dict['sdid'], arch)
-    if chip_info == '--' or chip_info == 'A300i-pro':
-        return chip_info
-
-    find_a500_cmd = ["stat", "/run/board_cfg.ini"]
-    return_code = subprocess.call(find_a500_cmd, shell=False,
-                                  stdout=DEVNULL, stderr=subprocess.STDOUT)
-    if return_code == 0:
-        return "Atlas 500 (Model 3000)"
 
+def get_product_from_dmi(cmd):
     try:
-        cp = subprocess.Popen(args=shlex.split(FIND_PRODUCT_CMD),
-                              shell=False,
-                              universal_newlines=True,
-                              stdin=subprocess.PIPE,
-                              stdout=subprocess.PIPE,
-                              stderr=subprocess.PIPE)
-    except Exception:
-        return chip_info
-    dmi_info_lines = cp.stdout.readlines()
-    raw_product = ""
-    for item in dmi_info_lines:
-        if 'Product' in item:
-            product_infos = item.split(':')
+        cp = subprocess.Popen(
+            args=shlex.split(cmd), shell=False, universal_newlines=True,
+            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    except OSError:
+        return ''
+    for line in cp.stdout.readlines():
+        if 'Product' in line:
+            product_infos = line.split(':')
             if len(product_infos) < 2:
-                return chip_info
+                return ''
             raw_product = product_infos[1]
-            break
-    product = raw_product.replace('\t', '').replace('\n', '').strip()
-    product_name = (
-        "Atlas 800 (Model 9000)",
-        "Atlas 800 (Model 9010)",
-        "Atlas 900 (Model 9000)",
-        "Atlas 900 Compute Node",
-        "Atlas 500 Pro (Model 3000)",
-        "Atlas 500 Pro(Model 3000)",
-        "Atlas 500 (Model 3000)",
-    )
-    if product in product_name:
-        return product
-
-    return chip_info
-
-
-def get_product(model):
-    product_dict = {
-        'Atlas 800 (Model 9000)': 'A800',
-        'Atlas 800 (Model 9010)': 'A800',
-        'Atlas 900 (Model 9000)': 'A900',
-        'Atlas 900 Compute Node': 'A900',
-        'A300T-9000': 'A300t',
-        'Atlas 800 (Model 3000)': 'A300',
-        'Atlas 800 (Model 3010)': 'A300',
-        'Atlas 500 Pro (Model 3000)': 'A300',
-        'Atlas 500 Pro(Model 3000)': 'A300',
-        'A300-3010': 'A300',
-        'A300-3000': 'A300',
-        'Atlas 500 (Model 3000)': 'A300',
-        'A300i-pro': 'A300i',
-        'A200-3000': 'A200',
-        'A300i-duo': 'Atlas-300i-duo'
-    }
-    if model in product_dict.keys():
-        return product_dict[model]
-    return ""
-
-
-def get_model_number(model):
-    model_dict = {
-        'Atlas 800 (Model 9000)': '9000',
-        'Atlas 800 (Model 9010)': '9010',
-        'Atlas 900 (Model 9000)': '9000',
-        'Atlas 900 Compute Node': '9000',
-        'A300T-9000': '9000',
-        'Atlas 800 (Model 3000)': '3000',
-        'Atlas 800 (Model 3010)': '3010',
-        'Atlas 500 Pro (Model 3000)': '3000',
-        'Atlas 500 Pro(Model 3000)': '3000',
-        'A300-3010': '3010',
-        'A300-3000': '3000',
-        'Atlas 500 (Model 3000)': '3000',
-        'A300i-pro': 'pro',
-        'A200-3000': '3000',
-        'A300i-duo': 'duo'
-    }
-    if model in model_dict.keys():
-        return model_dict[model]
-    return ""
-
-
-ALL_MODEL_DICT = {
-'Atlas 800 (Model 9000)': 'A800-9000',
-'Atlas 800 (Model 9010)': 'A800-9010',
-'A300T-9000': 'A300t-9000',
-'Atlas 800 (Model 3000)': 'A300-3000',
-'Atlas 800 (Model 3010)': 'A300-3010',
-'Atlas 500 Pro (Model 3000)': 'A300-3000',
-'Atlas 500 Pro(Model 3000)': 'A300-3000',
-'A300-3010': 'A300-3010',
-'A300-3000': 'A300-3000',
-'Atlas 500 (Model 3000)': 'A300-3000',
-'A300i-pro': 'A300i-pro',
-'A300i-duo': 'A300i-duo'
-}
+            return raw_product.replace('\t', '').replace('\n', '').strip()
+
+
+def parse_model(card):
+    if card == 'A300i-pro':
+        return card
+    if card != '--':
+        if os.path.exists("/run/board_cfg.ini"):
+            return "Atlas 500 (Model 3000)"
+        model_from_system = get_product_from_dmi(FIND_PRODUCT_CMD)
+        if model_from_system in product_model_dict:
+            return model_from_system
+    model_from_baseboard = get_product_from_dmi(FIND_SOC_PRODUCT_CMD)
+    if model_from_baseboard == 'Atlas 200I SoC A1':
+        return model_from_baseboard
+    return card
 
 
 def main():
-    arch = platform.machine()
-    model = get_model()
-    profile_model = get_profile_model(arch, model)
-    scene = get_scene(profile_model)
+    card = parse_card()
+    model = parse_model(card)
+    profile_model = get_profile_model(model)
+    scene = scene_dict.get(profile_model, '')
+    product = product_model_dict.get(model, {}).get('product', '')
+    model_num = product_model_dict.get(model, {}).get('model', '')
 
     ret = {
+        "card": card,
         "model": model,
         "scene": scene,
-        "python375_installed": os.path.exists('/usr/local/python3.7.5') if os.getuid() == 0 else os.path.exists(os.path.expanduser('~/.local/python3.7.5')),
-        "product": get_product(model),
-        "model_number": get_model_number(model),
-        "all_model_dict": ALL_MODEL_DICT
+        "python375_installed": os.path.exists('/usr/local/python3.7.5') if os.getuid() == 0 else os.path.exists(
+            os.path.expanduser('~/.local/python3.7.5')),
+        "product": product,
+        "model_number": model_num,
+        "all_model_dict": {k: v.get('name') for k, v in product_model_dict.items() if v.get('name')}
     }
     json.dump(ret, sys.stdout, indent=2)
 
 
 main()
```

## ascend_deployer/playbooks/install/task_driver_bcinux.yml

```diff
@@ -143,22 +143,34 @@
 
 - name: upgrade driver
   shell: "bash {{driver_run|default(driver_pro_run)}} --nox11 --upgrade --quiet"
   register: driver_up_result
   failed_when: driver_up_result.rc == 1
   when: (driver_run is defined and driver_run|length > 0 or driver_pro_run is defined and driver_pro_run|length > 0) and (up_tool.matched > 0)
 
+- name: set need_reboot fact
+  set_fact:
+    need_reboot: "{{'1' if 'Reboot' in driver_up_result.stdout or 'reboot' in driver_up_result.stdout else '0'}}"
+    cacheable: yes
+  when: driver_up_result.changed
+
 - name: install driver
   shell: "bash {{driver_run|default(driver_pro_run)}} --nox11 --full --quiet --install-username={{user}} --install-usergroup={{group}}"
   environment:
     PATH: /opt/rh/devtoolset-8/root/usr/bin/:/usr/sbin/:/sbin:{{ ansible_env.PATH }}
   register: driver_result
   failed_when: driver_result.rc == 1
   when: (driver_run is defined and driver_run|length > 0 or driver_pro_run is defined and driver_pro_run|length > 0) and (up_tool.matched == 0)
 
+- name: set need_reboot fact
+  set_fact:
+    need_reboot: "{{'1' if 'Reboot' in driver_result.stdout or 'reboot' in driver_result.stdout else '0'}}"
+    cacheable: yes
+  when: driver_result.changed
+
 - name: message
   debug:
     msg:
       - "can not find driver package, driver install skipped"
   when: driver_run is undefined and driver_pro_run is undefined
 
 - name: message
```

## ascend_deployer/playbooks/install/task_driver_common.yml

```diff
@@ -143,22 +143,34 @@
 
 - name: upgrade driver
   shell: "bash {{driver_run|default(driver_pro_run)}} --nox11 --upgrade --quiet"
   register: driver_up_result
   failed_when: driver_up_result.rc == 1
   when: (driver_run is defined and driver_run|length > 0 or driver_pro_run is defined and driver_pro_run|length > 0) and (up_tool.matched > 0)
 
+- name: set need_reboot fact
+  set_fact:
+    need_reboot: "{{'1' if 'Reboot' in driver_up_result.stdout or 'reboot' in driver_up_result.stdout else '0'}}"
+    cacheable: yes
+  when: driver_up_result.changed
+
 - name: install driver
   shell: "bash {{driver_run|default(driver_pro_run)}} --nox11 --full --quiet --install-username={{user}} --install-usergroup={{group}}"
   environment:
     PATH: /opt/rh/devtoolset-8/root/usr/bin/:/usr/sbin/:/sbin:{{ ansible_env.PATH }}
   register: driver_result
   failed_when: driver_result.rc == 1
   when: (driver_run is defined and driver_run|length > 0 or driver_pro_run is defined and driver_pro_run|length > 0) and (up_tool.matched == 0)
 
+- name: set need_reboot fact
+  set_fact:
+    need_reboot: "{{'1' if 'Reboot' in driver_result.stdout or 'reboot' in driver_result.stdout else '0'}}"
+    cacheable: yes
+  when: driver_result.changed
+
 - name: message
   debug:
     msg:
       - "can not find driver package, driver install skipped"
   when: driver_run is undefined and driver_pro_run is undefined
 
 - name: message
```

## ascend_deployer/playbooks/install/task_firmware.yml

```diff
@@ -133,20 +133,32 @@
 
 - name: upgrade firmware
   shell: "bash {{ firmware_run|default(firmware_pro_run) }} --nox11 --upgrade --quiet"
   register: firmware_up_result
   when: (firmware_run is defined and firmware_run|length > 0 or firmware_pro_run is defined and firmware_pro_run|length > 0) and (up_firm.matched > 0)
   failed_when: firmware_up_result.rc != 0 and firmware_up_result.rc != 2
 
+- name: set need_reboot_firmware fact
+  set_fact:
+    need_reboot_firmware: "{{'1' if 'Reboot' in firmware_up_result.stdout or 'reboot' in firmware_up_result.stdout else '0'}}"
+    cacheable: yes
+  when: firmware_up_result.changed
+
 - name: install firmware
   shell: "bash {{ firmware_run|default(firmware_pro_run) }} --nox11 --full --quiet"
   register: firmware_result
   when: (firmware_run is defined and firmware_run|length > 0 or firmware_pro_run is defined and firmware_pro_run|length > 0) and (up_firm.matched == 0)
   failed_when: firmware_result.rc != 0 and firmware_result.rc != 2
 
+- name: set need_reboot_firmware fact
+  set_fact:
+    need_reboot_firmware: "{{'1' if 'Reboot' in firmware_result.stdout or 'reboot' in firmware_result.stdout else '0'}}"
+    cacheable: yes
+  when: firmware_result.changed
+
 - name: message
   debug:
     msg:
       - "can not find firmware package, firmware install skipped"
   when: firmware_run is undefined and firmware_pro_run is undefined
 
 - name: message
```

## ascend_deployer/playbooks/install/task_kernels.yml

```diff
@@ -50,36 +50,99 @@
   when: ansible_user_uid == 0 and (kernels_310P.matched > 0 or kernels_910.matched > 0)
 
 - name: set log_path for non-root
   set_fact:
     log_path: ~/var/log/ascend_seclog/
   when: ansible_user_uid != 0 and (kernels_310P.matched > 0 or kernels_910.matched > 0)
 
+- name: get kernels version
+  shell: echo $(basename {{kernels_910_run.files[0].path}}) | awk -F '_' '{print $2}'
+  register: kernels_ver
+  when: kernels_910_run.matched > 0
+
+- name: set kernels_version fact
+  set_fact:
+    kernels_version: "{{kernels_ver.stdout}}"
+    cacheable: yes
+  when: kernels_910_run.matched > 0
+
+- name: get kernels version again
+  shell: echo $(basename {{kernels_310P_run.files[0].path}}) | awk -F '_' '{print $2}'
+  register: kernels_ver
+  when: kernels_910_run.matched == 0 and kernels_310P_run.matched > 0
+
+- name: set kernels_version fact again
+  set_fact:
+    kernels_version: "{{kernels_ver.stdout}}"
+    cacheable: yes
+  when: kernels_910_run.matched == 0 and kernels_310P_run.matched > 0
+
+- name: set kernels_version when can not find kernels
+  set_fact:
+    kernels_version: "NA"
+    cacheable: yes
+  when: kernels_910_run.matched == 0 and kernels_310P_run.matched == 0
+
+- name: check if toolkit is installed
+  find:
+    paths: "{{ascend_install_path}}/ascend-toolkit/{{kernels_version}}"
+    recurse: yes
+    file_type: file
+    use_regex: yes
+    patterns: "ascend_toolkit_install.info"
+  register: toolkit_status
+  when: kernels_version != 'NA'
+
+- name: check if nnae is installed
+  find:
+    paths: "{{ascend_install_path}}/nnae/{{kernels_version}}"
+    recurse: no
+    file_type: file
+    use_regex: yes
+    patterns: "ascend_nnae_install.info"
+  register: nnae_status
+  when: kernels_version != 'NA' and toolkit_status.matched == 0
+
+- name: message
+  debug:
+    msg:
+      - "The nnae and toolkit packages are not installed, kernels install skipped"
+  when: kernels_version != 'NA' and toolkit_status.matched == 0 and nnae_status.matched == 0
+
+- name: set kernels_type
+  set_fact:
+    kernels_type: "{{'toolkit' if toolkit_status.matched > 0 else 'nnae'}}"
+  when: kernels_version != 'NA'
+
 - name: install kernels using scripts for 310P
   shell: "bash {{ kernels_310P.files[0].path }} {{ log_path }} {{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_310P_result
-  when: kernels_310P.matched > 0
+  when:
+    - kernels_310P.matched > 0
+    - toolkit_status.matched > 0 or nnae_status.matched > 0
   failed_when: kernels_310P_result.rc != 0
 
 - name: message for 310P
   debug:
     msg:
       - "{{ kernels_310P_result | default('NOT DEFINED') }}"
   when: kernels_310P_result.changed
 
 - name: install kernels for 310P
   shell: "bash {{ kernels_310P_run.files[0].path }} --install --type={{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_310P_run_result
-  when: kernels_310P_run.matched > 0 and kernels_310P.matched == 0
+  when:
+    - kernels_310P_run.matched > 0 and kernels_310P.matched == 0
+    - toolkit_status.matched > 0 or nnae_status.matched > 0
   failed_when: kernels_310P_run_result.rc != 0
 
 - name: message for 310P
   debug:
     msg:
       - "{{ kernels_310P_run_result | default('NOT DEFINED') }}"
   when: kernels_310P_run_result.changed
@@ -92,30 +155,34 @@
 
 - name: install kernels using scripts for 910
   shell: "bash {{ kernels_910.files[0].path }} {{ log_path }} {{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910_result
-  when: kernels_910.matched > 0
+  when:
+    - kernels_910.matched > 0
+    - toolkit_status.matched > 0 or nnae_status.matched > 0
   failed_when: kernels_910_result.rc != 0
 
 - name: message for 910
   debug:
     msg:
       - "{{ kernels_910_result | default('NOT DEFINED') }}"
   when: kernels_910_result.changed
 
 - name: install kernels for 910
   shell: "bash {{ kernels_910_run.files[0].path }} --install --type={{ kernels_type }}"
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ansible_env.PATH}}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib"
   register: kernels_910_run_result
-  when: kernels_910_run.matched > 0 and kernels_910.matched == 0
+  when:
+    - kernels_910_run.matched > 0 and kernels_910.matched == 0
+    - toolkit_status.matched > 0 or nnae_status.matched > 0
   failed_when: kernels_910_run_result.rc != 0
 
 - name: message for 910
   debug:
     msg:
       - "{{ kernels_910_run_result | default('NOT DEFINED') }}"
   when: kernels_910_run_result.changed
```

## ascend_deployer/playbooks/install/task_mindspore.yml

```diff
@@ -1,48 +1,29 @@
-- name: find Ascend310 mindspore wheel package
+- name: find Ascend mindspore wheel package
   find:
-    paths: "{{ resources_dir }}/{{ os_and_arch }}/Ascend310/"
+    paths: "{{ resources_dir }}/pylibs/Ascend/"
     recurse: no
     file_type: file
     use_regex: yes
     patterns: "mindspore.*{{ ansible_architecture }}.whl"
-  register: mindspore_whl_310
+  register: mindspore_whl_ascend
   when:
-    - ansible_local.npu_info.scene == "infer"
+    - ansible_local.npu_info.scene != ""
 
-- name: find Ascend910 mindspore wheel package
-  find:
-    paths: "{{ resources_dir }}/{{ os_and_arch }}/Ascend910/"
-    recurse: no
-    file_type: file
-    use_regex: yes
-    patterns: "mindspore.*{{ ansible_architecture }}.whl"
-  register: mindspore_whl_910
-  when:
-    - ansible_local.npu_info.scene == "train" or ansible_local.npu_info.scene == "a910b"
-
-- name: install mindspore_ascend 310
-  shell: python3 -m pip install {{ mindspore_whl_310.files[0].path }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
-  environment:
-    PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
-    LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64:{{ local_path }}/gcc8.4.0/lib64"
-  when:
-    - mindspore_whl_310.matched is defined and mindspore_whl_310.matched > 0
-
-- name: install mindspore_ascend 910
-  shell: python3 -m pip install {{ mindspore_whl_910.files[0].path }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
+- name: install mindspore_ascend
+  shell: python3 -m pip install {{ mindspore_whl_ascend.files[0].path }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
   environment:
     PATH: "{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64:{{ local_path }}/gcc8.4.0/lib64"
   when:
-    - mindspore_whl_910.matched is defined and mindspore_whl_910.matched > 0
+    - mindspore_whl_ascend.matched is defined and mindspore_whl_ascend.matched > 0
 
 - name: find mindspore_cpu wheel package
   find:
-    paths: "{{ resources_dir }}/{{ os_and_arch }}/CPU/"
+    paths: "{{ resources_dir }}/pylibs/CPU/"
     recurse: no
     file_type: file
     use_regex: yes
     patterns: "mindspore.*{{ ansible_architecture }}.whl"
   register: mindspore_whl_cpu
   when:
     - ansible_local.npu_info.scene == ""
@@ -55,12 +36,11 @@
   when:
     - mindspore_whl_cpu.matched is defined and mindspore_whl_cpu.matched > 0
 
 - name: message
   debug:
     msg:
       - "os: {{ os_and_arch }}, scene: {{ ansible_local.npu_info.scene }}, mindspore install skipped"
-      - "maybe you should check mindspore whl package in dir: ascend-deployer/resources/{{ os_and_arch }}/Ascend910(or Ascend310 or CPU)/"
+      - "maybe you should check mindspore whl package in dir: ascend-deployer/resources/{{ os_and_arch }}/Ascend(or CPU)/"
   when:
-    - mindspore_whl_310.skipped is true
-    - mindspore_whl_910.skipped is true
+    - mindspore_whl_ascend.skipped is true
     - mindspore_whl_cpu.skipped is true
```

## ascend_deployer/playbooks/install/task_sys_apt.yml

```diff
@@ -1,18 +1,66 @@
+- name: copy gpg public key
+  copy:
+    src: "{{inventory_dir}}/resources/nexus/nexus_pub.asc"
+    dest: /etc/apt/trusted.gpg.d/
+    force: yes
+    mode: 0644
+  when:
+    - ansible_pkg_mgr != 'apt'
+
+- name: apt install system packages
+  shell: |
+    export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical
+    apt clean all
+    apt update -o Dir::Etc::sourcelist=/root/nexus/sources.list &>/dev/null
+    apt -f -y install
+    apt install -y {{sys_pkgs}} -o Dir::Etc::sourcelist=/root/nexus/sources.list
+  register: sys_result
+  environment:
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+    - ansible_pkg_mgr != 'apt'
+
+- name: message
+  debug:
+    msg:
+      - "{{ sys_result | default('NOT DEFINED') }}"
+  when: ansible_pkg_mgr != 'apt' and sys_result.changed
+
+- name: check if Docker is installed
+  shell: command -v docker | wc -l
+  register: docker_status
+  when:
+    - ansible_pkg_mgr != 'apt'
+
+- name: install Docker when Docker is not installed
+  shell: |
+    apt install -y {{docker_pkgs}} -o Dir::Etc::sourcelist=/root/nexus/sources.list
+  register: docker_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: ansible_pkg_mgr != 'apt' and docker_status.stdout == "0"
+
+- name: message
+  debug: var=docker_result
+  when:
+    - ansible_pkg_mgr != 'apt'
+    - docker_result.changed
+
 - name: apt install system packages
   shell: export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ resources_dir }}/{{ os_and_arch }}/*.deb
   when:
-      - ansible_pkg_mgr == 'apt'
-      - "'Linx' not in ansible_distribution"
+    - ansible_pkg_mgr == 'apt'
   register: sys_result
 
-- name: apt install system packages in Linx OS
-  shell: export DEBIAN_FRONTEND=noninteractive && export DEBIAN_PRIORITY=critical; dpkg --force-all -i {{ resources_dir }}/Linx_{{ os_version }}_{{ ansible_architecture }}/*.deb
-  when: "'Linx' in ansible_distribution"
-  register: sys_result_linx
-
 - name: message
   debug:
     msg:
       - "{{ sys_result | default('NOT DEFINED') }}"
-      - "{{ sys_result_linx | default('NOT DEFINED') }}"
   when: sys_result.changed or sys_result_linx.changed
```

## ascend_deployer/playbooks/install/task_sys_dnf.yml

```diff
@@ -2,15 +2,62 @@
   include_tasks: task_kernel.yml
   when: "'EulerOS' in os_and_arch"
 
 - name: install kernel headers devel force for euler
   include_tasks: task_kernel_euleros.yml
   when: "'EulerOS' in os_and_arch"
 
-# currently dnf also use rpm to install
+- name: install system packages
+  shell: |
+    yum clean all &>/dev/null
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y {{sys_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
+  register: sys_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: "'OpenEuler_22.03LTS' in os_and_arch"
+
+- name: message
+  debug: var=sys_result
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - sys_result.changed
+
+- name: check if Docker is installed
+  shell: command -v docker | wc -l
+  register: docker_status
+  when: "'OpenEuler_22.03LTS' in os_and_arch"
+
+- name: install Docker when Docker is not installed
+  shell: |
+    yum install -y {{docker_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
+  register: docker_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - docker_status.stdout == "0"
+
+- name: message
+  debug: var=docker_result
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - docker_result.changed
+
 - name: dnf install system packages
   shell: rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/*.rpm
   register: sys_result
+  when: "'OpenEuler_22.03LTS' not in os_and_arch"
 
 - name: message
   debug: var=sys_result
-  when: sys_result.changed
+  when:
+    - "'OpenEuler_22.03LTS' not in os_and_arch"
+    - sys_result.changed
```

## ascend_deployer/playbooks/install/task_sys_pkg.yml

```diff
@@ -1,16 +1,100 @@
-- name: check docker exists
-  shell: command -v docker | wc -l
-  register: docker_status
-
-- name: message
-  debug:
-    msg: "[WARNING] Docker is already installed on the system, and errors may occur when installing system dependencies"
-  changed_when: true
-  when: docker_status.stdout != "0"
+- name: get nexus ip
+  shell: env | grep SSH_CONNECTION | awk '{print $3}'
+  register: nexus_ip
+  delegate_to: localhost
+  run_once: true
+
+- name: set nexus_url fact
+  set_fact:
+    nexus_url: "http://{{nexus_ip.stdout}}:58081"
+    cacheable: true
+
+- name: clean nexus dir
+  file:
+    state: absent
+    path: ~/nexus
+
+- name: copy nexus_config.json
+  copy:
+    src: "{{inventory_dir}}/scripts/nexus_config.json"
+    dest: ~/nexus/
+    force: yes
+
+- name: get nexus config
+  shell: cat ~/nexus/nexus_config.json
+  register: nexus_config
+
+- name: set nexus_data fact
+  set_fact:
+    nexus_data: "{{nexus_config.stdout|from_json}}"
+    cacheable: yes
+
+- name: set nexus codename fact
+  set_fact:
+    nexus_codename: "{{nexus_data.codename.get(os_and_arch)}}"
+    cacheable: yes
+  when: os_and_arch in nexus_data.deb_os
+
+- name: touch sources config file for deb
+  shell: echo "deb {{nexus_url}}/repository/{{os_and_arch}}/ {{nexus_codename}} main" > ~/nexus/sources.list
+  when: os_and_arch in nexus_data.deb_os
+
+- name: touch sources config file for rpm
+  shell: |
+    cat <<EOF >~/nexus/sources.repo
+    [nexus]
+    name = {{os_and_arch}}
+    baseurl = {{nexus_url}}/repository/{{os_and_arch}}/
+    gpgcheck=0
+    enabled=1
+    EOF
+  when: os_and_arch in nexus_data.rpm_os
+
+- name: copy pkg_info.json
+  copy:
+    src: "{{inventory_dir}}/downloader/config/{{os_and_arch}}/pkg_info.json"
+    dest: ~/nexus/
+    force: yes
+
+- name: get pkg info
+  shell: cat ~/nexus/pkg_info.json
+  register: pkg_info
+
+- name: set json_data fact
+  set_fact:
+    json_data: "{{pkg_info.stdout | from_json}}"
+    cacheable: yes
+
+- name: set sys_pkgs_list fact
+  set_fact:
+    sys_pkgs_list: "{{json_data|map(attribute='name') | list}}"
+    cacheable: yes
+
+- name: set docker pkg for common OS
+  set_fact:
+    docker_pkgs_list: "{{nexus_data.common_docker}}"
+    cacheable: yes
+  when: "'EulerOS' not in os_and_arch"
+
+- name: set docker pkg for EulerOS OS
+  set_fact:
+    docker_pkgs_list: "{{nexus_data.euler_docker}}"
+    cacheable: yes
+  when: "'EulerOS' in os_and_arch"
+
+- name: set sys_pkgs fact
+  set_fact:
+    sys_pkgs: "{{sys_pkgs_list | difference(docker_pkgs_list) | join(' ')}}"
+    cacheable: yes
+
+- name: set docker_pkgs fact
+  set_fact:
+    docker_pkgs: "{{docker_pkgs_list | join(' ')}}"
+    cacheable: yes
 
 - name: install system packages
   include_tasks: "task_sys_{{ansible_pkg_mgr}}.yml"
 
 - name: get cmake version
   shell: cmake --version | awk -F" " '{print $3;exit}'
   register: cmake_ver
@@ -30,15 +114,16 @@
     patterns: "libprotobuf.so.*"
   register: libprotobuf
 
 - name: install protobuf 3.13.0
   import_tasks: task_protobuf.yml
   when: libprotobuf.matched == 0
 
-- name: find docker command
-  shell: command -v docker | wc -l
-  register: docker_exists
+- name: check docker status
+  shell: docker ps
+  register: docker_status
+  failed_when: false
 
 - name: restart docker
   shell: "systemctl restart docker"
-  when: docker_exists.stdout != "0"
+  when: docker_status.rc != 0
   failed_when: false
```

## ascend_deployer/playbooks/install/task_sys_yum.yml

```diff
@@ -3,13 +3,61 @@
   when: "'EulerOS' in os_and_arch"
 
 - name: install kernel headers devel force for euler
   include_tasks: task_kernel_euleros.yml
   when: "'EulerOS' in os_and_arch"
 
 - name: yum install system packages
+  shell: |
+    yum clean all &>/dev/null
+    yum makecache --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo &>/dev/null
+    yum install --skip-broken -y {{sys_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
+  register: sys_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when: "'OpenEuler_22.03LTS' in os_and_arch"
+
+- name: message
+  debug: var=sys_result
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - sys_result.changed
+
+- name: check if Docker is installed
+  shell: command -v docker | wc -l
+  register: docker_status
+  when: "'OpenEuler_22.03LTS' in os_and_arch"
+
+- name: install Docker when Docker is not installed
+  shell: |
+    yum install -y {{docker_pkgs}} --disablerepo="*" --enablerepo=nexus -c ~/nexus/sources.repo
+  register: docker_result
+  environment:
+    LD_LIBRARY_PATH: ""
+    http_proxy: ""
+    https_proxy: ""
+    HTTP_PROXY: ""
+    HTTPS_PROXY: ""
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - docker_status.stdout == "0"
+
+- name: message
+  debug: var=docker_result
+  when:
+    - "'OpenEuler_22.03LTS' in os_and_arch"
+    - docker_result.changed
+
+- name: yum install system packages
   shell: rpm -ivh --force --nodeps --replacepkgs {{ resources_dir }}/{{ os_and_arch }}/*.rpm
   register: sys_result
+  when: "'OpenEuler_22.03LTS' not in os_and_arch"
 
 - name: message
   debug: var=sys_result
-  when: sys_result.changed
+  when:
+    - "'OpenEuler_22.03LTS' not in os_and_arch"
+    - sys_result.changed
```

## ascend_deployer/playbooks/install/task_tensorflow.yml

```diff
@@ -19,15 +19,7 @@
 
 - name: install tensorflow
   shell: python3 -m pip install tensorflow=={{ tensorflow_version }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
   environment:
     PATH: "{{ local_path }}/gcc7.3.0/bin:{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
     LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64"
     CPATH: /usr/include/hdf5/include/:/usr/include/hdf5/lib/
-  when: ansible_architecture == 'aarch64'
-
-- name: install tensorflow_cpu
-  shell: python3 -m pip install tensorflow_cpu=={{ tensorflow_version }} --no-index --find-links {{ resources_dir }}/pylibs {{ pip_install_option }}
-  environment:
-    PATH: "{{ local_path }}/gcc7.3.0/bin:{{ local_path }}/{{ python_version }}/bin:{{ ansible_env.PATH }}"
-    LD_LIBRARY_PATH: "{{ local_path }}/{{ python_version }}/lib:{{ local_path }}/gcc7.3.0/lib64"
-  when: ansible_architecture == 'x86_64'
```

## ascend_deployer/playbooks/scene/scene_auto.yml

```diff
@@ -1,14 +1,14 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install toolkit
   import_playbook: ../install/install_toolkit.yml
```

## ascend_deployer/playbooks/scene/scene_mindspore.yml

```diff
@@ -1,16 +1,19 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install toolkit
   import_playbook: ../install/install_toolkit.yml
 
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
+
 - name: install mindspore
   import_playbook: ../install/install_mindspore.yml
```

## ascend_deployer/playbooks/scene/scene_offline_dev.yml

```diff
@@ -1,13 +1,16 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install toolkit
   import_playbook: ../install/install_toolkit.yml
+
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
```

## ascend_deployer/playbooks/scene/scene_offline_run.yml

```diff
@@ -1,13 +1,13 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install nnrt
   import_playbook: ../install/install_nnrt.yml
```

## ascend_deployer/playbooks/scene/scene_pytorch_dev.yml

```diff
@@ -1,16 +1,19 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install toolkit
   import_playbook: ../install/install_toolkit.yml
 
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
+
 - name: install pytorch
   import_playbook: ../install/install_pytorch.yml
```

## ascend_deployer/playbooks/scene/scene_pytorch_run.yml

```diff
@@ -1,16 +1,19 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install nnae
   import_playbook: ../install/install_nnae.yml
 
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
+
 - name: install pytorch
   import_playbook: ../install/install_pytorch.yml
```

## ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml

```diff
@@ -1,19 +1,22 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install toolkit
   import_playbook: ../install/install_toolkit.yml
 
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
+
 - name: install tfplugin
   import_playbook: ../install/install_tfplugin.yml
 
 - name: install tensorflow
   import_playbook: ../install/install_tensorflow.yml
```

## ascend_deployer/playbooks/scene/scene_tensorflow_run.yml

```diff
@@ -1,19 +1,22 @@
 - hosts: '{{ hosts_name }}'
 
 - name: install system dependencies
   import_playbook: ../install/install_sys_pkg.yml
 
 - name: install {{ python_version }}
-  import_playbook: ../install/install_python375.yml
+  import_playbook: ../install/install_python.yml
 
 - name: install driver and firmware
   import_playbook: ../install/install_npu.yml
 
 - name: install nnae
   import_playbook: ../install/install_nnae.yml
 
+- name: install kernels
+  import_playbook: ../install/install_kernels.yml
+
 - name: install tfplugin
   import_playbook: ../install/install_tfplugin.yml
 
 - name: install tensorflow
   import_playbook: ../install/install_tensorflow.yml
```

## Comparing `ascend_deployer/README.rst` & `ascend_deployer-5.0.0b4.dist-info/DESCRIPTION.rst`

 * *Files 0% similar despite different names*

```diff
@@ -80,7 +80,9 @@
 
    ::
 
       source /usr/local/ascendrc                # 配置python环境变量
       source /usr/local/Ascend/nnae/set_env.sh  # 配置nnae的环境变量
 
 8. 详细指南请参考\ `ascend-deployer用户指南 <https://www.hiascend.com/document/detail/zh/ascend-deployer>`__\
+
+
```

## Comparing `ascend_deployer/downloader/downloader_ui.py` & `ascend_deployer/downloader_ui.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,217 +1,170 @@
 #!/usr/bin/env python3
 # coding: utf-8
-# Copyright 2020 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ===========================================================================
 """gui application using tk"""
-import configparser
-import os
-import sys
 import tkinter as tk
 import tkinter.messagebox
+from tkinter import ttk
 
-
-CUR_DIR = os.path.dirname(os.path.realpath(__file__))
-OS_LIST = os.listdir(os.path.join(CUR_DIR, 'config'))
-PKG_LIST = [pkg.split(".json")[0] for pkg in os.listdir(os.path.join(CUR_DIR, 'software'))]
+import ascend_download
+from downloader.download_util import check_version_matched, State
+from utils import os_items, pkg_items
 
 
 class Win(object):
     """
-    the basic window
+    downloader ui window
     """
 
     def __init__(self):
-        self.config_file = os.path.join(CUR_DIR, 'config.ini')
         self.root = tk.Tk()
         self.root.title('离线安装下载器')
-        self.root.geometry('620x500')
-        self.root.protocol('WM_DELETE_WINDOW', self.on_closing)
-        self.frame_left = self._create_frame("OS_LIST", 0, 0, 250, 480, "left")
-        self.frame_right = self._create_frame("PKG_LIST", 0, 2, 250, 480, "left")
-        self.frame_bottom = tk.LabelFrame(
-            tk.Button(self.root, text="开始下载").grid(row=0, column=1)
-        )
-        self.frame_bottom.grid(row=0, column=1)
-        self.all_opt = tk.IntVar()
-        self.all_opt.set(1)
-        self.all_not_opt = tk.IntVar()
-        self.all_not_opt.set(0)
+        self.root.geometry('620x480')
+        self.root.resizable(False, False)
+        self.root.protocol('WM_DELETE_WINDOW', self.root.destroy)
+
         self.os_dict = {}
         self.pkg_dict = {}
-        tk.Button(self.frame_left, text="全选",
-                  command=lambda: self.select_os_all(self.all_opt)).grid(row=0, column=0, sticky='w')
-        tk.Button(self.frame_left, text="全不选",
-                  command=lambda: self.select_os_all(self.all_not_opt)).grid(row=0, column=0)
-        tk.Button(self.frame_right, text="全选",
-                  command=lambda: self.select_pkg_all(self.all_opt)).grid(row=0, column=0, sticky='w')
-        tk.Button(self.frame_right, text="全不选",
-                  command=lambda: self.select_pkg_all(self.all_not_opt)).grid(row=0, column=0)
-        tk.Button(self.frame_bottom, text='开始下载',
-                  command=self.start_download).pack()
-        self.read_config()
-        self.display()
-
-    def _create_frame(self, text, row, column, width, heigh, pack_side):
-        box = tk.LabelFrame(self.root, text=text)
-        box.grid(row=row, column=column)
-        canvas = tk.Canvas(box)
-        canvas.pack(side=pack_side, fill="both", expand=True)
-        frame = tk.Frame(canvas)
-        scrollbar = tk.Scrollbar(box, orient="vertical", command=canvas.yview)
-        canvas.configure(
-            yscrollcommand=scrollbar.set, width=width, height=heigh
-        )
-        scrollbar.pack(side=pack_side, fill="y")
-        frame.bind(
-            "<Configure>",
-            lambda event, canvas=canvas: self._on_frame_configure(canvas)
+        self.os_list = []
+        self.pkg_list = []
+        self.combo_list = []
+        self.init()
+        self.layout()
+
+    def layout(self):
+        frame_left = self.create_frame("OS_LIST", 0, True)
+        frame_right = self.create_frame("PKG_LIST", 2, False)
+        frame_middle = tk.LabelFrame(
+            tk.Button(self.root, text="开始下载").grid(row=0, column=1)
         )
-        canvas.create_window((4, 4), window=frame, anchor="nw", tags="frame")
-        return frame
-
-    @staticmethod
-    def _on_frame_configure(canvas):
-        canvas.configure(scrollregion=canvas.bbox("all"))
-
-    def display(self):
-        """
-        display the Checkbutton
-        """
-        os_idx, pkg_idx = 0, 0
+        frame_middle.grid(row=0, column=1, padx=5)
+        tk.Button(frame_left, text="全选",
+                  command=self.select_all_os).grid(row=0, column=0, sticky='w')
+        tk.Button(frame_left, text="全不选",
+                  command=self.unselect_all_os).grid(row=0, column=0)
+        tk.Button(frame_right, text="清空",
+                  command=self.unselect_all_pkg).grid(row=0, column=0, sticky='w')
+        tk.Button(frame_middle, text='开始下载',
+                  command=self.start_download).pack()
+        os_idx = 0
         for os_name, var in sorted(self.os_dict.items()):
             os_idx += 1
-            tk.Checkbutton(self.frame_left, width=30, text=os_name,
+            tk.Checkbutton(frame_left, width=30, text=os_name,
                            variable=var, anchor='w').grid(row=os_idx,
                                                           column=0)
-        for pkg_name, var in sorted(self.pkg_dict.items()):
-            pkg_idx += 1
-            tk.Checkbutton(self.frame_right, width=30, text=pkg_name,
-                           variable=var, anchor='w').grid(row=pkg_idx,
-                                                          column=0)
+
+        for i, name in enumerate(sorted(self.pkg_dict.keys())):
+            tk.Label(frame_right, text=name).grid(row=i + 1, sticky='W')
+            combo = ttk.Combobox(frame_right, textvariable=tk.StringVar(), state='readonly')
+            combo['value'] = self.pkg_dict.get(name, [])
+            combo.grid(row=i + 1, sticky='W', padx=80, pady=5)
+            self.combo_list.append([name, combo])
 
     def run(self):
         """
         the main loop of the window
         """
         self.root.mainloop()
 
     def start_download(self):
         """
-        start downading, the window will exit
+        start downloading, the window will exit
         """
-        self.write_config()
-        config = configparser.ConfigParser()
-        config.read(self.config_file)
-
-        if not config['download']['os_list'] and not config['software']['pkg_list']:
-            tkinter.messagebox.showwarning(title="Warning", message="至少勾选一项")
-        elif not config['download']['os_list'] and "MindSpore" in config['software']['pkg_list']:
-            tkinter.messagebox.showwarning(title="Warning", message="下载MindSpore时OS_LIST至少勾选一项")
-        elif not config['download']['os_list'] and "MindStudio" in config['software']['pkg_list']:
-            tkinter.messagebox.showwarning(title="Warning", message="下载MindStudio时OS_LIST至少勾选一项")
+        self.refresh_data()
+        check_stat, msg = check_version_matched(self.os_list, self.pkg_list)
+        if not self.os_list or not self.pkg_list:
+            tkinter.messagebox.showwarning(title="Warning", message="os_list和pkg_list必须勾选")
+        elif check_stat == State.EXIT:
+            tkinter.messagebox.showwarning(title="Warning", message=msg)
+        elif check_stat == State.ASK:
+            if tkinter.messagebox.askyesnocancel(title="Warning", message=msg + ", need to force download or not?"):
+                self.work()
         else:
-            self.root.destroy()
-            sys.exit(0)
+            self.work()
 
-    def read_config(self):
+    def init(self):
         """
-        read the configuration file
+        init os_dict and pkg_dict
         """
-        config = configparser.ConfigParser()
-        config.read(self.config_file)
-        configured_os = [t.strip() for t in config['download']['os_list'].split(',') if t]
-        configured_pkg = [t.strip() for t in config['software']['pkg_list'].split(',') if t]
-        not_configured_os = list(set(OS_LIST) - set(configured_os))
-        not_configured_pkg = list(set(PKG_LIST) - set(configured_pkg))
-        for os_name in configured_os:
-            var = tk.IntVar()
-            var.set(1)
-            self.os_dict[os_name] = var
-        for os_name in not_configured_os:
+        for os_name in os_items:
             var = tk.IntVar()
             var.set(0)
             self.os_dict[os_name] = var
-        for pkg_name in configured_pkg:
-            var = tk.IntVar()
-            var.set(1)
-            self.pkg_dict[pkg_name] = var
-        for pkg_name in not_configured_pkg:
-            var = tk.IntVar()
-            var.set(0)
-            self.pkg_dict[pkg_name] = var
+        for pkg_name in pkg_items:
+            if '=' not in pkg_name:
+                continue
+            name, version = pkg_name.split('==')
+            self.pkg_dict.setdefault(name, []).append(version)
 
-    def write_config(self):
+    def refresh_data(self):
         """
-        write the configuration file
+        refresh os_list and pkg_list
         """
-        config = configparser.ConfigParser()
-        config.read(self.config_file)
-
-        oslist = []
+        self.os_list.clear()
         for os_name, var in sorted(self.os_dict.items()):
             if var.get() == 1:
-                oslist.append(os_name)
-        config['download']['os_list'] = ','.join(oslist)
+                self.os_list.append(os_name)
 
-        pkg_list = []
-        for pkg_name, var in sorted(self.pkg_dict.items()):
-            if var.get() == 1:
-                pkg_list.append(pkg_name)
-        config['software']['pkg_list'] = ','.join(pkg_list)
-        fd = os.open(self.config_file, os.O_WRONLY, 0o640)
-        cfg = os.fdopen(fd, 'w+')
-        cfg.truncate()
-        config.write(cfg, space_around_delimiters=False)
-        cfg.close()
-
-    def select_os_all(self, opt):
-        """
-        select os all
-        """
-        if opt.get() == 1:
-            for os_name in OS_LIST:
-                self.os_dict[os_name].set(1)
-        else:
-            for os_name in OS_LIST:
-                self.os_dict[os_name].set(0)
+        self.pkg_list.clear()
+        for name, combo in self.combo_list:
+            if combo.get() != "":
+                self.pkg_list.append('{}=={}'.format(name, combo.get()))
+
+    def select_all_os(self):
+        for item in os_items:
+            self.os_dict.get(item).set(1)
+
+    def unselect_all_os(self):
+        for item in os_items:
+            self.os_dict.get(item).set(0)
+
+    def unselect_all_pkg(self):
+        for _, combo in self.combo_list:
+            combo.set('')
 
-        self.display()
+    def create_frame(self, text, column, scroll):
+        box = tk.LabelFrame(self.root, text=text)
+        box.grid(row=0, column=column)
+        canvas = tk.Canvas(box)
+        canvas.pack(side='left', fill="both", expand=True)
+        frame = tk.Frame(canvas)
+        scrollbar = tk.Scrollbar(box, orient="vertical", command=canvas.yview)
+        canvas.configure(
+            yscrollcommand=scrollbar.set, width=250, height=450
+        )
+        if scroll:
+            scrollbar.pack(side='left', fill="y")
 
-    def select_pkg_all(self, opt):
-        """
-        select pkg all
-        """
-        if opt.get() == 1:
-            for pkg_name in PKG_LIST:
-                self.pkg_dict[pkg_name].set(1)
-        else:
-            for pkg_name in PKG_LIST:
-                self.pkg_dict[pkg_name].set(0)
+        def on_frame_configure(_):
+            canvas.configure(scrollregion=canvas.bbox("all"))
 
-        self.display()
+        frame.bind("<Configure>", on_frame_configure)
+        canvas.create_window((4, 4), window=frame, anchor="nw", tags="frame")
+        return frame
 
-    def on_closing(self):
-        """
-        closing the window and exit
-        """
+    def work(self):
         self.root.destroy()
-        sys.exit(1)
+        ascend_download.main(
+            args=['--os-list', ','.join(self.os_list), '--download', ','.join(self.pkg_list)],
+            check=False
+        )
 
 
 def win_main():
     """
     start gui application
     """
     app = Win()
```

## Comparing `ascend_deployer/playbooks/install/task_python375.yml` & `ascend_deployer/playbooks/install/task_python.yml`

 * *Files identical despite different names*

## Comparing `ascend_deployer-5.0.0b3.data/scripts/ascend-deployer` & `ascend_deployer-5.0.0b4.data/scripts/ascend-deployer`

 * *Files identical despite different names*

## Comparing `ascend_deployer-5.0.0b3.dist-info/DESCRIPTION.rst` & `ascend_deployer-5.0.0b4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.0
+Name: ascend-deployer
+Version: 5.0.0b4
+Summary: ascend offline installer
+Home-page: https://gitee.com/ascend/ascend-deployer
+License: Apache
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >= 3.6
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: NOTICE
+
 .. sectnum::
 
 简介
 =======
 
 离线安装工具提供系统组件、python第三方依赖自动下载以及一键式安装的功能，并支持驱动、固件以及CANN软件包的安装。
```

## Comparing `ascend_deployer-5.0.0b3.dist-info/metadata.json` & `ascend_deployer-5.0.0b4.dist-info/metadata.json`

 * *Files 11% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9507575757575757%*

 * *Differences: {"'extensions'": "{'python.commands': {'wrap_console': {'ascend-download': "*

 * *                 "'ascend_deployer.ascend_download:main'}}, 'python.exports': {'console_scripts': "*

 * *                 "{'ascend-download': 'ascend_deployer.ascend_download:main'}}}",*

 * * "'version'": "'5.0.0b4'"}*

```diff
@@ -4,33 +4,33 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent"
     ],
     "description_content_type": "text/x-rst",
     "extensions": {
         "python.commands": {
             "wrap_console": {
-                "ascend-download": "ascend_deployer.downloader.downloader:main"
+                "ascend-download": "ascend_deployer.ascend_download:main"
             }
         },
         "python.details": {
             "document_names": {
                 "description": "DESCRIPTION.rst"
             },
             "project_urls": {
                 "Home": "https://gitee.com/ascend/ascend-deployer"
             }
         },
         "python.exports": {
             "console_scripts": {
-                "ascend-download": "ascend_deployer.downloader.downloader:main"
+                "ascend-download": "ascend_deployer.ascend_download:main"
             }
         }
     },
     "generator": "bdist_wheel (0.30.0)",
     "license": "Apache",
     "license_file": "LICENSE",
     "metadata_version": "2.0",
     "name": "ascend-deployer",
     "requires_python": ">= 3.6",
     "summary": "ascend offline installer",
-    "version": "5.0.0b3"
+    "version": "5.0.0b4"
 }
```

## Comparing `ascend_deployer-5.0.0b3.dist-info/RECORD` & `ascend_deployer-5.0.0b4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,208 +1,217 @@
-ascend_deployer/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ascend_deployer/README.en.rst,sha256=Dzxbc26GokNQh0SNYs6o2uL4_fkoRVHwG5tf9AlHN04,67023
-ascend_deployer/README.rst,sha256=R_J7UCgGEDCIY9PhaEzMZXJW9DKSEcFgBHlF7G05Yi8,4129
-ascend_deployer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ascend_deployer/ansible.cfg,sha256=YVG-6i-sohTyLRF3zNzALM8M6nm6LkuMdTan2H0if64,244
-ascend_deployer/install.sh,sha256=Ck_qW19IwJIDGZLyY2xEBhGFYS5HOx1b_ipa-iNX1o8,61429
-ascend_deployer/inventory_file,sha256=4V8POz1njlE9zXXhBePOPkOuPiShxNO2DqzUKgWk-fg,125
-ascend_deployer/start_download.bat,sha256=G71xW_anaQ1vt6aFkkq38vwaiCdGc7vS8VL9-7KwfmA,46
-ascend_deployer/start_download.sh,sha256=3kpmBHObtAW7QOLko9ibd8NN1KUXSmMdkgWuxggUwHw,10751
-ascend_deployer/start_download_ui.bat,sha256=oOjFSHADbqxRj4psOU9HqQRL1cx2CcY2XMka3bMxK-E,112
-ascend_deployer/downloader/__init__.py,sha256=vDleqozXpbjkaQaK8RgEtSmG7XUBYtSxnzHLczCADUs,2104
-ascend_deployer/downloader/config.ini,sha256=cnTL7ONeMBRNB6tmSba1Dmts7oO-aFx5X0TbOJmpWB4,325
-ascend_deployer/downloader/deb_downloader.py,sha256=Q6e4xAuP57WUCHllzqI-sICyw3i7ekZJfvFn0wjqsXg,11164
-ascend_deployer/downloader/download_util.py,sha256=adQL6Lx1OWHI-J9Z-Fq6u5NKP9ygs4qZTxEdGy_mWJg,21026
-ascend_deployer/downloader/downloader.py,sha256=0ar3C0g0Rmd-TkPREZxj7HXT6Z3o0yhlni1B5gG2qmg,8717
-ascend_deployer/downloader/downloader_ui.py,sha256=vJPoyPcp2D3poXFyNnc5I-eqIb3oChlqP3YkUO0UdWU,7914
+ascend_deployer/Inventory_Template.CSV,sha256=0j1bDd9jpDhgrMpiih_q7cvotkM3mT9_M0MjyNEBEZg,797
+ascend_deployer/__init__.py,sha256=3geaeGzhrlHQWFzpr3TqJSebV4Xzi1goFBjRH-QgqpQ,769
+ascend_deployer/ansible.cfg,sha256=_xFcFD4oavHhko4NCrmpx-9frb2Iyj0z3t7il0aPniw,348
+ascend_deployer/ascend_deployer.py,sha256=O-LKT0cfiQTlZCAiznlwh_T6kj-UJnJigySE7cQV2GI,6434
+ascend_deployer/ascend_download.py,sha256=fkFrUcmM7jnZxB3PrSkEAPWUgH0viq8sF9ebyiHUNzs,2076
+ascend_deployer/downloader_ui.py,sha256=rdYUohHoCRkKQUXDxLIgssg59HoA665DdEsglpAR_lc,5986
+ascend_deployer/install.sh,sha256=dK1jcjQQfQfKQGBDaavVzB0Le_2rkcW4Ie2CMmBvgbE,16597
+ascend_deployer/inventory_file,sha256=QVuje0dBIH-kWmdnWo32v_8mFsogbKDmCsQ4dftx4M8,491
+ascend_deployer/jobs.py,sha256=W0ubAfyXMLN7xEBBlxE6TvYhzeCzhKgpF_Z4w4NGsYY,3379
+ascend_deployer/start_download.sh,sha256=V0gI6j99_6QqgLom3WColQJf8P1Rh4dwzJmqIn76ey8,3367
+ascend_deployer/start_download_ui.bat,sha256=S4Aporvo3W__1O77dLC7JY0y-v6I8petduDdM8gsNEQ,57
+ascend_deployer/utils.py,sha256=yaH-U2aTr3ftl3b0OuxS-WVw8rCIt7Sx1OOzIvDKEmc,4507
+ascend_deployer/version.json,sha256=HA6x_geHEIgQPolmzJ-qv1Zmt6ESu2S6xXnvn-gxAPk,54
+ascend_deployer/ansible_plugin/ansible_log.py,sha256=GrqIc5VPUTMqfmlfRcyKt0y-Ge0um3CWNfUsd7NUx-c,13617
+ascend_deployer/ansible_plugin/install_info.yaml,sha256=sv6NOIG0Ii2IRXCefbq2oCyz3BqAOG9r61FPg8JZ1fo,1123
+ascend_deployer/downloader/__init__.py,sha256=GpJGe2tXVoYiy8NSeW42G8XULrTkL-ZPV-bgNYZXXwE,2218
+ascend_deployer/downloader/config.ini,sha256=NvDponJ-1G_1iY2IpXhwP0DCdhBYpFRdPiwJH74OhzY,137
+ascend_deployer/downloader/deb_downloader.py,sha256=yZN5A3sQP-3oKXfNo05LuHU0wwVY2E1RjO9vITEnV4E,11014
+ascend_deployer/downloader/dl_mef_dependency_downloader.py,sha256=il55l-wp0Vk2IwA14ZDTNrNLcC3bf_jCGid48UmGFCs,3811
+ascend_deployer/downloader/download_util.py,sha256=E27jty-tPLB7p-QtsdKkqKGSpDfEUPi79jgihFDX5tU,17797
+ascend_deployer/downloader/downloader.py,sha256=_MfeLZhGpbcDvKXaz5HpJb90wTXNjcqfcd9LNP-d99Y,15709
 ascend_deployer/downloader/logger_config.py,sha256=EuUhFLUkMWkslKgNgzcDte_WxyJ6X6Lcv8gDPF2Se4o,4552
-ascend_deployer/downloader/os_dep_downloader.py,sha256=9AeZZAxYyN0OHrPwoamOomCRY0lIITEsI3UhJmSpLnw,4470
-ascend_deployer/downloader/other_downloader.py,sha256=te9ar50weftVaMlM976EzYEwqgoyWXkMt2XA7YVy2EM,12509
-ascend_deployer/downloader/other_resources.json,sha256=2Wf5qxHkyPW6FbIMLBOhetg2SRlRfGbR_iBZh02xGNI,2258
-ascend_deployer/downloader/pip_downloader.py,sha256=biqiRR3I74m0Wmua0v-xkZkYC7Uz3yWHg_DSP7Vtq-I,11816
+ascend_deployer/downloader/obs_resources.json,sha256=DY1ixcTYQRxFcWALN5C9WvPhRg5Hf7s91214Brs9MJ4,2730
+ascend_deployer/downloader/os_dep_downloader.py,sha256=OxvmabobxJ2Q7hfM7Iv8EHwej-rkiBDHYqTnPjTqxW4,4562
+ascend_deployer/downloader/other_downloader.py,sha256=43p0UbvjxR7LETFjzbqDPmkXC-2ZxBaOG2llY77YZDY,14390
+ascend_deployer/downloader/other_resources.json,sha256=zf7TLLS3dmwpBC6hvsalgNswBdxkABxyVtDq2yQKx3c,2870
+ascend_deployer/downloader/pip_downloader.py,sha256=lFEfmAUJYXxJmcR266AKEylV2blF1y8QTU-H6f9xkWM,13377
 ascend_deployer/downloader/python_version.json,sha256=9pSqHUoRuHczku4tbP66Io8q519P8zCnDbPd49mgX38,8754
-ascend_deployer/downloader/requirements.txt,sha256=58g-jcQXeA5eyYidbbpTHY2W_eYTDOHGjLJtG0Afotc,1783
-ascend_deployer/downloader/rpm_downloader.py,sha256=nbFxt43J-QTzvwWDFaKMJXnTVzgsr6Ry9XWJGJoFqXc,21007
-ascend_deployer/downloader/software_mgr.py,sha256=qqOKezFYc3TaTIJ0o7iwnfMSyj2DXT2dsxnNzGsccOc,7161
+ascend_deployer/downloader/requirements.txt,sha256=6camZ9H2M60scc935IpL6edSsyKJNKVhN_tjX4fHwxM,1775
+ascend_deployer/downloader/rpm_downloader.py,sha256=KBFLBDltYR4HWh5ku5IIiSiRXP4lYMU-606r_GWiJEM,20876
+ascend_deployer/downloader/software_mgr.py,sha256=5JIjLKwSmkh6QjlXmLon_2AFjhd0_onJGvurhc45BBE,8430
 ascend_deployer/downloader/support_url.json,sha256=72oucjrIKKoIF1QEaOyNhd8JOvpCfTADNWk7Gf4lobs,284
-ascend_deployer/downloader/__pycache__/deb_downloader.cpython-36.pyc,sha256=GI0LVI5Zk8mKJRDmGJx-peYvl5ZOZ-2yOO1IVzBlpLQ,9087
-ascend_deployer/downloader/__pycache__/download_util.cpython-36.pyc,sha256=Kwo8EL5kQEsAPVzSVSSuc0kamMRKbadl7jz3tY8yh1A,18614
-ascend_deployer/downloader/__pycache__/downloader.cpython-36.pyc,sha256=BbQtmje--wrOx7OSf_YpIrFOVZb4LnEHFVDSo3Ep0XM,6124
-ascend_deployer/downloader/__pycache__/logger_config.cpython-36.pyc,sha256=zO4nk9wn5pntbMyzX99FQTovxcjJpgaExQI1TvKdtc0,3190
-ascend_deployer/downloader/__pycache__/os_dep_downloader.cpython-36.pyc,sha256=rpaaLQY9DJbwgUqrRIPRA_IIwqGZtG_93CstWTD3zK8,3350
-ascend_deployer/downloader/__pycache__/other_downloader.cpython-36.pyc,sha256=YgPj0RofxKlV-J-NSowaakc6Cb-0RQiI-AqYVmIEfSQ,8456
-ascend_deployer/downloader/__pycache__/pip_downloader.cpython-36.pyc,sha256=oW9jtXRUCy44SPR7rHTf8EQ6K0xQ7OH42bXauBBhVxs,9460
-ascend_deployer/downloader/__pycache__/rpm_downloader.cpython-36.pyc,sha256=y9pq0U_pJlcrj-MNpY607vwJ5sVR2YcSr0DaILduIA4,15637
-ascend_deployer/downloader/__pycache__/software_mgr.cpython-36.pyc,sha256=cDSEdsEHyVazFUlfgylSSRCrB6EofdiqjDhelzgNy6o,6264
-ascend_deployer/downloader/config/BCLinux_7.6_aarch64/pkg_info.json,sha256=d1JDFJjNGAUM2uL272SxgglT6FIpyIWPn7D1vfz1YrU,6926
-ascend_deployer/downloader/config/BCLinux_7.6_aarch64/source.repo,sha256=wW_5xH_BGBjpFIKslLjnzZ3ZVuxSJFoP5g-TJmmhGiE,378
-ascend_deployer/downloader/config/BCLinux_7.6_x86_64/pkg_info.json,sha256=vPl0fR-stbxoPHSHqGV5nP1ZNg8N-RDCrCvRm3aKKls,6287
-ascend_deployer/downloader/config/BCLinux_7.6_x86_64/source.repo,sha256=wDpxJX15DCUc6_47-ndXnNUD9a3cRO6H8VVVrBXCs90,391
-ascend_deployer/downloader/config/BCLinux_7.7_aarch64/pkg_info.json,sha256=d1JDFJjNGAUM2uL272SxgglT6FIpyIWPn7D1vfz1YrU,6926
-ascend_deployer/downloader/config/BCLinux_7.7_aarch64/source.repo,sha256=wbZFUrMduc6YS30H4ihAuZmqQEhYnmvw1l4kWG_3Fao,378
+ascend_deployer/downloader/version_match.json,sha256=PCIqV3xUOThg9-LS-Eb92j73MfTSSdmtp1G-llTSH3A,654
 ascend_deployer/downloader/config/CentOS_7.6_aarch64/pkg_info.json,sha256=CZ6-sQmpwyZb1F0uifYkgLzLM1EqhJuj_jyhn_W6dlI,8690
 ascend_deployer/downloader/config/CentOS_7.6_aarch64/source.repo,sha256=MXAKWne-AouqA4H0T3YO1gmRCsOKwY-TeG5MbBDqff8,234
-ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json,sha256=Ydx3iH0sabubCwikz40JICCZl46FlVidNBWkS_aEreY,8475
-ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo,sha256=UAkL5U0cWgp_wO5O2Kw-_FSbnLFm_PZ98AmTyfDEH_0,223
-ascend_deployer/downloader/config/CentOS_8.2_aarch64/pkg_info.json,sha256=qYcZxiOWA15cN7dcpO7-wGrLGSFePArAw95SQNbBM6A,12171
-ascend_deployer/downloader/config/CentOS_8.2_aarch64/source.repo,sha256=Dy54CPD2PRAlPCvWRbiXn2zChVCY2AtcBokgX5NTZCA,457
-ascend_deployer/downloader/config/CentOS_8.2_x86_64/pkg_info.json,sha256=fStE6P5NZkpSaR086DyBTkHrKMssf6iMMcIFqEJ_t5U,11193
-ascend_deployer/downloader/config/CentOS_8.2_x86_64/source.repo,sha256=m9crtfojVuFErSk3vT0T2lzZ5A9TMFXJvke0avMOVyw,452
-ascend_deployer/downloader/config/Debian_10.0_x86_64/pkg_info.json,sha256=7xFI2t7_rH9Q9O7YI8GVz2HvWGeBaCouSnjdbmDJHCo,12274
-ascend_deployer/downloader/config/Debian_10.0_x86_64/source.list,sha256=9rEl9HOOiKH0sHfAS3CC-yTb4AffG3VAbO5Cx_wZGtY,131
-ascend_deployer/downloader/config/Debian_9.9_aarch64/pkg_info.json,sha256=CGkU_cLJqipH1roVxegHye2O9zfjehoceIkFHjfw-cw,9007
-ascend_deployer/downloader/config/Debian_9.9_aarch64/source.list,sha256=ceDZ0jqV5hsMvo0_020DUI4L4Huz0Lllz47Fmj7TFAw,129
-ascend_deployer/downloader/config/Debian_9.9_x86_64/pkg_info.json,sha256=BbCbDyVEh7twICjhiBUtN3U1hkqFEPsnRipecuk4lEs,9447
-ascend_deployer/downloader/config/Debian_9.9_x86_64/source.list,sha256=ceDZ0jqV5hsMvo0_020DUI4L4Huz0Lllz47Fmj7TFAw,129
+ascend_deployer/downloader/config/CentOS_7.6_x86_64/pkg_info.json,sha256=X-S-xPgrlgGmVXpGBjdGWh0t1QLZRTkDMLql0PzWmf4,10223
+ascend_deployer/downloader/config/CentOS_7.6_x86_64/source.repo,sha256=oOiLtW45sOuZZ_P_pugv7LhrEgs3uw_xrRY5-FOjNtM,371
+ascend_deployer/downloader/config/EulerOS_2.10_aarch64/installed.txt,sha256=nKuC_VfjU73aukPARJMi1U9a9ZdUItqZCcvz0W_edaQ,43257
+ascend_deployer/downloader/config/EulerOS_2.10_aarch64/pkg_info.json,sha256=Z4Qyn3_SFLYrrhApOUnA98OimISEcl0J4Kx9_wSrvWo,4596
+ascend_deployer/downloader/config/EulerOS_2.10_aarch64/source.repo,sha256=eysNjtYexsTQGiWpLqXoN9BYfCgLxfQN8cjcb8GDQtg,131
+ascend_deployer/downloader/config/EulerOS_2.10_x86_64/installed.txt,sha256=s_R0_DEUFrxq40paa3aDFxOeqFAiyq1G0K-kLOwAEMg,42707
+ascend_deployer/downloader/config/EulerOS_2.10_x86_64/pkg_info.json,sha256=54rvT7MMq9gqOEeVsRo2eHfCoYLVN32JiVCRkC8rsPE,3668
+ascend_deployer/downloader/config/EulerOS_2.10_x86_64/source.repo,sha256=4C0abYxsv25uVugAAdc4mPhbMxiaO-4vN8TnNgwqBXY,65
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/installed.txt,sha256=RABC9Ydam7O91w4uymLiO04HCDgSG8RigE_2u1Sx6Iw,65900
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/pkg_info.json,sha256=43TNgHse2fYxbWu2Yjm_PIZrcsRCAaAOPpCWW27gWYg,6028
 ascend_deployer/downloader/config/EulerOS_2.8_aarch64/source.repo,sha256=-4n539gqg17t4JRpUyqctcJ0eQK5-1KZuHqDFLvtKqM,130
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/installed.txt,sha256=B1qfqvax5MY4ZBvzHa0z9cZNPgjymCcqOV9mDz-RdAE,42840
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/pkg_info.json,sha256=ijfqWmNevX6JwNp7hHijKIRpfuMYtUjaFtqFsYTaa8A,4518
 ascend_deployer/downloader/config/EulerOS_2.9_aarch64/source.repo,sha256=Cvl3U3MpU0IQc8gTvS6HdkDGIzRQzKsWChIMQhfTEyQ,130
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/installed.txt,sha256=JAcDXwKy_6MSFPVc_5ntA_JTlP3VpfWE0P6NHLlRECw,42208
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/pkg_info.json,sha256=zTTYc2gZ7uokYNaIumr5QU0ssitOXsDSXpf0_xpmRhQ,3827
 ascend_deployer/downloader/config/EulerOS_2.9_x86_64/source.repo,sha256=44o98hE2tl4xd0ScyHk89RYwk58p7Eq92qysQZ_PmgY,65
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/installed.txt,sha256=sItZv2m9qFp8vdh6xsopvEQICxIsyKCWkrGMudbBmNI,60396
 ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/pkg_info.json,sha256=NgUA1HE1qksNBx6wtHYOh3FV_TslCOl2ovzau6kmK1M,2490
-ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo,sha256=L-eyXb2mLsFCEpDvfu83POuhBchERJzSUIL86J84Ixg,187
+ascend_deployer/downloader/config/Kylin_V10Tercel_aarch64/source.repo,sha256=AHNc3TMBXQyjH24qmOfQJbqubB2WtVXCj1vpwgynMl4,182
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/installed.txt,sha256=_wVdEw615qxHMyxH06QJPIuvBLapIG9r46oK6XY0pck,60964
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/pkg_info.json,sha256=Ez3hz0-lj1Hfdy0LvVEtR_h915Kev5dn12bnjj9TYlU,2156
 ascend_deployer/downloader/config/Kylin_V10Tercel_x86_64/source.repo,sha256=ncCki_ycCYh6at3tw5o14JliFt6-9zKtuaXJpWwMYns,180
-ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/pkg_info.json,sha256=j6dz5c05sowZBglS774UQX4bdpTqT1PlOAi4srqKMSU,3831
-ascend_deployer/downloader/config/Kylin_v10juniper_aarch64/source.list,sha256=GdxwoPDqxZU74oYec3CYrBKblpRv-5D2nMTQJIULhIs,222
-ascend_deployer/downloader/config/Linx_6.0.100_aarch64/pkg_info.json,sha256=9Vjw2V8aox-ayQxDR_PJMsQ28eMHvMzSyJV2i-FgGOo,5526
-ascend_deployer/downloader/config/Linx_6.0.100_aarch64/source.list,sha256=pmaZyPJ5cQHJ6sMYvfU-O8xCPcOpo4cmX3dy26yLEzk,127
-ascend_deployer/downloader/config/Linx_6_aarch64/pkg_info.json,sha256=AOozkvcEdYpxqxBIocIAJKF4Yv6dEY6bWRscGu-9YgM,8000
-ascend_deployer/downloader/config/Linx_6_aarch64/source.list,sha256=ceDZ0jqV5hsMvo0_020DUI4L4Huz0Lllz47Fmj7TFAw,129
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/installed.txt,sha256=ItxvYYCtXV-E-9aVtk_YelIQ91MLQuA3byYuTrGz0Yg,51454
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/pkg_info.json,sha256=-KI3Hi0p4cpaqSHxkTwksBZRTcsXt6FtV8En9KAkUzo,2549
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_aarch64/source.repo,sha256=AHNc3TMBXQyjH24qmOfQJbqubB2WtVXCj1vpwgynMl4,182
 ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/installed.txt,sha256=59jrLcg4b3IR3wjBavS0g040YW__-uC4EdEoW99bl8g,51932
-ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json,sha256=94rzF_qmtNF-Sv6Qmgh0v9gXXb_k0gVIy45Rn12_15g,2209
-ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo,sha256=ncCki_ycCYh6at3tw5o14JliFt6-9zKtuaXJpWwMYns,180
+ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/pkg_info.json,sha256=M9StadsdGG5Bd2PdrSYPvj6ygGrtmFlUPkBhGLh8Qo0,3651
+ascend_deployer/downloader/config/OpenEuler_20.03LTS_x86_64/source.repo,sha256=F17X4kGY5WKb76bn6wbLK8qSbV7c4qTJa44aJMgZ7Ao,445
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/installed.txt,sha256=kNV9sbRHNGfDPh44gJRfKeT_1ixx1G5AVsk2lF-rziQ,51351
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json,sha256=W3LYuBm1sP-Qu5Fi2eDI9hAVHsKtUWxvdSeczmSO7TU,2424
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo,sha256=YIHupZYYJLwnCSV__v6DOglj5lA5eNLdf-Z6FfGmx8A,182
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/pkg_info.json,sha256=7w8QiW99KBuSANC613IVPImWsiNUAAySucQBdh_TbNA,5439
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_aarch64/source.repo,sha256=koyb7uyQaYLNckSFx2dipEQME7k29Qz9YJYRo-UslvU,458
 ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/installed.txt,sha256=dTh1kpyfwd7wD2-6YypziUtVmDMBiLSOMQPaAuo10K0,43010
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json,sha256=OPCQK3TMQpVa7zhah4H0gz9fd-jBEPeFbmgDM-7IIWs,2422
-ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo,sha256=MwcrWXHf8gSsvdEM8qOkZ44dJ9dRXeW14TqnDoL8Bq0,180
-ascend_deployer/downloader/config/Tlinux_2.4_aarch64/pkg_info.json,sha256=hyJSWXNFtAAiczYWhiByc0djohF_Uqa1U3E76WsFDBg,7930
-ascend_deployer/downloader/config/Tlinux_2.4_aarch64/source.repo,sha256=4D-nSWdZscS7kb3zfxvqy2RI7OiggHP_cPfjp7Rtm8Y,587
-ascend_deployer/downloader/config/Tlinux_2.4_x86_64/pkg_info.json,sha256=RwRJPUskaNnS9nrCqGciXsop8O7n98o08kEbOX69yI8,8101
-ascend_deployer/downloader/config/Tlinux_2.4_x86_64/source.repo,sha256=vsNFD5uLtL3VCjZUl6Ei6vra7LTP5qtWabA6rhNXdfk,473
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/pkg_info.json,sha256=zWvYiYFtRgB0w6TRznJ1bmPK13E-fsKP52-gyo3m0Ic,3220
+ascend_deployer/downloader/config/OpenEuler_22.03LTS_x86_64/source.repo,sha256=dckwsHk8V5ZZYeJBG5Y-_KE9lztKhBEn4Fi7rLAN6_g,445
 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/installed.txt,sha256=pvn_9ISn9UwCwLTuSanehgzyEamY80SGUC8jjtWdNCs,57488
 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/pkg_info.json,sha256=ekkYSxtur5m2PyKMyyEHpc1v_9JIvIzTWldbqAGxJYQ,2460
 ascend_deployer/downloader/config/UOS_20-1020e_aarch64/source.repo,sha256=FvnrmUSa31HWb0rHRYASmHQKmH8769lem8t0-XzBj00,186
-ascend_deployer/downloader/config/UOS_20-1021e_aarch64/installed.txt,sha256=pvn_9ISn9UwCwLTuSanehgzyEamY80SGUC8jjtWdNCs,57488
-ascend_deployer/downloader/config/UOS_20-1021e_aarch64/pkg_info.json,sha256=ekkYSxtur5m2PyKMyyEHpc1v_9JIvIzTWldbqAGxJYQ,2460
-ascend_deployer/downloader/config/UOS_20-1021e_aarch64/source.repo,sha256=FvnrmUSa31HWb0rHRYASmHQKmH8769lem8t0-XzBj00,186
-ascend_deployer/downloader/config/UOS_20SP1_aarch64/pkg_info.json,sha256=yeEoGwdNiGCfy1PTZTpfqyQVFduohgsquswWq8lJqsE,4884
-ascend_deployer/downloader/config/UOS_20SP1_aarch64/source.list,sha256=9rEl9HOOiKH0sHfAS3CC-yTb4AffG3VAbO5Cx_wZGtY,131
-ascend_deployer/downloader/config/UOS_20SP1_x86_64/pkg_info.json,sha256=qAFhacydacdlP_AnirU2Ff1Ecfx8ARcV2bN71bW0Xf4,4610
-ascend_deployer/downloader/config/UOS_20SP1_x86_64/source.list,sha256=9rEl9HOOiKH0sHfAS3CC-yTb4AffG3VAbO5Cx_wZGtY,131
-ascend_deployer/downloader/config/UOS_20_aarch64/pkg_info.json,sha256=yeEoGwdNiGCfy1PTZTpfqyQVFduohgsquswWq8lJqsE,4884
-ascend_deployer/downloader/config/UOS_20_aarch64/source.list,sha256=9rEl9HOOiKH0sHfAS3CC-yTb4AffG3VAbO5Cx_wZGtY,131
-ascend_deployer/downloader/config/UOS_20_x86_64/pkg_info.json,sha256=qAFhacydacdlP_AnirU2Ff1Ecfx8ARcV2bN71bW0Xf4,4610
-ascend_deployer/downloader/config/UOS_20_x86_64/source.list,sha256=9rEl9HOOiKH0sHfAS3CC-yTb4AffG3VAbO5Cx_wZGtY,131
 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/pkg_info.json,sha256=vDkUrniUl19gY8wBgB5Awdtq7-qrMZpXgSHNBGAOCHo,4177
 ascend_deployer/downloader/config/Ubuntu_18.04_aarch64/source.list,sha256=hDXHX8w0fwit1D2njIhhBTOjCzwehVkd5INGTmmwSFU,370
-ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json,sha256=T-fjjK3m0-4s6T2PYfmAUc36OIQTWpkK0HsjRTxX3Sg,5004
+ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/pkg_info.json,sha256=zmSn9E_WQ1ihMvQdBVLeTtIeAdu-wTZwlTY1TRvb9NM,5691
 ascend_deployer/downloader/config/Ubuntu_18.04_x86_64/source.list,sha256=-ZN1Y__CqGtpqogO3QHVnOVl04MBxQvu9CQn3wNJt_I,352
 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/pkg_info.json,sha256=wjz9fC3vxo9NaStiAH8NAX-N47i_MSYBDN7QSKkY8x8,5145
 ascend_deployer/downloader/config/Ubuntu_20.04_aarch64/source.list,sha256=8QbZP5aNc9uYxYVTe7WmeGYZljWPZ_Av6bvkgb4hwqE,366
-ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json,sha256=L5ngeeDbQaHVIPqIAFDizMpR0lKEswdLsqs4EGxJ82c,5563
+ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/pkg_info.json,sha256=havZNJ2-Vd_j6bNoh4SDSJO-EQB954fLUi33ggfrfOk,6229
 ascend_deployer/downloader/config/Ubuntu_20.04_x86_64/source.list,sha256=Fpa9xHLXJBSoHonzvop98ucN4yOE2q9FAuu06UKHFL4,348
 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/pkg_info.json,sha256=xT9VsnztrIO_zeqgGDR72jVFMVJQzUotTb9xiTCEqUo,5864
 ascend_deployer/downloader/config/Ubuntu_22.04_aarch64/source.list,sha256=dVuItkYL-4PTn0tTbcBbObkaXOYD7JlBOid9LHoAlWk,366
-ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json,sha256=R4gfVtF9FG0-oQJsFQPwjlt73rQZ4OO1tGGsTsWzHMw,5604
+ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/pkg_info.json,sha256=cCjqFOk2NKo51n3qxBEFwzS8imVJMXpx3SMW9vK-egs,6617
 ascend_deployer/downloader/config/Ubuntu_22.04_x86_64/source.list,sha256=CZWl_Rw_Qdy_qpekt40YqzeDtmS3GEjmsF-6HIntiGM,348
-ascend_deployer/downloader/software/CANN_5.0.4.json,sha256=eMJWko7x72ukyDlJb-eaLXGubzYGZVoDmcN7NS9PQtI,5041
-ascend_deployer/downloader/software/CANN_5.1.RC1.1.json,sha256=A2ki5uCXPPOvfjCGDH0dcr5rkXtg1dUQUpyJttwa5fg,3983
-ascend_deployer/downloader/software/CANN_5.1.RC2.json,sha256=JQChjdgq5IwgirLjxRbYgCXFwQ2NercufwSVG8zHSK4,5626
-ascend_deployer/downloader/software/CANN_6.0.1.json,sha256=NofokrfQGe8LxS3RbXhXNYiwGEl5hV78OC3xsXpnxjI,5201
-ascend_deployer/downloader/software/CANN_6.0.RC1.json,sha256=Q1WIskI2QAW2CV95Hjf58x2l4F-MqiTGSrysV3zolIE,5525
-ascend_deployer/downloader/software/MindSpore_1.10.0.json,sha256=POVFbqgEzwwc4KyqJYzVR4z_dPX8ElcdlNuAVHYu7ME,5340
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_aarch64/resource.json,sha256=QT9NZVDlzmJKwWbQe5dSl0i3NE3HzoPMgqoj08p80SY,3352
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/CentOS_7.6_x86_64/resource.json,sha256=xnIx7ZcZXo4PEdqRHCvmCSZVnnBPfY81VRPuD0-_bJM,3336
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_aarch64/resource.json,sha256=WT86C2afIjCBmNrBC940V_QXyuKIsT4cNSBF-ez2558,3344
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Kylin_V10Tercel_x86_64/resource.json,sha256=dr0pLHB091xgbYYcCszJgNsb3P-CKzqeXCcAKHeto6Y,3328
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_aarch64/resource.json,sha256=Fp1X_VaeRj8kOCWBXE_wqNiKKAop-z780hsitEP7RiQ,3424
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_20.03LTS_x86_64/resource.json,sha256=i9EFAZ6qV_oGPYsh195k5l67yHNgEwhWH7TFLoQzXFE,3408
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_aarch64/resource.json,sha256=JhvUWyx3IY5p2WydK5I1DG4M_TbprWaKoFMn0W0xOjY,3424
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/OpenEuler_22.03LTS_x86_64/resource.json,sha256=9pAsg27nguZG0W0hMYyogmGveCwe_xRXQ2JUq4XbaQc,3408
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_aarch64/resource.json,sha256=lEkmSYaWF320A2mXfPpALTLFGjny7COyTWL92dkGcxc,3368
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_18.04_x86_64/resource.json,sha256=DFJZh5SX-S0j718uN1rXaHs573wd-Cjwt_0qKidhiJw,3352
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_aarch64/resource.json,sha256=juUDO6PPNIISLiXsxoa78nOiC7lNYUSzZHVJb4BirrU,3368
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_20.04_x86_64/resource.json,sha256=lDeqmB5WxTGCV57cRxcWA0N1u6sHKfXYf11RBfu3I8Y,3352
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_aarch64/resource.json,sha256=hWpih-TCISMJQSggGzAuw5X27BOteYDdULXCWwnqmfk,3368
+ascend_deployer/downloader/dependency/5.0.RC1/COMMON/Ubuntu_22.04_x86_64/resource.json,sha256=liUJrJD-epN-hBOcUyOG3HkKYuUAlMDxDsQOM7bRY8A,3352
+ascend_deployer/downloader/dependency/5.0.RC1/DL/aarch64/resource.json,sha256=vQpZ0u_oqbj56IO_uC0XytzfCr2LVeQVq77uIQuN9Ww,2948
+ascend_deployer/downloader/dependency/5.0.RC1/DL/x86_64/resource.json,sha256=-Nr37Dd2jfRjDzH4QlEBcMlKKABf-0qROakQ9cIE0d0,2920
+ascend_deployer/downloader/dependency/5.0.RC1/MEF/aarch64/resource.json,sha256=jmGTn41DdL-5zRhI_gGYDTonLDbYDEd7v9z8xw_kAog,853
+ascend_deployer/downloader/dependency/5.0.RC1/MEF/x86_64/resource.json,sha256=y1k3e_IYmaKi-MZ-HWpzyCBLOL4O0-b5LBK1Os4or9Y,847
+ascend_deployer/downloader/software/CANN_6.0.1.json,sha256=vfr3eQxwSE4uAPRPQUzqftAyy3w9KuAJrykZ_2xNSFQ,5822
+ascend_deployer/downloader/software/CANN_6.0.RC1.json,sha256=2yy6KVNMvpfKDIfu96DRYfHrozHLjhD8NW4wAfAv8RQ,5438
+ascend_deployer/downloader/software/CANN_6.3.RC1.json,sha256=cRTw1JDZTMiL4BxK65v1Wz4IxBn9T2ODnUjc7HJU6Pw,5287
+ascend_deployer/downloader/software/DL_5.0.RC1.json,sha256=3KtJsNus91RJbf4PEpA16iP3F6v0a6wI3eumDpRgQyw,84
+ascend_deployer/downloader/software/MEF_5.0.RC1.json,sha256=FC8X1k_m6MeY-wJGsIJM4U29bRUMtITebbzukZeat5s,85
+ascend_deployer/downloader/software/MindSpore_1.10.0.json,sha256=uE3HrIzVgzpBxnDgOhxLAYDFZmQNVYwWXhiSpdr19FM,5341
 ascend_deployer/downloader/software/MindSpore_1.5.0.json,sha256=Vj2-kvDFUpyyJRNlAWrEnh8-VydcwzA3aMValMzACRg,3660
 ascend_deployer/downloader/software/MindSpore_1.6.2.json,sha256=rXKFRZK8JkE1_KNQOWCXDJ-xaSYEz5SPqiwT6HFZqbs,3660
 ascend_deployer/downloader/software/MindSpore_1.7.0.json,sha256=3nXDbFHkBxhi-lROYnCP21OyUZYQcn5Ngv2Ew4k2WXQ,5304
 ascend_deployer/downloader/software/MindSpore_1.8.0.json,sha256=TpYxbObIBDaJsDWt5j9KpzNmg2F-omIUt4MohbomY-k,5304
 ascend_deployer/downloader/software/MindSpore_1.9.0.json,sha256=17mw5-y5VHObof2pcBK7ouu6IZZGyWcJabQ1imC-Uyw,5304
+ascend_deployer/downloader/software/MindSpore_2.0.0rc1.json,sha256=faoPDysE0FeHs-9h49-O6C2hgShSVqv6itu0GmWNf9c,5360
 ascend_deployer/downloader/software/MindStudio_3.0.3.json,sha256=H6RPwO93VYomVZlHKoSURwpD79X8PPtASK-4LHjlBDQ,26018
 ascend_deployer/downloader/software/MindStudio_3.0.4.json,sha256=kYUWzhLaPdk45DZl7HySctnovza6qd788FDg-bJlM2g,26018
-ascend_deployer/downloader/software/MindStudio_5.0.0.json,sha256=aV7ZBjXXxMkuOJO3HLQMwQ9aGRWrZNqR4XsVX9XDm9w,48360
+ascend_deployer/downloader/software/MindStudio_5.0.0.json,sha256=Eo_mjiStaqYrAhlTBXzBzOV8pW7eILYwCZAWnZHQJck,48361
 ascend_deployer/downloader/software/MindStudio_5.0.RC1.json,sha256=5-WHXpPdEyZP-8oIcedPETMT88lxFpfbXV10eY_FQLc,25492
 ascend_deployer/downloader/software/MindStudio_5.0.RC2.json,sha256=g2r9TUy1PrKmNFPF23ppPRdoLyRNHvTr2R3E4TaMGL8,25492
 ascend_deployer/downloader/software/MindStudio_5.0.RC3.json,sha256=BgaX-Ndr24DOFZx8ZvtSw0ynu8XRXqDSLHj0MViAWT4,25492
+ascend_deployer/downloader/software/MindStudio_6.0.RC1.json,sha256=MK1ArxrjmC5XdWXv3i4bZ6tH4cMEYeCf5j0jQ6QDoYQ,48368
+ascend_deployer/downloader/software/Torch-npu_1.11.0.json,sha256=UQMLBvcgtnbnWv91-GRfZP0vJ82W3eifHNfAAMT1ePI,2890
+ascend_deployer/downloader/software/Torch-npu_1.11.0rc2.json,sha256=bb0bDdL4XRILfnFu4mpEg5asVXUGRls5uCNTwt98cHY,2906
+ascend_deployer/downloader/software/Torch-npu_1.8.1.json,sha256=BpRKP5Rfa5BEOG2n959ebvUWFQqVdLHDA8MxG8uqpLI,2895
+ascend_deployer/downloader/software/Torch-npu_1.8.1.post1.json,sha256=SK07iWwoeL7HiMy8uYsrNzW7tJmfOv-MtcaAz9MGUBo,2920
 ascend_deployer/downloader/yum_metadata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ascend_deployer/downloader/yum_metadata/create_yum_metadata_primary_db.sql,sha256=4TE3bYIpTQ0uFUhEHO94OBpU81WN3YygtrkUjd38DQw,1772
-ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py,sha256=Ko-goWu-OGrn_YslHm5AFm0cOHVN_48Ul5sqSAdUCJY,11322
-ascend_deployer/downloader/yum_metadata/__pycache__/__init__.cpython-36.pyc,sha256=04wNyh2ndPYcfYY48otWtXoDH1a3IQbQVhktthgdEj0,140
-ascend_deployer/downloader/yum_metadata/__pycache__/gen_yum_metadata.cpython-36.pyc,sha256=y-JWb2E39xz88L1CdUa-I1jyyBulKx1ILCxajDD9Jsg,9172
+ascend_deployer/downloader/yum_metadata/gen_yum_metadata.py,sha256=cypQrOYhYRvhOAXGBbcYcHyVTaJC1d6GB6dylMnvnvw,11330
+ascend_deployer/group_vars/all.yaml,sha256=9oewGhNLFy1Rjr9V6Oqd7b45zBiezyD_ub1HWqp91Zc,1572
+ascend_deployer/patch/selenium_firefox.patch,sha256=MD5-UZ717Hca32fdmKa21g_JnbxKRM4BlVx-U-EPALA,807
+ascend_deployer/patch/selenium_firefox_profile.patch,sha256=K89iaIG9x0RX9qO0_LXISXSGDsG9QdzgvflrQWsrqYk,1127
+ascend_deployer/playbooks/basic.yaml,sha256=Ou1DidGhODBKq82i31KLe1HpOjMqo320AJndcSL3yMQ,236
+ascend_deployer/playbooks/check.yaml,sha256=FGf3L5QqmSTxpS7C_Ofe0S13_0NroU10CAjlXXkB5dg,479
+ascend_deployer/playbooks/check_pkgs.yml,sha256=vFej41gd3l3fq8khqR6jtsLPw0NU9JM1POQpbx4qmzE,94
 ascend_deployer/playbooks/create_user.yml,sha256=If1dyZgM2xEn34Mq2aVBg2W3uJWDefgJLnylkKyMkXg,1136
 ascend_deployer/playbooks/distribution.yml,sha256=E_uC40STeGsDNWhchHE8PQmReyf99oGrHUyJJmqC_Fo,835
-ascend_deployer/playbooks/gather_app_info.yml,sha256=i_VQWIYIXXXlQAnUKX5iFQG1YVoZ4oXFVze6x1TCWjQ,1061
-ascend_deployer/playbooks/gather_npu_fact.yml,sha256=UHphnVHqAS1nbO41JVa3SSnhkbRGtc1OLOQLEvvdasw,938
+ascend_deployer/playbooks/docker.yaml,sha256=OjJ3rcnQRZ_aRsE-Pg1ygAcRFJzs1Vi7PMErFjxpoi8,672
+ascend_deployer/playbooks/gather_app_info.yml,sha256=Bmhjybkgks8NKxwwyTJtGHXeJqbOW66hn9uByAt2xJE,1021
+ascend_deployer/playbooks/gather_facts.yaml,sha256=UtX8qT8HT0RIThtEFEPmMHUu8dVUYZTvfI-4pACA2O0,3487
+ascend_deployer/playbooks/gather_npu_fact.yml,sha256=fSOcEcUx0XeXaN3vDNWAiDk50zrRCQznb13ZR_pTwc4,1162
+ascend_deployer/playbooks/harbor.yaml,sha256=_MLo4qg26_e9Nu1lVxK8zduhieyd1gY9oq7AfmJAuuY,121
+ascend_deployer/playbooks/hccn.yaml,sha256=hX6LLQxYvaB4NHN-GKbHzmFlyF1SsdUhi7LPnAJRkNQ,122
+ascend_deployer/playbooks/image_load.yaml,sha256=LnuzoVRFz2Tx9Iyl8tKFx_SihI-TtOqZjcyHOnCx9ig,134
+ascend_deployer/playbooks/k8s.yaml,sha256=Mwg6Z5QolEsJTfgdF_dVVFpo00jmZD0zxw7kuUsF6c4,2213
+ascend_deployer/playbooks/kubeedge.yaml,sha256=bcF_WC6RqCBTA38P-hNWeCvBP38yIS-MdB333e08Lok,85
+ascend_deployer/playbooks/mindxdl.yaml,sha256=w4KV2_Xy3408FilwEsjOnP-ECES6P8nT0SDm5rkISpk,1654
 ascend_deployer/playbooks/modify_user_group.yml,sha256=nFrPwxyL9wzrslWPcjz-w2mOZmqMrui4_-sPJmWpx3U,491
-ascend_deployer/playbooks/os_map.yml,sha256=skX5EA8cQ_D9WC-jTpVR6AfVO5F85v6f80A2okoY7JA,1311
+ascend_deployer/playbooks/os_map.yaml,sha256=gvdLP3qgFyHOkB3afyUR4PhAhz4TMH-Ad9_AVG27oN8,225
+ascend_deployer/playbooks/os_map.yml,sha256=oZM6qaOYNbhJw3VvQ2o1V-lAQr5QJuKtPXUsftCQI3I,2065
 ascend_deployer/playbooks/prepare_CentOS_7.6_aarch64.yml,sha256=Az8oJzhsZLYh14r67nhykgb9tXONmDXfiHefyzUJ5tU,1073
 ascend_deployer/playbooks/prepare_CentOS_7.6_x86_64.yml,sha256=Az8oJzhsZLYh14r67nhykgb9tXONmDXfiHefyzUJ5tU,1073
 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_aarch64.yml,sha256=s1A2FkFxrY3IVsJHHmplmCGlU7Cum9q4j5-lXKg72pc,1076
 ascend_deployer/playbooks/prepare_OpenEuler_22.03LTS_x86_64.yml,sha256=s1A2FkFxrY3IVsJHHmplmCGlU7Cum9q4j5-lXKg72pc,1076
+ascend_deployer/playbooks/report.yaml,sha256=dUjp7DIOhyOGavCdvP9W-da1sRDWbDjZ4lVJBXuxtMc,422
 ascend_deployer/playbooks/set_facts_cache_permission.yml,sha256=vMTb7wIDN5utqsrGd8myI2l8U-hQVloe-AJZIrJTAC8,139
-ascend_deployer/playbooks/task_set_custom_fact.yml,sha256=b8hdEPOsjC_lQbLGwHyQb6ojUYUBjEOu1pRyZsE_U-4,4459
-ascend_deployer/playbooks/facts/app_info.fact.j2,sha256=pokWKSg9xJFYi2CBasFkt-ASm42mzUf4UwAwQ2Df9W0,6621
-ascend_deployer/playbooks/facts/npu_info.fact.j2,sha256=UVE_wxcqcYrZrsocqWjr_3iPbs0c7EUOCA7ibLnNGB0,10259
+ascend_deployer/playbooks/sync_time.yml,sha256=yXuZoZ1EkInR6C-lNSzLZik7W4xNj92yfLTpoy3LynQ,381
+ascend_deployer/playbooks/task_set_custom_fact.yml,sha256=gVsxg5vZVqOufhDDS77PLegbIG7mK-5Iyha-op9Fhqs,6051
+ascend_deployer/playbooks/uninstall_mef_kubeedge.yaml,sha256=n3PyVh4k72KzXuJEbBvtWGRcSGV_iDloiDp5TpJHFBI,155
+ascend_deployer/playbooks/uninstall_mef_releate.yaml,sha256=TZraFst-Ykc0wHKAoswYe3tW2a_yUGIS4CjFt631UHc,246
+ascend_deployer/playbooks/facts/app_info.fact.j2,sha256=KdVRCDzhLtGMqpKo1USq4YXrS3rxi-aSoKeV02YZT1A,5199
+ascend_deployer/playbooks/facts/npu_info.fact.j2,sha256=7lGRDlLvVRSI6-2NS245Qb3Mw6KiSbAUXz3CrGWjAME,6149
 ascend_deployer/playbooks/install/install_atlasedge.yml,sha256=uOHSZp6aaRISBCnY1Mk1V5PUSMf0y6dekRFfSsPCms0,409
 ascend_deployer/playbooks/install/install_docker_images.yml,sha256=-Rro75RJhvTbvNW9TC9b2EGhkAlS5FifcuBAUGUj-2A,323
 ascend_deployer/playbooks/install/install_driver.yml,sha256=3UJJwBjVy1C2nIs5xFAMwzufhhQf0OFm0icK5TohbxA,1128
 ascend_deployer/playbooks/install/install_firmware.yml,sha256=QHPajyYbBjjmKzJeq3sRt487smN8hHu2o5ZqvRddkAo,1151
 ascend_deployer/playbooks/install/install_gcc.yml,sha256=l8xK00FYxDXlbfxBcg_UJpu_LM7A3SxbMxZSbX81sSc,888
 ascend_deployer/playbooks/install/install_ha.yml,sha256=upUDdabvJQiB27vyAWlLZoY4o9ePdaArCmw61ar46Sk,388
 ascend_deployer/playbooks/install/install_ief.yml,sha256=ZSAjTn_aasQ_tB39RzIU9F3IQGSg1voPhsPc8ei0UtU,293
 ascend_deployer/playbooks/install/install_kernels.yml,sha256=GLwjT3L0VAKJtcdOC_zcbs8Zb95-a-jZEnRRDGDGoAg,216
 ascend_deployer/playbooks/install/install_mindspore.yml,sha256=-UyBs_sScqFKNltEr_jYbwFJfGsqSqRblfuPZM2jzDY,1223
 ascend_deployer/playbooks/install/install_mindstudio.yml,sha256=QwjoTpiD8Ymw5i-7HZHgOpHl7G_mLT-Vo48wlULy-Sw,9015
 ascend_deployer/playbooks/install/install_nnae.yml,sha256=Uxp-GvbbdcBe7c7vHRnuS10u804G0z2WA867bfMSYwk,96
 ascend_deployer/playbooks/install/install_nnrt.yml,sha256=pZ9uamO_fg25jmOOmH7ka9eRCztniDpWgoy4sNuEEJc,210
 ascend_deployer/playbooks/install/install_npu.yml,sha256=WP7-_H0GRGoM2ei9Lb05exf_LWIBiEZ65533Ia5PTIc,1398
-ascend_deployer/playbooks/install/install_python375.yml,sha256=6QZGYM2licrdTqxyNKFzZcBgHhAnd-a48KM7-oXKJ94,108
+ascend_deployer/playbooks/install/install_python.yml,sha256=62I2D8DdE178Mum9k32gTFCNPXsMeGB5bA0RbSIe5iM,105
 ascend_deployer/playbooks/install/install_pytorch.yml,sha256=KP6GeRd5xuY77TdKUkJiiNkgSA9A5pxS26sEaKntZDA,2499
 ascend_deployer/playbooks/install/install_sys_pkg.yml,sha256=HrXn7aSL939RwoK_1fxmVuztr5xCYzGUP1r09dRGxvQ,313
 ascend_deployer/playbooks/install/install_tensorflow.yml,sha256=86pspWkfl9LQwE96px2lmCPqYMmsjg8XsELc4qNMmC4,3007
 ascend_deployer/playbooks/install/install_tfplugin.yml,sha256=gVqt5EkpXApkLxeG8KBx87oGraCpkF3hfgoJenXSsAM,104
 ascend_deployer/playbooks/install/install_toolbox.yml,sha256=V5aXG6MHAyNbh1N6HQF1h5E69yBEwz8MsZMT7LBuwxU,102
 ascend_deployer/playbooks/install/install_toolkit.yml,sha256=dkg6uB8hWXjG5SGXxNbRzDHlLLOw_YauhGMi1DE3Erc,216
 ascend_deployer/playbooks/install/task_atlasedge.yml,sha256=T6QGv590ME2i3zlETEY5Y0nTdgBzARlzVPMRLa72s4I,1263
 ascend_deployer/playbooks/install/task_cmake.yml,sha256=ue2t4_13xOEt9nRbEt6iCRHemHDH8_FaNz4doUAfhq0,663
+ascend_deployer/playbooks/install/task_dl.yml,sha256=1V9pLmChX5L6SMRHai2i60oa_qpARk16gpfNI5y8QOM,769
 ascend_deployer/playbooks/install/task_docker_images.yml,sha256=piJlx21vBg1hLsmwM6-FE3QBCMQWXC86HknnPR-Mcc0,810
 ascend_deployer/playbooks/install/task_driver.yml,sha256=sb3MuzsVmFLqIRDc-Dzu96QZKojtT_ojz_QPSl3gBMY,239
-ascend_deployer/playbooks/install/task_driver_bcinux.yml,sha256=PQfkW7iS31rs3YoEOMj5Y-T3fUXndllwT5iDHs85Le0,5640
-ascend_deployer/playbooks/install/task_driver_common.yml,sha256=W86ay_SHc0m57cskSUL0cw8BsCuiGaOmH7QfbQ1RJWs,5723
-ascend_deployer/playbooks/install/task_firmware.yml,sha256=YF1ekZ0kBt7i8QCtNfAfXvK_2vfDMJ9RN-pftRtf5LY,4840
+ascend_deployer/playbooks/install/task_driver_bcinux.yml,sha256=f-bbx-pWZ1gDGgHKJB2LQY3fgSvbVP0hplI_G_lO434,6047
+ascend_deployer/playbooks/install/task_driver_common.yml,sha256=83CEvbo12riFnYE_VDBoQ-RfqAkvJuSoEI1Q8KMevIU,6130
+ascend_deployer/playbooks/install/task_firmware.yml,sha256=xD4Fq3UOsoJLRigDfuupj4fezEf3jp8YKG62uCD5ZaQ,5295
 ascend_deployer/playbooks/install/task_gcc.yml,sha256=nPcCmo6N30E00uV9-8vpokgLA06uetpbc81Whfl_yas,2210
 ascend_deployer/playbooks/install/task_get_npu_scene.yml,sha256=aa6P4mAcn9ExFxEwCOyg8leM7dssZbQC3FWMo-c_OdQ,3055
 ascend_deployer/playbooks/install/task_ha.yml,sha256=3vnX3IVHKrZO63OMbp1QezCdVjmiGrPMbjKwANtwtvE,1056
 ascend_deployer/playbooks/install/task_ief.yml,sha256=oA-mTO09S9G_4eHeE5fm0RNTiI7mZwHW4qvHRKQ3dQM,662
 ascend_deployer/playbooks/install/task_ief_a500.yml,sha256=E9QiD3RagW3bgG_UdN-EC6vOfNotwyNnMOB4LP0KAVw,2777
 ascend_deployer/playbooks/install/task_ief_a500pro.yml,sha256=SKbPruc7lmt7P6KpAO4wC-MC-0i0QEjtWxi8hMxdg6U,1665
 ascend_deployer/playbooks/install/task_kernel.yml,sha256=a7i2WhK6d-zCO9R5E8WI1frktRMcZBoxl0KATzXxv3s,1395
 ascend_deployer/playbooks/install/task_kernel_euleros.yml,sha256=AAtwILRPMJhFjfSbiDDZRk_ELfqgVBcJSsUMJQp4gLw,1317
-ascend_deployer/playbooks/install/task_kernels.yml,sha256=cADQdb4GL8eKZdS1SUGltuQbeicfrWiI1IkNaExkESg,3933
-ascend_deployer/playbooks/install/task_mindspore.yml,sha256=2GsLeLfxr1JdJL5KcVCuZT3PK01JMiJMslfHg447nfU,2805
+ascend_deployer/playbooks/install/task_kernels.yml,sha256=C9U0rzjESel-8SMK3Pb60gIsD2o_wKVFIbCfJZLCki4,6030
+ascend_deployer/playbooks/install/task_mindspore.yml,sha256=RPQhI0ZfQCKBBNgIC73zQeNWh3D0vWIF6XD9jo40wvE,1879
 ascend_deployer/playbooks/install/task_nnae.yml,sha256=n8Pwlke5fnbrVag2-7bx4PlbYnDuExRZKQEEWXI5f2g,3270
 ascend_deployer/playbooks/install/task_nnrt.yml,sha256=9oyJsE8kvOCtLpHzkeJ_pqucGw8quWO2cHxpKJCmx0Y,2992
 ascend_deployer/playbooks/install/task_protobuf.yml,sha256=wisHWXln-3KJNKNAEujdEyG4R34xd8tPie9C1JpoEPU,709
-ascend_deployer/playbooks/install/task_python375.yml,sha256=8757_kb8MqLYikXQGtuTVYt6dtQGqidk9hutOUIJkUk,3209
+ascend_deployer/playbooks/install/task_python.yml,sha256=8757_kb8MqLYikXQGtuTVYt6dtQGqidk9hutOUIJkUk,3209
 ascend_deployer/playbooks/install/task_pytorch.yml,sha256=M9g3OQLMDUpQrwNvyK7nk_XiybgB15SNn0sOVevj7ec,1265
-ascend_deployer/playbooks/install/task_sys_apt.yml,sha256=Vp7fGE7oY4t6HETI8tCHaSkAJ0uRAeTCmx_gqhxM64Y,785
-ascend_deployer/playbooks/install/task_sys_dnf.yml,sha256=7KbC3BJvA-rGYs_VnFMdwxwywrcyQd4zhNw6OTa36JQ,496
-ascend_deployer/playbooks/install/task_sys_pkg.yml,sha256=w73xjhPIunG7qFGFPUaAxSyvU91i87zMDpSntnFxZvA,1226
-ascend_deployer/playbooks/install/task_sys_yum.yml,sha256=qI60hTNQQYrFRBiW4IW753Gevkc1QaSEfY6gJeRP9rg,456
-ascend_deployer/playbooks/install/task_tensorflow.yml,sha256=y6qVB-JlHGy8xCWcLz2dZZmgeIsetHyzI5eB5_6qVsU,1556
+ascend_deployer/playbooks/install/task_sys_apt.yml,sha256=jd8c4CB4_bdP-dAB05Ry51SDiiVj5d1urSiJ8nR7qxI,1810
+ascend_deployer/playbooks/install/task_sys_dnf.yml,sha256=tTL5PGBno66rb6g3-Ys_4xfay-jKrilBhI7R7jO7aqE,1794
+ascend_deployer/playbooks/install/task_sys_pkg.yml,sha256=yQt__pF0q_6OtiSQanMU71U1prFmg2Jql96yJv9ACi8,3230
+ascend_deployer/playbooks/install/task_sys_yum.yml,sha256=SSysrdzpIz-CDeYhxhzVE36pFvfuA8O4JSZfeyq516I,1798
+ascend_deployer/playbooks/install/task_tensorflow.yml,sha256=-JHHIg7YlvxPHe7zzDn3pXY2hbRH9in_21SmuWOHuIA,1073
 ascend_deployer/playbooks/install/task_tfplugin.yml,sha256=x3tsYPVIPa_S_Acs0wdpuWO2Qn4DXBkeGxPnf0FMswo,3449
 ascend_deployer/playbooks/install/task_toolbox.yml,sha256=hlkw38EYGdwUXiRLgCts-bx_y8VsWduL5bJ2URW6IL8,3298
 ascend_deployer/playbooks/install/task_toolkit.yml,sha256=L71y-dtO4hh_ty71zF4FFJ4UAGyJ3agHCFqGVa_LK88,6307
 ascend_deployer/playbooks/install/patch/install_nnae.yml,sha256=Bjt_L7j-afhIo4wNzHYz-x8tGdk4JJZDzEjI_bTEgU0,102
 ascend_deployer/playbooks/install/patch/install_nnrt.yml,sha256=xBqvjCC-rxEtPppD9YyvIV85EGCNzrzqluVH6lb3kc8,219
 ascend_deployer/playbooks/install/patch/install_tfplugin.yml,sha256=aly9mNlv0lFBjLNpyS_IhiFJiRs3l4Ob3ImtAJcsavI,110
 ascend_deployer/playbooks/install/patch/install_toolkit.yml,sha256=K4ZbG5y58eheZm6u7G6di8vbmZUs2pLVOIWfUtYXwTs,225
@@ -214,23 +223,115 @@
 ascend_deployer/playbooks/install/patch/task_nnrt.yml,sha256=alvNx9XjHJz6WBrrbGqlTyEyDb11O24koTgtu_puibY,1255
 ascend_deployer/playbooks/install/patch/task_rollback_nnae.yml,sha256=Bqd1aUEEqE1wQNcmemUZNVeAOr7p3dA4nhwbl0aGwEE,555
 ascend_deployer/playbooks/install/patch/task_rollback_nnrt.yml,sha256=XnMRpCJg0iyH15SMsNDaMdeC1mMLJ84HGQtLwWedqkk,1468
 ascend_deployer/playbooks/install/patch/task_rollback_tfplugin.yml,sha256=Ir8kfgyc4PxsAewcUHMamH1Czotvs5zSKHWqCvfcKk0,606
 ascend_deployer/playbooks/install/patch/task_rollback_toolkit.yml,sha256=imnloMyS_GluTxsdb0fQ1rzg6cxJ4KpT7mbn0790Q9M,1563
 ascend_deployer/playbooks/install/patch/task_tfplugin.yml,sha256=Sct5UR3OwITKJN3swCA_ms9KPkoa_z3-1vhr-1eSmJs,1310
 ascend_deployer/playbooks/install/patch/task_toolkit.yml,sha256=VxZcl_ylAkfb08Tq6uSyNWY8t05WzsAXd0jr6kHvsqs,1303
-ascend_deployer/playbooks/scene/scene_auto.yml,sha256=0zhrALIsSXB8YXpEx3v9CkybXH9KIWEbmxEOnLQkvTM,963
+ascend_deployer/playbooks/process/process_check.yml,sha256=iDv0yzMTVaBYtMEZpditZr5Pf2xECbxhTMl7TXgPijg,369
+ascend_deployer/playbooks/process/process_install.yml,sha256=qz9-wdWlZ6nLZYT_gK51pE6oZ-wTCh2-BNGRRH-DRLM,2169
+ascend_deployer/playbooks/process/process_patch.yml,sha256=qAGVHYDjc6GGIyU606RQLwYyuBRpv61rJp1K2w146cE,711
+ascend_deployer/playbooks/process/process_patch_rollback.yml,sha256=i47p_OzeHZ2LxoijRqWgyO8a74KJpkdRvU7TchwP0Ic,715
+ascend_deployer/playbooks/process/process_scene.yml,sha256=EeBtpYPW6bc7EM2YcxDz3c3YA2-a7gOobxCd9yKCrUM,1588
+ascend_deployer/playbooks/process/process_test.yml,sha256=Kt8kHZE0PMglOBa1infYEs6EfMn395BqGo16HLEt8sg,967
+ascend_deployer/playbooks/roles/mindx.basic/defaults/main.yml,sha256=O8bMeN1kpRuHIr9qqpKnI3JhULaafjTpnVeVYVnB-WU,310
+ascend_deployer/playbooks/roles/mindx.basic/files/space.sh,sha256=sweRsZwzkCcoCWy5iWd2msj4oJdop3OraLOde-vytG0,1258
+ascend_deployer/playbooks/roles/mindx.basic/tasks/check.yml,sha256=dFYzXHI-iA7IJAdTMsbVYRyR1Ko_X2LfxW_W11fUCv8,4146
+ascend_deployer/playbooks/roles/mindx.basic/tasks/install.yml,sha256=pAdpt8prs3dVHLr6aoC0S5rkBbRe1tSAYykOMnG2ffg,1437
+ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_check.yml,sha256=CrIDq0u_nmU6svsDzS3KO3BRkB-F1aBH36ovIEEAoO0,4504
+ascend_deployer/playbooks/roles/mindx.basic/tasks/k8s_status_check.yml,sha256=NYYrJKbJwsDC_mqbDhOKZrbQxYj73gwpYnDVPfxfDXo,4892
+ascend_deployer/playbooks/roles/mindx.check/defaults/compatibility_map.yml,sha256=wu5Cc2y1_aokTKONPg2HCdY1baGIWK46gemDD_AbJf0,10079
+ascend_deployer/playbooks/roles/mindx.check/tasks/compatibility_check.yml,sha256=ICdzO3xr4zkRYj9GJdTvJk0ikrGnqDWUZvtxMDWIhlg,341
+ascend_deployer/playbooks/roles/mindx.dl/README.md,sha256=zVYAP3TfVYfVeqkuiCUs0hnhSID2Vx7xLc4ObZvIMnw,76
+ascend_deployer/playbooks/roles/mindx.dl/defaults/main.yml,sha256=LSbRMwZkChnKnzh7bxJ-E_eGRtHUU8XM3M2M99lC4No,1296
+ascend_deployer/playbooks/roles/mindx.dl/meta/main.yml,sha256=e4vPgX79HlfSjygJhGVEQT_g3qIMPWhV5P2j3D3t1rM,181
+ascend_deployer/playbooks/roles/mindx.dl/tasks/build_collect_images.yaml,sha256=f0e5evfp5JxOgI6iKcWvpQ3uytNtmmsVSf4Vwq18coY,9911
+ascend_deployer/playbooks/roles/mindx.dl/tasks/create_user.yaml,sha256=PfNpGclq1umyPnX0mc_nvi9tj6DZpVEEJBx6pbz-Nrk,675
+ascend_deployer/playbooks/roles/mindx.dl/tasks/deviceplugin.yaml,sha256=EFvx0Cn5RwudCA8I8ltJOTcfobAIZnBb_Ay6YXQuVps,12803
+ascend_deployer/playbooks/roles/mindx.dl/tasks/distribute_soft_package.yaml,sha256=3f24D9cAFb5upAlEplCQOm2iD3aHPPSg4M8K2yJVBtU,7226
+ascend_deployer/playbooks/roles/mindx.dl/tasks/dl_common.yaml,sha256=mJXlbSjdRrGmWgEujrZVLNd6d0qL2YvvAoPSHGtN1Gc,646
+ascend_deployer/playbooks/roles/mindx.dl/tasks/docker-runtime.yaml,sha256=yJe-9f0baw4tqCoGRrSsHS0Sa8ZgCR0XiAUQ1pd2OPI,1517
+ascend_deployer/playbooks/roles/mindx.dl/tasks/hccl.yaml,sha256=mGlDiozcWbq5cU1LmHoiJ-Z6VtusQOZy9YcC7ga-jPo,5651
+ascend_deployer/playbooks/roles/mindx.dl/tasks/noded.yaml,sha256=UUWA4pcS-0I8cJ7Ungk2u6C6bhQGIgx7K3Q4OiM0OA0,5906
+ascend_deployer/playbooks/roles/mindx.dl/tasks/npu-exporter.yaml,sha256=m2OQyWyJzCOuvlefiIdPZaMlUL9o-pmmLN3W1XhajGg,5550
+ascend_deployer/playbooks/roles/mindx.dl/tasks/push_image.yaml,sha256=VPAw9sLncOpAfvOPCOxgOg4JYa3iQEvEoqXJh7i5a-U,4386
+ascend_deployer/playbooks/roles/mindx.dl/tasks/volcano.yaml,sha256=C_O5q6Wmw2Y1_kfj-bWLlMyDdI2WYZaAU0Vjz3zDkc8,7418
+ascend_deployer/playbooks/roles/mindx.docker/README.md,sha256=_rk-uEyhUIyM1X9hFmBoR0cVNsCPjaFutgnLGY7Jnk8,67
+ascend_deployer/playbooks/roles/mindx.docker/meta/main.yml,sha256=HIK4udfQ5FIDSBZCHGmRI2fXksD_gpJZaYmTy6_s6ZQ,171
+ascend_deployer/playbooks/roles/mindx.docker/tasks/copy.yml,sha256=zhYaNVRkPWLkGUjlFAlOfuNVzp13LA5gKr3l08BaX14,500
+ascend_deployer/playbooks/roles/mindx.docker/tasks/install.yml,sha256=j8wMPI5_9498O-jVrvSbpONp96Jr-ODqYVdtF8Qya0A,418
+ascend_deployer/playbooks/roles/mindx.docker/tasks/main.yml,sha256=1S_zHployo8HJe7xz56YriqqBeT91kr_g97YW_znX7Y,892
+ascend_deployer/playbooks/roles/mindx.docker/tasks/post_install.yml,sha256=bXsWWUxC9WmfBUZCmT6eMS8daSSVkjCEl-5lpUAuZ5w,1160
+ascend_deployer/playbooks/roles/mindx.docker/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
+ascend_deployer/playbooks/roles/mindx.docker/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
+ascend_deployer/playbooks/roles/mindx.docker/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
+ascend_deployer/playbooks/roles/mindx.docker/vars/main.yml,sha256=1poZSfGzwYW8O_Lr-LRkYySUOPP4mr2zv_y3tnD7NDc,99
+ascend_deployer/playbooks/roles/mindx.harbor/tasks/check.yml,sha256=O-OHocr3VY8qFwybYKvzCrj5c5kRZyUujncLhBxllBg,1314
+ascend_deployer/playbooks/roles/mindx.harbor/tasks/http.yml,sha256=wDiwJIfN95dQ0PXvQv_UDxw6Kzr6bZghpxwZAhnUKqg,1158
+ascend_deployer/playbooks/roles/mindx.harbor/tasks/https.yml,sha256=t5N9tSuXR8MEo45hOr-6v-iTobl68LxBDXmxDHtqJwE,346
+ascend_deployer/playbooks/roles/mindx.harbor/tasks/main.yml,sha256=wZjzaWCiHwiLgr2jiXPTe0i6DHz9XuuHKIpYNpooC-s,1157
+ascend_deployer/playbooks/roles/mindx.harbor/vars/main.yml,sha256=hb6M4EeVx8416XPO-nIwpyHRW7V2iZsnMeVrLig_JgA,42
+ascend_deployer/playbooks/roles/mindx.hccn/tasks/hccn_conf.yaml,sha256=ayfhJmAYjAYoOcnVisVrC2n4jdmZ9OWiDy2dI7LQCbY,1707
+ascend_deployer/playbooks/roles/mindx.image/tasks/image_load.yaml,sha256=ye4H9F9Xy58tUZSebL02i_FGYSf9Dnhn9QJ5oSpwGPg,644
+ascend_deployer/playbooks/roles/mindx.k8s/README.md,sha256=yEssYhqELC5UiHFN7ooAN3vB48OZIc4EHaMucUfvQSE,536
+ascend_deployer/playbooks/roles/mindx.k8s/defaults/main.yml,sha256=2JbJVXoWYha-hy0_w9eKfQpSkLgNp4Ua1yy2PgMogjI,234
+ascend_deployer/playbooks/roles/mindx.k8s/files/10-kubeadm.conf,sha256=ICh5R0gs5GbvEdItYXv4XzgVOOsPKjdNjqQmBxzYyTI,929
+ascend_deployer/playbooks/roles/mindx.k8s/files/kubelet.service,sha256=SMj1pqE9QXn-FW9IExZ6WQF3z92nPBuWgf7H49FZtwk,283
+ascend_deployer/playbooks/roles/mindx.k8s/meta/main.yml,sha256=BRFTshnlZZPPYEvfccG4xZD4bvRLfA5JoWfEl2UZcIE,179
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/containerd.yml,sha256=1PCjhnosJZnTMAQwbRckw9pujMCWyNfGzgt4DXnDtRs,691
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_image.yml,sha256=EM7gV6rA9uIeFMDHB6L7cS812ZdZ9tkjEqCHpgas5vY,1169
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/copy_software.yml,sha256=XXyrSjfxprN61doTRZL-P0qbslM7TmTRMFztXormV9k,417
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/get_k8s_version.yml,sha256=_GCaJ2BvRoidQ4CtLI7zRCZpEkM0H7mt5Md432hW2t4,390
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/install.yml,sha256=rU7jbJ-ESswn9jI-MkM2PxgLlDQQjJvj6jDeEmnDEd4,869
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/main.yml,sha256=OPyz4OaqYC4XrebW_YkWHk6hy90rVD6go3Mn0sLqD70,1401
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/os_setting.yml,sha256=NCw5rn4vEzk1fnbpsk_wrqLeb8fbxOcvtegD3pzgI_o,897
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/install/push_image.yml,sha256=f-aeDQP4T6vXKMDygoqxNytyo3SxuoQgjGd8Ch3CsXo,4442
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/kubevip/main.yml,sha256=UgjXafZInXw1lwRJ7zpiObGgafHIxNwpAUI66_N-_XI,1797
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/master/main.yml,sha256=heQDTtxJsI1MUkBGwsivITSFwiV9DVuqVvOSPocsHPA,3518
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/master_backup/main.yml,sha256=bp02sszuA7KbwzaUgRq9flfWwC8_yaNYDapjTMXRkhs,1596
+ascend_deployer/playbooks/roles/mindx.k8s/tasks/worker/main.yml,sha256=9c5hE8eJWjhGSqT60_Z-2ikOaobRI0C5_AQ926Xyipw,860
+ascend_deployer/playbooks/roles/mindx.k8s/templates/calico_v3.20.2.yaml,sha256=0IuV_4dsttpiTK0gmRZrINL22Gj6-pW1nW553aT1naw,202740
+ascend_deployer/playbooks/roles/mindx.k8s/tests/ansible.cfg,sha256=o8K2az-hZ6dLhzVrfJdrpqKfXUpBBOAsHjneWGeuq4M,55
+ascend_deployer/playbooks/roles/mindx.k8s/tests/inventory,sha256=yKsxPZwunWReo9UF4Yeuzhktj9QBBOmrryHZukdAyak,37
+ascend_deployer/playbooks/roles/mindx.k8s/tests/test.yml,sha256=OfjTIOR1OLIp-jTG-H0JGrAgFfKgNFb9k40OwGZwwcI,116
+ascend_deployer/playbooks/roles/mindx.k8s/vars/main.yml,sha256=Qz0ltVfvffbwEuSEBB5_EBXNoRqAbzrqUIfz52yfCTs,485
+ascend_deployer/playbooks/roles/mindx.kubeedge/README.md,sha256=GR4-d5SLMMehmWBbBNrzcN9GQ6fJa19VYPNOdbsu55I,78
+ascend_deployer/playbooks/roles/mindx.kubeedge/defaults/main.yml,sha256=oPyGFMkifGhQuic6xMeZcjq1stZwz5beoIwHghXxwZk,243
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/certgen.sh,sha256=vGH1cb9rmzK2BcYQCsTeSugcOnejAowZotqcbmKi93E,3498
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/cloudcore.service,sha256=xxxJLX5WTE0IJrige-s8s6jnmkq-pCm09VqDQrvYpkM,162
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/cluster_objectsync_v1alpha1.yaml,sha256=vCVJRNNwuleGKWaoYz77DEYDst8Uv_Sw3lDfgV1EwAw,1896
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_device.yaml,sha256=ImwcEivucISHilWW2Qcf2YJcHF6O7XICmwzNq6MNcZw,8715
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/devices_v1alpha1_devicemodel.yaml,sha256=XXm1lB_aU1KOshj1Fi9if2jA98pMFdu1ISNbg-vvyy4,10576
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/objectsync_v1alpha1.yaml,sha256=h6btWq1S2NXWFLJUyIdaSSjpo699-ovF-nI_oWWqWxY,1877
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_rule.yaml,sha256=nry_fOwbj5epjvzi9ItjdwwCHudYz3NcGt84KHrlk5g,2443
+ascend_deployer/playbooks/roles/mindx.kubeedge/files/router_v1_ruleEndpoint.yaml,sha256=K2QGKpuGUgDuK5EbsWI5UTXaGwu_-TS8sOfcLslXvYo,1355
+ascend_deployer/playbooks/roles/mindx.kubeedge/meta/main.yml,sha256=EfM1TxOjLrD1JvVMnJI0hOrGGGXW8ukPeFU-i4CvVg4,176
+ascend_deployer/playbooks/roles/mindx.kubeedge/tasks/main.yml,sha256=dGktJj8fUB022D5BiAh8Y17Zp8WGzhHlFcSCG5JzeaI,5145
+ascend_deployer/playbooks/roles/mindx.rep/defaults/main.yml,sha256=a5xqx4dWRzMmrNs99mpt875vWZVqixR1y6wYz-0CE8E,144
+ascend_deployer/playbooks/roles/mindx.rep/tasks/get_npu_info.py,sha256=pKNZpC9IRYRstrQsp4kQVpg-duUF6AGABO3CL98mJn0,528
+ascend_deployer/playbooks/roles/mindx.rep/tasks/hccn_rep.yaml,sha256=aXqOVll8mYyJ3oHM-UvZxW8whY6pdtyuSSVfNll-g_k,1732
+ascend_deployer/playbooks/roles/mindx.rep/tasks/json_to_csv.py,sha256=AkkYNfy2u4nv_JhXkVvJ6FIVPA3mEYLjnjjRbgbT9eg,2268
+ascend_deployer/playbooks/roles/mindx.rep/tasks/k8s_rep.py,sha256=GzFoQG97RubW7sciJXRpc1lMY6y1BwsVxbuZrfWSJVE,6312
+ascend_deployer/playbooks/roles/mindx.rep/tasks/local_rep.yaml,sha256=7feyvSbmb9j4O3xB98m6k_endsDh3EOhK53lJM84_5s,1146
+ascend_deployer/playbooks/roles/mindx.rep/tasks/ls_format.py,sha256=KjjDJDv1rzCM7kVkUBg7C0sdcdTZEP8BQ2YMGQ_aYjY,1011
+ascend_deployer/playbooks/roles/mindx.rep/tasks/output_json.py,sha256=W0gdfG9JksCkYJQIS-XZyBdvCTXQbqRNyXX0oV-UUSs,786
+ascend_deployer/playbooks/roles/mindx.rep/tasks/packages_rep.yaml,sha256=bLJaJpEyAqSibIMSql8jHpbRY4n04RscgUXv1Ui8PhE,1666
+ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_k8s_docker.yaml,sha256=JDDiO0oedEzlSRz1uNeBPMrhWw86vhNtI2fN4PgKT7Q,389
+ascend_deployer/playbooks/roles/mindx.uninstall_mef_relate/task/mindx.uninstall_mef_kubeedge.yaml,sha256=z55v95_ueyFs3zQmUnkRt9ixoZcCZI0PsjD-w3ULxHM,390
+ascend_deployer/playbooks/scene/scene_auto.yml,sha256=tEPEu4K10RQZS3yw41r_Xjmt2vatlecQeIqPytSc6Bo,960
+ascend_deployer/playbooks/scene/scene_dl.yml,sha256=Kg2IjLVI9YSaEXDnWSWOCVkh7FT8C6TM0AL9XkJbbMQ,660
 ascend_deployer/playbooks/scene/scene_edge.yml,sha256=w3idz1HuKo6qKcJr-m44iTDOP4wOiBYdQlXvCDSsUYw,259
-ascend_deployer/playbooks/scene/scene_mindspore.yml,sha256=iFc5mDVl_St7AEScivuAKO6LR01W2lcT8ehmxVD8PqY,442
-ascend_deployer/playbooks/scene/scene_offline_dev.yml,sha256=aH96nywqvj5xVpqDzic5SNFaY_88eoG79MMa19wYwyI,363
-ascend_deployer/playbooks/scene/scene_offline_run.yml,sha256=hEsWh3v_TZWsXZLGNKkiFmfbRUAeeKYk8rNdYLMDx3g,357
-ascend_deployer/playbooks/scene/scene_pytorch_dev.yml,sha256=5pkIMQYNCCxnvdwqSOVLRNpxJGTgVAN-cCcUWxknJaw,438
-ascend_deployer/playbooks/scene/scene_pytorch_run.yml,sha256=8yFeVzYiPzJSyVqSIuHWrjDgXtaO56pAY1BEQjgoAzs,432
-ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml,sha256=dW-SX9hAdsjhH3ivqIm5CvxRBUwgcarCzNRMBxxvLp0,521
-ascend_deployer/playbooks/scene/scene_tensorflow_run.yml,sha256=TRKWd4MevaSbLNsTWrVCz4PF9I62WyhgpDMiJB3a7cA,515
+ascend_deployer/playbooks/scene/scene_mef.yml,sha256=Ha1s39j0tKwkhQag4YhD8ka1ZgyCh9v5WskhYaHGVsY,491
+ascend_deployer/playbooks/scene/scene_mindspore.yml,sha256=N8jl61OrdJ3Petl0irWUEXiDX4brIScPLa5il-UDNAw,514
+ascend_deployer/playbooks/scene/scene_offline_dev.yml,sha256=SEO7UmhRiBtoN_n9HJJyXaJs7bGe2BRR6pyYHI0OBkc,435
+ascend_deployer/playbooks/scene/scene_offline_run.yml,sha256=6aD5f1mua65hL8tB4osBmElFkW88PYosFsmR4OFYN1s,354
+ascend_deployer/playbooks/scene/scene_pytorch_dev.yml,sha256=jC69LyU98npgE1GIHMwaAvBKj5hnWQkeqNou5jdXr0I,510
+ascend_deployer/playbooks/scene/scene_pytorch_run.yml,sha256=em4k3qeeh_-qN8n-QJ2Oh1DQMUU9slsOTdg29eoUBkw,504
+ascend_deployer/playbooks/scene/scene_tensorflow_dev.yml,sha256=D4_mrI4NKLMD_4fsC7Njb2op103Ym9TzLVwaBlT65Xg,593
+ascend_deployer/playbooks/scene/scene_tensorflow_run.yml,sha256=usd-zORtPFqmsHEz3I1EMsCsvhm383eo2-EY2v8_BJg,587
 ascend_deployer/playbooks/scene/scene_vmhost.yml,sha256=g9ffCyxfOnsgTkUW3lwmYaps9ndwpTOqsy_MQtQA6Y4,273
 ascend_deployer/playbooks/test/case_driver.yml,sha256=9HlGjFD4sqpe-1OTObGUEO4ljKedTnsMwkis346CvMc,2180
 ascend_deployer/playbooks/test/case_firmware.yml,sha256=WEF3Lre7cxcCsPKLpgZFS5aCXAB6Yeyv-hIw2Ho-woA,567
 ascend_deployer/playbooks/test/case_mindspore.yml,sha256=HOBN29_UPO53tQHFmsngi4_6jp_LyrVpmf1-QAfwCBk,4679
 ascend_deployer/playbooks/test/case_nnae.yml,sha256=Yl-8OpMOHDnYhfrZbrYu9jPQjmbnX39FQQbLegFs2zM,1466
 ascend_deployer/playbooks/test/case_nnrt.yml,sha256=BSc8ub1z3G6jfIl5pf61nQX1SZTeg6cXTz18ZtuJYV8,1466
 ascend_deployer/playbooks/test/case_pytorch.yml,sha256=BjrWe331g-WtyeAVl2rpYwK6OBu8U5_APzt22204Hi0,3095
@@ -245,18 +346,55 @@
 ascend_deployer/playbooks/test/test_nnae.yml,sha256=XoQXcfFppRtu29ntX96xbP_EmjwkplqUvGRB2HITM4A,90
 ascend_deployer/playbooks/test/test_nnrt.yml,sha256=K1VWj2uRXfKqcjuMyU2PuOqLbzstgm-S5hwz5P8t2Rc,89
 ascend_deployer/playbooks/test/test_pytorch.yml,sha256=2hZXx8jklP6bmApcRNYelFwx7i9oGEak5-_Ag0pmH0c,96
 ascend_deployer/playbooks/test/test_tensorflow.yml,sha256=xVVNWd_c0DByGfi_jnwpe6vJgDrnBdYUDwGtcPkK6Wg,101
 ascend_deployer/playbooks/test/test_tfplugin.yml,sha256=fm-IvOolhycuY45svRn-cXt3cYcnwLKYzxtObWNR7Gg,97
 ascend_deployer/playbooks/test/test_toolbox.yml,sha256=5ifAcGk0GLj1GfZD1bljSObTy0_z-ehvqKQe6CPHqJQ,104
 ascend_deployer/playbooks/test/test_toolkit.yml,sha256=YfwXJlVmRewWXuSzeUK5Mi28LfXU9ytNvWbWbXEErBo,95
+ascend_deployer/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+ascend_deployer/scripts/ascend_deploy.py,sha256=Uf0_HEYbHf0ejruac33bzpPXGba0S2_qWZ_4d_ID7vU,19112
+ascend_deployer/scripts/backup.sh,sha256=IMtwx3X1rs64f5QVnbw0WxjUJ8ig4Cc9MFO5vdVt4eo,870
+ascend_deployer/scripts/check.sh,sha256=r3eBgNogwQ_BeM9BFUZDw7yXPvul9VhB7lzbXaRXLmA,368
+ascend_deployer/scripts/check_pkgs.sh,sha256=-h5QjBJ1S4WShBq-ayHvsO_SU89LdENqnF7vDw8Ulq8,20699
+ascend_deployer/scripts/hccn_set.sh,sha256=6FINjouAhzsuM1_UWnA65oqA6TCfOFKLH9QeLAnT8R8,249
+ascend_deployer/scripts/image_load.sh,sha256=qWdGBVy0_c60yDYmPAtnRPFwiCD_X-eOK7bROL-yyP8,1142
+ascend_deployer/scripts/install.sh,sha256=u-mtTLGfx_0FOuqrF0qV2QZD_oFwDeDf6_XMlNFiZ4g,969
+ascend_deployer/scripts/install_ansible.sh,sha256=DEXh1Acvs3gheDoVN8tuIKV8h_Tg9oHJpppnvxQ1Dhs,3587
+ascend_deployer/scripts/install_kubeedge.sh,sha256=tnEs3MPhjIRRn4OwVet3uTc4R9Bt72PXpeLSwCti2jw,272
+ascend_deployer/scripts/machine_report.sh,sha256=RO9NaI8CSRSXUEI42Cwu09Twjqzxmo9qkT8JgV8NTJA,248
+ascend_deployer/scripts/nexus.py,sha256=KAfQK61T77HzwcoT9XinqkXgRDLVBlKqaaRAuQ82X0c,14207
+ascend_deployer/scripts/nexus_config.json,sha256=yZ4oy6BkuBdVmoheGBw7yTs7FLnnE66o-ut34lcyT0Q,1257
+ascend_deployer/scripts/uninstall_k8s_docker.sh,sha256=nSY6GniAuiaDI3Emj-BCRY38IRPHklYZ2OIMDgDVf90,535
+ascend_deployer/scripts/uninstall_mef_kubeedge.sh,sha256=8g3Yni8tl1Rgy5slpNIqdJozZcmp5O9x0b7TBAjX2j4,643
+ascend_deployer/scripts/uninstall_mef_related.sh,sha256=7tu9AcnPMxpbsjBMicW3udsKn8_aIcA9Za9h75xp11c,679
+ascend_deployer/scripts/upgrade.sh,sha256=_V4HXlSRTdbrKvf3POHJJxN_9X-WFp0lPSbpHcgzXCc,673
+ascend_deployer/scripts/utils.sh,sha256=sHVwhZydgv2vF1GQ9QBPjWwCtWccb_Q5IGSeIbjWaOA,5723
 ascend_deployer/tools/DeviceIP-conf.sh,sha256=R74aTgi2D2TqggSvXLj6tViTC7FwTODvA5rSx26eCW8,10900
 ascend_deployer/tools/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
+ascend_deployer/tools/check.py,sha256=cu3uzA14apAt1DqK273XWkfABwxTUafDmRLN35tiI14,4049
+ascend_deployer/tools/hccn.py,sha256=q-7y4y93FOmKoqePnJNpE-DHOTVcEo3QzTSarZw_7mI,7085
 ascend_deployer/tools/update_crl.sh,sha256=VwBHBTughh1qOxqqurddYS37blB96iH2eTkBSHpcgaE,9930
-ascend_deployer-5.0.0b3.data/scripts/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
-ascend_deployer-5.0.0b3.dist-info/DESCRIPTION.rst,sha256=zON3uGMMQQVmrr8K226q5LJRxzdTaf470LeDWZ332Vw,4131
-ascend_deployer-5.0.0b3.dist-info/METADATA,sha256=ZjpXpuDWliBf1XX765GtPxsLSD8yxCgIFTcB8YMtqFk,4575
-ascend_deployer-5.0.0b3.dist-info/RECORD,,
-ascend_deployer-5.0.0b3.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-ascend_deployer-5.0.0b3.dist-info/entry_points.txt,sha256=c2iLI_gKqp8fhoFfDS3gGyWpKf5M5OqrMjq55UhjJ2M,80
-ascend_deployer-5.0.0b3.dist-info/metadata.json,sha256=bPYEG7Qej0fSauUYsFshOzT2IXqPMA9x0m54_6rcZ7c,789
-ascend_deployer-5.0.0b3.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
+ascend_deployer/tools/hccn/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
+ascend_deployer/tools/hccn/main/hccn.go,sha256=robmOcfv1cHeM__UTnU2-sP6wDRBcId4UwSP8hkbGVc,6863
+ascend_deployer/tools/report/main/go.mod,sha256=T_4E5SwIfDiUuU3LukbU4QKLaPEFaZ1lgb-GQcsNRuA,142
+ascend_deployer/tools/report/main/main.go,sha256=MnVc5U17AAEu150DdFrziPgRtfgqxLsav2PbOiagr80,18729
+ascend_deployer/tools/unzip/main/go.mod,sha256=YgIwnIERMSUYwOhf99p-SJRh8X__2XsNQVJOHMMx0eA,21
+ascend_deployer/tools/unzip/main/unzip.go,sha256=-Z0ihIicC_3GihItvhc1it3PQoyFLSz0ycGuKj82wlk,1587
+ascend_deployer/yamls/basic.yaml,sha256=LMbvOfJ78T5dXk0YEhATGNGiMe4_sSnzt6MoT_bu4I0,46
+ascend_deployer/yamls/check.yaml,sha256=74W_bQT1to6tJGK2FPrggJuFbogaAzXK7oDDLaR3xrk,46
+ascend_deployer/yamls/docker.yaml,sha256=4OEYn9_0xxyMCpl1qdJhiTZ3MctxhUdz3uXYRxzYwwY,132
+ascend_deployer/yamls/gather_facts.yaml,sha256=-LQEyu7YPjZ_BKJ9o606nkIIzWZXy4-AXjijkdTV63k,53
+ascend_deployer/yamls/harbor.yaml,sha256=4YmjA4UTdAhNLB4pH2d8G2jTnIiNELbMYY-VCqxO2y0,72
+ascend_deployer/yamls/hccn.yaml,sha256=5VuwXcGseHty7iA7s4z8YKlupyu0HRe9j_WvjLTCRKk,45
+ascend_deployer/yamls/image_load.yaml,sha256=8P1n5bl4dZo-F5Q_7-F2JIMngGnWESzEr3qzIC4JaPw,51
+ascend_deployer/yamls/k8s.yaml,sha256=OwWlFC9IPOYT-2GT4LJUYMZCC2qKSI1o9X1dw8vvEpo,126
+ascend_deployer/yamls/k8s_reset.yaml,sha256=BUkmH2NmaIPzevXbf6c_S8jT7kL7sHfVq9YILxqswVk,234
+ascend_deployer/yamls/mindxdl.yaml,sha256=xvHRj2q-tMw8G0x6CcXZ8gbdKuyEvsxEDj02u_1es4A,74
+ascend_deployer/yamls/report.yaml,sha256=OABhE8u336Y0ILTBln4mSw3s8llyDRnA1B5ZdVzmExY,47
+ascend_deployer-5.0.0b4.data/scripts/ascend-deployer,sha256=7KBABYrGdNiIJFzRpA90YMi7v9BDchcsDAji3JoCTOE,1409
+ascend_deployer-5.0.0b4.dist-info/DESCRIPTION.rst,sha256=zON3uGMMQQVmrr8K226q5LJRxzdTaf470LeDWZ332Vw,4131
+ascend_deployer-5.0.0b4.dist-info/METADATA,sha256=jePRQJDyqrnAdh_XT7jR7s69Z35__dtKJAeyGHJRXLE,4575
+ascend_deployer-5.0.0b4.dist-info/RECORD,,
+ascend_deployer-5.0.0b4.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+ascend_deployer-5.0.0b4.dist-info/entry_points.txt,sha256=HjyLLr0zJ_k7sWdPoQgJB-Tc2jKReTuJDbM-6LqbKbc,74
+ascend_deployer-5.0.0b4.dist-info/metadata.json,sha256=ptmSKHshtrwxCsAchP660a5uSy6ucRG5eTLRKXpFV3M,777
+ascend_deployer-5.0.0b4.dist-info/top_level.txt,sha256=T3GbQwFRI8Cl3QuJELdNLLkq3kGZrvYBykFox-L0XCw,16
```

