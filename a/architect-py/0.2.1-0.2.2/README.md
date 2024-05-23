# Comparing `tmp/architect_py-0.2.1.tar.gz` & `tmp/architect_py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architect_py-0.2.1.tar", max compression
+gzip compressed data, was "architect_py-0.2.2.tar", max compression
```

## Comparing `architect_py-0.2.1.tar` & `architect_py-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,31 @@
--rw-r--r--   0        0        0    11362 2024-04-01 23:48:50.192622 architect_py-0.2.1/LICENSE
--rw-r--r--   0        0        0      657 2024-04-01 23:49:46.235990 architect_py-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-01 22:50:17.669839 architect_py-0.2.1/architect_py/__init__.py
--rw-r--r--   0        0        0     1948 2024-04-02 17:39:38.312493 architect_py-0.2.1/architect_py/client.py
--rw-r--r--   0        0        0      613 2024-04-02 17:41:09.862335 architect_py-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 architect_py-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11362 2024-04-01 23:48:50.192622 architect_py-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1138 2024-05-23 01:54:47.403289 architect_py-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 22:50:17.669839 architect_py-0.2.2/architect_py/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-06 05:19:14.621077 architect_py-0.2.2/architect_py/client.py
+-rw-r--r--   0        0        0     5562 2024-05-22 22:05:56.032352 architect_py-0.2.2/architect_py/graphql_client/__init__.py
+-rw-r--r--   0        0        0      620 2024-05-15 17:03:05.821303 architect_py-0.2.2/architect_py/graphql_client/base_model.py
+-rw-r--r--   0        0        0      227 2024-05-15 17:03:05.781743 architect_py-0.2.2/architect_py/graphql_client/cancel_order.py
+-rw-r--r--   0        0        0    27071 2024-05-22 22:05:56.032613 architect_py-0.2.2/architect_py/graphql_client/client.py
+-rw-r--r--   0        0        0     2074 2024-05-22 22:05:56.032871 architect_py-0.2.2/architect_py/graphql_client/enums.py
+-rw-r--r--   0        0        0     2411 2024-05-15 17:03:05.820957 architect_py-0.2.2/architect_py/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      820 2024-05-22 22:05:56.033153 architect_py-0.2.2/architect_py/graphql_client/fills_subscription.py
+-rw-r--r--   0        0        0     3296 2024-05-15 17:03:05.820636 architect_py-0.2.2/architect_py/graphql_client/fragments.py
+-rw-r--r--   0        0        0      466 2024-05-15 17:03:05.754545 architect_py-0.2.2/architect_py/graphql_client/get_all_market_snapshots.py
+-rw-r--r--   0        0        0      694 2024-05-15 17:03:05.758152 architect_py-0.2.2/architect_py/graphql_client/get_balances_for_cpty.py
+-rw-r--r--   0        0        0      846 2024-05-15 17:03:05.768693 architect_py-0.2.2/architect_py/graphql_client/get_fills.py
+-rw-r--r--   0        0        0      426 2024-05-15 17:03:05.750146 architect_py-0.2.2/architect_py/graphql_client/get_filtered_markets.py
+-rw-r--r--   0        0        0      303 2024-05-15 17:03:05.745975 architect_py-0.2.2/architect_py/graphql_client/get_market.py
+-rw-r--r--   0        0        0      450 2024-05-15 17:03:05.752361 architect_py-0.2.2/architect_py/graphql_client/get_market_snapshot.py
+-rw-r--r--   0        0        0      322 2024-05-15 17:03:05.747912 architect_py-0.2.2/architect_py/graphql_client/get_markets.py
+-rw-r--r--   0        0        0      384 2024-05-15 17:03:05.760195 architect_py-0.2.2/architect_py/graphql_client/get_open_orders.py
+-rw-r--r--   0        0        0      300 2024-05-15 17:03:05.763894 architect_py-0.2.2/architect_py/graphql_client/get_order.py
+-rw-r--r--   0        0        0      384 2024-05-15 17:03:05.762227 architect_py-0.2.2/architect_py/graphql_client/get_out_orders.py
+-rw-r--r--   0        0        0     4716 2024-05-22 22:05:56.033446 architect_py-0.2.2/architect_py/graphql_client/input_types.py
+-rw-r--r--   0        0        0    13024 2024-05-15 17:03:05.821056 architect_py-0.2.2/architect_py/graphql_client/juniper_async_base_client.py
+-rw-r--r--   0        0        0      225 2024-05-15 17:03:05.780342 architect_py-0.2.2/architect_py/graphql_client/send_order.py
+-rw-r--r--   0        0        0      546 2024-05-15 17:03:05.775978 architect_py-0.2.2/architect_py/graphql_client/subscribe_book.py
+-rw-r--r--   0        0        0      295 2024-05-15 17:03:05.772860 architect_py-0.2.2/architect_py/graphql_client/subscribe_candles.py
+-rw-r--r--   0        0        0      709 2024-05-15 17:03:05.778972 architect_py-0.2.2/architect_py/graphql_client/subscribe_exchange_specific.py
+-rw-r--r--   0        0        0      356 2024-05-15 17:03:05.770835 architect_py-0.2.2/architect_py/graphql_client/subscribe_trades.py
+-rw-r--r--   0        0        0     1151 2024-05-23 01:55:00.591127 architect_py-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 architect_py-0.2.2/PKG-INFO
```

### Comparing `architect_py-0.2.1/LICENSE` & `architect_py-0.2.2/LICENSE`

 * *Files identical despite different names*

