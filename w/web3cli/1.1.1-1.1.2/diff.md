# Comparing `tmp/web3cli-1.1.1.tar.gz` & `tmp/web3cli-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.1.1.tar", last modified: Sat Jun 10 16:09:13 2023, max compression
+gzip compressed data, was "web3cli-1.1.2.tar", last modified: Sat Jun 10 18:04:07 2023, max compression
```

## Comparing `web3cli-1.1.1.tar` & `web3cli-1.1.2.tar`

### file list

```diff
@@ -1,172 +1,173 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.1/LICENSE
--rw-r--r--   0        0        0    12030 2023-06-10 16:07:05.654200 web3cli-1.1.1/README.md
--rw-r--r--   0        0        0     4026 2023-06-10 16:08:22.610889 web3cli-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.1/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.1/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.1/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.1.1/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.1.1/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.1.1/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.1.1/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.1.1/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.1/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.1/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.1.1/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.1.1/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4795 2023-05-31 08:43:28.096742 web3cli-1.1.1/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.1.1/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.1.1/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.1.1/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.1.1/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.1.1/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     4330 2023-05-31 11:18:25.258680 web3cli-1.1.1/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     4461 2023-06-08 17:37:43.908413 web3cli-1.1.1/src/web3cli/controllers/replay_controller.py
--rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.1.1/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     3890 2023-06-10 16:05:25.285160 web3cli-1.1.1/src/web3cli/controllers/subscribe_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.1/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     7872 2023-06-08 18:14:50.319839 web3cli-1.1.1/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.1/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1408 2023-06-07 17:07:38.026919 web3cli-1.1.1/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.1/src/web3cli/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.1/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    16208 2023-06-10 14:17:47.976710 web3cli-1.1.1/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.1/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.1/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.1/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.1/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     2163 2023-06-10 14:00:37.541209 web3cli-1.1.1/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.1/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.1/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.1/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-06-10 16:08:13.624292 web3cli-1.1.1/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.1/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7544 2023-06-10 15:35:59.359874 web3cli-1.1.1/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.1/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.1/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.1/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.1/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.1/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.1/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.1/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.1/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.1/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.1/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.1/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.1/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.1/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.1/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.1/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.1/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.1/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.1/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.1/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.1/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.1.1/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.1/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.1/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.1/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.1/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.1/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.1/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.1/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.1/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.1/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.1/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.1/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.1/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.1/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.1/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.1/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.1/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.1/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.1/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.1/src/web3core/seeds/contracts/erat_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.1/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.1/src/web3core/seeds/contracts/gno_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.1/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.1/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.1/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.1/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.1/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.1/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.1/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.1/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.1/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.1/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.1/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.1/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.1/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.1/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.1/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.1/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.1/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.1/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-06-10 16:08:27.555321 web3cli-1.1.1/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.1/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.1/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.1/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.1/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.1/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.1/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.1/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.1/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.1/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.1/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.1/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.1/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.1/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.1/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.1/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.1/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.1/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.1/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.1/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.1/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.1/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.1.1/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.1/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.1/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.1.1/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.1.1/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     6446 2023-06-08 18:14:50.320112 web3cli-1.1.1/tests/web3cli/controllers/crud/test_token_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.1/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.1.1/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.1.1/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.1.1/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     6099 2023-05-31 11:22:03.092128 web3cli-1.1.1/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.1/tests/web3cli/controllers/test_replay_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.1/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.1/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.1/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.1/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.1/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.1/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.1/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.1/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.1/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.1/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.1/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.1/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.1/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.1/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.1/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.1/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.1/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 web3cli-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.2/LICENSE
+-rw-r--r--   0        0        0    12030 2023-06-10 16:07:05.654200 web3cli-1.1.2/README.md
+-rw-r--r--   0        0        0     4026 2023-06-10 18:03:56.702529 web3cli-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.2/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.2/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.2/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4679 2023-06-10 16:49:18.164306 web3cli-1.1.2/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2049 2023-06-10 16:26:02.765052 web3cli-1.1.2/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1215 2023-06-10 16:26:21.840704 web3cli-1.1.2/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3106 2023-06-10 17:02:35.846994 web3cli-1.1.2/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2421 2023-06-10 16:26:42.723101 web3cli-1.1.2/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.2/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.2/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2530 2023-06-10 16:49:44.923130 web3cli-1.1.2/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4413 2023-06-10 16:50:02.537767 web3cli-1.1.2/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4785 2023-06-10 16:50:16.263301 web3cli-1.1.2/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3035 2023-06-10 16:21:12.060981 web3cli-1.1.2/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2972 2023-06-10 16:35:01.955138 web3cli-1.1.2/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5282 2023-06-10 16:51:30.999842 web3cli-1.1.2/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1390 2023-06-10 16:27:14.395424 web3cli-1.1.2/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1479 2023-06-10 16:29:57.178158 web3cli-1.1.2/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     4219 2023-06-10 17:56:43.550809 web3cli-1.1.2/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     4471 2023-06-10 16:33:44.421618 web3cli-1.1.2/src/web3cli/controllers/replay_controller.py
+-rw-r--r--   0        0        0     2403 2023-06-10 16:33:58.579948 web3cli-1.1.2/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     3890 2023-06-10 16:05:25.285160 web3cli-1.1.2/src/web3cli/controllers/subscribe_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.2/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     7848 2023-06-10 17:57:16.099321 web3cli-1.1.2/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.2/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1239 2023-06-10 17:31:55.330976 web3cli-1.1.2/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.2/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0     1329 2023-06-10 18:02:03.918760 web3cli-1.1.2/src/web3cli/framework/ext_print.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.2/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    16208 2023-06-10 14:17:47.976710 web3cli-1.1.2/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.2/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.2/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.2/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.2/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     2096 2023-06-10 18:03:21.873718 web3cli-1.1.2/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.2/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.2/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.2/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-06-10 18:03:42.667453 web3cli-1.1.2/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.2/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7566 2023-06-10 17:41:37.275895 web3cli-1.1.2/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.2/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.2/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.2/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.2/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.2/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.2/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.2/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.2/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.2/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.2/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.2/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.2/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.2/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.2/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.2/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.2/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.2/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.2/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.2/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.2/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.1.2/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.2/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.2/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.2/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.2/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.2/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.2/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.2/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.2/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.2/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.2/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.2/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.2/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.2/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.2/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.2/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.2/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.2/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.2/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.2/src/web3core/seeds/contracts/erat_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.2/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.2/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.2/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.2/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.2/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.2/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.2/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.2/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.2/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.2/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.2/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.2/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.2/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.2/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.2/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.2/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.2/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.2/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.2/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.2/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-06-10 18:04:00.512875 web3cli-1.1.2/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.2/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.2/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.2/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.2/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.2/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.2/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.2/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.2/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.2/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.2/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.2/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.2/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.2/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.2/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.2/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.2/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.2/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.2/tests/ape/tests/token/test_ape_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.2/tests/ape/tests/token/test_ape_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.2/tests/ape/tests/token/test_ape_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.2/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.2/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.2/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.2/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.2/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.2/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.2/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.2/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3510 2023-06-10 17:49:12.472139 web3cli-1.1.2/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.2/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.2/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3741 2023-06-10 17:49:22.329714 web3cli-1.1.2/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4912 2023-06-10 17:49:27.241897 web3cli-1.1.2/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     6497 2023-06-10 17:50:24.793662 web3cli-1.1.2/tests/web3cli/controllers/crud/test_token_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.2/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6385 2023-06-10 17:54:02.470548 web3cli-1.1.2/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1027 2023-06-10 17:47:40.979271 web3cli-1.1.2/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1664 2023-06-10 18:03:21.873923 web3cli-1.1.2/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     6102 2023-06-10 18:00:00.614466 web3cli-1.1.2/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.2/tests/web3cli/controllers/test_replay_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.2/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.2/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.2/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.2/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.2/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.2/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.2/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.2/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.2/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.2/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.2/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.2/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.2/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.2/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.2/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.2/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.2/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 web3cli-1.1.2/PKG-INFO
```

### Comparing `web3cli-1.1.1/LICENSE` & `web3cli-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/README.md` & `web3cli-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/pyproject.toml` & `web3cli-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.1.1"
+version = "1.1.2"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3cli-1.1.1/src/web3cli/.DS_Store` & `web3cli-1.1.2/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/controllers/abi_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/abi_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from cement import ex
 from web3.types import ABI
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
-from web3cli.helpers.render import render_json
+from web3cli.helpers.render import render
 from web3core.helpers.abi import (
     filter_abi_by_type_and_name,
     get_event_full_signatures,
     get_event_signatures,
     get_function_full_signatures,
     get_function_signatures,
 )
