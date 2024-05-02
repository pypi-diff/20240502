# Comparing `tmp/airbyte_source_shopify-2.0.7.tar.gz` & `tmp/airbyte_source_shopify-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.7.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.8.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.7.tar` & `airbyte_source_shopify-2.0.8.tar`

### file list

```diff
@@ -1,66 +1,68 @@
--rw-r--r--   0        0        0     4519 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/README.md
--rw-r--r--   0        0        0      800 2024-04-30 15:28:25.272251 airbyte_source_shopify-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1114 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0     1549 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-04-30 15:24:06.421962 airbyte_source_shopify-2.0.7/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4650 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    13110 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20743 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    56188 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-30 15:24:06.425962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/spec.json
--rw-r--r--   0        0        0    37097 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/transform.py
--rw-r--r--   0        0        0    13944 2024-04-30 15:24:06.433962 airbyte_source_shopify-2.0.7/source_shopify/utils.py
--rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/README.md
+-rw-r--r--   0        0        0      800 2024-05-02 15:40:09.627828 airbyte_source_shopify-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1114 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0     1549 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4650 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    13110 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    19793 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    56188 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1734 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/spec.json
+-rw-r--r--   0        0        0    37206 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11968 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-02 13:13:21.000000 airbyte_source_shopify-2.0.8/source_shopify/utils.py
+-rw-r--r--   0        0        0     5305 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.8/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.7/README.md` & `airbyte_source_shopify-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/pyproject.toml` & `airbyte_source_shopify-2.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.7"
+version = "2.0.8"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.8/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/auth.py` & `airbyte_source_shopify-2.0.8/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.8/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.0.8/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.8/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,361 +1,321 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
-from enum import Enum
 from time import sleep, time
-from typing import Any, Final, Iterable, List, Mapping, Optional, Union
+from typing import Any, Final, Iterable, List, Mapping, Optional
 
 import pendulum as pdm
 import requests
 from airbyte_cdk import AirbyteLogger
 from requests.exceptions import JSONDecodeError
 from source_shopify.utils import ApiTypeEnum
 from source_shopify.utils import ShopifyRateLimiter as limiter
 
 from .exceptions import AirbyteTracedException, ShopifyBulkExceptions
 from .query import ShopifyBulkTemplates
+from .retry import bulk_retry_on_exception
+from .status import ShopifyBulkJobStatus
 from .tools import END_OF_FILE, BulkTools
 
 
-class ShopifyBulkStatus(Enum):
-    CREATED = "CREATED"
-    CANCELED = "CANCELED"
-    CANCELING = "CANCELING"
-    COMPLETED = "COMPLETED"
-    RUNNING = "RUNNING"
-    FAILED = "FAILED"
-    TIMEOUT = "TIMEOUT"
-    ACCESS_DENIED = "ACCESS_DENIED"
-
-
 @dataclass
 class ShopifyBulkManager:
     session: requests.Session
     base_url: str
     stream_name: str
 
     # default logger
     logger: Final[AirbyteLogger] = logging.getLogger("airbyte")
 
     # 10Mb chunk size to save the file
-    retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
-    # time between job status checks
-    job_check_interval_sec: Final[int] = 2
+    _retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
+    _job_max_retries: Final[int] = 6
+    _job_backoff_time: int = 5
+    # saved latest request
+    _request: Optional[requests.Request] = None
+
+    # running job logger constrain, every 100-ish message will be printed
+    _log_job_msg_frequency: Final[int] = 100
+    # running job log counter
+    _log_job_msg_count: int = field(init=False, default=0)
 
+    # attempt counter
+    _concurrent_attempt: int = field(init=False, default=0)
     # sleep time per creation attempt
-    concurrent_interval_sec: Final[int] = 30
+    _concurrent_interval: Final[int] = 30
     # max attempts for job creation
-    concurrent_max_retry: Final[int] = 120
-    # Each job ideally should be executed within the specified time (in sec),
-    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 1 hours (3600 sec),
-    # Ideally the source will balance on it's own rate, based on the time taken to return the data for the slice.
-    job_max_elapsed_time_sec: Final[float] = 1800.0
+    _concurrent_max_retry: Final[int] = 120
+
+    # currents: _job_id, _job_state, _job_created_at, _job_self_canceled
+    _job_id: Optional[str] = field(init=False, default=None)
+    _job_state: ShopifyBulkJobStatus = field(init=False, default=None)
+    # completed and saved Bulk Job result filename
+    _job_result_filename: Optional[str] = field(init=False, default=None)
+    # date-time when the Bulk Job was created on the server
+    _job_created_at: Optional[str] = field(init=False, default=None)
+    # indicated whether or not we manually force-cancel the current job
+    _job_self_canceled: bool = field(init=False, default=False)
+    # time between job status checks
+    _job_check_interval: Final[int] = 3
+
     # 0.1 ~= P2H, default value, lower boundary for slice size
-    job_size_min: Final[float] = 0.1
+    _job_size_min: Final[float] = 0.1
     # P365D, upper boundary for slice size
-    job_size_max: Final[float] = 365.0
-    # running job logger constrain
-    log_job_state_msg_frequency: Final[int] = 10
-    # attempt limit indicator
-    concurrent_max_attempt_reached: bool = field(init=False, default=False)
-    # attempt counter
-    concurrent_attempt: int = field(init=False, default=0)
-    # currents: job_id, job_state, job_created_at, job_self_canceled
-    job_id: Optional[str] = field(init=False, default=None)
-    job_created_at: Optional[str] = field(init=False, default=None)
-    job_self_canceled: bool = field(init=False, default=False)
-    job_state: ShopifyBulkStatus = field(init=False, default=None)
-    # 2 sec is set as default value to cover the case with the empty-fast-completed jobs
-    job_last_elapsed_time: float = field(init=False, default=2.0)
+    _job_size_max: Final[float] = 365.0
     # dynamically adjusted slice interval
-    job_size: float = field(init=False, default=0.0)
+    _job_size: float = field(init=False, default=0.0)
     # expand slice factor
-    job_size_expand_factor: int = field(init=False, default=2)
+    _job_size_expand_factor: int = field(init=False, default=2)
     # reduce slice factor
-    job_size_reduce_factor: int = field(init=False, default=2)
+    _job_size_reduce_factor: int = field(init=False, default=2)
     # whether or not the slicer should revert the previous start value
-    job_should_revert_slice: bool = field(init=False, default=False)
-    # running job log counter
-    log_job_state_msg_count: int = field(init=False, default=0)
-    # one time retryable error counter
-    _one_time_error_retried: bool = field(init=False, default=False)
+    _job_should_revert_slice: bool = field(init=False, default=False)
+
+    # Each job ideally should be executed within the specified time (in sec),
+    # to maximize the performance for multi-connection syncs and control the bulk job size within +- 1 hours (3600 sec),
+    # Ideally the source will balance on it's own rate, based on the time taken to return the data for the slice.
+    _job_max_elapsed_time: Final[float] = 2700.0
+    # 2 sec is set as default value to cover the case with the empty-fast-completed jobs
+    _job_last_elapsed_time: float = field(init=False, default=2.0)
 
     @property
-    def tools(self) -> BulkTools:
+    def _tools(self) -> BulkTools:
         return BulkTools()
 
     @property
-    def job_state_to_fn_map(self) -> Mapping[str, Any]:
+    def _job_state_to_fn_map(self) -> Mapping[str, Any]:
         return {
-            ShopifyBulkStatus.CREATED.value: self.on_created_job,
-            ShopifyBulkStatus.CANCELING.value: self.on_canceling_job,
-            ShopifyBulkStatus.CANCELED.value: self.on_canceled_job,
-            ShopifyBulkStatus.COMPLETED.value: self.on_completed_job,
-            ShopifyBulkStatus.RUNNING.value: self.on_running_job,
-            ShopifyBulkStatus.TIMEOUT.value: self.on_timeout_job,
-            ShopifyBulkStatus.FAILED.value: self.on_failed_job,
-            ShopifyBulkStatus.ACCESS_DENIED.value: self.on_access_denied_job,
+            ShopifyBulkJobStatus.CREATED.value: self._on_created_job,
+            ShopifyBulkJobStatus.CANCELING.value: self._on_canceling_job,
+            ShopifyBulkJobStatus.CANCELED.value: self._on_canceled_job,
+            ShopifyBulkJobStatus.COMPLETED.value: self._on_completed_job,
+            ShopifyBulkJobStatus.RUNNING.value: self._on_running_job,
+            ShopifyBulkJobStatus.TIMEOUT.value: self._on_timeout_job,
+            ShopifyBulkJobStatus.FAILED.value: self._on_failed_job,
+            ShopifyBulkJobStatus.ACCESS_DENIED.value: self._on_access_denied_job,
         }
 
     @property
-    def job_size_adjusted_expand_factor(self, coef: float = 0.5) -> float:
+    def _job_size_adjusted_expand_factor(self, coef: float = 0.5) -> float:
         """
         The Job Size expand factor is calculated using EMA (Expotentional Moving Average):
             coef - the expantion coefficient
             previous_expand_factor - previous factor value
 
         Formula: expand_factor = coef * previous_expand_factor + (1 - coef)
         """
 
-        return coef * self.job_size_expand_factor + (1 - coef)
+        return coef * self._job_size_expand_factor + (1 - coef)
 
     @property
-    def job_size_adjusted_reduce_factor(self) -> float:
+    def _job_size_adjusted_reduce_factor(self) -> float:
         """
         The Job Size reduce factor is 2, by default.
         """
 
-        return self.job_size_reduce_factor
+        return self._job_size_reduce_factor
 
     @property
-    def job_elapsed_time_in_state(self) -> int:
+    def _job_elapsed_time_in_state(self) -> int:
         """
         Returns the elapsed time taken while Job is in certain status/state.
         """
-        return (pdm.now() - pdm.parse(self.job_created_at)).in_seconds() if self.job_created_at else 0
+        return (pdm.now() - pdm.parse(self._job_created_at)).in_seconds() if self._job_created_at else 0
 
     @property
-    def is_long_running_job(self) -> bool:
-        if self.job_elapsed_time_in_state:
-            if self.job_elapsed_time_in_state > self.job_max_elapsed_time_sec:
+    def _is_long_running_job(self) -> bool:
+        if self._job_elapsed_time_in_state:
+            if self._job_elapsed_time_in_state > self._job_max_elapsed_time:
                 # set the slicer to revert mode
-                self.job_should_revert_slice = True
+                self._job_should_revert_slice = True
                 return True
         # reset slicer to normal mode
-        self.job_should_revert_slice = False
+        self._job_should_revert_slice = False
         return False
 
-    def expand_job_size(self) -> None:
-        self.job_size += self.job_size_adjusted_expand_factor
+    def _expand_job_size(self) -> None:
+        self._job_size += self._job_size_adjusted_expand_factor
 
-    def reduce_job_size(self) -> None:
-        self.job_size /= self.job_size_adjusted_reduce_factor
+    def _reduce_job_size(self) -> None:
+        self._job_size /= self._job_size_adjusted_reduce_factor
 
-    def job_size_normalize(self, start: datetime, end: datetime) -> datetime:
-        # adjust slice size when it's bigger than the loop point when it should end,
-        # to preserve correct job size adjustments when this is the only job we need to run, based on STATE provided
-        requested_slice_size = (end - start).total_days()
-        self.job_size = requested_slice_size if requested_slice_size < self.job_size else self.job_size
-
-    def get_adjusted_job_end(self, slice_start: datetime, slice_end: datetime) -> datetime:
-        if self.is_long_running_job:
-            self._job_size_reduce_next()
-            return slice_start
-        else:
-            return slice_end
-
-    def get_adjusted_job_start(self, slice_start: datetime) -> datetime:
-        step = self.job_size if self.job_size else self.job_size_min
-        return slice_start.add(days=step)
+    def _save_latest_request(self, response: requests.Response) -> None:
+        self._request = response.request
 
     def _job_size_reduce_next(self) -> None:
         # revert the flag
-        self.job_should_revert_slice = False
-        self.reduce_job_size()
+        self._job_should_revert_slice = False
+        self._reduce_job_size()
 
     def __adjust_job_size(self, job_current_elapsed_time: float) -> None:
-        if self.job_should_revert_slice:
+        if self._job_should_revert_slice:
             pass
         else:
-            if job_current_elapsed_time < 1 or job_current_elapsed_time < self.job_last_elapsed_time:
-                self.expand_job_size()
-            elif job_current_elapsed_time > self.job_last_elapsed_time < self.job_max_elapsed_time_sec:
+            if job_current_elapsed_time < 1 or job_current_elapsed_time < self._job_last_elapsed_time:
+                self._expand_job_size()
+            elif job_current_elapsed_time > self._job_last_elapsed_time < self._job_max_elapsed_time:
                 pass
             # set the last job time
-            self.job_last_elapsed_time = job_current_elapsed_time
+            self._job_last_elapsed_time = job_current_elapsed_time
             # check the job size slice interval are acceptable
-            self.job_size = max(self.job_size_min, min(self.job_size, self.job_size_max))
+            self._job_size = max(self._job_size_min, min(self._job_size, self._job_size_max))
 
     def __reset_state(self) -> None:
-        # set current job state to default values
-        self.job_state, self.job_id = None, None
+        # reset the job state to default
+        self._job_state = None
+        # reset the filename to default
+        self._job_result_filename = None
         # setting self-cancelation to default
-        self.job_self_canceled = False
+        self._job_self_canceled = False
         # set the running job message counter to default
-        self.log_job_state_msg_count = 0
-        # set one time retry flag to default
-        self._one_time_error_retried = False
+        self._log_job_msg_count = 0
 
-    def job_completed(self) -> bool:
-        return self.job_state == ShopifyBulkStatus.COMPLETED.value
+    def _job_completed(self) -> bool:
+        return self._job_state == ShopifyBulkJobStatus.COMPLETED.value
 
-    def job_canceled(self) -> bool:
-        return self.job_state == ShopifyBulkStatus.CANCELED.value
+    def _job_canceled(self) -> bool:
+        return self._job_state == ShopifyBulkJobStatus.CANCELED.value
 
-    def job_cancel(self) -> None:
+    def _job_cancel(self) -> None:
         # re-use of `self._session(*, **)` to make BULK Job cancel request
-        cancel_args = self.job_get_request_args(ShopifyBulkTemplates.cancel)
+        cancel_args = self._job_get_request_args(ShopifyBulkTemplates.cancel)
         with self.session as cancel_job:
             canceled_response = cancel_job.request(**cancel_args)
             # mark the job was self-canceled
-            self.job_self_canceled = True
+            self._job_self_canceled = True
             # check CANCELED Job health
-            self.job_healthcheck(canceled_response)
+            self._job_healthcheck(canceled_response)
         # sleep to ensure the cancelation
-        sleep(self.job_check_interval_sec)
+        sleep(self._job_check_interval)
 
-    def log_job_state_with_count(self) -> None:
+    def _log_job_state_with_count(self) -> None:
         """
         Print the status/state Job info message every N request, to minimize the noise in the logs.
         """
-        if self.log_job_state_msg_count < self.log_job_state_msg_frequency:
-            self.log_job_state_msg_count += 1
+        if self._log_job_msg_count < self._log_job_msg_frequency:
+            self._log_job_msg_count += 1
         else:
-            message = f"Elapsed time: {self.job_elapsed_time_in_state} sec"
-            self.log_state(message)
-            self.log_job_state_msg_count = 0
+            message = f"Elapsed time: {self._job_elapsed_time_in_state} sec"
+            self._log_state(message)
+            self._log_job_msg_count = 0
 
-    def log_state(self, message: Optional[str] = None) -> None:
-        pattern = f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}"
+    def _log_state(self, message: Optional[str] = None) -> None:
+        pattern = f"Stream: `{self.stream_name}`, the BULK Job: `{self._job_id}` is {self._job_state}"
         if message:
             self.logger.info(f"{pattern}. {message}.")
         else:
             self.logger.info(pattern)
 
-    def job_get_request_args(self, template: ShopifyBulkTemplates) -> Mapping[str, Any]:
+    def _job_get_request_args(self, template: ShopifyBulkTemplates) -> Mapping[str, Any]:
         return {
             "method": "POST",
             "url": self.base_url,
-            "data": template(self.job_id),
+            "data": template(self._job_id),
             "headers": {"Content-Type": "application/graphql"},
         }
 
-    def job_get_result(self, response: Optional[requests.Response] = None) -> Optional[str]:
+    def _job_get_result(self, response: Optional[requests.Response] = None) -> Optional[str]:
         parsed_response = response.json().get("data", {}).get("node", {}) if response else None
-        job_result_url = parsed_response.get("url") if parsed_response and not self.job_self_canceled else None
+        job_result_url = parsed_response.get("url") if parsed_response and not self._job_self_canceled else None
         if job_result_url:
             # save to local file using chunks to avoid OOM
-            filename = self.tools.filename_from_url(job_result_url)
+            filename = self._tools.filename_from_url(job_result_url)
             with self.session.get(job_result_url, stream=True) as response:
                 response.raise_for_status()
                 with open(filename, "wb") as file:
-                    for chunk in response.iter_content(chunk_size=self.retrieve_chunk_size):
+                    for chunk in response.iter_content(chunk_size=self._retrieve_chunk_size):
                         file.write(chunk)
                     # add `<end_of_file>` line to the bottom  of the saved data for easy parsing
                     file.write(END_OF_FILE.encode())
             return filename
 
-    def job_update_state(self, response: Optional[requests.Response] = None) -> None:
+    def _job_update_state(self, response: Optional[requests.Response] = None) -> None:
         if response:
-            self.job_state = response.json().get("data", {}).get("node", {}).get("status")
-            if self.job_state in [ShopifyBulkStatus.RUNNING.value, ShopifyBulkStatus.CANCELING.value]:
-                self.log_job_state_with_count()
+            self._job_state = response.json().get("data", {}).get("node", {}).get("status")
+            if self._job_state in [ShopifyBulkJobStatus.RUNNING.value, ShopifyBulkJobStatus.CANCELING.value]:
+                self._log_job_state_with_count()
             else:
-                self.log_state()
+                self._log_state()
 
-    def on_created_job(self, **kwargs) -> None:
+    def _on_created_job(self, **kwargs) -> None:
         pass
 
-    def on_canceled_job(self, response: requests.Response) -> Optional[AirbyteTracedException]:
-        if not self.job_self_canceled:
+    def _on_canceled_job(self, response: requests.Response) -> Optional[AirbyteTracedException]:
+        if not self._job_self_canceled:
             raise ShopifyBulkExceptions.BulkJobCanceled(
-                f"The BULK Job: `{self.job_id}` exited with {self.job_state}, details: {response.text}",
+                f"The BULK Job: `{self._job_id}` exited with {self._job_state}, details: {response.text}",
             )
-        else:
-            pass
 
-    def on_canceling_job(self, **kwargs) -> None:
-        sleep(self.job_check_interval_sec)
+    def _on_canceling_job(self, **kwargs) -> None:
+        sleep(self._job_check_interval)
 
-    def on_running_job(self, **kwargs) -> None:
-        if self.is_long_running_job:
+    def _on_running_job(self, **kwargs) -> None:
+        if self._is_long_running_job:
             self.logger.info(
-                f"Stream: `{self.stream_name}` the BULK Job: {self.job_id} runs longer than expected. Retry with the reduced `Slice Size` after self-cancelation."
+                f"Stream: `{self.stream_name}` the BULK Job: {self._job_id} runs longer than expected. Retry with the reduced `Slice Size` after self-cancelation."
             )
             # cancel the long-running bulk job
-            self.job_cancel()
+            self._job_cancel()
         else:
-            sleep(self.job_check_interval_sec)
+            sleep(self._job_check_interval)
 
-    def on_completed_job(self, **kwargs) -> None:
-        pass
+    def _on_completed_job(self, response: Optional[requests.Response] = None) -> None:
+        self._job_result_filename = self._job_get_result(response)
 
-    def on_failed_job(self, response: requests.Response) -> AirbyteTracedException:
+    def _on_failed_job(self, response: requests.Response) -> AirbyteTracedException:
         raise ShopifyBulkExceptions.BulkJobFailed(
-            f"The BULK Job: `{self.job_id}` exited with {self.job_state}, details: {response.text}",
+            f"The BULK Job: `{self._job_id}` exited with {self._job_state}, details: {response.text}",
         )
 
-    def on_timeout_job(self, **kwargs) -> AirbyteTracedException:
+    def _on_timeout_job(self, **kwargs) -> AirbyteTracedException:
         raise ShopifyBulkExceptions.BulkJobTimout(
-            f"The BULK Job: `{self.job_id}` exited with {self.job_state}, please reduce the `GraphQL BULK Date Range in Days` in SOURCES > Your Shopify Source > SETTINGS.",
+            f"The BULK Job: `{self._job_id}` exited with {self._job_state}, please reduce the `GraphQL BULK Date Range in Days` in SOURCES > Your Shopify Source > SETTINGS.",
         )
 
-    def on_access_denied_job(self, **kwagrs) -> AirbyteTracedException:
+    def _on_access_denied_job(self, **kwagrs) -> AirbyteTracedException:
         raise ShopifyBulkExceptions.BulkJobAccessDenied(
-            f"The BULK Job: `{self.job_id}` exited with {self.job_state}, please check your PERMISSION to fetch the data for this stream.",
+            f"The BULK Job: `{self._job_id}` exited with {self._job_state}, please check your PERMISSION to fetch the data for this stream.",
         )
 
-    def on_job_with_errors(self, errors: List[Mapping[str, Any]]) -> AirbyteTracedException:
-        raise ShopifyBulkExceptions.BulkJobUnknownError(f"Could not validate the status of the BULK Job `{self.job_id}`. Errors: {errors}.")
+    def _on_job_with_errors(self, errors: List[Mapping[str, Any]]) -> AirbyteTracedException:
+        raise ShopifyBulkExceptions.BulkJobUnknownError(
+            f"Could not validate the status of the BULK Job `{self._job_id}`. Errors: {errors}."
+        )
 
-    def job_check_for_errors(self, response: requests.Response) -> Union[AirbyteTracedException, Iterable[Mapping[str, Any]]]:
+    def _job_check_for_errors(self, response: requests.Response) -> Optional[Iterable[Mapping[str, Any]]]:
         try:
+
             return response.json().get("errors") or response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("userErrors", [])
         except (Exception, JSONDecodeError) as e:
             raise ShopifyBulkExceptions.BulkJobBadResponse(
                 f"Couldn't check the `response` for `errors`, status: {response.status_code}, response: `{response.text}`. Trace: {repr(e)}."
             )
 
-    def job_one_time_retry_error(self, response: requests.Response, exception: Exception) -> Optional[requests.Response]:
-        if not self._one_time_error_retried:
-            request = response.request
-            self.logger.info(f"Stream: `{self.stream_name}`, retrying `Bad Request`: {request.body}. Error: {repr(exception)}.")
-            self._one_time_error_retried = True
-            return self.job_retry_request(request)
-        else:
-            self.on_job_with_errors(self.job_check_for_errors(response))
-
-    def job_track_running(self) -> Union[AirbyteTracedException, requests.Response]:
-        # format Job state check args
-        status_args = self.job_get_request_args(ShopifyBulkTemplates.status)
-        # re-use of `self._session(*, **)` to make BULK Job status checks
-        with self.session as track_running_job:
-            response = track_running_job.request(**status_args)
-        # errors check
-        try:
-            errors = self.job_check_for_errors(response)
-            if not errors:
-                self.job_update_state(response)
-                self.job_state_to_fn_map.get(self.job_state)(response=response)
-                return response
-            else:
-                # execute ERRORS scenario
-                self.on_job_with_errors(errors)
-        except (
-            ShopifyBulkExceptions.BulkJobBadResponse,
-            ShopifyBulkExceptions.BulkJobUnknownError,
-        ) as error:
-            return self.job_one_time_retry_error(response, error)
+    def _job_send_state_request(self) -> requests.Response:
+        with self.session as job_state_request:
+            status_args = self._job_get_request_args(ShopifyBulkTemplates.status)
+            self._request = requests.Request(**status_args, auth=self.session.auth).prepare()
+            return job_state_request.send(self._request)
+
+    def _job_track_running(self) -> None:
+        job_state_response = self._job_send_state_request()
+        errors = self._job_check_for_errors(job_state_response)
+        if errors:
+            # the exception raised when there are job-related errors, and the Job cannot be run futher.
+            self._on_job_with_errors(errors)
 
-    def job_check_state(self) -> Optional[str]:
-        response: Optional[requests.Response] = None
-        while not self.job_completed():
-            if self.job_canceled():
-                break
-            else:
-                response = self.job_track_running()
-        # return `job_result_url` when status is `COMPLETED`
-        return self.job_get_result(response)
+        self._job_update_state(job_state_response)
+        self._job_state_to_fn_map.get(self._job_state)(response=job_state_response)
 
-    def has_running_concurrent_job(self, errors: Optional[Iterable[Mapping[str, Any]]] = None) -> bool:
+    def _has_running_concurrent_job(self, errors: Optional[Iterable[Mapping[str, Any]]] = None) -> bool:
         """
         When concurent BULK Job is already running for the same SHOP we receive:
         Error example:
         [
             {
                 'field': None,
                 'message': 'A bulk query operation for this app and shop is already in progress: gid://shopify/BulkOperation/4039184154813.',
@@ -366,91 +326,114 @@
         concurent_job_pattern = "A bulk query operation for this app and shop is already in progress"
         # the errors are handled in `job_job_check_for_errors`
         if errors:
             for error in errors:
                 message = error.get("message", "") if isinstance(error, dict) else ""
                 if concurent_job_pattern in message:
                     return True
-        # reset the `concurrent_attempt` counter, once there is no concurrent job error
-        self.concurrent_attempt = 0
+        # reset the `_concurrent_attempt` counter, once there is no concurrent job error
+        self._concurrent_attempt = 0
         return False
 
-    def has_reached_max_concurrency_attempt(self) -> bool:
-        return self.concurrent_attempt == self.concurrent_max_retry
+    def _has_reached_max_concurrency(self) -> bool:
+        return self._concurrent_attempt == self._concurrent_max_retry
 
-    def job_retry_request(self, request: requests.PreparedRequest) -> Optional[requests.Response]:
-        with self.session.send(request) as retried_request:
+    def _job_retry_request(self) -> Optional[requests.Response]:
+        with self.session.send(self._request) as retried_request:
             return retried_request
 
-    def job_retry_concurrent(self, request: requests.PreparedRequest) -> Optional[requests.Response]:
-        self.concurrent_attempt += 1
+    def _job_retry_concurrent(self) -> Optional[requests.Response]:
+        self._concurrent_attempt += 1
         self.logger.warning(
-            f"Stream: `{self.stream_name}`, the BULK concurrency limit has reached. Waiting {self.concurrent_interval_sec} sec before retry, atttempt: {self.concurrent_attempt}.",
+            f"Stream: `{self.stream_name}`, the BULK concurrency limit has reached. Waiting {self._concurrent_interval} sec before retry, atttempt: {self._concurrent_attempt}.",
         )
-        sleep(self.concurrent_interval_sec)
-        return self.job_healthcheck(self.job_retry_request(request))
-
-    def job_get_id(self, response: requests.Response) -> Optional[str]:
-        response_data = response.json()
-        bulk_response = response_data.get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {})
-        if bulk_response and bulk_response.get("status") == ShopifyBulkStatus.CREATED.value:
-            job_id = bulk_response.get("id")
-            self.job_created_at = bulk_response.get("createdAt")
-            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{job_id}` is {ShopifyBulkStatus.CREATED.value}")
-            return job_id
-        else:
-            return None
+        sleep(self._concurrent_interval)
+        retried_response = self._job_retry_request()
+        return self._job_healthcheck(retried_response)
 
