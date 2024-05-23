# Comparing `tmp/pragma_sdk-1.3.5.tar.gz` & `tmp/pragma_sdk-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pragma_sdk-1.3.5.tar", max compression
+gzip compressed data, was "pragma_sdk-1.3.6.tar", max compression
```

## Comparing `pragma_sdk-1.3.5.tar` & `pragma_sdk-1.3.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      943 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/README.md
--rw-r--r--   0        0        0        0 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/__init__.py
--rw-r--r--   0        0        0      195 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/__init__.py
--rw-r--r--   0        0        0       55 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/abis/__init__.py
--rw-r--r--   0        0        0     1773 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/abis/abi.py
--rw-r--r--   0        0        0      375 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/abis/pragma_Admin.sierra.json
--rw-r--r--   0        0        0     6050 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/abis/pragma_ERC20.json
--rw-r--r--   0        0        0   140867 2024-05-23 15:33:12.086179 pragma_sdk-1.3.5/pragma/core/abis/pragma_ExampleRandomness.sierra.json
--rw-r--r--   0        0        0    34149 2024-05-23 15:33:12.090179 pragma_sdk-1.3.5/pragma/core/abis/pragma_MockOracle.sierra.json
--rw-r--r--   0        0        0  1705306 2024-05-23 15:33:12.094179 pragma_sdk-1.3.5/pragma/core/abis/pragma_Oracle.sierra.json
--rw-r--r--   0        0        0    42794 2024-05-23 15:33:12.094179 pragma_sdk-1.3.5/pragma/core/abis/pragma_Ownable.sierra.json
--rw-r--r--   0        0        0   275940 2024-05-23 15:33:12.094179 pragma_sdk-1.3.5/pragma/core/abis/pragma_PublisherRegistry.sierra.json
--rw-r--r--   0        0        0   544514 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/abis/pragma_Randomness.sierra.json
--rw-r--r--   0        0        0   323399 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/abis/pragma_SummaryStats.sierra.json
--rw-r--r--   0        0        0      686 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/abis/pragma_Upgradeable.sierra.json
--rw-r--r--   0        0        0   491352 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/abis/pragma_YieldCurve.sierra.json
--rw-r--r--   0        0        0     5669 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/assets.py
--rw-r--r--   0        0        0     6045 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/client.py
--rw-r--r--   0        0        0     1796 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/contract.py
--rw-r--r--   0        0        0    12550 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/entry.py
--rw-r--r--   0        0        0      393 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/logger.py
--rw-r--r--   0        0        0      344 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/__init__.py
--rw-r--r--   0        0        0     3831 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/nonce.py
--rw-r--r--   0        0        0     7303 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/offchain.py
--rw-r--r--   0        0        0    15874 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/oracle.py
--rw-r--r--   0        0        0     2505 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0    14419 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/mixins/transactions.py
--rw-r--r--   0        0        0        0 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/randomness/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/randomness/actions.py
--rw-r--r--   0        0        0    16307 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/randomness/randomness_utils.py
--rw-r--r--   0        0        0     1845 2024-05-23 15:33:12.098179 pragma_sdk-1.3.5/pragma/core/randomness/utils.py
--rw-r--r--   0        0        0    11211 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/core/types.py
--rw-r--r--   0        0        0     2598 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/core/utils.py
--rw-r--r--   0        0        0       59 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/__init__.py
--rw-r--r--   0        0        0    10500 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/client.py
--rw-r--r--   0        0        0      652 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3191 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     4694 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/binance.py
--rw-r--r--   0        0        0     2330 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     4756 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/bybit.py
--rw-r--r--   0        0        0     2832 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2565 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3243 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     5142 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     7690 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/gecko.py
--rw-r--r--   0        0        0     2706 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     4622 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/huobi.py
--rw-r--r--   0        0        0     3219 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/index.py
--rw-r--r--   0        0        0     3836 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/indexcoop.py
--rw-r--r--   0        0        0     4198 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/kucoin.py
--rw-r--r--   0        0        0     3350 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     6523 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/propeller.py
--rw-r--r--   0        0        0     6209 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/starknetamm.py
--rw-r--r--   0        0        0     5050 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0     2514 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/fetchers/upbit.py
--rw-r--r--   0        0        0      114 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/future_fetchers/__init__.py
--rw-r--r--   0        0        0     4855 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/future_fetchers/binance.py
--rw-r--r--   0        0        0     3161 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/future_fetchers/bybit.py
--rw-r--r--   0        0        0     4511 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/future_fetchers/okx.py
--rw-r--r--   0        0        0     1199 2024-05-23 15:33:12.102179 pragma_sdk-1.3.5/pragma/publisher/types.py
--rw-r--r--   0        0        0     4102 2024-05-23 15:33:12.106179 pragma_sdk-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.3.5/setup.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/core/abis/__init__.py
+-rw-r--r--   0        0        0     1773 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/core/abis/abi.py
+-rw-r--r--   0        0        0      375 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/core/abis/pragma_Admin.sierra.json
+-rw-r--r--   0        0        0     6050 2024-05-23 16:46:20.460783 pragma_sdk-1.3.6/pragma/core/abis/pragma_ERC20.json
+-rw-r--r--   0        0        0   140867 2024-05-23 16:46:20.464783 pragma_sdk-1.3.6/pragma/core/abis/pragma_ExampleRandomness.sierra.json
+-rw-r--r--   0        0        0    34149 2024-05-23 16:46:20.464783 pragma_sdk-1.3.6/pragma/core/abis/pragma_MockOracle.sierra.json
+-rw-r--r--   0        0        0  1705306 2024-05-23 16:46:20.468783 pragma_sdk-1.3.6/pragma/core/abis/pragma_Oracle.sierra.json
+-rw-r--r--   0        0        0    42794 2024-05-23 16:46:20.468783 pragma_sdk-1.3.6/pragma/core/abis/pragma_Ownable.sierra.json
+-rw-r--r--   0        0        0   275940 2024-05-23 16:46:20.468783 pragma_sdk-1.3.6/pragma/core/abis/pragma_PublisherRegistry.sierra.json
+-rw-r--r--   0        0        0   544514 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/abis/pragma_Randomness.sierra.json
+-rw-r--r--   0        0        0   323399 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/abis/pragma_SummaryStats.sierra.json
+-rw-r--r--   0        0        0      686 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/abis/pragma_Upgradeable.sierra.json
+-rw-r--r--   0        0        0   491352 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/abis/pragma_YieldCurve.sierra.json
+-rw-r--r--   0        0        0     5669 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/assets.py
+-rw-r--r--   0        0        0     6045 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/client.py
+-rw-r--r--   0        0        0     1796 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/contract.py
+-rw-r--r--   0        0        0    12550 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/entry.py
+-rw-r--r--   0        0        0      393 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/logger.py
+-rw-r--r--   0        0        0      344 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/__init__.py
+-rw-r--r--   0        0        0     3831 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/nonce.py
+-rw-r--r--   0        0        0     7303 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/offchain.py
+-rw-r--r--   0        0        0    15874 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2505 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0    14498 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/mixins/transactions.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/randomness/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 16:46:20.472783 pragma_sdk-1.3.6/pragma/core/randomness/actions.py
+-rw-r--r--   0        0        0    16307 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/core/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     1845 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/core/randomness/utils.py
+-rw-r--r--   0        0        0    11211 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/core/types.py
+-rw-r--r--   0        0        0     2598 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/core/utils.py
+-rw-r--r--   0        0        0       59 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/__init__.py
+-rw-r--r--   0        0        0    10500 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/client.py
+-rw-r--r--   0        0        0      652 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3191 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     4694 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/binance.py
+-rw-r--r--   0        0        0     2330 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     4756 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/bybit.py
+-rw-r--r--   0        0        0     2832 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2565 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3243 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     5142 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     7690 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/gecko.py
+-rw-r--r--   0        0        0     2706 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     4622 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/huobi.py
+-rw-r--r--   0        0        0     3219 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/index.py
+-rw-r--r--   0        0        0     3836 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/indexcoop.py
+-rw-r--r--   0        0        0     4198 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/kucoin.py
+-rw-r--r--   0        0        0     3350 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     6523 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/propeller.py
+-rw-r--r--   0        0        0     6209 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/starknetamm.py
+-rw-r--r--   0        0        0     5050 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0     2514 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/fetchers/upbit.py
+-rw-r--r--   0        0        0      114 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0     4855 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3161 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     4511 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     1199 2024-05-23 16:46:20.476783 pragma_sdk-1.3.6/pragma/publisher/types.py
+-rw-r--r--   0        0        0     4102 2024-05-23 16:46:20.480783 pragma_sdk-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.3.6/setup.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.3.6/PKG-INFO
```

### Comparing `pragma_sdk-1.3.5/README.md` & `pragma_sdk-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/abi.py` & `pragma_sdk-1.3.6/pragma/core/abis/abi.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_ERC20.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_ERC20.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_ExampleRandomness.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_ExampleRandomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_MockOracle.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_MockOracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_Oracle.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_Oracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_Ownable.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_Ownable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_PublisherRegistry.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_PublisherRegistry.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_Randomness.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_Randomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_SummaryStats.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_SummaryStats.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_Upgradeable.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_Upgradeable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/abis/pragma_YieldCurve.sierra.json` & `pragma_sdk-1.3.6/pragma/core/abis/pragma_YieldCurve.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/assets.py` & `pragma_sdk-1.3.6/pragma/core/assets.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/client.py` & `pragma_sdk-1.3.6/pragma/core/client.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/contract.py` & `pragma_sdk-1.3.6/pragma/core/contract.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/entry.py` & `pragma_sdk-1.3.6/pragma/core/entry.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/nonce.py` & `pragma_sdk-1.3.6/pragma/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/offchain.py` & `pragma_sdk-1.3.6/pragma/core/mixins/offchain.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/oracle.py` & `pragma_sdk-1.3.6/pragma/core/mixins/oracle.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/publisher_registry.py` & `pragma_sdk-1.3.6/pragma/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/randomness.py` & `pragma_sdk-1.3.6/pragma/core/mixins/randomness.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,17 @@
 
     async def handle_random(
         self,
         private_key: int,
         min_block: int = 0,
     ):
         block_number = await self.full_node_client.get_block_number()
