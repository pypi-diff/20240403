# Comparing `tmp/communex-0.1.6.tar.gz` & `tmp/communex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communex-0.1.6.tar", max compression
+gzip compressed data, was "communex-0.1.7.tar", max compression
```

## Comparing `communex-0.1.6.tar` & `communex-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.6/LICENSE
--rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.6/README.md
--rw-r--r--   0        0        0     1358 2024-03-25 17:03:49.287562 communex-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      313 2024-03-23 11:18:25.662457 communex-0.1.6/src/communex/__init__.py
--rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.6/src/communex/balance.py
--rw-r--r--   0        0        0       44 2024-03-23 11:18:25.662457 communex-0.1.6/src/communex/cli/__init__.py
--rw-r--r--   0        0        0       84 2024-03-23 11:18:25.662457 communex-0.1.6/src/communex/cli/__main__.py
--rw-r--r--   0        0        0     2855 2024-03-23 14:58:10.559875 communex-0.1.6/src/communex/cli/_common.py
--rw-r--r--   0        0        0     6787 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/cli/balance.py
--rw-r--r--   0        0        0     7494 2024-03-23 14:42:44.659770 communex-0.1.6/src/communex/cli/key.py
--rw-r--r--   0        0        0     2405 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/cli/misc.py
--rw-r--r--   0        0        0     5434 2024-03-25 14:07:05.057776 communex-0.1.6/src/communex/cli/module.py
--rw-r--r--   0        0        0     5533 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/cli/network.py
--rw-r--r--   0        0        0      807 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/cli/root.py
--rw-r--r--   0        0        0     3525 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/cli/subnet.py
--rw-r--r--   0        0        0    90970 2024-03-25 14:07:05.057776 communex-0.1.6/src/communex/client.py
--rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/compat/__init__.py
--rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/compat/_util.py
--rw-r--r--   0        0        0     4997 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/compat/key.py
--rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/compat/storage.py
--rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/compat/types.py
--rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/errors.py
--rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/key.py
--rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/misc.py
--rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/module/__init__.py
--rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.6/src/communex/module/_ip_limiter.py
--rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/module/_signer.py
--rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.6/src/communex/module/client.py
--rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.6/src/communex/module/example/__init__.py
--rw-r--r--   0        0        0     1468 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/module/example/gpt.py
--rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/module/example/openai.py
--rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/module/module.py
--rw-r--r--   0        0        0     7680 2024-03-25 14:07:08.731822 communex-0.1.6/src/communex/module/server.py
--rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/module/stuff.md
--rw-r--r--   0        0        0     2272 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/types.py
--rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.6/src/communex/util.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 communex-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      909 2024-03-23 11:18:25.661457 communex-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4575 2024-03-24 19:18:19.153594 communex-0.1.7/README.md
+-rw-r--r--   0        0        0     1385 2024-04-03 17:44:02.217963 communex-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      451 2024-03-30 15:42:14.063605 communex-0.1.7/src/communex/__init__.py
+-rw-r--r--   0        0        0     1237 2024-04-03 17:43:47.736268 communex-0.1.7/src/communex/_common.py
+-rw-r--r--   0        0        0      426 2024-03-23 11:18:25.662457 communex-0.1.7/src/communex/balance.py
+-rw-r--r--   0        0        0       41 2024-04-02 20:20:50.841713 communex-0.1.7/src/communex/cli/__init__.py
+-rw-r--r--   0        0        0       86 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/__main__.py
+-rw-r--r--   0        0        0     1985 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/_common.py
+-rw-r--r--   0        0        0     6735 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/balance.py
+-rw-r--r--   0        0        0     7590 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/key.py
+-rw-r--r--   0        0        0     2406 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/misc.py
+-rw-r--r--   0        0        0     6408 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/module.py
+-rw-r--r--   0        0        0     5536 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/network.py
+-rw-r--r--   0        0        0     1181 2024-04-02 20:25:06.421248 communex-0.1.7/src/communex/cli/root.py
+-rw-r--r--   0        0        0     3546 2024-03-30 16:23:28.998483 communex-0.1.7/src/communex/cli/subnet.py
+-rw-r--r--   0        0        0    91414 2024-03-30 15:44:47.719256 communex-0.1.7/src/communex/client.py
+-rw-r--r--   0        0        0      297 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/_util.py
+-rw-r--r--   0        0        0     5290 2024-03-25 19:42:20.678258 communex-0.1.7/src/communex/compat/key.py
+-rw-r--r--   0        0        0     2636 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/storage.py
+-rw-r--r--   0        0        0      386 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/compat/types.py
+-rw-r--r--   0        0        0      262 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/errors.py
+-rw-r--r--   0        0        0     1329 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/key.py
+-rw-r--r--   0        0        0    12756 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/misc.py
+-rw-r--r--   0        0        0      142 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/__init__.py
+-rw-r--r--   0        0        0     1533 2024-03-23 14:58:10.559875 communex-0.1.7/src/communex/module/_ip_limiter.py
+-rw-r--r--   0        0        0     2059 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/_signer.py
+-rw-r--r--   0        0        0     2712 2024-03-25 14:07:08.730822 communex-0.1.7/src/communex/module/client.py
+-rw-r--r--   0        0        0        0 2024-03-23 11:18:25.663457 communex-0.1.7/src/communex/module/example/__init__.py
+-rw-r--r--   0        0        0     1562 2024-03-30 16:16:22.622958 communex-0.1.7/src/communex/module/example/gpt.py
+-rw-r--r--   0        0        0      544 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/example/openai.py
+-rw-r--r--   0        0        0     2086 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/module.py
+-rw-r--r--   0        0        0     7676 2024-03-30 16:23:28.999483 communex-0.1.7/src/communex/module/server.py
+-rw-r--r--   0        0        0      381 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/module/stuff.md
+-rw-r--r--   0        0        0     2272 2024-03-30 16:12:44.684414 communex-0.1.7/src/communex/types.py
+-rw-r--r--   0        0        0     1333 2024-03-23 11:18:25.664457 communex-0.1.7/src/communex/util.py
+-rw-r--r--   0        0        0     5606 1970-01-01 00:00:00.000000 communex-0.1.7/PKG-INFO
```

### Comparing `communex-0.1.6/LICENSE` & `communex-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/README.md` & `communex-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/pyproject.toml` & `communex-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "communex"
-version = "0.1.6"
+version = "0.1.7"
 description = "A library for Commune network focused on simplicity"
 authors = ["agicommies <info@agicommies.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 comx = "communex.cli:app"
@@ -12,18 +12,17 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 
 # Substrate
 substrate-interface = "^1.7.4"
 scalecodec = "^1.2.7"
 py-sr25519-bindings = "^0.2.0"
-
 # Typing/Modeling/Validation
 pydantic = "^2.6.4"
-
+pydantic-settings = "^2.2.1"
 # CLI
 typer = "^0.9.0"
 rich = "^13.7.0"
 # HTTP
 aiohttp = "^3.9.3"
 fastapi = "^0.110.0"
 starlette = "^0.36.3"
```

### Comparing `communex-0.1.6/src/communex/cli/_common.py` & `communex-0.1.7/src/communex/cli/_common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,15 @@
 from dataclasses import dataclass
-from enum import Enum
 from typing import Any, Mapping
 
 import rich
 import typer
 from rich.console import Console
 from rich.table import Table
 
-from communex.client import CommuneClient
-from communex.balance import from_nano
-
-
-class BalanceUnit(str, Enum):
-    joule = "joule"
-    j = "j"
-    nano = "nano"
-    n = "n"
-
-
-class SortBalance(str, Enum):
-    all = "all"
-    free = "free"
-    staked = "staked"
-
 
 @dataclass
 class CustomCtx:
     typer_ctx: typer.Context
     console: rich.console.Console
     console_err: rich.console.Console
 
@@ -36,65 +19,42 @@
     def info(self, message: str) -> None:
         self.console_err.print(message)
 
     def error(self, message: str) -> None:
         message = f"ERROR: {message}"
         self.console_err.print(message, style="bold red")
 
+    def progress_status(self, message: str):
+        return self.console_err.status(message)
+
 
 def make_custom_context(ctx: typer.Context) -> CustomCtx:
     return CustomCtx(
         typer_ctx=ctx,
         console=Console(),
         console_err=Console(stderr=True),
     )
 
 
-# Client
-
-def get_node_url() -> str:
-    return "wss://commune-api-node-1.communeai.net"
-
-
-def make_client():
-    """
-    Create a client to the Commune network.
-    """
-
-    node_url = get_node_url()
-    return CommuneClient(url=node_url, num_connections=1, wait_for_finalization=False)
-
 # Formatting
 
 
 def eprint(e: Any) -> None:
     """
     Pretty prints an error.
     """
 
     console = Console()
 
     console.print(f"[bold red]ERROR: {e}", style="italic")
 
 
-def format_balance(balance: int, unit: BalanceUnit = BalanceUnit.nano) -> str:
-    """
-    Formats a balance.
-    """
-
-    match unit:
-        case BalanceUnit.nano | BalanceUnit.n:
-            return f"{balance}"
-        case BalanceUnit.joule | BalanceUnit.j:
-            in_joules = from_nano(balance)
-            round_joules = round(in_joules, 4)
-            return f"{round_joules:,} J"
-
-
-def print_table_from_plain_dict(result: Mapping[str, str | int | float], column_names: list[str], console: Console) -> None:
+def print_table_from_plain_dict(
+    result: Mapping[str, str | int | float], column_names: list[str], console: Console
+) -> None:
     """
     Creates a table for a plain dictionary.
     """
 
     table = Table(show_header=True, header_style="bold magenta")
 
     for name in column_names:
```

### Comparing `communex-0.1.6/src/communex/cli/balance.py` & `communex-0.1.7/src/communex/cli/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typer
 from rich.console import Console
 
 from communex.balance import to_nano
-from communex.compat.key import resolve_key_ss58, classic_load_key
+from communex.compat.key import classic_load_key, resolve_key_ss58
 from communex.errors import ChainTransactionError
 
-from ._common import BalanceUnit, format_balance, make_client, print_table_from_plain_dict
+from .._common import BalanceUnit, format_balance, make_client
+from ._common import print_table_from_plain_dict
 
 balance_app = typer.Typer()
 
 
 @balance_app.command()
 def show(key: str, unit: BalanceUnit = BalanceUnit.joule):
     """
@@ -125,29 +126,27 @@
     console = Console()
     client = make_client()
 
     nano_amount = to_nano(amount)
     resolved_key = classic_load_key(key)
     resolved_dest = resolve_key_ss58(dest)
 
-    # TODO: refactor yes/no prompts into function
-    console.print(
-        f"Please confirm that you want to transfer {amount} tokens to {dest} using key {key} (y/n)")
-
-    answer = input().lower()
-
-    if answer == "y":
-        with console.status(f"Transferring {amount} tokens to {dest}..."):
-            response = client.transfer(key=resolved_key,
-                                       amount=nano_amount, dest=resolved_dest)
-
-        if response.is_success:
-            console.print(f"Transferred {amount} tokens to {dest}")
-        else:
-            raise ChainTransactionError(response.error_message)  # type: ignore
+    transfer = typer.confirm(f"Are you sure you want to transfer {amount} tokens to {dest}?")
+    if not transfer:
+        print("Not transfering")
+        raise typer.Abort()
+
+    with console.status(f"Transferring {amount} tokens to {dest}..."):
+        response = client.transfer(key=resolved_key,
+                                    amount=nano_amount, dest=resolved_dest)
+
+    if response.is_success:
+        console.print(f"Transferred {amount} tokens to {dest}")
+    else:
+        raise ChainTransactionError(response.error_message)  # type: ignore
 
 
 @balance_app.command()
 def transfer_stake(key: str, amount: float, from_key: str, dest: str, netuid: int = 0):
     """
     Transfers stake of key from point A to point B
     """
```

### Comparing `communex-0.1.6/src/communex/cli/key.py` & `communex-0.1.7/src/communex/cli/key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import json
+from enum import Enum
 from typing import Any, cast
 
 import typer
 from rich.console import Console
 from substrateinterface import Keypair  # type: ignore
 from typer import Context
 
 from communex.compat.key import (classic_key_path, classic_store_key,
                                  local_key_addresses, resolve_key_ss58)
 from communex.compat.storage import classic_load
 from communex.key import generate_keypair
 from communex.misc import (local_keys_allbalance, local_keys_to_freebalance,
                            local_keys_to_stakedbalance)
 
-from ._common import (BalanceUnit, SortBalance, format_balance, make_client,
-                      make_custom_context, print_table_from_plain_dict,
+from .._common import BalanceUnit, format_balance, make_client
+from ._common import (make_custom_context, print_table_from_plain_dict,
                       print_table_standardize)
 
 key_app = typer.Typer()
 
 
+class SortBalance(str, Enum):
+    all = "all"
+    free = "free"
+    staked = "staked"
+
+
 @key_app.command()
 def create(ctx: Context, name: str):
     """
     Generates a new key and stores it on a disk with the given name.
     """
     context = make_custom_context(ctx)
```

### Comparing `communex-0.1.6/src/communex/cli/misc.py` & `communex-0.1.7/src/communex/cli/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typer
 from rich.console import Console
 
 from communex.balance import from_nano
 from communex.client import CommuneClient
 
-from ._common import BalanceUnit, format_balance, make_client
+from .._common import BalanceUnit, format_balance, make_client
 
 misc_app = typer.Typer()
 
 
 def circulating_tokens(c_client: CommuneClient) -> int:
     """
     Gets total circulating supply
```

### Comparing `communex-0.1.6/src/communex/cli/module.py` & `communex-0.1.7/src/communex/cli/module.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,90 @@
 import importlib.util
 from typing import Any, Optional, cast
 
 import typer
 import uvicorn
 from rich.console import Console
+from typer import Context
 
 import communex.balance as c_balance
 from communex.compat.key import classic_load_key
 from communex.errors import ChainTransactionError
 from communex.misc import get_map_modules
 from communex.module.server import ModuleServer
 from communex.util import is_ip_valid
 
-from ._common import make_client, make_custom_context, print_table_from_plain_dict
+from .._common import make_client
+from ._common import make_custom_context, print_table_from_plain_dict
 
 module_app = typer.Typer()
 
 
+# TODO: refactor CLI
+# - module address should be a single (arbitrary) parameter
+# - key can be infered from name or vice-versa?
 @module_app.command()
 def register(
+    ctx: Context,
     name: str,
     ip: str,
     port: int,
     key: str,
-    netuid: int,
+    netuid: Optional[int] = None,
     stake: Optional[float] = None,
+    new_subnet_name: Optional[str] = None,
 ):
     """
     Registers a module.
 
     Asks to generate a key if not provided.
     """
 
-    console = Console()
+    context = make_custom_context(ctx)
     client = make_client()
 
-    with console.status(f"Registering Module on a netuid '{netuid}' ..."):
-
-        if stake is None:
-            burn = client.get_burn()
-            stake = client.get_min_stake(netuid) + burn
-        stake_nano = c_balance.to_nano(stake)
+    match (netuid, new_subnet_name):
+        case (None, None):
+            raise ValueError("`netuid` or `new_subnet_name` must be provided")
+        case (netuid, None):
+            assert netuid is not None
+            subnet_name = client.get_subnet_name(netuid)
+        case (None, new_subnet_name):
+            subnet_name = new_subnet_name
+        case (_, _):
+            raise ValueError("`netuid` and `new_subnet_name` cannot be provided at the same time")
+
+    burn = client.get_burn()
+
+    do_burn = typer.confirm(f"{c_balance.from_nano(burn)} $COMAI will be permanently burned. Do you want to continue?")
+
+    if not do_burn:
+        print("Not registering")
+        raise typer.Abort()
+
+    with context.progress_status(f"Registering Module {name}..."):
+        if stake is not None:
+            stake_nano = c_balance.to_nano(stake)
+        else:
+            min_stake = client.get_min_stake(netuid) if netuid is not None else 0
+            stake_nano = min_stake + burn
 
         resolved_key = classic_load_key(key)
 
         if not is_ip_valid(ip):
             raise ValueError("Invalid ip address")
 
         address = f"{ip}:{port}"
-        subnet = client.get_name(netuid)
 
         response = client.register_module(
-            resolved_key, name=name, address=address, subnet=subnet, min_stake=stake_nano)
+            resolved_key, name=name, address=address, subnet=subnet_name, min_stake=stake_nano
+        )
 
         if response.is_success:
-            console.print(f"Module {name} registered")
+            context.info(f"Module {name} registered")
         else:
             raise ChainTransactionError(response.error_message)  # type: ignore
 
 
 @module_app.command()
 def update(key: str, name: str, ip: str, port: int, delegation_fee: int = 20, netuid: int = 0):
     """
@@ -123,16 +149,17 @@
     try:
         class_obj = getattr(module, class_name)
     except AttributeError:
         context.error(f"Class `{class_name}` not found in module `{module}`")
         raise typer.Exit(code=1)
 
     keypair = classic_load_key(key)
-    server = ModuleServer(class_obj(), keypair, whitelist=whitelist,
-                          blacklist=blacklist, subnets_whitelist=subnets_whitelist)
+    server = ModuleServer(
+        class_obj(), keypair, whitelist=whitelist, blacklist=blacklist, subnets_whitelist=subnets_whitelist
+    )
     app = server.get_fastapi_app()
     host = ip or "127.0.0.1"
     uvicorn.run(app, host=host, port=port)  # type: ignore
 
 
 @module_app.command()
 def info(name: str, balance: bool = False, netuid: int = 0):
```

### Comparing `communex-0.1.6/src/communex/cli/network.py` & `communex-0.1.7/src/communex/cli/network.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Any, cast
 
 import typer
 from rich.console import Console
+from typer import Context
 
 from communex.compat.key import classic_load_key, resolve_key_ss58
 from communex.misc import get_global_params
 from communex.types import NetworkParams, SubnetParams
 
-from ._common import make_client, print_table_from_plain_dict
+from .._common import make_client
+from ._common import make_custom_context, print_table_from_plain_dict
 
 network_app = typer.Typer()
 
 
 @network_app.command()
 def last_block(hash: bool = False):
     """
@@ -36,15 +38,17 @@
     """
     Gets global params
     """
 
     console = Console()
     client = make_client()
 
-    with console.status("Getting global network params ...",):
+    with console.status(
+        "Getting global network params ...",
+    ):
         global_params = get_global_params(client)
 
     general_params: dict[str, Any] = cast(dict[str, Any], global_params)
     print_table_from_plain_dict(general_params, ["Global params", "Value"], console)
 
 
 @network_app.command()
@@ -57,61 +61,76 @@
             proposals = client.query_map_proposals()
         except IndexError:
             console.print("No proposals found.")
             return
 
     for _, batch_proposal in proposals.items():
         for proposal_id, proposal in batch_proposal.items():
-            print_table_from_plain_dict(
-                proposal, [f"Proposal id: {proposal_id}", "Params"], console)
+            print_table_from_plain_dict(proposal, [f"Proposal id: {proposal_id}", "Params"], console)
 
 
 @network_app.command()
 def propose_globally(
+    ctx: Context,
     key: str,
     max_allowed_subnets: int,
     max_allowed_modules: int,
     max_registrations_per_block: int,
+    target_registrations_interval: int,
+    target_registrations_per_interval: int,
     unit_emission: int,
     tx_rate_limit: int,
     vote_threshold: int,
     vote_mode: str,
     max_proposals: int,
     max_name_length: int,
     burn_rate: int,
     min_burn: int,
+    max_burn: int,
+    burn: int,
     min_stake: int,
     min_weight_stake: int,
+    adjustment_alpha: int,
+    floor_delegation_fee: int,
 ):
     """
     Adds a global proposal to the network.
     """
 
-    console = Console()
     client = make_client()
+    context = make_custom_context(ctx)
 
     resolved_key = classic_load_key(key)
 
-    proposal: NetworkParams = {"max_allowed_subnets": max_allowed_subnets,
-                               "max_allowed_modules": max_allowed_modules,
-                               "max_registrations_per_block": max_registrations_per_block,
-                               "unit_emission": unit_emission,
-                               "tx_rate_limit": tx_rate_limit,
-                               "vote_threshold": vote_threshold,
-                               "vote_mode": vote_mode,
-                               "max_proposals": max_proposals,
-                               "max_name_length": max_name_length,
-                               "burn_rate": burn_rate,
-                               "min_burn": min_burn,
-                               "min_stake": min_stake,
-                               "min_weight_stake": min_weight_stake}
+    proposal: NetworkParams = {
+        "max_allowed_subnets": max_allowed_subnets,
+        "max_allowed_modules": max_allowed_modules,
+        "max_registrations_per_block": max_registrations_per_block,
+        "target_registrations_interval": target_registrations_interval,
+        "target_registrations_per_interval": target_registrations_per_interval,
+        "unit_emission": unit_emission,
+        "tx_rate_limit": tx_rate_limit,
+        "vote_threshold": vote_threshold,
+        "vote_mode": vote_mode,
+        "max_proposals": max_proposals,
+        "max_name_length": max_name_length,
+        "burn_rate": burn_rate,
+        "min_burn": min_burn,
+        "max_burn": max_burn,
+        "burn": burn,
+        "min_stake": min_stake,
+        "min_weight_stake": min_weight_stake,
+        "adjustment_alpha": adjustment_alpha,
+        "floor_delegation_fee": floor_delegation_fee,
+    }
 
-    with console.status("Adding a proposal..."):
+    with context.progress_status("Adding a proposal..."):
         client.add_global_proposal(resolved_key, proposal)
 