-    def job_retry_on_concurrency(self, request: requests.PreparedRequest) -> Union[AirbyteTracedException, Optional[requests.Response]]:
-        if self.has_reached_max_concurrency_attempt():
+    def _job_retry_on_concurrency(self) -> Optional[requests.Response]:
+        if self._has_reached_max_concurrency():
             # indicate we're out of attempts to retry with job creation
             message = f"The BULK Job couldn't be created at this time, since another job is running."
-            # log the message
             self.logger.error(message)
             # raise AibyteTracebackException with `INCOMPLETE` status
             raise ShopifyBulkExceptions.BulkJobConcurrentError(message)
         else:
-            return self.job_retry_concurrent(request)
+            return self._job_retry_concurrent()
 
-    def job_healthcheck(self, response: requests.Response) -> Optional[requests.Response]:
-        # get the latest request to retry
-        request: requests.PreparedRequest = response.request
-        try:
-            errors = self.job_check_for_errors(response)
-            # when the concurrent job takes place, we typically need to wait and retry, but no longer than 10 min.
-            if not self.has_running_concurrent_job(errors):
-                return response if not errors else None
+    def _job_healthcheck(self, response: requests.Response) -> Optional[requests.Response]:
+        # save the latest request to retry
+        self._save_latest_request(response)
+        # check for query errors
+        errors = self._job_check_for_errors(response)
+        # when the concurrent job takes place, we typically need to wait and retry, but no longer than 10 min.
+        if self._has_running_concurrent_job(errors):
+            return self._job_retry_on_concurrency()
+
+        return response if not errors else None
+
+    @bulk_retry_on_exception(logger)
+    def _job_check_state(self) -> Optional[str]:
+        while not self._job_completed():
+            if self._job_canceled():
+                break
             else:
