# Comparing `tmp/nonebot_plugin_mystool-0.2.9.tar.gz` & `tmp/nonebot_plugin_mystool-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-0.2.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-1.0.0b1.tar", max compression
```

## Comparing `nonebot_plugin_mystool-0.2.9.tar` & `nonebot_plugin_mystool-1.0.0b1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/LICENSE
--rw-r--r--   0        0        0     2820 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/README.md
--rw-r--r--   0        0        0     1317 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/addFriend.py
--rw-r--r--   0        0        0     6938 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    30682 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/bbsAPI.py
--rw-r--r--   0        0        0     7081 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/config.py
--rw-r--r--   0        0        0    15416 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/data.py
--rw-r--r--   0        0        0    22944 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    20570 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchangePlan.py
--rw-r--r--   0        0        0    15573 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/gameSign.py
--rw-r--r--   0        0        0     1884 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    14907 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    23334 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/mybMission.py
--rw-r--r--   0        0        0    24358 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0     9827 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    11531 2023-05-18 07:37:15.791978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     3538 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/README.md
+-rw-r--r--   0        0        0     1324 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1794 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     4494 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    12122 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/data_model.py
+-rw-r--r--   0        0        0    21278 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    10211 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/game_sign_api.py
+-rw-r--r--   0        0        0     5467 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/good_image.py
+-rw-r--r--   0        0        0     1959 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0     9562 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    21993 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/myb_missions_api.py
+-rw-r--r--   0        0        0    22256 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0    10693 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/plugin_data.py
+-rw-r--r--   0        0        0     8912 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    62140 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/simple_api.py
+-rw-r--r--   0        0        0     2230 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_check.py
+-rw-r--r--   0        0        0    11313 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/user_data.py
+-rw-r--r--   0        0        0     9199 2023-06-10 07:04:34.144244 nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-1.0.0b1/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-0.2.9/LICENSE` & `nonebot_plugin_mystool-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.9/README.md` & `nonebot_plugin_mystool-1.0.0b1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -46,132 +46,177 @@
 000002d0: 6c61 7374 2d63 6f6d 6d69 742f 4c6a 7a64  last-commit/Ljzd
 000002e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
 000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
 00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
 00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
 00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
 00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
