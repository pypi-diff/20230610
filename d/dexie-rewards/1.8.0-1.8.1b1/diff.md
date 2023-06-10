# Comparing `tmp/dexie_rewards-1.8.0.tar.gz` & `tmp/dexie_rewards-1.8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-1.8.0.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.1b1.tar", max compression
```

## Comparing `dexie_rewards-1.8.0.tar` & `dexie_rewards-1.8.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-30 14:18:44.184005 dexie_rewards-1.8.0/LICENSE
--rw-r--r--   0        0        0     5648 2023-05-30 14:22:56.660449 dexie_rewards-1.8.0/README.md
--rw-r--r--   0        0        0      796 2023-05-30 14:22:07.469088 dexie_rewards-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-30 14:18:44.186020 dexie_rewards-1.8.0/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-30 14:18:44.186139 dexie_rewards-1.8.0/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-30 14:18:44.186320 dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1207 2023-05-30 14:18:44.186442 dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-30 14:18:44.186544 dexie_rewards-1.8.0/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     3505 2023-05-30 14:18:44.186731 dexie_rewards-1.8.0/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-30 14:18:44.186863 dexie_rewards-1.8.0/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-30 14:18:44.186965 dexie_rewards-1.8.0/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     4791 2023-05-30 14:18:44.187119 dexie_rewards-1.8.0/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-30 14:18:44.187307 dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-30 14:18:44.187448 dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1759 2023-05-30 14:18:44.187557 dexie_rewards-1.8.0/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      801 2023-05-30 14:18:44.187717 dexie_rewards-1.8.0/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-30 14:18:44.187821 dexie_rewards-1.8.0/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1851 2023-05-30 14:18:44.187935 dexie_rewards-1.8.0/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6431 1970-01-01 00:00:00.000000 dexie_rewards-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.1b1/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-26 14:42:14.551472 dexie_rewards-1.8.1b1/README.md
+-rw-r--r--   0        0        0      800 2023-06-10 08:57:34.470245 dexie_rewards-1.8.1b1/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.1b1/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-10 08:56:40.442539 dexie_rewards-1.8.1b1/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.1b1/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     4557 2023-06-10 08:56:40.443604 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     5122 2023-06-10 08:56:40.444110 dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1759 2023-05-26 14:42:14.553106 dexie_rewards-1.8.1b1/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-1.8.1b1/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.1b1/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.1b1/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6472 1970-01-01 00:00:00.000000 dexie_rewards-1.8.1b1/PKG-INFO
```

### Comparing `dexie_rewards-1.8.0/LICENSE` & `dexie_rewards-1.8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/README.md` & `dexie_rewards-1.8.1b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically to claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -30,15 +30,14 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
-
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -72,26 +71,24 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
-
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
-
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
@@ -118,8 +115,8 @@
 
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
-Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
+Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
```

### Comparing `dexie_rewards-1.8.0/pyproject.toml` & `dexie_rewards-1.8.1b1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "1.8.0"
+version = "1.8.1-b1"
 description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.10"
 rich-click = "^1.6.1"
 aiomisc = "^17.0.9"
 aiohttp = "^3.8.4"
 based58 = "^0.1.1"
 chia-blockchain = "1.8.*"
 aiosqlite = "^0.17.0"
```

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/config.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 wallet_rpc_port = chia_config["wallet"]["rpc_port"]
 selected_network = chia_config["selected_network"]
 address_prefix = chia_config["network_overrides"]["config"][selected_network][
     "address_prefix"
 ]
 
 
-dexie_mainnet = "https://dexie.space/"
+dexie_mainnet = "https://dexie.space"
 dexie_testnet = "https://testnet.dexie.space"
 dexie_local = "http://localhost:3000"
 
 dexie_url = os.environ.get(
     "DEXIE_URL", dexie_mainnet if selected_network == "mainnet" else dexie_testnet
 )
```

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     def _with_wallet_rpc_client(f):  # type: ignore
         async def with_rpc_client(*args, **kwargs):  # type: ignore
             try:
                 rpc_client = await WalletRpcClient.create(
                     self_hostname, rpc_port, chia_root, chia_config
                 )
                 return await run_rpc(rpc_client, f, *args, **kwargs)  # type: ignore
-            except Exception:
-                Console(stderr=True, style="bold red").print(
-                    "Unable to connect to wallet"
-                )
+            except Exception as e:
+                Console(stderr=True, style="bold red").print(f"wallet rpc error: {e}")
                 sys.exit(1)
 
         return with_rpc_client
 
     return _with_wallet_rpc_client
