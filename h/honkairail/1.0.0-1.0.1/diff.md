# Comparing `tmp/honkairail-1.0.0.tar.gz` & `tmp/honkairail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honkairail-1.0.0.tar", max compression
+gzip compressed data, was "honkairail-1.0.1.tar", max compression
```

## Comparing `honkairail-1.0.0.tar` & `honkairail-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.0/honkairail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.0/honkairail/src/__init__.py
--rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.0/honkairail/src/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.0/honkairail/src/tools/__init__.py
--rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.0/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2760 2023-06-05 09:50:17.932351 honkairail-1.0.0/honkairail/src/tools/__pycache__/api.cpython-310.pyc
--rw-r--r--   0        0        0     6099 2023-06-05 09:48:10.659728 honkairail-1.0.0/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
--rw-r--r--   0        0        0     1045 2023-06-05 09:07:33.076315 honkairail-1.0.0/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
--rw-r--r--   0        0        0     2636 2023-06-05 09:50:07.425805 honkairail-1.0.0/honkairail/src/tools/api.py
--rw-r--r--   0        0        0     5115 2023-06-05 09:47:42.507367 honkairail-1.0.0/honkairail/src/tools/modal.py
--rw-r--r--   0        0        0      882 2023-06-05 08:56:51.817431 honkairail-1.0.0/honkairail/src/tools/utilities.py
--rw-r--r--   0        0        0      922 2023-06-05 09:50:08.978569 honkairail-1.0.0/honkairail/starrailapi.py
--rw-r--r--   0        0        0      489 2023-06-05 10:15:23.598467 honkairail-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3794 2023-06-05 10:18:04.453310 honkairail-1.0.0/README.md
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 honkairail-1.0.0/setup.py
--rw-r--r--   0        0        0     4342 1970-01-01 00:00:00.000000 honkairail-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 03:59:10.580471 honkairail-1.0.1/honkairail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:03:31.753289 honkairail-1.0.1/honkairail/src/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-05 09:07:32.687441 honkairail-1.0.1/honkairail/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-06-05 03:58:24.588036 honkairail-1.0.1/honkairail/src/tools/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-05 09:07:32.690434 honkairail-1.0.1/honkairail/src/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2867 2023-06-09 11:04:04.021741 honkairail-1.0.1/honkairail/src/tools/__pycache__/api.cpython-310.pyc
+-rw-r--r--   0        0        0    12087 2023-06-09 11:33:55.802274 honkairail-1.0.1/honkairail/src/tools/__pycache__/modal.cpython-310.pyc
+-rw-r--r--   0        0        0     1310 2023-06-09 11:18:15.642417 honkairail-1.0.1/honkairail/src/tools/__pycache__/utilities.cpython-310.pyc
+-rw-r--r--   0        0        0     2950 2023-06-09 11:04:00.928622 honkairail-1.0.1/honkairail/src/tools/api.py
+-rw-r--r--   0        0        0    11426 2023-06-09 11:33:52.556840 honkairail-1.0.1/honkairail/src/tools/modal.py
+-rw-r--r--   0        0        0     1127 2023-06-09 11:14:40.320720 honkairail-1.0.1/honkairail/src/tools/utilities.py
+-rw-r--r--   0        0        0     1010 2023-06-09 11:33:04.349430 honkairail-1.0.1/honkairail/starrailapi.py
+-rw-r--r--   0        0        0      489 2023-06-10 09:39:23.432897 honkairail-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3892 2023-06-10 09:41:05.266404 honkairail-1.0.1/README.md
+-rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 honkairail-1.0.1/setup.py
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 honkairail-1.0.1/PKG-INFO
```

### Comparing `honkairail-1.0.0/honkairail/src/tools/__pycache__/api.cpython-310.pyc` & `honkairail-1.0.1/honkairail/src/tools/__pycache__/api.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun  5 09:50:07 2023 UTC, .py size: 2636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,180 @@
-00000000: 6f0d 0d0a 0000 0000 cfaf 7d64 4c0a 0000  o.........}dL...
+00000000: 6f0d 0d0a 0000 0000 2007 8364 860b 0000  o....... ..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000e 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 0100 6402 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6406 6407 6408 6409 640a 640b  ..d.d.d.d.d.d.d.
-00000070: 640c 640d 640e 640f 6410 6411 6412 9c0d  d.d.d.d.d.d.d...
-00000080: 5a08 6413 5a09 6414 5a0a 6415 5a0b 6416  Z.d.Z.d.Z.d.Z.d.
-00000090: 6417 8400 5a0c 6418 6419 8400 5a0d 641a  d...Z.d.d...Z.d.
-000000a0: 641b 8400 5a0e 641c 641d 8400 5a0f 641e  d...Z.d.d...Z.d.
-000000b0: 641f 8400 5a10 6420 6421 8400 5a11 6422  d...Z.d d!..Z.d"
-000000c0: 6423 8400 5a12 6401 5300 2924 e900 0000  d#..Z.d.S.)$....
-000000d0: 004e e901 0000 0029 02da 0f53 7461 7252  .N.....)...StarR
+00000050: 6d05 5a05 6d06 5a06 0100 6402 6404 6c07  m.Z.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6405 6406 6407 6408 6409  m.Z...d.d.d.d.d.
+00000070: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
+00000080: 6412 9c0d 5a09 6413 5a0a 6414 5a0b 6415  d...Z.d.Z.d.Z.d.
+00000090: 5a0c 6416 5a0d 6417 6418 8400 5a0e 6419  Z.d.Z.d.d...Z.d.
+000000a0: 641a 8400 5a0f 641b 641c 8400 5a10 641d  d...Z.d.d...Z.d.
+000000b0: 641e 8400 5a11 641f 6420 8400 5a12 6421  d...Z.d.d ..Z.d!
+000000c0: 6422 8400 5a13 6401 5300 2923 e900 0000  d"..Z.d.S.)#....
+000000d0: 004e e901 0000 0029 03da 0f53 7461 7252  .N.....)...StarR
 000000e0: 6169 6c41 7069 4461 7461 da0a 506c 6179  ailApiData..Play
