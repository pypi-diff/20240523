# Comparing `tmp/hyperliquid_python_sdk-0.3.0.tar.gz` & `tmp/hyperliquid_python_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperliquid_python_sdk-0.3.0.tar", max compression
+gzip compressed data, was "hyperliquid_python_sdk-0.4.0.tar", max compression
```

## Comparing `hyperliquid_python_sdk-0.3.0.tar` & `hyperliquid_python_sdk-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-12-01 20:12:00.320554 hyperliquid_python_sdk-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     5741 2023-12-01 20:12:00.320814 hyperliquid_python_sdk-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 03:52:57.369329 hyperliquid_python_sdk-0.3.0/hyperliquid/__init__.py
--rw-r--r--   0        0        0     1677 2024-03-29 03:52:57.380100 hyperliquid_python_sdk-0.3.0/hyperliquid/api.py
--rw-r--r--   0        0        0    15943 2024-03-29 03:52:57.369193 hyperliquid_python_sdk-0.3.0/hyperliquid/exchange.py
--rw-r--r--   0        0        0    11036 2024-03-29 03:52:57.380331 hyperliquid_python_sdk-0.3.0/hyperliquid/info.py
--rw-r--r--   0        0        0        0 2024-03-29 03:52:57.370610 hyperliquid_python_sdk-0.3.0/hyperliquid/utils/__init__.py
--rw-r--r--   0        0        0      144 2024-03-29 03:52:57.370497 hyperliquid_python_sdk-0.3.0/hyperliquid/utils/constants.py
--rw-r--r--   0        0        0      479 2024-03-29 03:52:57.370282 hyperliquid_python_sdk-0.3.0/hyperliquid/utils/error.py
--rw-r--r--   0        0        0     8432 2024-03-29 03:52:57.369968 hyperliquid_python_sdk-0.3.0/hyperliquid/utils/signing.py
--rw-r--r--   0        0        0     3168 2024-03-29 03:52:57.370870 hyperliquid_python_sdk-0.3.0/hyperliquid/utils/types.py
--rw-r--r--   0        0        0     5150 2024-03-29 03:52:57.380525 hyperliquid_python_sdk-0.3.0/hyperliquid/websocket_manager.py
--rw-r--r--   0        0        0     3738 2024-03-29 03:53:28.299118 hyperliquid_python_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7019 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-23 03:24:02.690668 hyperliquid_python_sdk-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     5741 2024-05-23 03:24:02.706946 hyperliquid_python_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 03:24:02.683451 hyperliquid_python_sdk-0.4.0/hyperliquid/__init__.py
+-rw-r--r--   0        0        0     1563 2024-05-23 03:24:02.689765 hyperliquid_python_sdk-0.4.0/hyperliquid/api.py
+-rw-r--r--   0        0        0    15174 2024-05-23 03:24:02.683176 hyperliquid_python_sdk-0.4.0/hyperliquid/exchange.py
+-rw-r--r--   0        0        0    12629 2024-05-23 03:24:02.690074 hyperliquid_python_sdk-0.4.0/hyperliquid/info.py
+-rw-r--r--   0        0        0        0 2024-05-23 03:24:02.684925 hyperliquid_python_sdk-0.4.0/hyperliquid/utils/__init__.py
+-rw-r--r--   0        0        0      144 2024-05-23 03:24:02.684803 hyperliquid_python_sdk-0.4.0/hyperliquid/utils/constants.py
+-rw-r--r--   0        0        0      479 2024-05-23 03:24:02.684383 hyperliquid_python_sdk-0.4.0/hyperliquid/utils/error.py
+-rw-r--r--   0        0        0     7904 2024-05-23 03:24:02.683972 hyperliquid_python_sdk-0.4.0/hyperliquid/utils/signing.py
+-rw-r--r--   0        0        0     3168 2024-05-23 03:24:02.685206 hyperliquid_python_sdk-0.4.0/hyperliquid/utils/types.py
+-rw-r--r--   0        0        0     5152 2024-05-23 03:24:02.690378 hyperliquid_python_sdk-0.4.0/hyperliquid/websocket_manager.py
+-rw-r--r--   0        0        0     3738 2024-05-23 03:29:22.483210 hyperliquid_python_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7166 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.4.0/PKG-INFO
```

### Comparing `hyperliquid_python_sdk-0.3.0/LICENSE.md` & `hyperliquid_python_sdk-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.3.0/README.md` & `hyperliquid_python_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/api.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,52 +6,37 @@
 
 from hyperliquid.utils.constants import MAINNET_API_URL
 from hyperliquid.utils.error import ClientError, ServerError
 from hyperliquid.utils.types import Any
 
 
 class API:
-    def __init__(
-        self,
-        base_url=None,
-    ):
-        self.base_url = MAINNET_API_URL
+    def __init__(self, base_url=None):
+        self.base_url = base_url or MAINNET_API_URL
         self.session = requests.Session()
-        self.session.headers.update(
-            {
-                "Content-Type": "application/json",
-            }
-        )
-
-        if base_url is not None:
-            self.base_url = base_url
-
+        self.session.headers.update({"Content-Type": "application/json"})
         self._logger = logging.getLogger(__name__)
-        return
 
     def post(self, url_path: str, payload: Any = None) -> Any:
-        if payload is None:
-            payload = {}
+        payload = payload or {}
         url = self.base_url + url_path
-
         response = self.session.post(url, json=payload)
         self._handle_exception(response)
-
         try:
             return response.json()
         except ValueError:
             return {"error": f"Could not parse JSON: {response.text}"}
 
     def _handle_exception(self, response):
         status_code = response.status_code
         if status_code < 400:
             return
         if 400 <= status_code < 500:
             try:
                 err = json.loads(response.text)
             except JSONDecodeError:
                 raise ClientError(status_code, None, response.text, None, response.headers)
-            error_data = None
-            if "data" in err:
-                error_data = err["data"]
+            if err is None:
+                raise ClientError(status_code, None, response.text, None, response.headers)
+            error_data = err.get("data")
             raise ClientError(status_code, err["code"], err["msg"], response.headers, error_data)
         raise ServerError(status_code, response.text)
