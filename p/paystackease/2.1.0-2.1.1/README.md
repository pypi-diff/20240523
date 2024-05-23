# Comparing `tmp/paystackease-2.1.0.tar.gz` & `tmp/paystackease-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-2.1.0.tar", max compression
+gzip compressed data, was "paystackease-2.1.1.tar", max compression
```

## Comparing `paystackease-2.1.0.tar` & `paystackease-2.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1069 2024-05-23 08:45:37.339184 paystackease-2.1.0/LICENSE
--rw-r--r--   0        0        0     4802 2024-05-23 08:45:37.339184 paystackease-2.1.0/README.md
--rw-r--r--   0        0        0     1335 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/__init__.py
--rw-r--r--   0        0        0     5713 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apaystack.py
--rw-r--r--   0        0        0      988 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/__init__.py
--rw-r--r--   0        0        0     2137 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/aapple_pay.py
--rw-r--r--   0        0        0     4355 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/abulk_charges.py
--rw-r--r--   0        0        0     5820 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/acharges.py
--rw-r--r--   0        0        0     6762 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/acustomers.py
--rw-r--r--   0        0        0     9269 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7980 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/adisputes.py
--rw-r--r--   0        0        0     1146 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/aintegration.py
--rw-r--r--   0        0        0     4327 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/amiscellaneous.py
--rw-r--r--   0        0        0     5644 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/apayment_pages.py
--rw-r--r--   0        0        0     9834 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/apayment_requests.py
--rw-r--r--   0        0        0     4547 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/aplans.py
--rw-r--r--   0        0        0     4253 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/aproducts.py
--rw-r--r--   0        0        0     3233 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/arefund.py
--rw-r--r--   0        0        0     3250 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/asettlements.py
--rw-r--r--   0        0        0     6232 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/asubaccounts.py
--rw-r--r--   0        0        0     4396 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/asubscriptions.py
--rw-r--r--   0        0        0     5399 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/aterminal.py
--rw-r--r--   0        0        0     5844 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/atransaction_splits.py
--rw-r--r--   0        0        0    12559 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/atransactions.py
--rw-r--r--   0        0        0     5281 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/atransfer_recipients.py
--rw-r--r--   0        0        0     4822 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/atransfers.py
--rw-r--r--   0        0        0     2717 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/atransfers_control.py
--rw-r--r--   0        0        0     2802 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/async_apis/averification.py
--rw-r--r--   0        0        0        0 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/__init__.py
--rw-r--r--   0        0        0     2084 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/apple_pay.py
--rw-r--r--   0        0        0     4263 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/bulk_charges.py
--rw-r--r--   0        0        0     5724 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/charges.py
--rw-r--r--   0        0        0     6663 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/customers.py
--rw-r--r--   0        0        0     9141 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     7864 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/disputes.py
--rw-r--r--   0        0        0     1110 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/integration.py
--rw-r--r--   0        0        0     4283 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/miscellaneous.py
--rw-r--r--   0        0        0     5560 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/payment_pages.py
--rw-r--r--   0        0        0     9706 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/payment_requests.py
--rw-r--r--   0        0        0     4479 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/plans.py
--rw-r--r--   0        0        0     4185 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/products.py
--rw-r--r--   0        0        0     3177 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/refund.py
--rw-r--r--   0        0        0     3214 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/settlements.py
--rw-r--r--   0        0        0     6158 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/subaccounts.py
--rw-r--r--   0        0        0     4305 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/subscriptions.py
--rw-r--r--   0        0        0     5285 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/terminal.py
--rw-r--r--   0        0        0     5747 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/transaction_splits.py
--rw-r--r--   0        0        0    12421 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/transactions.py
--rw-r--r--   0        0        0     5189 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/transfer_recipients.py
--rw-r--r--   0        0        0     4730 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/transfers.py
--rw-r--r--   0        0        0     2625 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/transfers_control.py
--rw-r--r--   0        0        0     2746 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/apis/sync_apis/verification.py
--rw-r--r--   0        0        0      479 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/__init__.py
--rw-r--r--   0        0        0     3805 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_api_base.py
--rw-r--r--   0        0        0     6727 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_api_base_client.py
--rw-r--r--   0        0        0     4680 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_api_client_requests.py
--rw-r--r--   0        0        0      660 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_api_client_response.py
--rw-r--r--   0        0        0     5007 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_api_errors.py
--rw-r--r--   0        0        0     1463 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/core/_webhook.py
--rw-r--r--   0        0        0      552 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/helpers/__init__.py
--rw-r--r--   0        0        0      742 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/helpers/convert.py
--rw-r--r--   0        0        0     3566 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/helpers/tool_kit.py
--rw-r--r--   0        0        0        0 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/metadata/__init__.py
--rw-r--r--   0        0        0       98 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/metadata/__version__.py
--rw-r--r--   0        0        0     3074 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/paystack.py
--rw-r--r--   0        0        0        0 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/utils/__init__.py
--rw-r--r--   0        0        0      193 2024-05-23 08:45:37.343184 paystackease-2.1.0/paystackease/utils/_compact.py
--rw-r--r--   0        0        0     2259 2024-05-23 08:45:38.691189 paystackease-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-23 09:07:31.368129 paystackease-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4802 2024-05-23 09:07:31.368129 paystackease-2.1.1/README.md
+-rw-r--r--   0        0        0     1552 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/__init__.py
+-rw-r--r--   0        0        0     5713 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apaystack.py
+-rw-r--r--   0        0        0      988 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/__init__.py
+-rw-r--r--   0        0        0     2137 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/aapple_pay.py
+-rw-r--r--   0        0        0     4355 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/abulk_charges.py
+-rw-r--r--   0        0        0     5820 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/acharges.py
+-rw-r--r--   0        0        0     6762 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/acustomers.py
+-rw-r--r--   0        0        0     9269 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/adedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7980 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/adisputes.py
+-rw-r--r--   0        0        0     1146 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/aintegration.py
+-rw-r--r--   0        0        0     4327 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/amiscellaneous.py
+-rw-r--r--   0        0        0     5644 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/apayment_pages.py
+-rw-r--r--   0        0        0     9834 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/apayment_requests.py
+-rw-r--r--   0        0        0     4547 2024-05-23 09:07:31.372129 paystackease-2.1.1/paystackease/apis/async_apis/aplans.py
+-rw-r--r--   0        0        0     4253 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/aproducts.py
+-rw-r--r--   0        0        0     3233 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/arefund.py
+-rw-r--r--   0        0        0     3250 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/asettlements.py
+-rw-r--r--   0        0        0     6232 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/asubaccounts.py
+-rw-r--r--   0        0        0     4396 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/asubscriptions.py
+-rw-r--r--   0        0        0     5399 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/aterminal.py
+-rw-r--r--   0        0        0     5844 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/atransaction_splits.py
+-rw-r--r--   0        0        0    12559 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/atransactions.py
+-rw-r--r--   0        0        0     5281 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/atransfer_recipients.py
+-rw-r--r--   0        0        0     4822 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/atransfers.py
+-rw-r--r--   0        0        0     2717 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/atransfers_control.py
+-rw-r--r--   0        0        0     2802 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/async_apis/averification.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/__init__.py
+-rw-r--r--   0        0        0     2084 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/apple_pay.py
+-rw-r--r--   0        0        0     4263 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/bulk_charges.py
+-rw-r--r--   0        0        0     5724 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/charges.py
+-rw-r--r--   0        0        0     6663 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/customers.py
+-rw-r--r--   0        0        0     9141 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     7864 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/disputes.py
+-rw-r--r--   0        0        0     1110 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/integration.py
+-rw-r--r--   0        0        0     4283 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/miscellaneous.py
+-rw-r--r--   0        0        0     5560 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/payment_pages.py
+-rw-r--r--   0        0        0     9706 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/payment_requests.py
+-rw-r--r--   0        0        0     4479 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/plans.py
+-rw-r--r--   0        0        0     4185 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/products.py
+-rw-r--r--   0        0        0     3177 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/refund.py
+-rw-r--r--   0        0        0     3214 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/settlements.py
+-rw-r--r--   0        0        0     6158 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/subaccounts.py
+-rw-r--r--   0        0        0     4305 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/subscriptions.py
+-rw-r--r--   0        0        0     5285 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/terminal.py
+-rw-r--r--   0        0        0     5747 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/transaction_splits.py
+-rw-r--r--   0        0        0    12421 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/transactions.py
+-rw-r--r--   0        0        0     5189 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/transfer_recipients.py
+-rw-r--r--   0        0        0     4730 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/transfers.py
+-rw-r--r--   0        0        0     2625 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/transfers_control.py
+-rw-r--r--   0        0        0     2746 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/apis/sync_apis/verification.py
+-rw-r--r--   0        0        0      618 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/__init__.py
+-rw-r--r--   0        0        0     3805 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_api_base.py
+-rw-r--r--   0        0        0     6727 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_api_base_client.py
+-rw-r--r--   0        0        0     4680 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_api_client_requests.py
+-rw-r--r--   0        0        0      660 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_api_client_response.py
+-rw-r--r--   0        0        0     5007 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_api_errors.py
+-rw-r--r--   0        0        0     1463 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/core/_webhook.py
+-rw-r--r--   0        0        0      552 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/helpers/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/helpers/convert.py
+-rw-r--r--   0        0        0     3566 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/helpers/tool_kit.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/metadata/__init__.py
+-rw-r--r--   0        0        0       98 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/metadata/__version__.py
+-rw-r--r--   0        0        0     3074 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/paystack.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/utils/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-23 09:07:31.376129 paystackease-2.1.1/paystackease/utils/_compact.py
+-rw-r--r--   0        0        0     2259 2024-05-23 09:07:32.812120 paystackease-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.1.1/PKG-INFO
```

### Comparing `paystackease-2.1.0/LICENSE` & `paystackease-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/README.md` & `paystackease-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/__init__.py` & `paystackease-2.1.1/paystackease/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """ Wrappers for Paystack API calls"""
 from paystackease.core import (
+    APIConnectionError,
+    InvalidRequestMethodError,
     PayStackError,
+    PayStackServerError,
+    PayStackSignatureVerifyError,
+    PayStackWebhook,
     SecretKeyError,
     TypeValueError,
-    InvalidRequestMethodError
 )
 from paystackease.apaystack import AsyncPayStackBase
 from paystackease.paystack import PayStackBase
 from paystackease.helpers import (
     convert_to_subunit,
     AccountType,
     Bearer,
@@ -35,14 +39,18 @@
     TransactionStatus,
     USSD,
 )
 
 __all__ = [
     'PayStackBase',
     'AsyncPayStackBase',
+    'APIConnectionError',
+    'PayStackServerError',
+    'PayStackSignatureVerifyError',
+    'PayStackWebhook',
     'PayStackError',
     'SecretKeyError',
     'TypeValueError',
     'InvalidRequestMethodError',
     'convert_to_subunit',
     'AccountType',
     'Bearer',
```

### Comparing `paystackease-2.1.0/paystackease/apaystack.py` & `paystackease-2.1.1/paystackease/apaystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/__init__.py` & `paystackease-2.1.1/paystackease/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/aapple_pay.py` & `paystackease-2.1.1/paystackease/apis/async_apis/aapple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/abulk_charges.py` & `paystackease-2.1.1/paystackease/apis/async_apis/abulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/acharges.py` & `paystackease-2.1.1/paystackease/apis/async_apis/acharges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/acustomers.py` & `paystackease-2.1.1/paystackease/apis/async_apis/acustomers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py` & `paystackease-2.1.1/paystackease/apis/async_apis/adedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/adisputes.py` & `paystackease-2.1.1/paystackease/apis/async_apis/adisputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/aintegration.py` & `paystackease-2.1.1/paystackease/apis/async_apis/aintegration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/amiscellaneous.py` & `paystackease-2.1.1/paystackease/apis/async_apis/amiscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/apayment_pages.py` & `paystackease-2.1.1/paystackease/apis/async_apis/apayment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/apayment_requests.py` & `paystackease-2.1.1/paystackease/apis/async_apis/apayment_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/aplans.py` & `paystackease-2.1.1/paystackease/apis/async_apis/aplans.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/aproducts.py` & `paystackease-2.1.1/paystackease/apis/async_apis/aproducts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/arefund.py` & `paystackease-2.1.1/paystackease/apis/async_apis/arefund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/asettlements.py` & `paystackease-2.1.1/paystackease/apis/async_apis/asettlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/asubaccounts.py` & `paystackease-2.1.1/paystackease/apis/async_apis/asubaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/asubscriptions.py` & `paystackease-2.1.1/paystackease/apis/async_apis/asubscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/aterminal.py` & `paystackease-2.1.1/paystackease/apis/async_apis/aterminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/atransaction_splits.py` & `paystackease-2.1.1/paystackease/apis/async_apis/atransaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/atransactions.py` & `paystackease-2.1.1/paystackease/apis/async_apis/atransactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/atransfer_recipients.py` & `paystackease-2.1.1/paystackease/apis/async_apis/atransfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/atransfers.py` & `paystackease-2.1.1/paystackease/apis/async_apis/atransfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/atransfers_control.py` & `paystackease-2.1.1/paystackease/apis/async_apis/atransfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/async_apis/averification.py` & `paystackease-2.1.1/paystackease/apis/async_apis/averification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/apple_pay.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/bulk_charges.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/charges.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/charges.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/customers.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/customers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/disputes.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/disputes.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/integration.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/integration.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/miscellaneous.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/payment_pages.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/payment_requests.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/payment_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/plans.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/plans.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/products.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/products.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/refund.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/refund.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/settlements.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/settlements.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/subaccounts.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/subscriptions.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/terminal.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/terminal.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/transaction_splits.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/transaction_splits.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/transactions.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/transactions.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/transfer_recipients.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/transfers.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/transfers.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/transfers_control.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/apis/sync_apis/verification.py` & `paystackease-2.1.1/paystackease/apis/sync_apis/verification.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_api_base.py` & `paystackease-2.1.1/paystackease/core/_api_base.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_api_base_client.py` & `paystackease-2.1.1/paystackease/core/_api_base_client.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_api_client_requests.py` & `paystackease-2.1.1/paystackease/core/_api_client_requests.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_api_client_response.py` & `paystackease-2.1.1/paystackease/core/_api_client_response.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_api_errors.py` & `paystackease-2.1.1/paystackease/core/_api_errors.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/core/_webhook.py` & `paystackease-2.1.1/paystackease/core/_webhook.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/helpers/__init__.py` & `paystackease-2.1.1/paystackease/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/helpers/convert.py` & `paystackease-2.1.1/paystackease/helpers/convert.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/helpers/tool_kit.py` & `paystackease-2.1.1/paystackease/helpers/tool_kit.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/paystackease/paystack.py` & `paystackease-2.1.1/paystackease/paystack.py`

 * *Files identical despite different names*

### Comparing `paystackease-2.1.0/pyproject.toml` & `paystackease-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paystackease"
-version = "2.1.0"
+version = "2.1.1"
 description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
 authors = ["Peter Mbachu <doublep098@gmail.com>"]
 maintainers = []
 license = "MIT"
 readme = "README.md"
 keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
 classifiers = [
```

### Comparing `paystackease-2.1.0/PKG-INFO` & `paystackease-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 2.1.0
+Version: 2.1.1
 Summary: This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs.
 License: MIT
 Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

