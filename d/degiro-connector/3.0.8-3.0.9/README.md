# Comparing `tmp/degiro_connector-3.0.8.tar.gz` & `tmp/degiro_connector-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiro_connector-3.0.8.tar", max compression
+gzip compressed data, was "degiro_connector-3.0.9.tar", max compression
```

## Comparing `degiro_connector-3.0.8.tar` & `degiro_connector-3.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1524 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/LICENSE
--rw-r--r--   0        0        0    62473 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/README.md
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/abstracts/__init__.py
--rw-r--r--   0        0        0     1903 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/abstracts/abstract_action.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/constants/__init__.py
--rw-r--r--   0        0        0      875 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/constants/headers.py
--rw-r--r--   0        0        0      235 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/constants/timeouts.py
--rw-r--r--   0        0        0     2900 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/constants/urls.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/helpers/__init__.py
--rw-r--r--   0        0        0     4029 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/helpers/lazy_loader.py
--rw-r--r--   0        0        0      644 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/helpers/pb_handler.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/models/__init__.py
--rw-r--r--   0        0        0     1937 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/models/model_connection.py
--rw-r--r--   0        0        0     2326 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/core/models/model_session.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/__init__.py
--rw-r--r--   0        0        0     4384 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/api.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/models/__init__.py
--rw-r--r--   0        0        0     1315 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/models/chart.py
--rw-r--r--   0        0        0     1254 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/models/message.py
--rw-r--r--   0        0        0     2347 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/models/metric.py
--rw-r--r--   0        0        0      549 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/models/ticker.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/tools/__init__.py
--rw-r--r--   0        0        0     8072 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/tools/chart_fetcher.py
--rw-r--r--   0        0        0     8540 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_fetcher.py
--rw-r--r--   0        0        0     6101 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_to_df.py
--rw-r--r--   0        0        0     7620 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_to_metric_list.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/__init__.py
--rw-r--r--   0        0        0     5150 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_check_order.py
--rw-r--r--   0        0        0     5531 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_confirm_order.py
--rw-r--r--   0        0        0     4241 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_connect.py
--rw-r--r--   0        0        0     3338 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_create_favourite_list.py
--rw-r--r--   0        0        0     2682 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_favourite_list.py
--rw-r--r--   0        0        0     2892 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_favourite_list_product.py
--rw-r--r--   0        0        0     2106 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_order.py
--rw-r--r--   0        0        0     1894 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_account_info.py
--rw-r--r--   0        0        0     5016 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_account_overview.py
--rw-r--r--   0        0        0     3613 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_agenda.py
--rw-r--r--   0        0        0     5327 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_cash_account_report.py
--rw-r--r--   0        0        0     1736 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_client_details.py
--rw-r--r--   0        0        0     2747 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_company_profile.py
--rw-r--r--   0        0        0     2733 2024-01-01 17:36:26.752560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_company_ratios.py
--rw-r--r--   0        0        0     1861 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_config.py
--rw-r--r--   0        0        0     2782 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_estimates_summaries.py
--rw-r--r--   0        0        0     3008 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_favourite.py
--rw-r--r--   0        0        0     3507 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_favourites_list.py
--rw-r--r--   0        0        0     2808 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_financial_statements.py
--rw-r--r--   0        0        0     3002 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_latest_news.py
--rw-r--r--   0        0        0     2406 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_news_by_company.py
--rw-r--r--   0        0        0     4943 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_orders_history.py
--rw-r--r--   0        0        0     4791 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_position_report.py
--rw-r--r--   0        0        0     3686 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_products_config.py
--rw-r--r--   0        0        0     4461 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_products_info.py
--rw-r--r--   0        0        0     2597 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_top_news_preview.py
--rw-r--r--   0        0        0     5114 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_transactions_history.py
--rw-r--r--   0        0        0     9092 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_update.py
--rw-r--r--   0        0        0     2128 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_logout.py
--rw-r--r--   0        0        0     3097 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_move_favourite.py
--rw-r--r--   0        0        0     4892 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_product_search.py
--rw-r--r--   0        0        0     2922 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_put_favourite_list_product.py
--rw-r--r--   0        0        0     3175 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_rename_favourite_list.py
--rw-r--r--   0        0        0     4385 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/actions/action_update_order.py
--rw-r--r--   0        0        0     4445 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/api.py
--rw-r--r--   0        0        0        0 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/__init__.py
--rw-r--r--   0        0        0      617 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/credentials.py
--rw-r--r--   0        0        0      748 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/favourite.py
--rw-r--r--   0        0        0     1298 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/login.py
--rw-r--r--   0        0        0      920 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/news.py
--rw-r--r--   0        0        0     2569 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/product_search.py
--rw-r--r--   0        0        0    21413 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/trading_pb2.py
--rw-r--r--   0        0        0    39200 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/trading_pb2.pyi
--rw-r--r--   0        0        0      159 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/degiro_connector/trading/models/trading_pb2_grpc.py
--rw-r--r--   0        0        0      921 2024-01-01 17:36:26.756560 degiro_connector-3.0.8/pyproject.toml
--rw-r--r--   0        0        0    63463 1970-01-01 00:00:00.000000 degiro_connector-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/LICENSE
+-rw-r--r--   0        0        0    62473 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/abstracts/__init__.py
+-rw-r--r--   0        0        0     1903 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/abstracts/abstract_action.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/constants/__init__.py
+-rw-r--r--   0        0        0      875 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/constants/headers.py
+-rw-r--r--   0        0        0      235 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/constants/timeouts.py
+-rw-r--r--   0        0        0     2900 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/constants/urls.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/helpers/__init__.py
+-rw-r--r--   0        0        0     4029 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/helpers/lazy_loader.py
+-rw-r--r--   0        0        0      644 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/helpers/pb_handler.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/models/__init__.py
+-rw-r--r--   0        0        0     1937 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/models/model_connection.py
+-rw-r--r--   0        0        0     2326 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/core/models/model_session.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/__init__.py
+-rw-r--r--   0        0        0     4384 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/api.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/models/__init__.py
+-rw-r--r--   0        0        0     1315 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/models/chart.py
+-rw-r--r--   0        0        0     1254 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/models/message.py
+-rw-r--r--   0        0        0     2347 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/models/metric.py
+-rw-r--r--   0        0        0      549 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/models/ticker.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/tools/__init__.py
+-rw-r--r--   0        0        0     8072 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/tools/chart_fetcher.py
+-rw-r--r--   0        0        0     8540 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_fetcher.py
+-rw-r--r--   0        0        0     6101 2024-01-01 17:38:43.114840 degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_to_df.py
+-rw-r--r--   0        0        0     7620 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_to_metric_list.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/__init__.py
+-rw-r--r--   0        0        0     5150 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_check_order.py
+-rw-r--r--   0        0        0     5531 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_confirm_order.py
+-rw-r--r--   0        0        0     4241 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_connect.py
+-rw-r--r--   0        0        0     3338 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_create_favourite_list.py
+-rw-r--r--   0        0        0     2682 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_favourite_list.py
+-rw-r--r--   0        0        0     2892 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_favourite_list_product.py
+-rw-r--r--   0        0        0     2106 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_order.py
+-rw-r--r--   0        0        0     1894 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_account_info.py
+-rw-r--r--   0        0        0     5016 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_account_overview.py
+-rw-r--r--   0        0        0     3613 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_agenda.py
+-rw-r--r--   0        0        0     5327 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_cash_account_report.py
+-rw-r--r--   0        0        0     1736 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_client_details.py
+-rw-r--r--   0        0        0     2747 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_company_profile.py
+-rw-r--r--   0        0        0     2733 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_company_ratios.py
+-rw-r--r--   0        0        0     1861 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_config.py
+-rw-r--r--   0        0        0     2782 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_estimates_summaries.py
+-rw-r--r--   0        0        0     3008 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_favourite.py
+-rw-r--r--   0        0        0     3507 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_favourites_list.py
+-rw-r--r--   0        0        0     2808 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_financial_statements.py
+-rw-r--r--   0        0        0     3002 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_latest_news.py
+-rw-r--r--   0        0        0     2406 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_news_by_company.py
+-rw-r--r--   0        0        0     4943 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_orders_history.py
+-rw-r--r--   0        0        0     4791 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_position_report.py
+-rw-r--r--   0        0        0     3686 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_products_config.py
+-rw-r--r--   0        0        0     4461 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_products_info.py
+-rw-r--r--   0        0        0     2597 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_top_news_preview.py
+-rw-r--r--   0        0        0     5114 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_transactions_history.py
+-rw-r--r--   0        0        0     9092 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_update.py
+-rw-r--r--   0        0        0     2128 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_logout.py
+-rw-r--r--   0        0        0     3097 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_move_favourite.py
+-rw-r--r--   0        0        0     4892 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_product_search.py
+-rw-r--r--   0        0        0     2922 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_put_favourite_list_product.py
+-rw-r--r--   0        0        0     3175 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_rename_favourite_list.py
+-rw-r--r--   0        0        0     4385 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/actions/action_update_order.py
+-rw-r--r--   0        0        0     4445 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/api.py
+-rw-r--r--   0        0        0        0 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/__init__.py
+-rw-r--r--   0        0        0      617 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/credentials.py
+-rw-r--r--   0        0        0      748 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/favourite.py
+-rw-r--r--   0        0        0     1298 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/login.py
+-rw-r--r--   0        0        0      920 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/news.py
+-rw-r--r--   0        0        0     2569 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/product_search.py
+-rw-r--r--   0        0        0    21413 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/trading_pb2.py
+-rw-r--r--   0        0        0    39200 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/trading_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/degiro_connector/trading/models/trading_pb2_grpc.py
+-rw-r--r--   0        0        0      940 2024-01-01 17:38:43.118840 degiro_connector-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0    63503 1970-01-01 00:00:00.000000 degiro_connector-3.0.9/PKG-INFO
```

### Comparing `degiro_connector-3.0.8/LICENSE` & `degiro_connector-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/README.md` & `degiro_connector-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/abstracts/abstract_action.py` & `degiro_connector-3.0.9/degiro_connector/core/abstracts/abstract_action.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/constants/headers.py` & `degiro_connector-3.0.9/degiro_connector/core/constants/headers.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/constants/urls.py` & `degiro_connector-3.0.9/degiro_connector/core/constants/urls.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/helpers/lazy_loader.py` & `degiro_connector-3.0.9/degiro_connector/core/helpers/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/helpers/pb_handler.py` & `degiro_connector-3.0.9/degiro_connector/core/helpers/pb_handler.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/models/model_connection.py` & `degiro_connector-3.0.9/degiro_connector/core/models/model_connection.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/core/models/model_session.py` & `degiro_connector-3.0.9/degiro_connector/core/models/model_session.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/api.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/api.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/models/chart.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/models/chart.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/models/message.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/models/message.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/models/metric.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/models/metric.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/models/ticker.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/models/ticker.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/tools/chart_fetcher.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/tools/chart_fetcher.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_fetcher.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_fetcher.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_to_df.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_to_df.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/quotecast/tools/ticker_to_metric_list.py` & `degiro_connector-3.0.9/degiro_connector/quotecast/tools/ticker_to_metric_list.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_check_order.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_check_order.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_confirm_order.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_confirm_order.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_connect.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_connect.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_create_favourite_list.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_create_favourite_list.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_favourite_list.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_favourite_list.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_favourite_list_product.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_favourite_list_product.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_delete_order.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_delete_order.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_account_info.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_account_info.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_account_overview.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_account_overview.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_agenda.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_agenda.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_cash_account_report.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_cash_account_report.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_client_details.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_client_details.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_company_profile.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_company_profile.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_company_ratios.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_company_ratios.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_config.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_config.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_estimates_summaries.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_estimates_summaries.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_favourite.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_favourite.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_favourites_list.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_favourites_list.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_financial_statements.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_financial_statements.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_latest_news.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_latest_news.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_news_by_company.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_news_by_company.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_orders_history.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_orders_history.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_position_report.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_position_report.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_products_config.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_products_config.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_products_info.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_products_info.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_top_news_preview.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_top_news_preview.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_transactions_history.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_transactions_history.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_get_update.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_get_update.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_logout.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_logout.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_move_favourite.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_move_favourite.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_product_search.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_product_search.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_put_favourite_list_product.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_put_favourite_list_product.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_rename_favourite_list.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_rename_favourite_list.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/actions/action_update_order.py` & `degiro_connector-3.0.9/degiro_connector/trading/actions/action_update_order.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/api.py` & `degiro_connector-3.0.9/degiro_connector/trading/api.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/credentials.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/credentials.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/favourite.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/favourite.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/login.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/login.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/news.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/news.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/product_search.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/product_search.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/trading_pb2.py` & `degiro_connector-3.0.9/degiro_connector/trading/models/trading_pb2.py`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/degiro_connector/trading/models/trading_pb2.pyi` & `degiro_connector-3.0.9/degiro_connector/trading/models/trading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `degiro_connector-3.0.8/pyproject.toml` & `degiro_connector-3.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 license = "BSD-3-Clause"
 name = "degiro-connector"
 packages = [
     { include = "degiro_connector" },
 ]
 readme = "README.md"
 repository = "https://github.com/chavithra/degiro-connector"