-00000340: b60a 0a2a 2ae7 8988 e69c ac20 2d20 7630  ...**...... - v0
-00000350: 2e32 2e39 2a2a 0a0a 2323 2320 f09f 93a3  .2.9**..### ....
-00000360: 20e6 9bb4 e696 b0e5 8685 e5ae b90a 0a23   ..............#
-00000370: 2323 2320 3230 3233 2e35 2e31 380a 2d20  ### 2023.5.18.- 
-00000380: e5a4 9ae8 bf9b e7a8 8be7 949f e688 90e5  ................
-00000390: 9586 e593 81e5 9bbe e789 87ef bc88 e5a4  ................
-000003a0: 9ae6 a0b8 efbc 89ef bc8c e58a a0e5 bfab  ................
-000003b0: e59b bee7 8987 e794 9fe6 8890 e980 9fe5  ................
-000003c0: baa6 0a2d 20e4 bfae e5a4 8de9 83a8 e588  ...- ...........
-000003d0: 86e5 9586 e593 81e5 8591 e68d a2e6 97b6  ................
-000003e0: e997 b4e9 9499 e8af afe7 9a84 e997 aee9  ................
-000003f0: a298 efbc 88e5 a682 e7b1 b3e6 b8b8 e7a4  ................
-00000400: bee5 9586 e593 81e6 999a e4ba 86e4 b880  ................
-00000410: e591 a8ef bc89 0a0a 2323 2323 2032 3032  ........#### 202
-00000420: 332e 352e 340a 2d20 e5a2 9ee5 8aa0 e5af  3.5.4.- ........
-00000430: b9e6 989f e7a9 b9e9 9381 e981 93e7 9a84  ................
-00000440: e7ad bee5 88b0 e58a 9fe8 83bd e79a 84e6  ................
-00000450: 94af e68c 8120 2d20 5b23 3839 5d28 6874  ..... - [#89](ht
-00000460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000470: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
-00000480: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000490: 2f70 756c 6c2f 3839 2920 6279 2040 6179  /pull/89) by @ay
-000004a0: 616b 6173 756b 690a 2d20 e4bf aee5 a48d  akasuki.- ......
-000004b0: e68f 92e4 bbb6 e591 bde4 bba4 e4bc 98e5  ................
-000004c0: 8588 e5ba a6e9 97ae e9a2 9820 2d20 5b23  ........... - [#
-000004d0: 3838 5d28 6874 7470 733a 2f2f 6769 7468  88](https://gith
-000004e0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-000004f0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000500: 7973 746f 6f6c 2f70 756c 6c2f 3838 2920  ystool/pull/88) 
-00000510: 6279 2040 6179 616b 6173 756b 690a 2d20  by @ayakasuki.- 
-00000520: e983 a8e5 8886 e696 87e6 9cac e994 99e8  ................
-00000530: afaf e4bf aee6 ada3 202d 205b 2339 305d  ........ - [#90]
-00000540: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000550: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-00000560: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000570: 6f6f 6c2f 7075 6c6c 2f39 3029 2062 7920  ool/pull/90) by 
-00000580: 4062 6c61 636b 2d7a 6572 6f33 3538 0a0a  @black-zero358..
-00000590: 2e2e 2e0a 0a23 2323 2320 3230 3233 2e33  .....#### 2023.3
-000005a0: 2e33 300a 2d20 e4bf aee5 a48d 2060 2fe5  .30.- ...... `/.
-000005b0: 8591 e68d a260 20e5 91bd e4bb a4e5 8faf  .....` .........
-000005c0: e883 bde4 b88e e585 b6e4 bb96 e68f 92e4  ................
-000005d0: bbb6 e591 bde4 bba4 e586 b2e7 aa81 e79a  ................
-000005e0: 84e9 97ae e9a2 98ef bc8c e590 8ce6 97b6  ................
-000005f0: 205b f09f 9497 e794 a8e6 b395 e58f 98e6   [..............
-00000600: 9bb4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000610: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000620: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000630: 7973 746f 6f6c 2f77 696b 692f 496e 666f  ystool/wiki/Info
-00000640: 726d 6174 696f 6e2d 4578 6368 616e 6765  rmation-Exchange
-00000650: 23e5 a29e e58a a0e5 88a0 e999 a4e5 8591  #...............
-00000660: e68d a2e8 aea1 e588 9229 0a2d 202e 2e2e  .........).- ...
-00000670: 0a0a 2323 20e5 8a9f e883 bde5 928c e789  ..## ...........
-00000680: b9e6 80a7 0a0a 2d20 e79f ade4 bfa1 e9aa  ......- ........
-00000690: 8ce8 af81 e799 bbe5 bd95 efbc 8ce5 858d  ................
-000006a0: e68a 93e5 8c85 e88e b7e5 8f96 2043 6f6f  ............ Coo
-000006b0: 6b69 650a 2d20 e887 aae5 8aa8 e5ae 8ce6  kie.- ..........
-000006c0: 8890 e6af 8fe6 97a5 e7b1 b3e6 b8b8 e5b8  ................
-000006d0: 81e4 bbbb e58a a10a 2d20 e887 aae5 8aa8  ........- ......
-000006e0: e8bf 9be8 a18c e6b8 b8e6 888f e7ad bee5  ................
-000006f0: 88b0 0a2d 20e5 8faf e588 b6e5 ae9a e7b1  ...- ...........
-00000700: b3e6 b8b8 e5b8 81e5 9586 e593 81e5 8591  ................
-00000710: e68d a2e8 aea1 e588 92ef bc8c e588 b0e7  ................
-00000720: 82b9 e585 91e6 8da2 0a2d 20e5 8faf e694  .........- .....
-00000730: afe6 8c81 e5a4 9ae4 b8aa 2051 5120 e8b4  .......... QQ ..
-00000740: a6e5 8fb7 efbc 8ce6 af8f e4b8 aa20 5151  ............. QQ
-00000750: 20e8 b4a6 e58f b7e5 8faf e7bb 91e5 ae9a   ...............
-00000760: e5a4 9ae4 b8aa e7b1 b3e5 9388 e6b8 b8e8  ................
-00000770: b4a6 e688 b70a 2d20 5151 20e6 8ea8 e980  ......- QQ .....
-00000780: 81e6 89a7 e8a1 8ce7 bb93 e69e 9ce9 809a  ................
-00000790: e79f a50a 2d20 e58e 9fe7 a59e e6a0 91e8  ....- ..........
-000007a0: 8482 e380 81e6 b49e e5a4 a9e5 ae9d e992  ................
-000007b0: b1e3 8081 e8b4 a8e9 878f e58f 82e5 8f98  ................
-000007c0: e4bb aae5 b7b2 e6bb a1e6 97b6 e68e a8e9  ................
-000007d0: 8081 e980 9ae7 9fa5 0a0a 2323 20e4 bdbf  ..........## ...
-000007e0: e794 a8e8 afb4 e698 8e0a 0a23 2323 20f0  ...........### .
-000007f0: 9f9b a0ef b88f 204e 6f6e 6542 6f74 3220  ...... NoneBot2 
-00000800: e69c bae5 99a8 e4ba bae9 83a8 e7bd b2e5  ................
-00000810: 928c e68f 92e4 bbb6 e5ae 89e8 a385 0a0a  ................
-00000820: e8af b7e6 9fa5 e79c 8b20 2d3e 205b f09f  ......... -> [..
-00000830: 9497 496e 7374 616c 6c61 7469 6f6e 5d28  ..Installation](
-00000840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000850: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
-00000860: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00000870: 6f6c 2f77 696b 692f 496e 7374 616c 6c61  ol/wiki/Installa
-00000880: 7469 6f6e 290a 0a23 2323 20f0 9f93 9620  tion)..### .... 
-00000890: e68f 92e4 bbb6 e585 b7e4 bd93 e4bd bfe7  ................
-000008a0: 94a8 e8af b4e6 988e 0a0a e8af b7e6 9fa5  ................
-000008b0: e79c 8b20 2d3e 205b f09f 9497 5769 6b69  ... -> [....Wiki
-000008c0: 20e6 9687 e6a1 a35d 2868 7474 7073 3a2f   ......](https:/
-000008d0: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-000008e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-000008f0: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
-00000900: 290a 0a23 2323 20e2 9d93 20e8 8eb7 e58f  )..### ... .....
-00000910: 96e6 8f92 e4bb b6e5 b8ae e58a a9e4 bfa1  ................
-00000920: e681 af0a 0a23 2323 2320 e68f 92e4 bbb6  .....#### ......
-00000930: e591 bde4 bba4 0a0a 6060 600a 2fe5 b8ae  ........```./...
-00000940: e58a a90a 6060 600a 0a3e 20e2 9aa0 efb8  ....```..> .....
-00000950: 8f20 e6b3 a8e6 848f 20e6 ada4 e5a4 84e6  . ...... .......
-00000960: b2a1 e69c 89e4 bdbf e794 a820 5bf0 9f94  ........... [...
-00000970: 9720 e68f 92e4 bbb6 e591 bde4 bba4 e5a4  . ..............
-00000980: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-00000990: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-000009a0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-000009b0: 7374 6f6f 6c2f 7769 6b69 2f43 6f6e 6669  stool/wiki/Confi
-000009c0: 6775 7261 7469 6f6e 2d43 6f6e 6669 6723  guration-Config#
-000009d0: 636f 6d6d 616e 645f 7374 6172 7429 0a0a  command_start)..
-000009e0: 2323 20e5 85b6 e4bb 960a 0a23 2323 205b  ## ........### [
-000009f0: f09f 9383 e6ba 90e7 a081 e8af b4e6 988e  ................
-00000a00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000a10: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00000a20: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000a30: 746f 6f6c 2f77 696b 692f 536f 7572 6365  tool/wiki/Source
-00000a40: 2d53 7472 7563 7475 7265 290a 2323 2320  -Structure).### 
-00000a50: e980 82e9 858d 205b e7bb aae5 b1b1 e79c  ...... [........
-00000a60: 9fe5 afbb 426f 745d 2868 7474 7073 3a2f  ....Bot](https:/
-00000a70: 2f67 6974 6875 622e 636f 6d2f 4869 6269  /github.com/Hibi
-00000a80: 4b69 6572 2f7a 6865 6e78 756e 5f62 6f74  Kier/zhenxun_bot
-00000a90: 2920 e79a 84e5 8886 e694 af0a 2d20 6874  ) ..........- ht
-00000aa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000ab0: 2f4d 5754 4a43 2f7a 6865 6e78 756e 2d70  /MWTJC/zhenxun-p
-00000ac0: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a 2d20  lugin-mystool.- 
-00000ad0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ae0: 6f6d 2f61 7961 6b61 7375 6b69 2f6e 6f6e  om/ayakasuki/non
-00000af0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-00000b00: 6f6f 6c0a                                ool.
+00000340: b60a 0a2a 2ae7 8988 e69c ac20 2d20 7631  ...**...... - v1
+00000350: 2e30 2e30 2d62 6574 612e 312a 2a0a 0a23  .0.0-beta.1**..#
+00000360: 2323 20f0 9f93 a320 e69b b4e6 96b0 e586  ## .... ........
+00000370: 85e5 aeb9 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
+00000380: 362e 3130 0a0a e694 b9e5 8aa8 e8be 83e5  6.10............
+00000390: a4a7 efbc 8ce7 9bae e589 8de6 98af 2042  .............. B
+000003a0: 6574 6120 e789 88ef bc8c e58f afe8 83bd  eta ............
+000003b0: e4b8 8de7 a8b3 e5ae 9a0a 0a2d 20e5 a4a7  ...........- ...
+000003c0: e987 8fe7 9a84 e4bb a3e7 a081 e987 8de6  ................
+000003d0: 9e84 efbc 8ce5 8c85 e68b ace7 b1b3 e6b8  ................
+000003e0: b8e7 a4be 4150 49e7 9a84 e5ae a2e6 88b7  ....API.........
+000003f0: e7ab afe5 ae9e e78e b0e3 8081 e794 a8e6  ................
+00000400: 88b7 e695 b0e6 8dae e79b b8e5 85b3 e380  ................
+00000410: 81e6 8f92 e4bb b6e9 858d e7bd aee7 9bb8  ................
+00000420: e585 b3e3 8081 4150 49e7 9bb8 e585 b3e6  ......API.......
+00000430: 95b0 e68d aee6 a8a1 e59e 8b0a 2d20 e4bf  ............- ..
+00000440: aee5 a48d e59c a820 5769 6e64 6f77 7320  ....... Windows 
+00000450: e4b8 8be6 97a0 e6b3 95e5 a49a e8bf 9be7  ................
+00000460: a88b e794 9fe6 8890 e595 86e5 9381 e59b  ................
+00000470: bee7 8987 e79a 84e9 97ae e9a2 980a 2d20  ..............- 
+00000480: e4bb 8ee6 98be e7a4 bae7 94a8 e688 b7e8  ................
+00000490: b4a6 e58f b7e7 bb91 e5ae 9ae7 9a84 e689  ................
+000004a0: 8be6 9cba e58f b7e6 94b9 e4b8 bae6 98be  ................
+000004b0: e7a4 bae8 b4a6 e58f b7e7 9a84 e7b1 b3e6  ................
+000004c0: b8b8 e7a4 be49 440a 2d20 e8ae bee7 bdae  .....ID.- ......
+000004d0: e380 81e5 8591 e68d a2e8 aea1 e588 92e5  ................
+000004e0: 8a9f e883 bde6 94af e68c 81e7 bea4 e881  ................
+000004f0: 8ae4 bdbf e794 a80a 2d20 e799 bbe9 9986  ........- ......
+00000500: e7bb 91e5 ae9a e58f aae9 9c80 e8a6 81e8  ................
+00000510: bf9b e8a1 8ce4 b880 e6ac a1e7 9fad e4bf  ................
+00000520: a1e9 aa8c e8af 810a 2d20 e794 a8e6 88b7  ........- ......
+00000530: e695 b0e6 8dae e696 87e4 bbb6 e380 81e6  ................
+00000540: 8f92 e4bb b6e9 858d e7bd aee6 9687 e4bb  ................
+00000550: b620 2a2a e6a0 bce5 bc8f e69b b4e6 96b0  . **............
+00000560: efbc 8ce4 b88e 2076 312e 302e 3020 e4b9  ...... v1.0.0 ..
+00000570: 8be5 898d e79a 84e7 8988 e69c ace4 b88d  ................
+00000580: e585 bce5 aeb9 2a2a 0a2d 20e4 bfae e5a4  ......**.- .....
+00000590: 8de6 b7bb e58a a0e5 8591 e68d a2e4 bbbb  ................
+000005a0: e58a a1e6 97b6 e587 bae7 8eb0 e79a 8455  ...............U
+000005b0: 4944 e4b8 8de5 ad98 e59c a8e9 9499 e8af  ID..............
+000005c0: af0a 2d20 e4bf aee5 a48d e595 86e5 9381  ..- ............
+000005d0: e59b bee7 8987 e794 9fe6 8890 e5ae 8ce6  ................
+000005e0: 898d e58f 91e5 87ba e590 8ee5 8fb0 e6ad  ................
+000005f0: a3e5 9ca8 e794 9fe6 8890 e68f 90e7 a4ba  ................
+00000600: e79a 84e9 97ae e9a2 980a 2d20 e5bc 82e5  ..........- ....
+00000610: b8b8 e68d 95e8 8eb7 e69b b4e5 8aa0 e587  ................
+00000620: 86e7 a1ae 0a2d 20e6 94b9 e8bf 9be4 ba86  .....- .........
+00000630: e4b8 80e4 ba9b e696 87e6 9cac 0a0a 2323  ..............##
+00000640: 2323 2032 3032 332e 352e 3138 0a2d 20e5  ## 2023.5.18.- .
+00000650: a49a e8bf 9be7 a88b e794 9fe6 8890 e595  ................
+00000660: 86e5 9381 e59b bee7 8987 efbc 88e5 a49a  ................
+00000670: e6a0 b8ef bc89 efbc 8ce5 8aa0 e5bf abe5  ................
+00000680: 9bbe e789 87e7 949f e688 90e9 809f e5ba  ................
+00000690: a60a 2d20 e4bf aee5 a48d e983 a8e5 8886  ..- ............
+000006a0: e595 86e5 9381 e585 91e6 8da2 e697 b6e9  ................
+000006b0: 97b4 e994 99e8 afaf e79a 84e9 97ae e9a2  ................
+000006c0: 98ef bc88 e5a6 82e7 b1b3 e6b8 b8e7 a4be  ................
+000006d0: e595 86e5 9381 e699 9ae4 ba86 e4b8 80e5  ................
+000006e0: 91a8 efbc 890a 0a23 2323 2320 3230 3233  .......#### 2023
+000006f0: 2e35 2e34 0a2d 20e5 a29e e58a a0e5 afb9  .5.4.- .........
+00000700: e698 9fe7 a9b9 e993 81e9 8193 e79a 84e7  ................
+00000710: adbe e588 b0e5 8a9f e883 bde7 9a84 e694  ................
+00000720: afe6 8c81 202d 205b 2338 395d 2868 7474  .... - [#89](htt
+00000730: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000740: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000750: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000760: 7075 6c6c 2f38 3929 2062 7920 4061 7961  pull/89) by @aya
+00000770: 6b61 7375 6b69 0a2d 20e4 bfae e5a4 8de6  kasuki.- .......
+00000780: 8f92 e4bb b6e5 91bd e4bb a4e4 bc98 e585  ................
+00000790: 88e5 baa6 e997 aee9 a298 202d 205b 2338  .......... - [#8
+000007a0: 385d 2868 7474 7073 3a2f 2f67 6974 6875  8](https://githu
+000007b0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000007c0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+000007d0: 7374 6f6f 6c2f 7075 6c6c 2f38 3829 2062  stool/pull/88) b
+000007e0: 7920 4061 7961 6b61 7375 6b69 0a2d 20e9  y @ayakasuki.- .
+000007f0: 83a8 e588 86e6 9687 e69c ace9 9499 e8af  ................
+00000800: afe4 bfae e6ad a320 2d20 5b23 3930 5d28  ....... - [#90](
+00000810: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000820: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000830: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000840: 6f6c 2f70 756c 6c2f 3930 2920 6279 2040  ol/pull/90) by @
+00000850: 626c 6163 6b2d 7a65 726f 3335 380a 0a2e  black-zero358...
+00000860: 2e2e 0a0a 2323 2323 2032 3032 332e 332e  ....#### 2023.3.
+00000870: 3330 0a2d 20e4 bfae e5a4 8d20 602f e585  30.- ...... `/..
+00000880: 91e6 8da2 6020 e591 bde4 bba4 e58f afe8  ....` ..........
+00000890: 83bd e4b8 8ee5 85b6 e4bb 96e6 8f92 e4bb  ................
+000008a0: b6e5 91bd e4bb a4e5 86b2 e7aa 81e7 9a84  ................
+000008b0: e997 aee9 a298 efbc 8ce5 908c e697 b620  ............... 
+000008c0: 5bf0 9f94 97e7 94a8 e6b3 95e5 8f98 e69b  [...............
+000008d0: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+000008e0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000008f0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000900: 7374 6f6f 6c2f 7769 6b69 2f49 6e66 6f72  stool/wiki/Infor
+00000910: 6d61 7469 6f6e 2d45 7863 6861 6e67 6523  mation-Exchange#
+00000920: e5a2 9ee5 8aa0 e588 a0e9 99a4 e585 91e6  ................
+00000930: 8da2 e8ae a1e5 8892 290a 2d20 2e2e 2e0a  ........).- ....
+00000940: 0a23 2320 e58a 9fe8 83bd e592 8ce7 89b9  .## ............
+00000950: e680 a70a 0a2d 20e7 9fad e4bf a1e9 aa8c  .....- .........
+00000960: e8af 81e7 99bb e5bd 95ef bc8c e585 8de6  ................
+00000970: 8a93 e58c 85e8 8eb7 e58f 9620 436f 6f6b  ........... Cook
+00000980: 6965 0a2d 20e8 87aa e58a a8e5 ae8c e688  ie.- ...........
+00000990: 90e6 af8f e697 a5e7 b1b3 e6b8 b8e5 b881  ................
+000009a0: e4bb bbe5 8aa1 0a2d 20e8 87aa e58a a8e8  .......- .......
+000009b0: bf9b e8a1 8ce6 b8b8 e688 8fe7 adbe e588  ................
+000009c0: b00a 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3  ..- ............
+000009d0: e6b8 b8e5 b881 e595 86e5 9381 e585 91e6  ................
+000009e0: 8da2 e8ae a1e5 8892 efbc 8ce5 88b0 e782  ................
+000009f0: b9e5 8591 e68d a20a 2d20 e58f afe6 94af  ........- ......
+00000a00: e68c 81e5 a49a e4b8 aa20 5151 20e8 b4a6  ......... QQ ...
+00000a10: e58f b7ef bc8c e6af 8fe4 b8aa 2051 5120  ............ QQ 
+00000a20: e8b4 a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5  ................
+00000a30: a49a e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4  ................
+00000a40: a6e6 88b7 0a2d 2051 5120 e68e a8e9 8081  .....- QQ ......
+00000a50: e689 a7e8 a18c e7bb 93e6 9e9c e980 9ae7  ................
+00000a60: 9fa5 0a2d 20e5 8e9f e7a5 9ee6 a091 e884  ...- ...........
+00000a70: 82e3 8081 e6b4 9ee5 a4a9 e5ae 9de9 92b1  ................
+00000a80: e380 81e8 b4a8 e987 8fe5 8f82 e58f 98e4  ................
+00000a90: bbaa e5b7 b2e6 bba1 e697 b6e6 8ea8 e980  ................
+00000aa0: 81e9 809a e79f a50a 0a23 2320 e4bd bfe7  .........## ....
+00000ab0: 94a8 e8af b4e6 988e 0a0a 2323 2320 f09f  ..........### ..
+00000ac0: 9ba0 efb8 8f20 4e6f 6e65 426f 7432 20e6  ..... NoneBot2 .
+00000ad0: 9cba e599 a8e4 baba e983 a8e7 bdb2 e592  ................
+00000ae0: 8ce6 8f92 e4bb b6e5 ae89 e8a3 850a 0ae8  ................
+00000af0: afb7 e69f a5e7 9c8b 202d 3e20 5bf0 9f94  ........ -> [...
+00000b00: 9749 6e73 7461 6c6c 6174 696f 6e5d 2868  .Installation](h
+00000b10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000b20: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
+00000b30: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
+00000b40: 6c2f 7769 6b69 2f49 6e73 7461 6c6c 6174  l/wiki/Installat
+00000b50: 696f 6e29 0a0a 2323 2320 f09f 9396 20e6  ion)..### .... .
+00000b60: 8f92 e4bb b6e5 85b7 e4bd 93e4 bdbf e794  ................
+00000b70: a8e8 afb4 e698 8e0a 0ae8 afb7 e69f a5e7  ................
+00000b80: 9c8b 202d 3e20 5bf0 9f94 9757 696b 6920  .. -> [....Wiki 
+00000b90: e696 87e6 a1a3 5d28 6874 7470 733a 2f2f  ......](https://
+00000ba0: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000bb0: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000bc0: 696e 2d6d 7973 746f 6f6c 2f77 696b 6929  in-mystool/wiki)
+00000bd0: 0a0a 2323 2320 e29d 9320 e88e b7e5 8f96  ..### ... ......
+00000be0: e68f 92e4 bbb6 e5b8 aee5 8aa9 e4bf a1e6  ................
+00000bf0: 81af 0a0a 2323 2323 20e6 8f92 e4bb b6e5  ....#### .......
+00000c00: 91bd e4bb a40a 0a60 6060 0a2f e5b8 aee5  .......```./....
+00000c10: 8aa9 0a60 6060 0a0a 3e20 e29a a0ef b88f  ...```..> ......
+00000c20: 20e6 b3a8 e684 8f20 e6ad a4e5 a484 e6b2   ...... ........
+00000c30: a1e6 9c89 e4bd bfe7 94a8 205b f09f 9497  .......... [....
+00000c40: 20e6 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4   ...............
+00000c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000c60: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000c70: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000c80: 746f 6f6c 2f77 696b 692f 436f 6e66 6967  tool/wiki/Config
+00000c90: 7572 6174 696f 6e2d 436f 6e66 6967 2363  uration-Config#c
+00000ca0: 6f6d 6d61 6e64 7374 6172 7429 0a0a 2323  ommandstart)..##
+00000cb0: 20e5 85b6 e4bb 960a 0a23 2323 205b f09f   ........### [..
+00000cc0: 9383 e6ba 90e7 a081 e8af b4e6 988e 5d28  ..............](
+00000cd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ce0: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000cf0: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000d00: 6f6c 2f77 696b 692f 536f 7572 6365 2d53  ol/wiki/Source-S
+00000d10: 7472 7563 7475 7265 290a 2323 2320 e980  tructure).### ..
+00000d20: 82e9 858d 205b e7bb aae5 b1b1 e79c 9fe5  .... [..........
+00000d30: afbb 426f 745d 2868 7474 7073 3a2f 2f67  ..Bot](https://g
+00000d40: 6974 6875 622e 636f 6d2f 4869 6269 4b69  ithub.com/HibiKi
+00000d50: 6572 2f7a 6865 6e78 756e 5f62 6f74 2920  er/zhenxun_bot) 
+00000d60: e79a 84e5 8886 e694 af0a 2d20 6874 7470  ..........- http
+00000d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+00000d80: 5754 4a43 2f7a 6865 6e78 756e 2d70 6c75  WTJC/zhenxun-plu
+00000d90: 6769 6e2d 6d79 7374 6f6f 6c0a 2d20 6874  gin-mystool.- ht
+00000da0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000db0: 2f61 7961 6b61 7375 6b69 2f6e 6f6e 6562  /ayakasuki/noneb
+00000dc0: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
+00000dd0: 6c0a                                     l.
```

### Comparing `nonebot_plugin_mystool-0.2.9/pyproject.toml` & `nonebot_plugin_mystool-1.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v0.2.9"
+version = "v1.0.0-beta.1"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
@@ -20,19 +20,19 @@
 ]
 packages = [
     { include = "nonebot_plugin_mystool", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-httpx = "^0.24.0"
+httpx = "^0.24.1"
 nonebot_plugin_apscheduler = ">=0.2.0"
 ntplib = "^0.4.0"
 Pillow = "^9.5.0"
-requests = "^2.30.0"
+requests = "^2.31.0"
 nonebot_adapter_onebot = "^2.2.3"
 tenacity = "^8.2.2"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues"
 
 [build-system]
```

### Comparing `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchangePlan.py` & `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/exchange.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,96 +2,47 @@
 ### 米游社商品兑换前端以及计划任务相关
 """
 import asyncio
 import io
 import os
 import threading
 import time
-from copy import deepcopy
 from datetime import datetime
 from multiprocessing import Manager
 from multiprocessing.pool import Pool
 from multiprocessing.synchronize import Lock
-from typing import List, Set, Union, Callable, Any
+from typing import List, Union, Callable, Any, Tuple, Optional, Dict
 
-from nonebot import get_bot, on_command
+from apscheduler.events import JobExecutionEvent, EVENT_JOB_EXECUTED
+from nonebot import on_command, get_bot
 from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
                                          PrivateMessageEvent, GroupMessageEvent)
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
 from nonebot_plugin_apscheduler import scheduler
 
-from .bbsAPI import get_game_record
-from .config import config as conf
-from .data import UserData
-from .exchange import (Exchange, Good, UserAccount, get_good_detail,
-                       get_good_list, game_list_to_image)
-from .gameSign import GameInfo
-from .utils import NtpTime, COMMAND_BEGIN, logger, driver, get_last_command_sep
-
-
-class ExchangeStart:
-    """
-    异步多线程兑换
-    """
-
-    def __init__(self, account: UserAccount, qq: int, exchange_plan: Exchange, thread: int) -> None:
-        self.plans: List[Exchange] = []
-        self.tasks: Set[asyncio.Task] = set()
-        self.finishedCount = 0
-        self.account = account
-        self.qq = qq
-
-        for _ in range(thread):
-            self.plans.append(deepcopy(exchange_plan))
-
-    async def start(self):
-        """
-        执行兑换
-        """
-        # 在后台启动兑换操作
-        for plan in self.plans:
-            self.tasks.add(asyncio.create_task(plan.start()))
-        # 等待兑换线程全部结束
-        for task in self.tasks:
-            await task
-
-        bot = get_bot()
-
-        success_tasks: List[asyncio.Task] = list(filter(lambda task: isinstance(
-            task.result(), tuple) and task.result()[0], self.tasks))
-        if success_tasks:
-            await bot.send_private_msg(
-                user_id=self.qq,
-                message=f"🎉用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换成功，可前往米游社查看")
-        else:
-            msg = f"⚠️用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换失败\n返回结果：\n"
-            num = 0
-            for task in self.tasks:
-                num += 1
-                msg += f"{num}: "
-                if isinstance(task.result(), tuple):
-                    msg += str(task.result()[1])
-                else:
-                    msg += f"异常，程序返回结果为 {task.result()}"
-                msg += "\n"
-            await bot.send_private_msg(user_id=self.qq, message=msg)
-        for plan in self.account.exchange:
-            if plan == (self.plans[0].goodID, self.plans[0].gameUID):
-                self.account.exchange.remove(plan)
-        UserData.set_account(self.account, self.qq,
-                             self.account.phone)
-
-
-myb_exchange_plan = on_command(f"{conf.COMMAND_START}兑换",
-                               aliases={(f"{conf.COMMAND_START}兑换", "+"), (f"{conf.COMMAND_START}兑换", "-")},
+from .data_model import Good, GameRecord, ExchangeStatus
+from .good_image import game_list_to_image
+from .plugin_data import PluginDataManager, write_plugin_data
+from .simple_api import get_game_record, get_good_detail, get_good_list, good_exchange_sync
+from .user_data import UserAccount, ExchangePlan, ExchangeResult
+from .utils import NtpTime, COMMAND_BEGIN, logger, _driver, get_last_command_sep
+
+_conf = PluginDataManager.plugin_data_obj
+
+myb_exchange_plan = on_command(f"{_conf.preference.command_start}兑换",
+                               aliases={(f"{_conf.preference.command_start}兑换", "+"),
+                                        (f"{_conf.preference.command_start}兑换", "-")},
                                priority=5, block=True)
 myb_exchange_plan.name = "兑换"
-myb_exchange_plan.usage = f"跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，并使用『{COMMAND_BEGIN}地址』选择你要使用的地址。所需的商品ID可通过命令『{COMMAND_BEGIN}商品』获取。注意，不限兑换时间的商品将不会在此处显示。 "
+myb_exchange_plan.usage = "跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，" \
+                          "并使用『{HEAD}地址』选择你要使用的地址。" \
+                          "所需的商品ID可通过命令『{HEAD}商品』获取。" \
+                          "注意，不限兑换时间的商品将不会在此处显示。 "
 myb_exchange_plan.extra_usage = """\
 具体用法：
 {HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
 {HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
 {HEAD}商品 ➢ 查看米游社商品
 『{SEP}』为分隔符，使用NoneBot配置中的其他分隔符亦可\
 """
@@ -116,339 +67,401 @@
                 '⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
                                                                                         SEP=get_last_command_sep()))
         elif not str(command_arg).isdigit():
             await matcher.reject(
                 '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
                                                                                  SEP=get_last_command_sep()))
 
-    if isinstance(event, GroupMessageEvent):
-        await matcher.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行操作")
-    qq_account = int(event.user_id)
-    user_account = UserData.read_account_all(qq_account)
+    user = _conf.users.get(event.user_id)
+    user_account = user.accounts if user else None
     if not user_account:
-        await matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}{conf.COMMAND_START}登录』进行登录")
-    state['qq_account'] = qq_account
-    state['user_account'] = user_account
+        await matcher.finish(
+            f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}登录』进行登录")
 
     # 如果使用了二级命令 + - 则跳转进下一步，通过phone选择账户进行设置
     if len(command) > 1:
         state['command_2'] = command[1]
         matcher.set_arg("good_id", command_arg)
         if len(user_account) == 1:
-            matcher.set_arg('phone', Message(str(user_account[0].phone)))
+            uid = next(iter(user_account.values())).bbs_uid
+            matcher.set_arg('bbs_uid', Message(uid))
         else:
-            phones = [str(user_account[i].phone)
-                      for i in range(len(user_account))]
+            uids = map(lambda x: x.bbs_uid, user_account.values())
             msg = "您有多个账号，您要配置以下哪个账号的兑换计划？\n"
-            msg += "📱" + "\n📱".join(phones)
+            msg += "\n".join(map(lambda x: f"🆔{x}", uids))
             msg += "\n🚪发送“退出”即可退出"
             await matcher.send(msg)
     # 如果未使用二级命令，则进行查询操作，并结束交互
     else:
         msg = ""
-        for account in user_account:
-            for plan in account.exchange:
-                good = await get_good_detail(plan[0])
-                if not good:
-                    await matcher.finish("⚠️获取商品详情失败，请稍后再试")
-                msg += f"""\
-                \n-- 商品 {good.name}\
-                \n- 🔢商品ID：{good.good_id}\
-                \n- 💰商品价格：{good.price} 米游币\
-                \n- 📅兑换时间：{time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))}\
-                \n- 📱账户：{account.phone}""".strip()
-                msg += "\n\n"
+        for plan in user.exchange_plans:
+            good_detail_status, good = await get_good_detail(plan.good)
+            if not good_detail_status:
+                await matcher.finish("⚠️获取商品详情失败，请稍后再试")
+            msg += f"-- 商品：{good.general_name}" \
+                   f"\n- 🔢商品ID：{good.goods_id}" \
+                   f"\n- 💰商品价格：{good.price} 米游币" \
+                   f"\n- 📅兑换时间：{good.time_text}" \
+                   f"\n- 🆔账户：{plan.account.bbs_uid}"
+            msg += "\n\n"
         if not msg:
             msg = '您还没有兑换计划哦~\n\n'
         await matcher.finish(msg + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
 
 
-@myb_exchange_plan.got('phone')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, phone=ArgStr('phone')):
+@myb_exchange_plan.got('bbs_uid')
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
+            uid=ArgStr('bbs_uid')):
     """
     请求用户输入手机号以对账户设置兑换计划
     """
-    user_account: List[UserAccount] = state['user_account']
-
-    if phone == '退出':
+    user_account = _conf.users[event.user_id].accounts
+    if uid == '退出':
         await matcher.finish('🚪已成功退出')
-    try:
-        state["account"] = list(
-            filter(lambda account: account.phone == int(phone), user_account))[0]
-    except IndexError:
+    if uid in user_account:
+        state["account"] = user_account[uid]
+    else:
         await matcher.reject('⚠️您发送的账号不在以上账号内，请重新发送')
-    except ValueError:
-        await matcher.reject('⚠️您发送的账号不是手机号，请重新发送')
 
 
 @myb_exchange_plan.got('good_id')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, good_id=ArgPlainText('good_id')):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
+            good_id=ArgPlainText('good_id')):
     """
     处理三级命令，即商品ID
     """
     account: UserAccount = state['account']
     command_2 = state['command_2']
     if command_2 == '+':
         good_dict = {
-            'bh3': await get_good_list('bh3'),
-            'ys': await get_good_list('ys'),
-            'bh2': await get_good_list('bh2'),
-            'xq': await get_good_list('xq'),
-            'wd': await get_good_list('wd'),
-            'bbs': await get_good_list('bbs')
+            'bh3': (await get_good_list('bh3'))[1],
+            'ys': (await get_good_list('hk4e'))[1],
+            'bh2': (await get_good_list('bh2'))[1],
+            'xq': (await get_good_list('hkrpg'))[1],
+            'wd': (await get_good_list('nxx'))[1],
+            'bbs': (await get_good_list('bbs'))[1]
         }
         flag = True
         break_flag = False
         good = None
-        game = None
-        for game, good_list in good_dict.items():
-            for good in good_list:
-                if good.good_id == good_id:
+        for good_list in good_dict.values():
+            goods_on_sell = filter(lambda x: not x.time_end and x.time_limited, good_list)
+            for good in goods_on_sell:
+                if good.goods_id == good_id:
                     flag = False
                     break_flag = True
                     break
             if break_flag:
                 break
         if flag:
             await matcher.finish('⚠️您发送的商品ID不在可兑换的商品列表内，程序已退出')
         state['good'] = good
-        uids = []
         if good.time:
             # 若为实物商品，也进入下一步骤，但是传入uid为None
-            if good.is_visual:
-                game_records = await get_game_record(account)
+            if good.is_virtual:
+                game_records_status, records = await get_game_record(account)
 
-                if isinstance(game_records, int):
-                    pass
-                else:
-                    game_name = list(filter(lambda abbr: abbr[0] == game, GameInfo.ABBR_TO_ID.values()))[0][1]
-                    msg = f'您米游社账户下的『{game_name}』账号：'
-                    for record in game_records:
-                        if GameInfo.ABBR_TO_ID[record.game_id][0] == game:
-                            msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.uid}'
-                        uids.append(record.uid)
-                    if uids:
-                        await matcher.send("您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
-                        await asyncio.sleep(0.5)
-                        await matcher.send(msg)
+                if game_records_status:
+                    if len(records) == 0:
+                        matcher.set_arg('uid', Message(records[0].game_role_id))
                     else:
-                        await matcher.finish(
-                            f"您还没有绑定『{game_name}』账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
+                        msg = f'您米游社账户下的游戏账号：'
+                        for record in records:
+                            msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.game_role_id}'
+                        if records:
+                            state['records'] = records
+                            await matcher.send(
+                                "您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
+                            await asyncio.sleep(0.5)
+                            await matcher.send(msg)
+                        else:
+                            await matcher.finish(
+                                f"您的米游社账户下还没有绑定游戏账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
             else:
                 if not account.address:
                     await matcher.finish('⚠️您还没有配置地址哦，请先配置地址')
-            state['uids'] = uids
-            matcher.set_arg('uid', Message())
+                matcher.set_arg('uid', Message())
         else:
             await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
 
     elif command_2 == '-':
-        if account.exchange:
-            for exchange_good in account.exchange:
-                if exchange_good[0] == good_id:
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, event.user_id, account.phone)
-                    scheduler.remove_job(job_id=str(
-                        account.phone) + '_' + good_id)
+        plans = _conf.users[event.user_id].exchange_plans
+        if plans:
+            for plan in plans:
+                if plan.good.goods_id == good_id:
+                    plans.remove(plan)
+                    write_plugin_data()
+                    for i in range(_conf.preference.exchange_thread_count):
+                        scheduler.remove_job(job_id=f"exchange-plan-{hash(plan)}-{i}")
                     await matcher.finish('兑换计划删除成功')
             await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
         else:
             await matcher.finish("您还没有配置兑换计划哦~")
 
     else:
         await matcher.reject(
             '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
                                                                          SEP=get_last_command_sep()))
 
 
 @myb_exchange_plan.got('uid')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, uid=ArgPlainText('uid')):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State,
+            uid=ArgPlainText('uid')):
     """
     初始化商品兑换任务，如果传入UID为None则为实物商品，仍可继续
     """
+    user = _conf.users[event.user_id]
     account: UserAccount = state['account']
     good: Good = state['good']
-    uids: List[str] = state['uids']
-    if good.is_visual:
+    if good.is_virtual:
+        records: List[GameRecord] = state['records']
         if uid == '退出':
             await matcher.finish('🚪已成功退出')
-        if uid not in uids:
+        record_filter = filter(lambda x: x.game_role_id == uid, records)
+        record = next(record_filter, None)
+        if not record:
             await matcher.reject('⚠️您输入的UID不在上述账号内，请重新输入')
-
-    if (good.good_id, uid) in account.exchange:
+        plan = ExchangePlan(good=good, address=account.address, game_record=record, account=account)
+    else:
+        plan = ExchangePlan(good=good, address=account.address, account=account)
+    if plan in user.exchange_plans:
         await matcher.finish('⚠️您已经配置过该商品的兑换哦！')
     else:
-        account.exchange.append((good.good_id, uid))
+        user.exchange_plans.add(plan)
+        write_plugin_data()
 
     # 初始化兑换任务
-    exchange_plan = await Exchange(account, good.good_id, uid).async_init()
-    if exchange_plan.result == -1:
-        await matcher.finish(f"⚠️账户 {account.phone} 登录失效，请重新登录")
-    elif exchange_plan.result == -2:
-        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于未配置stoken，放弃兑换")
-    elif exchange_plan.result == -3:
-        await matcher.finish(f"⚠️商品 {good.good_id} 为游戏内物品，由于stoken为\"v2\"类型，且未配置mid，放弃兑换")
-    elif exchange_plan.result == -4:
-        await matcher.finish(f"⚠️暂不支持商品 {good.good_id} 所属的游戏，放弃兑换")
-    elif exchange_plan.result == -5:
-        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，网络连接失败或服务器返回不正确，放弃兑换")
-    elif exchange_plan.result == -6:
-        await matcher.finish(f"⚠️获取商品 {good.good_id} 的信息时，获取用户游戏账户数据失败，放弃兑换")
-    else:
-        scheduler.add_job(id=str(account.phone) + '_' + good.good_id, replace_existing=True, trigger='date',
-                          func=ExchangeStart(
-                              account, event.user_id, exchange_plan, conf.EXCHANGE_THREAD).start,
-                          next_run_time=datetime.fromtimestamp(good.time))
-
-    UserData.set_account(account, event.user_id, account.phone)
+    finished.setdefault(plan, [])
+    for i in range(_conf.preference.exchange_thread_count):
+        scheduler.add_job(
+            good_exchange_sync,
+            "date",
+            id=f"exchange-plan-{hash(plan)}-{i}",
+            replace_existing=True,
+            args=(plan,),
+            run_date=datetime.fromtimestamp(good.time),
+            max_instances=_conf.preference.exchange_thread_count
+        )
 
     await matcher.finish(
-        f'🎉设置兑换计划成功！将于 {time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(good.time))} 开始兑换，到时将会私聊告知您兑换结果')
+        f'🎉设置兑换计划成功！将于 {plan.good.time_text} 开始兑换，到时将会私聊告知您兑换结果')
 
 
-get_good_image = on_command(conf.COMMAND_START + '商品', priority=5, block=True)
+get_good_image = on_command(_conf.preference.command_start + '商品', priority=5, block=True)
 get_good_image.name = "商品"
 get_good_image.usage = "获取当日米游币商品信息。添加自动兑换计划需要商品ID，请记下您要兑换的商品的ID。"
 
 
 @get_good_image.handle()
 async def _(_: MessageEvent, matcher: Matcher, arg=CommandArg()):
     # 若有使用二级命令，即传入了想要查看的商品类别，则跳过询问
     if arg:
         matcher.set_arg("content", arg)
 
 
-@get_good_image.got("content", prompt="""\
-        \n请发送您要查看的商品类别:\
-        \n- 崩坏3\
-        \n- 原神\
-        \n- 崩坏2\
-        \n- 崩坏：星穹铁道\
-        \n- 未定事件簿\
-        \n- 米游社\
-        \n若是商品图片与米游社商品不符或报错 请发送“更新”哦~\
-        \n—— 🚪发送“退出”以结束""".strip())
+@get_good_image.got("content", prompt="请发送您要查看的商品类别:"
+                                      "\n- 崩坏3"
+                                      "\n- 原神"
+                                      "\n- 崩坏2"
+                                      "\n- 崩坏：星穹铁道"
+                                      "\n- 未定事件簿"
+                                      "\n- 米游社"
+                                      "\n若是商品图片与米游社商品不符或报错 请发送“更新”哦~"
+                                      "\n—— 🚪发送“退出”以结束")
 async def _(_: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
     """
     根据传入的商品类别，发送对应的商品列表图片
     """
     if arg == '退出':
         await matcher.finish('🚪已成功退出')
     elif arg in ['原神', 'ys']:
-        arg = ('ys', '原神')
+        arg = ('hk4e', '原神')
     elif arg in ['崩坏3', '崩坏三', '崩3', '崩三', '崩崩崩', '蹦蹦蹦', 'bh3']:
         arg = ('bh3', '崩坏3')
     elif arg in ['崩坏2', '崩坏二', '崩2', '崩二', '崩崩', '蹦蹦', 'bh2']:
         arg = ('bh2', '崩坏2')
     elif arg in ['崩坏：星穹铁道', '星铁', '星穹铁道', '铁道', '轨子', '星穹', 'xq']:
-        arg = ('xq', '崩坏：星穹铁道')
+        arg = ('hkrpg', '崩坏：星穹铁道')
     elif arg in ['未定', '未定事件簿', 'wd']:
-        arg = ('wd', '未定事件簿')
+        arg = ('nxx', '未定事件簿')
     elif arg in ['大别野', '米游社']:
         arg = ('bbs', '米游社')
     elif arg == '更新':
-        threading.Thread(generate_image(is_auto=False)).start()
-        await get_good_image.finish('✔后台已生成商品信息图片')
+        threading.Thread(target=generate_image, kwargs={"is_auto": False}).start()
+        await get_good_image.finish('⏳后台正在生成商品信息图片，请稍后查询')
     else:
         await get_good_image.reject('⚠️您的输入有误，请重新输入')
-    good_list = await get_good_list(arg[0])
-    if good_list:
-        img_path = time.strftime(
-            f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
-        if os.path.exists(img_path):
-            with open(img_path, 'rb') as f:
-                image_bytes = io.BytesIO(f.read())
-            await get_good_image.finish(MessageSegment.image(image_bytes))
-        else:
-            threading.Thread(generate_image(is_auto=False)).start()
-            await get_good_image.finish('⏳后台正在生成商品信息图片，请稍后查询')
+
+    img_path = time.strftime(
+        f'{_conf.good_list_image_config.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
+    if os.path.exists(img_path):
+        with open(img_path, 'rb') as f:
+            image_bytes = io.BytesIO(f.read())
+        await get_good_image.finish(MessageSegment.image(image_bytes))
     else:
-        await get_good_image.finish(f"{arg[1]} 部分目前没有可兑换商品哦~")
+        await get_good_image.finish(
+            f'{arg[1]} 分区暂时没有可兑换的限时商品。如果这与实际不符，你可以尝试用『{COMMAND_BEGIN}商品 更新』进行更新。')
 
 
-@driver.on_startup
+lock = threading.Lock()
+finished: Dict[ExchangePlan, List[bool]] = {}
+
+
+@lambda func: scheduler.add_listener(func, EVENT_JOB_EXECUTED)
+def exchange_notice(event: JobExecutionEvent):
+    """
+    接收兑换结果
+    """
+    if event.job_id.startswith("exchange-plan"):
+        bot = get_bot()
+        loop = asyncio.get_event_loop()
+
+        thread_id = int(event.job_id.split('-')[-1]) + 1
+        result: Tuple[ExchangeStatus, Optional[ExchangeResult]] = event.retval
+        exchange_status, exchange_result = result
+
+        if not exchange_status:
+            hash_value = int(event.job_id.split('-')[-2])
+            plans = map(lambda x: x.exchange_plans, _conf.users.values())
+            plan_filter = filter(lambda x: hash(x[0]) == hash_value, zip(plans, _conf.users.keys()))
+            plan_tuple = next(plan_filter)
+            plan, user_id = plan_tuple
+            with lock:
+                finished[plan].append(False)
+                loop.create_task(
+                    bot.send_private_msg(
+                        user_id=user_id,
+                        message=f"⚠️账户 {plan.account.bbs_uid}"
+                                f"\n- {plan.good.general_name}"
+                                f"\n- 线程 {thread_id}"
+                                f"\n- 兑换请求发送失败"
+                    )
+                )
+                if len(finished[plan]) == _conf.preference.exchange_thread_count:
+                    del plan
+                    write_plugin_data()
+
+        else:
+            plan = exchange_result.plan
+            user_filter = filter(lambda x: plan in x[1].exchange_plans, _conf.users.items())
+            user_id, user = next(user_filter)
+            with lock:
+                # 如果已经有一个线程兑换成功，就不再接收结果
+                if True not in finished[plan]:
+                    if exchange_result.result:
+                        finished[plan].append(True)
+                        loop.create_task(
+                            bot.send_private_msg(
+                                user_id=user_id,
+                                message=f"🎉账户 {plan.account.bbs_uid}"
+                                        f"\n- {plan.good.general_name}"
+                                        f"\n- 线程 {thread_id}"
+                                        f"\n- 兑换成功"
+                            )
+                        )
+                    else:
+                        finished[plan].append(False)
+                        loop.create_task(
+                            bot.send_private_msg(
+                                user_id=user_id,
+                                message=f"💦账户 {plan.account.bbs_uid}"
+                                        f"\n- {plan.good.general_name}"
+                                        f"\n- 线程 {thread_id}"
+                                        f"\n- 兑换失败"
+                            )
+                        )
+
+                if len(finished[plan]) == _conf.preference.exchange_thread_count:
+                    try:
+                        user.exchange_plans.remove(plan)
+                    except KeyError:
+                        pass
+                    else:
+                        write_plugin_data()
+
+
+@_driver.on_startup
 async def _():
     """
     启动机器人时自动初始化兑换任务
     """
-    all_accounts = UserData.read_all()
-    for qq in all_accounts.keys():
-        qq = int(qq)
-        accounts = UserData.read_account_all(qq)
-        for account in accounts:
-            exchange_list = account.exchange
-            for exchange_good in exchange_list:
-                good_detail = await get_good_detail(exchange_good[0])
-                if good_detail == -1:
-                    # 若商品不存在则删除
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                    continue
-                if not good_detail.time:
-                    # 若商品已下架则删除
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                    continue
-                if good_detail.time < NtpTime.time():
-                    # 若重启时兑换超时则删除该兑换
-                    account.exchange.remove(exchange_good)
-                    UserData.set_account(account, qq, account.phone)
-                else:
-                    exchange_plan = await Exchange(account, exchange_good[0], exchange_good[1]).async_init()
-                    scheduler.add_job(id=str(account.phone) + '_' + exchange_good[0], replace_existing=True,
-                                      trigger='date', func=ExchangeStart(
-                            account, qq, exchange_plan, conf.EXCHANGE_THREAD).start,
-                                      next_run_time=datetime.fromtimestamp(good_detail.time))
+    for user_id, user in _conf.users.items():
+        plans = user.exchange_plans
+        for plan in plans:
+            good_detail_status, good = await get_good_detail(plan.good)
+            if good_detail_status.good_not_existed or good.time < NtpTime.time():
+                # 若商品不存在则删除
+                # 若重启时兑换超时则删除该兑换
+                user.exchange_plans.remove(plan)
+                write_plugin_data()
+                continue
+            else:
+                finished.setdefault(plan, [])
+                for i in range(_conf.preference.exchange_thread_count):
+                    scheduler.add_job(
+                        good_exchange_sync,
+                        "date",
+                        id=f"exchange-plan-{hash(plan)}-{i}",
+                        replace_existing=True,
+                        args=(plan,),
+                        run_date=datetime.fromtimestamp(good.time),
+                        max_instances=_conf.preference.exchange_thread_count
+                    )
 
 
 def image_process(game: str, lock: Lock):
     """
     生成并保存图片的进程函数
 
     :param game: 游戏名
     :param lock: 进程锁
     :return: 生成成功或无商品返回True，否则返回False
     """
     loop = asyncio.new_event_loop()
-    good_list = loop.run_until_complete(get_good_list(game))
+    good_list_status, good_list = loop.run_until_complete(get_good_list(game))
+    if not good_list_status:
+        logger.error(f"{_conf.preference.log_head}获取 {game} 分区的商品列表失败，跳过该分区的商品图片生成")
+        return False
+    good_list = list(filter(lambda x: not x.time_end and x.time_limited, good_list))
     if good_list:
-        logger.info(f"{conf.LOG_HEAD}正在生成 {game} 分区的商品列表图片")
+        logger.info(f"{_conf.preference.log_head}正在生成 {game} 分区的商品列表图片")
         image_bytes = loop.run_until_complete(game_list_to_image(good_list, lock))
         if not image_bytes:
             return False
         date = time.strftime('%m-%d', time.localtime())
-        path = conf.goodListImage.SAVE_PATH / f"{date}-{game}.jpg"
+        path = _conf.good_list_image_config.SAVE_PATH / f"{date}-{game}.jpg"
         with open(path, 'wb') as f:
             f.write(image_bytes)
-        logger.info(f"{conf.LOG_HEAD}已完成 {game} 分区的商品列表图片生成")
+        logger.info(f"{_conf.preference.log_head}已完成 {game} 分区的商品列表图片生成")
     else:
-        logger.info(f"{conf.LOG_HEAD}{game}分区暂时没有商品，跳过生成商品列表图片")
+        logger.info(f"{_conf.preference.log_head}{game}分区暂时没有可兑换的限时商品，跳过该分区的商品图片生成")
     return True
 
 
 def generate_image(is_auto=True, callback: Callable[[bool], Any] = None):
     """
     生成米游币商品信息图片。该函数会阻塞当前线程
 
     :param is_auto: True为每日自动生成，False为用户手动更新
     :param callback: 回调函数，参数为生成成功与否
-    >>> generate_image(is_auto=False)
     """
-    for root, _, files in os.walk(conf.goodListImage.SAVE_PATH, topdown=False):
+    for root, _, files in os.walk(_conf.good_list_image_config.SAVE_PATH, topdown=False):
         for name in files:
             date = time.strftime('%m-%d', time.localtime())
             # 若图片开头为当日日期，则退出函数不执行
             if name.startswith(date):
                 if is_auto:
                     return
             # 删除旧图片
             if name.endswith('.jpg'):
                 os.remove(os.path.join(root, name))
 
     lock: Lock = Manager().Lock()
     with Pool() as pool:
-        for game in "bh3", "ys", "bh2", "xq", "wd", "bbs":
+        for game in "bh3", "hk4e", "bh2", "hkrpg", "nxx", "bbs":
             pool.apply_async(image_process,
                              args=(game, lock),
                              callback=callback)
         pool.close()
         pool.join()
+
+    logger.info(f"{_conf.preference.log_head}已完成所有分区的商品列表图片生成")
```

### Comparing `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/help.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 """
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, CommandArg
 
-from .config import config as conf
+from .plugin_data import PluginDataManager
 from .utils import PLUGIN, COMMAND_BEGIN
 
-helper = on_command(conf.COMMAND_START + "help",
+_conf = PluginDataManager.plugin_data_obj
+
+helper = on_command(_conf.preference.command_start + "help",
                     priority=1,
-                    aliases={conf.COMMAND_START + "帮助"},
+                    aliases={_conf.preference.command_start + "帮助"},
                     block=True)
 
 helper.name = '帮助'
 helper.usage = '''\
     🍺欢迎使用米游社小助手帮助系统！\
     \n{HEAD}帮助 ➢ 查看米游社小助手使用说明\
     \n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明\
```

### Comparing `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/mybMission.py` & `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/myb_missions_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,535 +1,498 @@
 """
-### 米游币任务相关
+### 米游社的米游币任务相关API
 """
 import asyncio
-import traceback
-from typing import Any, Dict, List, Literal, NewType, Tuple, Union, Optional
+from typing import List, Optional, Tuple, Set, Type
 
 import httpx
 import tenacity
 
-from .bbsAPI import device_login, device_save
-from .config import config as conf
-from .data import UserAccount
-from .utils import (Subscribe, check_ds, check_login, custom_attempt_times,
-                    generate_ds, logger)
+from .data_model import BaseApiStatus, MissionStatus, MissionData, \
+    MissionState
+from .plugin_data import PluginDataManager
+from .simple_api import ApiResultHandler, is_incorrect_return
+from .user_data import UserAccount
+from .utils import logger, generate_ds, \
+    get_async_retry
+
+_conf = PluginDataManager.plugin_data_obj
 
 URL_SIGN = "https://bbs-api.mihoyo.com/apihub/app/api/signIn"
 URL_GET_POST = "https://bbs-api.miyoushe.com/post/api/feeds/posts?fresh_action=1&gids={}&is_first_initialize=false" \
-               "&last_id= "
+               "&last_id="
 URL_READ = "https://bbs-api.miyoushe.com/post/api/getPostFull?post_id={}"
 URL_LIKE = "https://bbs-api.miyoushe.com/apihub/sapi/upvotePost"
 URL_SHARE = "https://bbs-api.miyoushe.com/apihub/api/getShareConf?entity_id={}&entity_type=1"
 URL_MISSION = "https://api-takumi.mihoyo.com/apihub/wapi/getMissions?point_sn=myb"
 URL_MISSION_STATE = "https://api-takumi.mihoyo.com/apihub/wapi/getUserMissionsState?point_sn=myb"
-HEADERS = {
+HEADERS_BASE = {
     "Host": "bbs-api.miyoushe.com",
     "Referer": "https://app.mihoyo.com",
-    'User-Agent': conf.device.USER_AGENT_ANDROID_OTHER,
-    "x-rpc-app_version": conf.device.X_RPC_APP_VERSION,
-    "x-rpc-channel": conf.device.X_RPC_CHANNEL_ANDROID,
+    'User-Agent': _conf.device_config.USER_AGENT_ANDROID_OTHER,
+    "x-rpc-app_version": _conf.device_config.X_RPC_APP_VERSION,
+    "x-rpc-channel": _conf.device_config.X_RPC_CHANNEL_ANDROID,
     "x-rpc-client_type": "2",
     "x-rpc-device_id": None,
-    "x-rpc-device_model": conf.device.X_RPC_DEVICE_MODEL_ANDROID,
-    "x-rpc-device_name": conf.device.X_RPC_DEVICE_NAME_ANDROID,
-    "x-rpc-sys_version": conf.device.X_RPC_SYS_VERSION_ANDROID,
+    "x-rpc-device_model": _conf.device_config.X_RPC_DEVICE_MODEL_ANDROID,
+    "x-rpc-device_name": _conf.device_config.X_RPC_DEVICE_NAME_ANDROID,
+    "x-rpc-sys_version": _conf.device_config.X_RPC_SYS_VERSION_ANDROID,
     "Accept-Encoding": "gzip",
     "Connection": "Keep-Alive",
     "DS": None
 }
 HEADERS_MISSION = {
     "Host": "api-takumi.mihoyo.com",
     "Origin": "https://webstatic.mihoyo.com",
     "Connection": "keep-alive",
     "Accept": "application/json, text/plain, */*",
-    "User-Agent": conf.device.USER_AGENT_MOBILE,
+    "User-Agent": _conf.device_config.USER_AGENT_MOBILE,
     "Accept-Language": "zh-CN,zh-Hans;q=0.9",
     "Referer": "https://webstatic.mihoyo.com/",
     "Accept-Encoding": "gzip, deflate, br"
 }
 HEADERS_GET_POSTS = {
     "Host": "bbs-api.miyoushe.com",
     "Accept": "*/*",
     "x-rpc-client_type": "1",
     "x-rpc-device_id": None,
-    "x-rpc-channel": conf.device.X_RPC_CHANNEL,
+    "x-rpc-channel": _conf.device_config.X_RPC_CHANNEL,
     "Accept-Language": "zh-CN,zh-Hans;q=0.9",
     "Accept-Encoding": "gzip, deflate, br",
-    "x-rpc-sys_version": conf.device.X_RPC_SYS_VERSION,
+    "x-rpc-sys_version": _conf.device_config.X_RPC_SYS_VERSION,
     "Referer": "https://app.mihoyo.com",
-    "x-rpc-device_name": conf.device.X_RPC_DEVICE_NAME_MOBILE,
-    "x-rpc-app_version": conf.device.X_RPC_APP_VERSION,
-    "User-Agent": conf.device.USER_AGENT_OTHER,
+    "x-rpc-device_name": _conf.device_config.X_RPC_DEVICE_NAME_MOBILE,
+    "x-rpc-app_version": _conf.device_config.X_RPC_APP_VERSION,
+    "User-Agent": _conf.device_config.USER_AGENT_OTHER,
     "Connection": "keep-alive"
 }
 
 # 旧的API
 HEADERS_OLD = {
     "Host": "bbs-api.mihoyo.com",
     "Referer": "https://app.mihoyo.com",
-    'User-Agent': conf.device.USER_AGENT_ANDROID_OTHER,
+    'User-Agent': _conf.device_config.USER_AGENT_ANDROID_OTHER,
     "x-rpc-app_version": "2.36.1",
-    "x-rpc-channel": conf.device.X_RPC_CHANNEL_ANDROID,
+    "x-rpc-channel": _conf.device_config.X_RPC_CHANNEL_ANDROID,
     "x-rpc-client_type": "2",
     "x-rpc-device_id": None,
-    "x-rpc-device_model": conf.device.X_RPC_DEVICE_MODEL_ANDROID,
-    "x-rpc-device_name": conf.device.X_RPC_DEVICE_NAME_ANDROID,
-    "x-rpc-sys_version": conf.device.X_RPC_SYS_VERSION_ANDROID,
+    "x-rpc-device_model": _conf.device_config.X_RPC_DEVICE_MODEL_ANDROID,
+    "x-rpc-device_name": _conf.device_config.X_RPC_DEVICE_NAME_ANDROID,
+    "x-rpc-sys_version": _conf.device_config.X_RPC_SYS_VERSION_ANDROID,
     "Accept-Encoding": "gzip",
     "Connection": "Keep-Alive",
     "DS": None
 }
 
 
-class GameID:
+class BaseMission:
     """
-    米游社任务所需的gid和fid
+    米游币任务基类
     """
+    NAME = ""
+    """米游社分区名字"""
+    GIDS = 0
+    FID = 0
 
-    def __init__(self, gids: int, fid: int):
-        self.gids: int = gids
-        self.fid: int = fid
-
-
-GAME_ID = {
-    "bbs": GameID(5, 0),
-    # TODO: bbs fid暂时未知
-    "bh3": GameID(1, 1),
-    "ys": GameID(2, 26),
-    "bh2": GameID(3, 30),
-    "wd": GameID(4, 37),
-    "xq": GameID(5, 52),
-}
-'''所有的gid和fid'''
-
-Prograss_Now = NewType("Prograss_Now", int)
-Myb_Num = NewType("Myb_Num", int)
-
-
-class Mission:
-    """
-    任务信息数据
-
-    通过对象的`key_name`属性来判断该任务是什么\n
-    各个任务对应的`key_name`值在类属性中\n
-    (`Mission.SIGN`, `Mission.VIEW`, `Mission.LIKE`, `Mission.SHARE`)
-    """
     SIGN = "continuous_sign"
-    '''签到任务的 key_name'''
+    '''签到任务的 mission_key'''
     VIEW = "view_post_0"
-    '''阅读任务的 key_name'''
+    '''阅读任务的 mission_key'''
     LIKE = "post_up_0"
-    '''点赞任务的 key_name'''
+    '''点赞任务的 mission_key'''
     SHARE = "share_post_0"
-    '''分享任务的 key_name'''
-
-    def __init__(self, mission_dict: dict) -> None:
-        self.mission_dict = mission_dict
-        try:
-            for func in dir(Mission):
-                if func.startswith("__"):
-                    continue
-                getattr(self, func)
-        except KeyError:
-            logger.error(f"{conf.LOG_HEAD}米游币任务数据 - 初始化对象: dict数据不正确")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
+    '''分享任务的 mission_key'''
 
-    @property
-    def points(self) -> int:
-        """
-        任务米游币奖励
-        """
-        return self.mission_dict["points"]
+    AVAILABLE_GAMES: Set[Type["BaseMission"]] = set()
+    """可用的子类"""
 
-    @property
-    def name(self) -> str:
-        """
-        任务名字，如 讨论区签到
-        """
-        return self.mission_dict["name"]
-
-    @property
-    def key_name(self):
-        """
-        任务代号，如 continuous_sign
+    def __init__(self, account: UserAccount) -> None:
         """
-        for name in (self.SIGN, self.VIEW, self.LIKE, self.SHARE):
-            if name == self.mission_dict["mission_key"]:
-                return name
+        米游币任务相关
 
-    @property
-    def total_times(self) -> int:
-        """
-        任务完成的次数要求
+        :param account: 账号对象
         """
-        return self.mission_dict["threshold"]
-
-
-class Action:
-    """
-    米游币任务相关(需先初始化对象)
-
-    类属性有`NAME_TO_FUNC`，是任务`key_name`与函数的对应关系
-    """
-    Action_Method = NewType("Action_Method", Any)
-
-    def __init__(self, account: UserAccount) -> None:
         self.account = account
-        self.headers = HEADERS.copy()
-        self.headers["x-rpc-device_id"] = account.deviceID_2
-        self.client = httpx.AsyncClient(cookies=account.cookie)
-
-    async def async_init(self):
-        """
-        初始化米游币任务(异步，返回`self`对象)(执行deviceLogin和saveDevice)
-        """
-        await device_login(self.account)
-        await device_save(self.account)
-        return self
+        self.headers = HEADERS_BASE.copy()
+        self.headers["x-rpc-device_id"] = account.device_id_android
 
-    async def sign(self, game: Literal["bh3", "ys", "bh2", "wd", "xq"], retry: bool = True) -> Union[
-        int, Literal[-1, -2, -3]]:
+    async def sign(self, retry: bool = True) -> Tuple[MissionStatus, Optional[int]]:
         """
         签到
 
-        :param game: 游戏简称
         :param retry: 是否允许重试
-
-        - 若返回 `-1` 说明用户登录失效
-        - 若返回 `-2` 说明服务器没有正确返回
-        - 若返回 `-3` 说明请求失败
+        :return: (BaseApiStatus, 签到获得的米游币数量)
         """
-        data = {"gids": GAME_ID[game].gids}
+        content = {"gids": self.GIDS}
         try:
-            subscribe = Subscribe()
-            async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
-                                                        wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+            async for attempt in get_async_retry(retry):
                 with attempt:
                     headers = HEADERS_OLD.copy()
-                    headers["x-rpc-device_id"] = self.account.deviceID_2
-                    headers["DS"] = generate_ds(data)
-                    res = await self.client.post(URL_SIGN, headers=headers, json=data, timeout=conf.TIME_OUT)
-                    if not check_login(res.text):
+                    headers["x-rpc-device_id"] = self.account.device_id_android
+                    headers["DS"] = generate_ds(data=content)
+                    async with httpx.AsyncClient() as client:
+                        res = await client.post(
+                            URL_SIGN,
+                            headers=headers,
+                            json=content,
+                            timeout=_conf.preference.timeout,
+                            cookies=self.account.cookies.dict(v2_stoken=True, cookie_type=True)
+                        )
+                    api_result = ApiResultHandler(res.json())
+                    if api_result.login_expired:
                         logger.info(
-                            f"{conf.LOG_HEAD}米游币任务 - 讨论区签到: 用户 {self.account.phone} 登录失效")
-                        logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                        return -1
-                    if not check_ds(res.text):
+                            f"米游币任务 - 讨论区签到: 用户 {self.account.bbs_uid} 登录失效")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(login_expired=True), None
+                    if api_result.invalid_ds:
                         logger.info(
-                            f"{conf.LOG_HEAD}米游币任务 - 讨论区签到: DS无效，正在在线获取salt以重新生成...")
-                        await subscribe.load()
-                        headers["DS"] = generate_ds(data)
-                    return res.json()["data"]["points"]
-        except KeyError and ValueError and TypeError:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 讨论区签到: 服务器没有正确返回")
-            logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return -2
-        except Exception:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 讨论区签到: 请求失败")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return -3
+                            f"米游币任务 - 讨论区签到: 用户 {self.account.bbs_uid} DS 校验失败")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(invalid_ds=True), None
+                    return api_result.data["points"]
+        except tenacity.RetryError as e:
+            if is_incorrect_return(e):
+                logger.exception(f"米游币任务 - 讨论区签到: 服务器没有正确返回")
+                logger.debug(f"网络请求返回: {res.text}")
+                return MissionStatus(incorrect_return=True), None
+            else:
+                logger.exception("米游币任务 - 讨论区签到: 请求失败")
+                return MissionStatus(network_error=True), None
 
-    async def get_posts(self, game: Literal["bh3", "ys", "bh2", "wd", "xq"], retry: bool = True) -> Optional[List[str]]:
+    async def get_posts(self, retry: bool = True) -> Tuple[BaseApiStatus, Optional[List[str]]]:
         """
         获取文章ID列表，若失败返回 `None`
 
-        :param game: 游戏简称
         :param retry: 是否允许重试
-        :return: 文章ID列表
+        :return: (BaseApiStatus, 文章ID列表)
         """
         post_id_list = []
         try:
-            async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
-                                                        wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+            async for attempt in get_async_retry(retry):
                 with attempt:
                     headers = HEADERS_GET_POSTS.copy()
-                    headers["x-rpc-device_id"] = self.account.deviceID
-                    res = await self.client.get(URL_GET_POST.format(GAME_ID[game].gids), headers=headers,
-                                                timeout=conf.TIME_OUT)
-                    data = res.json()["data"]["list"]
-                    for post in data:
+                    headers["x-rpc-device_id"] = self.account.device_id_ios
+                    async with httpx.AsyncClient() as client:
+                        res = await client.get(
+                            URL_GET_POST.format(self.GIDS),
+                            headers=headers,
+                            timeout=_conf.preference.timeout
+                        )
+                    api_result = ApiResultHandler(res.json())
+                    for post in api_result.data["list"]:
                         if post["self_operation"]["attitude"] == 0:
                             post_id_list.append(post['post']['post_id'])
                     break
-        except KeyError and ValueError and TypeError:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 获取文章列表: 服务器没有正确返回")
-            logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-            logger.debug(f"{conf.LOG_HEAD}发送数据：url={URL_GET_POST.format(GAME_ID[game].gids)}, headers={self.headers}")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return None
-        except Exception:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 获取文章列表: 网络请求失败")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return None
-        return post_id_list
+            return BaseApiStatus(success=True), post_id_list
+        except tenacity.RetryError as e:
+            if is_incorrect_return(e):
+                logger.exception(f"米游币任务 - 获取文章列表: 服务器没有正确返回")
+                logger.debug(f"网络请求返回: {res.text}")
+                return BaseApiStatus(incorrect_return=True), None
+            else:
+                logger.exception(f"米游币任务 - 获取文章列表: 请求失败")
+                return BaseApiStatus(network_error=True), None
 
-    async def read(self, game: Literal["bh3", "ys", "bh2", "wd", "xq"], read_times: int = 5, retry: bool = True):
+    async def read(self, read_times: int = 5, retry: bool = True) -> MissionStatus:
         """
         阅读
 
-        :param game: 游戏简称
         :param read_times: 阅读文章数
         :param retry: 是否允许重试
-
-        - 若执行成功，返回 `1`
-        - 若返回 `-1` 说明用户登录失效
-        - 若返回 `-2` 说明服务器没有正确返回或请求失败
-        - 若返回 `-3` 说明请求失败
-        - 若返回 `-4` 说明获取文章失败
         """
         count = 0
-        post_id_list = await self.get_posts(game)
-        if post_id_list is None:
-            return -4
+        get_post_status, posts = await self.get_posts(retry)
+        if not get_post_status:
+            return MissionStatus(failed_getting_post=True)
         while count < read_times:
-            for postID in post_id_list:
+            for post_id in posts:
                 if count == read_times:
                     break
                 try:
-                    subscribe = Subscribe()
-                    async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
-                                                                wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+                    async for attempt in get_async_retry(retry):
                         with attempt:
                             self.headers["DS"] = generate_ds(platform="android")
-                            res = await self.client.get(URL_READ.format(postID), headers=self.headers,
-                                                        timeout=conf.TIME_OUT)
-                            if not check_login(res.text):
+                            async with httpx.AsyncClient() as client:
+                                res = await client.get(
+                                    URL_READ.format(post_id),
+                                    headers=self.headers,
+                                    timeout=_conf.preference.timeout,
+                                    cookies=self.account.cookies.dict(v2_stoken=True, cookie_type=True)
+                                )
+                            api_result = ApiResultHandler(res.json())
+                            if api_result.login_expired:
                                 logger.info(
-                                    f"{conf.LOG_HEAD}米游币任务 - 阅读: 用户 {self.account.phone} 登录失效")
-                                logger.debug(
-                                    f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                                return -1
-                            if not check_ds(res.text):
+                                    f"米游币任务 - 阅读: 用户 {self.account.bbs_uid} 登录失效")
+                                logger.debug(f"网络请求返回: {res.text}")
+                                return MissionStatus(login_expired=True)
+                            if api_result.invalid_ds:
                                 logger.info(
-                                    f"{conf.LOG_HEAD}米游币任务 - 阅读: DS无效，正在在线获取salt以重新生成...")
-                                await subscribe.load()
-                                self.headers["DS"] = generate_ds(
-                                    platform="android")
-                            if res.json()["message"] == "帖子不存在":
+                                    f"米游币任务 - 阅读: 用户 {self.account.bbs_uid} DS 校验失败")
+                                logger.debug(f"网络请求返回: {res.text}")
+                                return MissionStatus(invalid_ds=True)
+                            if api_result.message == "帖子不存在":
                                 continue
-                            if "self_operation" not in res.json()["data"]["post"]:
+                            temp = api_result.data.get("post")
+                            if temp is not None and "self_operation" not in temp:
                                 raise ValueError
                             count += 1
-                except KeyError and ValueError and TypeError:
-                    logger.error(f"{conf.LOG_HEAD}米游币任务 - 阅读: 服务器没有正确返回")
-                    logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                    logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-                    return -2
-                except Exception:
-                    logger.error(f"{conf.LOG_HEAD}米游币任务 - 阅读: 网络请求失败")
-                    logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-                    return -3
+                except tenacity.RetryError as e:
+                    if is_incorrect_return(e, ValueError):
+                        logger.exception(f"米游币任务 - 阅读: 服务器没有正确返回")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(incorrect_return=True)
+                    else:
+                        logger.exception(f"米游币任务 - 阅读: 请求失败")
+                        return MissionStatus(network_error=True)
                 if count != read_times:
-                    await asyncio.sleep(conf.SLEEP_TIME)
-            post_id_list = await self.get_posts(game)
-            if post_id_list is None:
-                return -4
+                    await asyncio.sleep(_conf.preference.sleep_time)
+            get_post_status, posts = await self.get_posts(retry)
+            if not get_post_status:
+                return MissionStatus(failed_getting_post=True)
 
-        return 1
+        return MissionStatus(success=True)
 
-    async def like(self, game: Literal["bh3", "ys", "bh2", "wd", "xq"], like_times: int = 10, retry: bool = True):
+    async def like(self, like_times: int = 10, retry: bool = True) -> MissionStatus:
         """
         点赞文章
 
-        :param game: 游戏简称
         :param like_times: 点赞次数
         :param retry: 是否允许重试
-
-        - 若执行成功，返回 `1`
-        - 若返回 `-1` 说明用户登录失效
-        - 若返回 `-2` 说明服务器没有正确返回或请求失败
-        - 若返回 `-3` 说明请求失败
-        - 若返回 `-4` 说明获取文章失败
         """
         count = 0
-        post_id_list = await self.get_posts(game)
-        if post_id_list is None:
-            return -4
+        get_post_status, posts = await self.get_posts(retry)
+        if not get_post_status:
+            return MissionStatus(failed_getting_post=True)
         while count < like_times:
-            for postID in post_id_list:
+            for post_id in posts:
                 if count == like_times:
                     break
                 try:
-                    subscribe = Subscribe()
-                    async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
-                                                                wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+                    async for attempt in get_async_retry(retry):
                         with attempt:
                             headers = HEADERS_OLD.copy()
-                            headers["x-rpc-device_id"] = self.account.deviceID_2
+                            headers["x-rpc-device_id"] = self.account.device_id_android
                             headers["DS"] = generate_ds(platform="android")
-                            res = await self.client.post(URL_LIKE, headers=headers,
-                                                         json={'is_cancel': False, 'post_id': postID},
-                                                         timeout=conf.TIME_OUT)
-                            if not check_login(res.text):
+                            async with httpx.AsyncClient() as client:
+                                res = await client.post(
+                                    URL_LIKE, headers=headers,
+                                    json={'is_cancel': False, 'post_id': post_id},
+                                    timeout=_conf.preference.timeout,
+                                    cookies=self.account.cookies.dict(v2_stoken=True, cookie_type=True)
+                                )
+                            api_result = ApiResultHandler(res.json())
+                            if api_result.login_expired:
                                 logger.info(
-                                    f"{conf.LOG_HEAD}米游币任务 - 点赞: 用户 {self.account.phone} 登录失效")
-                                logger.debug(
-                                    f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                                return -1
-                            if not check_ds(res.text):
+                                    f"米游币任务 - 点赞: 用户 {self.account.bbs_uid} 登录失效")
+                                logger.debug(f"网络请求返回: {res.text}")
+                                return MissionStatus(login_expired=True)
+                            if api_result.invalid_ds:
                                 logger.info(
-                                    f"{conf.LOG_HEAD}米游币任务 - 点赞: DS无效，正在在线获取salt以重新生成...")
-                                await subscribe.load()
-                                headers["DS"] = generate_ds(
-                                    platform="android")
-                            if res.json()["message"] == "帖子不存在":
+                                    f"米游币任务 - 点赞: 用户 {self.account.bbs_uid} DS 校验失败")
+                                logger.debug(f"网络请求返回: {res.text}")
+                                return MissionStatus(invalid_ds=True)
+                            if api_result.message == "帖子不存在":
                                 continue
-                            elif res.json()["message"] != "OK":
+                            if api_result.message != "OK":
                                 raise ValueError
                             count += 1
-                except KeyError and ValueError and TypeError:
-                    logger.error(f"{conf.LOG_HEAD}米游币任务 - 点赞: 服务器没有正确返回")
-                    logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                    logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-                    return -2
-                except Exception:
-                    logger.error(f"{conf.LOG_HEAD}米游币任务 - 点赞: 网络请求失败")
-                    logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-                    return -3
+                except tenacity.RetryError as e:
+                    if is_incorrect_return(e, ValueError):
+                        logger.exception(f"米游币任务 - 点赞: 服务器没有正确返回")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(incorrect_return=True)
+                    else:
+                        logger.exception(f"米游币任务 - 点赞: 请求失败")
+                        return MissionStatus(network_error=True)
                 if count != like_times:
-                    await asyncio.sleep(conf.SLEEP_TIME)
-            post_id_list = await self.get_posts(game)
-            if post_id_list is None:
-                return -4
+                    await asyncio.sleep(_conf.preference.sleep_time)
+            get_post_status, posts = await self.get_posts(retry)
+            if not get_post_status:
+                return MissionStatus(failed_getting_post=True)
 
-        return 1
+        return MissionStatus(success=True)
 
-    async def share(self, game: Literal["bh3", "ys", "bh2", "wd", "xq"], retry: bool = True):
+    async def share(self, retry: bool = True):
         """
         分享文章
 
-        :param game: 游戏简称
         :param retry: 是否允许重试
-
-        - 若执行成功，返回 `1`
-        - 若返回 `-1` 说明用户登录失效
-        - 若返回 `-2` 说明服务器没有正确返回
-        - 若返回 `-3` 说明请求失败
-        - 若返回 `-4` 说明网络请求发送成功，但是可能未签到成功
-        - 若返回 `-5` 说明获取文章失败
-        """
-        post_id_list = await self.get_posts(game)
-        if post_id_list is None:
-            return -5
+        """
+        get_post_status, posts = await self.get_posts(retry)
+        if not get_post_status or not posts:
+            return MissionStatus(failed_getting_post=True)
         try:
-            subscribe = Subscribe()
-            async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
-                                                        wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+            async for attempt in get_async_retry(retry):
                 with attempt:
                     headers = HEADERS_OLD.copy()
-                    headers["x-rpc-device_id"] = self.account.deviceID_2
+                    headers["x-rpc-device_id"] = self.account.device_id_android
                     headers["DS"] = generate_ds(platform="android")
-                    res = await self.client.get(URL_SHARE.format(post_id_list[0]), headers=headers,
-                                                timeout=conf.TIME_OUT)
-                    if not check_login(res.text):
+                    async with httpx.AsyncClient() as client:
+                        res = await client.get(
+                            URL_SHARE.format(posts[0]),
+                            headers=headers,
+                            timeout=_conf.preference.timeout,
+                            cookies=self.account.cookies.dict(v2_stoken=True, cookie_type=True)
+                        )
+                    api_result = ApiResultHandler(res.json())
+                    if api_result.login_expired:
                         logger.info(
-                            f"{conf.LOG_HEAD}米游币任务 - 分享: 用户 {self.account.phone} 登录失效")
-                        logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-                        return -1
-                    if not check_ds(res.text):
+                            f"米游币任务 - 分享: 用户 {self.account.bbs_uid} 登录失效")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(login_expired=True)
+                    if api_result.invalid_ds:
                         logger.info(
-                            f"{conf.LOG_HEAD}米游币任务 - 分享: DS无效，正在在线获取salt以重新生成...")
-                        conf.salt.SALT_ANDROID = await subscribe.load()
-                        headers["DS"] = generate_ds(
-                            platform="android")
-                    if res.json()["message"] == "帖子不存在":
+                            f"米游币任务 - 分享: 用户 {self.account.bbs_uid} DS 校验失败")
+                        logger.debug(f"网络请求返回: {res.text}")
+                        return MissionStatus(invalid_ds=True)
+                    if api_result.message == "帖子不存在":
                         continue
-                    elif res.json()["message"] != "OK":
-                        return -4
-        except KeyError and ValueError and TypeError:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 分享: 服务器没有正确返回")
-            logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return -2
-        except Exception:
-            logger.error(f"{conf.LOG_HEAD}米游币任务 - 分享: 网络请求失败")
-            logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-            return -3
-        return 1
-
-    NAME_TO_FUNC: Dict[str, Action_Method] = {
-        Mission.SIGN: sign,
-        Mission.VIEW: read,
-        Mission.LIKE: like,
-        Mission.SHARE: share
-    }
+                    if api_result.message != "OK":
+                        raise ValueError
+        except tenacity.RetryError as e:
+            if is_incorrect_return(e, ValueError):
+                logger.exception(f"米游币任务 - 分享: 服务器没有正确返回")
+                logger.debug(f"网络请求返回: {res.text}")
+                return MissionStatus(incorrect_return=True)
+            else:
+                logger.exception(f"米游币任务 - 分享: 请求失败")
+                return MissionStatus(network_error=True)
+        return MissionStatus(success=True)
+
+
+class GenshinImpactMission(BaseMission):
+    """
+    原神 米游币任务
+    """
+    NAME = "原神"
+    GIDS = 2
+    FID = 26
+
+
+class HonkaiImpact3Mission(BaseMission):
+    """
+    崩坏3 米游币任务
+    """
+    NAME = "崩坏3"
+    GIDS = 1
+    FID = 1
+
+
+class HoukaiGakuen2Mission(BaseMission):
+    """
+    崩坏学园2 米游币任务
+    """
+    NAME = "崩坏学园2"
+    GIDS = 3
+    FID = 30
+
+
+class TearsOfThemisMission(BaseMission):
+    """
+    未定事件簿 米游币任务
+    """
+    NAME = "未定事件簿"
+    GIDS = 4
+    FID = 37
+
+
+class StarRailMission(BaseMission):
+    """
+    崩坏：星穹铁道 米游币任务
+    """
+    NAME = "崩坏：星穹铁道"
+    GIDS = 5
+    FID = 52
+
+
+class BBSMission(BaseMission):
+    """
+    大别野 米游币任务
+    """
+    NAME = "大别野"
+    GIDS = 5
+    # TODO: bbs fid暂时未知
 
 
-async def get_missions(account: UserAccount):
+BaseMission.AVAILABLE_GAMES.add(GenshinImpactMission)
+BaseMission.AVAILABLE_GAMES.add(HonkaiImpact3Mission)
+BaseMission.AVAILABLE_GAMES.add(HoukaiGakuen2Mission)
+BaseMission.AVAILABLE_GAMES.add(TearsOfThemisMission)
+BaseMission.AVAILABLE_GAMES.add(StarRailMission)
+BaseMission.AVAILABLE_GAMES.add(BBSMission)
+
+
+async def get_missions(account: UserAccount, retry: bool = True) -> Tuple[BaseApiStatus, Optional[List[MissionData]]]:
     """
     获取米游币任务信息
 
-    - 若返回 `-1` 说明用户登录失效
-    - 若返回 `-2` 说明服务器没有正确返回
-    - 若返回 `-3` 说明请求失败
+    :param account: 用户账号
+    :param retry: 是否允许重试
     """
     try:
-        async with httpx.AsyncClient() as client:
-            res = await client.get(URL_MISSION, headers=HEADERS_MISSION, cookies=account.cookie, timeout=conf.TIME_OUT)
-        if not check_login(res.text):
-            logger.info(f"{conf.LOG_HEAD}获取米游币任务列表 - 用户 {account.phone} 登录失效")
-            logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-            return -1
-        mission_list: List[Mission] = []
-        for mission in res.json()["data"]["missions"]:
-            mission_list.append(Mission(mission))
-        return mission_list
-    except KeyError and ValueError and TypeError:
-        logger.error(f"{conf.LOG_HEAD}获取米游币任务列表 - 服务器没有正确返回")
-        logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-        logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-        return -2
-    except Exception:
-        logger.error(f"{conf.LOG_HEAD}获取米游币任务列表 - 请求失败")
-        logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-        return -3
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                async with httpx.AsyncClient() as client:
+                    res = await client.get(URL_MISSION, headers=HEADERS_MISSION,
+                                           cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
+                                           timeout=_conf.preference.timeout)
+                api_result = ApiResultHandler(res.json())
+                if api_result.login_expired:
+                    logger.info(
+                        f"获取米游币任务列表: 用户 {account.bbs_uid} 登录失效")
+                    logger.debug(f"网络请求返回: {res.text}")
+                    return BaseApiStatus(login_expired=True), None
+                mission_list: List[MissionData] = []
+                for mission in api_result.data["missions"]:
+                    mission_list.append(MissionData.parse_obj(mission))
+                return BaseApiStatus(success=True), mission_list
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception(f"获取米游币任务列表: 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception("获取米游币任务列表: 请求失败")
+            return BaseApiStatus(network_error=True), None
 
 
-async def get_missions_state(account: UserAccount) -> Union[Tuple[List[Tuple[Mission, Prograss_Now]], Myb_Num], int]:
+async def get_missions_state(account: UserAccount, retry: bool = True) -> Tuple[BaseApiStatus, Optional[MissionState]]:
     """
     获取米游币任务完成情况
 
-    返回数据格式:
-    `tuple[ list[ tuple[任务信息对象, 当前进度] ], 用户当前米游币数量 ]`
-
-    - 若返回 `-1` 说明用户登录失效
-    - 若返回 `-2` 说明服务器没有正确返回
-    - 若返回 `-3` 说明请求失败
-    """
-    missions: List[Mission] = await get_missions(account)
-    if isinstance(missions, int):
-        if missions == -1:
-            return -1
-        elif missions == -2:
-            return -2
-        elif missions == -3:
-            return -3
+    :param account: 用户账号
+    :param retry: 是否允许重试
+    """
+    get_missions_status, missions = await get_missions(account)
+    if not get_missions_status:
+        return get_missions_status, None
     try:
-        async with httpx.AsyncClient() as client:
-            res = await client.get(URL_MISSION_STATE, headers=HEADERS_MISSION, cookies=account.cookie,
-                                   timeout=conf.TIME_OUT)
-        if not check_login(res.text):
-            logger.info(
-                f"{conf.LOG_HEAD}获取米游币任务完成情况 - 用户 {account.phone} 登录失效")
-            logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-            return -1
-        state_list: List[Tuple[Mission, Prograss_Now]] = []
-        data = res.json()["data"]
-        for mission in missions:
-            try:
-                state_list.append((mission, list(filter(lambda state: state["mission_key"] ==
-                                                                      mission.key_name, data["states"]))[0][
-                    "happened_times"]))
-            except IndexError:
-                state_list.append((mission, 0))
-        return state_list, data["total_points"]
-    except KeyError and ValueError and TypeError:
-        logger.error(f"{conf.LOG_HEAD}获取米游币任务完成情况 - 服务器没有正确返回")
-        logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
-        logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-        return -2
-    except Exception:
-        logger.error(f"{conf.LOG_HEAD}获取米游币任务完成情况 - 请求失败")
-        logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-        return -3
+        async for attempt in get_async_retry(retry):
+            with attempt:
+                async with httpx.AsyncClient() as client:
+                    res = await client.get(URL_MISSION_STATE, headers=HEADERS_MISSION,
+                                           cookies=account.cookies.dict(v2_stoken=True, cookie_type=True),
+                                           timeout=_conf.preference.timeout)
+                api_result = ApiResultHandler(res.json())
+                if api_result.login_expired:
+                    logger.info(
+                        f"获取米游币任务完成情况: 用户 {account.bbs_uid} 登录失效")
+                    logger.debug(f"网络请求返回: {res.text}")
+                    return BaseApiStatus(login_expired=True), None
+                state_dict = {}
+                for mission in missions:
+                    try:
+                        current = list(filter(lambda state: state["mission_key"] == mission.mission_key,
+                                              api_result.data["states"]))[0]["happened_times"]
+                        state_dict.setdefault(mission.mission_key, (mission, current))
+                    except IndexError:
+                        state_dict.setdefault(mission.mission_key, (mission, 0))
+                return BaseApiStatus(success=True), MissionState(state_dict=state_dict,
+                                                                 current_myb=api_result.data["total_points"])
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception("获取米游币任务完成情况: 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception("获取米游币任务完成情况: 请求失败")
+            return BaseApiStatus(network_error=True), None
```

### Comparing `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/setting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,203 +1,196 @@
 """
 ### 用户设置相关
 """
-from typing import List, Union
+from typing import Union
 
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent, GroupMessageEvent, MessageEvent
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, ArgPlainText, T_State
 
-from .bbsAPI import GameInfo
-from .config import config as conf
-from .data import UserAccount, UserData
-from .mybMission import GAME_ID
+from .myb_missions_api import BaseMission
+from .plugin_data import PluginDataManager, write_plugin_data
+from .user_data import UserAccount
 from .utils import COMMAND_BEGIN
 
-setting = on_command(conf.COMMAND_START + '设置', priority=4, block=True)
+_conf = PluginDataManager.plugin_data_obj
+
+setting = on_command(_conf.preference.command_start + '设置', priority=4, block=True)
 setting.name = "设置"
-setting.usage = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令。\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令。'
+setting.usage = '如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{HEAD}账号设置』命令。' \
+                '\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{HEAD}通知设置』命令。'
 
 
 @setting.handle()
-async def _(event: MessageEvent):
-    msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
+async def _(_: MessageEvent):
+    msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令' \
+          f'\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
     await setting.send(msg)
 
 
-account_setting = on_command(conf.COMMAND_START + '账号设置', priority=5, block=True)
+account_setting = on_command(_conf.preference.command_start + '账号设置', priority=5, block=True)
 account_setting.name = "账号设置"
 account_setting.usage = "配置游戏自动签到、米游币任务是否开启、设备平台、频道任务相关选项"
 
 
 @account_setting.handle()
-async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher):
     """
     账号设置命令触发
     """
-    if isinstance(event, GroupMessageEvent):
-        await account_setting.finish('⚠️为了保护您的隐私，请添加机器人好友后私聊进行设置操作')
-    user_account = UserData.read_account_all(event.user_id)
-    state['user_account'] = user_account
+    user = _conf.users.get(event.user_id)
+    user_account = user.accounts if user else None
     if not user_account:
-        await account_setting.finish(f"⚠️你尚未绑定米游社账户，请先使用『{conf.COMMAND_START}登录』进行登录")
+        await account_setting.finish(
+            f"⚠️你尚未绑定米游社账户，请先使用『{_conf.preference.command_start}登录』进行登录")
     if len(user_account) == 1:
-        matcher.set_arg('phone', Message(str(user_account[0].phone)))
+        uid = next(iter(user_account.values())).bbs_uid
+        matcher.set_arg('bbs_uid', Message(uid))
     else:
-        phones = [str(user_account[i].phone) for i in range(len(user_account))]
+        uids = map(lambda x: x.bbs_uid, user_account.values())
         msg = "您有多个账号，您要更改以下哪个账号的设置？\n"
-        msg += "📱" + "\n📱".join(phones)
+        msg += "\n".join(map(lambda x: f"🆔{x}", uids))
         msg += "\n🚪发送“退出”即可退出"
         await matcher.send(msg)
 
 
-@account_setting.got('phone')
-async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, phone=Arg('phone')):
+@account_setting.got('bbs_uid')
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State, uid=Arg('bbs_uid')):
     """
     根据手机号设置相应的账户
     """
-    if isinstance(phone, Message):
-        phone = phone.extract_plain_text().strip()
-    if phone == '退出':
+    if isinstance(uid, Message):
+        uid = uid.extract_plain_text().strip()
+    if uid == '退出':
         await matcher.finish('🚪已成功退出')
-    user_account: List[UserAccount] = state['user_account']
-    phones = [str(user_account[i].phone) for i in range(len(user_account))]
-    account = None
-    if phone in phones:
-        account = UserData.read_account(event.user_id, int(phone))
-    else:
-        await matcher.reject('⚠️您输入的账号不在以上账号内，请重新输入')
+
+    user_account = _conf.users[event.user_id].accounts
+    if uid not in user_account:
+        await account_setting.reject('⚠️您发送的账号不在以上账号内，请重新发送')
+    account = user_account[uid]
     state['account'] = account
     state["prepare_to_delete"] = False
+
     user_setting = ""
-    user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.mybMission else '关'}\n"
-    user_setting += f"2️⃣ 游戏自动签到：{'开' if account.gameSign else '关'}\n"
+    user_setting += f"1️⃣ 米游币任务自动执行：{'开' if account.enable_mission else '关'}"
+    user_setting += f"\n2️⃣ 游戏自动签到：{'开' if account.enable_mission else '关'}"
     platform_show = "iOS" if account.platform == "ios" else "安卓"
-    user_setting += f"3️⃣ 设备平台：{platform_show}\n"
+    user_setting += f"\n3️⃣ 设备平台：{platform_show}"
 
     # 筛选出用户数据中的missionGame对应的游戏全称
-    user_setting += "4️⃣ 执行米游币任务的频道：『" + \
-                    "、".join([game_tuple[1] for game_tuple in list(filter(
-                        lambda game_tuple: game_tuple[0] in account.missionGame,
-                        GameInfo.ABBR_TO_ID.values()))]) + "』\n"
-    user_setting += f"5️⃣ 原神树脂恢复提醒：{'开' if account.checkResin else '关'}\n"
-    user_setting += "⚠️6⃣️ 删除账户数据"
+    user_setting += "\n\n4️⃣ 执行米游币任务的频道：" + \
+                    "\n- " + "、".join(map(lambda x: f"『{x.NAME}』", account.mission_games))
+    user_setting += f"\n\n5️⃣ 原神树脂恢复提醒：{'开' if account.enable_resin else '关'}"
+    user_setting += "\n6️⃣⚠️删除账户数据"
 
-    await account_setting.send(user_setting + '\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6\n🚪发送“退出”即可退出')
+    await account_setting.send(user_setting + '\n\n您要更改哪一项呢？请发送 1 / 2 / 3 / 4 / 5 / 6'
+                                              '\n🚪发送“退出”即可退出')
 
 
 @account_setting.got('arg')
-async def _(event: PrivateMessageEvent, state: T_State, arg=ArgPlainText('arg')):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], state: T_State, arg=ArgPlainText('arg')):
     """
     根据所选更改相应账户的相应设置
     """
     arg = arg.strip()
     account: UserAccount = state['account']
+    user_account = _conf.users[event.user_id].accounts
     if arg == '退出':
         await account_setting.finish('🚪已成功退出')
     elif arg == '1':
-        account.mybMission = not account.mybMission
-        UserData.set_account(account, event.user_id, account.phone)
-        await account_setting.finish(f"📅米游币任务自动执行已 {'✅开启' if account.mybMission else '❌关闭'}")
+        account.enable_mission = not account.enable_mission
+        write_plugin_data()
+        await account_setting.finish(f"📅米游币任务自动执行已 {'✅开启' if account.enable_mission else '❌关闭'}")
     elif arg == '2':
-        account.gameSign = not account.gameSign
-        UserData.set_account(account, event.user_id, account.phone)
-        await account_setting.finish(f"📅米哈游游戏自动签到已 {'✅开启' if account.gameSign else '❌关闭'}")
+        account.enable_game_sign = not account.enable_game_sign
+        write_plugin_data()
+        await account_setting.finish(f"📅米哈游游戏自动签到已 {'✅开启' if account.enable_game_sign else '❌关闭'}")
     elif arg == '3':
         if account.platform == "ios":
             account.platform = "android"
             platform_show = "安卓"
         else:
             account.platform = "ios"
             platform_show = "iOS"
-        UserData.set_account(account, event.user_id, account.phone)
+        write_plugin_data()
         await account_setting.finish(f"📲设备平台已更改为 {platform_show}")
     elif arg == '4':
-        games_show = "、".join([name_tuple[1]
-                               for name_tuple in list(
-                filter(lambda name_tuple: name_tuple[0] in GAME_ID,
-                       GameInfo.ABBR_TO_ID.values())
-            )
-                               ])
+        games_show = "、".join(map(lambda x: f"『{x.NAME}』", BaseMission.AVAILABLE_GAMES))
         await account_setting.send(
-            "请发送你想要执行米游币任务的频道：\n"
-            "❕多个频道请用空格分隔，如 “原神 崩坏3 大别野”\n"
-            f"可选的频道『{games_show}』\n"
-            "🚪发送“退出”即可退出"
+            "请发送你想要执行米游币任务的频道："
+            "\n❕多个频道请用空格分隔，如 “原神 崩坏3 大别野”"
+            "\n\n可选的频道："
+            f"\n- {games_show}"
+            "\n\n🚪发送“退出”即可退出"
         )
     elif arg == '5':
-        account.checkResin = not account.checkResin
-        UserData.set_account(account, event.user_id, account.phone)
-        await account_setting.finish(f"📅原神树脂恢复提醒已 {'✅开启' if account.checkResin else '❌关闭'}")
+        account.enable_resin = not account.enable_resin
+        write_plugin_data()
+        await account_setting.finish(f"📅原神树脂恢复提醒已 {'✅开启' if account.enable_resin else '❌关闭'}")
     elif arg == '6':
         state["prepare_to_delete"] = True
-        await account_setting.reject(f"⚠️确认删除账号 {account.phone} ？发送 \"确认删除\" 以确定。")
-
+        await account_setting.reject(f"⚠️确认删除账号 {account.phone_number} ？发送 \"确认删除\" 以确定。")
     elif arg == '确认删除' and state["prepare_to_delete"]:
-        del_result = UserData.del_account(event.user_id, account.phone)
-        if del_result:
-            await account_setting.finish(f"已删除账号 {account.phone} 的数据")
-        else:
-            await account_setting.finish(f"删除账号 {account.phone} 的数据失败")
+        user_account.pop(account.bbs_uid)
+        write_plugin_data()
+        await account_setting.finish(f"已删除账号 {account.phone_number} 的数据")
     else:
         await account_setting.reject("⚠️您的输入有误，请重新输入")
 
 
 @account_setting.got('missionGame')
-async def _(event: PrivateMessageEvent, state: T_State, arg=ArgPlainText('missionGame')):
+async def _(_: Union[PrivateMessageEvent, GroupMessageEvent], state: T_State, arg=ArgPlainText('missionGame')):
     arg = arg.strip()
     if arg == '退出':
         await account_setting.finish('🚪已成功退出')
     account: UserAccount = state['account']
     games_input = arg.split()
-    for game in arg.split():
-        if game not in [name_tuple[1]
-                        for name_tuple in GameInfo.ABBR_TO_ID.values()]:
+    mission_games = set()
+    for game in games_input:
+        game_filter = filter(lambda x: x.NAME == game, BaseMission.AVAILABLE_GAMES)
+        game_obj = next(game_filter, None)
+        if game_obj is None:
             await account_setting.reject("⚠️您的输入有误，请重新输入")
+        else:
+            mission_games.add(game_obj)
 
-    # 查找输入的内容是否有不在游戏(频道)列表里的
-    incorrect = list(filter(lambda game: game not in [name_tuple[1]
-                                                      for name_tuple in GameInfo.ABBR_TO_ID.values()], games_input))
-    if incorrect:
-        await account_setting.reject("⚠️您的输入有误，请重新输入")
-    else:
-        account.missionGame = []
-
-        # 查找输入的每个游戏全名的对应缩写
-        for game_input in games_input:
-            account.missionGame.append(list(filter(
-                lambda game_tuple: game_tuple[1] == game_input, GameInfo.ABBR_TO_ID.values()))[0][0])
-    UserData.set_account(account, event.user_id, account.phone)
+    account.mission_games = mission_games
+    write_plugin_data()
     arg = arg.replace(" ", "、")
     await account_setting.finish(f"💬执行米游币任务的频道已更改为『{arg}』")
 
 
-global_setting = on_command(conf.COMMAND_START + '通知设置', priority=5, block=True)
+global_setting = on_command(_conf.preference.command_start + '通知设置', priority=5, block=True)
 global_setting.name = "通知设置"
 global_setting.usage = "设置每日签到后是否进行QQ通知"
 
 
 @global_setting.handle()
-async def _(event: MessageEvent, matcher: Matcher):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher):
     """
     通知设置命令触发
     """
+    user = _conf.users[event.user_id]
     await matcher.send(
-        f"自动通知每日计划任务结果：{'🔔开' if UserData.is_notice(event.user_id) else '🔕关'}\n请问您是否需要更改呢？\n请回复“是”或“否”\n🚪发送“退出”即可退出")
+        f"自动通知每日计划任务结果：{'🔔开' if user.enable_notice else '🔕关'}"
+        "\n请问您是否需要更改呢？\n请回复“是”或“否”\n🚪发送“退出”即可退出")
 
 
 @global_setting.got('choice')
-async def _(event: PrivateMessageEvent, matcher: Matcher, choice: Message = ArgPlainText('choice')):
+async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher,
+            choice: Message = ArgPlainText('choice')):
     """
     根据选择变更通知设置
     """
+    user = _conf.users[event.user_id]
     if choice == '退出':
         await matcher.finish("🚪已成功退出")
     elif choice == '是':
-        UserData.set_notice(not UserData.is_notice(event.user_id), event.user_id)
-        await matcher.finish(f"自动通知每日计划任务结果 已 {'🔔开启' if UserData.is_notice(event.user_id) else '🔕关闭'}")
+        user.enable_notice = not user.enable_notice
+        write_plugin_data()
+        await matcher.finish(f"自动通知每日计划任务结果 已 {'🔔开启' if user.enable_notice else '🔕关闭'}")
     elif choice == '否':
         await matcher.finish("没有做修改哦~")
     else:
         await matcher.reject("⚠️您的输入有误，请重新输入")
```

### Comparing `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-1.0.0b1/src/nonebot_plugin_mystool/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
 ### 工具函数
 """
 import hashlib
 import json
-import os
 import random
 import string
 import time
 import traceback
 import uuid
-from typing import (TYPE_CHECKING, Any, Dict, List, Literal,
-                    Union)
+from typing import (TYPE_CHECKING, Dict, Literal,
+                    Union, Optional)
 from urllib.parse import urlencode
 
 import httpx
 import nonebot
 import nonebot.log
 import nonebot.plugin
 import ntplib
 import tenacity
 from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 
-from .config import config as conf
+from .plugin_data import PluginDataManager
 
 if TYPE_CHECKING:
     from loguru import Logger
 
-driver = nonebot.get_driver()
+_conf = PluginDataManager.plugin_data_obj
+_driver = nonebot.get_driver()
 
 
 class CommandBegin:
     """
     命令开头字段
     （包括例如'/'和插件命令起始字段例如'mystool'）
     已重写__str__方法
@@ -41,111 +41,125 @@
 
     @classmethod
     def set_command_begin(cls):
         """
         机器人启动时设置命令开头字段
         """
         if nonebot.get_driver().config.command_start:
-            cls.string = list(nonebot.get_driver().config.command_start)[0] + conf.COMMAND_START
+            cls.string = list(nonebot.get_driver().config.command_start)[0] + _conf.preference.command_start
         else:
-            cls.string = conf.COMMAND_START
+            cls.string = _conf.preference.command_start
 
     @classmethod
     def __str__(cls):
         return cls.string
 
 
 def get_last_command_sep():
     """
     获取第最后一个命令分隔符
     """
-    if driver.config.command_sep:
-        return list(driver.config.command_sep)[-1]
+    if _driver.config.command_sep:
+        return list(_driver.config.command_sep)[-1]
 
 
-driver.on_startup(CommandBegin.set_command_begin)
+_driver.on_startup(CommandBegin.set_command_begin)
 COMMAND_BEGIN = CommandBegin()
 '''命令开头字段（包括例如'/'和插件命令起始字段例如'mystool'）'''
 
 
 def set_logger(logger: "Logger"):
     """
     给日志记录器对象增加输出到文件的Handler
     """
     # 根据"name"筛选日志，如果在 plugins 目录加载，则通过 LOG_HEAD 识别
     # 如果不是插件输出的日志，但是与插件有关，则也进行保存
-    logger.add(conf.LOG_PATH, diagnose=False, format=nonebot.log.default_format,
-               filter=lambda record: record["name"] == conf.PLUGIN_NAME or
-                                     (conf.LOG_HEAD != "" and record["message"].find(conf.LOG_HEAD) == 0) or
-                                     record["message"].find(f"plugins.{conf.PLUGIN_NAME}") != -1,
-               rotation=conf.LOG_ROTATION)
+    logger.add(_conf.preference.log_path, diagnose=False, format=nonebot.log.default_format,
+               filter=lambda record: record["name"] == _conf.preference.plugin_name or
+                                     (_conf.preference.log_head != "" and record["message"].find(
+                                         _conf.preference.log_head) == 0) or
+                                     record["message"].find(f"plugins.{_conf.preference.plugin_name}") != -1,
+               rotation=_conf.preference.log_rotation)
     return logger
 
 
 logger = set_logger(logger)
 """本插件所用日志记录器对象（包含输出到文件）"""
 
-PLUGIN = nonebot.plugin.get_plugin(conf.PLUGIN_NAME)
+PLUGIN = nonebot.plugin.get_plugin(_conf.preference.plugin_name)
 '''本插件数据'''
 
 if not PLUGIN:
-    logger.warning("插件数据(Plugin)获取失败，如果插件是从本地加载的，需要修改配置文件中 PLUGIN_NAME 为插件目录，否则将导致无法获取插件帮助信息等")
-
-
-class NtpTime:
-    """
-    `NtpTime.time() #获取校准后的时间（如果校准成功）`
-    """
-    time_offset = 0
-
-    @classmethod
-    def time(cls) -> float:
-        """
-        获取校准后的时间（如果校准成功）
-        """
-        return time.time() + cls.time_offset
+    logger.warning(
+        "插件数据(Plugin)获取失败，如果插件是从本地加载的，需要修改配置文件中 PLUGIN_NAME 为插件目录，否则将导致无法获取插件帮助信息等")
 
 
 def custom_attempt_times(retry: bool):
     """
     自定义的重试机制停止条件\n
     根据是否要重试的bool值，给出相应的`tenacity.stop_after_attempt`对象
 
     :param retry True - 重试次数达到配置中 MAX_RETRY_TIMES 时停止; False - 执行次数达到1时停止，即不进行重试
     """
     if retry:
-        return tenacity.stop_after_attempt(conf.MAX_RETRY_TIMES + 1)
+        return tenacity.stop_after_attempt(_conf.preference.max_retry_times + 1)
     else:
         return tenacity.stop_after_attempt(1)
 
 
-@driver.on_startup
-def ntp_time_sync():
+def get_async_retry(retry: bool):
     """
-    启动时校对互联网时间
+    获取异步重试装饰器
+
+    :param retry: True - 重试次数达到偏好设置中 max_retry_times 时停止; False - 执行次数达到1时停止，即不进行重试
     """
-    NtpTime.time_offset = 0
-    try:
-        for attempt in tenacity.Retrying(stop=custom_attempt_times(True)):
-            with attempt:
-                logger.info(f"{conf.LOG_HEAD}正在校对互联网时间")
-                try:
-                    NtpTime.time_offset = ntplib.NTPClient().request(
-                        conf.NTP_SERVER).tx_time - time.time()
-                    format_offset = "%.2f" % NtpTime.time_offset
-                    logger.info(
-                        f"{conf.LOG_HEAD}系统时间与网络时间的误差为 {format_offset} 秒")
-                    if abs(NtpTime.time_offset) > 0.2:
-                        logger.warning(
-                            f"{conf.LOG_HEAD}系统时间与网络时间误差偏大，可能影响商品兑换成功概率，建议同步系统时间")
-                except Exception:
-                    logger.warning(f"{conf.LOG_HEAD}校对互联网时间失败，正在重试")
-                    raise
-    except tenacity.RetryError:
-        logger.warning(f"{conf.LOG_HEAD}校对互联网时间失败")
+    return tenacity.AsyncRetrying(
+        stop=custom_attempt_times(retry),
+        retry=tenacity.retry_if_exception_type(BaseException),
+        wait=tenacity.wait_fixed(_conf.preference.retry_interval),
+    )
+
+
+class NtpTime:
+    """
+    NTP时间校准相关
+    """
+    time_offset = 0
+    """本地时间与互联网时间的偏差"""
+
+    @classmethod
+    def sync(cls):
+        """
+        校准时间
+        """
+        if _conf.preference.enable_ntp_sync:
+            if not _conf.preference.ntp_server:
+                logger.error("开启了互联网时间校对，但未配置NTP服务器 preference.ntp_server，放弃时间同步")
+                return False
+            try:
+                for attempt in get_async_retry(True):
+                    with attempt:
+                        cls.time_offset = ntplib.NTPClient().request(
+                            _conf.preference.ntp_server).tx_time - time.time()
+            except tenacity.RetryError:
+                logger.error("校对互联网时间失败，改为使用本地时间")
+                logger.debug(traceback.format_exc())
+                return False
+            logger.info("互联网时间校对完成")
+            return True
+        else:
+            logger.info("未开启互联网时间校对，跳过时间同步")
+            return True
+
+    @classmethod
+    def time(cls) -> float:
+        """
+        获取校准后的时间（如果校准成功）
+        """
+        return time.time() + cls.time_offset
 
 
 def generate_device_id() -> str:
     """
     生成随机的x-rpc-device_id
     """
     return str(uuid.uuid4()).upper()
@@ -176,41 +190,54 @@
     """
     cookie_str = ""
     for key in cookie_dict:
         cookie_str += (key + "=" + cookie_dict[key] + ";")
     return cookie_str
 
 
-def generate_ds(data: Union[str, dict, list] = "", params: Union[str, dict] = "",
-                platform: Literal["ios", "android"] = "ios"):
+def generate_ds(data: Union[str, dict, list, None] = None, params: Union[str, dict, None] = None,
+                platform: Literal["ios", "android"] = "ios", salt: Optional[str] = None):
     """
     获取Headers中所需DS
 
     :param data: 可选，网络请求中需要发送的数据
     :param params: 可选，URL参数
     :param platform: 可选，平台，ios或android
+    :param salt: 可选，自定义salt
     """
-    if data == "" and params == "":
+    if data is None and params is None or salt != _conf.salt_config.SALT_PROD:
         if platform == "ios":
-            salt = conf.salt.SALT_IOS
+            salt = salt or _conf.salt_config.SALT_IOS
         else:
-            salt = conf.salt.SALT_ANDROID
+            salt = salt or _conf.salt_config.SALT_ANDROID
         t = str(int(NtpTime.time()))
         a = "".join(random.sample(
             string.ascii_lowercase + string.digits, 6))
         re = hashlib.md5(
             f"salt={salt}&t={t}&r={a}".encode()).hexdigest()
         return f"{t},{a},{re}"
     else:
-        salt = conf.salt.SALT_DATA
+        if params:
+            salt = _conf.salt_config.SALT_PARAMS if not salt else salt
+        else:
+            salt = _conf.salt_config.SALT_DATA if not salt else salt
+
+        if not data:
+            if salt == _conf.salt_config.SALT_PROD:
+                data = {}
+            else:
+                data = ""
+        if not params:
+            params = ""
+
         if not isinstance(data, str):
             data = json.dumps(data)
         if not isinstance(params, str):
             params = urlencode(params)
-            salt = conf.salt.SALT_PARAMS
+
         t = str(int(time.time()))
         r = str(random.randint(100000, 200000))
         c = hashlib.md5(
             f"salt={salt}&t={t}&r={r}&b={data}&q={params}".encode()).hexdigest()
         return f"{t},{r},{c}"
 
 
@@ -219,142 +246,44 @@
     下载文件
 
     :param url: 文件URL
     :param retry: 是否允许重试
     :return: 文件数据
     """
     try:
-        async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry),
-                                                    wait=tenacity.wait_fixed(conf.SLEEP_TIME_RETRY)):
+        async for attempt in get_async_retry(retry):
             with attempt:
                 async with httpx.AsyncClient() as client:
-                    res = await client.get(url, timeout=conf.TIME_OUT, follow_redirects=True)
+                    res = await client.get(url, timeout=_conf.preference.timeout, follow_redirects=True)
                 return res.content
     except tenacity.RetryError:
-        logger.error(f"{conf.LOG_HEAD}下载文件 - {url} 失败")
-        logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
-
-
-def check_login(response: str):
-    """
-    通过网络请求返回的数据，检查是否登录失效
-
-    如果返回数据为`None`，返回`True`
-
-    :param response: 网络请求返回的数据
-    :return: 是否登录失效
-    """
-    try:
-        if response is None:
-            return True
-        res_dict = json.loads(response)
-        if "message" in res_dict:
-            response: str = res_dict["message"]
-            for string in ("Please login", "登录失效", "尚未登录"):
-                if response.find(string) != -1:
-                    return False
-            return True
-    except (json.JSONDecodeError, KeyError):
-        return True
-
-
-def check_ds(response: str):
-    """
-    通过网络请求返回的数据，检查Header中DS是否有效
-
-    如果返回数据为`None`，返回`True`
-
-    :param response: 网络请求返回的数据
-    :return: DS是否有效
-    """
-    try:
-        if response is None:
-            return True
-        res_dict = json.loads(response)
-        if res_dict["message"] == "invalid request":
-            return False
-        else:
-            return True
-    except (json.JSONDecodeError, KeyError):
-        return True
+        logger.error(f"{_conf.preference.log_head}下载文件 - {url} 失败")
+        logger.debug(f"{_conf.preference.log_head}{traceback.format_exc()}")
 
 
 def blur_phone(phone: Union[str, int]) -> str:
     """
     模糊手机号
 
     :param phone: 手机号
     :return: 模糊后的手机号
     """
     if isinstance(phone, int):
         phone = str(phone)
     return f"{phone[:3]}****{phone[-4:]}"
 
 
-class Subscribe:
-    """
-    在线配置相关(需实例化)
-    """
-    URL = os.path.join(
-        conf.GITHUB_PROXY, "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/raw/dev/subscribe/config.json")
-    conf_list: List[Dict[str, Any]] = []
-    '''当前插件版本可用的配置资源'''
-
-    def __init__(self):
-        self.index = 0
-
-    @classmethod
-    async def download(cls) -> bool:
-        """
-        读取在线配置资源
-        :return: 是否成功
-        """
-        try:
-            for attempt in tenacity.Retrying(stop=custom_attempt_times(True)):
-                with attempt:
-                    file = await get_file(cls.URL)
-                    file = json.loads(file.decode())
-                    if not file:
-                        return False
-                    cls.conf_list = list(
-                        filter(lambda co: PLUGIN.metadata.extra["version"] in co["version"], file))
-                    cls.conf_list.sort(
-                        key=lambda co: conf["time"], reverse=True)
-                    return True
-        except (json.JSONDecodeError, KeyError):
-            logger.error(f"{conf.LOG_HEAD}获取在线配置资源 - 解析文件失败")
-            return False
-
-    async def load(self, force: bool = False) -> bool:
-        """
-        优先加载来自网络的配置，若获取失败，则返回本地默认配置。\n
-        若下载失败返回`False`
-
-        :param force: 是否强制在线读取配置，而不使用本地缓存的
-        """
-        success = True
-        if not Subscribe.conf_list or force or self.index >= len(Subscribe.conf_list):
-            logger.info(f"{conf.LOG_HEAD}读取配置 - 开始下载配置...")
-            success = await self.download()
-            self.index = 0
-        if not success:
-            return False
-        else:
-            conf.parse_obj(Subscribe.conf_list[self.index]["config"])
-            self.index += 1
-            return True
-
 # TODO: 一个用于构建on_command事件相应器的函数，
 #  将使用偏好设置里的priority优先级和block设置，
 #  可能可以作为装饰器使用
 #   （需要先等用户数据改用Pydantic作为数据模型）
 def command_matcher(command: str, priority: int = None, block: bool = None) -> Matcher:
     """
     用于构建on_command事件相应器的函数，
     将使用偏好设置里的priority优先级和block设置
 
     :param command: 指令名
     :param priority: 优先级，为 None 则读取偏好设置
     :param block: 是否阻塞，为 None 则读取偏好设置
     :return: 事件响应器
     """
-    ...
+    ...
```

### Comparing `nonebot_plugin_mystool-0.2.9/PKG-INFO` & `nonebot_plugin_mystool-1.0.0b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 0.2.9
+Version: 1.0.0b1
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: Pillow (>=9.5.0,<10.0.0)
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot_adapter_onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
 Requires-Dist: ntplib (>=0.4.0,<0.5.0)
-Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues
 Project-URL: Documentation, https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki
 Project-URL: Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 Description-Content-Type: text/markdown
 
 ```
@@ -40,18 +39,33 @@
   <img alt="CodeFactor" src="https://www.codefactor.io/repository/github/ljzd-pro/nonebot-plugin-mystool/badge?style=for-the-badge">
   <img alt="最新发行版" src="https://img.shields.io/github/v/release/Ljzd-PRO/nonebot-plugin-mysTool?logo=python&style=for-the-badge">
   <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.9**
+**版本 - v1.0.0-beta.1**
 
 ### 📣 更新内容
 
+#### 2023.6.10
+
+改动较大，目前是 Beta 版，可能不稳定
+
+- 大量的代码重构，包括米游社API的客户端实现、用户数据相关、插件配置相关、API相关数据模型
+- 修复在 Windows 下无法多进程生成商品图片的问题
+- 从显示用户账号绑定的手机号改为显示账号的米游社ID
+- 设置、兑换计划功能支持群聊使用
+- 登陆绑定只需要进行一次短信验证
+- 用户数据文件、插件配置文件 **格式更新，与 v1.0.0 之前的版本不兼容**
+- 修复添加兑换任务时出现的UID不存在错误
+- 修复商品图片生成完才发出后台正在生成提示的问题
+- 异常捕获更加准确
+- 改进了一些文本
+
 #### 2023.5.18
 - 多进程生成商品图片（多核），加快图片生成速度
 - 修复部分商品兑换时间错误的问题（如米游社商品晚了一周）
 
 #### 2023.5.4
 - 增加对星穹铁道的签到功能的支持 - [#89](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/89) by @ayakasuki
 - 修复插件命令优先度问题 - [#88](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/88) by @ayakasuki
@@ -87,15 +101,15 @@
 
 #### 插件命令
 
 ```
 /帮助
 ```
 
-> ⚠️ 注意 此处没有使用 [🔗 插件命令头](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Configuration-Config#command_start)
+> ⚠️ 注意 此处没有使用 [🔗 插件命令头](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Configuration-Config#commandstart)
 
 ## 其他
 
 ### [📃源码说明](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Source-Structure)
 ### 适配 [绪山真寻Bot](https://github.com/HibiKier/zhenxun_bot) 的分支
 - https://github.com/MWTJC/zhenxun-plugin-mystool
 - https://github.com/ayakasuki/nonebot-plugin-mystool
```