+
 # ! THESE ARE BETA COMMANDS (might not have full substrate support)
 
 
 @network_app.command()
 def propose_on_subnet(
     key: str,
     name: str,
@@ -136,30 +155,31 @@
 
     console = Console()
     client = make_client()
 
     resolve_founder = resolve_key_ss58(founder)
     resolved_key = classic_load_key(key)
 
-    proposal: SubnetParams = {"name": name,
-                              "founder": resolve_founder,
-                              "founder_share": founder_share,
-                              "immunity_period": immunity_period,
-                              "incentive_ratio": incentive_ratio,
-                              "max_allowed_uids": max_allowed_uids,
-                              "max_allowed_weights": max_allowed_weights,
-                              "min_allowed_weights": min_allowed_weights,
-                              "max_stake": max_stake,
-                              "min_stake": min_stake,
-                              "tempo": tempo,
-                              "trust_ratio": trust_ratio,
-                              "vote_mode": vote_mode,
-                              "vote_threshold": vote_threshold,
-                              "max_weight_age": max_weight_age,
-                              }
+    proposal: SubnetParams = {
+        "name": name,
+        "founder": resolve_founder,
+        "founder_share": founder_share,
+        "immunity_period": immunity_period,
+        "incentive_ratio": incentive_ratio,
+        "max_allowed_uids": max_allowed_uids,
+        "max_allowed_weights": max_allowed_weights,
+        "min_allowed_weights": min_allowed_weights,
+        "max_stake": max_stake,
+        "min_stake": min_stake,
+        "tempo": tempo,
+        "trust_ratio": trust_ratio,
+        "vote_mode": vote_mode,
+        "vote_threshold": vote_threshold,
+        "max_weight_age": max_weight_age,
+    }
 
     with console.status("Adding a proposal..."):
         client.add_subnet_proposal(resolved_key, proposal)
 
 
 @network_app.command()
 def vote_proposal(key: str, proposal_id: int):
@@ -179,8 +199,8 @@
     resolved_key = classic_load_key(key)
     with console.status(f"Unvoting on a proposal {proposal_id}..."):
         client.unvote_on_proposal(resolved_key, proposal_id)
 
 
 if __name__ == "__main__":
     client = make_client()
-    proposals = client.query_map_proposals()
+    proposals = client.query_map_proposals()
```

### Comparing `communex-0.1.6/src/communex/cli/subnet.py` & `communex-0.1.7/src/communex/cli/subnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 from communex.balance import from_nano
 from communex.compat.key import classic_load_key
 from communex.errors import ChainTransactionError
 from communex.misc import get_map_subnets_params
 from communex.types import Ss58Address, SubnetParams
 
-from ._common import make_client, print_table_from_plain_dict
+from .._common import make_client
+from ._common import print_table_from_plain_dict
 
 subnet_app = typer.Typer()
 
 
 @subnet_app.command()
 def list():
     """
```

### Comparing `communex-0.1.6/src/communex/client.py` & `communex-0.1.7/src/communex/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4699,988 +4699,1016 @@
 000125a0: 2049 6620 7468 6520 7175 6572 7920 746f   If the query to
 000125b0: 2074 6865 206e 6574 776f 726b 2066 6169   the network fai
 000125c0: 6c73 206f 7220 6973 2069 6e76 616c 6964  ls or is invalid
 000125d0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
 000125e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
 000125f0: 6c66 2e71 7565 7279 2822 4e61 6d65 222c  lf.query("Name",
 00012600: 2070 6172 616d 733d 5b6e 6574 7569 645d   params=[netuid]
-00012610: 290a 0a20 2020 2064 6566 2067 6574 5f6e  )..    def get_n
-00012620: 2873 656c 662c 206e 6574 7569 643a 2069  (self, netuid: i
-00012630: 6e74 203d 2030 2920 2d3e 2069 6e74 3a0a  nt = 0) -> int:.
-00012640: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012650: 2020 2020 5175 6572 6965 7320 7468 6520      Queries the 
-00012660: 6e65 7477 6f72 6b20 666f 7220 7468 6520  network for the 
-00012670: 274e 2720 6879 7065 7270 6172 616d 6574  'N' hyperparamet
-00012680: 6572 2c20 7768 6963 6820 7265 7072 6573  er, which repres
-00012690: 656e 7473 2068 6f77 0a20 2020 2020 2020  ents how.       
-000126a0: 206d 616e 7920 6d6f 6475 6c65 7320 6172   many modules ar
-000126b0: 6520 6f6e 2074 6865 206e 6574 776f 726b  e on the network
-000126c0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-000126d0: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
-000126e0: 7569 643a 2054 6865 206e 6574 776f 726b  uid: The network
-000126f0: 2055 4944 2066 6f72 2077 6869 6368 2074   UID for which t
-00012700: 6f20 7175 6572 7920 7468 6520 274e 2720  o query the 'N' 
-00012710: 6879 7065 7270 6172 616d 6574 6572 2e0a  hyperparameter..
-00012720: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00012730: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00012740: 6520 7661 6c75 6520 6f66 2074 6865 2027  e value of the '
-00012750: 4e27 2068 7970 6572 7061 7261 6d65 7465  N' hyperparamete
-00012760: 7220 666f 7220 7468 6520 7370 6563 6966  r for the specif
-00012770: 6965 6420 6e65 7477 6f72 6b0a 2020 2020  ied network.    
-00012780: 2020 2020 2020 2020 2020 7375 626e 6574            subnet
-00012790: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-000127a0: 733a 0a20 2020 2020 2020 2020 2020 2051  s:.            Q
-000127b0: 7565 7279 4572 726f 723a 2049 6620 7468  ueryError: If th
-000127c0: 6520 7175 6572 7920 746f 2074 6865 206e  e query to the n
-000127d0: 6574 776f 726b 2066 6169 6c73 206f 7220  etwork fails or 
-000127e0: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
-000127f0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00012800: 2072 6574 7572 6e20 7365 6c66 2e71 7565   return self.que
-00012810: 7279 2822 4e22 2c20 7061 7261 6d73 3d5b  ry("N", params=[
-00012820: 6e65 7475 6964 5d29 0a0a 2020 2020 6465  netuid])..    de
-00012830: 6620 6765 745f 7465 6d70 6f28 7365 6c66  f get_tempo(self
-00012840: 2c20 6e65 7475 6964 3a20 696e 7420 3d20  , netuid: int = 
-00012850: 3029 202d 3e20 696e 743a 0a20 2020 2020  0) -> int:.     
-00012860: 2020 2022 2222 0a20 2020 2020 2020 2051     """.        Q
-00012870: 7565 7269 6573 2074 6865 206e 6574 776f  ueries the netwo
-00012880: 726b 2066 6f72 2074 6865 2074 656d 706f  rk for the tempo
-00012890: 2073 6574 7469 6e67 2c20 6d65 6173 7572   setting, measur
-000128a0: 6564 2069 6e20 626c 6f63 6b73 2c20 666f  ed in blocks, fo
-000128b0: 7220 7468 650a 2020 2020 2020 2020 7370  r the.        sp
-000128c0: 6563 6966 6965 6420 7375 626e 6574 2e0a  ecified subnet..
-000128d0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000128e0: 2020 2020 2020 2020 2020 206e 6574 7569             netui
-000128f0: 643a 2054 6865 206e 6574 776f 726b 2055  d: The network U
-00012900: 4944 2066 6f72 2077 6869 6368 2074 6f20  ID for which to 
-00012910: 7175 6572 7920 7468 6520 7465 6d70 6f2e  query the tempo.
-00012920: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00012930: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00012940: 6865 2074 656d 706f 2073 6574 7469 6e67  he tempo setting
-00012950: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
-00012960: 6564 2073 7562 6e65 742e 0a0a 2020 2020  ed subnet...    
-00012970: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00012980: 2020 2020 2020 2020 5175 6572 7945 7272          QueryErr
-00012990: 6f72 3a20 4966 2074 6865 2071 7565 7279  or: If the query
-000129a0: 2074 6f20 7468 6520 6e65 7477 6f72 6b20   to the network 
-000129b0: 6661 696c 7320 6f72 2069 7320 696e 7661  fails or is inva
-000129c0: 6c69 642e 0a20 2020 2020 2020 2022 2222  lid..        """
-000129d0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000129e0: 2073 656c 662e 7175 6572 7928 2254 656d   self.query("Tem
-000129f0: 706f 222c 2070 6172 616d 733d 5b6e 6574  po", params=[net
-00012a00: 7569 645d 290a 0a20 2020 2064 6566 2067  uid])..    def g
-00012a10: 6574 5f74 6f74 616c 5f73 7461 6b65 2873  et_total_stake(s
-00012a20: 656c 662c 206e 6574 7569 643a 2069 6e74  elf, netuid: int
-00012a30: 203d 2030 293a 0a20 2020 2020 2020 2022   = 0):.        "
-00012a40: 2222 0a20 2020 2020 2020 2051 7565 7269  "".        Queri
-00012a50: 6573 2074 6865 206e 6574 776f 726b 2066  es the network f
-00012a60: 6f72 2074 6865 2074 6f74 616c 2073 7461  or the total sta
-00012a70: 6b65 2061 6d6f 756e 742e 0a0a 2020 2020  ke amount...    
-00012a80: 2020 2020 5265 7472 6965 7665 7320 7468      Retrieves th
-00012a90: 6520 746f 7461 6c20 616d 6f75 6e74 206f  e total amount o
-00012aa0: 6620 7374 616b 6520 7769 7468 696e 2061  f stake within a
-00012ab0: 2073 7065 6369 6669 6320 6e65 7477 6f72   specific networ
-00012ac0: 6b20 7375 626e 6574 2e0a 0a20 2020 2020  k subnet...     
-00012ad0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012ae0: 2020 2020 206e 6574 7569 643a 2054 6865       netuid: The
-00012af0: 206e 6574 776f 726b 2055 4944 2066 6f72   network UID for
-00012b00: 2077 6869 6368 2074 6f20 7175 6572 7920   which to query 
-00012b10: 7468 6520 746f 7461 6c20 7374 616b 652e  the total stake.
-00012b20: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00012b30: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00012b40: 6865 2074 6f74 616c 2073 7461 6b65 2061  he total stake a
-00012b50: 6d6f 756e 7420 666f 7220 7468 6520 7370  mount for the sp
-00012b60: 6563 6966 6965 6420 6e65 7477 6f72 6b20  ecified network 
-00012b70: 7375 626e 6574 2e0a 0a20 2020 2020 2020  subnet...       
-00012b80: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00012b90: 2020 2020 2051 7565 7279 4572 726f 723a       QueryError:
-00012ba0: 2049 6620 7468 6520 7175 6572 7920 746f   If the query to
-00012bb0: 2074 6865 206e 6574 776f 726b 2066 6169   the network fai
-00012bc0: 6c73 206f 7220 6973 2069 6e76 616c 6964  ls or is invalid
-00012bd0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00012be0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012bf0: 6c66 2e71 7565 7279 2822 546f 7461 6c53  lf.query("TotalS
-00012c00: 7461 6b65 222c 2070 6172 616d 733d 5b6e  take", params=[n
-00012c10: 6574 7569 645d 2c29 0a0a 2020 2020 6465  etuid],)..    de
-00012c20: 6620 6765 745f 7265 6769 7374 7261 7469  f get_registrati
-00012c30: 6f6e 735f 7065 725f 626c 6f63 6b28 7365  ons_per_block(se
-00012c40: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00012c50: 0a20 2020 2020 2020 2051 7565 7269 6573  .        Queries
-00012c60: 2074 6865 206e 6574 776f 726b 2066 6f72   the network for
-00012c70: 2074 6865 206e 756d 6265 7220 6f66 2072   the number of r
-00012c80: 6567 6973 7472 6174 696f 6e73 2070 6572  egistrations per
-00012c90: 2062 6c6f 636b 2e0a 0a20 2020 2020 2020   block...       
-00012ca0: 2046 6574 6368 6573 2074 6865 206e 756d   Fetches the num
-00012cb0: 6265 7220 6f66 2072 6567 6973 7472 6174  ber of registrat
-00012cc0: 696f 6e73 2074 6861 7420 6172 6520 7072  ions that are pr
-00012cd0: 6f63 6573 7365 6420 7065 7220 0a20 2020  ocessed per .   
-00012ce0: 2020 2020 2062 6c6f 636b 2077 6974 6869       block withi
-00012cf0: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a0a  n the network...
-00012d00: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00012d10: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00012d20: 206e 756d 6265 7220 6f66 2072 6567 6973   number of regis
-00012d30: 7472 6174 696f 6e73 2070 726f 6365 7373  trations process
-00012d40: 6564 2070 6572 2062 6c6f 636b 2e0a 0a20  ed per block... 
-00012d50: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00012d60: 2020 2020 2020 2020 2020 2051 7565 7279             Query
-00012d70: 4572 726f 723a 2049 6620 7468 6520 7175  Error: If the qu
-00012d80: 6572 7920 746f 2074 6865 206e 6574 776f  ery to the netwo
-00012d90: 726b 2066 6169 6c73 206f 7220 6973 2069  rk fails or is i
-00012da0: 6e76 616c 6964 2e0a 2020 2020 2020 2020  nvalid..        
-00012db0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-00012dc0: 7572 6e20 7365 6c66 2e71 7565 7279 2822  urn self.query("
-00012dd0: 5265 6769 7374 7261 7469 6f6e 7350 6572  RegistrationsPer
-00012de0: 426c 6f63 6b22 2c29 0a0a 2020 2020 6465  Block",)..    de
-00012df0: 6620 6d61 785f 7265 6769 7374 7261 7469  f max_registrati
-00012e00: 6f6e 735f 7065 725f 626c 6f63 6b28 7365  ons_per_block(se
-00012e10: 6c66 2c20 6e65 7475 6964 3a20 696e 7420  lf, netuid: int 
-00012e20: 3d20 3029 3a0a 2020 2020 2020 2020 2222  = 0):.        ""
-00012e30: 220a 2020 2020 2020 2020 5175 6572 6965  ".        Querie
-00012e40: 7320 7468 6520 6e65 7477 6f72 6b20 666f  s the network fo
-00012e50: 7220 7468 6520 6d61 7869 6d75 6d20 6e75  r the maximum nu
-00012e60: 6d62 6572 206f 6620 7265 6769 7374 7261  mber of registra
-00012e70: 7469 6f6e 7320 7065 7220 626c 6f63 6b2e  tions per block.
-00012e80: 0a0a 2020 2020 2020 2020 5265 7472 6965  ..        Retrie
-00012e90: 7665 7320 7468 6520 7570 7065 7220 6c69  ves the upper li
-00012ea0: 6d69 7420 6f66 2072 6567 6973 7472 6174  mit of registrat
-00012eb0: 696f 6e73 2074 6861 7420 6361 6e20 6265  ions that can be
-00012ec0: 2070 726f 6365 7373 6564 2069 6e20 0a20   processed in . 
-00012ed0: 2020 2020 2020 2065 6163 6820 626c 6f63         each bloc
-00012ee0: 6b20 7769 7468 696e 2061 2073 7065 6369  k within a speci
-00012ef0: 6669 6320 6e65 7477 6f72 6b20 7375 626e  fic network subn
-00012f00: 6574 2e0a 0a20 2020 2020 2020 2041 7267  et...        Arg
-00012f10: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
-00012f20: 6574 7569 643a 2054 6865 206e 6574 776f  etuid: The netwo
-00012f30: 726b 2055 4944 2066 6f72 2077 6869 6368  rk UID for which
-00012f40: 2074 6f20 7175 6572 792e 0a0a 2020 2020   to query...    
-00012f50: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00012f60: 2020 2020 2020 2020 2054 6865 206d 6178           The max
-00012f70: 696d 756d 206e 756d 6265 7220 6f66 2072  imum number of r
-00012f80: 6567 6973 7472 6174 696f 6e73 2070 6572  egistrations per
-00012f90: 2062 6c6f 636b 2066 6f72 200a 2020 2020   block for .    
-00012fa0: 2020 2020 2020 2020 7468 6520 7370 6563          the spec
-00012fb0: 6966 6965 6420 6e65 7477 6f72 6b20 7375  ified network su
-00012fc0: 626e 6574 2e0a 0a20 2020 2020 2020 2052  bnet...        R
-00012fd0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-00012fe0: 2020 2051 7565 7279 4572 726f 723a 2049     QueryError: I
-00012ff0: 6620 7468 6520 7175 6572 7920 746f 2074  f the query to t
-00013000: 6865 206e 6574 776f 726b 2066 6169 6c73  he network fails
-00013010: 206f 7220 6973 2069 6e76 616c 6964 2e0a   or is invalid..
-00013020: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00013030: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00013040: 2e71 7565 7279 2822 4d61 7852 6567 6973  .query("MaxRegis
-00013050: 7472 6174 696f 6e73 5065 7242 6c6f 636b  trationsPerBlock
-00013060: 222c 2070 6172 616d 733d 5b6e 6574 7569  ", params=[netui
-00013070: 645d 2c29 0a0a 2020 2020 6465 6620 6765  d],)..    def ge
-00013080: 745f 7072 6f70 6f73 616c 2873 656c 662c  t_proposal(self,
-00013090: 2070 726f 706f 7361 6c5f 6964 3a20 696e   proposal_id: in
-000130a0: 7420 3d20 3029 3a0a 2020 2020 2020 2020  t = 0):.        
-000130b0: 2222 220a 2020 2020 2020 2020 5175 6572  """.        Quer
-000130c0: 6965 7320 7468 6520 6e65 7477 6f72 6b20  ies the network 
-000130d0: 666f 7220 6120 7370 6563 6966 6963 2070  for a specific p
-000130e0: 726f 706f 7361 6c2e 0a0a 2020 2020 2020  roposal...      
-000130f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00013100: 2020 2020 7072 6f70 6f73 616c 5f69 643a      proposal_id:
-00013110: 2054 6865 2049 4420 6f66 2074 6865 2070   The ID of the p
-00013120: 726f 706f 7361 6c20 746f 2071 7565 7279  roposal to query
-00013130: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00013140: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00013150: 5468 6520 6465 7461 696c 7320 6f66 2074  The details of t
-00013160: 6865 2073 7065 6369 6669 6564 2070 726f  he specified pro
-00013170: 706f 7361 6c2e 0a0a 2020 2020 2020 2020  posal...        
-00013180: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00013190: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
-000131a0: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
-000131b0: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
-000131c0: 732c 2069 7320 696e 7661 6c69 642c 200a  s, is invalid, .
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 6f72 2069 6620 7468 6520 7072 6f70 6f73  or if the propos
-000131f0: 616c 2049 4420 646f 6573 206e 6f74 2065  al ID does not e
-00013200: 7869 7374 2e0a 2020 2020 2020 2020 2222  xist..        ""
-00013210: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00013220: 6e20 7365 6c66 2e71 7565 7279 2822 5072  n self.query("Pr
-00013230: 6f70 6f73 616c 7322 2c20 7061 7261 6d73  oposals", params
-00013240: 3d5b 7072 6f70 6f73 616c 5f69 645d 2c29  =[proposal_id],)
-00013250: 0a0a 2020 2020 6465 6620 6765 745f 7472  ..    def get_tr
-00013260: 7573 7428 7365 6c66 2c20 6e65 7475 6964  ust(self, netuid
-00013270: 3a20 696e 7420 3d20 3029 3a0a 2020 2020  : int = 0):.    
-00013280: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013290: 5175 6572 6965 7320 7468 6520 6e65 7477  Queries the netw
-000132a0: 6f72 6b20 666f 7220 7468 6520 7472 7573  ork for the trus
-000132b0: 7420 7365 7474 696e 6720 6f66 2061 2073  t setting of a s
-000132c0: 7065 6369 6669 6320 6e65 7477 6f72 6b20  pecific network 
-000132d0: 7375 626e 6574 2e0a 0a20 2020 2020 2020  subnet...       
-000132e0: 2052 6574 7269 6576 6573 2074 6865 2074   Retrieves the t
-000132f0: 7275 7374 206c 6576 656c 206f 7220 7363  rust level or sc
-00013300: 6f72 652c 2077 6869 6368 206d 6179 2072  ore, which may r
-00013310: 6570 7265 7365 6e74 2074 6865 200a 2020  epresent the .  
-00013320: 2020 2020 2020 6c65 7665 6c20 6f66 2074        level of t
-00013330: 7275 7374 776f 7274 6869 6e65 7373 206f  rustworthiness o
-00013340: 7220 7265 6c69 6162 696c 6974 7920 7769  r reliability wi
-00013350: 7468 696e 2061 200a 2020 2020 2020 2020  thin a .        
-00013360: 7061 7274 6963 756c 6172 206e 6574 776f  particular netwo
-00013370: 726b 2073 7562 6e65 742e 0a0a 2020 2020  rk subnet...    
-00013380: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00013390: 2020 2020 2020 6e65 7475 6964 3a20 5468        netuid: Th
-000133a0: 6520 6e65 7477 6f72 6b20 5549 4420 666f  e network UID fo
-000133b0: 7220 7768 6963 6820 746f 2071 7565 7279  r which to query
-000133c0: 2074 6865 2074 7275 7374 2073 6574 7469   the trust setti
-000133d0: 6e67 2e0a 0a20 2020 2020 2020 2052 6574  ng...        Ret
-000133e0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000133f0: 2020 5468 6520 7472 7573 7420 6c65 7665    The trust leve
-00013400: 6c20 6f72 2073 636f 7265 2066 6f72 2074  l or score for t
-00013410: 6865 2073 7065 6369 6669 6564 206e 6574  he specified net
-00013420: 776f 726b 2073 7562 6e65 742e 0a0a 2020  work subnet...  
-00013430: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-00013440: 2020 2020 2020 2020 2020 5175 6572 7945            QueryE
-00013450: 7272 6f72 3a20 4966 2074 6865 2071 7565  rror: If the que
-00013460: 7279 2074 6f20 7468 6520 6e65 7477 6f72  ry to the networ
-00013470: 6b20 6661 696c 7320 6f72 2069 7320 696e  k fails or is in
-00013480: 7661 6c69 642e 0a20 2020 2020 2020 2022  valid..        "
-00013490: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-000134a0: 726e 2073 656c 662e 7175 6572 7928 2254  rn self.query("T
-000134b0: 7275 7374 222c 2070 6172 616d 733d 5b6e  rust", params=[n
-000134c0: 6574 7569 645d 2c29 0a0a 2020 2020 6465  etuid],)..    de
-000134d0: 6620 6765 745f 7569 6473 2873 656c 662c  f get_uids(self,
-000134e0: 206b 6579 3a20 5373 3538 4164 6472 6573   key: Ss58Addres
-000134f0: 732c 206e 6574 7569 643a 2069 6e74 203d  s, netuid: int =
-00013500: 2030 2920 2d3e 2062 6f6f 6c20 7c20 4e6f   0) -> bool | No
-00013510: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
-00013520: 2020 2020 2020 2020 5175 6572 6965 7320          Queries 
-00013530: 7468 6520 6e65 7477 6f72 6b20 666f 7220  the network for 
-00013540: 6d6f 6475 6c65 2055 4944 7320 6173 736f  module UIDs asso
-00013550: 6369 6174 6564 2077 6974 6820 6120 7370  ciated with a sp
-00013560: 6563 6966 6963 206b 6579 2e0a 0a20 2020  ecific key...   
-00013570: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00013580: 2020 2020 2020 206b 6579 3a20 5468 6520         key: The 
-00013590: 6b65 7920 6164 6472 6573 7320 666f 7220  key address for 
-000135a0: 7768 6963 6820 746f 2071 7565 7279 2055  which to query U
-000135b0: 4944 732e 0a20 2020 2020 2020 2020 2020  IDs..           
-000135c0: 206e 6574 7569 643a 2054 6865 206e 6574   netuid: The net
-000135d0: 776f 726b 2055 4944 2077 6974 6869 6e20  work UID within 
-000135e0: 7768 6963 6820 746f 2073 6561 7263 6820  which to search 
-000135f0: 666f 7220 7468 6520 6b65 792e 0a0a 2020  for the key...  
-00013600: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00013610: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
-00013620: 7420 6f66 2055 4944 7320 6173 736f 6369  t of UIDs associ
-00013630: 6174 6564 2077 6974 6820 7468 6520 7370  ated with the sp
-00013640: 6563 6966 6965 6420 6b65 792e 0a0a 2020  ecified key...  
-00013650: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-00013660: 2020 2020 2020 2020 2020 5175 6572 7945            QueryE
-00013670: 7272 6f72 3a20 4966 2074 6865 2071 7565  rror: If the que
-00013680: 7279 2074 6f20 7468 6520 6e65 7477 6f72  ry to the networ
-00013690: 6b20 6661 696c 7320 6f72 2069 7320 696e  k fails or is in
-000136a0: 7661 6c69 642e 0a20 2020 2020 2020 2022  valid..        "
-000136b0: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-000136c0: 726e 2073 656c 662e 7175 6572 7928 2255  rn self.query("U
-000136d0: 6964 7322 2c20 7061 7261 6d73 3d5b 6e65  ids", params=[ne
-000136e0: 7475 6964 2c20 6b65 795d 2c29 0a0a 2020  tuid, key],)..  
-000136f0: 2020 6465 6620 6765 745f 756e 6974 5f65    def get_unit_e
-00013700: 6d69 7373 696f 6e28 7365 6c66 2920 2d3e  mission(self) ->
-00013710: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00013720: 220a 2020 2020 2020 2020 5175 6572 6965  ".        Querie
-00013730: 7320 7468 6520 6e65 7477 6f72 6b20 666f  s the network fo
-00013740: 7220 7468 6520 756e 6974 2065 6d69 7373  r the unit emiss
-00013750: 696f 6e20 7365 7474 696e 672e 0a0a 2020  ion setting...  
-00013760: 2020 2020 2020 5265 7472 6965 7665 7320        Retrieves 
-00013770: 7468 6520 756e 6974 2065 6d69 7373 696f  the unit emissio
-00013780: 6e20 7661 6c75 652c 2077 6869 6368 2072  n value, which r
-00013790: 6570 7265 7365 6e74 7320 7468 6520 0a20  epresents the . 
-000137a0: 2020 2020 2020 2065 6d69 7373 696f 6e20         emission 
-000137b0: 7261 7465 206f 7220 7175 616e 7469 7479  rate or quantity
-000137c0: 2066 6f72 2074 6865 2024 434f 4d41 4920   for the $COMAI 
-000137d0: 746f 6b65 6e2e 0a0a 2020 2020 2020 2020  token...        
-000137e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000137f0: 2020 2020 2054 6865 2075 6e69 7420 656d       The unit em
-00013800: 6973 7369 6f6e 2076 616c 7565 2069 6e20  ission value in 
-00013810: 6e61 6e6f 7320 666f 7220 7468 6520 6e65  nanos for the ne
-00013820: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
-00013830: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00013840: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
-00013850: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
-00013860: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
-00013870: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
-00013880: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00013890: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000138a0: 662e 7175 6572 7928 2255 6e69 7445 6d69  f.query("UnitEmi
-000138b0: 7373 696f 6e22 290a 0a20 2020 2064 6566  ssion")..    def
-000138c0: 2067 6574 5f74 785f 7261 7465 5f6c 696d   get_tx_rate_lim
-000138d0: 6974 2873 656c 6629 202d 3e20 696e 743a  it(self) -> int:
-000138e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000138f0: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
-00013900: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
-00013910: 2074 7261 6e73 6163 7469 6f6e 2072 6174   transaction rat
-00013920: 6520 6c69 6d69 742e 0a0a 2020 2020 2020  e limit...      
-00013930: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
-00013940: 7261 7465 206c 696d 6974 2066 6f72 2074  rate limit for t
-00013950: 7261 6e73 6163 7469 6f6e 7320 7769 7468  ransactions with
-00013960: 696e 2074 6865 206e 6574 776f 726b 2c20  in the network, 
-00013970: 0a20 2020 2020 2020 2077 6869 6368 2064  .        which d
-00013980: 6566 696e 6573 2074 6865 206d 6178 696d  efines the maxim
-00013990: 756d 206e 756d 6265 7220 6f66 2074 7261  um number of tra
-000139a0: 6e73 6163 7469 6f6e 7320 7468 6174 2063  nsactions that c
-000139b0: 616e 2062 6520 0a20 2020 2020 2020 2070  an be .        p
-000139c0: 726f 6365 7373 6564 2077 6974 6869 6e20  rocessed within 
-000139d0: 6120 6365 7274 6169 6e20 7469 6d65 6672  a certain timefr
-000139e0: 616d 652e 0a0a 2020 2020 2020 2020 5265  ame...        Re
-000139f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00013a00: 2020 2054 6865 2074 7261 6e73 6163 7469     The transacti
-00013a10: 6f6e 2072 6174 6520 6c69 6d69 7420 666f  on rate limit fo
-00013a20: 7220 7468 6520 6e65 7477 6f72 6b2e 0a0a  r the network...
-00013a30: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-00013a40: 2020 2020 2020 2020 2020 2020 5175 6572              Quer
-00013a50: 7945 7272 6f72 3a20 4966 2074 6865 2071  yError: If the q
-00013a60: 7565 7279 2074 6f20 7468 6520 6e65 7477  uery to the netw
-00013a70: 6f72 6b20 6661 696c 7320 6f72 2069 7320  ork fails or is 
-00013a80: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
-00013a90: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
-00013aa0: 7475 726e 2073 656c 662e 7175 6572 7928  turn self.query(
-00013ab0: 2254 7852 6174 654c 696d 6974 222c 290a  "TxRateLimit",).
-00013ac0: 0a20 2020 2064 6566 2067 6574 5f62 7572  .    def get_bur
-00013ad0: 6e5f 7261 7465 2873 656c 6629 202d 3e20  n_rate(self) -> 
-00013ae0: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00013af0: 0a20 2020 2020 2020 2051 7565 7269 6573  .        Queries
-00013b00: 2074 6865 206e 6574 776f 726b 2066 6f72   the network for
-00013b10: 2074 6865 2062 7572 6e20 7261 7465 2073   the burn rate s
-00013b20: 6574 7469 6e67 2e0a 0a20 2020 2020 2020  etting...       
-00013b30: 2052 6574 7269 6576 6573 2074 6865 2062   Retrieves the b
-00013b40: 7572 6e20 7261 7465 2c20 7768 6963 6820  urn rate, which 
-00013b50: 7265 7072 6573 656e 7473 2074 6865 2072  represents the r
-00013b60: 6174 6520 6174 200a 2020 2020 2020 2020  ate at .        
-00013b70: 7768 6963 6820 7468 6520 2443 4f4d 4149  which the $COMAI
-00013b80: 2074 6f6b 656e 2069 7320 7065 726d 616e   token is perman
-00013b90: 656e 746c 7920 0a20 2020 2020 2020 2072  ently .        r
-00013ba0: 656d 6f76 6564 206f 7220 2762 7572 6e65  emoved or 'burne
-00013bb0: 6427 2066 726f 6d20 6369 7263 756c 6174  d' from circulat
-00013bc0: 696f 6e2e 0a0a 2020 2020 2020 2020 5265  ion...        Re
-00013bd0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00013be0: 2020 2054 6865 2062 7572 6e20 7261 7465     The burn rate
-00013bf0: 2066 6f72 2074 6865 206e 6574 776f 726b   for the network
-00013c00: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00013c10: 733a 0a20 2020 2020 2020 2020 2020 2051  s:.            Q
-00013c20: 7565 7279 4572 726f 723a 2049 6620 7468  ueryError: If th
-00013c30: 6520 7175 6572 7920 746f 2074 6865 206e  e query to the n
-00013c40: 6574 776f 726b 2066 6169 6c73 206f 7220  etwork fails or 
-00013c50: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
-00013c60: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00013c70: 2072 6574 7572 6e20 7365 6c66 2e71 7565   return self.que
-00013c80: 7279 2822 4275 726e 5261 7465 222c 2070  ry("BurnRate", p
-00013c90: 6172 616d 733d 5b5d 2c29 0a0a 2020 2020  arams=[],)..    
-00013ca0: 6465 6620 6765 745f 6275 726e 2873 656c  def get_burn(sel
-00013cb0: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00013cc0: 2020 2022 2222 0a20 2020 2020 2020 2051     """.        Q
-00013cd0: 7565 7269 6573 2074 6865 206e 6574 776f  ueries the netwo
-00013ce0: 726b 2066 6f72 2074 6865 2062 7572 6e20  rk for the burn 
-00013cf0: 7365 7474 696e 672e 0a0a 2020 2020 2020  setting...      
-00013d00: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
-00013d10: 6275 726e 2076 616c 7565 2c20 7768 6963  burn value, whic
-00013d20: 6820 7265 7072 6573 656e 7473 2074 6865  h represents the
-00013d30: 2061 6d6f 756e 7420 6f66 200a 2020 2020   amount of .    
-00013d40: 2020 2020 7468 6520 2443 4f4d 4149 2074      the $COMAI t
-00013d50: 6f6b 656e 7320 7468 6174 2061 7265 2027  okens that are '
-00013d60: 6275 726e 6564 2720 6f72 2070 6572 6d61  burned' or perma
-00013d70: 6e65 6e74 6c79 200a 2020 2020 2020 2020  nently .        
-00013d80: 7265 6d6f 7665 6420 6672 6f6d 2063 6972  removed from cir
-00013d90: 6375 6c61 7469 6f6e 2e0a 0a20 2020 2020  culation...     
-00013da0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00013db0: 2020 2020 2020 2020 5468 6520 6275 726e          The burn
-00013dc0: 2076 616c 7565 2066 6f72 2074 6865 206e   value for the n
-00013dd0: 6574 776f 726b 2e0a 0a20 2020 2020 2020  etwork...       
-00013de0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00013df0: 2020 2020 2051 7565 7279 4572 726f 723a       QueryError:
-00013e00: 2049 6620 7468 6520 7175 6572 7920 746f   If the query to
-00013e10: 2074 6865 206e 6574 776f 726b 2066 6169   the network fai
-00013e20: 6c73 206f 7220 6973 2069 6e76 616c 6964  ls or is invalid
-00013e30: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00013e40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00013e50: 6c66 2e71 7565 7279 2822 4275 726e 222c  lf.query("Burn",
-00013e60: 2070 6172 616d 733d 5b5d 2c29 0a0a 2020   params=[],)..  
-00013e70: 2020 6465 6620 6765 745f 6d69 6e5f 6275    def get_min_bu
-00013e80: 726e 2873 656c 6629 202d 3e20 696e 743a  rn(self) -> int:
-00013e90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013ea0: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
-00013eb0: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
-00013ec0: 206d 696e 696d 756d 2062 7572 6e20 7365   minimum burn se
-00013ed0: 7474 696e 672e 0a0a 2020 2020 2020 2020  tting...        
-00013ee0: 5265 7472 6965 7665 7320 7468 6520 6d69  Retrieves the mi
-00013ef0: 6e69 6d75 6d20 6275 726e 2076 616c 7565  nimum burn value
-00013f00: 2c20 696e 6469 6361 7469 6e67 2074 6865  , indicating the
-00013f10: 206c 6f77 6573 7420 0a20 2020 2020 2020   lowest .       
-00013f20: 2061 6d6f 756e 7420 6f66 2074 6865 2024   amount of the $
-00013f30: 434f 4d41 4920 746f 6b65 6e73 2074 6861  COMAI tokens tha
-00013f40: 7420 6361 6e20 6265 2027 6275 726e 6564  t can be 'burned
-00013f50: 2720 6f72 200a 2020 2020 2020 2020 7065  ' or .        pe
-00013f60: 726d 616e 656e 746c 7920 7265 6d6f 7665  rmanently remove
-00013f70: 6420 6672 6f6d 2063 6972 6375 6c61 7469  d from circulati
-00013f80: 6f6e 2e0a 0a20 2020 2020 2020 2052 6574  on...        Ret
-00013f90: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00013fa0: 2020 5468 6520 6d69 6e69 6d75 6d20 6275    The minimum bu
-00013fb0: 726e 2076 616c 7565 2066 6f72 2074 6865  rn value for the
-00013fc0: 206e 6574 776f 726b 2e0a 0a20 2020 2020   network...     
-00013fd0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-00013fe0: 2020 2020 2020 2051 7565 7279 4572 726f         QueryErro
-00013ff0: 723a 2049 6620 7468 6520 7175 6572 7920  r: If the query 
-00014000: 746f 2074 6865 206e 6574 776f 726b 2066  to the network f
-00014010: 6169 6c73 206f 7220 6973 2069 6e76 616c  ails or is inval
-00014020: 6964 2e0a 2020 2020 2020 2020 2222 220a  id..        """.
-00014030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014040: 7365 6c66 2e71 7565 7279 2822 4d69 6e42  self.query("MinB
-00014050: 7572 6e22 2c20 7061 7261 6d73 3d5b 5d2c  urn", params=[],
-00014060: 290a 0a20 2020 2064 6566 2067 6574 5f6d  )..    def get_m
-00014070: 696e 5f77 6569 6768 745f 7374 616b 6528  in_weight_stake(
-00014080: 7365 6c66 2920 2d3e 2069 6e74 3a0a 2020  self) -> int:.  
-00014090: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000140a0: 2020 5175 6572 6965 7320 7468 6520 6e65    Queries the ne
-000140b0: 7477 6f72 6b20 666f 7220 7468 6520 6d69  twork for the mi
-000140c0: 6e69 6d75 6d20 7765 6967 6874 2073 7461  nimum weight sta
-000140d0: 6b65 2073 6574 7469 6e67 2e0a 0a20 2020  ke setting...   
-000140e0: 2020 2020 2052 6574 7269 6576 6573 2074       Retrieves t
-000140f0: 6865 206d 696e 696d 756d 2077 6569 6768  he minimum weigh
-00014100: 7420 7374 616b 652c 2077 6869 6368 2072  t stake, which r
-00014110: 6570 7265 7365 6e74 7320 7468 6520 6c6f  epresents the lo
-00014120: 7765 7374 200a 2020 2020 2020 2020 7374  west .        st
-00014130: 616b 6520 7765 6967 6874 2074 6861 7420  ake weight that 
-00014140: 6973 2061 6c6c 6f77 6564 2066 6f72 2063  is allowed for c
-00014150: 6572 7461 696e 206f 7065 7261 7469 6f6e  ertain operation
-00014160: 7320 6f72 200a 2020 2020 2020 2020 7472  s or .        tr
-00014170: 616e 7361 6374 696f 6e73 2077 6974 6869  ansactions withi
-00014180: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a0a  n the network...
-00014190: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000141a0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000141b0: 206d 696e 696d 756d 2077 6569 6768 7420   minimum weight 
-000141c0: 7374 616b 6520 666f 7220 7468 6520 6e65  stake for the ne
-000141d0: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
-000141e0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-000141f0: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
-00014200: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
-00014210: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
-00014220: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
-00014230: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00014240: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00014250: 662e 7175 6572 7928 224d 696e 5765 6967  f.query("MinWeig
-00014260: 6874 5374 616b 6522 2c20 7061 7261 6d73  htStake", params
-00014270: 3d5b 5d29 0a0a 2020 2020 6465 6620 6765  =[])..    def ge
-00014280: 745f 766f 7465 5f6d 6f64 655f 676c 6f62  t_vote_mode_glob
-00014290: 616c 2873 656c 6629 202d 3e20 7374 723a  al(self) -> str:
-000142a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000142b0: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
-000142c0: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
-000142d0: 2067 6c6f 6261 6c20 766f 7465 206d 6f64   global vote mod
-000142e0: 6520 7365 7474 696e 672e 0a0a 2020 2020  e setting...    
-000142f0: 2020 2020 5265 7472 6965 7665 7320 7468      Retrieves th
-00014300: 6520 676c 6f62 616c 2076 6f74 6520 6d6f  e global vote mo
-00014310: 6465 2c20 7768 6963 6820 6465 6669 6e65  de, which define
-00014320: 7320 7468 6520 6f76 6572 616c 6c20 766f  s the overall vo
-00014330: 7469 6e67 200a 2020 2020 2020 2020 6d65  ting .        me
-00014340: 7468 6f64 6f6c 6f67 7920 6f72 2061 7070  thodology or app
-00014350: 726f 6163 6820 7573 6564 2061 6372 6f73  roach used acros
-00014360: 7320 7468 6520 6e65 7477 6f72 6b20 696e  s the network in
-00014370: 2064 6566 6175 6c74 2e0a 0a20 2020 2020   default...     
-00014380: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00014390: 2020 2020 2020 2020 5468 6520 676c 6f62          The glob
-000143a0: 616c 2076 6f74 6520 6d6f 6465 2073 6574  al vote mode set
-000143b0: 7469 6e67 2066 6f72 2074 6865 206e 6574  ting for the net
-000143c0: 776f 726b 2e0a 0a20 2020 2020 2020 2052  work...        R
-000143d0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-000143e0: 2020 2051 7565 7279 4572 726f 723a 2049     QueryError: I
-000143f0: 6620 7468 6520 7175 6572 7920 746f 2074  f the query to t
-00014400: 6865 206e 6574 776f 726b 2066 6169 6c73  he network fails
-00014410: 206f 7220 6973 2069 6e76 616c 6964 2e0a   or is invalid..
-00014420: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00014430: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00014440: 2e71 7565 7279 2822 566f 7465 4d6f 6465  .query("VoteMode
-00014450: 476c 6f62 616c 222c 290a 0a20 2020 2064  Global",)..    d
-00014460: 6566 2067 6574 5f6d 6178 5f70 726f 706f  ef get_max_propo
-00014470: 7361 6c73 2873 656c 6629 202d 3e20 696e  sals(self) -> in
-00014480: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-00014490: 2020 2020 2020 2051 7565 7269 6573 2074         Queries t
-000144a0: 6865 206e 6574 776f 726b 2066 6f72 2074  he network for t
-000144b0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-000144c0: 7220 6f66 2070 726f 706f 7361 6c73 2061  r of proposals a
-000144d0: 6c6c 6f77 6564 2e0a 0a20 2020 2020 2020  llowed...       
-000144e0: 2052 6574 7269 6576 6573 2074 6865 2075   Retrieves the u
-000144f0: 7070 6572 206c 696d 6974 206f 6e20 7468  pper limit on th
-00014500: 6520 6e75 6d62 6572 206f 6620 7072 6f70  e number of prop
-00014510: 6f73 616c 7320 7468 6174 2063 616e 2062  osals that can b
-00014520: 6520 0a20 2020 2020 2020 2061 6374 6976  e .        activ
-00014530: 6520 6f72 2063 6f6e 7369 6465 7265 6420  e or considered 
-00014540: 6174 2061 6e79 2067 6976 656e 2074 696d  at any given tim
-00014550: 6520 7769 7468 696e 2074 6865 206e 6574  e within the net
-00014560: 776f 726b 2e0a 0a20 2020 2020 2020 2052  work...        R
-00014570: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00014580: 2020 2020 5468 6520 6d61 7869 6d75 6d20      The maximum 
-00014590: 6e75 6d62 6572 206f 6620 7072 6f70 6f73  number of propos
-000145a0: 616c 7320 616c 6c6f 7765 6420 6f6e 2074  als allowed on t
-000145b0: 6865 206e 6574 776f 726b 2e0a 0a20 2020  he network...   
-000145c0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-000145d0: 2020 2020 2020 2020 2051 7565 7279 4572           QueryEr
-000145e0: 726f 723a 2049 6620 7468 6520 7175 6572  ror: If the quer
-000145f0: 7920 746f 2074 6865 206e 6574 776f 726b  y to the network
-00014600: 2066 6169 6c73 206f 7220 6973 2069 6e76   fails or is inv
-00014610: 616c 6964 2e0a 2020 2020 2020 2020 2222  alid..        ""
-00014620: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00014630: 6e20 7365 6c66 2e71 7565 7279 2822 4d61  n self.query("Ma
-00014640: 7850 726f 706f 7361 6c73 222c 290a 0a20  xProposals",).. 
-00014650: 2020 2064 6566 2067 6574 5f6d 6178 5f72     def get_max_r
-00014660: 6567 6973 7472 6174 696f 6e73 5f70 6572  egistrations_per
-00014670: 5f62 6c6f 636b 2873 656c 6629 202d 3e20  _block(self) -> 
-00014680: 696e 743a 0a20 2020 2020 2020 2022 2222  int:.        """
-00014690: 0a20 2020 2020 2020 2051 7565 7269 6573  .        Queries
-000146a0: 2074 6865 206e 6574 776f 726b 2066 6f72   the network for
-000146b0: 2074 6865 206d 6178 696d 756d 206e 756d   the maximum num
-000146c0: 6265 7220 6f66 2072 6567 6973 7472 6174  ber of registrat
-000146d0: 696f 6e73 2070 6572 2062 6c6f 636b 2e0a  ions per block..
-000146e0: 0a20 2020 2020 2020 2052 6574 7269 6576  .        Retriev
-000146f0: 6573 2074 6865 206d 6178 696d 756d 206e  es the maximum n
-00014700: 756d 6265 7220 6f66 2072 6567 6973 7472  umber of registr
-00014710: 6174 696f 6e73 2074 6861 7420 6361 6e20  ations that can 
-00014720: 0a20 2020 2020 2020 2062 6520 7072 6f63  .        be proc
-00014730: 6573 7365 6420 696e 2065 6163 6820 626c  essed in each bl
-00014740: 6f63 6b20 7769 7468 696e 2074 6865 206e  ock within the n
-00014750: 6574 776f 726b 2e0a 0a20 2020 2020 2020  etwork...       
-00014760: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00014770: 2020 2020 2020 5468 6520 6d61 7869 6d75        The maximu
-00014780: 6d20 6e75 6d62 6572 206f 6620 7265 6769  m number of regi
-00014790: 7374 7261 7469 6f6e 7320 7065 7220 626c  strations per bl
-000147a0: 6f63 6b20 6f6e 2074 6865 206e 6574 776f  ock on the netwo
-000147b0: 726b 2e0a 0a20 2020 2020 2020 2052 6169  rk...        Rai
-000147c0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-000147d0: 2051 7565 7279 4572 726f 723a 2049 6620   QueryError: If 
-000147e0: 7468 6520 7175 6572 7920 746f 2074 6865  the query to the
-000147f0: 206e 6574 776f 726b 2066 6169 6c73 206f   network fails o
-00014800: 7220 6973 2069 6e76 616c 6964 2e0a 2020  r is invalid..  
-00014810: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00014820: 2020 2072 6574 7572 6e20 7365 6c66 2e71     return self.q
-00014830: 7565 7279 2822 4d61 7852 6567 6973 7472  uery("MaxRegistr
-00014840: 6174 696f 6e73 5065 7242 6c6f 636b 222c  ationsPerBlock",
-00014850: 2070 6172 616d 733d 5b5d 2c29 0a0a 2020   params=[],)..  
-00014860: 2020 6465 6620 6765 745f 6d61 785f 6e61    def get_max_na
-00014870: 6d65 5f6c 656e 6774 6828 7365 6c66 2920  me_length(self) 
-00014880: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00014890: 2222 220a 2020 2020 2020 2020 5175 6572  """.        Quer
-000148a0: 6965 7320 7468 6520 6e65 7477 6f72 6b20  ies the network 
-000148b0: 666f 7220 7468 6520 6d61 7869 6d75 6d20  for the maximum 
-000148c0: 6c65 6e67 7468 2061 6c6c 6f77 6564 2066  length allowed f
-000148d0: 6f72 206e 616d 6573 2e0a 0a20 2020 2020  or names...     
-000148e0: 2020 2052 6574 7269 6576 6573 2074 6865     Retrieves the
-000148f0: 206d 6178 696d 756d 2063 6861 7261 6374   maximum charact
-00014900: 6572 206c 656e 6774 6820 7065 726d 6974  er length permit
-00014910: 7465 6420 666f 7220 6e61 6d65 7320 0a20  ted for names . 
-00014920: 2020 2020 2020 2077 6974 6869 6e20 7468         within th
-00014930: 6520 6e65 7477 6f72 6b2e 2053 7563 6820  e network. Such 
-00014940: 6173 2074 6865 206d 6f64 756c 6520 6e61  as the module na
-00014950: 6d65 730a 0a20 2020 2020 2020 2052 6574  mes..        Ret
-00014960: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00014970: 2020 5468 6520 6d61 7869 6d75 6d20 6c65    The maximum le
-00014980: 6e67 7468 2061 6c6c 6f77 6564 2066 6f72  ngth allowed for
-00014990: 206e 616d 6573 206f 6e20 7468 6520 6e65   names on the ne
-000149a0: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
-000149b0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-000149c0: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
-000149d0: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
-000149e0: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
-000149f0: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
-00014a00: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00014a10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00014a20: 662e 7175 6572 7928 224d 6178 4e61 6d65  f.query("MaxName
-00014a30: 4c65 6e67 7468 222c 2070 6172 616d 733d  Length", params=
-00014a40: 5b5d 2c29 0a0a 2020 2020 6465 6620 6765  [],)..    def ge
-00014a50: 745f 676c 6f62 616c 5f76 6f74 655f 7468  t_global_vote_th
-00014a60: 7265 7368 6f6c 6428 7365 6c66 2920 2d3e  reshold(self) ->
-00014a70: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
-00014a80: 220a 2020 2020 2020 2020 5175 6572 6965  ".        Querie
-00014a90: 7320 7468 6520 6e65 7477 6f72 6b20 666f  s the network fo
-00014aa0: 7220 7468 6520 676c 6f62 616c 2076 6f74  r the global vot
-00014ab0: 6520 7468 7265 7368 6f6c 642e 0a0a 2020  e threshold...  
-00014ac0: 2020 2020 2020 5265 7472 6965 7665 7320        Retrieves 
-00014ad0: 7468 6520 676c 6f62 616c 2076 6f74 6520  the global vote 
-00014ae0: 7468 7265 7368 6f6c 642c 2077 6869 6368  threshold, which
-00014af0: 2069 7320 7468 6520 6372 6974 6963 616c   is the critical
-00014b00: 2076 616c 7565 206f 7220 0a20 2020 2020   value or .     
-00014b10: 2020 2070 6572 6365 6e74 6167 6520 7265     percentage re
-00014b20: 7175 6972 6564 2066 6f72 2064 6563 6973  quired for decis
-00014b30: 696f 6e73 2069 6e20 7468 6520 6e65 7477  ions in the netw
-00014b40: 6f72 6b27 7320 676f 7665 726e 616e 6365  ork's governance
-00014b50: 2070 726f 6365 7373 2e0a 0a20 2020 2020   process...     
-00014b60: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00014b70: 2020 2020 2020 2020 5468 6520 676c 6f62          The glob
-00014b80: 616c 2076 6f74 6520 7468 7265 7368 6f6c  al vote threshol
-00014b90: 6420 666f 7220 7468 6520 6e65 7477 6f72  d for the networ
-00014ba0: 6b2e 0a0a 2020 2020 2020 2020 5261 6973  k...        Rais
-00014bb0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00014bc0: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
-00014bd0: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
-00014be0: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
-00014bf0: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
-00014c00: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00014c10: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
-00014c20: 6572 7928 2247 6c6f 6261 6c56 6f74 6554  ery("GlobalVoteT
-00014c30: 6872 6573 686f 6c64 222c 290a 0a20 2020  hreshold",)..   
-00014c40: 2064 6566 2067 6574 5f6d 6178 5f61 6c6c   def get_max_all
-00014c50: 6f77 6564 5f73 7562 6e65 7473 2873 656c  owed_subnets(sel
-00014c60: 6629 202d 3e20 696e 743a 0a20 2020 2020  f) -> int:.     
-00014c70: 2020 2022 2222 0a20 2020 2020 2020 2051     """.        Q
-00014c80: 7565 7269 6573 2074 6865 206e 6574 776f  ueries the netwo
-00014c90: 726b 2066 6f72 2074 6865 206d 6178 696d  rk for the maxim
-00014ca0: 756d 206e 756d 6265 7220 6f66 2061 6c6c  um number of all
-00014cb0: 6f77 6564 2073 7562 6e65 7473 2e0a 0a20  owed subnets... 
-00014cc0: 2020 2020 2020 2052 6574 7269 6576 6573         Retrieves
-00014cd0: 2074 6865 2075 7070 6572 206c 696d 6974   the upper limit
-00014ce0: 206f 6e20 7468 6520 6e75 6d62 6572 206f   on the number o
-00014cf0: 6620 7375 626e 6574 7320 7468 6174 2063  f subnets that c
-00014d00: 616e 200a 2020 2020 2020 2020 6265 2063  an .        be c
-00014d10: 7265 6174 6564 206f 7220 6f70 6572 6174  reated or operat
-00014d20: 6564 2077 6974 6869 6e20 7468 6520 6e65  ed within the ne
-00014d30: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
-00014d40: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00014d50: 2020 2020 2054 6865 206d 6178 696d 756d       The maximum
-00014d60: 206e 756d 6265 7220 6f66 2061 6c6c 6f77   number of allow
-00014d70: 6564 2073 7562 6e65 7473 206f 6e20 7468  ed subnets on th
-00014d80: 6520 6e65 7477 6f72 6b2e 0a0a 2020 2020  e network...    
-00014d90: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00014da0: 2020 2020 2020 2020 5175 6572 7945 7272          QueryErr
-00014db0: 6f72 3a20 4966 2074 6865 2071 7565 7279  or: If the query
-00014dc0: 2074 6f20 7468 6520 6e65 7477 6f72 6b20   to the network 
-00014dd0: 6661 696c 7320 6f72 2069 7320 696e 7661  fails or is inva
-00014de0: 6c69 642e 0a20 2020 2020 2020 2022 2222  lid..        """
-00014df0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00014e00: 2073 656c 662e 7175 6572 7928 224d 6178   self.query("Max
-00014e10: 416c 6c6f 7765 6453 7562 6e65 7473 222c  AllowedSubnets",
-00014e20: 2070 6172 616d 733d 5b5d 2c29 0a0a 2020   params=[],)..  
-00014e30: 2020 6465 6620 6765 745f 6d61 785f 616c    def get_max_al
-00014e40: 6c6f 7765 645f 6d6f 6475 6c65 7328 7365  lowed_modules(se
-00014e50: 6c66 2920 2d3e 2069 6e74 3a0a 2020 2020  lf) -> int:.    
-00014e60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00014e70: 5175 6572 6965 7320 7468 6520 6e65 7477  Queries the netw
-00014e80: 6f72 6b20 666f 7220 7468 6520 6d61 7869  ork for the maxi
-00014e90: 6d75 6d20 6e75 6d62 6572 206f 6620 616c  mum number of al
-00014ea0: 6c6f 7765 6420 6d6f 6475 6c65 732e 0a0a  lowed modules...
-00014eb0: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
-00014ec0: 7320 7468 6520 7570 7065 7220 6c69 6d69  s the upper limi
-00014ed0: 7420 6f6e 2074 6865 206e 756d 6265 7220  t on the number 
-00014ee0: 6f66 206d 6f64 756c 6573 2074 6861 7420  of modules that 
-00014ef0: 0a20 2020 2020 2020 2063 616e 2062 6520  .        can be 
-00014f00: 7265 6769 7374 6572 6564 2077 6974 6869  registered withi
-00014f10: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a0a  n the network...
-00014f20: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00014f30: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00014f40: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
-00014f50: 6f66 2061 6c6c 6f77 6564 206d 6f64 756c  of allowed modul
-00014f60: 6573 206f 6e20 7468 6520 6e65 7477 6f72  es on the networ
-00014f70: 6b2e 0a0a 2020 2020 2020 2020 5261 6973  k...        Rais
-00014f80: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00014f90: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
-00014fa0: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
-00014fb0: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
-00014fc0: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
-00014fd0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00014fe0: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
-00014ff0: 6572 7928 224d 6178 416c 6c6f 7765 644d  ery("MaxAllowedM
-00015000: 6f64 756c 6573 222c 2070 6172 616d 733d  odules", params=
-00015010: 5b5d 2c29 0a0a 2020 2020 6465 6620 6765  [],)..    def ge
-00015020: 745f 6d69 6e5f 7374 616b 6528 7365 6c66  t_min_stake(self
-00015030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015040: 2020 2020 2020 2020 6e65 7475 6964 3a20          netuid: 
-00015050: 696e 7420 3d20 3029 202d 3e20 696e 743a  int = 0) -> int:
-00015060: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015070: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
-00015080: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
-00015090: 206d 696e 696d 756d 2073 7461 6b65 2072   minimum stake r
-000150a0: 6571 7569 7265 6420 746f 2072 6567 6973  equired to regis
-000150b0: 7465 7220 6120 6b65 792e 0a0a 2020 2020  ter a key...    
-000150c0: 2020 2020 5265 7472 6965 7665 7320 7468      Retrieves th
-000150d0: 6520 6d69 6e69 6d75 6d20 616d 6f75 6e74  e minimum amount
-000150e0: 206f 6620 7374 616b 6520 6e65 6365 7373   of stake necess
-000150f0: 6172 7920 666f 7220 0a20 2020 2020 2020  ary for .       
-00015100: 2072 6567 6973 7465 7269 6e67 2061 206b   registering a k
-00015110: 6579 2077 6974 6869 6e20 6120 7370 6563  ey within a spec
-00015120: 6966 6963 206e 6574 776f 726b 2073 7562  ific network sub
-00015130: 6e65 742e 0a0a 2020 2020 2020 2020 4172  net...        Ar
-00015140: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00015150: 6e65 7475 6964 3a20 5468 6520 6e65 7477  netuid: The netw
-00015160: 6f72 6b20 5549 4420 666f 7220 7768 6963  ork UID for whic
-00015170: 6820 746f 2071 7565 7279 2074 6865 206d  h to query the m
-00015180: 696e 696d 756d 2073 7461 6b65 2e0a 0a20  inimum stake... 
-00015190: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000151a0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-000151b0: 6d69 6e69 6d75 6d20 7374 616b 6520 7265  minimum stake re
-000151c0: 7175 6972 6564 2066 6f72 206b 6579 2072  quired for key r
-000151d0: 6567 6973 7472 6174 696f 6e20 696e 206e  egistration in n
-000151e0: 616e 6f73 2e0a 0a20 2020 2020 2020 2052  anos...        R
-000151f0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-00015200: 2020 2051 7565 7279 4572 726f 723a 2049     QueryError: I
-00015210: 6620 7468 6520 7175 6572 7920 746f 2074  f the query to t
-00015220: 6865 206e 6574 776f 726b 2066 6169 6c73  he network fails
-00015230: 206f 7220 6973 2069 6e76 616c 6964 2e0a   or is invalid..
-00015240: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00015250: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00015260: 2e71 7565 7279 2827 4d69 6e53 7461 6b65  .query('MinStake
-00015270: 272c 2070 6172 616d 733d 5b6e 6574 7569  ', params=[netui
-00015280: 645d 290a 0a20 2020 2064 6566 2067 6574  d])..    def get
-00015290: 5f73 7461 6b65 2873 656c 662c 0a20 2020  _stake(self,.   
-000152a0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-000152b0: 6579 3a20 5373 3538 4164 6472 6573 732c  ey: Ss58Address,
-000152c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000152d0: 2020 206e 6574 7569 643a 2069 6e74 203d     netuid: int =
-000152e0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
-000152f0: 2020 2020 2020 2920 2d3e 2069 6e74 3a0a        ) -> int:.
-00015300: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00015310: 2020 2020 5175 6572 6965 7320 7468 6520      Queries the 
-00015320: 6e65 7477 6f72 6b20 666f 7220 7468 6520  network for the 
-00015330: 7374 616b 6520 6465 6c65 6761 7465 6420  stake delegated 
-00015340: 7769 7468 2061 2073 7065 6369 6669 6320  with a specific 
-00015350: 6b65 792e 0a0a 2020 2020 2020 2020 5265  key...        Re
-00015360: 7472 6965 7665 7320 7468 6520 616d 6f75  trieves the amou
-00015370: 6e74 206f 6620 746f 7461 6c20 7374 616b  nt of total stak
-00015380: 6564 2074 6f6b 656e 7320 0a20 2020 2020  ed tokens .     
-00015390: 2020 2064 656c 6567 6174 6564 2061 2073     delegated a s
-000153a0: 7065 6369 6669 6320 6b65 7920 6164 6472  pecific key addr
-000153b0: 6573 730a 0a20 2020 2020 2020 2041 7267  ess..        Arg
-000153c0: 733a 0a20 2020 2020 2020 2020 2020 206b  s:.            k
-000153d0: 6579 3a20 5468 6520 6164 6472 6573 7320  ey: The address 
-000153e0: 6f66 2074 6865 206b 6579 2074 6f20 7175  of the key to qu
-000153f0: 6572 7920 7468 6520 7374 616b 6520 666f  ery the stake fo
-00015400: 722e 0a20 2020 2020 2020 2020 2020 206e  r..            n
-00015410: 6574 7569 643a 2054 6865 206e 6574 776f  etuid: The netwo
-00015420: 726b 2055 4944 2066 726f 6d20 7768 6963  rk UID from whic
-00015430: 6820 746f 2067 6574 2074 6865 2071 7565  h to get the que
-00015440: 7279 2e0a 0a20 2020 2020 2020 2052 6574  ry...        Ret
-00015450: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00015460: 2020 5468 6520 616d 6f75 6e74 206f 6620    The amount of 
-00015470: 7374 616b 6520 6865 6c64 2062 7920 7468  stake held by th
-00015480: 6520 7370 6563 6966 6965 6420 6b65 7920  e specified key 
-00015490: 696e 206e 616e 6f73 2e0a 0a20 2020 2020  in nanos...     
-000154a0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-000154b0: 2020 2020 2020 2051 7565 7279 4572 726f         QueryErro
-000154c0: 723a 2049 6620 7468 6520 7175 6572 7920  r: If the query 
-000154d0: 746f 2074 6865 206e 6574 776f 726b 2066  to the network f
-000154e0: 6169 6c73 206f 7220 6973 2069 6e76 616c  ails or is inval
-000154f0: 6964 2e0a 2020 2020 2020 2020 2222 220a  id..        """.
-00015500: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015510: 7365 6c66 2e71 7565 7279 2822 5374 616b  self.query("Stak
-00015520: 6522 2c20 7061 7261 6d73 3d5b 6e65 7475  e", params=[netu
-00015530: 6964 2c20 6b65 795d 2c29 0a0a 2020 2020  id, key],)..    
-00015540: 6465 6620 6765 745f 7374 616b 6566 726f  def get_stakefro
-00015550: 6d28 0a20 2020 2020 2020 2073 656c 662c  m(.        self,
-00015560: 0a20 2020 2020 2020 206b 6579 5f61 6464  .        key_add
-00015570: 723a 2053 7335 3841 6464 7265 7373 2c0a  r: Ss58Address,.
-00015580: 2020 2020 2020 2020 6e65 7475 6964 3a20          netuid: 
-00015590: 696e 7420 3d20 302c 0a20 2020 2029 202d  int = 0,.    ) -
-000155a0: 3e20 6469 6374 5b73 7472 2c20 696e 745d  > dict[str, int]
-000155b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000155c0: 2020 2020 2020 5265 7472 6965 7665 7320        Retrieves 
-000155d0: 6120 6c69 7374 206f 6620 6b65 7973 2066  a list of keys f
-000155e0: 726f 6d20 7768 6963 6820 6120 7370 6563  rom which a spec
-000155f0: 6966 6963 206b 6579 2061 6464 7265 7373  ific key address
-00015600: 2069 7320 7374 616b 6564 2e0a 0a20 2020   is staked...   
-00015610: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
-00015620: 206e 6574 776f 726b 2066 6f72 2061 6c6c   network for all
-00015630: 2074 6865 2073 7461 6b65 7320 7265 6365   the stakes rece
-00015640: 6976 6564 2062 7920 6120 0a20 2020 2020  ived by a .     
-00015650: 2020 2070 6172 7469 6375 6c61 7220 6b65     particular ke
-00015660: 7920 6672 6f6d 2064 6966 6665 7265 6e74  y from different
-00015670: 2073 6f75 7263 6573 2e0a 0a20 2020 2020   sources...     
-00015680: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00015690: 2020 2020 206b 6579 5f61 6464 723a 2054       key_addr: T
-000156a0: 6865 2061 6464 7265 7373 206f 6620 7468  he address of th
-000156b0: 6520 6b65 7920 746f 2071 7565 7279 2073  e key to query s
-000156c0: 7461 6b65 7320 6672 6f6d 2e0a 0a20 2020  takes from...   
-000156d0: 2020 2020 2020 2020 206e 6574 7569 643a           netuid:
-000156e0: 2054 6865 206e 6574 776f 726b 2055 4944   The network UID
-000156f0: 2066 726f 6d20 7768 6963 6820 746f 2067   from which to g
-00015700: 6574 2074 6865 2071 7565 7279 2e0a 0a20  et the query... 
-00015710: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00015720: 2020 2020 2020 2020 2020 2020 4120 6469              A di
-00015730: 6374 696f 6e61 7279 206d 6170 7069 6e67  ctionary mapping
-00015740: 206b 6579 2061 6464 7265 7373 6573 2074   key addresses t
-00015750: 6f20 7468 6520 616d 6f75 6e74 206f 6620  o the amount of 
-00015760: 7374 616b 6520 0a20 2020 2020 2020 2020  stake .         
-00015770: 2020 2072 6563 6569 7665 6420 6672 6f6d     received from
-00015780: 2065 6163 682e 0a0a 2020 2020 2020 2020   each...        
-00015790: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-000157a0: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
-000157b0: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
-000157c0: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
-000157d0: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
-000157e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000157f0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00015800: 6c66 2e71 7565 7279 2827 5374 616b 6546  lf.query('StakeF
-00015810: 726f 6d27 2c20 5b6e 6574 7569 642c 206b  rom', [netuid, k
-00015820: 6579 5f61 6464 725d 290a 0a20 2020 2020  ey_addr])..     
-00015830: 2020 2072 6574 7572 6e20 7b6b 3a20 7620     return {k: v 
-00015840: 666f 7220 6b2c 2076 2069 6e20 7265 7375  for k, v in resu
-00015850: 6c74 7d0a 0a20 2020 2064 6566 2067 6574  lt}..    def get
-00015860: 5f73 7461 6b65 746f 280a 2020 2020 2020  _staketo(.      
-00015870: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00015880: 6b65 795f 6164 6472 3a20 5373 3538 4164  key_addr: Ss58Ad
-00015890: 6472 6573 732c 0a20 2020 2020 2020 206e  dress,.        n
-000158a0: 6574 7569 643a 2069 6e74 203d 2030 2c0a  etuid: int = 0,.
-000158b0: 2020 2020 2920 2d3e 2064 6963 745b 7374      ) -> dict[st
-000158c0: 722c 2069 6e74 5d3a 0a20 2020 2020 2020  r, int]:.       
-000158d0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-000158e0: 7269 6576 6573 2061 206c 6973 7420 6f66  rieves a list of
-000158f0: 206b 6579 7320 746f 2077 6869 6368 2061   keys to which a
-00015900: 2073 7065 6369 6669 6320 6b65 7920 6164   specific key ad
-00015910: 6472 6573 7320 7374 616b 6573 2074 6f2e  dress stakes to.
-00015920: 0a0a 2020 2020 2020 2020 5175 6572 6965  ..        Querie
-00015930: 7320 7468 6520 6e65 7477 6f72 6b20 666f  s the network fo
-00015940: 7220 616c 6c20 7468 6520 7374 616b 6573  r all the stakes
-00015950: 206d 6164 6520 6279 2061 2070 6172 7469   made by a parti
-00015960: 6375 6c61 7220 6b65 7920 746f 200a 2020  cular key to .  
-00015970: 2020 2020 2020 6469 6666 6572 656e 7420        different 
-00015980: 6465 7374 696e 6174 696f 6e73 2e0a 0a20  destinations... 
-00015990: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000159a0: 2020 2020 2020 2020 206b 6579 5f61 6464           key_add
-000159b0: 723a 2054 6865 2061 6464 7265 7373 206f  r: The address o
-000159c0: 6620 7468 6520 6b65 7920 746f 2071 7565  f the key to que
-000159d0: 7279 2073 7461 6b65 7320 746f 2e0a 0a20  ry stakes to... 
-000159e0: 2020 2020 2020 2020 2020 206e 6574 7569             netui
-000159f0: 643a 2054 6865 206e 6574 776f 726b 2055  d: The network U
-00015a00: 4944 2066 726f 6d20 7768 6963 6820 746f  ID from which to
-00015a10: 2067 6574 2074 6865 2071 7565 7279 2e0a   get the query..
-00015a20: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00015a30: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
-00015a40: 6469 6374 696f 6e61 7279 206d 6170 7069  dictionary mappi
-00015a50: 6e67 206b 6579 2061 6464 7265 7373 6573  ng key addresses
-00015a60: 2074 6f20 7468 6520 0a20 2020 2020 2020   to the .       
-00015a70: 2020 2020 2061 6d6f 756e 7420 6f66 2073       amount of s
-00015a80: 7461 6b65 2067 6976 656e 2074 6f20 6561  take given to ea
-00015a90: 6368 2e0a 0a20 2020 2020 2020 2052 6169  ch...        Rai
-00015aa0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00015ab0: 2051 7565 7279 4572 726f 723a 2049 6620   QueryError: If 
-00015ac0: 7468 6520 7175 6572 7920 746f 2074 6865  the query to the
-00015ad0: 206e 6574 776f 726b 2066 6169 6c73 206f   network fails o
-00015ae0: 7220 6973 2069 6e76 616c 6964 2e0a 2020  r is invalid..  
-00015af0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00015b00: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-00015b10: 2e71 7565 7279 2827 5374 616b 6554 6f27  .query('StakeTo'
-00015b20: 2c20 5b6e 6574 7569 642c 206b 6579 5f61  , [netuid, key_a
-00015b30: 6464 725d 290a 0a20 2020 2020 2020 2072  ddr])..        r
-00015b40: 6574 7572 6e20 7b6b 3a20 7620 666f 7220  eturn {k: v for 
-00015b50: 6b2c 2076 2069 6e20 7265 7375 6c74 7d0a  k, v in result}.
-00015b60: 0a20 2020 2064 6566 2067 6574 5f62 616c  .    def get_bal
-00015b70: 616e 6365 280a 2020 2020 2020 2020 7365  ance(.        se
-00015b80: 6c66 2c0a 2020 2020 2020 2020 6164 6472  lf,.        addr
-00015b90: 3a20 5373 3538 4164 6472 6573 732c 0a20  : Ss58Address,. 
-00015ba0: 2020 2029 202d 3e20 696e 743a 0a20 2020     ) -> int:.   
-00015bb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015bc0: 2052 6574 7269 6576 6573 2074 6865 2062   Retrieves the b
-00015bd0: 616c 616e 6365 206f 6620 6120 7370 6563  alance of a spec
-00015be0: 6966 6963 206b 6579 2e0a 0a20 2020 2020  ific key...     
-00015bf0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00015c00: 2020 2020 2061 6464 723a 2054 6865 2061       addr: The a
-00015c10: 6464 7265 7373 206f 6620 7468 6520 6b65  ddress of the ke
-00015c20: 7920 746f 2071 7565 7279 2074 6865 2062  y to query the b
-00015c30: 616c 616e 6365 2066 6f72 2e0a 0a20 2020  alance for...   
-00015c40: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00015c50: 2020 2020 2020 2020 2020 5468 6520 6261            The ba
-00015c60: 6c61 6e63 6520 6f66 2074 6865 2073 7065  lance of the spe
-00015c70: 6369 6669 6564 206b 6579 2e0a 0a20 2020  cified key...   
-00015c80: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-00015c90: 2020 2020 2020 2020 2051 7565 7279 4572           QueryEr
-00015ca0: 726f 723a 2049 6620 7468 6520 7175 6572  ror: If the quer
-00015cb0: 7920 746f 2074 6865 206e 6574 776f 726b  y to the network
-00015cc0: 2066 6169 6c73 206f 7220 6973 2069 6e76   fails or is inv
-00015cd0: 616c 6964 2e0a 2020 2020 2020 2020 2222  alid..        ""
-00015ce0: 220a 0a20 2020 2020 2020 2072 6573 756c  "..        resul
-00015cf0: 7420 3d20 7365 6c66 2e71 7565 7279 2827  t = self.query('
-00015d00: 4163 636f 756e 7427 2c20 6d6f 6475 6c65  Account', module
-00015d10: 3d27 5379 7374 656d 272c 2070 6172 616d  ='System', param
-00015d20: 733d 5b61 6464 725d 290a 0a20 2020 2020  s=[addr])..     
-00015d30: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00015d40: 5b22 6461 7461 225d 5b22 6672 6565 225d  ["data"]["free"]
-00015d50: 0a0a 2020 2020 6465 6620 6765 745f 626c  ..    def get_bl
-00015d60: 6f63 6b28 7365 6c66 2c20 626c 6f63 6b5f  ock(self, block_
-00015d70: 6861 7368 3a20 7374 7220 7c20 4e6f 6e65  hash: str | None
-00015d80: 203d 204e 6f6e 6529 202d 3e20 6469 6374   = None) -> dict
-00015d90: 5b41 6e79 2c20 416e 795d 207c 204e 6f6e  [Any, Any] | Non
-00015da0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00015db0: 2020 2020 2020 2052 6574 7269 6576 6573         Retrieves
-00015dc0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00015dd0: 7574 2061 2073 7065 6369 6669 6320 626c  ut a specific bl
-00015de0: 6f63 6b20 696e 2074 6865 206e 6574 776f  ock in the netwo
-00015df0: 726b 2e0a 0a20 2020 2020 2020 2051 7565  rk...        Que
-00015e00: 7269 6573 2074 6865 206e 6574 776f 726b  ries the network
-00015e10: 2066 6f72 2064 6574 6169 6c73 2061 626f   for details abo
-00015e20: 7574 2061 2062 6c6f 636b 2c20 7375 6368  ut a block, such
-00015e30: 2061 7320 6974 7320 6e75 6d62 6572 2c20   as its number, 
-00015e40: 0a20 2020 2020 2020 2068 6173 682c 2061  .        hash, a
-00015e50: 6e64 206f 7468 6572 2072 656c 6576 616e  nd other relevan
-00015e60: 7420 696e 666f 726d 6174 696f 6e2e 0a0a  t information...
-00015e70: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00015e80: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00015e90: 2072 6571 7565 7374 6564 2069 6e66 6f72   requested infor
-00015ea0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
-00015eb0: 2062 6c6f 636b 2c20 0a20 2020 2020 2020   block, .       
-00015ec0: 2020 2020 206f 7220 4e6f 6e65 2069 6620       or None if 
-00015ed0: 7468 6520 626c 6f63 6b20 646f 6573 206e  the block does n
-00015ee0: 6f74 2065 7869 7374 200a 2020 2020 2020  ot exist .      
-00015ef0: 2020 2020 2020 6f72 2074 6865 2069 6e66        or the inf
-00015f00: 6f72 6d61 7469 6f6e 2069 7320 6e6f 7420  ormation is not 
-00015f10: 6176 6169 6c61 626c 652e 0a0a 2020 2020  available...    
-00015f20: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00015f30: 2020 2020 2020 2020 5175 6572 7945 7272          QueryErr
-00015f40: 6f72 3a20 4966 2074 6865 2071 7565 7279  or: If the query
-00015f50: 2074 6f20 7468 6520 6e65 7477 6f72 6b20   to the network 
-00015f60: 6661 696c 7320 6f72 2069 7320 696e 7661  fails or is inva
-00015f70: 6c69 642e 0a20 2020 2020 2020 2022 2222  lid..        """
-00015f80: 0a0a 2020 2020 2020 2020 7769 7468 2073  ..        with s
-00015f90: 656c 662e 6765 745f 636f 6e6e 2829 2061  elf.get_conn() a
-00015fa0: 7320 7375 6273 7472 6174 653a 0a20 2020  s substrate:.   
-00015fb0: 2020 2020 2020 2020 2062 6c6f 636b 3a20           block: 
-00015fc0: 6469 6374 5b41 6e79 2c20 416e 795d 207c  dict[Any, Any] |
-00015fd0: 204e 6f6e 6520 3d20 7375 6273 7472 6174   None = substrat
-00015fe0: 652e 6765 745f 626c 6f63 6b28 2020 2320  e.get_block(  # 
-00015ff0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-00016000: 2020 2020 2020 2020 2020 2020 2062 6c6f               blo
-00016010: 636b 5f68 6173 6820 2023 2074 7970 653a  ck_hash  # type:
-00016020: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
-00016030: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-00016040: 6574 7572 6e20 626c 6f63 6b0a 0a20 2020  eturn block..   
-00016050: 2064 6566 2067 6574 5f65 7869 7374 656e   def get_existen
-00016060: 7469 616c 5f64 6570 6f73 6974 2873 656c  tial_deposit(sel
-00016070: 662c 2062 6c6f 636b 5f68 6173 683a 2073  f, block_hash: s
-00016080: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
-00016090: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-000160a0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-000160b0: 7472 6965 7665 7320 7468 6520 6578 6973  trieves the exis
-000160c0: 7465 6e74 6961 6c20 6465 706f 7369 7420  tential deposit 
-000160d0: 7661 6c75 6520 666f 7220 7468 6520 6e65  value for the ne
-000160e0: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
-000160f0: 5468 6520 6578 6973 7465 6e74 6961 6c20  The existential 
-00016100: 6465 706f 7369 7420 6973 2074 6865 206d  deposit is the m
-00016110: 696e 696d 756d 2062 616c 616e 6365 2074  inimum balance t
-00016120: 6861 7420 6d75 7374 2062 6520 6d61 696e  hat must be main
-00016130: 7461 696e 6564 200a 2020 2020 2020 2020  tained .        
-00016140: 696e 2061 6e20 6163 636f 756e 7420 746f  in an account to
-00016150: 2070 7265 7665 6e74 2069 7420 6672 6f6d   prevent it from
-00016160: 2062 6569 6e67 2070 7572 6765 642e 2044   being purged. D
-00016170: 656e 6f74 6174 6564 2069 6e20 6e61 6e6f  enotated in nano
-00016180: 2075 6e69 7473 2e0a 0a20 2020 2020 2020   units...       
-00016190: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000161a0: 2020 2020 2020 5468 6520 6578 6973 7465        The existe
-000161b0: 6e74 6961 6c20 6465 706f 7369 7420 7661  ntial deposit va
-000161c0: 6c75 6520 696e 206e 616e 6f20 756e 6974  lue in nano unit
-000161d0: 732e 200a 2020 2020 2020 2020 4e6f 7465  s. .        Note
-000161e0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-000161f0: 6520 7661 6c75 6520 7265 7475 726e 6564  e value returned
-00016200: 2069 7320 6120 6669 7865 6420 7661 6c75   is a fixed valu
-00016210: 6520 6465 6669 6e65 6420 696e 2074 6865  e defined in the
-00016220: 200a 2020 2020 2020 2020 2020 2020 636c   .            cl
-00016230: 6965 6e74 2061 6e64 206d 6179 206e 6f74  ient and may not
-00016240: 2072 6566 6c65 6374 2063 6861 6e67 6573   reflect changes
-00016250: 2069 6e20 7468 6520 6e65 7477 6f72 6b27   in the network'
-00016260: 7320 636f 6e66 6967 7572 6174 696f 6e2e  s configuration.
-00016270: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00016280: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-00016290: 6765 745f 636f 6e6e 2829 2061 7320 7375  get_conn() as su
-000162a0: 6273 7472 6174 653a 0a20 2020 2020 2020  bstrate:.       
-000162b0: 2020 2020 2072 6573 756c 743a 2069 6e74       result: int
-000162c0: 203d 2073 7562 7374 7261 7465 2e67 6574   = substrate.get
-000162d0: 5f63 6f6e 7374 616e 7428 2020 2320 c2a0  _constant(  # ..
-000162e0: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-000162f0: 2020 2020 2020 2020 2020 2020 2022 4261               "Ba
-00016300: 6c61 6e63 6573 222c 2022 4578 6973 7465  lances", "Existe
-00016310: 6e74 6961 6c44 6570 6f73 6974 222c 2062  ntialDeposit", b
-00016320: 6c6f 636b 5f68 6173 6829 2e76 616c 7565  lock_hash).value
-00016330: 2020 2320 c2a0 7479 7065 3a20 6967 6e6f    # ..type: igno
-00016340: 7265 0a0a 2020 2020 2020 2020 7265 7475  re..        retu
-00016350: 726e 2072 6573 756c 740a                 rn result.
+00012610: 290a 0a20 2020 2064 6566 2067 6574 5f73  )..    def get_s
+00012620: 7562 6e65 745f 6e61 6d65 2873 656c 662c  ubnet_name(self,
+00012630: 206e 6574 7569 643a 2069 6e74 203d 2030   netuid: int = 0
+00012640: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00012650: 2020 2222 220a 2020 2020 2020 2020 5175    """.        Qu
+00012660: 6572 6965 7320 7468 6520 6e65 7477 6f72  eries the networ
+00012670: 6b20 666f 7220 7468 6520 6e61 6d65 206f  k for the name o
+00012680: 6620 6120 7370 6563 6966 6963 2073 7562  f a specific sub
+00012690: 6e65 742e 0a0a 2020 2020 2020 2020 4172  net...        Ar
+000126a0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000126b0: 6e65 7475 6964 3a20 5468 6520 6e65 7477  netuid: The netw
+000126c0: 6f72 6b20 5549 4420 666f 7220 7768 6963  ork UID for whic
+000126d0: 6820 746f 2071 7565 7279 2074 6865 206e  h to query the n
+000126e0: 616d 652e 0a0a 2020 2020 2020 2020 5265  ame...        Re
+000126f0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00012700: 2020 2054 6865 206e 616d 6520 6f66 2074     The name of t
+00012710: 6865 2073 7065 6369 6669 6564 206e 6574  he specified net
+00012720: 776f 726b 2073 7562 6e65 742e 0a0a 2020  work subnet...  
+00012730: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+00012740: 2020 2020 2020 2020 2020 5175 6572 7945            QueryE
+00012750: 7272 6f72 3a20 4966 2074 6865 2071 7565  rror: If the que
+00012760: 7279 2074 6f20 7468 6520 6e65 7477 6f72  ry to the networ
+00012770: 6b20 6661 696c 7320 6f72 2069 7320 696e  k fails or is in
+00012780: 7661 6c69 642e 0a20 2020 2020 2020 2022  valid..        "
+00012790: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
+000127a0: 726e 2073 656c 662e 7175 6572 7928 2253  rn self.query("S
+000127b0: 7562 6e65 744e 616d 6573 222c 2070 6172  ubnetNames", par
+000127c0: 616d 733d 5b6e 6574 7569 645d 290a 0a20  ams=[netuid]).. 
+000127d0: 2020 2064 6566 2067 6574 5f6e 2873 656c     def get_n(sel
+000127e0: 662c 206e 6574 7569 643a 2069 6e74 203d  f, netuid: int =
+000127f0: 2030 2920 2d3e 2069 6e74 3a0a 2020 2020   0) -> int:.    
+00012800: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012810: 5175 6572 6965 7320 7468 6520 6e65 7477  Queries the netw
+00012820: 6f72 6b20 666f 7220 7468 6520 274e 2720  ork for the 'N' 
+00012830: 6879 7065 7270 6172 616d 6574 6572 2c20  hyperparameter, 
+00012840: 7768 6963 6820 7265 7072 6573 656e 7473  which represents
+00012850: 2068 6f77 0a20 2020 2020 2020 206d 616e   how.        man
+00012860: 7920 6d6f 6475 6c65 7320 6172 6520 6f6e  y modules are on
+00012870: 2074 6865 206e 6574 776f 726b 2e0a 0a20   the network... 
+00012880: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00012890: 2020 2020 2020 2020 206e 6574 7569 643a           netuid:
+000128a0: 2054 6865 206e 6574 776f 726b 2055 4944   The network UID
+000128b0: 2066 6f72 2077 6869 6368 2074 6f20 7175   for which to qu
+000128c0: 6572 7920 7468 6520 274e 2720 6879 7065  ery the 'N' hype
+000128d0: 7270 6172 616d 6574 6572 2e0a 0a20 2020  rparameter...   
+000128e0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+000128f0: 2020 2020 2020 2020 2020 5468 6520 7661            The va
+00012900: 6c75 6520 6f66 2074 6865 2027 4e27 2068  lue of the 'N' h
+00012910: 7970 6572 7061 7261 6d65 7465 7220 666f  yperparameter fo
+00012920: 7220 7468 6520 7370 6563 6966 6965 6420  r the specified 
+00012930: 6e65 7477 6f72 6b0a 2020 2020 2020 2020  network.        
+00012940: 2020 2020 2020 7375 626e 6574 2e0a 0a20        subnet... 
+00012950: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+00012960: 2020 2020 2020 2020 2020 2051 7565 7279             Query
+00012970: 4572 726f 723a 2049 6620 7468 6520 7175  Error: If the qu
+00012980: 6572 7920 746f 2074 6865 206e 6574 776f  ery to the netwo
+00012990: 726b 2066 6169 6c73 206f 7220 6973 2069  rk fails or is i
+000129a0: 6e76 616c 6964 2e0a 2020 2020 2020 2020  nvalid..        
+000129b0: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+000129c0: 7572 6e20 7365 6c66 2e71 7565 7279 2822  urn self.query("
+000129d0: 4e22 2c20 7061 7261 6d73 3d5b 6e65 7475  N", params=[netu
+000129e0: 6964 5d29 0a0a 2020 2020 6465 6620 6765  id])..    def ge
+000129f0: 745f 7465 6d70 6f28 7365 6c66 2c20 6e65  t_tempo(self, ne
+00012a00: 7475 6964 3a20 696e 7420 3d20 3029 202d  tuid: int = 0) -
+00012a10: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00012a20: 2222 0a20 2020 2020 2020 2051 7565 7269  "".        Queri
+00012a30: 6573 2074 6865 206e 6574 776f 726b 2066  es the network f
+00012a40: 6f72 2074 6865 2074 656d 706f 2073 6574  or the tempo set
+00012a50: 7469 6e67 2c20 6d65 6173 7572 6564 2069  ting, measured i
+00012a60: 6e20 626c 6f63 6b73 2c20 666f 7220 7468  n blocks, for th
+00012a70: 650a 2020 2020 2020 2020 7370 6563 6966  e.        specif
+00012a80: 6965 6420 7375 626e 6574 2e0a 0a20 2020  ied subnet...   
+00012a90: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00012aa0: 2020 2020 2020 206e 6574 7569 643a 2054         netuid: T
+00012ab0: 6865 206e 6574 776f 726b 2055 4944 2066  he network UID f
+00012ac0: 6f72 2077 6869 6368 2074 6f20 7175 6572  or which to quer
+00012ad0: 7920 7468 6520 7465 6d70 6f2e 0a0a 2020  y the tempo...  
+00012ae0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00012af0: 2020 2020 2020 2020 2020 2054 6865 2074             The t
+00012b00: 656d 706f 2073 6574 7469 6e67 2066 6f72  empo setting for
+00012b10: 2074 6865 2073 7065 6369 6669 6564 2073   the specified s
+00012b20: 7562 6e65 742e 0a0a 2020 2020 2020 2020  ubnet...        
+00012b30: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00012b40: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
+00012b50: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
+00012b60: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
+00012b70: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
+00012b80: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00012b90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00012ba0: 662e 7175 6572 7928 2254 656d 706f 222c  f.query("Tempo",
+00012bb0: 2070 6172 616d 733d 5b6e 6574 7569 645d   params=[netuid]
+00012bc0: 290a 0a20 2020 2064 6566 2067 6574 5f74  )..    def get_t
+00012bd0: 6f74 616c 5f73 7461 6b65 2873 656c 662c  otal_stake(self,
+00012be0: 206e 6574 7569 643a 2069 6e74 203d 2030   netuid: int = 0
+00012bf0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012c00: 2020 2020 2020 2051 7565 7269 6573 2074         Queries t
+00012c10: 6865 206e 6574 776f 726b 2066 6f72 2074  he network for t
+00012c20: 6865 2074 6f74 616c 2073 7461 6b65 2061  he total stake a
+00012c30: 6d6f 756e 742e 0a0a 2020 2020 2020 2020  mount...        
+00012c40: 5265 7472 6965 7665 7320 7468 6520 746f  Retrieves the to
+00012c50: 7461 6c20 616d 6f75 6e74 206f 6620 7374  tal amount of st
+00012c60: 616b 6520 7769 7468 696e 2061 2073 7065  ake within a spe
+00012c70: 6369 6669 6320 6e65 7477 6f72 6b20 7375  cific network su
+00012c80: 626e 6574 2e0a 0a20 2020 2020 2020 2041  bnet...        A
+00012c90: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012ca0: 206e 6574 7569 643a 2054 6865 206e 6574   netuid: The net
+00012cb0: 776f 726b 2055 4944 2066 6f72 2077 6869  work UID for whi
+00012cc0: 6368 2074 6f20 7175 6572 7920 7468 6520  ch to query the 
+00012cd0: 746f 7461 6c20 7374 616b 652e 0a0a 2020  total stake...  
+00012ce0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00012cf0: 2020 2020 2020 2020 2020 2054 6865 2074             The t
+00012d00: 6f74 616c 2073 7461 6b65 2061 6d6f 756e  otal stake amoun
+00012d10: 7420 666f 7220 7468 6520 7370 6563 6966  t for the specif
+00012d20: 6965 6420 6e65 7477 6f72 6b20 7375 626e  ied network subn
+00012d30: 6574 2e0a 0a20 2020 2020 2020 2052 6169  et...        Rai
+00012d40: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00012d50: 2051 7565 7279 4572 726f 723a 2049 6620   QueryError: If 
+00012d60: 7468 6520 7175 6572 7920 746f 2074 6865  the query to the
+00012d70: 206e 6574 776f 726b 2066 6169 6c73 206f   network fails o
+00012d80: 7220 6973 2069 6e76 616c 6964 2e0a 2020  r is invalid..  
+00012d90: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00012da0: 2020 2072 6574 7572 6e20 7365 6c66 2e71     return self.q
+00012db0: 7565 7279 2822 546f 7461 6c53 7461 6b65  uery("TotalStake
+00012dc0: 222c 2070 6172 616d 733d 5b6e 6574 7569  ", params=[netui
+00012dd0: 645d 2c29 0a0a 2020 2020 6465 6620 6765  d],)..    def ge
+00012de0: 745f 7265 6769 7374 7261 7469 6f6e 735f  t_registrations_
+00012df0: 7065 725f 626c 6f63 6b28 7365 6c66 293a  per_block(self):
+00012e00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012e10: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
+00012e20: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
+00012e30: 206e 756d 6265 7220 6f66 2072 6567 6973   number of regis
+00012e40: 7472 6174 696f 6e73 2070 6572 2062 6c6f  trations per blo
+00012e50: 636b 2e0a 0a20 2020 2020 2020 2046 6574  ck...        Fet
+00012e60: 6368 6573 2074 6865 206e 756d 6265 7220  ches the number 
+00012e70: 6f66 2072 6567 6973 7472 6174 696f 6e73  of registrations
+00012e80: 2074 6861 7420 6172 6520 7072 6f63 6573   that are proces
+00012e90: 7365 6420 7065 7220 0a20 2020 2020 2020  sed per .       
+00012ea0: 2062 6c6f 636b 2077 6974 6869 6e20 7468   block within th
+00012eb0: 6520 6e65 7477 6f72 6b2e 0a0a 2020 2020  e network...    
+00012ec0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00012ed0: 2020 2020 2020 2020 2054 6865 206e 756d           The num
+00012ee0: 6265 7220 6f66 2072 6567 6973 7472 6174  ber of registrat
+00012ef0: 696f 6e73 2070 726f 6365 7373 6564 2070  ions processed p
+00012f00: 6572 2062 6c6f 636b 2e0a 0a20 2020 2020  er block...     
+00012f10: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+00012f20: 2020 2020 2020 2051 7565 7279 4572 726f         QueryErro
+00012f30: 723a 2049 6620 7468 6520 7175 6572 7920  r: If the query 
+00012f40: 746f 2074 6865 206e 6574 776f 726b 2066  to the network f
+00012f50: 6169 6c73 206f 7220 6973 2069 6e76 616c  ails or is inval
+00012f60: 6964 2e0a 2020 2020 2020 2020 2222 220a  id..        """.
+00012f70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012f80: 7365 6c66 2e71 7565 7279 2822 5265 6769  self.query("Regi
+00012f90: 7374 7261 7469 6f6e 7350 6572 426c 6f63  strationsPerBloc
+00012fa0: 6b22 2c29 0a0a 2020 2020 6465 6620 6d61  k",)..    def ma
+00012fb0: 785f 7265 6769 7374 7261 7469 6f6e 735f  x_registrations_
+00012fc0: 7065 725f 626c 6f63 6b28 7365 6c66 2c20  per_block(self, 
+00012fd0: 6e65 7475 6964 3a20 696e 7420 3d20 3029  netuid: int = 0)
+00012fe0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00012ff0: 2020 2020 2020 5175 6572 6965 7320 7468        Queries th
+00013000: 6520 6e65 7477 6f72 6b20 666f 7220 7468  e network for th
+00013010: 6520 6d61 7869 6d75 6d20 6e75 6d62 6572  e maximum number
+00013020: 206f 6620 7265 6769 7374 7261 7469 6f6e   of registration
+00013030: 7320 7065 7220 626c 6f63 6b2e 0a0a 2020  s per block...  
+00013040: 2020 2020 2020 5265 7472 6965 7665 7320        Retrieves 
+00013050: 7468 6520 7570 7065 7220 6c69 6d69 7420  the upper limit 
+00013060: 6f66 2072 6567 6973 7472 6174 696f 6e73  of registrations
+00013070: 2074 6861 7420 6361 6e20 6265 2070 726f   that can be pro
+00013080: 6365 7373 6564 2069 6e20 0a20 2020 2020  cessed in .     
+00013090: 2020 2065 6163 6820 626c 6f63 6b20 7769     each block wi
+000130a0: 7468 696e 2061 2073 7065 6369 6669 6320  thin a specific 
+000130b0: 6e65 7477 6f72 6b20 7375 626e 6574 2e0a  network subnet..
+000130c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+000130d0: 2020 2020 2020 2020 2020 206e 6574 7569             netui
+000130e0: 643a 2054 6865 206e 6574 776f 726b 2055  d: The network U
+000130f0: 4944 2066 6f72 2077 6869 6368 2074 6f20  ID for which to 
+00013100: 7175 6572 792e 0a0a 2020 2020 2020 2020  query...        
+00013110: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00013120: 2020 2020 2054 6865 206d 6178 696d 756d       The maximum
+00013130: 206e 756d 6265 7220 6f66 2072 6567 6973   number of regis
+00013140: 7472 6174 696f 6e73 2070 6572 2062 6c6f  trations per blo
+00013150: 636b 2066 6f72 200a 2020 2020 2020 2020  ck for .        
+00013160: 2020 2020 7468 6520 7370 6563 6966 6965      the specifie
+00013170: 6420 6e65 7477 6f72 6b20 7375 626e 6574  d network subnet
+00013180: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00013190: 733a 0a20 2020 2020 2020 2020 2020 2051  s:.            Q
+000131a0: 7565 7279 4572 726f 723a 2049 6620 7468  ueryError: If th
+000131b0: 6520 7175 6572 7920 746f 2074 6865 206e  e query to the n
+000131c0: 6574 776f 726b 2066 6169 6c73 206f 7220  etwork fails or 
+000131d0: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
+000131e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000131f0: 2072 6574 7572 6e20 7365 6c66 2e71 7565   return self.que
+00013200: 7279 2822 4d61 7852 6567 6973 7472 6174  ry("MaxRegistrat
+00013210: 696f 6e73 5065 7242 6c6f 636b 222c 2070  ionsPerBlock", p
+00013220: 6172 616d 733d 5b6e 6574 7569 645d 2c29  arams=[netuid],)
+00013230: 0a0a 2020 2020 6465 6620 6765 745f 7072  ..    def get_pr
+00013240: 6f70 6f73 616c 2873 656c 662c 2070 726f  oposal(self, pro
+00013250: 706f 7361 6c5f 6964 3a20 696e 7420 3d20  posal_id: int = 
+00013260: 3029 3a0a 2020 2020 2020 2020 2222 220a  0):.        """.
+00013270: 2020 2020 2020 2020 5175 6572 6965 7320          Queries 
+00013280: 7468 6520 6e65 7477 6f72 6b20 666f 7220  the network for 
+00013290: 6120 7370 6563 6966 6963 2070 726f 706f  a specific propo
+000132a0: 7361 6c2e 0a0a 2020 2020 2020 2020 4172  sal...        Ar
+000132b0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000132c0: 7072 6f70 6f73 616c 5f69 643a 2054 6865  proposal_id: The
+000132d0: 2049 4420 6f66 2074 6865 2070 726f 706f   ID of the propo
+000132e0: 7361 6c20 746f 2071 7565 7279 2e0a 0a20  sal to query... 
+000132f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00013300: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00013310: 6465 7461 696c 7320 6f66 2074 6865 2073  details of the s
+00013320: 7065 6369 6669 6564 2070 726f 706f 7361  pecified proposa
+00013330: 6c2e 0a0a 2020 2020 2020 2020 5261 6973  l...        Rais
+00013340: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00013350: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
+00013360: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
+00013370: 6e65 7477 6f72 6b20 6661 696c 732c 2069  network fails, i
+00013380: 7320 696e 7661 6c69 642c 200a 2020 2020  s invalid, .    
+00013390: 2020 2020 2020 2020 2020 2020 6f72 2069              or i
+000133a0: 6620 7468 6520 7072 6f70 6f73 616c 2049  f the proposal I
+000133b0: 4420 646f 6573 206e 6f74 2065 7869 7374  D does not exist
+000133c0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+000133d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000133e0: 6c66 2e71 7565 7279 2822 5072 6f70 6f73  lf.query("Propos
+000133f0: 616c 7322 2c20 7061 7261 6d73 3d5b 7072  als", params=[pr
+00013400: 6f70 6f73 616c 5f69 645d 2c29 0a0a 2020  oposal_id],)..  
+00013410: 2020 6465 6620 6765 745f 7472 7573 7428    def get_trust(
+00013420: 7365 6c66 2c20 6e65 7475 6964 3a20 696e  self, netuid: in
+00013430: 7420 3d20 3029 3a0a 2020 2020 2020 2020  t = 0):.        
+00013440: 2222 220a 2020 2020 2020 2020 5175 6572  """.        Quer
+00013450: 6965 7320 7468 6520 6e65 7477 6f72 6b20  ies the network 
+00013460: 666f 7220 7468 6520 7472 7573 7420 7365  for the trust se
+00013470: 7474 696e 6720 6f66 2061 2073 7065 6369  tting of a speci
+00013480: 6669 6320 6e65 7477 6f72 6b20 7375 626e  fic network subn
+00013490: 6574 2e0a 0a20 2020 2020 2020 2052 6574  et...        Ret
+000134a0: 7269 6576 6573 2074 6865 2074 7275 7374  rieves the trust
+000134b0: 206c 6576 656c 206f 7220 7363 6f72 652c   level or score,
+000134c0: 2077 6869 6368 206d 6179 2072 6570 7265   which may repre
+000134d0: 7365 6e74 2074 6865 200a 2020 2020 2020  sent the .      
+000134e0: 2020 6c65 7665 6c20 6f66 2074 7275 7374    level of trust
+000134f0: 776f 7274 6869 6e65 7373 206f 7220 7265  worthiness or re
+00013500: 6c69 6162 696c 6974 7920 7769 7468 696e  liability within
+00013510: 2061 200a 2020 2020 2020 2020 7061 7274   a .        part
+00013520: 6963 756c 6172 206e 6574 776f 726b 2073  icular network s
+00013530: 7562 6e65 742e 0a0a 2020 2020 2020 2020  ubnet...        
+00013540: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00013550: 2020 6e65 7475 6964 3a20 5468 6520 6e65    netuid: The ne
+00013560: 7477 6f72 6b20 5549 4420 666f 7220 7768  twork UID for wh
+00013570: 6963 6820 746f 2071 7565 7279 2074 6865  ich to query the
+00013580: 2074 7275 7374 2073 6574 7469 6e67 2e0a   trust setting..
+00013590: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000135a0: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+000135b0: 6520 7472 7573 7420 6c65 7665 6c20 6f72  e trust level or
+000135c0: 2073 636f 7265 2066 6f72 2074 6865 2073   score for the s
+000135d0: 7065 6369 6669 6564 206e 6574 776f 726b  pecified network
+000135e0: 2073 7562 6e65 742e 0a0a 2020 2020 2020   subnet...      
+000135f0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00013600: 2020 2020 2020 5175 6572 7945 7272 6f72        QueryError
+00013610: 3a20 4966 2074 6865 2071 7565 7279 2074  : If the query t
+00013620: 6f20 7468 6520 6e65 7477 6f72 6b20 6661  o the network fa
+00013630: 696c 7320 6f72 2069 7320 696e 7661 6c69  ils or is invali
+00013640: 642e 0a20 2020 2020 2020 2022 2222 0a0a  d..        """..
+00013650: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00013660: 656c 662e 7175 6572 7928 2254 7275 7374  elf.query("Trust
+00013670: 222c 2070 6172 616d 733d 5b6e 6574 7569  ", params=[netui
+00013680: 645d 2c29 0a0a 2020 2020 6465 6620 6765  d],)..    def ge
+00013690: 745f 7569 6473 2873 656c 662c 206b 6579  t_uids(self, key
+000136a0: 3a20 5373 3538 4164 6472 6573 732c 206e  : Ss58Address, n
+000136b0: 6574 7569 643a 2069 6e74 203d 2030 2920  etuid: int = 0) 
+000136c0: 2d3e 2062 6f6f 6c20 7c20 4e6f 6e65 3a0a  -> bool | None:.
+000136d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000136e0: 2020 2020 5175 6572 6965 7320 7468 6520      Queries the 
+000136f0: 6e65 7477 6f72 6b20 666f 7220 6d6f 6475  network for modu
+00013700: 6c65 2055 4944 7320 6173 736f 6369 6174  le UIDs associat
+00013710: 6564 2077 6974 6820 6120 7370 6563 6966  ed with a specif
+00013720: 6963 206b 6579 2e0a 0a20 2020 2020 2020  ic key...       
+00013730: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00013740: 2020 206b 6579 3a20 5468 6520 6b65 7920     key: The key 
+00013750: 6164 6472 6573 7320 666f 7220 7768 6963  address for whic
+00013760: 6820 746f 2071 7565 7279 2055 4944 732e  h to query UIDs.
+00013770: 0a20 2020 2020 2020 2020 2020 206e 6574  .            net
+00013780: 7569 643a 2054 6865 206e 6574 776f 726b  uid: The network
+00013790: 2055 4944 2077 6974 6869 6e20 7768 6963   UID within whic
+000137a0: 6820 746f 2073 6561 7263 6820 666f 7220  h to search for 
+000137b0: 7468 6520 6b65 792e 0a0a 2020 2020 2020  the key...      
+000137c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000137d0: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
+000137e0: 2055 4944 7320 6173 736f 6369 6174 6564   UIDs associated
+000137f0: 2077 6974 6820 7468 6520 7370 6563 6966   with the specif
+00013800: 6965 6420 6b65 792e 0a0a 2020 2020 2020  ied key...      
+00013810: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00013820: 2020 2020 2020 5175 6572 7945 7272 6f72        QueryError
+00013830: 3a20 4966 2074 6865 2071 7565 7279 2074  : If the query t
+00013840: 6f20 7468 6520 6e65 7477 6f72 6b20 6661  o the network fa
+00013850: 696c 7320 6f72 2069 7320 696e 7661 6c69  ils or is invali
+00013860: 642e 0a20 2020 2020 2020 2022 2222 0a0a  d..        """..
+00013870: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00013880: 656c 662e 7175 6572 7928 2255 6964 7322  elf.query("Uids"
+00013890: 2c20 7061 7261 6d73 3d5b 6e65 7475 6964  , params=[netuid
+000138a0: 2c20 6b65 795d 2c29 0a0a 2020 2020 6465  , key],)..    de
+000138b0: 6620 6765 745f 756e 6974 5f65 6d69 7373  f get_unit_emiss
+000138c0: 696f 6e28 7365 6c66 2920 2d3e 2069 6e74  ion(self) -> int
+000138d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000138e0: 2020 2020 2020 5175 6572 6965 7320 7468        Queries th
+000138f0: 6520 6e65 7477 6f72 6b20 666f 7220 7468  e network for th
+00013900: 6520 756e 6974 2065 6d69 7373 696f 6e20  e unit emission 
+00013910: 7365 7474 696e 672e 0a0a 2020 2020 2020  setting...      
+00013920: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
+00013930: 756e 6974 2065 6d69 7373 696f 6e20 7661  unit emission va
+00013940: 6c75 652c 2077 6869 6368 2072 6570 7265  lue, which repre
+00013950: 7365 6e74 7320 7468 6520 0a20 2020 2020  sents the .     
+00013960: 2020 2065 6d69 7373 696f 6e20 7261 7465     emission rate
+00013970: 206f 7220 7175 616e 7469 7479 2066 6f72   or quantity for
+00013980: 2074 6865 2024 434f 4d41 4920 746f 6b65   the $COMAI toke
+00013990: 6e2e 0a0a 2020 2020 2020 2020 5265 7475  n...        Retu
+000139a0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+000139b0: 2054 6865 2075 6e69 7420 656d 6973 7369   The unit emissi
+000139c0: 6f6e 2076 616c 7565 2069 6e20 6e61 6e6f  on value in nano
+000139d0: 7320 666f 7220 7468 6520 6e65 7477 6f72  s for the networ
+000139e0: 6b2e 0a0a 2020 2020 2020 2020 5261 6973  k...        Rais
+000139f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00013a00: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
+00013a10: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
+00013a20: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
+00013a30: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
+00013a40: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00013a50: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
+00013a60: 6572 7928 2255 6e69 7445 6d69 7373 696f  ery("UnitEmissio
+00013a70: 6e22 290a 0a20 2020 2064 6566 2067 6574  n")..    def get
+00013a80: 5f74 785f 7261 7465 5f6c 696d 6974 2873  _tx_rate_limit(s
+00013a90: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00013aa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013ab0: 2051 7565 7269 6573 2074 6865 206e 6574   Queries the net
+00013ac0: 776f 726b 2066 6f72 2074 6865 2074 7261  work for the tra
+00013ad0: 6e73 6163 7469 6f6e 2072 6174 6520 6c69  nsaction rate li
+00013ae0: 6d69 742e 0a0a 2020 2020 2020 2020 5265  mit...        Re
+00013af0: 7472 6965 7665 7320 7468 6520 7261 7465  trieves the rate
+00013b00: 206c 696d 6974 2066 6f72 2074 7261 6e73   limit for trans
+00013b10: 6163 7469 6f6e 7320 7769 7468 696e 2074  actions within t
+00013b20: 6865 206e 6574 776f 726b 2c20 0a20 2020  he network, .   
+00013b30: 2020 2020 2077 6869 6368 2064 6566 696e       which defin
+00013b40: 6573 2074 6865 206d 6178 696d 756d 206e  es the maximum n
+00013b50: 756d 6265 7220 6f66 2074 7261 6e73 6163  umber of transac
+00013b60: 7469 6f6e 7320 7468 6174 2063 616e 2062  tions that can b
+00013b70: 6520 0a20 2020 2020 2020 2070 726f 6365  e .        proce
+00013b80: 7373 6564 2077 6974 6869 6e20 6120 6365  ssed within a ce
+00013b90: 7274 6169 6e20 7469 6d65 6672 616d 652e  rtain timeframe.
+00013ba0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00013bb0: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00013bc0: 6865 2074 7261 6e73 6163 7469 6f6e 2072  he transaction r
+00013bd0: 6174 6520 6c69 6d69 7420 666f 7220 7468  ate limit for th
+00013be0: 6520 6e65 7477 6f72 6b2e 0a0a 2020 2020  e network...    
+00013bf0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00013c00: 2020 2020 2020 2020 5175 6572 7945 7272          QueryErr
+00013c10: 6f72 3a20 4966 2074 6865 2071 7565 7279  or: If the query
+00013c20: 2074 6f20 7468 6520 6e65 7477 6f72 6b20   to the network 
+00013c30: 6661 696c 7320 6f72 2069 7320 696e 7661  fails or is inva
+00013c40: 6c69 642e 0a20 2020 2020 2020 2022 2222  lid..        """
+00013c50: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013c60: 2073 656c 662e 7175 6572 7928 2254 7852   self.query("TxR
+00013c70: 6174 654c 696d 6974 222c 290a 0a20 2020  ateLimit",)..   
+00013c80: 2064 6566 2067 6574 5f62 7572 6e5f 7261   def get_burn_ra
+00013c90: 7465 2873 656c 6629 202d 3e20 696e 743a  te(self) -> int:
+00013ca0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013cb0: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
+00013cc0: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
+00013cd0: 2062 7572 6e20 7261 7465 2073 6574 7469   burn rate setti
+00013ce0: 6e67 2e0a 0a20 2020 2020 2020 2052 6574  ng...        Ret
+00013cf0: 7269 6576 6573 2074 6865 2062 7572 6e20  rieves the burn 
+00013d00: 7261 7465 2c20 7768 6963 6820 7265 7072  rate, which repr
+00013d10: 6573 656e 7473 2074 6865 2072 6174 6520  esents the rate 
+00013d20: 6174 200a 2020 2020 2020 2020 7768 6963  at .        whic
+00013d30: 6820 7468 6520 2443 4f4d 4149 2074 6f6b  h the $COMAI tok
+00013d40: 656e 2069 7320 7065 726d 616e 656e 746c  en is permanentl
+00013d50: 7920 0a20 2020 2020 2020 2072 656d 6f76  y .        remov
+00013d60: 6564 206f 7220 2762 7572 6e65 6427 2066  ed or 'burned' f
+00013d70: 726f 6d20 6369 7263 756c 6174 696f 6e2e  rom circulation.
+00013d80: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00013d90: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00013da0: 6865 2062 7572 6e20 7261 7465 2066 6f72  he burn rate for
+00013db0: 2074 6865 206e 6574 776f 726b 2e0a 0a20   the network... 
+00013dc0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+00013dd0: 2020 2020 2020 2020 2020 2051 7565 7279             Query
+00013de0: 4572 726f 723a 2049 6620 7468 6520 7175  Error: If the qu
+00013df0: 6572 7920 746f 2074 6865 206e 6574 776f  ery to the netwo
+00013e00: 726b 2066 6169 6c73 206f 7220 6973 2069  rk fails or is i
+00013e10: 6e76 616c 6964 2e0a 2020 2020 2020 2020  nvalid..        
+00013e20: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+00013e30: 7572 6e20 7365 6c66 2e71 7565 7279 2822  urn self.query("
+00013e40: 4275 726e 5261 7465 222c 2070 6172 616d  BurnRate", param
+00013e50: 733d 5b5d 2c29 0a0a 2020 2020 6465 6620  s=[],)..    def 
+00013e60: 6765 745f 6275 726e 2873 656c 6629 202d  get_burn(self) -
+00013e70: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00013e80: 2222 0a20 2020 2020 2020 2051 7565 7269  "".        Queri
+00013e90: 6573 2074 6865 206e 6574 776f 726b 2066  es the network f
+00013ea0: 6f72 2074 6865 2062 7572 6e20 7365 7474  or the burn sett
+00013eb0: 696e 672e 0a0a 2020 2020 2020 2020 5265  ing...        Re
+00013ec0: 7472 6965 7665 7320 7468 6520 6275 726e  trieves the burn
+00013ed0: 2076 616c 7565 2c20 7768 6963 6820 7265   value, which re
+00013ee0: 7072 6573 656e 7473 2074 6865 2061 6d6f  presents the amo
+00013ef0: 756e 7420 6f66 200a 2020 2020 2020 2020  unt of .        
+00013f00: 7468 6520 2443 4f4d 4149 2074 6f6b 656e  the $COMAI token
+00013f10: 7320 7468 6174 2061 7265 2027 6275 726e  s that are 'burn
+00013f20: 6564 2720 6f72 2070 6572 6d61 6e65 6e74  ed' or permanent
+00013f30: 6c79 200a 2020 2020 2020 2020 7265 6d6f  ly .        remo
+00013f40: 7665 6420 6672 6f6d 2063 6972 6375 6c61  ved from circula
+00013f50: 7469 6f6e 2e0a 0a20 2020 2020 2020 2052  tion...        R
+00013f60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00013f70: 2020 2020 5468 6520 6275 726e 2076 616c      The burn val
+00013f80: 7565 2066 6f72 2074 6865 206e 6574 776f  ue for the netwo
+00013f90: 726b 2e0a 0a20 2020 2020 2020 2052 6169  rk...        Rai
+00013fa0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00013fb0: 2051 7565 7279 4572 726f 723a 2049 6620   QueryError: If 
+00013fc0: 7468 6520 7175 6572 7920 746f 2074 6865  the query to the
+00013fd0: 206e 6574 776f 726b 2066 6169 6c73 206f   network fails o
+00013fe0: 7220 6973 2069 6e76 616c 6964 2e0a 2020  r is invalid..  
+00013ff0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00014000: 2020 2072 6574 7572 6e20 7365 6c66 2e71     return self.q
+00014010: 7565 7279 2822 4275 726e 222c 2070 6172  uery("Burn", par
+00014020: 616d 733d 5b5d 2c29 0a0a 2020 2020 6465  ams=[],)..    de
+00014030: 6620 6765 745f 6d69 6e5f 6275 726e 2873  f get_min_burn(s
+00014040: 656c 6629 202d 3e20 696e 743a 0a20 2020  elf) -> int:.   
+00014050: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014060: 2051 7565 7269 6573 2074 6865 206e 6574   Queries the net
+00014070: 776f 726b 2066 6f72 2074 6865 206d 696e  work for the min
+00014080: 696d 756d 2062 7572 6e20 7365 7474 696e  imum burn settin
+00014090: 672e 0a0a 2020 2020 2020 2020 5265 7472  g...        Retr
+000140a0: 6965 7665 7320 7468 6520 6d69 6e69 6d75  ieves the minimu
+000140b0: 6d20 6275 726e 2076 616c 7565 2c20 696e  m burn value, in
+000140c0: 6469 6361 7469 6e67 2074 6865 206c 6f77  dicating the low
+000140d0: 6573 7420 0a20 2020 2020 2020 2061 6d6f  est .        amo
+000140e0: 756e 7420 6f66 2074 6865 2024 434f 4d41  unt of the $COMA
+000140f0: 4920 746f 6b65 6e73 2074 6861 7420 6361  I tokens that ca
+00014100: 6e20 6265 2027 6275 726e 6564 2720 6f72  n be 'burned' or
+00014110: 200a 2020 2020 2020 2020 7065 726d 616e   .        perman
+00014120: 656e 746c 7920 7265 6d6f 7665 6420 6672  ently removed fr
+00014130: 6f6d 2063 6972 6375 6c61 7469 6f6e 2e0a  om circulation..
+00014140: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00014150: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00014160: 6520 6d69 6e69 6d75 6d20 6275 726e 2076  e minimum burn v
+00014170: 616c 7565 2066 6f72 2074 6865 206e 6574  alue for the net
+00014180: 776f 726b 2e0a 0a20 2020 2020 2020 2052  work...        R
+00014190: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+000141a0: 2020 2051 7565 7279 4572 726f 723a 2049     QueryError: I
+000141b0: 6620 7468 6520 7175 6572 7920 746f 2074  f the query to t
+000141c0: 6865 206e 6574 776f 726b 2066 6169 6c73  he network fails
+000141d0: 206f 7220 6973 2069 6e76 616c 6964 2e0a   or is invalid..
+000141e0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+000141f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00014200: 2e71 7565 7279 2822 4d69 6e42 7572 6e22  .query("MinBurn"
+00014210: 2c20 7061 7261 6d73 3d5b 5d2c 290a 0a20  , params=[],).. 
+00014220: 2020 2064 6566 2067 6574 5f6d 696e 5f77     def get_min_w
+00014230: 6569 6768 745f 7374 616b 6528 7365 6c66  eight_stake(self
+00014240: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
+00014250: 2020 2222 220a 2020 2020 2020 2020 5175    """.        Qu
+00014260: 6572 6965 7320 7468 6520 6e65 7477 6f72  eries the networ
+00014270: 6b20 666f 7220 7468 6520 6d69 6e69 6d75  k for the minimu
+00014280: 6d20 7765 6967 6874 2073 7461 6b65 2073  m weight stake s
+00014290: 6574 7469 6e67 2e0a 0a20 2020 2020 2020  etting...       
+000142a0: 2052 6574 7269 6576 6573 2074 6865 206d   Retrieves the m
+000142b0: 696e 696d 756d 2077 6569 6768 7420 7374  inimum weight st
+000142c0: 616b 652c 2077 6869 6368 2072 6570 7265  ake, which repre
+000142d0: 7365 6e74 7320 7468 6520 6c6f 7765 7374  sents the lowest
+000142e0: 200a 2020 2020 2020 2020 7374 616b 6520   .        stake 
+000142f0: 7765 6967 6874 2074 6861 7420 6973 2061  weight that is a
+00014300: 6c6c 6f77 6564 2066 6f72 2063 6572 7461  llowed for certa
+00014310: 696e 206f 7065 7261 7469 6f6e 7320 6f72  in operations or
+00014320: 200a 2020 2020 2020 2020 7472 616e 7361   .        transa
+00014330: 6374 696f 6e73 2077 6974 6869 6e20 7468  ctions within th
+00014340: 6520 6e65 7477 6f72 6b2e 0a0a 2020 2020  e network...    
+00014350: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00014360: 2020 2020 2020 2020 2054 6865 206d 696e           The min
+00014370: 696d 756d 2077 6569 6768 7420 7374 616b  imum weight stak
+00014380: 6520 666f 7220 7468 6520 6e65 7477 6f72  e for the networ
+00014390: 6b2e 0a0a 2020 2020 2020 2020 5261 6973  k...        Rais
+000143a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+000143b0: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
+000143c0: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
+000143d0: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
+000143e0: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
+000143f0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00014400: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
+00014410: 6572 7928 224d 696e 5765 6967 6874 5374  ery("MinWeightSt
+00014420: 616b 6522 2c20 7061 7261 6d73 3d5b 5d29  ake", params=[])
+00014430: 0a0a 2020 2020 6465 6620 6765 745f 766f  ..    def get_vo
+00014440: 7465 5f6d 6f64 655f 676c 6f62 616c 2873  te_mode_global(s
+00014450: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
+00014460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014470: 2051 7565 7269 6573 2074 6865 206e 6574   Queries the net
+00014480: 776f 726b 2066 6f72 2074 6865 2067 6c6f  work for the glo
+00014490: 6261 6c20 766f 7465 206d 6f64 6520 7365  bal vote mode se
+000144a0: 7474 696e 672e 0a0a 2020 2020 2020 2020  tting...        
+000144b0: 5265 7472 6965 7665 7320 7468 6520 676c  Retrieves the gl
+000144c0: 6f62 616c 2076 6f74 6520 6d6f 6465 2c20  obal vote mode, 
+000144d0: 7768 6963 6820 6465 6669 6e65 7320 7468  which defines th
+000144e0: 6520 6f76 6572 616c 6c20 766f 7469 6e67  e overall voting
+000144f0: 200a 2020 2020 2020 2020 6d65 7468 6f64   .        method
+00014500: 6f6c 6f67 7920 6f72 2061 7070 726f 6163  ology or approac
+00014510: 6820 7573 6564 2061 6372 6f73 7320 7468  h used across th
+00014520: 6520 6e65 7477 6f72 6b20 696e 2064 6566  e network in def
+00014530: 6175 6c74 2e0a 0a20 2020 2020 2020 2052  ault...        R
+00014540: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00014550: 2020 2020 5468 6520 676c 6f62 616c 2076      The global v
+00014560: 6f74 6520 6d6f 6465 2073 6574 7469 6e67  ote mode setting
+00014570: 2066 6f72 2074 6865 206e 6574 776f 726b   for the network
+00014580: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00014590: 733a 0a20 2020 2020 2020 2020 2020 2051  s:.            Q
+000145a0: 7565 7279 4572 726f 723a 2049 6620 7468  ueryError: If th
+000145b0: 6520 7175 6572 7920 746f 2074 6865 206e  e query to the n
+000145c0: 6574 776f 726b 2066 6169 6c73 206f 7220  etwork fails or 
+000145d0: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
+000145e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000145f0: 2072 6574 7572 6e20 7365 6c66 2e71 7565   return self.que
+00014600: 7279 2822 566f 7465 4d6f 6465 476c 6f62  ry("VoteModeGlob
+00014610: 616c 222c 290a 0a20 2020 2064 6566 2067  al",)..    def g
+00014620: 6574 5f6d 6178 5f70 726f 706f 7361 6c73  et_max_proposals
+00014630: 2873 656c 6629 202d 3e20 696e 743a 0a20  (self) -> int:. 
+00014640: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014650: 2020 2051 7565 7269 6573 2074 6865 206e     Queries the n
+00014660: 6574 776f 726b 2066 6f72 2074 6865 206d  etwork for the m
+00014670: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+00014680: 2070 726f 706f 7361 6c73 2061 6c6c 6f77   proposals allow
+00014690: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+000146a0: 7269 6576 6573 2074 6865 2075 7070 6572  rieves the upper
+000146b0: 206c 696d 6974 206f 6e20 7468 6520 6e75   limit on the nu
+000146c0: 6d62 6572 206f 6620 7072 6f70 6f73 616c  mber of proposal
+000146d0: 7320 7468 6174 2063 616e 2062 6520 0a20  s that can be . 
+000146e0: 2020 2020 2020 2061 6374 6976 6520 6f72         active or
+000146f0: 2063 6f6e 7369 6465 7265 6420 6174 2061   considered at a
+00014700: 6e79 2067 6976 656e 2074 696d 6520 7769  ny given time wi
+00014710: 7468 696e 2074 6865 206e 6574 776f 726b  thin the network
+00014720: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00014730: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00014740: 5468 6520 6d61 7869 6d75 6d20 6e75 6d62  The maximum numb
+00014750: 6572 206f 6620 7072 6f70 6f73 616c 7320  er of proposals 
+00014760: 616c 6c6f 7765 6420 6f6e 2074 6865 206e  allowed on the n
+00014770: 6574 776f 726b 2e0a 0a20 2020 2020 2020  etwork...       
+00014780: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00014790: 2020 2020 2051 7565 7279 4572 726f 723a       QueryError:
+000147a0: 2049 6620 7468 6520 7175 6572 7920 746f   If the query to
+000147b0: 2074 6865 206e 6574 776f 726b 2066 6169   the network fai
+000147c0: 6c73 206f 7220 6973 2069 6e76 616c 6964  ls or is invalid
+000147d0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+000147e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000147f0: 6c66 2e71 7565 7279 2822 4d61 7850 726f  lf.query("MaxPro
+00014800: 706f 7361 6c73 222c 290a 0a20 2020 2064  posals",)..    d
+00014810: 6566 2067 6574 5f6d 6178 5f72 6567 6973  ef get_max_regis
+00014820: 7472 6174 696f 6e73 5f70 6572 5f62 6c6f  trations_per_blo
+00014830: 636b 2873 656c 6629 202d 3e20 696e 743a  ck(self) -> int:
+00014840: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014850: 2020 2020 2051 7565 7269 6573 2074 6865       Queries the
+00014860: 206e 6574 776f 726b 2066 6f72 2074 6865   network for the
+00014870: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+00014880: 6f66 2072 6567 6973 7472 6174 696f 6e73  of registrations
+00014890: 2070 6572 2062 6c6f 636b 2e0a 0a20 2020   per block...   
+000148a0: 2020 2020 2052 6574 7269 6576 6573 2074       Retrieves t
+000148b0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
+000148c0: 7220 6f66 2072 6567 6973 7472 6174 696f  r of registratio
+000148d0: 6e73 2074 6861 7420 6361 6e20 0a20 2020  ns that can .   
+000148e0: 2020 2020 2062 6520 7072 6f63 6573 7365       be processe
+000148f0: 6420 696e 2065 6163 6820 626c 6f63 6b20  d in each block 
+00014900: 7769 7468 696e 2074 6865 206e 6574 776f  within the netwo
+00014910: 726b 2e0a 0a20 2020 2020 2020 2052 6574  rk...        Ret
+00014920: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00014930: 2020 5468 6520 6d61 7869 6d75 6d20 6e75    The maximum nu
+00014940: 6d62 6572 206f 6620 7265 6769 7374 7261  mber of registra
+00014950: 7469 6f6e 7320 7065 7220 626c 6f63 6b20  tions per block 
+00014960: 6f6e 2074 6865 206e 6574 776f 726b 2e0a  on the network..
+00014970: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+00014980: 0a20 2020 2020 2020 2020 2020 2051 7565  .            Que
+00014990: 7279 4572 726f 723a 2049 6620 7468 6520  ryError: If the 
+000149a0: 7175 6572 7920 746f 2074 6865 206e 6574  query to the net
+000149b0: 776f 726b 2066 6169 6c73 206f 7220 6973  work fails or is
+000149c0: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
+000149d0: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
+000149e0: 6574 7572 6e20 7365 6c66 2e71 7565 7279  eturn self.query
+000149f0: 2822 4d61 7852 6567 6973 7472 6174 696f  ("MaxRegistratio
+00014a00: 6e73 5065 7242 6c6f 636b 222c 2070 6172  nsPerBlock", par
+00014a10: 616d 733d 5b5d 2c29 0a0a 2020 2020 6465  ams=[],)..    de
+00014a20: 6620 6765 745f 6d61 785f 6e61 6d65 5f6c  f get_max_name_l
+00014a30: 656e 6774 6828 7365 6c66 2920 2d3e 2069  ength(self) -> i
+00014a40: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+00014a50: 2020 2020 2020 2020 5175 6572 6965 7320          Queries 
+00014a60: 7468 6520 6e65 7477 6f72 6b20 666f 7220  the network for 
+00014a70: 7468 6520 6d61 7869 6d75 6d20 6c65 6e67  the maximum leng
+00014a80: 7468 2061 6c6c 6f77 6564 2066 6f72 206e  th allowed for n
+00014a90: 616d 6573 2e0a 0a20 2020 2020 2020 2052  ames...        R
+00014aa0: 6574 7269 6576 6573 2074 6865 206d 6178  etrieves the max
+00014ab0: 696d 756d 2063 6861 7261 6374 6572 206c  imum character l
+00014ac0: 656e 6774 6820 7065 726d 6974 7465 6420  ength permitted 
+00014ad0: 666f 7220 6e61 6d65 7320 0a20 2020 2020  for names .     
+00014ae0: 2020 2077 6974 6869 6e20 7468 6520 6e65     within the ne
+00014af0: 7477 6f72 6b2e 2053 7563 6820 6173 2074  twork. Such as t
+00014b00: 6865 206d 6f64 756c 6520 6e61 6d65 730a  he module names.
+00014b10: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00014b20: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00014b30: 6520 6d61 7869 6d75 6d20 6c65 6e67 7468  e maximum length
+00014b40: 2061 6c6c 6f77 6564 2066 6f72 206e 616d   allowed for nam
+00014b50: 6573 206f 6e20 7468 6520 6e65 7477 6f72  es on the networ
+00014b60: 6b2e 0a0a 2020 2020 2020 2020 5261 6973  k...        Rais
+00014b70: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00014b80: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
+00014b90: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
+00014ba0: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
+00014bb0: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
+00014bc0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00014bd0: 2020 7265 7475 726e 2073 656c 662e 7175    return self.qu
+00014be0: 6572 7928 224d 6178 4e61 6d65 4c65 6e67  ery("MaxNameLeng
+00014bf0: 7468 222c 2070 6172 616d 733d 5b5d 2c29  th", params=[],)
+00014c00: 0a0a 2020 2020 6465 6620 6765 745f 676c  ..    def get_gl
+00014c10: 6f62 616c 5f76 6f74 655f 7468 7265 7368  obal_vote_thresh
+00014c20: 6f6c 6428 7365 6c66 2920 2d3e 2069 6e74  old(self) -> int
+00014c30: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00014c40: 2020 2020 2020 5175 6572 6965 7320 7468        Queries th
+00014c50: 6520 6e65 7477 6f72 6b20 666f 7220 7468  e network for th
+00014c60: 6520 676c 6f62 616c 2076 6f74 6520 7468  e global vote th
+00014c70: 7265 7368 6f6c 642e 0a0a 2020 2020 2020  reshold...      
+00014c80: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
+00014c90: 676c 6f62 616c 2076 6f74 6520 7468 7265  global vote thre
+00014ca0: 7368 6f6c 642c 2077 6869 6368 2069 7320  shold, which is 
+00014cb0: 7468 6520 6372 6974 6963 616c 2076 616c  the critical val
+00014cc0: 7565 206f 7220 0a20 2020 2020 2020 2070  ue or .        p
+00014cd0: 6572 6365 6e74 6167 6520 7265 7175 6972  ercentage requir
+00014ce0: 6564 2066 6f72 2064 6563 6973 696f 6e73  ed for decisions
+00014cf0: 2069 6e20 7468 6520 6e65 7477 6f72 6b27   in the network'
+00014d00: 7320 676f 7665 726e 616e 6365 2070 726f  s governance pro
+00014d10: 6365 7373 2e0a 0a20 2020 2020 2020 2052  cess...        R
+00014d20: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00014d30: 2020 2020 5468 6520 676c 6f62 616c 2076      The global v
+00014d40: 6f74 6520 7468 7265 7368 6f6c 6420 666f  ote threshold fo
+00014d50: 7220 7468 6520 6e65 7477 6f72 6b2e 0a0a  r the network...
+00014d60: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00014d70: 2020 2020 2020 2020 2020 2020 5175 6572              Quer
+00014d80: 7945 7272 6f72 3a20 4966 2074 6865 2071  yError: If the q
+00014d90: 7565 7279 2074 6f20 7468 6520 6e65 7477  uery to the netw
+00014da0: 6f72 6b20 6661 696c 7320 6f72 2069 7320  ork fails or is 
+00014db0: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
+00014dc0: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+00014dd0: 7475 726e 2073 656c 662e 7175 6572 7928  turn self.query(
+00014de0: 2247 6c6f 6261 6c56 6f74 6554 6872 6573  "GlobalVoteThres
+00014df0: 686f 6c64 222c 290a 0a20 2020 2064 6566  hold",)..    def
+00014e00: 2067 6574 5f6d 6178 5f61 6c6c 6f77 6564   get_max_allowed
+00014e10: 5f73 7562 6e65 7473 2873 656c 6629 202d  _subnets(self) -
+00014e20: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+00014e30: 2222 0a20 2020 2020 2020 2051 7565 7269  "".        Queri
+00014e40: 6573 2074 6865 206e 6574 776f 726b 2066  es the network f
+00014e50: 6f72 2074 6865 206d 6178 696d 756d 206e  or the maximum n
+00014e60: 756d 6265 7220 6f66 2061 6c6c 6f77 6564  umber of allowed
+00014e70: 2073 7562 6e65 7473 2e0a 0a20 2020 2020   subnets...     
+00014e80: 2020 2052 6574 7269 6576 6573 2074 6865     Retrieves the
+00014e90: 2075 7070 6572 206c 696d 6974 206f 6e20   upper limit on 
+00014ea0: 7468 6520 6e75 6d62 6572 206f 6620 7375  the number of su
+00014eb0: 626e 6574 7320 7468 6174 2063 616e 200a  bnets that can .
+00014ec0: 2020 2020 2020 2020 6265 2063 7265 6174          be creat
+00014ed0: 6564 206f 7220 6f70 6572 6174 6564 2077  ed or operated w
+00014ee0: 6974 6869 6e20 7468 6520 6e65 7477 6f72  ithin the networ
+00014ef0: 6b2e 0a0a 2020 2020 2020 2020 5265 7475  k...        Retu
+00014f00: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00014f10: 2054 6865 206d 6178 696d 756d 206e 756d   The maximum num
+00014f20: 6265 7220 6f66 2061 6c6c 6f77 6564 2073  ber of allowed s
+00014f30: 7562 6e65 7473 206f 6e20 7468 6520 6e65  ubnets on the ne
+00014f40: 7477 6f72 6b2e 0a0a 2020 2020 2020 2020  twork...        
+00014f50: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00014f60: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
+00014f70: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
+00014f80: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
+00014f90: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
+00014fa0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00014fb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00014fc0: 662e 7175 6572 7928 224d 6178 416c 6c6f  f.query("MaxAllo
+00014fd0: 7765 6453 7562 6e65 7473 222c 2070 6172  wedSubnets", par
+00014fe0: 616d 733d 5b5d 2c29 0a0a 2020 2020 6465  ams=[],)..    de
+00014ff0: 6620 6765 745f 6d61 785f 616c 6c6f 7765  f get_max_allowe
+00015000: 645f 6d6f 6475 6c65 7328 7365 6c66 2920  d_modules(self) 
+00015010: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
+00015020: 2222 220a 2020 2020 2020 2020 5175 6572  """.        Quer
+00015030: 6965 7320 7468 6520 6e65 7477 6f72 6b20  ies the network 
+00015040: 666f 7220 7468 6520 6d61 7869 6d75 6d20  for the maximum 
+00015050: 6e75 6d62 6572 206f 6620 616c 6c6f 7765  number of allowe
+00015060: 6420 6d6f 6475 6c65 732e 0a0a 2020 2020  d modules...    
+00015070: 2020 2020 5265 7472 6965 7665 7320 7468      Retrieves th
+00015080: 6520 7570 7065 7220 6c69 6d69 7420 6f6e  e upper limit on
+00015090: 2074 6865 206e 756d 6265 7220 6f66 206d   the number of m
+000150a0: 6f64 756c 6573 2074 6861 7420 0a20 2020  odules that .   
+000150b0: 2020 2020 2063 616e 2062 6520 7265 6769       can be regi
+000150c0: 7374 6572 6564 2077 6974 6869 6e20 7468  stered within th
+000150d0: 6520 6e65 7477 6f72 6b2e 0a0a 2020 2020  e network...    
+000150e0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000150f0: 2020 2020 2020 2020 2054 6865 206d 6178           The max
+00015100: 696d 756d 206e 756d 6265 7220 6f66 2061  imum number of a
+00015110: 6c6c 6f77 6564 206d 6f64 756c 6573 206f  llowed modules o
+00015120: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a0a  n the network...
+00015130: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00015140: 2020 2020 2020 2020 2020 2020 5175 6572              Quer
+00015150: 7945 7272 6f72 3a20 4966 2074 6865 2071  yError: If the q
+00015160: 7565 7279 2074 6f20 7468 6520 6e65 7477  uery to the netw
+00015170: 6f72 6b20 6661 696c 7320 6f72 2069 7320  ork fails or is 
+00015180: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
+00015190: 2022 2222 0a0a 2020 2020 2020 2020 7265   """..        re
+000151a0: 7475 726e 2073 656c 662e 7175 6572 7928  turn self.query(
+000151b0: 224d 6178 416c 6c6f 7765 644d 6f64 756c  "MaxAllowedModul
+000151c0: 6573 222c 2070 6172 616d 733d 5b5d 2c29  es", params=[],)
+000151d0: 0a0a 2020 2020 6465 6620 6765 745f 6d69  ..    def get_mi
+000151e0: 6e5f 7374 616b 6528 7365 6c66 2c0a 2020  n_stake(self,.  
+000151f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015200: 2020 2020 6e65 7475 6964 3a20 696e 7420      netuid: int 
+00015210: 3d20 3029 202d 3e20 696e 743a 0a20 2020  = 0) -> int:.   
+00015220: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00015230: 2051 7565 7269 6573 2074 6865 206e 6574   Queries the net
+00015240: 776f 726b 2066 6f72 2074 6865 206d 696e  work for the min
+00015250: 696d 756d 2073 7461 6b65 2072 6571 7569  imum stake requi
+00015260: 7265 6420 746f 2072 6567 6973 7465 7220  red to register 
+00015270: 6120 6b65 792e 0a0a 2020 2020 2020 2020  a key...        
+00015280: 5265 7472 6965 7665 7320 7468 6520 6d69  Retrieves the mi
+00015290: 6e69 6d75 6d20 616d 6f75 6e74 206f 6620  nimum amount of 
+000152a0: 7374 616b 6520 6e65 6365 7373 6172 7920  stake necessary 
+000152b0: 666f 7220 0a20 2020 2020 2020 2072 6567  for .        reg
+000152c0: 6973 7465 7269 6e67 2061 206b 6579 2077  istering a key w
+000152d0: 6974 6869 6e20 6120 7370 6563 6966 6963  ithin a specific
+000152e0: 206e 6574 776f 726b 2073 7562 6e65 742e   network subnet.
+000152f0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00015300: 2020 2020 2020 2020 2020 2020 6e65 7475              netu
+00015310: 6964 3a20 5468 6520 6e65 7477 6f72 6b20  id: The network 
+00015320: 5549 4420 666f 7220 7768 6963 6820 746f  UID for which to
+00015330: 2071 7565 7279 2074 6865 206d 696e 696d   query the minim
+00015340: 756d 2073 7461 6b65 2e0a 0a20 2020 2020  um stake...     
+00015350: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00015360: 2020 2020 2020 2020 5468 6520 6d69 6e69          The mini
+00015370: 6d75 6d20 7374 616b 6520 7265 7175 6972  mum stake requir
+00015380: 6564 2066 6f72 206b 6579 2072 6567 6973  ed for key regis
+00015390: 7472 6174 696f 6e20 696e 206e 616e 6f73  tration in nanos
+000153a0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+000153b0: 733a 0a20 2020 2020 2020 2020 2020 2051  s:.            Q
+000153c0: 7565 7279 4572 726f 723a 2049 6620 7468  ueryError: If th
+000153d0: 6520 7175 6572 7920 746f 2074 6865 206e  e query to the n
+000153e0: 6574 776f 726b 2066 6169 6c73 206f 7220  etwork fails or 
+000153f0: 6973 2069 6e76 616c 6964 2e0a 2020 2020  is invalid..    
+00015400: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00015410: 2072 6574 7572 6e20 7365 6c66 2e71 7565   return self.que
+00015420: 7279 2827 4d69 6e53 7461 6b65 272c 2070  ry('MinStake', p
+00015430: 6172 616d 733d 5b6e 6574 7569 645d 290a  arams=[netuid]).
+00015440: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+00015450: 6b65 2873 656c 662c 0a20 2020 2020 2020  ke(self,.       
+00015460: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
+00015470: 5373 3538 4164 6472 6573 732c 0a20 2020  Ss58Address,.   
+00015480: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00015490: 6574 7569 643a 2069 6e74 203d 2030 2c0a  etuid: int = 0,.
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2920 2d3e 2069 6e74 3a0a 2020 2020    ) -> int:.    
+000154c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000154d0: 5175 6572 6965 7320 7468 6520 6e65 7477  Queries the netw
+000154e0: 6f72 6b20 666f 7220 7468 6520 7374 616b  ork for the stak
+000154f0: 6520 6465 6c65 6761 7465 6420 7769 7468  e delegated with
+00015500: 2061 2073 7065 6369 6669 6320 6b65 792e   a specific key.
+00015510: 0a0a 2020 2020 2020 2020 5265 7472 6965  ..        Retrie
+00015520: 7665 7320 7468 6520 616d 6f75 6e74 206f  ves the amount o
+00015530: 6620 746f 7461 6c20 7374 616b 6564 2074  f total staked t
+00015540: 6f6b 656e 7320 0a20 2020 2020 2020 2064  okens .        d
+00015550: 656c 6567 6174 6564 2061 2073 7065 6369  elegated a speci
+00015560: 6669 6320 6b65 7920 6164 6472 6573 730a  fic key address.
+00015570: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00015580: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
+00015590: 5468 6520 6164 6472 6573 7320 6f66 2074  The address of t
+000155a0: 6865 206b 6579 2074 6f20 7175 6572 7920  he key to query 
+000155b0: 7468 6520 7374 616b 6520 666f 722e 0a20  the stake for.. 
+000155c0: 2020 2020 2020 2020 2020 206e 6574 7569             netui
+000155d0: 643a 2054 6865 206e 6574 776f 726b 2055  d: The network U
+000155e0: 4944 2066 726f 6d20 7768 6963 6820 746f  ID from which to
+000155f0: 2067 6574 2074 6865 2071 7565 7279 2e0a   get the query..
+00015600: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00015610: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00015620: 6520 616d 6f75 6e74 206f 6620 7374 616b  e amount of stak
+00015630: 6520 6865 6c64 2062 7920 7468 6520 7370  e held by the sp
+00015640: 6563 6966 6965 6420 6b65 7920 696e 206e  ecified key in n
+00015650: 616e 6f73 2e0a 0a20 2020 2020 2020 2052  anos...        R
+00015660: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+00015670: 2020 2051 7565 7279 4572 726f 723a 2049     QueryError: I
+00015680: 6620 7468 6520 7175 6572 7920 746f 2074  f the query to t
+00015690: 6865 206e 6574 776f 726b 2066 6169 6c73  he network fails
+000156a0: 206f 7220 6973 2069 6e76 616c 6964 2e0a   or is invalid..
+000156b0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+000156c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000156d0: 2e71 7565 7279 2822 5374 616b 6522 2c20  .query("Stake", 
+000156e0: 7061 7261 6d73 3d5b 6e65 7475 6964 2c20  params=[netuid, 
+000156f0: 6b65 795d 2c29 0a0a 2020 2020 6465 6620  key],)..    def 
+00015700: 6765 745f 7374 616b 6566 726f 6d28 0a20  get_stakefrom(. 
+00015710: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00015720: 2020 2020 206b 6579 5f61 6464 723a 2053       key_addr: S
+00015730: 7335 3841 6464 7265 7373 2c0a 2020 2020  s58Address,.    
+00015740: 2020 2020 6e65 7475 6964 3a20 696e 7420      netuid: int 
+00015750: 3d20 302c 0a20 2020 2029 202d 3e20 6469  = 0,.    ) -> di
+00015760: 6374 5b73 7472 2c20 696e 745d 3a0a 2020  ct[str, int]:.  
+00015770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00015780: 2020 5265 7472 6965 7665 7320 6120 6c69    Retrieves a li
+00015790: 7374 206f 6620 6b65 7973 2066 726f 6d20  st of keys from 
+000157a0: 7768 6963 6820 6120 7370 6563 6966 6963  which a specific
+000157b0: 206b 6579 2061 6464 7265 7373 2069 7320   key address is 
+000157c0: 7374 616b 6564 2e0a 0a20 2020 2020 2020  staked...       
+000157d0: 2051 7565 7269 6573 2074 6865 206e 6574   Queries the net
+000157e0: 776f 726b 2066 6f72 2061 6c6c 2074 6865  work for all the
+000157f0: 2073 7461 6b65 7320 7265 6365 6976 6564   stakes received
+00015800: 2062 7920 6120 0a20 2020 2020 2020 2070   by a .        p
+00015810: 6172 7469 6375 6c61 7220 6b65 7920 6672  articular key fr
+00015820: 6f6d 2064 6966 6665 7265 6e74 2073 6f75  om different sou
+00015830: 7263 6573 2e0a 0a20 2020 2020 2020 2041  rces...        A
+00015840: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00015850: 206b 6579 5f61 6464 723a 2054 6865 2061   key_addr: The a
+00015860: 6464 7265 7373 206f 6620 7468 6520 6b65  ddress of the ke
+00015870: 7920 746f 2071 7565 7279 2073 7461 6b65  y to query stake
+00015880: 7320 6672 6f6d 2e0a 0a20 2020 2020 2020  s from...       
+00015890: 2020 2020 206e 6574 7569 643a 2054 6865       netuid: The
+000158a0: 206e 6574 776f 726b 2055 4944 2066 726f   network UID fro
+000158b0: 6d20 7768 6963 6820 746f 2067 6574 2074  m which to get t
+000158c0: 6865 2071 7565 7279 2e0a 0a20 2020 2020  he query...     
+000158d0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000158e0: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
+000158f0: 6e61 7279 206d 6170 7069 6e67 206b 6579  nary mapping key
+00015900: 2061 6464 7265 7373 6573 2074 6f20 7468   addresses to th
+00015910: 6520 616d 6f75 6e74 206f 6620 7374 616b  e amount of stak
+00015920: 6520 0a20 2020 2020 2020 2020 2020 2072  e .            r
+00015930: 6563 6569 7665 6420 6672 6f6d 2065 6163  eceived from eac
+00015940: 682e 0a0a 2020 2020 2020 2020 5261 6973  h...        Rais
+00015950: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00015960: 5175 6572 7945 7272 6f72 3a20 4966 2074  QueryError: If t
+00015970: 6865 2071 7565 7279 2074 6f20 7468 6520  he query to the 
+00015980: 6e65 7477 6f72 6b20 6661 696c 7320 6f72  network fails or
+00015990: 2069 7320 696e 7661 6c69 642e 0a20 2020   is invalid..   
+000159a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000159b0: 2072 6573 756c 7420 3d20 7365 6c66 2e71   result = self.q
+000159c0: 7565 7279 2827 5374 616b 6546 726f 6d27  uery('StakeFrom'
+000159d0: 2c20 5b6e 6574 7569 642c 206b 6579 5f61  , [netuid, key_a
+000159e0: 6464 725d 290a 0a20 2020 2020 2020 2072  ddr])..        r
+000159f0: 6574 7572 6e20 7b6b 3a20 7620 666f 7220  eturn {k: v for 
+00015a00: 6b2c 2076 2069 6e20 7265 7375 6c74 7d0a  k, v in result}.
+00015a10: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+00015a20: 6b65 746f 280a 2020 2020 2020 2020 7365  keto(.        se
+00015a30: 6c66 2c0a 2020 2020 2020 2020 6b65 795f  lf,.        key_
+00015a40: 6164 6472 3a20 5373 3538 4164 6472 6573  addr: Ss58Addres
+00015a50: 732c 0a20 2020 2020 2020 206e 6574 7569  s,.        netui
+00015a60: 643a 2069 6e74 203d 2030 2c0a 2020 2020  d: int = 0,.    
+00015a70: 2920 2d3e 2064 6963 745b 7374 722c 2069  ) -> dict[str, i
+00015a80: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
+00015a90: 0a20 2020 2020 2020 2052 6574 7269 6576  .        Retriev
+00015aa0: 6573 2061 206c 6973 7420 6f66 206b 6579  es a list of key
+00015ab0: 7320 746f 2077 6869 6368 2061 2073 7065  s to which a spe
+00015ac0: 6369 6669 6320 6b65 7920 6164 6472 6573  cific key addres
+00015ad0: 7320 7374 616b 6573 2074 6f2e 0a0a 2020  s stakes to...  
+00015ae0: 2020 2020 2020 5175 6572 6965 7320 7468        Queries th
+00015af0: 6520 6e65 7477 6f72 6b20 666f 7220 616c  e network for al
+00015b00: 6c20 7468 6520 7374 616b 6573 206d 6164  l the stakes mad
+00015b10: 6520 6279 2061 2070 6172 7469 6375 6c61  e by a particula
+00015b20: 7220 6b65 7920 746f 200a 2020 2020 2020  r key to .      
+00015b30: 2020 6469 6666 6572 656e 7420 6465 7374    different dest
+00015b40: 696e 6174 696f 6e73 2e0a 0a20 2020 2020  inations...     
+00015b50: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00015b60: 2020 2020 206b 6579 5f61 6464 723a 2054       key_addr: T
+00015b70: 6865 2061 6464 7265 7373 206f 6620 7468  he address of th
+00015b80: 6520 6b65 7920 746f 2071 7565 7279 2073  e key to query s
+00015b90: 7461 6b65 7320 746f 2e0a 0a20 2020 2020  takes to...     
+00015ba0: 2020 2020 2020 206e 6574 7569 643a 2054         netuid: T
+00015bb0: 6865 206e 6574 776f 726b 2055 4944 2066  he network UID f
+00015bc0: 726f 6d20 7768 6963 6820 746f 2067 6574  rom which to get
+00015bd0: 2074 6865 2071 7565 7279 2e0a 0a20 2020   the query...   
+00015be0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00015bf0: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
+00015c00: 696f 6e61 7279 206d 6170 7069 6e67 206b  ionary mapping k
+00015c10: 6579 2061 6464 7265 7373 6573 2074 6f20  ey addresses to 
+00015c20: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
+00015c30: 2061 6d6f 756e 7420 6f66 2073 7461 6b65   amount of stake
+00015c40: 2067 6976 656e 2074 6f20 6561 6368 2e0a   given to each..
+00015c50: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+00015c60: 0a20 2020 2020 2020 2020 2020 2051 7565  .            Que
+00015c70: 7279 4572 726f 723a 2049 6620 7468 6520  ryError: If the 
+00015c80: 7175 6572 7920 746f 2074 6865 206e 6574  query to the net
+00015c90: 776f 726b 2066 6169 6c73 206f 7220 6973  work fails or is
+00015ca0: 2069 6e76 616c 6964 2e0a 2020 2020 2020   invalid..      
+00015cb0: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
+00015cc0: 6573 756c 7420 3d20 7365 6c66 2e71 7565  esult = self.que
+00015cd0: 7279 2827 5374 616b 6554 6f27 2c20 5b6e  ry('StakeTo', [n
+00015ce0: 6574 7569 642c 206b 6579 5f61 6464 725d  etuid, key_addr]
+00015cf0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00015d00: 6e20 7b6b 3a20 7620 666f 7220 6b2c 2076  n {k: v for k, v
+00015d10: 2069 6e20 7265 7375 6c74 7d0a 0a20 2020   in result}..   
+00015d20: 2064 6566 2067 6574 5f62 616c 616e 6365   def get_balance
+00015d30: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00015d40: 2020 2020 2020 2020 6164 6472 3a20 5373          addr: Ss
+00015d50: 3538 4164 6472 6573 732c 0a20 2020 2029  58Address,.    )
+00015d60: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00015d70: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00015d80: 7269 6576 6573 2074 6865 2062 616c 616e  rieves the balan
+00015d90: 6365 206f 6620 6120 7370 6563 6966 6963  ce of a specific
+00015da0: 206b 6579 2e0a 0a20 2020 2020 2020 2041   key...        A
+00015db0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00015dc0: 2061 6464 723a 2054 6865 2061 6464 7265   addr: The addre
+00015dd0: 7373 206f 6620 7468 6520 6b65 7920 746f  ss of the key to
+00015de0: 2071 7565 7279 2074 6865 2062 616c 616e   query the balan
+00015df0: 6365 2066 6f72 2e0a 0a20 2020 2020 2020  ce for...       
+00015e00: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00015e10: 2020 2020 2020 5468 6520 6261 6c61 6e63        The balanc
+00015e20: 6520 6f66 2074 6865 2073 7065 6369 6669  e of the specifi
+00015e30: 6564 206b 6579 2e0a 0a20 2020 2020 2020  ed key...       
+00015e40: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00015e50: 2020 2020 2051 7565 7279 4572 726f 723a       QueryError:
+00015e60: 2049 6620 7468 6520 7175 6572 7920 746f   If the query to
+00015e70: 2074 6865 206e 6574 776f 726b 2066 6169   the network fai
+00015e80: 6c73 206f 7220 6973 2069 6e76 616c 6964  ls or is invalid
+00015e90: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00015ea0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00015eb0: 7365 6c66 2e71 7565 7279 2827 4163 636f  self.query('Acco
+00015ec0: 756e 7427 2c20 6d6f 6475 6c65 3d27 5379  unt', module='Sy
+00015ed0: 7374 656d 272c 2070 6172 616d 733d 5b61  stem', params=[a
+00015ee0: 6464 725d 290a 0a20 2020 2020 2020 2072  ddr])..        r
+00015ef0: 6574 7572 6e20 7265 7375 6c74 5b22 6461  eturn result["da
+00015f00: 7461 225d 5b22 6672 6565 225d 0a0a 2020  ta"]["free"]..  
+00015f10: 2020 6465 6620 6765 745f 626c 6f63 6b28    def get_block(
+00015f20: 7365 6c66 2c20 626c 6f63 6b5f 6861 7368  self, block_hash
+00015f30: 3a20 7374 7220 7c20 4e6f 6e65 203d 204e  : str | None = N
+00015f40: 6f6e 6529 202d 3e20 6469 6374 5b41 6e79  one) -> dict[Any
+00015f50: 2c20 416e 795d 207c 204e 6f6e 653a 0a20  , Any] | None:. 
+00015f60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00015f70: 2020 2052 6574 7269 6576 6573 2069 6e66     Retrieves inf
+00015f80: 6f72 6d61 7469 6f6e 2061 626f 7574 2061  ormation about a
+00015f90: 2073 7065 6369 6669 6320 626c 6f63 6b20   specific block 
+00015fa0: 696e 2074 6865 206e 6574 776f 726b 2e0a  in the network..
+00015fb0: 0a20 2020 2020 2020 2051 7565 7269 6573  .        Queries
+00015fc0: 2074 6865 206e 6574 776f 726b 2066 6f72   the network for
+00015fd0: 2064 6574 6169 6c73 2061 626f 7574 2061   details about a
+00015fe0: 2062 6c6f 636b 2c20 7375 6368 2061 7320   block, such as 
+00015ff0: 6974 7320 6e75 6d62 6572 2c20 0a20 2020  its number, .   
+00016000: 2020 2020 2068 6173 682c 2061 6e64 206f       hash, and o
+00016010: 7468 6572 2072 656c 6576 616e 7420 696e  ther relevant in
+00016020: 666f 726d 6174 696f 6e2e 0a0a 2020 2020  formation...    
+00016030: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00016040: 2020 2020 2020 2020 2054 6865 2072 6571           The req
+00016050: 7565 7374 6564 2069 6e66 6f72 6d61 7469  uested informati
+00016060: 6f6e 2061 626f 7574 2074 6865 2062 6c6f  on about the blo
+00016070: 636b 2c20 0a20 2020 2020 2020 2020 2020  ck, .           
+00016080: 206f 7220 4e6f 6e65 2069 6620 7468 6520   or None if the 
+00016090: 626c 6f63 6b20 646f 6573 206e 6f74 2065  block does not e
+000160a0: 7869 7374 200a 2020 2020 2020 2020 2020  xist .          
+000160b0: 2020 6f72 2074 6865 2069 6e66 6f72 6d61    or the informa
+000160c0: 7469 6f6e 2069 7320 6e6f 7420 6176 6169  tion is not avai
+000160d0: 6c61 626c 652e 0a0a 2020 2020 2020 2020  lable...        
+000160e0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+000160f0: 2020 2020 5175 6572 7945 7272 6f72 3a20      QueryError: 
+00016100: 4966 2074 6865 2071 7565 7279 2074 6f20  If the query to 
+00016110: 7468 6520 6e65 7477 6f72 6b20 6661 696c  the network fail
+00016120: 7320 6f72 2069 7320 696e 7661 6c69 642e  s or is invalid.
+00016130: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00016140: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
+00016150: 6765 745f 636f 6e6e 2829 2061 7320 7375  get_conn() as su
+00016160: 6273 7472 6174 653a 0a20 2020 2020 2020  bstrate:.       
+00016170: 2020 2020 2062 6c6f 636b 3a20 6469 6374       block: dict
+00016180: 5b41 6e79 2c20 416e 795d 207c 204e 6f6e  [Any, Any] | Non
+00016190: 6520 3d20 7375 6273 7472 6174 652e 6765  e = substrate.ge
+000161a0: 745f 626c 6f63 6b28 2020 2320 7479 7065  t_block(  # type
+000161b0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+000161c0: 2020 2020 2020 2020 2062 6c6f 636b 5f68           block_h
+000161d0: 6173 6820 2023 2074 7970 653a 2069 676e  ash  # type: ign
+000161e0: 6f72 650a 2020 2020 2020 2020 2020 2020  ore.            
+000161f0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00016200: 6e20 626c 6f63 6b0a 0a20 2020 2064 6566  n block..    def
+00016210: 2067 6574 5f65 7869 7374 656e 7469 616c   get_existential
+00016220: 5f64 6570 6f73 6974 2873 656c 662c 2062  _deposit(self, b
+00016230: 6c6f 636b 5f68 6173 683a 2073 7472 207c  lock_hash: str |
+00016240: 204e 6f6e 6520 3d20 4e6f 6e65 2920 2d3e   None = None) ->
+00016250: 2069 6e74 3a0a 2020 2020 2020 2020 2222   int:.        ""
+00016260: 220a 2020 2020 2020 2020 5265 7472 6965  ".        Retrie
+00016270: 7665 7320 7468 6520 6578 6973 7465 6e74  ves the existent
+00016280: 6961 6c20 6465 706f 7369 7420 7661 6c75  ial deposit valu
+00016290: 6520 666f 7220 7468 6520 6e65 7477 6f72  e for the networ
+000162a0: 6b2e 0a0a 2020 2020 2020 2020 5468 6520  k...        The 
+000162b0: 6578 6973 7465 6e74 6961 6c20 6465 706f  existential depo
+000162c0: 7369 7420 6973 2074 6865 206d 696e 696d  sit is the minim
+000162d0: 756d 2062 616c 616e 6365 2074 6861 7420  um balance that 
+000162e0: 6d75 7374 2062 6520 6d61 696e 7461 696e  must be maintain
+000162f0: 6564 200a 2020 2020 2020 2020 696e 2061  ed .        in a
+00016300: 6e20 6163 636f 756e 7420 746f 2070 7265  n account to pre
+00016310: 7665 6e74 2069 7420 6672 6f6d 2062 6569  vent it from bei
+00016320: 6e67 2070 7572 6765 642e 2044 656e 6f74  ng purged. Denot
+00016330: 6174 6564 2069 6e20 6e61 6e6f 2075 6e69  ated in nano uni
+00016340: 7473 2e0a 0a20 2020 2020 2020 2052 6574  ts...        Ret
+00016350: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00016360: 2020 5468 6520 6578 6973 7465 6e74 6961    The existentia
+00016370: 6c20 6465 706f 7369 7420 7661 6c75 6520  l deposit value 
+00016380: 696e 206e 616e 6f20 756e 6974 732e 200a  in nano units. .
+00016390: 2020 2020 2020 2020 4e6f 7465 3a0a 2020          Note:.  
+000163a0: 2020 2020 2020 2020 2020 5468 6520 7661            The va
+000163b0: 6c75 6520 7265 7475 726e 6564 2069 7320  lue returned is 
+000163c0: 6120 6669 7865 6420 7661 6c75 6520 6465  a fixed value de
+000163d0: 6669 6e65 6420 696e 2074 6865 200a 2020  fined in the .  
+000163e0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000163f0: 2061 6e64 206d 6179 206e 6f74 2072 6566   and may not ref
+00016400: 6c65 6374 2063 6861 6e67 6573 2069 6e20  lect changes in 
+00016410: 7468 6520 6e65 7477 6f72 6b27 7320 636f  the network's co
+00016420: 6e66 6967 7572 6174 696f 6e2e 0a20 2020  nfiguration..   
+00016430: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00016440: 2020 7769 7468 2073 656c 662e 6765 745f    with self.get_
+00016450: 636f 6e6e 2829 2061 7320 7375 6273 7472  conn() as substr
+00016460: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00016470: 2072 6573 756c 743a 2069 6e74 203d 2073   result: int = s
+00016480: 7562 7374 7261 7465 2e67 6574 5f63 6f6e  ubstrate.get_con
+00016490: 7374 616e 7428 2020 2320 c2a0 7479 7065  stant(  # ..type
+000164a0: 3a20 6967 6e6f 7265 0a20 2020 2020 2020  : ignore.       
+000164b0: 2020 2020 2020 2020 2022 4261 6c61 6e63           "Balanc
+000164c0: 6573 222c 2022 4578 6973 7465 6e74 6961  es", "Existentia
+000164d0: 6c44 6570 6f73 6974 222c 2062 6c6f 636b  lDeposit", block
+000164e0: 5f68 6173 6829 2e76 616c 7565 2020 2320  _hash).value  # 
+000164f0: c2a0 7479 7065 3a20 6967 6e6f 7265 0a0a  ..type: ignore..
+00016500: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00016510: 6573 756c 740a                           esult.
```

### Comparing `communex-0.1.6/src/communex/compat/_util.py` & `communex-0.1.7/src/communex/compat/_util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/compat/key.py` & `communex-0.1.7/src/communex/compat/key.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,18 @@
     key_dir = home / '.commune' / "key"
 
     key_names = [f.stem for f in key_dir.iterdir() if f.is_file()]
 
     addresses_map: dict[str, Ss58Address] = {}
 
     for key_name in key_names:
+        # issue #11 https://github.com/agicommies/communex/issues/12 added check for key2address to stop error from being thrown by wrong key type. 
+        if key_name == "key2address": 
+            print("key2address is saved in an invalid format. It will be ignored.")
+            continue
         key_dict = classic_load_key(key_name)
         addresses_map[key_name] = check_ss58_address(key_dict.ss58_address)
 
     return addresses_map
 
 
 def resolve_key_ss58(key: Ss58Address | Keypair | str) -> Ss58Address:
```

### Comparing `communex-0.1.6/src/communex/compat/storage.py` & `communex-0.1.7/src/communex/compat/storage.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/key.py` & `communex-0.1.7/src/communex/key.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/misc.py` & `communex-0.1.7/src/communex/misc.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/_ip_limiter.py` & `communex-0.1.7/src/communex/module/_ip_limiter.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/_signer.py` & `communex-0.1.7/src/communex/module/_signer.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/client.py` & `communex-0.1.7/src/communex/module/client.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/example/gpt.py` & `communex-0.1.7/src/communex/module/example/gpt.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,48 +6,50 @@
 from openai import OpenAI
 
 from communex.module.module import Module, endpoint
 from communex.module.server import ModuleServer
 
 OPENAI_API_KEY = getenv("OPENAI_API_KEY")
 
+
 class OpenAIModels(str, Enum):
     three = "gpt-3.5-turbo"
 
 
 class OpenAIModule(Module):
     def __init__(self) -> None:
         super().__init__()
         self.client = OpenAI(api_key=OPENAI_API_KEY)
 
-
     @endpoint
     def prompt(self, text: str, model: OpenAIModels):
         response = self.client.chat.completions.create(
             model=model,
-            response_format = {"type": "json_object"},
-            messages= [
+            response_format={"type": "json_object"},
+            messages=[
                 {"role": "system", "content": "You are a helpful assistant designed to output JSON."},
-                {"role": "user", "content": text}
-            ]
+                {"role": "user", "content": text},
+            ],
         )
         answers: list[dict[str, str]] = []
         for msg in response.choices:
             finish_reason = msg.finish_reason
             if finish_reason != "stop":
                 raise HTTPException(418, finish_reason)
             content = msg.message.content
             if content:
                 answers.append(json.loads(content))
 
         return {"Answer": answers}
 
 
-
 if __name__ == "__main__":
     import uvicorn
 
+    from communex.compat.key import classic_load_key
+
     model = OpenAIModule()
-    model_server = ModuleServer(model)
+    key = classic_load_key("test")
+    model_server = ModuleServer(model, key)
     app = model_server.get_fastapi_app()
 
-    uvicorn.run(app, host="127.0.0.1", port=8000) #type: ignore
+    uvicorn.run(app, host="127.0.0.1", port=8000)  # type: ignore
```

### Comparing `communex-0.1.6/src/communex/module/example/openai.py` & `communex-0.1.7/src/communex/module/example/openai.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/module.py` & `communex-0.1.7/src/communex/module/module.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/module/server.py` & `communex-0.1.7/src/communex/module/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from fastapi.responses import JSONResponse
 from fastapi.routing import APIRoute
 from keylimiter import KeyLimiter
 from pydantic import BaseModel
 from scalecodec.utils.ss58 import ss58_encode  # type: ignore
 from substrateinterface import Keypair  # type: ignore
 
-from communex.cli._common import make_client
+from communex._common import make_client
 from communex.key import check_ss58_address
 from communex.module import _signer as signer
 from communex.module._ip_limiter import IpLimiterMiddleware
 from communex.module.module import Module, endpoint
 
 # Regular expression to match a hexadecimal number
 HEX_PATTERN = re.compile(r"^[0-9a-fA-F]+$")
@@ -39,24 +39,24 @@
 
 def build_input_handler_route_class(subnets_whitelist: list[int] | None) -> type[APIRoute]:
     class InputHandlerRoute(APIRoute):
         def get_route_handler(self):
             original_route_handler = super().get_route_handler()
 
             async def custom_route_handler(request: Request) -> Response:
-                response: Response = await original_route_handler(request)
                 body = await request.body()
 
                 # TODO: we'll replace this by a Result ADT :)
                 match self._check_inputs(request, body):
                     case (False, error):
                         return error
                     case (True, _):
                         pass
 
+                response: Response = await original_route_handler(request)
                 return response
 
             return custom_route_handler
 
         @staticmethod
         def _check_inputs(request: Request, body: bytes):
             required_headers = ["x-signature", "x-key", "x-crypto"]
```

### Comparing `communex-0.1.6/src/communex/types.py` & `communex-0.1.7/src/communex/types.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/src/communex/util.py` & `communex-0.1.7/src/communex/util.py`

 * *Files identical despite different names*

### Comparing `communex-0.1.6/PKG-INFO` & `communex-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communex
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for Commune network focused on simplicity
 License: MIT
 Author: agicommies
 Author-email: info@agicommies.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: keylimiter (>=0.1.5,<0.2.0)
 Requires-Dist: py-sr25519-bindings (>=0.2.0,<0.3.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: scalecodec (>=1.2.7,<2.0.0)
 Requires-Dist: starlette (>=0.36.3,<0.37.0)
 Requires-Dist: substrate-interface (>=1.7.4,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
```