-version = "3.0.8"
+version = "3.0.9"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 onetimepass = "^1.0.1"
 requests = "^2.31.0"
 pydantic = "^2.0.3"
 polars = "^0.20.2"
 grpcio = "^1.51.1"
 protobuf = "^4.21.12"
 wrapt = "^1.14.1"
+orjson = "^3.9.10"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.9.2"
 pytest = "^7.2.0"
 black = "^22.12.0"
 mypy = "^0.991"
 types-requests = "^2.28.11"
```

### Comparing `degiro_connector-3.0.8/PKG-INFO` & `degiro_connector-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: degiro-connector
-Version: 3.0.8
+Version: 3.0.9
 Summary: This is yet another library to access Degiro's API.
 Home-page: https://github.com/chavithra/degiro-connector
 License: BSD-3-Clause
 Author: Chavithra PARANA
 Author-email: chavithra@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: grpcio (>=1.51.1,<2.0.0)
 Requires-Dist: onetimepass (>=1.0.1,<2.0.0)
+Requires-Dist: orjson (>=3.9.10,<4.0.0)
 Requires-Dist: polars (>=0.20.2,<0.21.0)
 Requires-Dist: protobuf (>=4.21.12,<5.0.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: wrapt (>=1.14.1,<2.0.0)
 Project-URL: Repository, https://github.com/chavithra/degiro-connector
 Description-Content-Type: text/markdown
```