@@ -54,15 +54,15 @@
     def functions(self) -> None:
         abi = self.parse_abi()
         functions = (
             get_function_full_signatures(abi)
             if self.app.pargs.full
             else get_function_signatures(abi)
         )
-        render_json(self.app, sorted(functions, key=str.lower))
+        render(self.app, sorted(functions, key=str.lower))
 
     @ex(
         help="List the events in the given contract, contract type or ABI string, with signatures",
         arguments=[
             (
                 ["contract"],
                 {
@@ -88,15 +88,15 @@
     def events(self) -> None:
         abi = self.parse_abi()
         events = (
             get_event_full_signatures(abi)
             if self.app.pargs.full
             else get_event_signatures(abi)
         )
-        render_json(self.app, sorted(events, key=str.lower))
+        render(self.app, sorted(events, key=str.lower))
 
     @ex(
         help="Show the ABI of a specific contract function or event",
         arguments=[
             (
                 ["contract"],
                 {"help": "Name of the contract or contract type in the database"},
@@ -110,15 +110,15 @@
         obj = filter_abi_by_type_and_name(
             abi, type=None, name=self.app.pargs.function_name
         )
         if not obj:
             self.app.log.warning(
                 f"Function or event '{self.app.pargs.function_name}' not found"
             )
-        render_json(self.app, obj)
+        render(self.app, obj)
 
     def parse_abi(self) -> ABI:
         """Parse the 'contract' and '--abi' arguments and return the ABI"""
         # Contract name given, try to retrieve the ABI from the database
         if self.app.pargs.contract:
             # Try to retrieve ABI from contracts table
             contract = Contract.get_by_name_and_chain(
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/app_key_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
 from web3cli.helpers.config import update_setting_in_config_file
+from web3cli.helpers.render import render
 
 
 class AppKeyController(Controller):
     """Handler of the `w3 app-key` commands"""
 
     class Meta:
         label = "app-key"
@@ -52,8 +53,8 @@
             )
 
     @ex(
         help="generate and show a new random password, suitable to encrypt a private key; the password will not be stored anywhere, so take note of it if you want to use it!",
     )
     def generate(self) -> None:
         key = secrets.token_bytes(32)
-        self.app.print(str(key))
+        render(self.app, str(key))
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/base_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/base_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
+from web3cli.helpers.render import render
 from web3cli.helpers.version import get_version_message
 
 
 class BaseController(Controller):
     """Base controller. Can be used to implement global arguments"""
 
     class Meta:
@@ -23,15 +24,15 @@
                 ["-v", "--version"],
                 {"action": "version", "version": get_version_message()},
             )
         ]
 
     @ex(help="Show the version of web3cli")
     def version(self) -> None:
-        self.app.print(get_version_message())
+        render(self.app, get_version_message())
 
     def _post_argument_parsing(self) -> None:
         """Parse global arguments"""
 
         # Do nothing if no command is invoked (for example
         # if one simply runs `w3` or `w3 db`)
         if not args.get_command(self.app):
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/call_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/call_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.args import parse_block
 from web3cli.helpers.client_factory import make_contract_client
-from web3cli.helpers.render import render_json
+from web3cli.helpers.render import render
 from web3core.helpers.abi import (
     does_function_write_to_state,
     get_function_abis,
     parse_abi_values,
 )
 from web3core.helpers.resolve import resolve_address
 
@@ -76,8 +76,8 @@
         # Call the function
         if from_address is None:
             result = function(*function_args).call(block_identifier=block)
         else:  # from address needed
             result = function(*function_args).call(
                 {"from": from_address}, block_identifier=block
             )
-        render_json(self.app, result)
+        render(self.app, result)
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/config_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/config_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers.config import update_setting_in_config_file
+from web3cli.helpers.render import render, render_yaml
 
 
 class ConfigController(Controller):
     """Handler of the `w3 config` commands"""
 
     class Meta:
         label = "config"
@@ -26,21 +27,21 @@
                     "nargs": "?",
                 },
             ),
         ],
     )
     def get(self) -> None:
         if self.app.pargs.setting:
-            self.app.print(self.app.config.get("web3cli", self.app.pargs.setting))
+            render(self.app, self.app.config.get("web3cli", self.app.pargs.setting))
         else:
             output = {}
             all_config = self.app.config.get_dict()
             for section in ["web3cli"]:
                 output[section] = all_config[section]
-            self.app.render(output, handler="yaml")
+            render_yaml(self.app, output)
 
     @ex(
         help="set the value of a setting. IMPORTANT: supports only string settings!",
         arguments=[
             (
                 ["setting"],
                 {
@@ -71,8 +72,8 @@
             value=self.app.pargs.value,
             do_log=True,
             is_global=self.app.pargs.is_global,
         )
 
     @ex(help="show the location of the configuration files")
     def where(self) -> None:
-        self.app.print("\n".join(self.app.Meta.config_files))
+        render(self.app, "\n".join(self.app.Meta.config_files))
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/controller.py` & `web3cli-1.1.2/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/address_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
-from web3cli.helpers.render import render_json, render_table
+from web3cli.helpers.render import render, render_table
 from web3core.models.address import Address
 
 
 class AddressController(Controller):
     """Handler of the `w3 address` CRUD commands"""
 
     class Meta:
@@ -30,15 +30,15 @@
     @ex(
         help="show the details of the given address by name",
         arguments=[
             (["name"], {"help": "name of the address to show"}),
         ],
     )
     def get(self) -> None:
-        render_json(self.app, Address.get_as_dict(Address.name == self.app.pargs.name))
+        render(self.app, Address.get_as_dict(Address.name == self.app.pargs.name))
 
     @ex(
         help="add a new address",
         arguments=[
             (["name"], {"help": "name of the address"}),
             (["address"], {"help": "blockchain address (0x...)"}),
             (["-d", "--desc"], {"action": "store"}),
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/chain_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
-from web3cli.helpers.render import render_json, render_table
+from web3cli.helpers.render import render, render_table
 from web3core.exceptions import ChainNotFound
 from web3core.models.chain import Chain
 from web3core.seeds import chain_seeds
 
 
 class ChainController(Controller):
     """Handler of the `w3 chain` CRUD commands"""
@@ -97,19 +97,19 @@
         )
 
     @ex(
         help="show the details of the given chain",
         arguments=[(["name"], {"help": "the name of the chain to look up"})],
     )
     def get(self) -> None:
-        render_json(self.app, Chain.get_as_dict(Chain.name == self.app.pargs.name))
+        render(self.app, Chain.get_as_dict(Chain.name == self.app.pargs.name))
 
     @ex(help="get the active chain's name", arguments=[args.chain()])
     def active(self) -> None:
-        self.app.print(self.app.chain.name)
+        render(self.app, self.app.chain.name)
 
     @ex(
         help="delete a chain",
         arguments=[
             (["name"], {"help": "name of the chain to delete"}),
         ],
     )
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/contract_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cement import ex
 from playhouse.shortcuts import model_to_dict
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
-from web3cli.helpers.render import render_json, render_table
+from web3cli.helpers.render import render, render_table
 from web3core.helpers.seed import seed_contracts
 from web3core.models.contract import Contract
 from web3core.seeds import contract_seeds
 
 
 class ContractController(Controller):
     """Handler of the `w3 contract` CRUD commands"""
@@ -53,15 +53,15 @@
             args.chain(),
         ],
     )
     def get(self) -> None:
         contract = Contract.get_by_name_and_chain_or_raise(
             self.app.pargs.name, self.app.chain.name
         )
-        render_json(self.app, model_to_dict(contract))
+        render(self.app, model_to_dict(contract))
 
     @ex(
         help="add a new contract to the database",
         arguments=[
             (["name"], {"help": "name of the contract, for reference"}),
             (["-d", "--desc"], {"action": "store"}),
             (
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/history_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cement import ex
 from playhouse.shortcuts import model_to_dict
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
-from web3cli.helpers.render import render_table
+from web3cli.helpers.render import render, render_table
 from web3core.helpers.format import cut
 from web3core.models.tx import Tx
 
 
 class HistoryController(Controller):
     """Handler of the `w3 history` CRUD commands"""
 
@@ -34,15 +34,15 @@
         help="show details of the given transaction in the history",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
         ],
     )
     def get(self) -> None:
         tx = Tx.get_by_hash_or_raise(self.app.pargs.hash)
-        self.app.render(model_to_dict(tx), indent=4, handler="json")
+        render(self.app, model_to_dict(tx))
 
     @ex(
         help="add a new transaction to the history",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
             (
                 ["from"],
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
-from web3cli.helpers.render import render_table
+from web3cli.helpers.render import render, render_table
 from web3core.models.chain import Rpc
 
 
 class RpcController(Controller):
     """Handler of the `w3 rpc` CRUD commands"""
 
     class Meta:
@@ -55,15 +55,15 @@
                     "type": int,
                 },
             ),
         ],
     )
     def get_url(self) -> None:
         rpc = Rpc.get(self.app.pargs.id)
-        self.app.print(rpc.url)
+        render(self.app, rpc.url)
 
     @ex(
         help="show the URL of an RPC by its ID; without arguments, shows the RPC that will be used by the CLI",
         arguments=[
             (
                 ["id"],
                 {
@@ -75,18 +75,18 @@
             *args.chain_and_rpc(),
         ],
     )
     def get(self) -> None:
         # Case 1: Show the URL of the RPC with the given ID
         if self.app.pargs.id:
             rpc = Rpc.get(self.app.pargs.id)
-            self.app.print(rpc.url)
+            render(self.app, rpc.url)
         # Case 2: RPC was forced via CLI argument
         else:
-            self.app.print(self.app.rpc.url)
+            render(self.app, self.app.rpc.url)
 
     @ex(
         help="delete one or more rpcs",
         arguments=[
             (
                 ["ids"],
                 {
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/crud/signer_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from cement import ex
 from eth_account import Account
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.crypto import decrypt_keyfile, encrypt_string_with_app_key
-from web3cli.helpers.render import render_json, render_table
+from web3cli.helpers.render import render, render_table
 from web3cli.helpers.signer import get_signer
 from web3core.exceptions import KeyIsInvalid, SignerNotFound
 from web3core.helpers.misc import are_mutually_exclusive
 from web3core.models.signer import Signer
 
 
 class SignerController(Controller):
@@ -44,15 +44,15 @@
                 },
             )
         ],
     )
     def get(self) -> None:
         signer = get_signer(self.app, self.app.pargs.name).as_dict()
         signer["key"] = "********"
-        render_json(self.app, signer)
+        render(self.app, signer)
 
     @ex(
         help="show the active signer's address",
         arguments=[
             (
                 ["--show-name"],
                 {
@@ -61,17 +61,17 @@
                 },
             ),
             args.signer(),
         ],
     )
     def active(self) -> None:
         if self.app.pargs.show_name:
-            self.app.print(self.app.signer.name)
+            render(self.app, self.app.signer.name)
         else:
-            self.app.print(self.app.signer.address)
+            render(self.app, self.app.signer.address)
 
     @ex(
         help="add a new signer; you will be asked for the private key",
         arguments=[
             (["name"], {"help": "name identifying the signer"}),
             (
                 ["--create"],
@@ -135,15 +135,15 @@
             address=address,
         )
         self.app.log.info(
             f"Signer '{self.app.pargs.name}' added correctly (address={address})"
         )
         if self.app.pargs.create:
             # Print private key
-            self.app.print(key)
+            render(self.app, key)
 
     @ex(
         help="delete a signer",
         arguments=[
             (["name"], {"help": "name of the signer to delete"}),
         ],
     )
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/db_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/db_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
 from web3cli.helpers.database import delete_db_file, get_db_filepath
+from web3cli.helpers.render import render
 from web3core.helpers.misc import yes_or_exit
 
 
 class DbController(Controller):
     """Base controller for the `w3 db` command"""
 
     class Meta:
@@ -32,8 +33,8 @@
         if delete_db_file(self.app):
             self.app.log.info(f"Database file deleted ({db_path})")
         else:
             self.app.log.info(f"Database not found at {db_path}")
 
     @ex(help="show the path of the database file")
     def where(self) -> None:
-        self.app.print(get_db_filepath(self.app))
+        render(self.app, get_db_filepath(self.app))
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/keyfile_controller.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers.crypto import decrypt_keyfile, encrypt_to_keyfile
+from web3cli.helpers.render import render
 
 
 class KeyfileController(Controller):
     """Handler of the `w3 keyfile` commands"""
 
     class Meta:
         label = "keyfile"
@@ -20,15 +21,15 @@
         arguments=[
             (["path"], {"help": "path to input keyfile (JSON)"}),
         ],
         aliases=["decrypt"],
     )
     def decode(self) -> None:
         key = decrypt_keyfile(self.app.pargs.path)
-        self.app.print(key.replace("0x", ""))
+        render(self.app, key.replace("0x", ""))
 
     @ex(
         help="Create a new keyfile from a private key",
         arguments=[
             (
                 ["path"],
                 {
@@ -41,8 +42,8 @@
     )
     def create(self) -> None:
         keyfile_dict = encrypt_to_keyfile()
         if self.app.pargs.path:
             json.dump(keyfile_dict, open(self.app.pargs.path, "w"))
             self.app.log.info(f"Keyfile saved to {self.app.pargs.path}")
         else:
-            self.app.print(json.dumps(keyfile_dict))
+            render(self.app, json.dumps(keyfile_dict))
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/misc_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/misc_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import json
 from pprint import pformat
 
 from cement import ex
 from web3 import Web3
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.args import parse_block
 from web3cli.helpers.client_factory import make_client
-from web3cli.helpers.render import render_balance, render_number
+from web3cli.helpers.render import render, render_balance
 from web3core.helpers.client_factory import make_base_wallet
 from web3core.helpers.resolve import resolve_address
 
 
 class MiscController(Controller):
     """Handler of simple top-level commands"""
 
@@ -59,45 +58,44 @@
     )
     def tx_count(self) -> None:
         address = resolve_address(self.app.pargs.address, chain=self.app.chain.name)
         nonce = make_client(self.app).w3.eth.get_transaction_count(
             Web3.to_checksum_address(address),
             block_identifier=parse_block(self.app, "block"),
         )
-        render_number(self.app, nonce)
+        render(self.app, nonce)
 
     @ex(
         help="Get the latest block, or the block corresponding to the given identifier",
         arguments=[args.block("block_identifier", nargs="?"), *args.chain_and_rpc()],
     )
     def block(self) -> None:
         block_identifier = parse_block(self.app, "block_identifier")
         block = make_client(self.app).w3.eth.get_block(block_identifier)
-        block_as_dict = json.loads(Web3.to_json(block))
-        self.app.render(block_as_dict, indent=4, handler="json")
+        render(self.app, block)
 
     @ex(
         help="Sign the given message and show the signed message, as returned by web3.py",
         arguments=[(["msg"], {"action": "store"}), args.signer()],
     )
     def sign(self) -> None:
         wallet = make_base_wallet(
             chain=None, signer=self.app.signer, password=self.app.app_key, node_uri=None
         )
         signed_message = wallet.sign_message(self.app.pargs.msg)
-        self.app.print(pformat(signed_message._asdict()))
+        render(self.app, pformat(signed_message._asdict()))
 
     @ex(
         help="Get the current gas price in gwei by calling the eth_gasPrice method. For EIP1559 chains, this should return the max priority fee per gas.",
         arguments=[*args.chain_and_rpc()],
     )
     def gas_price(self) -> None:
         gas_price_in_wei = make_client(self.app).w3.eth.gas_price
         gas_price_in_gwei = Web3.from_wei(gas_price_in_wei, "gwei")
-        self.app.render(gas_price_in_gwei)
+        render(self.app, gas_price_in_gwei)
 
     @ex(
         help="Get the base fee in gwei of the last block. Will error for non-EIP1559 chains.",
         arguments=[*args.chain_and_rpc()],
     )
     def base_fee(self) -> None:
         try:
@@ -105,8 +103,8 @@
                 "baseFeePerGas"
             ]
         except KeyError:
             raise Web3CliError(
                 f"Could not find base fee. Please check that chain '{self.app.chain.name}' is EIP-1599 compatible."
             )
         base_fee_in_gwei = Web3.from_wei(base_fee_in_wei, "gwei")
-        self.app.render(base_fee_in_gwei)
+        render(self.app, base_fee_in_gwei)
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/replay_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/replay_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.client_factory import make_client, make_wallet
-from web3cli.helpers.render import render_web3py
+from web3cli.helpers.render import render, render_web3py
 from web3core.helpers.misc import yes_or_exit
 
 
 class ReplayController(Controller):
     """Handler of the `w3 replay` commands"""
 
     class Meta:
@@ -107,8 +107,8 @@
         try:
             tx_hash = signer.sign_and_send_tx(tx)
         except TypeError as e:
             raise Web3CliError(
                 f"Failed to send transaction: {e}. "
                 f"Try using the flag --type {self.app.chain.tx_type} to prevent type-related errors."
             )
-        self.app.print(tx_hash)
+        render(self.app, tx_hash)
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/send_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/send_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
+from web3cli.helpers.render import render
 from web3cli.helpers.send import send_coin_or_token
 from web3core.helpers.misc import to_number, yes_or_exit
 from web3core.helpers.resolve import resolve_address
 from web3core.models.address import Address
 from web3core.models.signer import Signer
 
 
@@ -61,8 +62,8 @@
         tx_hash = send_coin_or_token(
             self.app,
             ticker=ticker,
             to=to_address,
             amount=amount,
             unit=self.app.pargs.unit,
         )
-        self.app.print(tx_hash)
+        render(self.app, tx_hash)
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/subscribe_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/subscribe_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/controllers/swap_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/controllers/token_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/token_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from cement import ex
 
 from web3cli.controllers.controller import Controller
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers import args
 from web3cli.helpers.client_factory import make_contract_client, make_contract_wallet
-from web3cli.helpers.render import render_number, render_table, render_web3py
+from web3cli.helpers.render import render, render_table, render_web3py
 from web3cli.helpers.tx import send_contract_tx
 from web3core.helpers.misc import yes_or_exit
 from web3core.helpers.resolve import resolve_address
 from web3core.models.contract import Contract
 
 
 class TokenController(Controller):
@@ -105,18 +105,18 @@
         ],
     )
     def balance(self) -> None:
         address = resolve_address(self.app.pargs.address, chain=self.app.chain.name)
         client = make_contract_client(self.app, self.app.pargs.token)
         balance_in_wei = client.functions["balanceOf"](address).call()
         if self.app.pargs.wei:
-            render_number(self.app, balance_in_wei)
+            render(self.app, balance_in_wei)
         else:
             balance = balance_in_wei / 10 ** client.functions["decimals"]().call()
-            render_number(self.app, balance)
+            render(self.app, balance)
 
     @ex(
         help="Return the allowance of the given spender to spend the given token for the given address",
         arguments=[
             (["token"], {"help": "Token to check, by name"}),
             (["owner"], {"help": "Address or name of the account to check"}),
             (["spender"], {"help": "Address or name of the spender to check"}),
@@ -128,15 +128,15 @@
         spender = resolve_address(self.app.pargs.spender, chain=self.app.chain.name)
         owner = resolve_address(self.app.pargs.owner, chain=self.app.chain.name)
         # Initialize client
         client = make_contract_client(self.app, self.app.pargs.token)
         decimals = client.functions["decimals"]().call()
         allowance_in_wei = client.functions["allowance"](owner, spender).call()
         allowance = allowance_in_wei / 10**decimals
-        self.app.print(str(allowance))
+        render(self.app, allowance)
 
     #    ____                      _
     #   / ___|  _ __   _   _    __| |
     #  | |     | '__| | | | |  / _` |
     #  | |___  | |    | |_| | | (_| |
     #   \____| |_|     \__,_|  \__,_|
```

### Comparing `web3cli-1.1.1/src/web3cli/controllers/transact_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/controllers/tx_controller.py` & `web3cli-1.1.2/src/web3cli/controllers/tx_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import json
-
 from cement import ex
-from web3 import Web3
 
 from web3cli.controllers.controller import Controller
 from web3cli.helpers import args
 from web3cli.helpers.client_factory import make_client
+from web3cli.helpers.render import render
 
 
 class TxController(Controller):
     """Handler of the `w3 tx` commands"""
 
     class Meta:
         label = "tx"
@@ -23,23 +21,21 @@
             (["hash"], {"help": "hash of the transaction"}),
             *args.chain_and_rpc(),
         ],
     )
     def get(self) -> None:
         client = make_client(self.app)
         tx = client.w3.eth.get_transaction(self.app.pargs.hash)
-        tx_as_dict = json.loads(Web3.to_json(tx))
-        self.app.render(tx_as_dict, indent=4, handler="json")
+        render(self.app, tx)
 
     @ex(
         help="fetch the receipt of the given transaction from the blockchain",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
             *args.chain_and_rpc(),
         ],
         aliases=["rc"],
     )
     def get_receipt(self) -> None:
         client = make_client(self.app)
         receipt = client.w3.eth.wait_for_transaction_receipt(self.app.pargs.hash)
-        receipt_as_dict = json.loads(Web3.to_json(receipt))
-        self.app.render(receipt_as_dict, indent=4, handler="json")
+        render(self.app, receipt)
```

### Comparing `web3cli-1.1.1/src/web3cli/helpers/args.py` & `web3cli-1.1.2/src/web3cli/helpers/args.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/client_factory.py` & `web3cli-1.1.2/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/config.py` & `web3cli-1.1.2/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/crypto.py` & `web3cli-1.1.2/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/database.py` & `web3cli-1.1.2/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/send.py` & `web3cli-1.1.2/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/signer.py` & `web3cli-1.1.2/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/helpers/tx.py` & `web3cli-1.1.2/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/hooks.py` & `web3cli-1.1.2/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3cli/main.py` & `web3cli-1.1.2/src/web3cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         # load additional framework extensions
         extensions = [
             "yaml",
             "json",
             "colorlog",
             "jinja2",
-            "print",
+            "web3cli.framework.ext_print",
             "tabulate",
         ]
 
         # configuration handler
         config_handler = "yaml"
 
         # Path of configuration file(s).
```

### Comparing `web3cli-1.1.1/src/web3core/exceptions.py` & `web3cli-1.1.2/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/abi.py` & `web3cli-1.1.2/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/blocks.py` & `web3cli-1.1.2/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/client_factory.py` & `web3cli-1.1.2/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/crypto.py` & `web3cli-1.1.2/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/database.py` & `web3cli-1.1.2/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/dex.py` & `web3cli-1.1.2/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/misc.py` & `web3cli-1.1.2/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/os.py` & `web3cli-1.1.2/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/resolve.py` & `web3cli-1.1.2/src/web3core/helpers/resolve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/rpc.py` & `web3cli-1.1.2/src/web3core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/seed.py` & `web3cli-1.1.2/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/tx.py` & `web3cli-1.1.2/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/helpers/yaml.py` & `web3cli-1.1.2/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/address.py` & `web3cli-1.1.2/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/base_model.py` & `web3cli-1.1.2/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/chain.py` & `web3cli-1.1.2/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/contract.py` & `web3cli-1.1.2/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/signer.py` & `web3cli-1.1.2/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/timestamps_model.py` & `web3cli-1.1.2/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/tx.py` & `web3cli-1.1.2/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/models/types.py` & `web3cli-1.1.2/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/chain_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/chain_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/bnb_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/bnb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/erat_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/erat_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/seeds/contracts/gno_contract_seeds.py` & `web3cli-1.1.2/src/web3core/seeds/contracts/gno_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/src/web3core/types.py` & `web3cli-1.1.2/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/.DS_Store` & `web3cli-1.1.2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.DS_Store` & `web3cli-1.1.2/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.1.2/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.1.2/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_Math.json` & `web3cli-1.1.2/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.1.2/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.1.2/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IERC20.json` & `web3cli-1.1.2/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.1.2/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_IWETH.json` & `web3cli-1.1.2/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.1.2/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.1.2/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.1.2/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Token.json` & `web3cli-1.1.2/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.1.2/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.1.2/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.1.2/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.1.2/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.1.2/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/.build/__local__.json` & `web3cli-1.1.2/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/.DS_Store` & `web3cli-1.1.2/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/token/Token.sol` & `web3cli-1.1.2/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.1.2/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.1.2/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.1.2/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.1.2/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/fixtures.py` & `web3cli-1.1.2/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/helpers/token.py` & `web3cli-1.1.2/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.1.2/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_approve.py` & `web3cli-1.1.2/tests/ape/tests/token/test_ape_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transfer.py` & `web3cli-1.1.2/tests/ape/tests/token/test_ape_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transferFrom.py` & `web3cli-1.1.2/tests/ape/tests/token/test_ape_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py` & `web3cli-1.1.2/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py` & `web3cli-1.1.2/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/helper.py` & `web3cli-1.1.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/seed.py` & `web3cli-1.1.2/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 def test_chain_active(chains: List[ChainFields]) -> None:
     for chain in chains:
         with Web3CliTest() as app:
             seed_chains(chains)
             app.config.set("web3cli", "default_chain", chain["name"])
             app.set_args(["chain", "active"]).run()
             data, output = app.last_rendered
-            assert data["out"] == chain["name"]
+            assert data == chain["name"]
 
 
 def test_chain_delete(chains: List[ChainFields]) -> None:
     for c in chains:
         with Web3CliTest() as app:
             seed_chains(chains)
             app.set_args(
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,37 +49,37 @@
     with Web3CliTest() as app:
         seed_chains(chains)
         rpcs = Rpc.get_all()
     for rpc in rpcs:
         with Web3CliTest(delete_db=False) as app:
             app.set_args(["rpc", "get", str(rpc.id)]).run()
             data, output = app.last_rendered
-            assert data["out"] == rpc.url
+            assert data == rpc.url
 
 
 def test_rpc_get_with_rpc_argument(chains: List[ChainFields]) -> None:
     """With RPC argument > it should return the argument"""
     test_rpcs = ["https://www.example-1.com", "https://www.example-2.com"]
     for rpc_url in test_rpcs:
         with Web3CliTest() as app:
             seed_chains(chains)
             app.set_args(["rpc", "get", "--rpc", rpc_url]).run()
             data, output = app.last_rendered
-            assert data["out"] == rpc_url
+            assert data == rpc_url
 
 
 def test_rpc_get_with_no_args(chains: List[ChainFields]) -> None:
     """Without arguments > should return an RPC of the user-provided chain"""
     for c in chains:
         with Web3CliTest() as app:
             seed_chains(chains)
             app.set_args(["rpc", "get", "--chain", c["name"]]).run()
             data, output = app.last_rendered
             chain: Chain = Chain.select().where(Chain.name == c["name"]).get()
-            assert data["out"] in [r.url for r in chain.get_rpcs()]
+            assert data in [r.url for r in chain.get_rpcs()]
 
 
 def test_rpc_delete(chains: List[ChainFields]) -> None:
     with Web3CliTest() as app:
         seed_chains(chains)
         rpcs = Rpc.get_all()
     n_rpcs = len(rpcs)
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,36 +43,36 @@
 # Test with --signer argument > returns address of signer
 def test_signer_active(signers: List[Dict[str, Any]]) -> None:
     for s in signers:
         with Web3CliTest() as app:
             seed_signers(signers, app.app_key)
             app.set_args(["signer", "active", "--signer", s["name"]]).run()
             data, output = app.last_rendered
-            assert data["out"] == s["address"]
+            assert data == s["address"]
 
 
 # Test without arguments > returns whatever is written in config file
 def test_signer_active_with_default_signer(signers: List[Dict[str, Any]]) -> None:
     s = signers[0]
     with Web3CliTest() as app:
         seed_signers(signers, app.app_key)
         app.config.set("web3cli", "default_signer", s["name"])
         app.set_args(["signer", "active"]).run()
         data, output = app.last_rendered
-        assert data["out"] == s["address"]
+        assert data == s["address"]
 
 
 # Test without arguments, without config file, but there's one signer in the DB > returns that one signer
 def test_signer_active_with_one_signer(signers: List[Dict[str, Any]]) -> None:
     s = signers[0]
     with Web3CliTest() as app:
         seed_signers([s], app.app_key)
         app.set_args(["signer", "active"]).run()
         data, output = app.last_rendered
-        assert data["out"] == s["address"]
+        assert data == s["address"]
 
 
 # Test without arguments, without config file, but there are multiple signers in the DB > raise error
 def test_signer_active_with_multiple_signers(signers: List[Dict[str, Any]]) -> None:
     with Web3CliTest() as app:
         seed_signers(signers, app.app_key)
         with pytest.raises(SignerNotResolved):
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/crud/test_token_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/crud/test_token_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,32 @@
 ) -> None:
     amount = 10**18
     bob_balance = TST.balanceOf(bob) / 10**18
     TST.transfer(bob, amount, sender=alice)
     seed_local_token(app, TST)
     app.set_args(["token", "balance", "tst", "bob"]).run()
     data, output = app.last_rendered
-    assert float(data["out"]) == bob_balance + amount / 10**18
+    assert type(data) is float
+    assert data == bob_balance + amount / 10**18
 
 
 def test_token_balance_wei(
     app: Web3CliTest,
     alice: ape.api.AccountAPI,
     bob: ape.api.AccountAPI,
     TST: ape.contracts.ContractInstance,
 ) -> None:
     amount = 10**18
     bob_balance = TST.balanceOf(bob)
     TST.transfer(bob, amount, sender=alice)
     seed_local_token(app, TST)
     app.set_args(["token", "balance", "tst", "bob", "--wei"]).run()
     data, output = app.last_rendered
-    assert int(data["out"]) == bob_balance + amount
+    assert type(data) is int
+    assert data == bob_balance + amount
 
 
 def test_token_approve(
     app: Web3CliTest,
     alice: ape.api.AccountAPI,
     bob: ape.api.AccountAPI,
     TST: ape.contracts.ContractInstance,
@@ -115,15 +117,16 @@
     bob: ape.api.AccountAPI,
     TST: ape.contracts.ContractInstance,
 ) -> None:
     TST.approve(bob, 2 * 10**18, sender=alice)
     seed_local_token(app, TST)
     app.set_args(["token", "allowance", "tst", "alice", "bob"]).run()
     data, output = app.last_rendered
-    assert float(data["out"]) == 2.0
+    assert type(data) is float
+    assert data == 2.0
 
 
 def test_token_list(contracts: List[ContractFields], chains: List[ChainFields]) -> None:
     """Add contracts and check that they are listed alphabetically
     by name and chain"""
     contracts = sorted(contracts, key=lambda c: c["name"])
     for chain in chains:
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_call_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,17 @@
             "bob",
             "1e18",
             "--from",
             "alice",
         ]
     ).run()
     data, output = app.last_rendered
-    assert output == "true"
+    print(data)
+    assert type(data) is bool
+    assert data == True
 
 
 @pytest.mark.remote
 # Test calling the Uniswap Router V2 contract's getAmountsOut function
 # (2 arguments of which one is an array)
 def test_call_eth_uniswap_v2_get_amounts_out(
     contracts: List[ContractFields], chains: List[ChainFields]
@@ -164,15 +166,15 @@
                 "totalSupply",
                 "--chain",
                 "eth",
             ]
         ).run()
         data, output = app.last_rendered
         assert type(data) is int
