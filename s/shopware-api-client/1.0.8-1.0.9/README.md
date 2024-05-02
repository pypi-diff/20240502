# Comparing `tmp/shopware_api_client-1.0.8.tar.gz` & `tmp/shopware_api_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopware_api_client-1.0.8.tar", max compression
+gzip compressed data, was "shopware_api_client-1.0.9.tar", max compression
```

## Comparing `shopware_api_client-1.0.8.tar` & `shopware_api_client-1.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1107 2024-03-11 09:43:03.651370 shopware_api_client-1.0.8/LICENSE
--rw-r--r--   0        0        0    21769 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/README.md
--rw-r--r--   0        0        0     1582 2024-03-11 09:43:19.251506 shopware_api_client-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/__init__.py
--rw-r--r--   0        0        0    15423 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/base.py
--rw-r--r--   0        0        0     4203 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/client.py
--rw-r--r--   0        0        0     1463 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/config.py
--rw-r--r--   0        0        0        0 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/__init__.py
--rw-r--r--   0        0        0     5199 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/__init__.py
--rw-r--r--   0        0        0     7262 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/category.py
--rw-r--r--   0        0        0     3817 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_block.py
--rw-r--r--   0        0        0     2574 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_page.py
--rw-r--r--   0        0        0     3309 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_section.py
--rw-r--r--   0        0        0     2187 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_slot.py
--rw-r--r--   0        0        0     5163 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/country.py
--rw-r--r--   0        0        0     2055 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/country_state.py
--rw-r--r--   0        0        0     3328 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/currency.py
--rw-r--r--   0        0        0     2067 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/currency_country_rounding.py
--rw-r--r--   0        0        0     9558 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer.py
--rw-r--r--   0        0        0     3450 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_address.py
--rw-r--r--   0        0        0     2772 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_group.py
--rw-r--r--   0        0        0     1413 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_recovery.py
--rw-r--r--   0        0        0     2031 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_wishlist.py
--rw-r--r--   0        0        0     1972 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_wishlist_product.py
--rw-r--r--   0        0        0     1563 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/delivery_time.py
--rw-r--r--   0        0        0     3275 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document.py
--rw-r--r--   0        0        0     2830 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_base_config.py
--rw-r--r--   0        0        0     2382 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_base_config_sales_channel.py
--rw-r--r--   0        0        0     1945 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_type.py
--rw-r--r--   0        0        0     2846 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/landing_page.py
--rw-r--r--   0        0        0     3246 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/language.py
--rw-r--r--   0        0        0     1429 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/locale.py
--rw-r--r--   0        0        0     2298 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/main_category.py
--rw-r--r--   0        0        0     5995 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/media.py
--rw-r--r--   0        0        0     1763 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/media_thumbnail.py
--rw-r--r--   0        0        0     7729 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order.py
--rw-r--r--   0        0        0     3999 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_address.py
--rw-r--r--   0        0        0     3265 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_customer.py
--rw-r--r--   0        0        0     3890 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_delivery.py
--rw-r--r--   0        0        0     3046 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_delivery_position.py
--rw-r--r--   0        0        0     5108 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_line_item.py
--rw-r--r--   0        0        0     2498 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_line_item_download.py
--rw-r--r--   0        0        0     2646 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction.py
--rw-r--r--   0        0        0     2854 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture.py
--rw-r--r--   0        0        0     2901 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund.py
--rw-r--r--   0        0        0     3146 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund_position.py
--rw-r--r--   0        0        0     4748 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/payment_method.py
--rw-r--r--   0        0        0    14145 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product.py
--rw-r--r--   0        0        0     2662 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_configurator_setting.py
--rw-r--r--   0        0        0     2681 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_cross_selling.py
--rw-r--r--   0        0        0     2222 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_cross_selling_assigned_products.py
--rw-r--r--   0        0        0     2166 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_download.py
--rw-r--r--   0        0        0     4612 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_export.py
--rw-r--r--   0        0        0     1361 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_feature_set.py
--rw-r--r--   0        0        0     1998 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_manufacturer.py
--rw-r--r--   0        0        0     2238 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_media.py
--rw-r--r--   0        0        0     2428 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_price.py
--rw-r--r--   0        0        0     3032 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_review.py
--rw-r--r--   0        0        0     2097 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_search_keyword.py
--rw-r--r--   0        0        0     2069 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_stream.py
--rw-r--r--   0        0        0     1921 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_visibility.py
--rw-r--r--   0        0        0     4620 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion.py
--rw-r--r--   0        0        0     2743 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion_discount.py
--rw-r--r--   0        0        0     1796 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion_discount_prices.py
--rw-r--r--   0        0        0     2079 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/property_group.py
--rw-r--r--   0        0        0     2563 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/property_group_option.py
--rw-r--r--   0        0        0     2714 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/rule.py
--rw-r--r--   0        0        0    11236 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/sales_channel.py
--rw-r--r--   0        0        0     2920 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/sales_channel_domain.py
--rw-r--r--   0        0        0     2257 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/salutation.py
--rw-r--r--   0        0        0     3076 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/seo_url.py
--rw-r--r--   0        0        0     3609 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/shipping_method.py
--rw-r--r--   0        0        0     2122 2024-03-11 09:43:03.655370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine.py
--rw-r--r--   0        0        0     3159 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_history.py
--rw-r--r--   0        0        0     3441 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_state.py
--rw-r--r--   0        0        0     2399 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_transition.py
--rw-r--r--   0        0        0     1816 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tag.py
--rw-r--r--   0        0        0     1632 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax.py
--rw-r--r--   0        0        0     2076 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax_rule.py
--rw-r--r--   0        0        0     1516 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax_rule_type.py
--rw-r--r--   0        0        0     1423 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/unit.py
--rw-r--r--   0        0        0     3253 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/user.py
--rw-r--r--   0        0        0     4086 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/base_fields.py
--rw-r--r--   0        0        0     1460 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/relations.py
--rw-r--r--   0        0        0       57 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/store/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/store/core/__init__.py
--rw-r--r--   0        0        0     3107 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/endpoints/store/core/address.py
--rw-r--r--   0        0        0      406 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/exceptions.py
--rw-r--r--   0        0        0      251 2024-03-11 09:43:03.659370 shopware_api_client-1.0.8/src/shopware_api_client/logging.py
--rw-r--r--   0        0        0    22784 1970-01-01 00:00:00.000000 shopware_api_client-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/LICENSE
+-rw-r--r--   0        0        0    21769 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/README.md
+-rw-r--r--   0        0        0     1582 2024-03-11 09:44:31.581102 shopware_api_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/__init__.py
+-rw-r--r--   0        0        0    15423 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/base.py
+-rw-r--r--   0        0        0     4203 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/client.py
+-rw-r--r--   0        0        0     1463 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/config.py
+-rw-r--r--   0        0        0        0 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     5199 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/__init__.py
+-rw-r--r--   0        0        0     7262 2024-03-11 09:44:18.109175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/category.py
+-rw-r--r--   0        0        0     3817 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_block.py
+-rw-r--r--   0        0        0     2574 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_page.py
+-rw-r--r--   0        0        0     3309 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_section.py
+-rw-r--r--   0        0        0     2187 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_slot.py
+-rw-r--r--   0        0        0     5163 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/country.py
+-rw-r--r--   0        0        0     2055 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/country_state.py
+-rw-r--r--   0        0        0     3328 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/currency.py
+-rw-r--r--   0        0        0     2067 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/currency_country_rounding.py
+-rw-r--r--   0        0        0     9558 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer.py
+-rw-r--r--   0        0        0     3450 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_address.py
+-rw-r--r--   0        0        0     2772 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_group.py
+-rw-r--r--   0        0        0     1413 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_recovery.py
+-rw-r--r--   0        0        0     2031 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_wishlist.py
+-rw-r--r--   0        0        0     1972 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_wishlist_product.py
+-rw-r--r--   0        0        0     1563 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/delivery_time.py
+-rw-r--r--   0        0        0     3275 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document.py
+-rw-r--r--   0        0        0     2830 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_base_config.py
+-rw-r--r--   0        0        0     2382 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_base_config_sales_channel.py
+-rw-r--r--   0        0        0     1945 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_type.py
+-rw-r--r--   0        0        0     2846 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/landing_page.py
+-rw-r--r--   0        0        0     3246 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/language.py
+-rw-r--r--   0        0        0     1429 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/locale.py
+-rw-r--r--   0        0        0     2298 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/main_category.py
+-rw-r--r--   0        0        0     5995 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/media.py
+-rw-r--r--   0        0        0     1763 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/media_thumbnail.py
+-rw-r--r--   0        0        0     7729 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order.py
+-rw-r--r--   0        0        0     3999 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_address.py
+-rw-r--r--   0        0        0     3265 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_customer.py
+-rw-r--r--   0        0        0     3890 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_delivery.py
+-rw-r--r--   0        0        0     3046 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_delivery_position.py
+-rw-r--r--   0        0        0     5108 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_line_item.py
+-rw-r--r--   0        0        0     2498 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_line_item_download.py
+-rw-r--r--   0        0        0     2646 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction.py
+-rw-r--r--   0        0        0     2854 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture.py
+-rw-r--r--   0        0        0     2901 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund.py
+-rw-r--r--   0        0        0     3146 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund_position.py
+-rw-r--r--   0        0        0     4748 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/payment_method.py
+-rw-r--r--   0        0        0    14145 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product.py
+-rw-r--r--   0        0        0     2662 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_configurator_setting.py
+-rw-r--r--   0        0        0     2681 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_cross_selling.py
+-rw-r--r--   0        0        0     2222 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_cross_selling_assigned_products.py
+-rw-r--r--   0        0        0     2166 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_download.py
+-rw-r--r--   0        0        0     4612 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_export.py
+-rw-r--r--   0        0        0     1361 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_feature_set.py
+-rw-r--r--   0        0        0     1998 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_manufacturer.py
+-rw-r--r--   0        0        0     2238 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_media.py
+-rw-r--r--   0        0        0     2428 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_price.py
+-rw-r--r--   0        0        0     3032 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_review.py
+-rw-r--r--   0        0        0     2097 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_search_keyword.py
+-rw-r--r--   0        0        0     2069 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_stream.py
+-rw-r--r--   0        0        0     1921 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_visibility.py
+-rw-r--r--   0        0        0     4620 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion.py
+-rw-r--r--   0        0        0     2743 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion_discount.py
+-rw-r--r--   0        0        0     1796 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion_discount_prices.py
+-rw-r--r--   0        0        0     2079 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/property_group.py
+-rw-r--r--   0        0        0     2563 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/property_group_option.py
+-rw-r--r--   0        0        0     2714 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/rule.py
+-rw-r--r--   0        0        0    11236 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/sales_channel.py
+-rw-r--r--   0        0        0     2920 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/sales_channel_domain.py
+-rw-r--r--   0        0        0     2257 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/salutation.py
+-rw-r--r--   0        0        0     3076 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/seo_url.py
+-rw-r--r--   0        0        0     3609 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/shipping_method.py
+-rw-r--r--   0        0        0     2122 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine.py
+-rw-r--r--   0        0        0     3159 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_history.py
+-rw-r--r--   0        0        0     3441 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_state.py
+-rw-r--r--   0        0        0     2399 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_transition.py
+-rw-r--r--   0        0        0     1816 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tag.py
+-rw-r--r--   0        0        0     1632 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax.py
+-rw-r--r--   0        0        0     2076 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax_rule.py
+-rw-r--r--   0        0        0     1516 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax_rule_type.py
+-rw-r--r--   0        0        0     1423 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/unit.py
+-rw-r--r--   0        0        0     3253 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/user.py
+-rw-r--r--   0        0        0     4086 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/base_fields.py
+-rw-r--r--   0        0        0     1460 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/relations.py
+-rw-r--r--   0        0        0       57 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/store/core/__init__.py
+-rw-r--r--   0        0        0     3107 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/endpoints/store/core/address.py
+-rw-r--r--   0        0        0      406 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/exceptions.py
+-rw-r--r--   0        0        0      251 2024-03-11 09:44:18.113175 shopware_api_client-1.0.9/src/shopware_api_client/logging.py
+-rw-r--r--   0        0        0    22784 1970-01-01 00:00:00.000000 shopware_api_client-1.0.9/PKG-INFO
```

### Comparing `shopware_api_client-1.0.8/LICENSE` & `shopware_api_client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/README.md` & `shopware_api_client-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/pyproject.toml` & `shopware_api_client-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "shopware-api-client"
 description = " An api client for the Shopware API"