+
+        min_block = max(min_block, block_number - IGNORE_REQUEST_THRESHOLD)
+
         sk = felt_to_secret_key(private_key)
 
         more_pages = True
         continuation_token = None
 
         # TODO(#000): add nonce tracking
         while more_pages:
@@ -349,15 +352,15 @@
                 self.randomness.address,
                 keys=[
                     ["0xe3e1c077138abb6d570b1a7ba425f5479b12f50a78a72be680167d4cf79c48"]
                 ],
                 from_block_number=min_block,
                 to_block_number="pending",
                 continuation_token=continuation_token,
-                chunk_size=50,
+                chunk_size=500,
             )
             for event in event_list.events:
                 index_to_split = 7
                 event.data.pop(index_to_split)
                 first_part = event.data[:index_to_split]
                 second_part = event.data[index_to_split:]
                 event.data = first_part + [second_part]
```

### Comparing `pragma_sdk-1.3.5/pragma/core/mixins/transactions.py` & `pragma_sdk-1.3.6/pragma/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/randomness/randomness_utils.py` & `pragma_sdk-1.3.6/pragma/core/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/randomness/utils.py` & `pragma_sdk-1.3.6/pragma/core/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/types.py` & `pragma_sdk-1.3.6/pragma/core/types.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/core/utils.py` & `pragma_sdk-1.3.6/pragma/core/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/client.py` & `pragma_sdk-1.3.6/pragma/publisher/client.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/__init__.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/ascendex.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/binance.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/binance.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/bitstamp.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/bybit.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/cex.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/coinbase.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/coingecko.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/defillama.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/gecko.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/gecko.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/gemini.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/huobi.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/huobi.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/index.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/index.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/indexcoop.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/indexcoop.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/kucoin.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/kucoin.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/okx.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/propeller.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/propeller.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/starknetamm.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/starknetamm.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/thegraph.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/fetchers/upbit.py` & `pragma_sdk-1.3.6/pragma/publisher/fetchers/upbit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/future_fetchers/binance.py` & `pragma_sdk-1.3.6/pragma/publisher/future_fetchers/binance.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/future_fetchers/bybit.py` & `pragma_sdk-1.3.6/pragma/publisher/future_fetchers/bybit.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/future_fetchers/okx.py` & `pragma_sdk-1.3.6/pragma/publisher/future_fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pragma/publisher/types.py` & `pragma_sdk-1.3.6/pragma/publisher/types.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.3.5/pyproject.toml` & `pragma_sdk-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pragma-sdk"
-version = "1.3.5"
+version = "1.3.6"
 authors = ["0xevolve <matthias@pragma.build>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragma.build"
 repository = "https://github.com/Astraly-Labs/pragma-sdk"
 documentation = "https://docs.pragma.build"
 classifiers = [
```

### Comparing `pragma_sdk-1.3.5/setup.py` & `pragma_sdk-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'requests-mock>=1.11.0,<2.0.0',
  'starknet.py==0.20.0',
  'typer==0.6.1']
 
 setup_kwargs = {
     'name': 'pragma-sdk',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'Core package for rollup-native Pragma Oracle',
     'long_description': "# Pragma SDK\n\n[![codecov](https://codecov.io/gh/Astraly-Labs/pragma-sdk/graph/badge.svg?token=98pUFYGHIK)](https://codecov.io/gh/Astraly-Labs/pragma-sdk)\n\n[![Checks](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml/badge.svg)](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml)\n\n[![Package](https://img.shields.io/pypi/v/pragma-sdk)](https://pypi.org/project/pragma-sdk/)\n\n---\n\n**Pragma SDK, written in Python.**\n\nOne can leverage this SDK to interact with Pragma on Starknet.\nThis SDK should also be used by Data Providers willing to push data on Pragma contracts.\n\n## About\n\nFor more information, see the [project's repository](https://github.com/Astraly-Labs/Pragma), [documentation overview](https://docs.pragmaoracle.com/) and [documentation on how to publish data](https://docs.pragmaoracle.com/using-pragma/publishing-data).\n\n## Contributing\n\nSee the [CONTRIBUTING](./CONTRIBUTING.md) guide.",
     'author': '0xevolve',
     'author_email': 'matthias@pragma.build',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pragma.build',
```

### Comparing `pragma_sdk-1.3.5/PKG-INFO` & `pragma_sdk-1.3.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pragma-sdk
-Version: 1.3.5
+Version: 1.3.6
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragma.build
 Author: 0xevolve
 Author-email: matthias@pragma.build
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