-        assert data > 1e18
+        assert data > 10**18
 
 
 @pytest.mark.remote
 # Test calling the WETH contract's totalSupply function
 # (two blocks ago)
 def test_call_eth_weth_total_supply_two_blocks_ago(
     contracts: List[ContractFields], chains: List[ChainFields]
@@ -202,15 +204,15 @@
                 str(latest - 2),
                 "--chain",
                 "eth",
             ]
         ).run()
         data, output = app.last_rendered
         assert type(data) is int
-        assert data > 1e18
+        assert data > 10**18
 
 
 @pytest.mark.remote
 # Test that calling a write function without a from address fails
 def test_call_eth_weth_transfer_without_from_address(
     contracts: List[ContractFields], chains: List[ChainFields]
 ) -> None:
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_db_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 
 def test_db_where(tmp: fs.Tmp) -> None:
     # Test with default path
     with Web3CliTest() as app:
         app.set_args(["db", "where"]).run()
         data, output = app.last_rendered
-        assert data["out"] == CONFIG["web3cli"]["db_file"]
+        assert data == CONFIG["web3cli"]["db_file"]
 
     # Test with custom path
     CONFIG["web3cli"]["db_file"] = f"{tmp.dir}/web3cli.sqlite"
     with Web3CliTest() as app:
         app.set_args(["db", "where"]).run()
         data, output = app.last_rendered
