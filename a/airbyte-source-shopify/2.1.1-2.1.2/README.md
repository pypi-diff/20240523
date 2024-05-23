# Comparing `tmp/airbyte_source_shopify-2.1.1.tar.gz` & `tmp/airbyte_source_shopify-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.1.2.tar", max compression
```

## Comparing `airbyte_source_shopify-2.1.1.tar` & `airbyte_source_shopify-2.1.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4529 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/README.md
--rw-r--r--   0        0        0      800 2024-05-22 19:57:02.553799 airbyte_source_shopify-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1114 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0     1549 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4886 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    13110 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/scopes.py
--rw-r--r--   0        0        0        0 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/__init__.py
--rw-r--r--   0        0        0     1813 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20372 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    74527 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6479 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     1704 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/retry.py
--rw-r--r--   0        0        0      328 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/status.py
--rw-r--r--   0        0        0     3629 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8518 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/spec.json
--rw-r--r--   0        0        0    37215 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11754 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/transform.py
--rw-r--r--   0        0        0    13468 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/utils.py
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/README.md
+-rw-r--r--   0        0        0      800 2024-05-23 10:10:05.833154 airbyte_source_shopify-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1114 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0    10425 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4886 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    13110 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/scopes.py
+-rw-r--r--   0        0        0        0 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/__init__.py
+-rw-r--r--   0        0        0     1813 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20372 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    81938 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6526 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1704 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8518 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/spec.json
+-rw-r--r--   0        0        0    37215 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11626 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-23 09:08:39.000000 airbyte_source_shopify-2.1.2/source_shopify/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.2/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.1.1/README.md` & `airbyte_source_shopify-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/pyproject.toml` & `airbyte_source_shopify-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.1"
+version = "2.1.2"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/__init__.py` & `airbyte_source_shopify-2.1.2/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/auth.py` & `airbyte_source_shopify-2.1.2/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.1.2/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/product_images.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6805555555555555%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the image'}, 'shop_url': "*

 * *                 "{'description': 'URL of the shop where the image is hosted'}, 'created_at': "*

 * *                 "OrderedDict([('description', 'Date and time when the image was created'), "*

 * *                 "('type', ['null', 'string']), ('format', 'date-time')]), 'position': "*

 * *                 "OrderedDict([('description', 'Position order of the image relative to other "*

 * *                 "images of the same product') […]*