-000000f0: 6572 496e 666f 2901 da09 7574 696c 6974  erInfo)...utilit
-00000100: 6965 73da 0363 6874 da02 636e da02 6465  ies..cht..cn..de
-00000110: da02 656e da02 6573 da02 6672 da02 6964  ..en..es..fr..id
-00000120: da02 6a70 da02 6b72 da02 7074 da02 7275  ..jp..kr..pt..ru
-00000130: da02 7468 da02 7669 290d 7206 0000 0072  ..th..vi).r....r
-00000140: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
-00000150: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000160: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000170: 0072 1100 0000 7212 0000 007a 3668 7474  .r....r....z6htt
-00000180: 7073 3a2f 2f61 7069 2e6d 6968 6f6d 6f2e  ps://api.mihomo.
-00000190: 6d65 2f73 725f 696e 666f 5f70 6172 7365  me/sr_info_parse
-000001a0: 642f 7b75 6964 7d3f 6c61 6e67 3d7b 6c61  d/{uid}?lang={la
-000001b0: 6e67 7d7a 2f68 7474 7073 3a2f 2f61 7069  ng}z/https://api
-000001c0: 2e6d 6968 6f6d 6f2e 6d65 2f73 725f 696e  .mihomo.me/sr_in
-000001d0: 666f 2f7b 7569 647d 3f6c 616e 673d 7b6c  fo/{uid}?lang={l
-000001e0: 616e 677d 7a81 6874 7470 733a 2f2f 6d61  ang}z.https://ma
-000001f0: 6e61 2e77 696b 692f 7374 6172 7261 696c  na.wiki/starrail
-00000200: 2f63 6f6c 6c65 6374 696f 6e73 2f6c 6967  /collections/lig
-00000210: 6874 436f 6e65 732f 7b69 647d 3f5f 6461  htCones/{id}?_da
-00000220: 7461 3d5f 6375 7374 6f6d 2532 4672 6f75  ta=_custom%2Frou
-00000230: 7465 7325 3246 2532 3473 6974 6549 642e  tes%2F%24siteId.
-00000240: 636f 6c6c 6563 7469 6f6e 7325 3242 2532  collections%2B%2
-00000250: 466c 6967 6874 436f 6e65 735f 2e25 3234  FlightCones_.%24
-00000260: 656e 7472 7949 6463 0100 0000 0000 0000  entryIdc........
-00000270: 0000 0000 0400 0000 0a00 0000 c300 0000  ................
-00000280: 73bc 0000 0081 0174 00a0 01a1 0034 0049  s......t.....4.I
-00000290: 0064 0048 009a 487d 017c 01a0 027c 00a1  .d.H..H}.|...|..
-000002a0: 0134 0049 0064 0048 009a 287d 027c 02a0  .4.I.d.H..(}.|..
-000002b0: 03a1 0049 0064 0048 007d 0364 017c 0376  ...I.d.H.}.d.|.v
-000002c0: 0072 2574 047c 0364 0119 0083 0182 017c  .r%t.|.d.......|
-000002d0: 0357 0002 0064 0004 0004 0083 0349 0064  .W...d.......I.d
-000002e0: 0048 0001 0057 0002 0064 0004 0004 0083  .H...W...d......
-000002f0: 0349 0064 0048 0001 0053 0031 0049 0064  .I.d.H...S.1.I.d
-00000300: 0048 0073 4177 0101 0001 0001 0059 0001  .H.sAw.......Y..
-00000310: 0057 0064 0004 0004 0083 0349 0064 0048  .W.d.......I.d.H
-00000320: 0001 0064 0053 0031 0049 0064 0048 0073  ...d.S.1.I.d.H.s
-00000330: 5777 0101 0001 0001 0059 0001 0064 0053  Ww.......Y...d.S
-00000340: 0029 024e 5a06 6465 7461 696c 2905 da07  .).NZ.detail)...
-00000350: 6169 6f68 7474 705a 0d43 6c69 656e 7453  aiohttpZ.ClientS
-00000360: 6573 7369 6f6e da03 6765 74da 046a 736f  ession..get..jso
-00000370: 6eda 0954 7970 6545 7272 6f72 2904 da03  n..TypeError)...
-00000380: 7572 6cda 0773 6573 7369 6f6e da08 7265  url..session..re
-00000390: 7370 6f6e 7365 da04 6461 7461 a900 721b  sponse..data..r.
-000003a0: 0000 00fa 3743 3a5c 5573 6572 735c 4461  ....7C:\Users\Da
-000003b0: 7273 6f58 5c44 6573 6b74 6f70 5c72 6573  rsoX\Desktop\res
-000003c0: 5c68 6f6e 6b61 6972 6169 6c5c 7372 635c  \honkairail\src\
-000003d0: 746f 6f6c 735c 6170 692e 7079 da0a 6665  tools\api.py..fe
-000003e0: 7463 685f 6461 7461 1b00 0000 7316 0000  tch_data....s...
-000003f0: 0002 8012 0114 010e 0108 010c 0102 0114  ................
-00000400: fc16 ff18 012e ff72 1d00 0000 6302 0000  .......r....c...
-00000410: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000420: 00c3 0000 00f3 2e00 0000 8101 7400 a001  ............t...
-00000430: 7c01 a002 a100 6401 a102 7d01 7403 6a04  |.....d...}.t.j.
-00000440: 7c00 7c01 6402 8d02 7d02 7405 7c02 8301  |.|.d...}.t.|...
-00000450: 4900 6400 4800 5300 a903 4e72 0900 0000  I.d.H.S...Nr....
-00000460: 2902 da03 7569 64da 046c 616e 6729 06da  )...uid..lang)..
-00000470: 1353 5550 504f 5254 4544 5f4c 414e 4755  .SUPPORTED_LANGU
-00000480: 4147 4553 7214 0000 00da 056c 6f77 6572  AGESr......lower
-00000490: da08 4150 495f 4c49 4e4b da06 666f 726d  ..API_LINK..form
-000004a0: 6174 721d 0000 00a9 0372 2000 0000 7221  atr......r ...r!
-000004b0: 0000 0072 1700 0000 721b 0000 0072 1b00  ...r....r....r..
-000004c0: 0000 721c 0000 00da 0d67 6574 5f75 7365  ..r......get_use
-000004d0: 725f 6461 7461 2300 0000 f308 0000 0002  r_data#.........
-000004e0: 8010 010e 010e 0172 2700 0000 6302 0000  .......r'...c...
-000004f0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000500: 00c3 0000 0072 1e00 0000 721f 0000 0029  .....r....r....)
-00000510: 0672 2200 0000 7214 0000 0072 2300 0000  .r"...r....r#...
-00000520: da0d 4655 4c4c 5f41 5049 5f4c 494e 4b72  ..FULL_API_LINKr
-00000530: 2500 0000 721d 0000 0072 2600 0000 721b  %...r....r&...r.
-00000540: 0000 0072 1b00 0000 721c 0000 00da 1267  ...r....r......g
-00000550: 6574 5f66 756c 6c5f 7573 6572 5f64 6174  et_full_user_dat
-00000560: 6128 0000 0072 2800 0000 722a 0000 0063  a(...r(...r*...c
-00000570: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000580: 0300 0000 c300 0000 731c 0000 0081 0174  ........s......t
-00000590: 006a 017c 0064 018d 017d 0174 027c 0183  .j.|.d...}.t.|..
-000005a0: 0149 0064 0048 0053 0029 024e 2901 720c  .I.d.H.S.).N).r.
-000005b0: 0000 0029 03da 104c 4947 4854 5f43 4f4e  ...)...LIGHT_CON
-000005c0: 4553 5f4c 494e 4b72 2500 0000 721d 0000  ES_LINKr%...r...
-000005d0: 0029 0272 0c00 0000 7217 0000 0072 1b00  .).r....r....r..
-000005e0: 0000 721b 0000 0072 1c00 0000 da14 6765  ..r....r......ge
-000005f0: 745f 6c69 6768 745f 636f 6e65 735f 6461  t_light_cones_da
-00000600: 7461 2d00 0000 7306 0000 0002 800c 010e  ta-...s.........
-00000610: 0172 2c00 0000 6302 0000 0000 0000 0000  .r,...c.........
-00000620: 0000 0003 0000 0004 0000 00c3 0000 0073  ...............s
-00000630: 2600 0000 8101 7400 7c01 7c00 8302 4900  &.....t.|.|...I.
-00000640: 6400 4800 7d02 7401 7c02 6401 1900 7c02  d.H.}.t.|.d...|.
-00000650: 6402 1900 6403 8d02 5300 2904 4eda 0670  d...d...S.).N..p
-00000660: 6c61 7965 72da 0a63 6861 7261 6374 6572  layer..character
-00000670: 73a9 0272 2d00 0000 722e 0000 0029 0272  s..r-...r....).r
-00000680: 2700 0000 7203 0000 0029 0372 2100 0000  '...r....).r!...
-00000690: 7220 0000 0072 1a00 0000 721b 0000 0072  r ...r....r....r
-000006a0: 1b00 0000 721c 0000 00da 0867 6574 5f64  ....r......get_d
-000006b0: 6174 6131 0000 0073 0600 0000 0280 1001  ata1...s........
-000006c0: 1401 7230 0000 0063 0200 0000 0000 0000  ..r0...c........
-000006d0: 0000 0000 0400 0000 0400 0000 c300 0000  ................
-000006e0: 7326 0000 0081 0174 007c 017c 0083 0249  s&.....t.|.|...I
-000006f0: 0064 0048 007d 0274 0164 0169 007c 02a4  .d.H.}.t.d.i.|..
-00000700: 018e 017d 037c 036a 0253 0029 024e 721b  ...}.|.j.S.).Nr.
-00000710: 0000 0029 0372 2a00 0000 7204 0000 005a  ...).r*...r....Z
-00000720: 1050 6c61 7965 7244 6574 6169 6c49 6e66  .PlayerDetailInf
-00000730: 6f29 0472 2100 0000 7220 0000 0072 1a00  o).r!...r ...r..
-00000740: 0000 da0b 706c 6179 6572 5f69 6e66 6f72  ....player_infor
-00000750: 1b00 0000 721b 0000 0072 1c00 0000 da0b  ....r....r......
-00000760: 6765 745f 7072 6f66 696c 6535 0000 0073  get_profile5...s
-00000770: 0800 0000 0280 1001 0e01 0601 7232 0000  ............r2..
-00000780: 0063 0200 0000 0000 0000 0000 0000 0600  .c..............
-00000790: 0000 0600 0000 c300 0000 73e6 0000 0081  ..........s.....
-000007a0: 0174 00a0 0174 027c 007c 0183 0274 037c  .t...t.|.|...t.|
-000007b0: 017c 0083 02a1 0249 0064 0048 005c 027d  .|.....I.d.H.\.}
-000007c0: 027d 0374 04a0 057c 02a0 04a1 00a1 017d  .}.t...|.......}
-000007d0: 027c 0364 0119 0044 005d 0c7d 047c 0464  .|.d...D.].}.|.d
-000007e0: 0219 0069 006b 0272 2964 007c 0464 023c  ...i.k.r)d.|.d.<
-000007f0: 0071 1d7c 0264 0319 007d 057c 0264 0419  .q.|.d...}.|.d..
-00000800: 007c 0364 0519 0064 063c 007c 0264 0719  .|.d...d.<.|.d..
-00000810: 007c 0364 0519 0064 083c 0074 06a0 077c  .|.d...d.<.t...|
-00000820: 0264 0919 00a1 017c 0364 0519 0064 0a3c  .d.....|.d...d.<
-00000830: 007c 0564 0b19 007c 0364 0519 0064 0c3c  .|.d...|.d...d.<
-00000840: 007c 0564 0d19 007c 0364 0519 0064 023c  .|.d...|.d...d.<
-00000850: 007c 0564 0e19 007c 0364 0519 0064 013c  .|.d...|.d...d.<
-00000860: 007c 0564 0f19 007c 0364 0519 0064 103c  .|.d...|.d...d.<
-00000870: 0074 087c 0364 0519 007c 0364 0119 0064  .t.|.d...|.d...d
-00000880: 118d 0253 0029 124e 722e 0000 00da 0a6c  ...S.).Nr......l
-00000890: 6967 6874 5f63 6f6e 655a 0f50 6c61 7965  ight_coneZ.Playe
-000008a0: 7253 7061 6365 496e 666f 5a0e 4375 7246  rSpaceInfoZ.CurF
-000008b0: 7269 656e 6443 6f75 6e74 722d 0000 00da  riendCountr-....
-000008c0: 0766 7269 656e 6473 5a0a 576f 726c 644c  .friendsZ.WorldL
-000008d0: 6576 656c da0a 776f 726c 646c 6576 656c  evel..worldlevel
-000008e0: 5a08 4269 7274 6864 6179 da08 6269 7274  Z.Birthday..birt
-000008f0: 6864 6179 5a10 5061 7373 4172 6561 5072  hdayZ.PassAreaPr
-00000900: 6f67 7265 7373 da12 7061 7373 5f61 7265  ogress..pass_are
-00000910: 615f 7072 6f67 7265 7373 5a0e 4c69 6768  a_progressZ.Ligh
-00000920: 7443 6f6e 6543 6f75 6e74 5a0b 4176 6174  tConeCountZ.Avat
-00000930: 6172 436f 756e 745a 1041 6368 6965 7665  arCountZ.Achieve
-00000940: 6d65 6e74 436f 756e 74da 0b61 6368 6965  mentCount..achie
-00000950: 7665 6d65 6e74 722f 0000 0029 09da 0761  vementr/...)...a
-00000960: 7379 6e63 696f 5a06 6761 7468 6572 7232  syncioZ.gatherr2
-00000970: 0000 0072 2700 0000 7215 0000 00da 056c  ...r'...r......l
-00000980: 6f61 6473 7205 0000 005a 0c63 6f6e 7665  oadsr....Z.conve
-00000990: 7274 5f64 6174 6572 0300 0000 2906 7221  rt_dater....).r!
-000009a0: 0000 0072 2000 0000 5a07 7072 6f66 696c  ...r ...Z.profil
-000009b0: 6572 1a00 0000 da03 6b65 7972 3100 0000  er......keyr1...
-000009c0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-000009d0: 0867 6574 5f66 756c 6c3a 0000 0073 2000  .get_full:...s .
-000009e0: 0000 0280 2201 0e01 0c02 0c01 0801 0280  ...."...........
-000009f0: 0802 1001 1001 1601 1001 1001 1001 1001  ................
-00000a00: 1402 723c 0000 0029 1372 1300 0000 7239  ..r<...).r....r9
-00000a10: 0000 0072 1500 0000 da05 6d6f 6461 6c72  ...r......modalr
-00000a20: 0300 0000 7204 0000 00da 0072 0500 0000  ....r......r....
-00000a30: 7222 0000 0072 2400 0000 7229 0000 0072  r"...r$...r)...r
-00000a40: 2b00 0000 721d 0000 0072 2700 0000 722a  +...r....r'...r*
-00000a50: 0000 0072 2c00 0000 7230 0000 0072 3200  ...r,...r0...r2.
-00000a60: 0000 723c 0000 0072 1b00 0000 721b 0000  ..r<...r....r...
-00000a70: 0072 1b00 0000 721c 0000 00da 083c 6d6f  .r....r......<mo
-00000a80: 6475 6c65 3e01 0000 0073 3a00 0000 0800  dule>....s:.....
-00000a90: 0801 0801 1001 0c01 0203 0201 0201 0201  ................
-00000aa0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000ab0: 0201 06f3 0410 0401 0401 0802 0808 0805  ................
-00000ac0: 0805 0804 0804 0c05                      ........
+000000f0: 6572 496e 666f da11 5374 6172 5261 696c  erInfo..StarRail
+00000100: 4170 6944 6174 6156 3229 01da 0975 7469  ApiDataV2)...uti
+00000110: 6c69 7469 6573 da03 6368 74da 0263 6eda  lities..cht..cn.
+00000120: 0264 65da 0265 6eda 0265 73da 0266 72da  .de..en..es..fr.
+00000130: 0269 64da 026a 70da 026b 72da 0270 74da  .id..jp..kr..pt.
+00000140: 0272 75da 0274 68da 0276 6929 0d72 0700  .ru..th..vi).r..
+00000150: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000160: 0072 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000170: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00000180: 1100 0000 7212 0000 0072 1300 0000 7a41  ....r....r....zA
+00000190: 6874 7470 733a 2f2f 6170 692e 6d69 686f  https://api.miho
+000001a0: 6d6f 2e6d 652f 7372 5f69 6e66 6f5f 7061  mo.me/sr_info_pa
+000001b0: 7273 6564 2f7b 7569 647d 3f6c 616e 673d  rsed/{uid}?lang=
+000001c0: 7b6c 616e 677d 2676 6572 7369 6f6e 3d76  {lang}&version=v
+000001d0: 317a 3668 7474 7073 3a2f 2f61 7069 2e6d  1z6https://api.m
+000001e0: 6968 6f6d 6f2e 6d65 2f73 725f 696e 666f  ihomo.me/sr_info
+000001f0: 5f70 6172 7365 642f 7b75 6964 7d3f 6c61  _parsed/{uid}?la
+00000200: 6e67 3d7b 6c61 6e67 7d7a 3a68 7474 7073  ng={lang}z:https
+00000210: 3a2f 2f61 7069 2e6d 6968 6f6d 6f2e 6d65  ://api.mihomo.me
+00000220: 2f73 725f 696e 666f 2f7b 7569 647d 3f6c  /sr_info/{uid}?l
+00000230: 616e 673d 7b6c 616e 677d 2676 6572 7369  ang={lang}&versi
+00000240: 6f6e 3d76 317a 8168 7474 7073 3a2f 2f6d  on=v1z.https://m
+00000250: 616e 612e 7769 6b69 2f73 7461 7272 6169  ana.wiki/starrai
+00000260: 6c2f 636f 6c6c 6563 7469 6f6e 732f 6c69  l/collections/li
+00000270: 6768 7443 6f6e 6573 2f7b 6964 7d3f 5f64  ghtCones/{id}?_d
+00000280: 6174 613d 5f63 7573 746f 6d25 3246 726f  ata=_custom%2Fro
+00000290: 7574 6573 2532 4625 3234 7369 7465 4964  utes%2F%24siteId
+000002a0: 2e63 6f6c 6c65 6374 696f 6e73 2532 4225  .collections%2B%
+000002b0: 3246 6c69 6768 7443 6f6e 6573 5f2e 2532  2FlightCones_.%2
+000002c0: 3465 6e74 7279 4964 6301 0000 0000 0000  4entryIdc.......
+000002d0: 0000 0000 0004 0000 000a 0000 00c3 0000  ................
+000002e0: 0073 bc00 0000 8101 7400 a001 a100 3400  .s......t.....4.
+000002f0: 4900 6400 4800 9a48 7d01 7c01 a002 7c00  I.d.H..H}.|...|.
+00000300: a101 3400 4900 6400 4800 9a28 7d02 7c02  ..4.I.d.H..(}.|.
+00000310: a003 a100 4900 6400 4800 7d03 6401 7c03  ....I.d.H.}.d.|.
+00000320: 7600 7225 7404 7c03 6401 1900 8301 8201  v.r%t.|.d.......
+00000330: 7c03 5700 0200 6400 0400 0400 8303 4900  |.W...d.......I.
+00000340: 6400 4800 0100 5700 0200 6400 0400 0400  d.H...W...d.....
+00000350: 8303 4900 6400 4800 0100 5300 3100 4900  ..I.d.H...S.1.I.
+00000360: 6400 4800 7341 7701 0100 0100 0100 5900  d.H.sAw.......Y.
+00000370: 0100 5700 6400 0400 0400 8303 4900 6400  ..W.d.......I.d.
+00000380: 4800 0100 6400 5300 3100 4900 6400 4800  H...d.S.1.I.d.H.
+00000390: 7357 7701 0100 0100 0100 5900 0100 6400  sWw.......Y...d.
+000003a0: 5300 2902 4e5a 0664 6574 6169 6c29 05da  S.).NZ.detail)..
+000003b0: 0761 696f 6874 7470 5a0d 436c 6965 6e74  .aiohttpZ.Client
+000003c0: 5365 7373 696f 6eda 0367 6574 da04 6a73  Session..get..js
+000003d0: 6f6e da09 5479 7065 4572 726f 7229 04da  on..TypeError)..
+000003e0: 0375 726c da07 7365 7373 696f 6eda 0872  .url..session..r
+000003f0: 6573 706f 6e73 65da 0464 6174 61a9 0072  esponse..data..r
+00000400: 1c00 0000 fa37 433a 5c55 7365 7273 5c44  .....7C:\Users\D
+00000410: 6172 736f 585c 4465 736b 746f 705c 7265  arsoX\Desktop\re
+00000420: 735c 686f 6e6b 6169 7261 696c 5c73 7263  s\honkairail\src
+00000430: 5c74 6f6f 6c73 5c61 7069 2e70 79da 0a66  \tools\api.py..f
+00000440: 6574 6368 5f64 6174 611c 0000 0073 1600  etch_data....s..
+00000450: 0000 0280 1201 1401 0e01 0801 0c01 0201  ................
+00000460: 14fc 16ff 1801 2eff 721e 0000 0063 0300  ........r....c..
+00000470: 0000 0000 0000 0000 0000 0400 0000 0400  ................
+00000480: 0000 c300 0000 7346 0000 0081 0174 00a0  ......sF.....t..
+00000490: 017c 01a0 02a1 0064 01a1 027d 017c 0264  .|.....d...}.|.d
+000004a0: 026b 0272 1574 036a 047c 007c 0164 038d  .k.r.t.j.|.|.d..
+000004b0: 027d 036e 0774 056a 047c 007c 0164 038d  .}.n.t.j.|.|.d..
+000004c0: 027d 0374 067c 0383 0149 0064 0048 0053  .}.t.|...I.d.H.S
+000004d0: 0029 044e 720a 0000 0072 0200 0000 a902  .).Nr....r......
+000004e0: da03 7569 64da 046c 616e 6729 07da 1353  ..uid..lang)...S
+000004f0: 5550 504f 5254 4544 5f4c 414e 4755 4147  UPPORTED_LANGUAG
+00000500: 4553 7215 0000 00da 056c 6f77 6572 da08  ESr......lower..
+00000510: 4150 495f 4c49 4e4b da06 666f 726d 6174  API_LINK..format
+00000520: da0b 4150 495f 4c49 4e4b 5f56 3272 1e00  ..API_LINK_V2r..
+00000530: 0000 2904 7220 0000 0072 2100 0000 da01  ..).r ...r!.....
+00000540: 7672 1800 0000 721c 0000 0072 1c00 0000  vr....r....r....
+00000550: 721d 0000 00da 0d67 6574 5f75 7365 725f  r......get_user_
+00000560: 6461 7461 2400 0000 730c 0000 0002 8010  data$...s.......
+00000570: 0108 0110 010e 020e 0172 2800 0000 6302  .........r(...c.
+00000580: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000590: 0000 00c3 0000 0073 2e00 0000 8101 7400  .......s......t.
+000005a0: a001 7c01 a002 a100 6401 a102 7d01 7403  ..|.....d...}.t.
+000005b0: 6a04 7c00 7c01 6402 8d02 7d02 7405 7c02  j.|.|.d...}.t.|.
+000005c0: 8301 4900 6400 4800 5300 2903 4e72 0a00  ..I.d.H.S.).Nr..
+000005d0: 0000 721f 0000 0029 0672 2200 0000 7215  ..r....).r"...r.
+000005e0: 0000 0072 2300 0000 da0d 4655 4c4c 5f41  ...r#.....FULL_A
+000005f0: 5049 5f4c 494e 4b72 2500 0000 721e 0000  PI_LINKr%...r...
+00000600: 0029 0372 2000 0000 7221 0000 0072 1800  .).r ...r!...r..
+00000610: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000620: 00da 1267 6574 5f66 756c 6c5f 7573 6572  ...get_full_user
+00000630: 5f64 6174 612c 0000 0073 0800 0000 0280  _data,...s......
+00000640: 1001 0e01 0e01 722a 0000 0063 0100 0000  ......r*...c....
+00000650: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000660: c300 0000 731c 0000 0081 0174 006a 017c  ....s......t.j.|
+00000670: 0064 018d 017d 0174 027c 0183 0149 0064  .d...}.t.|...I.d
+00000680: 0048 0053 0029 024e 2901 720d 0000 0029  .H.S.).N).r....)
+00000690: 03da 104c 4947 4854 5f43 4f4e 4553 5f4c  ...LIGHT_CONES_L
+000006a0: 494e 4b72 2500 0000 721e 0000 0029 0272  INKr%...r....).r
+000006b0: 0d00 0000 7218 0000 0072 1c00 0000 721c  ....r....r....r.
+000006c0: 0000 0072 1d00 0000 da14 6765 745f 6c69  ...r......get_li
+000006d0: 6768 745f 636f 6e65 735f 6461 7461 3100  ght_cones_data1.
+000006e0: 0000 7306 0000 0002 800c 010e 0172 2c00  ..s..........r,.
+000006f0: 0000 6303 0000 0000 0000 0000 0000 0004  ..c.............
+00000700: 0000 0004 0000 00c3 0000 0073 4400 0000  ...........sD...
+00000710: 8101 7400 7c01 7c00 7c02 8303 4900 6400  ..t.|.|.|...I.d.
+00000720: 4800 7d03 7c02 6401 6b02 7218 7401 7c03  H.}.|.d.k.r.t.|.
+00000730: 6402 1900 7c03 6403 1900 6404 8d02 5300  d...|.d...d...S.
+00000740: 7402 7c03 6402 1900 7c03 6403 1900 6404  t.|.d...|.d...d.
+00000750: 8d02 5300 2905 4e72 0200 0000 da06 706c  ..S.).Nr......pl
+00000760: 6179 6572 da0a 6368 6172 6163 7465 7273  ayer..characters
+00000770: a902 722d 0000 0072 2e00 0000 2903 7228  ..r-...r....).r(
+00000780: 0000 0072 0300 0000 7205 0000 0029 0472  ...r....r....).r
+00000790: 2100 0000 7220 0000 0072 2700 0000 721b  !...r ...r'...r.
+000007a0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+000007b0: 0000 da08 6765 745f 6461 7461 3500 0000  ....get_data5...
+000007c0: 730a 0000 0002 8012 0108 0114 0114 0172  s..............r
+000007d0: 3000 0000 6303 0000 0000 0000 0000 0000  0...c...........
+000007e0: 0007 0000 0004 0000 00c3 0000 0073 fe00  .............s..
+000007f0: 0000 8101 7400 7c01 7c00 7c02 8303 4900  ....t.|.|.|...I.
+00000800: 6400 4800 7d03 7401 7c01 7c00 8302 4900  d.H.}.t.|.|...I.
+00000810: 6400 4800 7d04 7c03 6401 1900 4400 5d0c  d.H.}.|.d...D.].
+00000820: 7d05 7c05 6402 1900 6900 6b02 7222 6400  }.|.d...i.k.r"d.
+00000830: 7c05 6402 3c00 7116 7c02 6403 6b02 7275  |.d.<.q.|.d.k.ru
+00000840: 7c04 6404 1900 7d06 7c06 6405 1900 7c03  |.d...}.|.d...|.
+00000850: 6406 1900 6407 3c00 7c06 6408 1900 7c03  d...d.<.|.d...|.
+00000860: 6406 1900 6409 3c00 640a 7c03 6406 1900  d...d.<.d.|.d...
+00000870: 640b 3c00 7c06 640c 1900 640d 1900 640e  d.<.|.d...d...d.
+00000880: 1900 7c03 6406 1900 640f 3c00 7c06 640c  ..|.d...d.<.|.d.
+00000890: 1900 6410 1900 7c03 6406 1900 6402 3c00  ..d...|.d...d.<.
+000008a0: 7c06 640c 1900 6411 1900 7c03 6406 1900  |.d...d...|.d...
+000008b0: 6401 3c00 7c06 640c 1900 6412 1900 7c03  d.<.|.d...d...|.
+000008c0: 6406 1900 6413 3c00 7402 7c03 6406 1900  d...d.<.t.|.d...
+000008d0: 7c03 6401 1900 6414 8d02 5300 7403 7c03  |.d...d...S.t.|.
+000008e0: 6406 1900 7c03 6401 1900 6414 8d02 5300  d...|.d...d...S.
+000008f0: 2915 4e72 2e00 0000 da0a 6c69 6768 745f  ).Nr......light_
+00000900: 636f 6e65 7202 0000 005a 0a64 6574 6169  coner....Z.detai
+00000910: 6c49 6e66 6f5a 0b66 7269 656e 6443 6f75  lInfoZ.friendCou
+00000920: 6e74 722d 0000 005a 0766 7269 656e 6473  ntr-...Z.friends
+00000930: 5a0a 776f 726c 644c 6576 656c 5a0a 776f  Z.worldLevelZ.wo
+00000940: 726c 646c 6576 656c da01 305a 0862 6972  rldlevel..0Z.bir
+00000950: 7468 6461 795a 0a72 6563 6f72 6449 6e66  thdayZ.recordInf
+00000960: 6f5a 0d63 6861 6c6c 656e 6765 496e 666f  oZ.challengeInfo
+00000970: 5a10 7363 6865 6475 6c65 4d61 784c 6576  Z.scheduleMaxLev
+00000980: 656c 5a12 7061 7373 5f61 7265 615f 7072  elZ.pass_area_pr
+00000990: 6f67 7265 7373 5a0e 6571 7569 706d 656e  ogressZ.equipmen
+000009a0: 7443 6f75 6e74 5a0b 6176 6174 6172 436f  tCountZ.avatarCo
+000009b0: 756e 745a 1061 6368 6965 7665 6d65 6e74  untZ.achievement
+000009c0: 436f 756e 745a 0b61 6368 6965 7665 6d65  CountZ.achieveme
+000009d0: 6e74 722f 0000 0029 0472 2800 0000 722a  ntr/...).r(...r*
+000009e0: 0000 0072 0300 0000 7205 0000 0029 0772  ...r....r....).r
+000009f0: 2100 0000 7220 0000 0072 2700 0000 721b  !...r ...r'...r.
+00000a00: 0000 005a 0770 726f 6669 6c65 da03 6b65  ...Z.profile..ke
+00000a10: 795a 0b70 6c61 7965 725f 696e 666f 721c  yZ.player_infor.
+00000a20: 0000 0072 1c00 0000 721d 0000 00da 0867  ...r....r......g
+00000a30: 6574 5f66 756c 6c3b 0000 0073 2400 0000  et_full;...s$...
+00000a40: 0280 1201 1001 0c01 0c01 0801 0280 0801  ................
+00000a50: 0801 1001 1001 0c01 1801 1401 1401 1401  ................
+00000a60: 1402 1401 7234 0000 0029 1472 1400 0000  ....r4...).r....
+00000a70: da07 6173 796e 6369 6f72 1600 0000 da05  ..asyncior......
+00000a80: 6d6f 6461 6c72 0300 0000 7204 0000 0072  modalr....r....r
+00000a90: 0500 0000 da00 7206 0000 0072 2200 0000  ......r....r"...
+00000aa0: 7224 0000 0072 2600 0000 7229 0000 0072  r$...r&...r)...r
+00000ab0: 2b00 0000 721e 0000 0072 2800 0000 722a  +...r....r(...r*
+00000ac0: 0000 0072 2c00 0000 7230 0000 0072 3400  ...r,...r0...r4.
+00000ad0: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000ae0: 0072 1d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000af0: 0100 0000 733a 0000 0008 0008 0108 0114  ....s:..........
+00000b00: 010c 0102 0302 0102 0102 0102 0102 0102  ................
+00000b10: 0102 0102 0102 0102 0102 0102 0106 f304  ................
+00000b20: 1004 0104 0104 0108 0208 0808 0808 0508  ................
+00000b30: 040c 06                                  ...
```

### Comparing `honkairail-1.0.0/honkairail/src/tools/api.py` & `honkairail-1.0.1/honkairail/src/tools/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import aiohttp
 import asyncio
 import json
-from .modal import StarRailApiData, PlayerInfo
+from .modal import StarRailApiData, PlayerInfo,StarRailApiDataV2
 from . import utilities
 
 SUPPORTED_LANGUAGES = {
     'cht': 'cht',
     'cn': 'cn',
     'de': 'de',
     'en': 'en',
@@ -16,63 +16,64 @@
     'kr': 'kr',
     'pt': 'pt',
     'ru': 'ru',
     'th': 'th',
     'vi': 'vi'
 }
 
-API_LINK = "https://api.mihomo.me/sr_info_parsed/{uid}?lang={lang}"
-FULL_API_LINK = "https://api.mihomo.me/sr_info/{uid}?lang={lang}"
+API_LINK = "https://api.mihomo.me/sr_info_parsed/{uid}?lang={lang}&version=v1"
+API_LINK_V2 = "https://api.mihomo.me/sr_info_parsed/{uid}?lang={lang}"
+FULL_API_LINK = "https://api.mihomo.me/sr_info/{uid}?lang={lang}&version=v1"
 LIGHT_CONES_LINK = "https://mana.wiki/starrail/collections/lightCones/{id}?_data=_custom%2Froutes%2F%24siteId.collections%2B%2FlightCones_.%24entryId"
 
 async def fetch_data(url):
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             data = await response.json()
             if "detail" in data:
                 raise TypeError(data["detail"])
             return data
 
-async def get_user_data(uid, lang):
+async def get_user_data(uid, lang, v):
     lang = SUPPORTED_LANGUAGES.get(lang.lower(), "en")
-    url = API_LINK.format(uid=uid, lang=lang)
+    if v == 1:
+        url = API_LINK.format(uid=uid, lang=lang)
+    else:
+        url = API_LINK_V2.format(uid=uid, lang=lang)
     return await fetch_data(url)
 
 async def get_full_user_data(uid, lang):
     lang = SUPPORTED_LANGUAGES.get(lang.lower(), "en")
     url = FULL_API_LINK.format(uid=uid, lang=lang)
     return await fetch_data(url)
 
 async def get_light_cones_data(id):
     url = LIGHT_CONES_LINK.format(id=id)
     return await fetch_data(url)
 
-async def get_data(lang, uid):
-    data = await get_user_data(uid, lang)
-    return StarRailApiData(player=data["player"], characters=data["characters"])
-
-async def get_profile(lang, uid):
-    data = await get_full_user_data(uid, lang)
-    player_info = PlayerInfo(**data)
-    return player_info.PlayerDetailInfo
-
-async def get_full(lang, uid):
-    profile, data = await asyncio.gather(get_profile(lang, uid), get_user_data(uid, lang))
-    profile = json.loads(profile.json())
-
+async def get_data(lang, uid, v):
+    data = await get_user_data(uid, lang, v)
+    if v == 1:
+        return StarRailApiData(player=data["player"], characters=data["characters"])
+    return StarRailApiDataV2(player=data["player"], characters=data["characters"])
+
+async def get_full(lang, uid,v):
+    data = await get_user_data(uid, lang,v)
+    profile = await get_full_user_data(uid,lang)
     for key in data["characters"]:
         if key["light_cone"] == {}:
             key["light_cone"] = None
+    if v == 1:
+        player_info = profile["detailInfo"]
+        data["player"]["friends"] = player_info["friendCount"]
+        data["player"]["worldlevel"] = player_info["worldLevel"]
+        data["player"]["birthday"] = "0"#utilities.convert_date(profile["Birthday"])
+        data["player"]["pass_area_progress"] = player_info["recordInfo"]["challengeInfo"]["scheduleMaxLevel"]
+        data["player"]["light_cone"] = player_info["recordInfo"]["equipmentCount"]
+        data["player"]["characters"] = player_info["recordInfo"]["avatarCount"]
+        data["player"]["achievement"] = player_info["recordInfo"]["achievementCount"]
 
-    player_info = profile["PlayerSpaceInfo"]
-    data["player"]["friends"] = profile["CurFriendCount"]
-    data["player"]["worldlevel"] = profile["WorldLevel"]
-    data["player"]["birthday"] = utilities.convert_date(profile["Birthday"])
-    data["player"]["pass_area_progress"] = player_info["PassAreaProgress"]
-    data["player"]["light_cone"] = player_info["LightConeCount"]
-    data["player"]["characters"] = player_info["AvatarCount"]
-    data["player"]["achievement"] = player_info["AchievementCount"]
-    
-    return StarRailApiData(player=data["player"], characters=data["characters"])
+        return StarRailApiData(player=data["player"], characters=data["characters"])
+    return StarRailApiDataV2(player=data["player"], characters=data["characters"])
```

### Comparing `honkairail-1.0.0/honkairail/starrailapi.py` & `honkairail-1.0.1/honkairail/starrailapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from .src.tools import api, modal,utilities
 
 class StarRailApi():
-    def __init__(self,lang) -> None:
+    def __init__(self,lang, v = 1) -> None:
         self.lang = lang
+        if not v in [1,2]:
+            v = 1
+        self.v = v
 
     async def get_user(self,uid):
-        data = await api.get_data(self.lang,uid)
+        data = await api.get_data(self.lang,uid,self.v)
         return data
     
     async def get_user_profile(self,uid):
         data = await api.get_profile(self.lang,uid)
         return data
     
     async def get_full_data(self,uid):
-        data = await api.get_full(self.lang,uid)
+        data = await api.get_full(self.lang,uid,self.v)
         return data
     
     async def get_light_cone_info(self, instance):
         stats = await api.get_light_cones_data(instance.id)
         data = utilities.get_stats_light_cone(stats["defaultData"]["stats_csv"], instance.level)
         patch = stats["defaultData"]["path"]
         icon = patch["icon"]
```

### Comparing `honkairail-1.0.0/README.md` & `honkairail-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 ```
 
 ## Uses:
 ``` py
 from honkairail import starrailapi
 import asyncio
 
+#The sample code below matches version 1 (v = 1), but you can set it to 1 or 2. The second version is newer and contains a bit more data.
 async def main(uid,lang):
-    r = starrailapi.StarRailApi(lang)
+    r = starrailapi.StarRailApi(lang, v = 1)
     data = await r.get_full_data(uid)
     print(data)
 
 asyncio.run(main(700649319,"en"))
 ```
 
 ## Usage example:
@@ -33,15 +34,14 @@
     data = await r.get_full_data(uid)
     print("====Player====")
     print(f"Name: {data.player.name}")
     print(f"UID: {data.player.uid}")
     print(f"Level: {data.player.level}")
     print(f"World Level: {data.player.worldlevel}")
     
-    print(f"Birthday: {data.player.birthday}")
     print(f"Friends: {data.player.friends}")
 
     print(f"Pass Area Progress: {data.player.pass_area_progress}")
     print(f"Achievement: {data.player.achievement}")
 
     print(f"Characters: {data.player.characters}")
     print(f"Light Cone: {data.player.light_cone}")
```

### Comparing `honkairail-1.0.0/setup.py` & `honkairail-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['honkairail', 'honkairail.src', 'honkairail.src.tools']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'honkairail',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'A simple and convenient model for Mihoyo API which is complemented by other resources',
-    'long_description': '# HonkaiRail\n A simple and convenient model for Mihoyo API which is complemented by other resources\n\n\n## Install:\n\n```\npip install honkairail\n```\n\n## Uses:\n``` py\nfrom honkairail import starrailapi\nimport asyncio\n\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang)\n    data = await r.get_full_data(uid)\n    print(data)\n\nasyncio.run(main(700649319,"en"))\n```\n\n## Usage example:\n\n```py\nfrom honkairail import starrailapi\nimport asyncio\n\n\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang)\n    data = await r.get_full_data(uid)\n    print("====Player====")\n    print(f"Name: {data.player.name}")\n    print(f"UID: {data.player.uid}")\n    print(f"Level: {data.player.level}")\n    print(f"World Level: {data.player.worldlevel}")\n    \n    print(f"Birthday: {data.player.birthday}")\n    print(f"Friends: {data.player.friends}")\n\n    print(f"Pass Area Progress: {data.player.pass_area_progress}")\n    print(f"Achievement: {data.player.achievement}")\n\n    print(f"Characters: {data.player.characters}")\n    print(f"Light Cone: {data.player.light_cone}")\n\n    print(f"Icon: {data.player.icon}")\n    print(f"Signature: {data.player.signature}")\n    print(\'\\n\\n\')\n    print("====Characters====")\n    for character in data.characters:\n        print(f"Name: {character.name} | {character.id}")\n        print(f"Rarity: {\'★\'*character.rarity}")\n        print(f"LVL: {character.level}")\n        print(f"===={character.rank_text}====")\n        for rank in character.rank_icons:\n            print(f"Icon: {rank.icon}\\nUnlock: {rank.unlock}")\n        print("====Skill====")\n        for skill in character.skill:\n            print(f"Icon: {skill.icon}\\nLVL:{skill.level}")\n        print("=============")\n        if not character.light_cone is None:\n            print(f"Light Cone: {character.light_cone.name}")\n            print(f"Rarity: {\'★\'*character.light_cone.rarity}")\n            print(f"LVL: {character.light_cone.level} | R{character.light_cone.rank}")\n            print(f"Icon: {character.light_cone.icon}")\n            print(f"Portrait: {character.light_cone.portrait}")\n            light_cone = await r.get_light_cone_info(character.light_cone)\n            print(f"ATK: {light_cone.atk} | HP: {light_cone.hp} | DEF: {light_cone.defense}")\n            print(f"Path: {light_cone.patch.name}\\nImage: {light_cone.patch.url}")\n        print("====Stats====")\n        for property in character.property:\n            if property.addition is None:\n                print(f"{property.name}: {property.base}\\nIcon: {property.icon}")\n            else:\n                print(f"{property.name}: {property.base} ({property.addition})\\n==Icon: {property.icon}")\n        print(\'\\n\\n\')\n        print("====Relic====")\n        for i in character.relic:\n            print(f"{character.relic[i].name}: {character.relic[i].level} lvl | {\'★\'*character.relic[i].rarity}")\n            print(f"{character.relic[i].main_property.name}: {character.relic[i].main_property.value}")\n            for sub_property in character.relic[i].sub_property:\n                print(f"=={sub_property.name}: {sub_property.value}\\n====Icon: {sub_property.icon}")\n            print(\'\\n\')\n        print("\\n\\n")\n\nasyncio.run(main(700649319, "en"))\n```\n\n\n### Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cn  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n\n',
+    'long_description': '# HonkaiRail\n A simple and convenient model for Mihoyo API which is complemented by other resources\n\n\n## Install:\n\n```\npip install honkairail\n```\n\n## Uses:\n``` py\nfrom honkairail import starrailapi\nimport asyncio\n\n#The sample code below matches version 1 (v = 1), but you can set it to 1 or 2. The second version is newer and contains a bit more data.\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang, v = 1)\n    data = await r.get_full_data(uid)\n    print(data)\n\nasyncio.run(main(700649319,"en"))\n```\n\n## Usage example:\n\n```py\nfrom honkairail import starrailapi\nimport asyncio\n\n\nasync def main(uid,lang):\n    r = starrailapi.StarRailApi(lang)\n    data = await r.get_full_data(uid)\n    print("====Player====")\n    print(f"Name: {data.player.name}")\n    print(f"UID: {data.player.uid}")\n    print(f"Level: {data.player.level}")\n    print(f"World Level: {data.player.worldlevel}")\n    \n    print(f"Friends: {data.player.friends}")\n\n    print(f"Pass Area Progress: {data.player.pass_area_progress}")\n    print(f"Achievement: {data.player.achievement}")\n\n    print(f"Characters: {data.player.characters}")\n    print(f"Light Cone: {data.player.light_cone}")\n\n    print(f"Icon: {data.player.icon}")\n    print(f"Signature: {data.player.signature}")\n    print(\'\\n\\n\')\n    print("====Characters====")\n    for character in data.characters:\n        print(f"Name: {character.name} | {character.id}")\n        print(f"Rarity: {\'★\'*character.rarity}")\n        print(f"LVL: {character.level}")\n        print(f"===={character.rank_text}====")\n        for rank in character.rank_icons:\n            print(f"Icon: {rank.icon}\\nUnlock: {rank.unlock}")\n        print("====Skill====")\n        for skill in character.skill:\n            print(f"Icon: {skill.icon}\\nLVL:{skill.level}")\n        print("=============")\n        if not character.light_cone is None:\n            print(f"Light Cone: {character.light_cone.name}")\n            print(f"Rarity: {\'★\'*character.light_cone.rarity}")\n            print(f"LVL: {character.light_cone.level} | R{character.light_cone.rank}")\n            print(f"Icon: {character.light_cone.icon}")\n            print(f"Portrait: {character.light_cone.portrait}")\n            light_cone = await r.get_light_cone_info(character.light_cone)\n            print(f"ATK: {light_cone.atk} | HP: {light_cone.hp} | DEF: {light_cone.defense}")\n            print(f"Path: {light_cone.patch.name}\\nImage: {light_cone.patch.url}")\n        print("====Stats====")\n        for property in character.property:\n            if property.addition is None:\n                print(f"{property.name}: {property.base}\\nIcon: {property.icon}")\n            else:\n                print(f"{property.name}: {property.base} ({property.addition})\\n==Icon: {property.icon}")\n        print(\'\\n\\n\')\n        print("====Relic====")\n        for i in character.relic:\n            print(f"{character.relic[i].name}: {character.relic[i].level} lvl | {\'★\'*character.relic[i].rarity}")\n            print(f"{character.relic[i].main_property.name}: {character.relic[i].main_property.value}")\n            for sub_property in character.relic[i].sub_property:\n                print(f"=={sub_property.name}: {sub_property.value}\\n====Icon: {sub_property.icon}")\n            print(\'\\n\')\n        print("\\n\\n")\n\nasyncio.run(main(700649319, "en"))\n```\n\n\n### Languages Supported\n| Languege    |  Code   | Languege    |  Code   | Languege    |  Code   |\n|-------------|---------|-------------|---------|-------------|---------|\n|  English    |     en  |  русский    |     ru  |  Chinese    |    chs  |\n|  Tiếng Việt |     vi  |  ไทย        |     th  | Taiwan     |    cn  |\n|  português  |     pt  | 한국어      |     kr  | deutsch    |     de  |\n|  日本語      |     jp  | 中文        |     zh  | español    |     es  |\n|  中文        |     zh  | Indonesian |     id  | français   |     fr  |\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DEViantUA/HonkaiRail',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `honkairail-1.0.0/PKG-INFO` & `honkairail-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honkairail
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple and convenient model for Mihoyo API which is complemented by other resources
 Home-page: https://github.com/DEViantUA/HonkaiRail
 Author: None
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,16 +23,17 @@
 ```
 
 ## Uses:
 ``` py
 from honkairail import starrailapi
 import asyncio
 
+#The sample code below matches version 1 (v = 1), but you can set it to 1 or 2. The second version is newer and contains a bit more data.
 async def main(uid,lang):
-    r = starrailapi.StarRailApi(lang)
+    r = starrailapi.StarRailApi(lang, v = 1)
     data = await r.get_full_data(uid)
     print(data)
 
 asyncio.run(main(700649319,"en"))
 ```
 
 ## Usage example:
@@ -47,15 +48,14 @@
     data = await r.get_full_data(uid)
     print("====Player====")
     print(f"Name: {data.player.name}")
     print(f"UID: {data.player.uid}")
     print(f"Level: {data.player.level}")
     print(f"World Level: {data.player.worldlevel}")
     
-    print(f"Birthday: {data.player.birthday}")
     print(f"Friends: {data.player.friends}")
 
     print(f"Pass Area Progress: {data.player.pass_area_progress}")
     print(f"Achievement: {data.player.achievement}")
 
     print(f"Characters: {data.player.characters}")
     print(f"Light Cone: {data.player.light_cone}")
```