-        assert data["out"] == f"{tmp.dir}/web3cli.sqlite"
+        assert data == f"{tmp.dir}/web3cli.sqlite"
 
 
 def test_db_delete(tmp: fs.Tmp) -> None:
     # Test with default path
     with Web3CliTest() as app:
         app.set_args(["db", "delete", "--force"]).run()
         assert not os.path.isfile(app.db.database)
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from pathlib import Path
 from typing import Any, Dict, List
 
 import pytest
 
 from tests.web3cli.main import Web3CliTest
 from web3cli.helpers.crypto import decrypt_keyfile_dict
@@ -15,15 +14,15 @@
         with Web3CliTest() as app:
             # Create a keyfile JSON string from test signer private key
             responses = iter([s["private_key"], s["keyfile_password"]])
             monkeypatch.setattr("getpass.getpass", lambda _: next(responses))
             app.set_args(["keyfile", "create"]).run()
             data, output = app.last_rendered
             # Decrypt the keyfile to get again the private key
-            keyfile_dict = json.loads(data["out"])
+            keyfile_dict = data
             monkeypatch.setattr("getpass.getpass", lambda _: s["keyfile_password"])
             decoded_private_key = decrypt_keyfile_dict(keyfile_dict)
             # Test that the private key is the same
             assert decoded_private_key == s["private_key"]
 
 
 def test_keyfile_decode(
@@ -36,8 +35,8 @@
         keyfile = str(f)
         # Decode the keyfile
         with Web3CliTest() as app:
             responses = iter([s["keyfile_password"]])
             monkeypatch.setattr("getpass.getpass", lambda _: next(responses))
             app.set_args(["keyfile", "decrypt", keyfile]).run()
             data, output = app.last_rendered
-            assert data["out"] == s["private_key"]
+            assert data == s["private_key"]
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_misc_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import decimal
 import json
 from decimal import Decimal
 from typing import Any, Dict, List
 
 import pytest
 from web3 import Web3
 
@@ -81,15 +82,16 @@
 ) -> None:
     alice.transfer(bob, 10000)
     alice.transfer(bob, 20000)
     ape_chain.mine()
     alice.transfer(bob, 30000)
     app.set_args(["tx-count", "alice"]).run()
     data, output = app.last_rendered