-version = "1.0.8"
+version = "1.0.9"
 license = "MIT"
 authors = ["GWS Gesellschaft für Warenwirtschafts-Systeme mbH <ebusiness@gws.ms>"]
 readme = "README.md"
 homepage = "https://github.com/GWS-mbH"
 repository = "https://github.com/GWS-mbH/shopware-api-client"
 documentation = "https://github.com/GWS-mbH/shopware-api-client/wiki"
 keywords = ["shopware", "api", "client"]
```

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/base.py` & `shopware_api_client-1.0.9/src/shopware_api_client/base.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/client.py` & `shopware_api_client-1.0.9/src/shopware_api_client/client.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/config.py` & `shopware_api_client-1.0.9/src/shopware_api_client/config.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/__init__.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/category.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/category.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_block.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_block.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_page.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_page.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_section.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_section.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/cms_slot.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/cms_slot.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/country.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/country.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/country_state.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/country_state.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/currency.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/currency.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/currency_country_rounding.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/currency_country_rounding.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_address.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_address.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_group.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_group.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_recovery.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_recovery.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_wishlist.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_wishlist.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/customer_wishlist_product.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/customer_wishlist_product.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/delivery_time.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/delivery_time.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_base_config.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_base_config.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_base_config_sales_channel.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_base_config_sales_channel.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/document_type.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/document_type.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/landing_page.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/landing_page.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/language.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/language.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/locale.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/locale.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/main_category.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/main_category.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/media.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/media.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/media_thumbnail.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/media_thumbnail.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_address.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_address.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_customer.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_customer.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_delivery.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_delivery.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_delivery_position.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_delivery_position.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_line_item.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_line_item.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_line_item_download.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_line_item_download.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund_position.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/order_transaction_capture_refund_position.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/payment_method.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/payment_method.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_configurator_setting.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_configurator_setting.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_cross_selling.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_cross_selling.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_cross_selling_assigned_products.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_cross_selling_assigned_products.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_download.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_download.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_export.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_export.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_feature_set.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_feature_set.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_manufacturer.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_manufacturer.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_media.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_media.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_price.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_price.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_review.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_review.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_search_keyword.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_search_keyword.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_stream.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_stream.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/product_visibility.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/product_visibility.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion_discount.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion_discount.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/promotion_discount_prices.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/promotion_discount_prices.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/property_group.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/property_group.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/property_group_option.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/property_group_option.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/rule.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/rule.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/sales_channel.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/sales_channel.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/sales_channel_domain.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/sales_channel_domain.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/salutation.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/salutation.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/seo_url.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/seo_url.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/shipping_method.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/shipping_method.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_history.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_history.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_state.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_state.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/state_machine_transition.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/state_machine_transition.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tag.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tag.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax_rule.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax_rule.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/tax_rule_type.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/tax_rule_type.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/unit.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/unit.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/admin/core/user.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/admin/core/user.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/base_fields.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/base_fields.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/relations.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/relations.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/src/shopware_api_client/endpoints/store/core/address.py` & `shopware_api_client-1.0.9/src/shopware_api_client/endpoints/store/core/address.py`

 * *Files identical despite different names*

### Comparing `shopware_api_client-1.0.8/PKG-INFO` & `shopware_api_client-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopware-api-client
-Version: 1.0.8
+Version: 1.0.9
 Summary:  An api client for the Shopware API
 Home-page: https://github.com/GWS-mbH
 License: MIT
 Keywords: shopware,api,client
 Author: GWS Gesellschaft für Warenwirtschafts-Systeme mbH
 Author-email: ebusiness@gws.ms
 Requires-Python: >=3.12,<4.0
```

