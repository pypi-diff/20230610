# Comparing `tmp/web3cli-1.1.0.tar.gz` & `tmp/web3cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.1.0.tar", last modified: Thu Jun  8 18:16:53 2023, max compression
+gzip compressed data, was "web3cli-1.1.1.tar", last modified: Sat Jun 10 16:09:13 2023, max compression
```

## Comparing `web3cli-1.1.0.tar` & `web3cli-1.1.1.tar`

### file list

```diff
@@ -1,171 +1,172 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.0/LICENSE
--rw-r--r--   0        0        0    11240 2023-06-07 17:21:32.607065 web3cli-1.1.0/README.md
--rw-r--r--   0        0        0     4026 2023-06-08 18:16:41.983226 web3cli-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.0/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.0/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.0/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.1.0/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.1.0/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.1.0/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.1.0/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.1.0/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.0/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.0/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.1.0/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.1.0/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4795 2023-05-31 08:43:28.096742 web3cli-1.1.0/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.1.0/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.1.0/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.1.0/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.1.0/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.1.0/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     4330 2023-05-31 11:18:25.258680 web3cli-1.1.0/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     4461 2023-06-08 17:37:43.908413 web3cli-1.1.0/src/web3cli/controllers/replay_controller.py
--rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.1.0/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.0/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     7872 2023-06-08 18:14:50.319839 web3cli-1.1.0/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.0/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1408 2023-06-07 17:07:38.026919 web3cli-1.1.0/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.0/src/web3cli/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.0/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.1.0/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.0/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.0/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.0/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.0/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     1774 2023-06-08 18:15:33.914193 web3cli-1.1.0/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.0/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.0/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.0/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-06-08 18:16:07.880013 web3cli-1.1.0/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.0/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7358 2023-06-08 14:37:45.655105 web3cli-1.1.0/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.0/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.0/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.0/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.0/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.0/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.0/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.0/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.0/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.0/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.0/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.0/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.0/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.0/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.0/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.0/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.0/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.1.0/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.1.0/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.0/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.0/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.1.0/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.0/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.0/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.0/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.0/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.0/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.0/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.0/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.0/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.0/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.0/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.0/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.0/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.0/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.0/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.0/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.0/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.1.0/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.0/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.0/src/web3core/seeds/contracts/erat_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.0/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.0/src/web3core/seeds/contracts/gno_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.0/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.0/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.0/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.0/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.0/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.0/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.0/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.0/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.0/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.0/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.0/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.0/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.0/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.0/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.0/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.0/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.0/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.0/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-06-08 18:16:46.405077 web3cli-1.1.0/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.0/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.0/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.0/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.0/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.0/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.0/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.0/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.0/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.0/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.0/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.0/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.0/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.0/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.0/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.0/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.0/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.0/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.0/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.0/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.0/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.0/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.1.0/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.0/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.0/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.1.0/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.1.0/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     6446 2023-06-08 18:14:50.320112 web3cli-1.1.0/tests/web3cli/controllers/crud/test_token_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.0/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.1.0/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.1.0/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.1.0/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     6099 2023-05-31 11:22:03.092128 web3cli-1.1.0/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.0/tests/web3cli/controllers/test_replay_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.0/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.0/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.0/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.0/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.0/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.0/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.0/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.0/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.0/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.0/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.0/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.0/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.0/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.0/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.0/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.0/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.0/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    11697 1970-01-01 00:00:00.000000 web3cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.1/LICENSE
+-rw-r--r--   0        0        0    12030 2023-06-10 16:07:05.654200 web3cli-1.1.1/README.md
+-rw-r--r--   0        0        0     4026 2023-06-10 16:08:22.610889 web3cli-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.1/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.1/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.1/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.1.1/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.1.1/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.1.1/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.1.1/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.1.1/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.1/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.1/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.1.1/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.1.1/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4795 2023-05-31 08:43:28.096742 web3cli-1.1.1/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.1.1/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.1.1/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.1.1/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.1.1/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.1.1/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     4330 2023-05-31 11:18:25.258680 web3cli-1.1.1/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     4461 2023-06-08 17:37:43.908413 web3cli-1.1.1/src/web3cli/controllers/replay_controller.py
+-rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.1.1/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     3890 2023-06-10 16:05:25.285160 web3cli-1.1.1/src/web3cli/controllers/subscribe_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.1/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     7872 2023-06-08 18:14:50.319839 web3cli-1.1.1/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.1/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1408 2023-06-07 17:07:38.026919 web3cli-1.1.1/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.1/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.1/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    16208 2023-06-10 14:17:47.976710 web3cli-1.1.1/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.1/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.1/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.1/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.1/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     2163 2023-06-10 14:00:37.541209 web3cli-1.1.1/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.1/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.1/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.1/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-06-10 16:08:13.624292 web3cli-1.1.1/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.1/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7544 2023-06-10 15:35:59.359874 web3cli-1.1.1/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.1/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.1/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.1/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.1/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.1/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.1/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.1/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.1/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.1/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.1/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.1/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.1/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.1/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.1/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.1.1/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.1/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.1/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.1/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.1/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.1/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.1.1/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.1/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.1/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.1/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.1/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.1/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.1/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.1/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.1/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.1/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.1/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.1/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.1/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.1/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.1/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.1/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.1/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.1/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.1/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.1/src/web3core/seeds/contracts/erat_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.1/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.1/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.1/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.1.1/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.1/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.1/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.1/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.1/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.1/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.1/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.1/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.1/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.1/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.1/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.1/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.1/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.1/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.1/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.1/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.1/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-06-10 16:08:27.555321 web3cli-1.1.1/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.1/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.1/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.1/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.1/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.1/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.1/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.1/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.1/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.1/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.1/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.1/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.1/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.1/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.1/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.1/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.1/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.1/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.1/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.1/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.1/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.1/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.1.1/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.1/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.1/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.1.1/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.1.1/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     6446 2023-06-08 18:14:50.320112 web3cli-1.1.1/tests/web3cli/controllers/crud/test_token_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.1/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.1.1/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.1.1/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.1.1/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     6099 2023-05-31 11:22:03.092128 web3cli-1.1.1/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.1/tests/web3cli/controllers/test_replay_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.1/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.1/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.1/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.1/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.1/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.1/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.1/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.1/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.1/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.1/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.1/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.1/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.1/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.1/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.1/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.1/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.1/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 web3cli-1.1.1/PKG-INFO
```

### Comparing `web3cli-1.1.0/LICENSE` & `web3cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/README.md` & `web3cli-1.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,24 @@
 
 - Interact with Ethereum and EVM-compatible chains via your terminal
 - Bypass sluggish and potentially compromised frontends
 - No configuration needed
 - Label addresses, tokens and contracts for ease of use
 - Swap with Uniswap, TraderJoe, PancakeSwap, etc
 - Transfer tokens via their ticker