-    assert int(data["out"]) == 3
+    assert type(data) is int
+    assert data == 3
 
 
 @pytest.mark.parametrize(
     "msg",
     [
         "Hello world!",
         "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam pulvinar lacus erat, et sollicitudin purus rutrum sed. Aliquam pulvinar nunc nec sagittis sagittis. Nunc efficitur lacus urna, sed dapibus lacus varius id. Nam laoreet convallis nisl, ut lacinia sem congue eu. Phasellus eu nisi in lectus lobortis viverra a at diam. Nulla dolor nisl, mollis efficitur venenatis in, elementum consequat quam. Sed a euismod justo, quis maximus velit. Maecenas varius augue dolor, sit amet elementum lacus pretium vitae. Fusce egestas condimentum quam eget elementum. Suspendisse vulputate ut urna a pretium. Nunc semper a sem fermentum dapibus.",
@@ -97,19 +99,19 @@
     ],
 )
 def test_sign(msg: str, signers: List[Dict[str, Any]]) -> None:
     with Web3CliTest() as app:
         seed_signers([signers[0]], app.app_key)
         app.set_args(["sign", msg]).run()
         data, output = app.last_rendered
-        assert "messageHash" in data["out"]
-        assert "r" in data["out"]
-        assert "s" in data["out"]
-        assert "v" in data["out"]
-        assert "signature" in data["out"]
+        assert "messageHash" in data
+        assert "r" in data
+        assert "s" in data
+        assert "v" in data
+        assert "signature" in data
 
 
 @pytest.mark.local
 def test_block_latest(
     app: Web3CliTest, alice: ape.api.AccountAPI, bob: ape.api.AccountAPI
 ) -> None:
     tx = alice.transfer(bob, 10000)
