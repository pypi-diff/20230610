# Comparing `tmp/networklab-1.5.3.post1.tar.gz` & `tmp/networklab-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.3.post1.tar", last modified: Tue May 16 06:08:39 2023, max compression
+gzip compressed data, was "networklab-1.5.4.tar", last modified: Sat Jun 10 16:47:15 2023, max compression
```

## Comparing `networklab-1.5.3.post1.tar` & `networklab-1.5.4.tar`

### file list

```diff
@@ -1,624 +1,621 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.819617 networklab-1.5.3.post1/
--rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/LICENSE.md
--rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/MANIFEST.in
--rw-r--r--   0 pipi       (501) staff       (20)     3878 2023-05-16 06:08:39.819384 networklab-1.5.3.post1/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)     3163 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/README.md
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.672731 networklab-1.5.3.post1/netsim/
--rwxr-xr-x   0 pipi       (501) staff       (20)       52 2023-05-16 06:02:15.000000 networklab-1.5.3.post1/netsim/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)    13301 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/addressing.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.674327 networklab-1.5.3.post1/netsim/ansible/
--rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     2714 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/config.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/create-config.ansible
--rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.3.post1/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     3424 2023-01-25 10:08:09.000000 networklab-1.5.3.post1/netsim/ansible/initial-config.ansible
--rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.3.post1/netsim/ansible/missing.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.675056 networklab-1.5.3.post1/netsim/ansible/tasks/
--rw-r--r--   0 pipi       (501) staff       (20)      684 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.679599 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3084 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2142 2023-01-25 10:08:09.000000 networklab-1.5.3.post1/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.686222 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.686700 networklab-1.5.3.post1/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.687019 networklab-1.5.3.post1/netsim/ansible/tasks/frr/
--rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.3.post1/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)      243 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/tasks/frr/mpls-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.687231 networklab-1.5.3.post1/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.687454 networklab-1.5.3.post1/netsim/ansible/tasks/linux/
--rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.687673 networklab-1.5.3.post1/netsim/ansible/tasks/nxos/
--rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.3.post1/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.688182 networklab-1.5.3.post1/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/tasks/readiness-check/routeros7.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.688352 networklab-1.5.3.post1/netsim/ansible/tasks/vmx/
--rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.3.post1/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.688589 networklab-1.5.3.post1/netsim/ansible/templates/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.690320 networklab-1.5.3.post1/netsim/ansible/templates/bfd/
--rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.696852 networklab-1.5.3.post1/netsim/ansible/templates/bgp/
--rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     8013 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3252 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.697196 networklab-1.5.3.post1/netsim/ansible/templates/eigrp/
--rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.699277 networklab-1.5.3.post1/netsim/ansible/templates/evpn/
--rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1580 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1782 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1090 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.701195 networklab-1.5.3.post1/netsim/ansible/templates/gateway/
--rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.3.post1/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.709743 networklab-1.5.3.post1/netsim/ansible/templates/initial/
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     5271 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.710471 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      906 2022-12-22 08:29:57.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2918 2022-12-22 09:39:24.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1933 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3479 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4711 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.3.post1/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.712775 networklab-1.5.3.post1/netsim/ansible/templates/isis/
--rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.3.post1/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.719343 networklab-1.5.3.post1/netsim/ansible/templates/mpls/
--rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      562 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1159 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      342 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.728440 networklab-1.5.3.post1/netsim/ansible/templates/ospf/
--rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.729901 networklab-1.5.3.post1/netsim/ansible/templates/sr/
--rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.730129 networklab-1.5.3.post1/netsim/ansible/templates/srv6/
--rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.733207 networklab-1.5.3.post1/netsim/ansible/templates/vlan/
--rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.744256 networklab-1.5.3.post1/netsim/ansible/templates/vrf/
--rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1202 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.746956 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/
--rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1651 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2234 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.3.post1/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/api.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.751564 networklab-1.5.3.post1/netsim/augment/
--rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/augment/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/augment/components.py
--rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/augment/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     3343 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/augment/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)    17444 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/augment/groups.py
--rw-r--r--   0 pipi       (501) staff       (20)    40712 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/augment/links.py
--rw-r--r--   0 pipi       (501) staff       (20)     3179 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/augment/main.py
--rw-r--r--   0 pipi       (501) staff       (20)    12604 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/augment/nodes.py
--rw-r--r--   0 pipi       (501) staff       (20)     2814 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/augment/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     7563 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/augment/topology.py
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/callback.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.757013 networklab-1.5.3.post1/netsim/cli/
--rwxr-xr-x   0 pipi       (501) staff       (20)     9700 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.3.post1/netsim/cli/alias.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1758 2022-03-20 09:00:36.000000 networklab-1.5.3.post1/netsim/cli/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     4192 2022-12-11 09:34:30.000000 networklab-1.5.3.post1/netsim/cli/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.3.post1/netsim/cli/collect.py
--rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.3.post1/netsim/cli/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     5556 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/connect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2974 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/create.py
--rw-r--r--   0 pipi       (501) staff       (20)     6747 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/down.py
--rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.3.post1/netsim/cli/empty.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6273 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/cli/external_commands.py
--rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/cli/initial.py
--rw-r--r--   0 pipi       (501) staff       (20)     2038 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/cli/install.py
--rw-r--r--   0 pipi       (501) staff       (20)     9143 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/cli/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.3.post1/netsim/cli/read.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/restart.py
--rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-03-06 07:47:06.000000 networklab-1.5.3.post1/netsim/cli/show.py
--rw-r--r--   0 pipi       (501) staff       (20)     4785 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/cli/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     3453 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/cli/test.py
--rw-r--r--   0 pipi       (501) staff       (20)    10689 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/cli/up.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.3.post1/netsim/cli/usage.py
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/cli/usage.txt
--rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/cli/version.py
--rw-r--r--   0 pipi       (501) staff       (20)     1470 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/common.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.757991 networklab-1.5.3.post1/netsim/data/
--rw-r--r--   0 pipi       (501) staff       (20)     4805 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/data/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3076 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/data/filemaps.py
--rw-r--r--   0 pipi       (501) staff       (20)     1329 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/data/global_vars.py
--rw-r--r--   0 pipi       (501) staff       (20)    20638 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/data/types.py
--rw-r--r--   0 pipi       (501) staff       (20)    19459 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/data/validate.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.759250 networklab-1.5.3.post1/netsim/defaults/
--rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/defaults/addressing.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2452 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/defaults/attributes.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/defaults/automation.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/defaults/hints.yml
--rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/defaults/multilab.yml
--rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/defaults/ports.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.770507 networklab-1.5.3.post1/netsim/devices/
--rw-r--r--   0 pipi       (501) staff       (20)     1812 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      854 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/arubacx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/arubacx.yml
--rw-r--r--   0 pipi       (501) staff       (20)      950 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/asav.py
--rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/devices/asav.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1223 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/csr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2241 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/eos.py
--rw-r--r--   0 pipi       (501) staff       (20)     1593 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      927 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      822 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/iosv.py
--rw-r--r--   0 pipi       (501) staff       (20)     1411 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/iosv.yml
--rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/junos.py
--rw-r--r--   0 pipi       (501) staff       (20)      705 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1148 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      858 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1355 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/devices/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1632 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/devices/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      932 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/devices/unknown.py
--rw-r--r--   0 pipi       (501) staff       (20)      115 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/devices/unknown.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/vmx.py
--rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/vmx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2314 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/devices/vsrx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/vsrx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/devices/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.668558 networklab-1.5.3.post1/netsim/extra/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.770685 networklab-1.5.3.post1/netsim/extra/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.3.post1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.776925 networklab-1.5.3.post1/netsim/extra/ebgp.utils/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.777475 networklab-1.5.3.post1/netsim/extra/ebgp.utils/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     4976 2023-04-15 13:39:23.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4470 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.3.post1/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.777738 networklab-1.5.3.post1/netsim/extra/multilab/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.778272 networklab-1.5.3.post1/netsim/extra/multilab/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.3.post1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3509 2023-04-15 10:43:11.000000 networklab-1.5.3.post1/netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.3.post1/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.778541 networklab-1.5.3.post1/netsim/extra/none/
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/extra/none/none.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.779108 networklab-1.5.3.post1/netsim/extra/proxy-arp/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.779861 networklab-1.5.3.post1/netsim/extra/proxy-arp/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     1772 2023-04-15 10:43:07.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.781131 networklab-1.5.3.post1/netsim/install/
--rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.3.post1/netsim/install/ansible.sh
--rwxr--r--   0 pipi       (501) staff       (20)     3619 2023-05-15 14:43:12.000000 networklab-1.5.3.post1/netsim/install/containerlab.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.3.post1/netsim/install/grpc.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.785015 networklab-1.5.3.post1/netsim/install/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.785370 networklab-1.5.3.post1/netsim/install/libvirt/asav/
--rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/install/libvirt/asav.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.3.post1/netsim/install/libvirt/csr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.3.post1/netsim/install/libvirt/eos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/install/libvirt/iosv.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.785760 networklab-1.5.3.post1/netsim/install/libvirt/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.3.post1/netsim/install/libvirt/iosxr/iosxr_config.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.3.post1/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.3.post1/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.786045 networklab-1.5.3.post1/netsim/install/libvirt/vsrx/
--rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.3.post1/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.3.post1/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 pipi       (501) staff       (20)     3179 2023-01-12 13:45:42.000000 networklab-1.5.3.post1/netsim/install/libvirt.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/install/ubuntu.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.792816 networklab-1.5.3.post1/netsim/modules/
--rw-r--r--   0 pipi       (501) staff       (20)    23624 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/modules/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6155 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/_dataplane.py
--rw-r--r--   0 pipi       (501) staff       (20)    10721 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/_routing.py
--rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.3.post1/netsim/modules/bfd.py
--rw-r--r--   0 pipi       (501) staff       (20)      702 2023-05-04 17:17:54.000000 networklab-1.5.3.post1/netsim/modules/bfd.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20495 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/bgp.py
--rw-r--r--   0 pipi       (501) staff       (20)     1470 2023-05-04 17:17:47.000000 networklab-1.5.3.post1/netsim/modules/bgp.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.3.post1/netsim/modules/eigrp.py
--rw-r--r--   0 pipi       (501) staff       (20)      324 2023-05-04 17:17:42.000000 networklab-1.5.3.post1/netsim/modules/eigrp.yml
--rw-r--r--   0 pipi       (501) staff       (20)    17695 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/evpn.py
--rw-r--r--   0 pipi       (501) staff       (20)      892 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/evpn.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6763 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/gateway.py
--rw-r--r--   0 pipi       (501) staff       (20)      960 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/gateway.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/modules/isis.py
--rw-r--r--   0 pipi       (501) staff       (20)      906 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/modules/isis.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7051 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/mpls.py
--rw-r--r--   0 pipi       (501) staff       (20)      879 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/mpls.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3036 2023-01-14 10:57:46.000000 networklab-1.5.3.post1/netsim/modules/ospf.py
--rw-r--r--   0 pipi       (501) staff       (20)     1067 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/modules/ospf.yml
--rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/modules/sr.py
--rw-r--r--   0 pipi       (501) staff       (20)      390 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/modules/sr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.3.post1/netsim/modules/srv6.py
--rw-r--r--   0 pipi       (501) staff       (20)      420 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/modules/srv6.yml
--rw-r--r--   0 pipi       (501) staff       (20)    58619 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vlan.py
--rw-r--r--   0 pipi       (501) staff       (20)     1022 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vlan.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20435 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vrf.py
--rw-r--r--   0 pipi       (501) staff       (20)      431 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vrf.yml
--rw-r--r--   0 pipi       (501) staff       (20)     9043 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vxlan.py
--rw-r--r--   0 pipi       (501) staff       (20)      564 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/modules/vxlan.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.796447 networklab-1.5.3.post1/netsim/outputs/
--rw-r--r--   0 pipi       (501) staff       (20)     2233 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     7081 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/outputs/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     1786 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/common.py
--rw-r--r--   0 pipi       (501) staff       (20)    10000 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/d2.py
--rw-r--r--   0 pipi       (501) staff       (20)      545 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/d2.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2754 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.3.post1/netsim/outputs/format.py
--rw-r--r--   0 pipi       (501) staff       (20)     7545 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/outputs/graph.yml
--rw-r--r--   0 pipi       (501) staff       (20)      641 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.3.post1/netsim/outputs/json.py
--rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.3.post1/netsim/outputs/none.py
--rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/outputs/provider.py
--rw-r--r--   0 pipi       (501) staff       (20)     2667 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/tools.py
--rw-r--r--   0 pipi       (501) staff       (20)     1688 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/outputs/yaml.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.799964 networklab-1.5.3.post1/netsim/providers/
--rw-r--r--   0 pipi       (501) staff       (20)     7933 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/providers/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3873 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/providers/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)      965 2023-05-15 14:43:12.000000 networklab-1.5.3.post1/netsim/providers/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.3.post1/netsim/providers/external.py
--rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/providers/external.yml
--rw-r--r--   0 pipi       (501) staff       (20)    11779 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/providers/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1157 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/providers/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.3.post1/netsim/providers/virtualbox.py
--rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/providers/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7799 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/read_topology.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.800205 networklab-1.5.3.post1/netsim/templates/
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.3.post1/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.669667 networklab-1.5.3.post1/netsim/templates/provider/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.800590 networklab-1.5.3.post1/netsim/templates/provider/clab/
--rw-r--r--   0 pipi       (501) staff       (20)     3143 2023-05-15 14:43:12.000000 networklab-1.5.3.post1/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.800868 networklab-1.5.3.post1/netsim/templates/provider/clab/frr/
--rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.801172 networklab-1.5.3.post1/netsim/templates/provider/clab/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.3.post1/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.801717 networklab-1.5.3.post1/netsim/templates/provider/external/
--rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.3.post1/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.809911 networklab-1.5.3.post1/netsim/templates/provider/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)      541 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      952 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:30:59.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.3.post1/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.812652 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/
--rw-r--r--   0 pipi       (501) staff       (20)      782 2022-05-02 06:40:29.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.3.post1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.813520 networklab-1.5.3.post1/netsim/templates/tests/
--rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.3.post1/netsim/templates/tests/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.3.post1/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.3.post1/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.815101 networklab-1.5.3.post1/netsim/tools/
--rw-r--r--   0 pipi       (501) staff       (20)      764 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/tools/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     5106 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/tools/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      614 2023-05-15 07:05:40.000000 networklab-1.5.3.post1/netsim/tools/graphite.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.815313 networklab-1.5.3.post1/netsim/tools/suzieq/
--rw-r--r--   0 pipi       (501) staff       (20)      304 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 pipi       (501) staff       (20)      643 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/tools/suzieq.yml
--rw-r--r--   0 pipi       (501) staff       (20)      542 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/topology-defaults.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.818060 networklab-1.5.3.post1/netsim/utils/
--rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/utils/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     4068 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/netsim/utils/log.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.3.post1/netsim/utils/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     1354 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/utils/strings.py
--rw-r--r--   0 pipi       (501) staff       (20)     4906 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/netsim/utils/templates.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.818922 networklab-1.5.3.post1/networklab.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)     3878 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)    21019 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       51 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/entry_points.txt
--rw-r--r--   0 pipi       (501) staff       (20)      120 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        7 2023-05-16 06:08:39.000000 networklab-1.5.3.post1/networklab.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)      181 2023-04-27 06:49:41.000000 networklab-1.5.3.post1/requirements.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-05-16 06:08:39.819662 networklab-1.5.3.post1/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.3.post1/setup.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-05-16 06:08:39.819076 networklab-1.5.3.post1/tests/
--rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.3.post1/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-10 16:47:05.000000 networklab-1.5.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-10 16:47:05.000000 networklab-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 16:47:15.521443 networklab-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-10 16:47:05.000000 networklab-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.421442 networklab-1.5.4/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/addressing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.425442 networklab-1.5.4/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2714 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1269 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3424 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/missing.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.425442 networklab-1.5.4/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/frr/mpls-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.429442 networklab-1.5.4/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.433442 networklab-1.5.4/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.437442 networklab-1.5.4/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.445442 networklab-1.5.4/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.449442 networklab-1.5.4/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.449442 networklab-1.5.4/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.457442 networklab-1.5.4/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.465443 networklab-1.5.4/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.469443 networklab-1.5.4/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.477443 networklab-1.5.4/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 16:47:05.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.477443 networklab-1.5.4/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.481443 networklab-1.5.4/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17444 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40808 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.481443 networklab-1.5.4/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9700 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.485443 networklab-1.5.4/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19459 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.485443 networklab-1.5.4/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.417442 networklab-1.5.4/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.493443 networklab-1.5.4/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3619 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.497443 networklab-1.5.4/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.501443 networklab-1.5.4/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1089 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.501443 networklab-1.5.4/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1881 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.505443 networklab-1.5.4/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    58619 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20435 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/providers/virtualbox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/read_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.421442 networklab-1.5.4/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.509443 networklab-1.5.4/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.517443 networklab-1.5.4/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-06-10 16:47:06.000000 networklab-1.5.4/netsim/utils/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 16:47:15.000000 networklab-1.5.4/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-10 16:47:06.000000 networklab-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 16:47:15.521443 networklab-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-10 16:47:06.000000 networklab-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 16:47:15.521443 networklab-1.5.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-06-10 16:47:06.000000 networklab-1.5.4/tests/test_transformation.py
```

### Comparing `networklab-1.5.3.post1/LICENSE.md` & `networklab-1.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/PKG-INFO` & `networklab-1.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.3.post1
+Version: 1.5.4
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.3](https://github.com/ipspace/netlab/releases/tag/release_1.5.3), which is the only release that works with the latest *containerlab* release (0.41.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
```

### Comparing `networklab-1.5.3.post1/README.md` & `networklab-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.3](https://github.com/ipspace/netlab/releases/tag/release_1.5.3), which is the only release that works with the latest *containerlab* release (0.41.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
```

### Comparing `networklab-1.5.3.post1/netsim/addressing.py` & `networklab-1.5.4/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/collect-configs.ansible` & `networklab-1.5.4/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/config.ansible` & `networklab-1.5.4/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/create-config.ansible` & `networklab-1.5.4/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/initial-config.ansible` & `networklab-1.5.4/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/create-config.yml` & `networklab-1.5.4/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.4/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.4/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.4/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.5.4/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.4/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.4/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.4/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files 8% similar despite different names*

```diff
@@ -86,8 +86,20 @@
 
 {%   else %}
 {# TODO BGP unnumbered #}
 {%   endif %}
 {%  endfor %}
 {% endfor %}
 
+{% for pfx in vrf_bgp.originate|default([]) %}
+{%  if loop.first %}
+- path: configure/{{ path }}/static-routes
+  val:
+   route:
+{%  endif %}
+   - ip-prefix: {{ pfx }}
+     route-type: "unicast"
+     blackhole:
+      admin-state: "enable"
+{% endfor %}
+
 {% endmacro %}
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/sros.j2`

 * *Files 9% similar despite different names*

```diff
@@ -29,17 +29,18 @@
      # route-distinguisher: "{{ vdata.evpn.rd }}" # use auto-rd
      route-target:
       export: "target:{{ vdata.evpn.export[0] }}"
       import: "target:{{ vdata.evpn.import[0] }}"
 
    bgp-evpn:
     evi: {{ vdata.evpn.evi }}
+    # TODO if evpn.transport == 'mpls'
     mpls:
     - bgp-instance: 1
       admin-state: enable
-      ecmp: 32
-      ingress-replication-bum-label: True
+      ecmp: {{ 2 if 'ixr' in clab.type else 32 }}
+      # ingress-replication-bum-label: True # TODO, requires reserved label range
       auto-bind-tunnel:
        resolution: any
-       ecmp: 32
+       ecmp: {{ 2 if 'ixr' in clab.type else 32 }}
 {%   endfor %}
 {% endif %}
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/cumulus.j2`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 echo "Use vtysh to connect to FRR daemon"
 echo
 SCRIPT
 #
 # Build hosts file
 #
 echo "INIT: setting hostname"
-hostname {{ inventory_hostname }}
+hostname {{ inventory_hostname.replace("_","-") }}
 echo "INIT: creating /etc/hosts"
 awk '/127.0.1.1/,/^$/' /etc/hosts >/tmp/hosts
 echo "127.0.0.1 {{ inventory_hostname }}" >>/tmp/hosts
 {% for k,v in hostvars.items() if k != inventory_hostname and v.af.ipv4|default(False) %}
 echo "{%- if v.loopback.ipv4 is defined %}{{ v.loopback.ipv4|ipaddr('address') }} {% endif %}
 {%- for l in v.interfaces|default([]) if 'ipv4' in l and l.ipv4 != True and l.ipv4|ipv4 %}{{ l.ipv4|ipaddr('address') }} {% endfor %}{{ k }}" >>/tmp/hosts
 {% endfor %}
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {#
 # RAW interfaces with flexible vlan tagging, + VLAN TAGS
+# In case of vPTX, handle here only the L3 Subintfs
 #}
 
 interfaces {
 
 {% for l in interfaces|default([]) %}
 
 {%   if l.junos_interface != 'irb' and l.junos_unit != '0' and l.type|default('') == 'vlan_member' %}
@@ -16,15 +17,15 @@
 
   {{ l.ifname }} {
     vlan-id {{ l.vlan.access_id }};
   }
 
 {%   endif %}
 
-{%   if l.junos_interface != 'irb' and l.junos_unit == '0' %}
+{%   if l.junos_interface != 'irb' and l.junos_unit == '0' and l._vlan_master is defined and l._vlan_mode|default('') == 'route' %}
 {# This is the ethernet subinterface 0 #}
 {# -> we need to check if it's a "native vlan routed port", if yes #}
 {# -> we need to set native-vlan-id on the basic interface, and report the vlan id on the subunit #}
 
 {%     set ns = namespace(native_vlan="1") %}
 {%     if l._vlan_master|default(false) %}
 {%       if l._vlan_native_id is defined %}
@@ -39,23 +40,27 @@
   {{ l.junos_interface }}.0 {
     vlan-id {{ ns.native_vlan }};
   }
 
 {%     endif %}
 {%   endif %}
 
-{%   if l.junos_interface != 'irb' and l.junos_unit == '0' and l._vlan_master is defined and l.vlan.access_id is defined %}
+{%   if netlab_device_type != 'vptx' %}
+
+{%     if l.junos_interface != 'irb' and l.junos_unit == '0' and l._vlan_master is defined and l.vlan.access_id is defined %}
 {# this is a irb port in access mode on unit 0 #}
   {{ l.junos_interface }} {
     flexible-vlan-tagging;
     native-vlan-id {{ l.vlan.access_id }};
   }
 
   {{ l.ifname }} {
     vlan-id {{ l.vlan.access_id }};
   }
 
+{%     endif %}
+
 {%   endif %}
 
 {% endfor %}
 
 }
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/sros.j2`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,22 @@
 {#  Remove connector from port name for IXR platform #}
 {%  set portname = portname.replace("c","") %}
 {%  endif %}
 {%  if l.type in ['p2p','lan','vlan_member'] %}
 {%   if 'c' in portname %}
 - path: configure/port[port-id={{portname}}]
   val:
+   admin-state: enable
    connector:
     breakout: "c1-100g"
 {%    set portname = portname + '/1' %}
 {%   endif %}
 - path: configure/port[port-id={{ portname }}]
   val:
+   admin-state: enable
    ethernet:
 {%   set eth_header = 14 + (4 if tagged else 0) %}
 {%   if l.mtu is defined and l.mtu <= (9800-eth_header) %}
     mtu: {{ l.mtu + eth_header }} # max 9800
 {%   endif %}
 {%   if l.vlan.trunk_id is defined or (l.parent_ifindex is defined and interfaces[l.parent_ifindex-1].vlan.trunk_id is defined) %}
     mode: hybrid # Support mixed trunks by using hybrid ports
@@ -131,14 +133,20 @@
 - path: configure/system/resource
   val:
    ecmp-profile:
    - profile-id: 1
      type: ip # or mpls
      links: 16
      groups: 64
+{%  if 'mpls' in module %}
+   - profile-id: 2
+     type: mpls
+     links: 16
+     groups: 64
+{%  endif %}
 {% endif %}
 
 {# Enable ECMP=64 by default #}
 - path: configure/router[router-name=Base]
   val:
    ecmp: {{ 1 if 'ixr' in clab.type else 64 }}
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.4/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.4/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.4/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.4/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/sros.j2`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 - path: configure/service/vprn[service-name={{ vname }}]
   val:
    service-id: {{ vdata.vrfidx }}
    customer: "1"
    autonomous-system: {{ bgp.as|default(vrf.as) }}
    router-id: {{ vdata.bgp.router_id|default(bgp.router_id if bgp is defined else loopback.ipv4|ipaddr('address')) }}
-   ecmp: 64
+   ecmp: {{ 1 if 'ixr' in clab.type else 64 }}
    admin-state: enable
 
 {% if mpls is defined and 'vpn' in mpls %}
    bgp-ipvpn:
      mpls:
       admin-state: enable
       route-distinguisher: "{{ vdata.rd }}"
       vrf-target:
        export-community: "target:{{ vdata.export[0] }}" # For now a single community, TODO import policy
        import-community: "target:{{ vdata.import[0] }}"
       auto-bind-tunnel:
        resolution: "any"
-       ecmp: 32
+       ecmp: {{ 2 if 'ixr' in clab.type else 32 }}
 {% endif %}
 
 {% if vdata.bgp is defined %}
 {{ bgp_config(vdata.bgp,vname) }}
 {% endif %}
 
 {% if 'ospf' in vdata %}
```

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.4/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.4/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/api.py` & `networklab-1.5.4/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/components.py` & `networklab-1.5.4/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/config.py` & `networklab-1.5.4/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/devices.py` & `networklab-1.5.4/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/groups.py` & `networklab-1.5.4/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/links.py` & `networklab-1.5.4/netsim/augment/links.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     link_data = data.get_box({ '_linkname' : linkname })              # ... create stub link data structure
     link_data.interfaces = adjust_interface_list(l,link_data,nodes)   # ... and adjust interface list
     return link_data
 
   if isinstance(l,str):                                       # String, split into a list of nodes
     link_intf = []
     for n in l.split('-'):                # ... split it into a list of nodes
+      n = n.strip()                       # ... strip leading and trailing spaces (fixing #816)
       valid_node = n in nodes
       if not valid_node:
         valid_node = len([ x for x in nodes if n.startswith(x) ]) > 0
 
       if valid_node:                      # If the node name is valid
         link_intf.append({ 'node': n })   # ... append it to the list of interfaces
       else:
```

### Comparing `networklab-1.5.3.post1/netsim/augment/main.py` & `networklab-1.5.4/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/nodes.py` & `networklab-1.5.4/netsim/augment/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 * Discover desired imagex (boxes)
 * Add default module list to nodes without specific modules
 * Set loopback and management interface data
 '''
 import typing
 
 from box import Box
+import netaddr
 
 from .. import common
 from .. import data
 from .. import utils
 from .. import addressing
 from .. import providers
 from . import devices
@@ -134,15 +135,15 @@
       common.error(
         f'Cannot assign management address from prefix {str(addrs[pfx])} (starting at {addrs.start}) to node with ID {node.id}',
         common.IncorrectValue,
         'nodes')
 
   if addrs.mac_eui and not 'mac' in node.mgmt:                        # Finally, assign management MAC address
     addrs.mac_eui[5] = node.id
-    node.mgmt.mac = str(addrs.mac_eui)
+    node.mgmt.mac = addrs.mac_eui.format(netaddr.mac_unix_expanded)
 
   if not 'ipv4' in node.mgmt and not 'ipv6' in node.mgmt:             # Final check: did we get a usable management address?
     common.error(
       f'Node {node.name} does not have a usable management IP addresss',
       common.MissingValue,
       'nodes')
 
@@ -343,25 +344,27 @@
 
     if not n.name: # pragma: no cover (name should have been checked way before)
       common.fatal(f"Internal error: node does not have a name {n}",'nodes')
       return
 
     augment_node_device_data(n,defaults)
 
+    n.af = {}                                                 # Nodes must have AF attribute
     if pools.loopback and n.get('role','') != 'host':
       prefix_list = addressing.get(pools,['loopback'],n.id)
       for af in prefix_list:
         if isinstance(prefix_list[af],bool):
           if prefix_list[af]:
             common.fatal( f"Loopback addresses must be valid IP prefixes, not 'True': {prefix_list}" )
         elif not n.loopback[af]:
           if af == 'ipv6':
             n.loopback[af] = addressing.get_addr_mask(prefix_list[af],1)
           else:
             n.loopback[af] = str(prefix_list[af])
+          n.af[af] = True
 
     augment_mgmt_if(n,defaults,topology.addressing.mgmt)
     providers.execute_node("augment_node_data",n,topology)
 
 '''
 Return a copy of the topology (leaving original topology unchanged) with unmanaged devices removed
 '''
```

### Comparing `networklab-1.5.3.post1/netsim/augment/plugin.py` & `networklab-1.5.4/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/augment/topology.py` & `networklab-1.5.4/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/callback.py` & `networklab-1.5.4/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/__init__.py` & `networklab-1.5.4/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/ansible.py` & `networklab-1.5.4/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/clab.py` & `networklab-1.5.4/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/collect.py` & `networklab-1.5.4/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/config.py` & `networklab-1.5.4/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/connect.py` & `networklab-1.5.4/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/create.py` & `networklab-1.5.4/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/down.py` & `networklab-1.5.4/netsim/cli/down.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,31 +149,15 @@
       continue
     external_commands.execute_tool_commands(cmds,topology)
     if not is_dry_run():
       print(f"... {tool} tool stopped")
 
   lab_status_change(topology,f'external tools stopped')
 
-def run(cli_args: typing.List[str]) -> None:
-  args = down_parse(cli_args)
-  set_dry_run(args)
-
-  topology = load_snapshot(args)
-  print(f"Read transformed lab topology from snapshot file {args.snapshot}")
-
-  mismatch = lab_dir_mismatch(topology)
-
-  lab_status_change(topology,f'lab shutdown requested{" in conflicting directory" if mismatch else ""}')
-  try:
-    provider_probes(topology,1)
-  except:
-    if not args.force:
-      return
-
-  stop_step = 2
+def stop_all(topology: Box, args: argparse.Namespace, stop_step: int) -> int:
   if 'tools' in topology:
     external_commands.print_step(stop_step,"Stopping external tools",spacing=True)
     stop_step = stop_step + 1
     stop_external_tools(args,topology)
 
   p_provider = topology.provider
   p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
@@ -183,24 +167,49 @@
   for s_provider in topology[p_provider].providers:
     lab_status_change(topology,f'stopping {s_provider} provider')
     try:
       stop_provider_lab(topology,p_provider,s_provider,step=stop_step)
       stop_step = stop_step + 1
     except:
       if not args.force:
-        return
+        sys.exit(1)
     print()
 
   try:
+    lab_status_change(topology,f'stopping {p_provider} provider')
     stop_provider_lab(topology,p_provider,step=stop_step)
     stop_step = stop_step + 1
   except:
     if not args.force:
+      sys.exit(1)
+
+  return stop_step
+
+def run(cli_args: typing.List[str]) -> None:
+  args = down_parse(cli_args)
+  set_dry_run(args)
+
+  topology = load_snapshot(args)
+  print(f"Read transformed lab topology from snapshot file {args.snapshot}")
+
+  mismatch = lab_dir_mismatch(topology)
+
+  probes_OK = True
+  lab_status_change(topology,f'lab shutdown requested{" in conflicting directory" if mismatch else ""}')
+  try:
+    provider_probes(topology,1)
+  except:
+    probes_OK = False
+    if not args.force:
       return
 
+  stop_step = 2
+  if probes_OK:
+    stop_step = stop_all(topology,args,stop_step)
+
   if args.cleanup:
     if 'tools' in topology:
       external_commands.print_step(stop_step,"Cleanup tool configurations",spacing=True)
       stop_step = stop_step + 1
       tool_cleanup(topology,True)
 
     external_commands.print_step(stop_step,"Cleanup configuration files",spacing=True)
```

### Comparing `networklab-1.5.3.post1/netsim/cli/external_commands.py` & `networklab-1.5.4/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/initial.py` & `networklab-1.5.4/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/install.py` & `networklab-1.5.4/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/libvirt.py` & `networklab-1.5.4/netsim/cli/libvirt.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import argparse
 import os
 import string
 import pathlib
 import glob
 import subprocess
 import shutil
+import sys
 
 from box import Box
 
 from .. import common
 from .. import read_topology
 from ..utils import strings,status
 from . import external_commands
@@ -90,14 +91,28 @@
     pass
 
   try:
     result = subprocess.run(['virsh','net-undefine',LIBVIRT_MANAGEMENT_NETWORK_NAME],capture_output=True,text=True)
   except:
     pass
 
+def lp_preinstall_hook(args: argparse.Namespace,settings: Box) -> None:
+  devdata = settings.devices[args.device]
+  if not 'pre_install' in devdata.libvirt:
+    return
+  print("Running pre-install hooks")
+  pre_inst_script = common.get_moddir() / "install/libvirt" / devdata.libvirt.pre_install / "run.sh"
+
+  if not os.access(pre_inst_script, os.X_OK):
+    print(" - run file not executable - skipping.")
+    return
+
+  abort_on_failure(pre_inst_script)
+  print("... done\n")
+
 def lp_create_bootstrap_iso(args: argparse.Namespace,settings: Box) -> None:
   devdata = settings.devices[args.device]
   if not 'create_iso' in devdata.libvirt:
     return
   print("Creating bootstrap ISO image")
 
   isodir = common.get_moddir() / "install/libvirt" / devdata.libvirt.create_iso
@@ -238,14 +253,16 @@
 """)
   if not strings.confirm('Do you want to continue?'):
     print('User decided to abort the box building process')
     return
 
   vm_cleanup('vm_box')
   start_vagrant_network()
+  if not 'preinstall' in skip:
+    lp_preinstall_hook(args,settings)
   if not 'disk' in skip:
     lp_create_vm_disk(args)
   if not 'iso' in skip:
     lp_create_bootstrap_iso(args,settings)
   if not 'vm' in skip:
     lp_create_vm(args,settings)
   stop_vagrant_network()
```

### Comparing `networklab-1.5.3.post1/netsim/cli/read.py` & `networklab-1.5.4/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/restart.py` & `networklab-1.5.4/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/show.py` & `networklab-1.5.4/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/status.py` & `networklab-1.5.4/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/test.py` & `networklab-1.5.4/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/up.py` & `networklab-1.5.4/netsim/cli/up.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/cli/usage.txt` & `networklab-1.5.4/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/common.py` & `networklab-1.5.4/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/data/__init__.py` & `networklab-1.5.4/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/data/filemaps.py` & `networklab-1.5.4/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/data/global_vars.py` & `networklab-1.5.4/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/data/types.py` & `networklab-1.5.4/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/data/validate.py` & `networklab-1.5.4/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/defaults/attributes.yml` & `networklab-1.5.4/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/__init__.py` & `networklab-1.5.4/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/arubacx.py` & `networklab-1.5.4/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/arubacx.yml` & `networklab-1.5.4/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/asav.py` & `networklab-1.5.4/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/asav.yml` & `networklab-1.5.4/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/csr.yml` & `networklab-1.5.4/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/cumulus.yml` & `networklab-1.5.4/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.4/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/dellos10.yml` & `networklab-1.5.4/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/eos.py` & `networklab-1.5.4/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/eos.yml` & `networklab-1.5.4/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/frr.yml` & `networklab-1.5.4/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/iosv.py` & `networklab-1.5.4/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/iosv.yml` & `networklab-1.5.4/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/iosxr.yml` & `networklab-1.5.4/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/junos.py` & `networklab-1.5.4/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/linux.yml` & `networklab-1.5.4/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/none.yml` & `networklab-1.5.4/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/nxos.yml` & `networklab-1.5.4/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/routeros7.yml` & `networklab-1.5.4/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/srlinux.yml` & `networklab-1.5.4/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/sros.yml` & `networklab-1.5.4/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/unknown.py` & `networklab-1.5.4/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/vmx.py` & `networklab-1.5.4/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/vmx.yml` & `networklab-1.5.4/netsim/devices/vmx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/vsrx.py` & `networklab-1.5.4/netsim/devices/vptx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/devices/vsrx.yml` & `networklab-1.5.4/netsim/devices/vsrx.yml`

 * *Files 14% similar despite different names*

```diff
@@ -35,10 +35,19 @@
 libvirt:
   image: juniper/vsrx3
   create_iso: vsrx
   create:
     virt-install --connect=qemu:///system --name=vm_box --os-variant=freebsd10.0 --arch=x86_64 --cpu host --vcpus=2 --hvm
       --ram=4096 --disk path=vm.qcow2,bus=ide,format=qcow2 --disk path=bootstrap.iso,device=cdrom,bus=ide
       --boot hd --network=network:vagrant-libvirt,model=virtio --graphics none --import
+clab:
+  image: vrnetlab/vr-vsrx:23.1R1.8
+  node:
+    kind: vr-vsrx
+  interface:
+    name: eth{ifindex+1}
+  group_vars:
+    ansible_user: admin
+    ansible_ssh_pass: "admin@123"
 external:
   image: none
 graphite.icon: firewall
```

### Comparing `networklab-1.5.3.post1/netsim/devices/vyos.yml` & `networklab-1.5.4/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.4/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.4/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.4/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/multilab/plugin.py` & `networklab-1.5.4/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.4/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.4/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.4/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/ansible.sh` & `networklab-1.5.4/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/containerlab.sh` & `networklab-1.5.4/netsim/install/containerlab.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/bash
 
 # Install a specific version of Containerlab
-CONTAINERLAB_VERSION="0.41.0"
+CONTAINERLAB_VERSION="0.41.2"
 
 cat <<EOM
 Docker/Containerlab Installation Script
 =====================================================================
 This script installs Docker and containerlab on a Debian or Ubuntu
 system. The script was tested on Debian 11.3 and Ubuntu 20.04.
```

### Comparing `networklab-1.5.3.post1/netsim/install/grpc.sh` & `networklab-1.5.4/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/arubacx.txt` & `networklab-1.5.4/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.4/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/csr.txt` & `networklab-1.5.4/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.4/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/eos.txt` & `networklab-1.5.4/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.4/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/iosv.txt` & `networklab-1.5.4/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.4/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.4/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/nxos.txt` & `networklab-1.5.4/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.4/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.4/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.4/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.4/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/install/libvirt.sh` & `networklab-1.5.4/netsim/install/libvirt.sh`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 $SUDO rm /etc/apt/sources.list.d/vagrant.list 2>/dev/null
 set -e
 # add-apt-repository has been deprecated, doesn't work on Debian 11 and will be removed from Ubuntu 22
 # changed to new method - ghostinthenet - 20220417
 curl -fsSL https://apt.releases.hashicorp.com/gpg | $SUDO gpg --dearmor -o /etc/apt/trusted.gpg.d/hashicorp-security.gpg
 $SUDO sh -c 'echo "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main" > /etc/apt/sources.list.d/vagrant.list'
 $SUDO apt-get update
-$SUDO apt-get install -y $FLAG_QUIET ruby-dev ruby-libvirt vagrant
+$SUDO apt-get install -y $FLAG_QUIET ruby-dev ruby-libvirt vagrant=2.3.4
 vagrant plugin install vagrant-libvirt --plugin-version=0.11.2
 echo ".. vagrant installed"
 echo
 set +e
 G="$(groups $USER|grep libvirt)"
 set -e
 if [[ -z "$G" ]]; then
```

### Comparing `networklab-1.5.3.post1/netsim/install/ubuntu.sh` & `networklab-1.5.4/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/__init__.py` & `networklab-1.5.4/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/_dataplane.py` & `networklab-1.5.4/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/_routing.py` & `networklab-1.5.4/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/bfd.py` & `networklab-1.5.4/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/bfd.yml` & `networklab-1.5.4/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/bgp.py` & `networklab-1.5.4/netsim/modules/bgp.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,16 @@
         continue
 
       if node_as == neighbor_real_as and node_local_as == neighbor_local_as:
         continue                                                      # Routers in the same AS + no local-as trickery => nothing to do here
 
       extra_data = data.get_empty_box()
       extra_data.ifindex = l.ifindex
+      if 'bgp' in ngb_ifdata and isinstance(ngb_ifdata.bgp,Box):      # Copy neighbor BGP interface attributes into neighbor data
+        extra_data = ngb_ifdata.bgp + extra_data                      # ... useful for things like BGP roles
 
       # Figure out whether both neighbors have IPv6 LLA and/or unnumbered IPv4 interfaces
       #
       ipv6_lla = l.get('ipv6',None) is True and ngb_ifdata.get('ipv6',None) is True
       ipv6_num = isinstance(l.get('ipv6',None),str) and isinstance(ngb_ifdata.get('ipv6',None),str)
       rfc8950  = l.get('unnumbered',None) is True and ngb_ifdata.get('unnumbered',None) is True
       ipv4_unnum = l.get('ipv4',None) is True and ngb_ifdata.get('ipv4',None) is True
@@ -241,18 +243,21 @@
         if not features.bgp.rfc8950:
           common.error(
             text=f'{node.name} (device {node.device}) does not support IPv4 RFC 8950-style AF over IPv6 LLA EBGP sessions (interface {l.name})',
             category=common.IncorrectValue,
             module='bgp')
           continue
 
-      for k in ('local_as','replace_global_as'):
+      for k in ('local_as','replace_global_as'):      # Special handling for local-as attributes
+        extra_data.pop(k,None)                        # These attributes are copied from local data, not neighbor data ==> remove neighbor data
+
+        # Get local settings from link or node
         local_as_data = l.get(f'bgp.{k}',None) or node.get(f'bgp.{k}',None)
         if not local_as_data is None:
-          extra_data[k] = local_as_data
+          extra_data[k] = local_as_data               # ... and copy it into neighbor data
 
       session_type = 'localas_ibgp' if neighbor_local_as == node_local_as else 'ebgp'
       if session_type == 'localas_ibgp':
         if not features.bgp.local_as_ibgp:
           common.error(
             text=f'You cannot use BGP local-as to create an IBGP session with {ngb_name} on {node.name} (device {node.device})',
             category=common.IncorrectValue,
```

### Comparing `networklab-1.5.3.post1/netsim/modules/bgp.yml` & `networklab-1.5.4/netsim/modules/bgp.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BGP default settings and attributes
 #
 supported_on: [ cumulus, cumulus_nvue, eos, frr, csr, iosv, nxos, asav, vsrx, vyos, routeros,
-  srlinux, sros, none, dellos10, routeros7, vmx, iosxr, arubacx, none ]
+  srlinux, sros, none, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
 ebgp_role: external
 advertise_roles: [ stub ]
 advertise_loopback: True
 community:
   ibgp: [ standard, extended ]
   ebgp: [ standard ]
 no_propagate: [ ebgp_role, advertise_roles, rr_list, as_list ]
```

### Comparing `networklab-1.5.3.post1/netsim/modules/evpn.py` & `networklab-1.5.4/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/evpn.yml` & `networklab-1.5.4/netsim/modules/evpn.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # EVPN default settings and attributes
 requires: [ bgp ]
-supported_on: [ sros, srlinux, frr, eos, vyos, dellos10, cumulus, nxos, arubacx, none ]
+supported_on: [ sros, srlinux, frr, eos, vyos, dellos10, cumulus, nxos, arubacx, vptx, none ]
 no_propagate: [ start_transit_vni, transport, vlan_bundle_service, as ]
 transform_after: [ vlan, vxlan, vrf ]
 config_after: [ vlan, vxlan, vrf ]
 session: [ ibgp ]
 start_transit_vni: 200000
 attributes:
   global:
```

### Comparing `networklab-1.5.3.post1/netsim/modules/gateway.py` & `networklab-1.5.4/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/gateway.yml` & `networklab-1.5.4/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/isis.py` & `networklab-1.5.4/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/isis.yml` & `networklab-1.5.4/netsim/modules/isis.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ISIS default settings and attributes
 #
-supported_on: [ eos, frr, csr, iosv, nxos, asav, vsrx, srlinux, sros, vyos, vmx, iosxr, none ]
+supported_on: [ eos, frr, csr, iosv, nxos, asav, vsrx, srlinux, sros, vyos, vmx, iosxr, vptx, none ]
 area: "49.0001"
 type: level-2
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
```

### Comparing `networklab-1.5.3.post1/netsim/modules/mpls.py` & `networklab-1.5.4/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/mpls.yml` & `networklab-1.5.4/netsim/modules/mpls.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MPLS (LDP, BGP LU, L3VPN, 6PE) default settings and attributes
 #
-supported_on: [ eos, iosv, csr, routeros, vyos, routeros7, sros, vmx, vsrx, frr, none, arubacx ]
+supported_on: [ eos, iosv, csr, routeros, vyos, routeros7, sros, vmx, vsrx, frr, none, vptx, arubacx ]
 config_after: [ vlan, ospf, isis, bgp ]
 transform_after: [ vlan, bgp ]
 ldp: True
 attributes:
   global:
     ldp:
       _alt_types: [ bool ]
```

### Comparing `networklab-1.5.3.post1/netsim/modules/ospf.py` & `networklab-1.5.4/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/ospf.yml` & `networklab-1.5.4/netsim/modules/ospf.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OSPFv2/OSPFv3 default settings and attributes
 #
 area: 0.0.0.0
 supported_on: [
   arcos, cumulus, cumulus_nvue, eos, fortios, frr, csr, iosv, nxos, vsrx, vyos, routeros,
-  srlinux, sros, dellos10, routeros7, vmx, iosxr, arubacx, none ]
+  srlinux, sros, dellos10, routeros7, vmx, iosxr, arubacx, vptx, none ]
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
       _list_to_dict: True
       _alt_types: [ NoneType ]
```

### Comparing `networklab-1.5.3.post1/netsim/modules/srv6.py` & `networklab-1.5.4/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/vlan.py` & `networklab-1.5.4/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/vlan.yml` & `networklab-1.5.4/netsim/modules/vlan.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # VLAN default settings and attributes
 #
-supported_on: [ eos, iosv, csr, vyos, dellos10, srlinux, none, routeros, nxos, frr, cumulus, sros, routeros7, vmx, vsrx, arubacx, none ]
+supported_on: [ eos, iosv, csr, vyos, dellos10, srlinux, none, routeros, nxos, frr, cumulus, sros, routeros7, vmx, vsrx, arubacx, vptx, none ]
 no_propagate: [ start_vlan_id, mode ]
 start_vlan_id: 1000
 mode: irb
 attributes:
   global:
     mode: { type: str, valid_values: [ bridge, irb, route] }
   node:
```

### Comparing `networklab-1.5.3.post1/netsim/modules/vrf.py` & `networklab-1.5.4/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/vxlan.py` & `networklab-1.5.4/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/modules/vxlan.yml` & `networklab-1.5.4/netsim/modules/vxlan.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # VXLAN default settings and attributes
 #
-supported_on: [ eos, nxos, vyos, csr, dellos10, srlinux, frr, cumulus, sros, arubacx, none ]
+supported_on: [ eos, nxos, vyos, csr, dellos10, srlinux, frr, cumulus, sros, arubacx, vptx, none ]
 requires: [ vlan ]
 config_after: [ vrf ] # For platforms that suppport L3 VXLAN, vrfs must be created first
 transform_after: [ vlan, vrf ]
 domain: global
 flooding: static
 start_vni: 100000
 attributes:
```

### Comparing `networklab-1.5.3.post1/netsim/outputs/__init__.py` & `networklab-1.5.4/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/ansible.py` & `networklab-1.5.4/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/common.py` & `networklab-1.5.4/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/d2.py` & `networklab-1.5.4/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/d2.yml` & `networklab-1.5.4/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/devices.py` & `networklab-1.5.4/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/format.py` & `networklab-1.5.4/netsim/outputs/format.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/graph.py` & `networklab-1.5.4/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/graphite.py` & `networklab-1.5.4/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/provider.py` & `networklab-1.5.4/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/tools.py` & `networklab-1.5.4/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/outputs/yaml.py` & `networklab-1.5.4/netsim/outputs/yaml.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,27 +31,28 @@
     output = common.open_output_file(outfile)
 
     for fmt in self.format:
       if fmt == 'nodefault':
         cleantopo.pop('defaults')
       elif fmt == 'noaddr':
         cleantopo.pop('addressing')
-      elif cleantopo.get(fmt,None):
-        result = cleantopo.get(fmt)
-        if not isinstance(result,Box) and not isinstance(result,BoxList):
-          common.fatal(f'Selecting {fmt} did not result in a usable dictionary, aborting')
+      else:
+        try:
+          result = eval(fmt,cleantopo)
+        except Exception as ex:
+          common.fatal(f'Error trying to evaluate {fmt}: {str(ex)}')
           return
         cleantopo = result
         break
-      else:
-        common.error('Invalid format modifier %s' % fmt,common.IncorrectValue,modname)
 
-    common.exit_on_error()
-    if modname == 'YAML':
+    if not isinstance(cleantopo,Box) and not isinstance(cleantopo,BoxList):
+      output.write(f"{str(result)}\n")
+    elif modname == 'YAML':
       output.write(common.get_yaml_string(cleantopo))
     else:
       output.write(cleantopo.to_json(indent=2,sort_keys=True))
+
     if outfile != '-':
       common.close_output_file(output)
-      print("Created transformed topology dump in YAML format in %s" % outfile)
+      print(f"Created transformed topology dump in {modname} format in {outfile}")
     else:
       output.write("\n")
```

### Comparing `networklab-1.5.3.post1/netsim/providers/__init__.py` & `networklab-1.5.4/netsim/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/providers/clab.py` & `networklab-1.5.4/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/providers/clab.yml` & `networklab-1.5.4/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/providers/external.py` & `networklab-1.5.4/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/providers/libvirt.py` & `networklab-1.5.4/netsim/providers/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/providers/libvirt.yml` & `networklab-1.5.4/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/read_topology.py` & `networklab-1.5.4/netsim/read_topology.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,14 +174,28 @@
           include_defaults(topology,user_defaults)
 
   if sys_defaults and 'global_defaults' in topology.includes:
     include_defaults(topology,sys_defaults)
 
   return topology
 
+#
+# Parse values specified in CLI settings. Return string, bool or int
+#
+def transform_cli_value(v: str) -> typing.Union[int,bool,str]:
+  try:                                            # Try to parse an integer
+    return int(v)
+  except:
+    pass
+
+  if v.lower() in ['true','false']:               # Recognize True or False
+    return v.lower() == 'true'                    # ... and return the result of "do we have true?"
+  
+  return v                                        # Otherwise it's a string
+
 def add_cli_args(topo: Box, args: typing.Union[argparse.Namespace,Box]) -> None:
   if args.device:
     topo.defaults.device = args.device
 
   if args.provider:
     topo.provider = args.provider
 
@@ -193,14 +207,15 @@
     topo.plugin.extend(args.plugin)
 
   if args.settings:
     for s in args.settings:
       if not "=" in s:
         common.error("Invalid CLI setting %s, should be in format key=value" % s)
       (k,v) = s.split("=")
+      v = transform_cli_value(v)
       try:
         topo[k] = v
       except TypeError as ex:
         if 'nodes.' in k:
           common.error(
             f'Cannot set {k}:\n... nodes element must be a dictionary if you want to set values via CLI arguments',
             common.IncorrectValue,
```

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.4/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.4/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.4/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/external/external.j2` & `networklab-1.5.4/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.4/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.4/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.4/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/tools/__init__.py` & `networklab-1.5.4/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/tools/graphite.py` & `networklab-1.5.4/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/tools/graphite.yml` & `networklab-1.5.4/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/tools/suzieq.yml` & `networklab-1.5.4/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/topology-defaults.yml` & `networklab-1.5.4/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/utils/log.py` & `networklab-1.5.4/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/utils/status.py` & `networklab-1.5.4/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/utils/strings.py` & `networklab-1.5.4/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/netsim/utils/templates.py` & `networklab-1.5.4/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/networklab.egg-info/PKG-INFO` & `networklab-1.5.4/networklab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.3.post1
+Version: 1.5.4
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.5.3](https://github.com/ipspace/netlab/releases/tag/release_1.5.3), which is the only release that works with the latest *containerlab* release (0.41.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
+The latest release is [release 1.5.4](https://github.com/ipspace/netlab/releases/tag/release_1.5.4). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netlab.tools/release/) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netlab.tools/netlab/up/)
```

### Comparing `networklab-1.5.3.post1/networklab.egg-info/SOURCES.txt` & `networklab-1.5.4/networklab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 netsim/ansible/tasks/frr/mpls-clab.yml
 netsim/ansible/tasks/iosxr/initial.yml
 netsim/ansible/tasks/linux/initial-clab.yml
 netsim/ansible/tasks/nxos/initial.yml
 netsim/ansible/tasks/readiness-check/dellos10.yml
 netsim/ansible/tasks/readiness-check/eos-clab.yml
 netsim/ansible/tasks/readiness-check/routeros7.yml
+netsim/ansible/tasks/readiness-check/vsrx.yml
 netsim/ansible/tasks/vmx/initial.yml
 netsim/ansible/templates/missing.j2
 netsim/ansible/templates/bfd/arubacx.j2
 netsim/ansible/templates/bfd/eos.j2
 netsim/ansible/templates/bfd/ios.j2
 netsim/ansible/templates/bfd/none.j2
 netsim/ansible/templates/bfd/nxos.j2
@@ -269,14 +270,15 @@
 netsim/ansible/templates/vlan/ios.j2
 netsim/ansible/templates/vlan/nxos.j2
 netsim/ansible/templates/vlan/routeros.j2
 netsim/ansible/templates/vlan/routeros7.j2
 netsim/ansible/templates/vlan/srlinux.j2
 netsim/ansible/templates/vlan/sros.j2
 netsim/ansible/templates/vlan/vmx.j2
+netsim/ansible/templates/vlan/vptx.j2
 netsim/ansible/templates/vlan/vsrx.j2
 netsim/ansible/templates/vlan/vyos.j2
 netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
 netsim/ansible/templates/vrf/arubacx.bgp.j2
 netsim/ansible/templates/vrf/arubacx.j2
 netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/cumulus.j2
@@ -396,39 +398,33 @@
 netsim/devices/routeros7.yml
 netsim/devices/srlinux.yml
 netsim/devices/sros.yml
 netsim/devices/unknown.py
 netsim/devices/unknown.yml
 netsim/devices/vmx.py
 netsim/devices/vmx.yml
+netsim/devices/vptx.py
+netsim/devices/vptx.yml
 netsim/devices/vsrx.py
 netsim/devices/vsrx.yml
 netsim/devices/vyos.yml
-netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
 netsim/extra/ebgp.utils/default-originate.yml
 netsim/extra/ebgp.utils/eos.j2
 netsim/extra/ebgp.utils/ios.j2
 netsim/extra/ebgp.utils/junos.j2
 netsim/extra/ebgp.utils/plugin.py
 netsim/extra/ebgp.utils/routeros7.j2
 netsim/extra/ebgp.utils/srlinux.j2
 netsim/extra/ebgp.utils/topology.yml
 netsim/extra/ebgp.utils/vyos.j2
-netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
-netsim/extra/ebgp.utils/__pycache__/plugin.cpython-311.pyc
 netsim/extra/multilab/plugin.py
-netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
-netsim/extra/multilab/__pycache__/plugin.cpython-311.pyc
 netsim/extra/none/none.j2
 netsim/extra/proxy-arp/plugin.py
 netsim/extra/proxy-arp/srlinux.j2
 netsim/extra/proxy-arp/sros.j2
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-311.pyc
-netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
 netsim/install/libvirt/arubacx.txt
 netsim/install/libvirt/asav.txt
@@ -438,17 +434,21 @@
 netsim/install/libvirt/eos.xml.j2
 netsim/install/libvirt/iosv.txt
 netsim/install/libvirt/iosv.xml.j2
 netsim/install/libvirt/iosxr.txt
 netsim/install/libvirt/nxos.txt
 netsim/install/libvirt/nxos.xml.j2
 netsim/install/libvirt/routeros7.txt
+netsim/install/libvirt/vptx.txt
+netsim/install/libvirt/vptx.xml.j2
 netsim/install/libvirt/vsrx.txt
 netsim/install/libvirt/asav/day0-config
-netsim/install/libvirt/iosxr/iosxr_config.txt
+netsim/install/libvirt/vptx/juniper.conf
+netsim/install/libvirt/vptx/make-config.sh
+netsim/install/libvirt/vptx/run.sh
 netsim/install/libvirt/vsrx/juniper.conf
 netsim/modules/__init__.py
 netsim/modules/_dataplane.py
 netsim/modules/_routing.py
 netsim/modules/bfd.py
 netsim/modules/bfd.yml
 netsim/modules/bgp.py
@@ -521,14 +521,15 @@
 netsim/templates/provider/libvirt/libvirt-tunnel.j2
 netsim/templates/provider/libvirt/linux-domain.j2
 netsim/templates/provider/libvirt/none-domain.j2
 netsim/templates/provider/libvirt/nxos-domain.j2
 netsim/templates/provider/libvirt/routeros-domain.j2
 netsim/templates/provider/libvirt/routeros7-domain.j2
 netsim/templates/provider/libvirt/vagrant-libvirt.xml
+netsim/templates/provider/libvirt/vptx-domain.j2
 netsim/templates/provider/libvirt/vsrx-domain.j2
 netsim/templates/provider/libvirt/vyos-domain.j2
 netsim/templates/provider/virtualbox/Vagrantfile.j2
 netsim/templates/provider/virtualbox/arcos-domain.j2
 netsim/templates/provider/virtualbox/cumulus-domain.j2
 netsim/templates/provider/virtualbox/eos-domain.j2
 netsim/templates/provider/virtualbox/linux-domain.j2
```

### Comparing `networklab-1.5.3.post1/setup.py` & `networklab-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.3.post1/tests/test_transformation.py` & `networklab-1.5.4/tests/test_transformation.py`

 * *Files identical despite different names*