+- Stream pending transactions, new blocks and contract events
 - Replay transactions just with the tx hash
 - Concatenate commands to build powerful scripts
 - Import signers via private key or keyfile
 - Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s testing framework
 - [Windows compatible](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)
 
 Soon:
 
+- React to pending transactions, new blocks and contract events
 - Set up scheduled buys and sells (DCA)
 - Automatically buy when slippage is low enough
 - Get notified on Telegram when a pair is liquid enough, or unbalanced
 - Analyze on-chain data for tax or sleuthing purposes
 - Claim and reinvest yield from DeFi protocols
 
 
@@ -112,14 +114,30 @@
 
 - Swap tokens on a DEX:
    ```
    w3 swap uniswap_v2 1 usdc usdt     # swap 1 USDC for USDT on Uniswap
    w3avax swap traderjoe 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe
    ```
 
+- Stream blocks, transactions and contract events as they happen in realtime:
+   ```
+   w3 subscribe blocks   # stream blocks as they are mined
+   w3 subscribe pending  # stream pending transactions
+   w3 subscribe events   # stream all contract events
+   ```
+  Streaming requires a websocket connection: specify one with the `--rpc wss://...` flag.
+
+- Listen to events from specific contracts with specific topics:
+   ```bash
+   # Stream all events from USDC token
+   w3 subscribe events --contracts usdc 
+   # Stream only transfer events
+   w3 subscribe events --contracts usdc --topics 0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   ```
+
 - Replay a given transactions on the blockchain:
    ```
    tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
    w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
```