@@ -163,19 +165,19 @@
 
 @pytest.mark.local
 def test_gas_price(app: Web3CliTest, is_eip1559: bool) -> None:
     if is_eip1559:
         pytest.skip("Local chain does not have gas price")
     app.set_args(["gas-price"]).run()
     data, output = app.last_rendered
-    assert type(data) is Decimal
+    assert type(data) is float
     assert data > 0
 
 
 @pytest.mark.local
 def test_base_fee(app: Web3CliTest, is_eip1559: bool) -> None:
     if not is_eip1559:
         pytest.skip("Local chain does not have base fee")
     app.set_args(["base-fee"]).run()
     data, output = app.last_rendered
-    assert type(data) is Decimal
+    assert type(data) is decimal.Decimal
     assert data > 0
```

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_replay_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.1.2/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/fixtures.py` & `web3cli-1.1.2/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.1.2/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/main.py` & `web3cli-1.1.2/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3cli/test_db.py` & `web3cli-1.1.2/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/fixtures.py` & `web3cli-1.1.2/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.1.2/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.1.2/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.1.2/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.1.2/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/tests/web3core/models/test_contract_model.py` & `web3cli-1.1.2/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.1/PKG-INFO` & `web3cli-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 1.1.1
+Version: 1.1.2
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.1.1 Summary: Interact with
+Metadata-Version: 2.1 Name: web3cli Version: 1.1.2 Summary: Interact with
 blockchains and smart contracts using the command line License: MIT Keywords:
 web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
 coccoinomane
 gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
 github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
 coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
```