```

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/list.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,129 +1,69 @@
 from io import StringIO
 from rich.console import Console
-from rich.prompt import Confirm
-from typing import Any, List, Optional
+from typing import Optional
 import asyncio
 import json
 import rich_click as click
 import traceback
 
-from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
-
-from chia.types.blockchain_format.sized_bytes import bytes32
-from chia.util.bech32m import encode_puzzle_hash
-
-from ..services import dexie_db as dexie_db
-from ..utils import wait_for_synced_wallet
-from .utils import (
-    claim_rewards,
-    create_claims,
-    display_rewards,
-    get_offers_with_claimable_rewards,
-)
+from ..services.dexie_db import create_db
 from ..types.offer_reward import OfferReward
+from ..utils import wait_for_synced_wallet
+from .utils import display_rewards, get_offers_with_claimable_rewards
 
 console = Console()
 
 
-@click.command("claim", short_help="Claim all offers with dexie rewards")
+@click.command("list", short_help="List all offers with dexie rewards")
 @click.option(
     "-f",
     "--fingerprint",
     required=False,
     help="Set the fingerprint to specify which wallet to use",
     type=int,
 )
 @click.option(
-    "-vo",
-    "--verify-only",
-    "verify_only",
-    help="Only verify the claim, don't actually claim",
-    is_flag=True,
-    default=False,
-    show_default=True,
-)
-@click.option(
-    "-y",
-    "--yes",
-    "skip_confirm",
-    help="Skip claim confirmation",
+    "-j",
+    "--json",
+    "as_json",
+    help="Displays offers as JSON",
     is_flag=True,
     default=False,
     show_default=True,
 )
 @click.option(
     "-v",
     "--verbose",
     "verbose",
     help="Display verbose output",
     is_flag=True,
     default=False,
     show_default=True,
 )
-def claim_cmds(
-    fingerprint: Optional[int],
-    verify_only: bool,
-    skip_confirm: bool,
-    verbose: bool,
-) -> None:
-    asyncio.run(claim_cmds_async(fingerprint, verify_only, skip_confirm, verbose))
+def list_cmds(fingerprint: Optional[int], as_json: bool, verbose: bool) -> None:
+    asyncio.run(list_cmds_async(fingerprint, as_json, verbose))
 
 
-async def claim_cmds_async(
-    fingerprint: Optional[int],
-    verify_only: bool,
-    skip_confirm: bool,
-    verbose: bool,
+async def list_cmds_async(
+    fingerprint: Optional[int], as_json: bool, verbose: bool
 ) -> None:
     try:
-        console = Console(file=StringIO()) if not verbose else Console()
+        console = Console(file=StringIO()) if as_json or (not verbose) else Console()
 
-        synced_fingerprint = await wait_for_synced_wallet(fingerprint)
-        await dexie_db.create_db(synced_fingerprint)
+        synced_fingerprint = await wait_for_synced_wallet(fingerprint, console)
+        await create_db(synced_fingerprint)
 
         offers_rewards_dict = await get_offers_with_claimable_rewards(
             synced_fingerprint, console
         )
-        offers_rewards = list(map(OfferReward.from_json_dict, offers_rewards_dict))
-        if len(offers_rewards) == 0:
-            console.print("No rewards to claim", style="bold red")
-            return
-
-        display_rewards(offers_rewards)
-
-        if not skip_confirm:
-            if not Confirm.ask("Claim all?"):
-                return
-
-        claims = await create_claims(offers_rewards)
-        ret: Any = {
-            "claims": claims,
-        }
-        if verify_only:
-            ret["verify_only"] = True
-
-        if verbose:
-            console.print(
-                "\nclaims request payload:", style="bold dodger_blue2 underline"
-            )
-            console.print_json(json.dumps(ret, indent=4))
-
-        result = await claim_rewards(ret)
-
-        if verbose or verify_only:
-            console.print("\nclaims result:", style="bold dodger_blue2 underline")
-            if verbose:
-                console.print_json(json.dumps(result, indent=4))
-            else:
-                console.print("\nsuccess", style="bold green")
-
-        if result["success"] and not verify_only:
-            await dexie_db.update_offers_rewards(
-                synced_fingerprint, False, list(result["verified_amount"].keys())
-            )
+        if as_json:
+            click.echo(json.dumps(offers_rewards_dict))
+        else:
+            offers_rewards = list(map(OfferReward.from_json_dict, offers_rewards_dict))
+            display_rewards(offers_rewards)
 
     except Exception as e:
-        console.print("Error claiming rewards", style="bold red")
+        console.print("Error listing rewards", style="bold red")
         traceback_string = traceback.format_exc()
         console.print(traceback_string)
         console.print(e)
```

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/rewards/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 import time
 import traceback
 
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.trading.offer import Offer
 
 from ..config import dexie_api_url, dexie_blue, dexie_url
 from ..services import wallet_rpc_client as wallet_rpc_client
 from ..services.dexie_api import Api, get_dexie_bs58_offer_hash
 from ..services import dexie_db as dexie_db
 from ..types.offer_reward import OfferReward
 
 