#### html2text {}

```diff
@@ -11,57 +11,67 @@
 book](#address-book) - [Wallet management](#wallet-management) + [Default
 signer](#default-signer) + [Create new private keys](#create-new-private-keys)
 - [Documentation](#documentation) - [Contributing](#contributing) -
 [Acknowledgements](#acknowledgements) # Features - Interact with Ethereum and
 EVM-compatible chains via your terminal - Bypass sluggish and potentially
 compromised frontends - No configuration needed - Label addresses, tokens and
 contracts for ease of use - Swap with Uniswap, TraderJoe, PancakeSwap, etc -
-Transfer tokens via their ticker - Replay transactions just with the tx hash -
-Concatenate commands to build powerful scripts - Import signers via private key
-or keyfile - Thoroughly tested using the [Ape Framework](https://github.com/
-ApeWorX/ape)'s testing framework - [Windows compatible](https://github.com/
-coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - Set up
-scheduled buys and sells (DCA) - Automatically buy when slippage is low enough
-- Get notified on Telegram when a pair is liquid enough, or unbalanced -
-Analyze on-chain data for tax or sleuthing purposes - Claim and reinvest yield
-from DeFi protocols # Install Make sure you have at least Python 3.7 installed,
-then run: ```bash pip3 install -U web3cli ``` Windows user? [Here's a tutorial
-for you](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-
-on-Windows)! # Simple examples - Get the ETH balance of any address: ``` w3
-balance 0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with
-easy-to-rember tags: ``` w3 address add unicef
+Transfer tokens via their ticker - Stream pending transactions, new blocks and
+contract events - Replay transactions just with the tx hash - Concatenate
+commands to build powerful scripts - Import signers via private key or keyfile
+- Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s
+testing framework - [Windows compatible](https://github.com/coccoinomane/
+web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - React to pending
+transactions, new blocks and contract events - Set up scheduled buys and sells
+(DCA) - Automatically buy when slippage is low enough - Get notified on
+Telegram when a pair is liquid enough, or unbalanced - Analyze on-chain data
+for tax or sleuthing purposes - Claim and reinvest yield from DeFi protocols #
+Install Make sure you have at least Python 3.7 installed, then run: ```bash
+pip3 install -U web3cli ``` Windows user? [Here's a tutorial for you](https://
+github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)! #
+Simple examples - Get the ETH balance of any address: ``` w3 balance
+0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with easy-to-
+rember tags: ``` w3 address add unicef
 0xa59b29d7dbc9794d1e7f45123c48b2b8d0a34636 ``` then use the tag in any command:
 ``` w3 balance unicef ``` - Fetch blocks from the blockchain, in easy-to-read
 JSON format: ```bash w3 block latest w3 block finalized w3 block 6094305 ``` -
 Fetch transactions & receipts from the blockchain: ```bash w3 tx get
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 w3 tx rc
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 ``` -
 Extract single fields from blocks or transactions, using `jq` (more details [in
 the Wiki](https://github.com/coccoinomane/web3cli/wiki/%E2%86%AA%EF%B8%8F-
 Output-processing)): ```bash w3 block latest | jq -r '.baseFeePerGas' ``` -
 Sign messages: ```bash w3 sign 'Hello world!' ``` # Advanced examples - Send
 coins or tokens to any address: ``` w3 send unicef 1 ETH # send 1 ETH, ask for
 confirmation w3 send unicef 1 ETH gwei # send 1 gwei, ask for confirmation w3
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
-1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Replay a given
-transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force` # send 1
-USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart Contract
-support `web3cli` comes preloaded with some popular smart contracts, including
-ERC20 tokens and Uniswap clones. See the available contracts with `w3 contract
-list`: ``` w3 contract list # contracts on Ethereum w3 contract list --chain
-bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on Ethereum
-``` You can also add custom contracts with `w3 contract add`: ``` w3 contract
-add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract
-add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To
-add or list new tokens, you can use the `w3 token` shorthand: ``` w3 token add
-weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete
-weth ``` See available functions and events on a contract with `w3 abi
-functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token
-w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
+1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Stream blocks,
+transactions and contract events as they happen in realtime: ``` w3 subscribe
+blocks # stream blocks as they are mined w3 subscribe pending # stream pending
+transactions w3 subscribe events # stream all contract events ``` Streaming
+requires a websocket connection: specify one with the `--rpc wss://...` flag. -
+Listen to events from specific contracts with specific topics: ```bash # Stream
+all events from USDC token w3 subscribe events --contracts usdc # Stream only
+transfer events w3 subscribe events --contracts usdc --topics
+0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef ``` - Replay
+a given transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force`
+# send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
+Contract support `web3cli` comes preloaded with some popular smart contracts,
+including ERC20 tokens and Uniswap clones. See the available contracts with `w3
+contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
+-chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
+Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
+contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
+contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
+``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
+token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
+token delete weth ``` See available functions and events on a contract with `w3
+abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
+token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
```

### Comparing `web3cli-1.1.0/pyproject.toml` & `web3cli-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3cli-1.1.0/src/web3cli/.DS_Store` & `web3cli-1.1.1/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/abi_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/abi_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/app_key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/base_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/call_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/config_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/controller.py` & `web3cli-1.1.1/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/crud/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/db_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/misc_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/replay_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/send_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/swap_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/token_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/transact_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/controllers/tx_controller.py` & `web3cli-1.1.1/src/web3cli/controllers/tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/args.py` & `web3cli-1.1.1/src/web3cli/helpers/args.py`

 * *Files 5% similar despite different names*

```diff
@@ -477,14 +477,25 @@
         {
             "help": "use this RPC url. If not specified, will use the default RPC for the chain ",
         }
         | kwargs,
     )
 
 