```diff
@@ -1,83 +1,101 @@
 {
     "additionalProperties": true,
     "properties": {
-        "cause_cancel": {
-            "description": "Reason indicating why the order is at risk of cancellation.",
+        "admin_graphql_api_id": {
+            "description": "Unique identifier for the image in the Admin GraphQL API",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "checkout_id": {
-            "description": "The unique identifier of the checkout associated with the order.",
+        "alt": {
+            "description": "Alternative text description of the image for accessibility",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "display": {
-            "description": "Flag to determine if the risk should be displayed to the merchant.",
+        "created_at": {
+            "description": "Date and time when the image was created",
+            "format": "date-time",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "id": {
-            "description": "Unique identifier for the order risk entry.",
+        "height": {
+            "description": "Height of the image in pixels",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "merchant_message": {
-            "description": "Message shown to the merchant regarding the risk.",
+        "id": {
+            "description": "Unique identifier for the image",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "message": {
-            "description": "Description of the risk associated with the order.",
+        "position": {
+            "description": "Position order of the image relative to other images of the same product",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "order_id": {
-            "description": "The identifier of the order to which the risk is related.",
+        "product_id": {
+            "description": "Unique identifier of the product associated with the image",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "recommendation": {
-            "description": "Suggested action to mitigate the risk.",
+        "shop_url": {
+            "description": "URL of the shop where the image is hosted",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "score": {
-            "description": "Numerical score indicating the level of risk.",
+        "src": {
+            "description": "URL of the image",
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "shop_url": {
-            "description": "URL of the shop where the order was placed.",
+        "updated_at": {
+            "description": "Date and time when the image was last updated",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "source": {
-            "description": "Source of the risk notification.",
+        "variant_ids": {
+            "description": "Array of unique identifiers for the product variants associated with the image",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
+            ]
+        },
+        "width": {
+            "description": "Width of the image in pixels",
+            "type": [
+                "null",
+                "integer"
             ]
         }
     },
-    "type": "object"
+    "type": [
+        "null",
+        "object"
+    ]
 }
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/smart_collections.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.861441798941799%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier for the smart collection'}, "*

 * *                 "'updated_at': {'description': 'The date and time when the collection was last "*

 * *                 "updated'}, 'admin_graphql_api_id': {'description': 'The unique identifier for "*

 * *                 "the collection in the GraphQL Admin API'}, 'shop_url': {'description': 'The URL "*

 * *                 "of the shop where the smart collection belongs'}, 'handle': "*

 * *                 "OrderedDict([('descripti […]*

```diff
@@ -1,100 +1,107 @@
 {
     "additionalProperties": true,
     "properties": {
         "admin_graphql_api_id": {
-            "description": "Unique identifier for the image in the Admin GraphQL API",
+            "description": "The unique identifier for the collection in the GraphQL Admin API",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "alt": {
-            "description": "Alternative text description of the image for accessibility",
+        "body_html": {
+            "description": "The description or details of the smart collection",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "created_at": {
-            "description": "Date and time when the image was created",
-            "format": "date-time",
+        "disjunctive": {
+            "description": "Indicates whether the collection uses disjunctive filtering",
             "type": [
                 "null",
-                "string"
+                "boolean"
             ]
         },
-        "height": {
-            "description": "Height of the image in pixels",
+        "handle": {
+            "description": "The human-friendly URL for the collection",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "id": {
-            "description": "Unique identifier for the image",
+            "description": "The unique identifier for the smart collection",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "position": {
-            "description": "Position order of the image relative to other images of the same product",
+        "published_at": {
+            "description": "The date and time when the collection was published",
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "product_id": {
-            "description": "Unique identifier of the product associated with the image",
+        "published_scope": {
+            "description": "The visibility of the collection to different sales channels",
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "rules": {
+            "description": "The filtering rules that determine which products are included in the collection",
+            "items": {
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
             ]
         },
         "shop_url": {
-            "description": "URL of the shop where the image is hosted",
+            "description": "The URL of the shop where the smart collection belongs",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "src": {
-            "description": "URL of the image",
+        "sort_order": {
+            "description": "The order in which the collection is displayed",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "description": "Date and time when the image was last updated",
-            "format": "date-time",
+        "template_suffix": {
+            "description": "The suffix added to the collection template filename",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "variant_ids": {
-            "description": "Array of unique identifiers for the product variants associated with the image",
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
+        "title": {
+            "description": "The title or name of the smart collection",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "width": {
-            "description": "Width of the image in pixels",
+        "updated_at": {
+            "description": "The date and time when the collection was last updated",
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         }
     },
     "type": [
         "null",
         "object"
     ]
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.1.2/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/scopes.py` & `airbyte_source_shopify-2.1.2/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1487,15 +1487,15 @@
         payment_details = record.get("paymentDetails", {})
         if payment_details:
             record["paymentDetails"] = self.tools.fields_names_to_snake_case(payment_details)
         # field names to snake case for root level
         record = self.tools.fields_names_to_snake_case(record)
         return record
 
-    def record_process_components(self, record: MutableMapping[str, Any]) -> Optional[MutableMapping[str, Any]]:
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Optional[Iterable[MutableMapping[str, Any]]]:
         """
         Defines how to process collected components.
         """
 
         if "transactions" in record.keys():
             transactions = record.get("transactions")
             if len(transactions) > 0:
@@ -1980,7 +1980,180 @@
         record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
         # clean up the leftovers
         record.pop("image", None)
         record.pop("product", None)
         record.pop("inventoryItem", None)
 
         yield record
+
+
+class OrderRisk(ShopifyBulkQuery):
+    """
+    {
+        orders(query: "updated_at:>='2021-04-13T00:00:00+00:00' AND updated_at:<='2024-05-20T13:50:06.882235+00:00'" sortKey: UPDATED_AT) {
+            edges {
+                node {
+                    __typename
+                    updatedAt
+                    order_id: id
+                    risk {
+                        recommendation
+                        assessments {
+                            risk_level: riskLevel
+                            facts {
+                                description
+                                sentiment
+                            }
+                            provider {
+                                features
+                                description
+                                handle
+                                embedded
+                                title
+                                published
+                                developer_name: developerName
+                                developer_type: developerType
+                                app_store_app_url: appStoreAppUrl
+                                install_url: installUrl
+                                app_store_developer_url: appStoreDeveloperUrl
+                                is_post_purchase_app_in_use: isPostPurchaseAppInUse
+                                previously_installed: previouslyInstalled
+                                pricing_details_summary: pricingDetailsSummary
+                                pricing_details: pricingDetails
+                                privacy_policy_url: privacyPolicyUrl
+                                public_category: publicCategory
+                                uninstall_message: uninstallMessage
+                                webhook_api_version: webhookApiVersion
+                                shopify_developed: shopifyDeveloped
+                                provider_id: id
+                                failed_requirements: failedRequirements {
+                                    message
+                                    action {
+                                        title
+                                        url
+                                        action_id: id
+                                    }
+                                }
+                                feedback {
+                                    link {
+                                        label
+                                        url
+                                    }
+                                    messages {
+                                        field
+                                        message
+                                    }
+                                }
+                            }
+                        }
+                    }
+                }
+            }
+        }
+    }
+    """
+
+    query_name = "orders"
+    sort_key = "UPDATED_AT"
+
+    action_fields: List[Field] = [
+        "title",
+        "url",
+        Field(name="id", alias="action_id"),
+    ]
+
+    failed_reqirements_fields: List[Field] = ["message", Field(name="action", fields=action_fields)]
+
+    feedback_fields: List[Field] = [
+        Field(name="link", fields=["label", "url"]),
+        Field(name="messages", fields=["field", "message"]),
+    ]
+
+    provider_fields: List[Field] = [
+        "features",
+        "description",
+        "handle",
+        "embedded",
+        "title",
+        "published",
+        Field(name="developerName", alias="developer_name"),
+        Field(name="developerType", alias="developer_type"),
+        Field(name="appStoreAppUrl", alias="app_store_app_url"),
+        Field(name="installUrl", alias="install_url"),
+        Field(name="appStoreDeveloperUrl", alias="app_store_developer_url"),
+        Field(name="isPostPurchaseAppInUse", alias="is_post_purchase_app_in_use"),
+        Field(name="previouslyInstalled", alias="previously_installed"),
+        Field(name="pricingDetailsSummary", alias="pricing_details_summary"),
+        Field(name="pricingDetails", alias="pricing_details"),
+        Field(name="privacyPolicyUrl", alias="privacy_policy_url"),
+        Field(name="publicCategory", alias="public_category"),
+        Field(name="uninstallMessage", alias="uninstall_message"),
+        Field(name="webhookApiVersion", alias="webhook_api_version"),
+        Field(name="shopifyDeveloped", alias="shopify_developed"),
+        Field(name="id", alias="provider_id"),
+        Field(name="failedRequirements", alias="failed_requirements", fields=failed_reqirements_fields),
+        Field(name="feedback", fields=feedback_fields),
+    ]
+
+    assessments_fields: List[Field] = [
+        Field(name="riskLevel", alias="risk_level"),
+        Field(name="facts", fields=["description", "sentiment"]),
+        Field(name="provider", fields=provider_fields),
+    ]
+
+    risk_fields: List[Field] = [
+        "recommendation",
+        Field(name="assessments", fields=assessments_fields),
+    ]
+
+    # main query
+    query_nodes: List[Field] = [
+        "__typename",
+        "updatedAt",
+        Field(name="id", alias="order_id"),
+        Field(name="risk", fields=risk_fields),
+    ]
+
+    record_composition = {
+        "new_record": "Order",
+        # there are no record components provided for this stream.
+    }
+
+    def _process_assessments(self, assessments: Iterable[MutableMapping[str, Any]]) -> Iterable[MutableMapping[str, Any]]:
+        for assessment in assessments:
+            provider = assessment.get("provider", {})
+            if provider:
+                # save and resolve provider id
+                provider["admin_graphql_api_id"] = provider.get("provider_id")
+                provider["provider_id"] = self.tools.resolve_str_id(provider.get("provider_id"))
+        return assessments
+
+    def _has_risk_recommendation(self, recommendation: Optional[str]) -> bool:
+        # if there are no risk recommendation, the value is literally "NONE",
+        # we should skip such record, because there is no risk info for it.
+        no_risk_pattern = "NONE"
+        return recommendation != no_risk_pattern if recommendation else False
+
+    def record_process_components(self, record: MutableMapping[str, Any]) -> Optional[Iterable[MutableMapping[str, Any]]]:
+        """
+        Defines how to process collected components.
+        """
+        # unnest mandatory fields from their placeholders
+        risk = record.get("risk", {})
+        recommendation = risk.get("recommendation") if risk else None
+        # process records which has some risk recommendation
+        if self._has_risk_recommendation(recommendation):
+            # save and resolve id
+            record["admin_graphql_api_id"] = record.get("order_id")
+            record["order_id"] = self.tools.resolve_str_id(record.get("order_id"))
+            # add old pk
+            record["id"] = record.get("order_id")
+            # add the `recommendation` field to the root lvl
+            record["recommendation"] = recommendation
+            assessments = risk.get("assessments", []) if risk else None
+            record["assessments"] = self._process_assessments(assessments) if assessments else None
+            # convert date-time cursors
+            record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
+            # clean up the leftovers
+            record.pop("risk", None)
+
+            yield record
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/record.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,22 +106,21 @@
         Output:
             { "id": 19435458986123, "admin_graphql_api_id": "gid://shopify/Order/19435458986123"}
         """
         # save the actual api id to the `admin_graphql_api_id`
         # while resolving the `id` in `record_resolve_id`,
         # we re-assign the original id like `"gid://shopify/Order/19435458986123"`,
         # into `admin_graphql_api_id` have the ability to identify the record oigin correctly in subsequent actions.
+        # IF NOT `id` field is provided by the query results, we should return composed record `as is`.
         id = record.get("id")
-        if isinstance(id, str):
+        if id and isinstance(id, str):
             record["admin_graphql_api_id"] = id
             # extracting the int(id) and reassign
             record["id"] = self.tools.resolve_str_id(id)
-            return record
-        elif isinstance(id, int):
-            return record
+        return record
 
     def produce_records(self, filename: str) -> Iterable[MutableMapping[str, Any]]:
         """
         Read the JSONL content saved from `job.job_retrieve_result()` line-by-line to avoid OOM.
         The filename example: `bulk-4039263649981.jsonl`,
             where `4039263649981` is the `id` of the COMPLETED BULK Jobw with `result_url`.
             Note: typically the `filename` is taken from the `result_url` string provided in the response.
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/retry.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/retry.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.1.2/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/source.py` & `airbyte_source_shopify-2.1.2/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/spec.json` & `airbyte_source_shopify-2.1.2/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.1.2/source_shopify/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.1.2/source_shopify/streams/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     MetafieldCustomer,
     MetafieldDraftOrder,
     MetafieldLocation,
     MetafieldOrder,
     MetafieldProduct,
     MetafieldProductImage,
     MetafieldProductVariant,
+    OrderRisk,
     Product,
     ProductImage,
     ProductVariant,
     Transaction,
 )
 from source_shopify.shopify_graphql.graphql import get_query_products
 from source_shopify.utils import ApiTypeEnum
@@ -253,23 +254,18 @@
 class OrderRefunds(IncrementalShopifyNestedStream):
     parent_stream_class = Orders
     # override default cursor field
     cursor_field = "created_at"
     nested_entity = "refunds"
 
 
-class OrderRisks(IncrementalShopifySubstream):
-    parent_stream_class = Orders
-    slice_key = "order_id"
-    data_field = "risks"
-    cursor_field = "id"
-
-    def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
-        order_id = stream_slice["order_id"]
-        return f"orders/{order_id}/{self.data_field}.json"
+class OrderRisks(IncrementalShopifyGraphQlBulkStream):
+    bulk_query: OrderRisk = OrderRisk
+    # the updated stream work only with >= `2024-04` shopify api version
+    api_version = "2024-04"
 
 
 class Transactions(IncrementalShopifySubstream):
     parent_stream_class = Orders
     slice_key = "order_id"
     data_field = "transactions"
     cursor_field = "created_at"
```

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/transform.py` & `airbyte_source_shopify-2.1.2/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/source_shopify/utils.py` & `airbyte_source_shopify-2.1.2/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.1/PKG-INFO` & `airbyte_source_shopify-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.1.1
+Version: 2.1.2
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