-async def create_claims(offers_rewards: List[OfferReward]) -> List[Any]:
+async def create_claims(
+    offers_rewards: List[OfferReward], target_puzzle_hash: Optional[bytes32]
+) -> List[Any]:
     timestamp = int(time.time())
     claims = []
     for offer_reward in offers_rewards:
         (
             public_key,
             signature,
             signing_mode,
         ) = await sign_claim(
             offer_reward.offer_id,
             timestamp,
             offer_reward.maker_puzzle_hash,
+            target_puzzle_hash,
         )
 
         # return offer hash, signature, pk, and puzzle hash
         claim_info = {
             "offer_id": offer_reward.offer_id,
             "signature": signature,
             "public_key": public_key,
@@ -89,17 +92,25 @@
         traceback_string = traceback.format_exc()
         console.print(traceback_string)
         console.print(e)
         return []
 
 
 async def sign_claim(
-    offer_id: str, timestamp: int, maker_puzzle_hash: bytes32
+    offer_id: str,
+    timestamp: int,
+    maker_puzzle_hash: bytes32,
+    target_puzzle_hash: Optional[bytes32],
 ) -> Tuple[str, str, str]:
-    message = f"Claim dexie liquidity rewards for offer {offer_id} ({timestamp})"
+    message = (
+        # TODO: removed in 2.0.0
+        f"Claim dexie liquidity rewards for offer {offer_id} ({timestamp})"
+        if target_puzzle_hash is None
+        else f"Claim dexie liquidity rewards for offer {offer_id} to {target_puzzle_hash} ({timestamp})"
+    )
     return await wallet_rpc_client.sign_message_by_puzzle_hash(
         maker_puzzle_hash, message
     )
 
 
 async def claim_rewards(claims_payload: Any) -> Dict[str, Any]:
     result = await Api(dexie_api_url).claim_rewards(claims_payload)
```

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.0/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.1b1/src/dexie_rewards/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import asyncio
 from rich.console import Console
 from rich.progress import (
     Progress,
     SpinnerColumn,
     TextColumn,
     TimeElapsedColumn,
 )
-import time
 
 from typing import Optional
 
 from blspy import AugSchemeMPL, G1Element, G2Element, PrivateKey
 from chia.cmds.keys_funcs import private_key_for_fingerprint
 from chia.consensus.coinbase import create_puzzlehash_for_pk
 from chia.types.blockchain_format.sized_bytes import bytes32
@@ -56,10 +56,10 @@
         f"[bold bright_cyan]Syncing {fingerprint}", total=None
     )
 
     with syncing_wallet_progress:
         while True:
             if await is_wallet_synced(fingerprint):
                 break
-            time.sleep(2)
+            await asyncio.sleep(2)
 
     return fingerprint
```

### Comparing `dexie_rewards-1.8.0/PKG-INFO` & `dexie_rewards-1.8.1b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 1.8.0
+Version: 1.8.1b1
 Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiomisc (>=17.0.9,<18.0.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
 Requires-Dist: based58 (>=0.1.1,<0.2.0)
 Requires-Dist: chia-blockchain (>=1.8.0,<1.9.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically to claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -49,15 +50,14 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
-
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -91,26 +91,24 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
-
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
-
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
@@ -138,8 +136,7 @@
 ## Alternatives
 
 Advanced market makers may develop their own tools for claiming liquidity rewards. Refer to the [dexie API documentation](https://dexie.space/api) for information on how to claim rewards for offers using the API.
 
 ## Contributions
 
 Contributions are welcome and encouraged. Please fork the repository and submit a pull request to the `main` branch. If you have any questions, feel free to reach out to us on [Discord](https://discord.gg/3xUrkAxUmd).
-
```