+def callback(*name_or_flags: str, **kwargs: Any) -> Tuple[List[str], dict[str, Any]]:
+    return (
+        list(name_or_flags) or ["--callback"],
+        {
+            "help": "function to call when stuff happens. For now, only 'print' is available",
+            "default": "print",
+        }
+        | kwargs,
+    )
+
+
 def signer_and_gas() -> List[Tuple[List[str], dict[str, Any]]]:
     """Shortcut for commands accepting both signer and gas arguments"""
     return [signer(), priority_fee()]
 
 
 def chain_and_rpc() -> List[Tuple[List[str], dict[str, Any]]]:
     """Shortcut for commands accepting both chain and rpc arguments"""
```

### Comparing `web3cli-1.1.0/src/web3cli/helpers/client_factory.py` & `web3cli-1.1.1/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/config.py` & `web3cli-1.1.1/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/crypto.py` & `web3cli-1.1.1/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/database.py` & `web3cli-1.1.1/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/render.py` & `web3cli-1.1.1/src/web3cli/helpers/render.py`

 * *Files 25% similar despite different names*

```diff
@@ -31,23 +31,24 @@
     except:
         return value
 
 
 def render_json(app: App, data: Any, indent: int = 4) -> None:
     """Print data as a JSON"""
     app.render(data, handler="json", indent=indent)
+    print()
 
 
 def render_yaml(app: App, data: Any) -> None:
     """Print data as a YAML"""
     app.render(data, handler="yaml")
 
 
 def render_web3py(app: App, data: Any, indent: int = 4) -> None:
-    """Print output from Web3.py as a Python dict"""
+    """Print AttributeDicts from Web3.py as a json"""
     render_json(app, json.loads(Web3.to_json(data)), indent=indent)
 
 
 def render_balance(
     app: App, balance: Union[int, float], ticker: str, unit: str = None
 ) -> None:
     """Print a balance"""