-                return self.job_retry_on_concurrency(request)
-        except (ShopifyBulkExceptions.BulkJobBadResponse, ShopifyBulkExceptions.BulkJobUnknownError) as err:
-            # sometimes we face with `HTTP-500 Internal Server Error`
-            # we should retry such at least once
-            self.logger.info(f"Stream: `{self.stream_name}`, retrying Bad Request: {request.body}, error: {repr(err)}.")
-            return self.job_retry_request(request)
+                self._job_track_running()
+
+    # external method to be used within other components
+
+    def job_process_created(self, response: requests.Response) -> None:
+        """
+        The Bulk Job with CREATED status, should be processed, before we move forward with Job Status Checks.
+        """
+        response = self._job_healthcheck(response)
+        bulk_response = response.json().get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {})
+        if bulk_response and bulk_response.get("status") == ShopifyBulkJobStatus.CREATED.value:
+            self._job_id = bulk_response.get("id")
+            self._job_created_at = bulk_response.get("createdAt")
+            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self._job_id}` is {ShopifyBulkJobStatus.CREATED.value}")
+
+    def job_size_normalize(self, start: datetime, end: datetime) -> datetime:
+        # adjust slice size when it's bigger than the loop point when it should end,
+        # to preserve correct job size adjustments when this is the only job we need to run, based on STATE provided
+        requested_slice_size = (end - start).total_days()
+        self._job_size = requested_slice_size if requested_slice_size < self._job_size else self._job_size
+
+    def get_adjusted_job_start(self, slice_start: datetime) -> datetime:
+        step = self._job_size if self._job_size else self._job_size_min
+        return slice_start.add(days=step)
+
+    def get_adjusted_job_end(self, slice_start: datetime, slice_end: datetime) -> datetime:
+        if self._is_long_running_job:
+            self._job_size_reduce_next()
+            return slice_start
+        else:
+            return slice_end
 
     @limiter.balance_rate_limit(api_type=ApiTypeEnum.graphql.value)
-    def job_check(self, created_job_response: requests.Response) -> Optional[str]:
+    def job_check_for_completion(self) -> Optional[str]:
         """
-        This method checks the status for the BULK Job created, using it's `ID`.
+        This method checks the status for the `CREATED` Shopify BULK Job, using it's `ID`.
         The time spent for the Job execution is tracked to understand the effort.
         """
-        job_response = self.job_healthcheck(created_job_response)
-        self.job_id: str = self.job_get_id(job_response)
+        # track created job until it's COMPLETED
         job_started = time()
         try:
-            return self.job_check_state()
+            self._job_check_state()
+            return self._job_result_filename
         except (
             ShopifyBulkExceptions.BulkJobCanceled,
             ShopifyBulkExceptions.BulkJobFailed,
             ShopifyBulkExceptions.BulkJobTimout,
             ShopifyBulkExceptions.BulkJobAccessDenied,
-            # this one is one-time retriable
+            # this one is retryable, but stil needs to be raised,
+            # if the max attempts value is reached.
             ShopifyBulkExceptions.BulkJobUnknownError,
         ) as bulk_job_error:
             raise bulk_job_error
         finally:
             job_current_elapsed_time = round((time() - job_started), 3)
-            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` time elapsed: {job_current_elapsed_time} sec.")
+            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self._job_id}` time elapsed: {job_current_elapsed_time} sec.")
             # check whether or not we should expand or reduce the size of the slice
             self.__adjust_job_size(job_current_elapsed_time)
             # reset the state for COMPLETED job
             self.__reset_state()
```

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.8/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/source.py` & `airbyte_source_shopify-2.0.8/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/spec.json` & `airbyte_source_shopify-2.0.8/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.8/source_shopify/streams/base_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
     def __init__(self, config: Dict) -> None:
         super().__init__(config)
         # init BULK Query instance, pass `shop_id` from config
         self.query = self.bulk_query(shop_id=config.get("shop_id"))
         # define BULK Manager instance
         self.job_manager: ShopifyBulkManager = ShopifyBulkManager(
             session=self._session,
-            base_url=f"{self.url_base}/{self.path()}",
+            base_url=f"{self.url_base}{self.path()}",
             stream_name=self.name,
         )
         # overide the default job slice size, if provided (it's auto-adjusted, later on)
         self.bulk_window_in_days = config.get("bulk_window_in_days")
         if self.bulk_window_in_days:
             self.job_manager.job_size = self.bulk_window_in_days
         # define Record Producer instance