```

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/exchange.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import eth_account
 import logging
 import secrets
 
-from eth_abi import encode
 from eth_account.signers.local import LocalAccount
-from eth_utils import keccak, to_hex
 
 from hyperliquid.api import API
 from hyperliquid.info import Info
 from hyperliquid.utils.constants import MAINNET_API_URL
 from hyperliquid.utils.signing import (
     CancelRequest,
     CancelByCloidRequest,
     ModifyRequest,
     OrderRequest,
     OrderType,
     OrderWire,
+    OidOrCloid,
     ScheduleCancelAction,
     float_to_usd_int,
     get_timestamp_ms,
     order_request_to_order_wire,
     order_wires_to_order_action,
     sign_l1_action,
     sign_usd_transfer_action,
     sign_withdraw_from_bridge_action,
     sign_agent,
 )
 from hyperliquid.utils.types import Any, List, Meta, SpotMeta, Optional, Tuple, Cloid
 
 
 class Exchange(API):
-
     # Default Max Slippage for Market Orders 5%
     DEFAULT_SLIPPAGE = 0.05
 
     def __init__(
         self,
         wallet: LocalAccount,
         base_url: Optional[str] = None,
@@ -77,15 +75,14 @@
     def _slippage_price(
         self,
         coin: str,
         is_buy: bool,
         slippage: float,
         px: Optional[float] = None,
     ) -> float:
-
         if not px:
             # Get midprice
             px = float(self.info.all_mids()[coin])
         # Calculate Slippage
         px *= (1 + slippage) if is_buy else (1 - slippage)
         # We round px to 5 significant figures and 6 decimals
         return round(float(f"{px:.5g}"), 6)
@@ -132,24 +129,23 @@
             order_action,
             signature,
             timestamp,
         )
 
     def modify_order(
         self,
-        oid: int,
+        oid: OidOrCloid,
         coin: str,
         is_buy: bool,
         sz: float,
         limit_px: float,
         order_type: OrderType,
         reduce_only: bool = False,
         cloid: Optional[Cloid] = None,
     ) -> Any:
-
         modify: ModifyRequest = {
             "oid": oid,
             "order": {
                 "coin": coin,
                 "is_buy": is_buy,
                 "sz": sz,
                 "limit_px": limit_px,
@@ -160,15 +156,15 @@
         }
         return self.bulk_modify_orders_new([modify])
 
     def bulk_modify_orders_new(self, modify_requests: List[ModifyRequest]) -> Any:
         timestamp = get_timestamp_ms()
         modify_wires = [
             {
-                "oid": modify["oid"],
+                "oid": modify["oid"].to_raw() if isinstance(modify["oid"], Cloid) else modify["oid"],
                 "order": order_request_to_order_wire(modify["order"], self.coin_to_asset[modify["order"]["coin"]]),
             }
             for modify in modify_requests
         ]
 
         modify_action = {
             "type": "batchModify",
@@ -194,15 +190,14 @@
         coin: str,
         is_buy: bool,
         sz: float,
         px: Optional[float] = None,
         slippage: float = DEFAULT_SLIPPAGE,
         cloid: Optional[Cloid] = None,
     ) -> Any:
-
         # Get aggressive Market Price
         px = self._slippage_price(coin, is_buy, slippage, px)
         # Market Order is an aggressive Limit Order IoC
         return self.order(coin, is_buy, sz, px, order_type={"limit": {"tif": "Ioc"}}, reduce_only=False, cloid=cloid)
 
     def market_close(
         self,
@@ -442,73 +437,49 @@
             sub_account_transfer_action,
             signature,
             timestamp,
         )
 
     def usd_transfer(self, amount: float, destination: str) -> Any:
         timestamp = get_timestamp_ms()
-        payload = {
-            "destination": destination,
-            "amount": str(amount),
-            "time": timestamp,
-        }
+        action = {"destination": destination, "amount": str(amount), "time": timestamp, "type": "usdSend"}
         is_mainnet = self.base_url == MAINNET_API_URL
-        signature = sign_usd_transfer_action(self.wallet, payload, is_mainnet)
+        signature = sign_usd_transfer_action(self.wallet, action, is_mainnet)
         return self._post_action(
-            {
-                "chain": "Arbitrum" if is_mainnet else "ArbitrumTestnet",
-                "payload": payload,
-                "type": "usdTransfer",
-            },
+            action,
             signature,
             timestamp,
         )
 
-    def withdraw_from_bridge(self, usd: float, destination: str) -> Any:
+    def withdraw_from_bridge(self, amount: float, destination: str) -> Any:
         timestamp = get_timestamp_ms()
-        payload = {
-            "destination": destination,
-            "usd": str(usd),
-            "time": timestamp,
-        }
+        action = {"destination": destination, "amount": str(amount), "time": timestamp, "type": "withdraw3"}
         is_mainnet = self.base_url == MAINNET_API_URL
-        signature = sign_withdraw_from_bridge_action(self.wallet, payload, is_mainnet)
+        signature = sign_withdraw_from_bridge_action(self.wallet, action, is_mainnet)
         return self._post_action(
-            {
-                "chain": "Arbitrum" if is_mainnet else "ArbitrumTestnet",
-                "payload": payload,
-                "type": "withdraw2",
-            },
+            action,
             signature,
             timestamp,
         )
 
     def approve_agent(self, name: Optional[str] = None) -> Tuple[Any, str]:
         agent_key = "0x" + secrets.token_hex(32)
         account = eth_account.Account.from_key(agent_key)
-        if name is not None:
-            connection_id = keccak(encode(["address", "string"], [account.address, name]))
-        else:
-            connection_id = keccak(encode(["address"], [account.address]))
-        agent = {
-            "source": "https://hyperliquid.xyz",
-            "connectionId": connection_id,
-        }
         timestamp = get_timestamp_ms()
         is_mainnet = self.base_url == MAINNET_API_URL
-        signature = sign_agent(self.wallet, agent, is_mainnet)
-        agent["connectionId"] = to_hex(agent["connectionId"])
         action = {
-            "chain": "Arbitrum" if is_mainnet else "ArbitrumTestnet",
-            "agent": agent,
+            "type": "approveAgent",
             "agentAddress": account.address,
-            "type": "connect",
+            "agentName": name or "",
+            "nonce": timestamp,
         }
-        if name is not None:
-            action["extraAgentName"] = name
+        signature = sign_agent(self.wallet, action, is_mainnet)
+        if name is None:
+            del action["agentName"]
+
         return (
             self._post_action(
                 action,
                 signature,
                 timestamp,
             ),
             agent_key,
```

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/info.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,14 +297,57 @@
                 },
                 ...
             ]
         """
         req = {"coin": coin, "interval": interval, "startTime": startTime, "endTime": endTime}
         return self.post("/info", {"type": "candleSnapshot", "req": req})
 
+    def user_fees(self, address: str) -> Any:
+        """Retrieve the volume of trading activity associated with a user.
+        POST /info
+        Args:
+            address (str): Onchain address in 42-character hexadecimal format;
+                            e.g. 0x0000000000000000000000000000000000000000.
+        Returns:
+            {
+                activeReferralDiscount: float string,
+                dailyUserVlm: [
+                    {
+                        date: str,
+                        exchange: str,
+                        userAdd: float string,
+                        userCross: float string
+                    },
+                ],
+                feeSchedule: {
+                    add: float string,
+                    cross: float string,
+                    referralDiscount: float string,
+                    tiers: {
+                        mm: [
+                            {
+                                add: float string,
+                                makerFractionCutoff: float string
+                            },
+                        ],
+                        vip: [
+                            {
+                                add: float string,
+                                cross: float string,
+                                ntlCutoff: float string
+                            },
+                        ]
+                    }
+                },
+                userAddRate: float string,
+                userCrossRate: float string
+            }
+        """
+        return self.post("/info", {"type": "userFees", "user": address})
+
     def query_order_by_oid(self, user: str, oid: int) -> Any:
         return self.post("/info", {"type": "orderStatus", "user": user, "oid": oid})
 
     def query_order_by_cloid(self, user: str, cloid: Cloid) -> Any:
         return self.post("/info", {"type": "orderStatus", "user": user, "oid": cloid.to_raw()})
 
     def query_referral_state(self, user: str) -> Any:
```

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/utils/signing.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/utils/signing.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,18 +23,19 @@
         "limit_px": float,
         "order_type": OrderType,
         "reduce_only": bool,
         "cloid": NotRequired[Optional[Cloid]],
     },
     total=False,
 )
+OidOrCloid = Union[int, Cloid]
 ModifyRequest = TypedDict(
     "ModifyRequest",
     {
-        "oid": int,
+        "oid": OidOrCloid,
         "order": OrderRequest,
     },
     total=False,
 )
 CancelRequest = TypedDict("CancelRequest", {"coin": str, "oid": int})
 CancelByCloidRequest = TypedDict("CancelByCloidRequest", {"coin": str, "cloid": Cloid})
 
@@ -131,92 +132,82 @@
         },
         "primaryType": "Agent",
         "message": phantom_agent,
     }
     return sign_inner(wallet, data)
 
 
-def sign_usd_transfer_action(wallet, message, is_mainnet):
-    data = {
-        "domain": {
-            "name": "Exchange",
-            "version": "1",
-            "chainId": 42161 if is_mainnet else 421614,
-            "verifyingContract": "0x0000000000000000000000000000000000000000",
-        },
-        "types": {
-            "UsdTransferSignPayload": [
-                {"name": "destination", "type": "string"},
-                {"name": "amount", "type": "string"},
-                {"name": "time", "type": "uint64"},
-            ],
-            "EIP712Domain": [
-                {"name": "name", "type": "string"},
-                {"name": "version", "type": "string"},
-                {"name": "chainId", "type": "uint256"},
-                {"name": "verifyingContract", "type": "address"},
-            ],
-        },
-        "primaryType": "UsdTransferSignPayload",
-        "message": message,
-    }
-    return sign_inner(wallet, data)
-
-
-def sign_withdraw_from_bridge_action(wallet, message, is_mainnet):
+def sign_user_signed_action(wallet, action, payload_types, primary_type, is_mainnet):
+    action["signatureChainId"] = "0x66eee"
+    action["hyperliquidChain"] = "Mainnet" if is_mainnet else "Testnet"
     data = {
         "domain": {
-            "name": "Exchange",
+            "name": "HyperliquidSignTransaction",
             "version": "1",
-            "chainId": 42161 if is_mainnet else 421614,
+            "chainId": 421614,
             "verifyingContract": "0x0000000000000000000000000000000000000000",
         },
         "types": {
-            "WithdrawFromBridge2SignPayload": [
-                {"name": "destination", "type": "string"},
-                {"name": "usd", "type": "string"},
-                {"name": "time", "type": "uint64"},
-            ],
+            primary_type: payload_types,
             "EIP712Domain": [
                 {"name": "name", "type": "string"},
                 {"name": "version", "type": "string"},
                 {"name": "chainId", "type": "uint256"},
                 {"name": "verifyingContract", "type": "address"},
             ],
         },
-        "primaryType": "WithdrawFromBridge2SignPayload",
-        "message": message,
+        "primaryType": primary_type,
+        "message": action,
     }
     return sign_inner(wallet, data)
 
 
-def sign_agent(wallet, agent, is_mainnet):
-    data = {
-        "domain": {
-            "name": "Exchange",
-            "version": "1",
-            "chainId": 42161 if is_mainnet else 421614,
-            "verifyingContract": "0x0000000000000000000000000000000000000000",
-        },
-        "types": {
-            "Agent": [
-                {"name": "source", "type": "string"},
-                {"name": "connectionId", "type": "bytes32"},
-            ],
-            "EIP712Domain": [
-                {"name": "name", "type": "string"},
-                {"name": "version", "type": "string"},
-                {"name": "chainId", "type": "uint256"},
-                {"name": "verifyingContract", "type": "address"},
-            ],
-        },
-        "primaryType": "Agent",
-        "message": agent,
-    }
-    return sign_inner(wallet, data)
+def sign_usd_transfer_action(wallet, action, is_mainnet):
+    return sign_user_signed_action(
+        wallet,
+        action,
+        [
+            {"name": "hyperliquidChain", "type": "string"},
+            {"name": "destination", "type": "string"},
+            {"name": "amount", "type": "string"},
+            {"name": "time", "type": "uint64"},
+        ],
+        "HyperliquidTransaction:UsdSend",
+        is_mainnet,
+    )
+
+
+def sign_withdraw_from_bridge_action(wallet, action, is_mainnet):
+    return sign_user_signed_action(
+        wallet,
+        action,
+        [
+            {"name": "hyperliquidChain", "type": "string"},
+            {"name": "destination", "type": "string"},
+            {"name": "amount", "type": "string"},
+            {"name": "time", "type": "uint64"},
+        ],
+        "HyperliquidTransaction:Withdraw",
+        is_mainnet,
+    )
+
+
+def sign_agent(wallet, action, is_mainnet):
+    return sign_user_signed_action(
+        wallet,
+        action,
+        [
+            {"name": "hyperliquidChain", "type": "string"},
+            {"name": "agentAddress", "type": "address"},
+            {"name": "agentName", "type": "string"},
+            {"name": "nonce", "type": "uint64"},
+        ],
+        "HyperliquidTransaction:ApproveAgent",
+        is_mainnet,
+    )
 
 
 def sign_inner(wallet, data):
     structured_data = encode_structured_data(data)
     signed = wallet.sign_message(structured_data)
     return {"r": to_hex(signed["r"]), "s": to_hex(signed["s"]), "v": signed["v"]}
```

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/utils/types.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/utils/types.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.3.0/hyperliquid/websocket_manager.py` & `hyperliquid_python_sdk-0.4.0/hyperliquid/websocket_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         else:
             for active_subscription in active_subscriptions:
                 active_subscription.callback(ws_msg)
 
     def on_open(self, _ws):
         logging.debug("on_open")
         self.ws_ready = True
-        for (subscription, active_subscription) in self.queued_subscriptions:
+        for subscription, active_subscription in self.queued_subscriptions:
             self.subscribe(subscription, active_subscription.callback, active_subscription.subscription_id)
 
     def subscribe(
         self, subscription: Subscription, callback: Callable[[Any], None], subscription_id: Optional[int] = None
     ) -> int:
         if subscription_id is None:
             self.subscription_id_counter += 1
@@ -111,8 +111,8 @@
             raise NotImplementedError("Can't unsubscribe before websocket connected")
         identifier = subscription_to_identifier(subscription)
         active_subscriptions = self.active_subscriptions[identifier]
         new_active_subscriptions = [x for x in active_subscriptions if x.subscription_id != subscription_id]
         if len(new_active_subscriptions) == 0:
             self.ws.send(json.dumps({"method": "unsubscribe", "subscription": subscription}))
         self.active_subscriptions[identifier] = new_active_subscriptions
-        return len(active_subscriptions) != len(active_subscriptions)
+        return len(active_subscriptions) != len(new_active_subscriptions)
```

### Comparing `hyperliquid_python_sdk-0.3.0/pyproject.toml` & `hyperliquid_python_sdk-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperliquid-python-sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = "SDK for Hyperliquid API trading with Python."
 readme = "README.md"
 authors = ["Hyperliquid <hello@hyperliquid.xyz>"]
 license = "MIT"
 repository = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 homepage = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 packages = [
```

### Comparing `hyperliquid_python_sdk-0.3.0/PKG-INFO` & `hyperliquid_python_sdk-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperliquid-python-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: SDK for Hyperliquid API trading with Python.
 Home-page: https://github.com/hyperliquid-dex/hyperliquid-python-sdk
 License: MIT
 Author: Hyperliquid
 Author-email: hello@hyperliquid.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: eth-abi (>=3.0.1,<4.0.0)
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: eth-utils (>=2.1.0,<3.0.0)
 Requires-Dist: msgpack (>=1.0.5,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
```