@@ -64,7 +65,19 @@
 
 def render_number(app: App, n: Union[int, float]) -> None:
     """Print a number"""
     if isinstance(n, int):
         app.print(f"{n}")
     else:
         app.print(f"{n:.18g}")
+
+
+def render(app: App, data: Any) -> None:
+    """Print the given variable using the best suited format"""
+    if isinstance(data, str):
+        app.print(data)
+    elif isinstance(data, int) or isinstance(data, float):
+        render_number(app, data)
+    elif type(data).__name__ == "AttributeDict":
+        render_web3py(app, data)
+    else:
+        render_json(app, data)
```

### Comparing `web3cli-1.1.0/src/web3cli/helpers/send.py` & `web3cli-1.1.1/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/signer.py` & `web3cli-1.1.1/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/helpers/tx.py` & `web3cli-1.1.1/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/hooks.py` & `web3cli-1.1.1/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3cli/main.py` & `web3cli-1.1.1/src/web3cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from web3cli.controllers.crud.rpc_controller import RpcController
 from web3cli.controllers.crud.signer_controller import SignerController
 from web3cli.controllers.db_controller import DbController
 from web3cli.controllers.keyfile_controller import KeyfileController
 from web3cli.controllers.misc_controller import MiscController
 from web3cli.controllers.replay_controller import ReplayController
 from web3cli.controllers.send_controller import SendController
+from web3cli.controllers.subscribe_controller import SubscribeController
 from web3cli.controllers.swap_controller import SwapController
 from web3cli.controllers.token_controller import TokenController
 from web3cli.controllers.transact_controller import TransactController
 from web3cli.controllers.tx_controller import TxController
 from web3cli.exceptions import Web3CliError
 from web3cli.helpers.args import override_arg
 from web3core.exceptions import Web3CoreError
@@ -108,14 +109,15 @@
             AbiController,
             CallController,
             TransactController,
             SwapController,
             TokenController,
             KeyfileController,
             ReplayController,
+            SubscribeController,
         ]
 
         # extend the app with cement hook system
         hooks = [
             ("post_setup", hooks.post_setup),
             ("post_argument_parsing", hooks.post_argument_parsing),
         ]
@@ -133,15 +135,20 @@
             app.exit_code = 1
 
             if app.debug is True:
                 import traceback
 
                 traceback.print_exc()
 
-        except (Web3CliError, Web3CoreError, configparser.NoOptionError) as e:
+        except (
+            Web3CliError,
+            Web3CoreError,
+            configparser.NoOptionError,
+            NotImplementedError,
+        ) as e:
             print("Web3CliError > %s" % e)
             app.exit_code = 1
 
             if app.debug is True:
                 import traceback
 
                 traceback.print_exc()