@@ -744,15 +744,15 @@
         if stream_state:
             return self.get_stream_state_value(stream_state)
         else:
             # for majority of cases we fallback to start_date, otherwise.
             return self.config.get("start_date")
 
     def emit_slice_message(self, slice_start: datetime, slice_end: datetime) -> None:
-        slice_size_message = f"Slice size: `P{round(self.job_manager.job_size, 1)}D`"
+        slice_size_message = f"Slice size: `P{round(self.job_manager._job_size, 1)}D`"
         self.logger.info(f"Stream: `{self.name}` requesting BULK Job for period: {slice_start} -- {slice_end}. {slice_size_message}")
 
     @stream_state_cache.cache_stream_state
     def stream_slices(self, stream_state: Optional[Mapping[str, Any]] = None, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         if self.filter_field:
             state = self.get_state_value(stream_state)
             start = pdm.parse(state)
@@ -769,16 +769,18 @@
             yield {"query": self.query.get()}
 
     def process_bulk_results(
         self,
         response: requests.Response,
         stream_state: Optional[Mapping[str, Any]] = None,
     ) -> Iterable[Mapping[str, Any]]:
-        # get results fetched from COMPLETED BULK Job or `None`
-        filename = self.job_manager.job_check(response)
+        # process the CREATED Job prior to other actions
+        self.job_manager.job_process_created(response)
+        # get results fetched from COMPLETED BULK Job
+        filename = self.job_manager.job_check_for_completion()
         # the `filename` could be `None`, meaning there are no data available for the slice period.
         if filename:
             # add `shop_url` field to each record produced
             records = self.add_shop_url_field(
                 # produce records from saved bulk job result
                 self.record_producer.read_file(filename)
             )
```

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.8/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/transform.py` & `airbyte_source_shopify-2.0.8/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.7/source_shopify/utils.py` & `airbyte_source_shopify-2.0.8/source_shopify/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     :: on_unknown_load = 1.0 sec - Shopify recommended time to hold between each API call.
     :: on_low_load = 0.2 sec (200 miliseconds) - ideal ratio between hold time and api call, also the standard hold time between each API call.
     :: on_mid_load = 1.5 sec - great timing to retrieve another 15% of request capacity while having mid_load.
     :: on_high_load = 5.0 sec - ideally we should wait 2.0 sec while having high_load, but we hold 5 sec to retrieve up to 80% of request capacity.
     """
 
     on_unknown_load: float = 1.0
+    on_very_low_load: float = 0.0
     on_low_load: float = 0.2
     on_mid_load: float = 1.5
     on_high_load: float = 5.0
 
     logger = logging.getLogger("airbyte")
 
     log_message_count = 0
@@ -118,28 +119,34 @@
         :: load - represents how close we are to being throttled
                 - 0.5 is half way through our allowance
                 - 1 indicates that all of the allowance is used and the api will start rejecting calls
         :: threshold - is the % cutoff for the rate_limits/load
         :: wait_time - time to wait between each request in seconds
 
         """
-        mid_load = threshold / 2  # average load based on threshold
+
+        half_of_threshold = threshold / 2  # average load based on threshold
+        quarter_of_threshold = threshold / 4  # low load based on threshold
+
         if not load:
             # when there is no rate_limits from header, use the `sleep_on_unknown_load`
             wait_time = ShopifyRateLimiter.on_unknown_load
             ShopifyRateLimiter.log_message_counter("API Load: `REGULAR`")
-        elif load >= threshold:
+        elif threshold <= load:
             wait_time = ShopifyRateLimiter.on_high_load
             ShopifyRateLimiter.log_message_counter("API Load: `HIGH`")
-        elif load >= mid_load:
+        elif half_of_threshold <= load < threshold:
             wait_time = ShopifyRateLimiter.on_mid_load
             ShopifyRateLimiter.log_message_counter("API Load: `MID`")
-        elif load < mid_load:
+        elif quarter_of_threshold <= load < half_of_threshold:
             wait_time = ShopifyRateLimiter.on_low_load
             ShopifyRateLimiter.log_message_counter("API Load: `LOW`")
+        elif load < quarter_of_threshold:
+            wait_time = ShopifyRateLimiter.on_very_low_load
+
         return wait_time
 
     @staticmethod
     def get_rest_api_wait_time(
         *args,
         threshold: float = 0.9,
         rate_limit_header: str = "X-Shopify-Shop-Api-Call-Limit",
@@ -215,30 +222,14 @@
                 load = None
         else:
             load = None
 
         wait_time = ShopifyRateLimiter._convert_load_to_time(load, threshold)
         return wait_time
 
-    def _debug_info(*args) -> Any:
-        # find the requests.Response inside args list
-        response = ShopifyRateLimiter.get_response_from_args(*args)
-
-        if response:
-            try:
-                content = response.json()
-                content_keys = list(content.keys())
-                stream_name = content_keys[0] if len(content_keys) > 0 else None
-                content_lengh = len(content.get(stream_name, [])) if stream_name else None
-                debug_info = {"stream": stream_name, "url": response.request.url, "n_records": content_lengh}
-                return debug_info
-            except (requests.JSONDecodeError, Exception):
-                # bypassing the errors, we don't care about it here
-                pass
-
     @staticmethod
     def wait_time(wait_time: float) -> None:
         return sleep(wait_time)
 
     @staticmethod
     def balance_rate_limit(
         threshold: float = 0.9,
```

### Comparing `airbyte_source_shopify-2.0.7/PKG-INFO` & `airbyte_source_shopify-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.7
+Version: 2.0.8
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