```

### Comparing `web3cli-1.1.0/src/web3core/exceptions.py` & `web3cli-1.1.1/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/abi.py` & `web3cli-1.1.1/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/blocks.py` & `web3cli-1.1.1/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/client_factory.py` & `web3cli-1.1.1/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/crypto.py` & `web3cli-1.1.1/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/database.py` & `web3cli-1.1.1/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/dex.py` & `web3cli-1.1.1/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/misc.py` & `web3cli-1.1.1/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/os.py` & `web3cli-1.1.1/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/resolve.py` & `web3cli-1.1.1/src/web3core/helpers/resolve.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     for model in models:
         try:
             if hasattr(model, "chain"):
                 if chain is not None:
                     return format(model.get(name=address_or_name, chain=chain).address)
                 raise ValueError(
-                    f"Chain must be specified for {model.__name__} model, but was not"
+                    f"Chain argument must be specified for {model.__name__} model, but was not"
                 )
             else:
                 return format(model.get(name=address_or_name).address)
         except model.DoesNotExist:
             pass
 
     raise AddressNotResolved(
```

### Comparing `web3cli-1.1.0/src/web3core/helpers/rpc.py` & `web3cli-1.1.1/src/web3core/helpers/rpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from urllib.parse import urlparse
 
+from web3core.exceptions import Web3CoreError
+
 HTTP_SCHEMES = {"http", "https"}
 WS_SCHEMES = {"ws", "wss"}
 
 
 def is_rpc_uri_valid(uri_string: str) -> bool:
     """Return True if the given string is a valid URI
     that can be used to access an RPC. Based on
@@ -13,7 +15,13 @@
         return True
     elif uri.scheme in HTTP_SCHEMES:
         return True
     elif uri.scheme in WS_SCHEMES:
         return True
     else:
         return False
+
+
+def check_ws_or_raise(rpc_url: str) -> None:
+    """Raise an error if the RPC URL is not a websocket or an IPC file"""
+    if not rpc_url.startswith("ws") and not rpc_url.endswith(".ipc"):
+        raise Web3CoreError("RPC must be a websocket URL or an IPC file")
```

### Comparing `web3cli-1.1.0/src/web3core/helpers/seed.py` & `web3cli-1.1.1/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/tx.py` & `web3cli-1.1.1/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/helpers/yaml.py` & `web3cli-1.1.1/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/address.py` & `web3cli-1.1.1/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/base_model.py` & `web3cli-1.1.1/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/chain.py` & `web3cli-1.1.1/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/contract.py` & `web3cli-1.1.1/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/signer.py` & `web3cli-1.1.1/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/timestamps_model.py` & `web3cli-1.1.1/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/tx.py` & `web3cli-1.1.1/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/models/types.py` & `web3cli-1.1.1/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/chain_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/chain_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/erat_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/erat_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/seeds/contracts/gno_contract_seeds.py` & `web3cli-1.1.1/src/web3core/seeds/contracts/gno_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/src/web3core/types.py` & `web3cli-1.1.1/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/.DS_Store` & `web3cli-1.1.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.DS_Store` & `web3cli-1.1.1/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.1.1/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.1.1/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_Math.json` & `web3cli-1.1.1/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.1.1/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.1.1/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IERC20.json` & `web3cli-1.1.1/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.1.1/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_IWETH.json` & `web3cli-1.1.1/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.1.1/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.1.1/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.1.1/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Token.json` & `web3cli-1.1.1/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.1.1/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.1.1/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.1.1/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.1.1/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.1.1/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/.build/__local__.json` & `web3cli-1.1.1/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/.DS_Store` & `web3cli-1.1.1/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/token/Token.sol` & `web3cli-1.1.1/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.1.1/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.1.1/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.1.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/fixtures.py` & `web3cli-1.1.1/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/helpers/token.py` & `web3cli-1.1.1/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.1.1/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_approve.py` & `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transfer.py` & `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/token/test_ape_token_transferFrom.py` & `web3cli-1.1.1/tests/ape/tests/token/test_ape_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py` & `web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py` & `web3cli-1.1.1/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/helper.py` & `web3cli-1.1.1/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/seed.py` & `web3cli-1.1.1/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/crud/test_token_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/crud/test_token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_replay_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.1.1/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/fixtures.py` & `web3cli-1.1.1/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.1.1/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/main.py` & `web3cli-1.1.1/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3cli/test_db.py` & `web3cli-1.1.1/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/fixtures.py` & `web3cli-1.1.1/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.1.1/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.1.1/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.1.1/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.1.1/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/tests/web3core/models/test_contract_model.py` & `web3cli-1.1.1/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.0/PKG-INFO` & `web3cli-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
@@ -45,22 +45,24 @@
 
 - Interact with Ethereum and EVM-compatible chains via your terminal
 - Bypass sluggish and potentially compromised frontends
 - No configuration needed
 - Label addresses, tokens and contracts for ease of use
 - Swap with Uniswap, TraderJoe, PancakeSwap, etc
 - Transfer tokens via their ticker
+- Stream pending transactions, new blocks and contract events
 - Replay transactions just with the tx hash
 - Concatenate commands to build powerful scripts
 - Import signers via private key or keyfile
 - Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s testing framework
 - [Windows compatible](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)
 
 Soon:
 
+- React to pending transactions, new blocks and contract events
 - Set up scheduled buys and sells (DCA)
 - Automatically buy when slippage is low enough
 - Get notified on Telegram when a pair is liquid enough, or unbalanced
 - Analyze on-chain data for tax or sleuthing purposes
 - Claim and reinvest yield from DeFi protocols
 
 
@@ -124,14 +126,30 @@
 
 - Swap tokens on a DEX:
    ```
    w3 swap uniswap_v2 1 usdc usdt     # swap 1 USDC for USDT on Uniswap
    w3avax swap traderjoe 1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe
    ```
 
+- Stream blocks, transactions and contract events as they happen in realtime:
+   ```
+   w3 subscribe blocks   # stream blocks as they are mined
+   w3 subscribe pending  # stream pending transactions
+   w3 subscribe events   # stream all contract events
+   ```
+  Streaming requires a websocket connection: specify one with the `--rpc wss://...` flag.
+
+- Listen to events from specific contracts with specific topics:
+   ```bash
+   # Stream all events from USDC token
+   w3 subscribe events --contracts usdc 
+   # Stream only transfer events
+   w3 subscribe events --contracts usdc --topics 0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef
+   ```
+
 - Replay a given transactions on the blockchain:
    ```
    tx=`w3 send unicef 1 USDC --force` # send 1 USDC to Unicef
    w3 replay $tx                      # re-send 1 USDC to Unicef
    ```
 
 # Smart Contract support
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.1.0 Summary: Interact with
+Metadata-Version: 2.1 Name: web3cli Version: 1.1.1 Summary: Interact with
 blockchains and smart contracts using the command line License: MIT Keywords:
 web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
 coccoinomane
 gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
 github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
 coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
@@ -18,57 +18,67 @@
 book](#address-book) - [Wallet management](#wallet-management) + [Default
 signer](#default-signer) + [Create new private keys](#create-new-private-keys)
 - [Documentation](#documentation) - [Contributing](#contributing) -
 [Acknowledgements](#acknowledgements) # Features - Interact with Ethereum and
 EVM-compatible chains via your terminal - Bypass sluggish and potentially
 compromised frontends - No configuration needed - Label addresses, tokens and
 contracts for ease of use - Swap with Uniswap, TraderJoe, PancakeSwap, etc -
-Transfer tokens via their ticker - Replay transactions just with the tx hash -
-Concatenate commands to build powerful scripts - Import signers via private key
-or keyfile - Thoroughly tested using the [Ape Framework](https://github.com/
-ApeWorX/ape)'s testing framework - [Windows compatible](https://github.com/
-coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - Set up
-scheduled buys and sells (DCA) - Automatically buy when slippage is low enough
-- Get notified on Telegram when a pair is liquid enough, or unbalanced -
-Analyze on-chain data for tax or sleuthing purposes - Claim and reinvest yield
-from DeFi protocols # Install Make sure you have at least Python 3.7 installed,
-then run: ```bash pip3 install -U web3cli ``` Windows user? [Here's a tutorial
-for you](https://github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-
-on-Windows)! # Simple examples - Get the ETH balance of any address: ``` w3
-balance 0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with
-easy-to-rember tags: ``` w3 address add unicef
+Transfer tokens via their ticker - Stream pending transactions, new blocks and
+contract events - Replay transactions just with the tx hash - Concatenate
+commands to build powerful scripts - Import signers via private key or keyfile
+- Thoroughly tested using the [Ape Framework](https://github.com/ApeWorX/ape)'s
+testing framework - [Windows compatible](https://github.com/coccoinomane/
+web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows) Soon: - React to pending
+transactions, new blocks and contract events - Set up scheduled buys and sells
+(DCA) - Automatically buy when slippage is low enough - Get notified on
+Telegram when a pair is liquid enough, or unbalanced - Analyze on-chain data
+for tax or sleuthing purposes - Claim and reinvest yield from DeFi protocols #
+Install Make sure you have at least Python 3.7 installed, then run: ```bash
+pip3 install -U web3cli ``` Windows user? [Here's a tutorial for you](https://
+github.com/coccoinomane/web3cli/wiki/%F0%9F%AA%9F-Run-web3cli-on-Windows)! #
+Simple examples - Get the ETH balance of any address: ``` w3 balance
+0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae ``` - Save addresses with easy-to-
+rember tags: ``` w3 address add unicef
 0xa59b29d7dbc9794d1e7f45123c48b2b8d0a34636 ``` then use the tag in any command:
 ``` w3 balance unicef ``` - Fetch blocks from the blockchain, in easy-to-read
 JSON format: ```bash w3 block latest w3 block finalized w3 block 6094305 ``` -
 Fetch transactions & receipts from the blockchain: ```bash w3 tx get
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 w3 tx rc
 0x3bbdcc2c7721521f7c767b7873ccb857f0816ac94e9f32c5601f4b15c87d1ef1 ``` -
 Extract single fields from blocks or transactions, using `jq` (more details [in
 the Wiki](https://github.com/coccoinomane/web3cli/wiki/%E2%86%AA%EF%B8%8F-
 Output-processing)): ```bash w3 block latest | jq -r '.baseFeePerGas' ``` -
 Sign messages: ```bash w3 sign 'Hello world!' ``` # Advanced examples - Send
 coins or tokens to any address: ``` w3 send unicef 1 ETH # send 1 ETH, ask for
 confirmation w3 send unicef 1 ETH gwei # send 1 gwei, ask for confirmation w3
 send unicef 1 usdc # send 1 USDC ``` - Swap tokens on a DEX: ``` w3 swap
 uniswap_v2 1 usdc usdt # swap 1 USDC for USDT on Uniswap w3avax swap traderjoe
-1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Replay a given
-transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force` # send 1
-USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart Contract
-support `web3cli` comes preloaded with some popular smart contracts, including
-ERC20 tokens and Uniswap clones. See the available contracts with `w3 contract
-list`: ``` w3 contract list # contracts on Ethereum w3 contract list --chain
-bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on Ethereum
-``` You can also add custom contracts with `w3 contract add`: ``` w3 contract
-add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3 contract
-add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2 ``` To
-add or list new tokens, you can use the `w3 token` shorthand: ``` w3 token add
-weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3 token delete
-weth ``` See available functions and events on a contract with `w3 abi
-functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH token
-w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
+1 usdc wavax # swap 1 USDC for WAVAX on TraderJoe ``` - Stream blocks,
+transactions and contract events as they happen in realtime: ``` w3 subscribe
+blocks # stream blocks as they are mined w3 subscribe pending # stream pending
+transactions w3 subscribe events # stream all contract events ``` Streaming
+requires a websocket connection: specify one with the `--rpc wss://...` flag. -
+Listen to events from specific contracts with specific topics: ```bash # Stream
+all events from USDC token w3 subscribe events --contracts usdc # Stream only
+transfer events w3 subscribe events --contracts usdc --topics
+0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef ``` - Replay
+a given transactions on the blockchain: ``` tx=`w3 send unicef 1 USDC --force`
+# send 1 USDC to Unicef w3 replay $tx # re-send 1 USDC to Unicef ``` # Smart
+Contract support `web3cli` comes preloaded with some popular smart contracts,
+including ERC20 tokens and Uniswap clones. See the available contracts with `w3
+contract list`: ``` w3 contract list # contracts on Ethereum w3 contract list -
+-chain bnb # contracts on BNB chain w3 contract list --type erc20 # tokens on
+Ethereum ``` You can also add custom contracts with `w3 contract add`: ``` w3
+contract add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 --type erc20 w3
+contract add sushi 0xd9e1cE17f2641f24aE83637ab66a2cca9C378B9F --type uniswap_v2
+``` To add or list new tokens, you can use the `w3 token` shorthand: ``` w3
+token add weth 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 w3 token list w3
+token delete weth ``` See available functions and events on a contract with `w3
+abi functions` and `w3 abi events`: ``` w3 abi fns weth # functions on WETH
+token w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
 uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
```

