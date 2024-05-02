# Comparing `tmp/lusid_sdk-2.1.79.tar.gz` & `tmp/lusid_sdk-2.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_sdk-2.1.79.tar", max compression
+gzip compressed data, was "lusid_sdk-2.1.81.tar", max compression
```

## Comparing `lusid_sdk-2.1.79.tar` & `lusid_sdk-2.1.81.tar`

### file list

```diff
@@ -1,1026 +1,1026 @@
--rw-r--r--   0        0        0   179507 2024-05-02 08:39:16.688008 lusid_sdk-2.1.79/README.md
--rw-r--r--   0        0        0   104391 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/__init__.py
--rw-r--r--   0        0        0     5388 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/api/__init__.py
--rw-r--r--   0        0        0   159655 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/api/abor_api.py
--rw-r--r--   0        0        0    64033 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/abor_configuration_api.py
--rw-r--r--   0        0        0    31640 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/address_key_definition_api.py
--rw-r--r--   0        0        0    38503 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/aggregation_api.py
--rw-r--r--   0        0        0    44687 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/allocations_api.py
--rw-r--r--   0        0        0    54742 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/amortisation_rule_sets_api.py
--rw-r--r--   0        0        0    23224 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/application_metadata_api.py
--rw-r--r--   0        0        0    43529 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/blocks_api.py
--rw-r--r--   0        0        0   126954 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/calendars_api.py
--rw-r--r--   0        0        0   363813 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/chart_of_accounts_api.py
--rw-r--r--   0        0        0    48588 2024-05-02 08:39:16.630009 lusid_sdk-2.1.79/lusid/api/complex_market_data_api.py
--rw-r--r--   0        0        0   113825 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/compliance_api.py
--rw-r--r--   0        0        0   101713 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/configuration_recipe_api.py
--rw-r--r--   0        0        0   106475 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/conventions_api.py
--rw-r--r--   0        0        0   102152 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/api/corporate_action_sources_api.py
--rw-r--r--   0        0        0    72539 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/counterparties_api.py
--rw-r--r--   0        0        0   165686 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/custom_entities_api.py
--rw-r--r--   0        0        0    40849 2024-05-02 08:39:16.631009 lusid_sdk-2.1.79/lusid/api/custom_entity_definitions_api.py
--rw-r--r--   0        0        0    41503 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/custom_entity_types_api.py
--rw-r--r--   0        0        0    47049 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/cut_label_definitions_api.py
--rw-r--r--   0        0        0    77801 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/data_types_api.py
--rw-r--r--   0        0        0    20227 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/derived_transaction_portfolios_api.py
--rw-r--r--   0        0        0    21368 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/entities_api.py
--rw-r--r--   0        0        0    44435 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/executions_api.py
--rw-r--r--   0        0        0   122388 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/funds_api.py
--rw-r--r--   0        0        0    81546 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/instrument_event_types_api.py
--rw-r--r--   0        0        0    45411 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/instrument_events_api.py
--rw-r--r--   0        0        0   281333 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/instruments_api.py
--rw-r--r--   0        0        0    96690 2024-05-02 08:39:16.632009 lusid_sdk-2.1.79/lusid/api/legacy_compliance_api.py
--rw-r--r--   0        0        0   268154 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/legal_entities_api.py
--rw-r--r--   0        0        0    45280 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/order_graph_api.py
--rw-r--r--   0        0        0    46091 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/order_instructions_api.py
--rw-r--r--   0        0        0    44646 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/order_management_api.py
--rw-r--r--   0        0        0    43587 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/orders_api.py
--rw-r--r--   0        0        0    43985 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/packages_api.py
--rw-r--r--   0        0        0    45263 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/participations_api.py
--rw-r--r--   0        0        0   247306 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/persons_api.py
--rw-r--r--   0        0        0    45797 2024-05-02 08:39:16.633009 lusid_sdk-2.1.79/lusid/api/placements_api.py
--rw-r--r--   0        0        0   378953 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/portfolio_groups_api.py
--rw-r--r--   0        0        0   366937 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/portfolios_api.py
--rw-r--r--   0        0        0   140397 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/property_definitions_api.py
--rw-r--r--   0        0        0    10281 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/queryable_keys_api.py
--rw-r--r--   0        0        0   115625 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/quotes_api.py
--rw-r--r--   0        0        0   143284 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/reconciliations_api.py
--rw-r--r--   0        0        0    39839 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/reference_lists_api.py
--rw-r--r--   0        0        0    47715 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/reference_portfolio_api.py
--rw-r--r--   0        0        0    27621 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/relation_definitions_api.py
--rw-r--r--   0        0        0    22888 2024-05-02 08:39:16.634009 lusid_sdk-2.1.79/lusid/api/relations_api.py
--rw-r--r--   0        0        0    54693 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/relationship_definitions_api.py
--rw-r--r--   0        0        0    19986 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/relationships_api.py
--rw-r--r--   0        0        0    30928 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/schemas_api.py
--rw-r--r--   0        0        0    16390 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/scopes_api.py
--rw-r--r--   0        0        0    84048 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/scripted_translation_api.py
--rw-r--r--   0        0        0    58533 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/search_api.py
--rw-r--r--   0        0        0    37460 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/sequences_api.py
--rw-r--r--   0        0        0    49946 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/staging_rule_set_api.py
--rw-r--r--   0        0        0   112489 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/structured_result_data_api.py
--rw-r--r--   0        0        0    62054 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/system_configuration_api.py
--rw-r--r--   0        0        0    50024 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/tax_rule_sets_api.py
--rw-r--r--   0        0        0   107626 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/transaction_configuration_api.py
--rw-r--r--   0        0        0    64512 2024-05-02 08:39:16.635009 lusid_sdk-2.1.79/lusid/api/transaction_fees_api.py
--rw-r--r--   0        0        0   555070 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/api/transaction_portfolios_api.py
--rw-r--r--   0        0        0    20092 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/api/translation_api.py
--rw-r--r--   0        0        0    30709 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/api_client.py
--rw-r--r--   0        0        0      852 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/api_response.py
--rw-r--r--   0        0        0    14404 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/configuration.py
--rw-r--r--   0        0        0     5326 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/exceptions.py
--rw-r--r--   0        0        0      560 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/__init__.py
--rw-r--r--   0        0        0    30567 2024-05-02 08:39:16.638009 lusid_sdk-2.1.79/lusid/extensions/api_client.py
--rw-r--r--   0        0        0     9772 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8052 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/api_configuration.py
--rw-r--r--   0        0        0     6760 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12698 2024-05-02 08:39:16.638009 lusid_sdk-2.1.79/lusid/extensions/rest.py
--rw-r--r--   0        0        0    11564 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-05-02 08:39:16.638009 lusid_sdk-2.1.79/lusid/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3877 2024-05-02 08:39:16.638009 lusid_sdk-2.1.79/lusid/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0    98046 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/__init__.py
--rw-r--r--   0        0        0     2947 2024-05-02 08:39:16.580009 lusid_sdk-2.1.79/lusid/models/a2_b_breakdown.py
--rw-r--r--   0        0        0     2725 2024-05-02 08:39:16.580009 lusid_sdk-2.1.79/lusid/models/a2_b_category.py
--rw-r--r--   0        0        0     9737 2024-05-02 08:39:16.580009 lusid_sdk-2.1.79/lusid/models/a2_b_data_record.py
--rw-r--r--   0        0        0    10650 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/a2_b_movement_record.py
--rw-r--r--   0        0        0     6987 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor.py
--rw-r--r--   0        0        0     7324 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor_configuration.py
--rw-r--r--   0        0        0     4373 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor_configuration_properties.py
--rw-r--r--   0        0        0     6539 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor_configuration_request.py
--rw-r--r--   0        0        0     4242 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor_properties.py
--rw-r--r--   0        0        0     5474 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/abor_request.py
--rw-r--r--   0        0        0     3863 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/access_controlled_action.py
--rw-r--r--   0        0        0     4806 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/access_controlled_resource.py
--rw-r--r--   0        0        0     3448 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/access_metadata_operation.py
--rw-r--r--   0        0        0     2396 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/access_metadata_value.py
--rw-r--r--   0        0        0     5144 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/account.py
--rw-r--r--   0        0        0     4272 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/account_properties.py
--rw-r--r--   0        0        0      837 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/accounting_method.py
--rw-r--r--   0        0        0     4120 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/accounts_upsert_response.py
--rw-r--r--   0        0        0     5707 2024-05-02 08:39:16.581009 lusid_sdk-2.1.79/lusid/models/accumulation_event.py
--rw-r--r--   0        0        0     2057 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/action_id.py
--rw-r--r--   0        0        0     2640 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/add_business_days_to_date_request.py
--rw-r--r--   0        0        0     2013 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/add_business_days_to_date_response.py
--rw-r--r--   0        0        0     2534 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/additional_payment.py
--rw-r--r--   0        0        0     4999 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_definition.py
--rw-r--r--   0        0        0     5281 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_compliance_parameter.py
--rw-r--r--   0        0        0     3212 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_definition.py
--rw-r--r--   0        0        0     2968 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_filter.py
--rw-r--r--   0        0        0     3275 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_list.py
--rw-r--r--   0        0        0     5505 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_list_compliance_parameter.py
--rw-r--r--   0        0        0     3451 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/address_key_option_definition.py
--rw-r--r--   0        0        0     4387 2024-05-02 08:39:16.582009 lusid_sdk-2.1.79/lusid/models/adjust_holding.py
--rw-r--r--   0        0        0     5986 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/adjust_holding_for_date_request.py
--rw-r--r--   0        0        0     5697 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/adjust_holding_request.py
--rw-r--r--   0        0        0     3334 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregate_spec.py
--rw-r--r--   0        0        0     5953 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregated_return.py
--rw-r--r--   0        0        0     5496 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregated_returns_dispersion_request.py
--rw-r--r--   0        0        0     7601 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregated_returns_request.py
--rw-r--r--   0        0        0     4098 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregated_returns_response.py
--rw-r--r--   0        0        0     5341 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregated_transactions_request.py
--rw-r--r--   0        0        0     2583 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_context.py
--rw-r--r--   0        0        0     3190 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_measure_failure_detail.py
--rw-r--r--   0        0        0     1062 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_op.py
--rw-r--r--   0        0        0     3128 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_options.py
--rw-r--r--   0        0        0     8326 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_query.py
--rw-r--r--   0        0        0      892 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/aggregation_type.py
--rw-r--r--   0        0        0    11554 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/allocation.py
--rw-r--r--   0        0        0     9777 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/allocation_request.py
--rw-r--r--   0        0        0     3454 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/allocation_service_run_response.py
--rw-r--r--   0        0        0     2851 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/allocation_set_request.py
--rw-r--r--   0        0        0     5344 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/amortisation_event.py
--rw-r--r--   0        0        0     3638 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/amortisation_rule.py
--rw-r--r--   0        0        0     5496 2024-05-02 08:39:16.583009 lusid_sdk-2.1.79/lusid/models/amortisation_rule_set.py
--rw-r--r--   0        0        0     4347 2024-05-02 08:39:16.580009 lusid_sdk-2.1.79/lusid/models/annul_quotes_response.py
--rw-r--r--   0        0        0     3328 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/annul_single_structured_data_response.py
--rw-r--r--   0        0        0     4499 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/annul_structured_data_response.py
--rw-r--r--   0        0        0      793 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/asset_class.py
--rw-r--r--   0        0        0     2435 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/asset_leg.py
--rw-r--r--   0        0        0     2745 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/barrier.py
--rw-r--r--   0        0        0     5886 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/basket.py
--rw-r--r--   0        0        0     2562 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/basket_identifier.py
--rw-r--r--   0        0        0     5687 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/batch_adjust_holdings_response.py
--rw-r--r--   0        0        0     4543 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/batch_upsert_instrument_properties_response.py
--rw-r--r--   0        0        0     5803 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/batch_upsert_portfolio_transactions_response.py
--rw-r--r--   0        0        0     4424 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/batch_upsert_property_definition_properties_response.py
--rw-r--r--   0        0        0     7158 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block.py
--rw-r--r--   0        0        0     2632 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_and_order_id_request.py
--rw-r--r--   0        0        0     2573 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_and_orders.py
--rw-r--r--   0        0        0     2513 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_and_orders_create_request.py
--rw-r--r--   0        0        0     6319 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_and_orders_request.py
--rw-r--r--   0        0        0     5797 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_request.py
--rw-r--r--   0        0        0     2620 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/block_set_request.py
--rw-r--r--   0        0        0     5839 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/blocked_order_request.py
--rw-r--r--   0        0        0    12280 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/bond.py
--rw-r--r--   0        0        0     5121 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/bond_coupon_event.py
--rw-r--r--   0        0        0     4599 2024-05-02 08:39:16.584009 lusid_sdk-2.1.79/lusid/models/bond_default_event.py
--rw-r--r--   0        0        0     5156 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bond_principal_event.py
--rw-r--r--   0        0        0     3719 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/book_transactions_request.py
--rw-r--r--   0        0        0     3537 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/book_transactions_response.py
--rw-r--r--   0        0        0     5168 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bool_compliance_parameter.py
--rw-r--r--   0        0        0     5457 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bool_list_compliance_parameter.py
--rw-r--r--   0        0        0     3857 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/branch_step.py
--rw-r--r--   0        0        0    10445 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bucketed_cash_flow_request.py
--rw-r--r--   0        0        0     5611 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bucketed_cash_flow_response.py
--rw-r--r--   0        0        0     2100 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/bucketing_schedule.py
--rw-r--r--   0        0        0     2480 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/calculation_info.py
--rw-r--r--   0        0        0     3961 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/calendar.py
--rw-r--r--   0        0        0     3688 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/calendar_date.py
--rw-r--r--   0        0        0     3871 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/calendar_dependency.py
--rw-r--r--   0        0        0     5980 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cap_floor.py
--rw-r--r--   0        0        0     4182 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_dependency.py
--rw-r--r--   0        0        0     6410 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_dividend_event.py
--rw-r--r--   0        0        0     3882 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_election.py
--rw-r--r--   0        0        0     5119 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_flow_event.py
--rw-r--r--   0        0        0     4785 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_flow_lineage.py
--rw-r--r--   0        0        0     5099 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_flow_value.py
--rw-r--r--   0        0        0     4424 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_flow_value_set.py
--rw-r--r--   0        0        0     2285 2024-05-02 08:39:16.585009 lusid_sdk-2.1.79/lusid/models/cash_ladder_record.py
--rw-r--r--   0        0        0     5183 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cash_perpetual.py
--rw-r--r--   0        0        0     8161 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cds_flow_conventions.py
--rw-r--r--   0        0        0     8115 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cds_index.py
--rw-r--r--   0        0        0     3213 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cds_protection_detail_specification.py
--rw-r--r--   0        0        0     5076 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/change.py
--rw-r--r--   0        0        0     4251 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/change_history.py
--rw-r--r--   0        0        0      702 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/change_history_action.py
--rw-r--r--   0        0        0     3837 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/change_item.py
--rw-r--r--   0        0        0     5391 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/chart_of_accounts.py
--rw-r--r--   0        0        0     4354 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/chart_of_accounts_properties.py
--rw-r--r--   0        0        0     4549 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/chart_of_accounts_request.py
--rw-r--r--   0        0        0     4758 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/check_step.py
--rw-r--r--   0        0        0     3332 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cleardown_module_details.py
--rw-r--r--   0        0        0     4507 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cleardown_module_request.py
--rw-r--r--   0        0        0     6150 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cleardown_module_response.py
--rw-r--r--   0        0        0     3505 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cleardown_module_rule.py
--rw-r--r--   0        0        0     4316 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/cleardown_module_rules_updated_response.py
--rw-r--r--   0        0        0     1980 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/client.py
--rw-r--r--   0        0        0     4801 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/close_event.py
--rw-r--r--   0        0        0     6413 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/close_period_diary_entry_request.py
--rw-r--r--   0        0        0     7827 2024-05-02 08:39:16.586009 lusid_sdk-2.1.79/lusid/models/complete_portfolio.py
--rw-r--r--   0        0        0     3908 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/complete_relation.py
--rw-r--r--   0        0        0     5168 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/complete_relationship.py
--rw-r--r--   0        0        0     9687 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/complex_bond.py
--rw-r--r--   0        0        0     5865 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/complex_market_data.py
--rw-r--r--   0        0        0     3964 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/complex_market_data_id.py
--rw-r--r--   0        0        0     2970 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_breached_order_info.py
--rw-r--r--   0        0        0     8295 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_parameter.py
--rw-r--r--   0        0        0     2172 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_parameter_type.py
--rw-r--r--   0        0        0     5581 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule.py
--rw-r--r--   0        0        0     4285 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_breakdown.py
--rw-r--r--   0        0        0     3951 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_breakdown_request.py
--rw-r--r--   0        0        0     6986 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_response.py
--rw-r--r--   0        0        0     4091 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_result.py
--rw-r--r--   0        0        0     4937 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_result_detail.py
--rw-r--r--   0        0        0     2320 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_result_portfolio_detail.py
--rw-r--r--   0        0        0     3061 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_result_v2.py
--rw-r--r--   0        0        0     7163 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_upsert_request.py
--rw-r--r--   0        0        0     2503 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_rule_upsert_response.py
--rw-r--r--   0        0        0     3437 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_run_info.py
--rw-r--r--   0        0        0     2703 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/compliance_run_info_v2.py
--rw-r--r--   0        0        0     3801 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_step.py
--rw-r--r--   0        0        0      827 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_step_type.py
--rw-r--r--   0        0        0     4919 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_summary_rule_result.py
--rw-r--r--   0        0        0     5038 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_summary_rule_result_request.py
--rw-r--r--   0        0        0     4039 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_template.py
--rw-r--r--   0        0        0     2383 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_template_parameter.py
--rw-r--r--   0        0        0     4961 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compliance_template_variation.py
--rw-r--r--   0        0        0     3645 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/component_transaction.py
--rw-r--r--   0        0        0     3350 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/composite_breakdown.py
--rw-r--r--   0        0        0     5315 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/composite_breakdown_request.py
--rw-r--r--   0        0        0     3925 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/composite_breakdown_response.py
--rw-r--r--   0        0        0     6527 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/composite_dispersion.py
--rw-r--r--   0        0        0     4138 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/composite_dispersion_response.py
--rw-r--r--   0        0        0     5481 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/compounding.py
--rw-r--r--   0        0        0     5894 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/configuration_recipe.py
--rw-r--r--   0        0        0     5178 2024-05-02 08:39:16.587009 lusid_sdk-2.1.79/lusid/models/constant_volatility_surface.py
--rw-r--r--   0        0        0     3233 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/constituents_adjustment_header.py
--rw-r--r--   0        0        0     6933 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/contract_for_difference.py
--rw-r--r--   0        0        0     4151 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/corporate_action.py
--rw-r--r--   0        0        0     5011 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/corporate_action_source.py
--rw-r--r--   0        0        0     3508 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/corporate_action_transition.py
--rw-r--r--   0        0        0     3122 2024-05-02 08:39:16.588009 lusid_sdk-2.1.79/lusid/models/corporate_action_transition_component.py
--rw-r--r--   0        0        0     2705 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/corporate_action_transition_component_request.py
--rw-r--r--   0        0        0     3529 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/corporate_action_transition_request.py
--rw-r--r--   0        0        0     4158 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/counterparty_agreement.py
--rw-r--r--   0        0        0     4209 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/counterparty_risk_information.py
--rw-r--r--   0        0        0     2826 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/counterparty_signatory.py
--rw-r--r--   0        0        0     2230 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_address_key_definition_request.py
--rw-r--r--   0        0        0     3478 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_amortisation_rule_set_request.py
--rw-r--r--   0        0        0     4454 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_calendar_request.py
--rw-r--r--   0        0        0     4734 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_corporate_action_source_request.py
--rw-r--r--   0        0        0     3948 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_custom_entity_type_request.py
--rw-r--r--   0        0        0     3723 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_cut_label_definition_request.py
--rw-r--r--   0        0        0     2478 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_data_map_request.py
--rw-r--r--   0        0        0     8058 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_data_type_request.py
--rw-r--r--   0        0        0     4785 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_date_request.py
--rw-r--r--   0        0        0     5951 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_derived_property_definition_request.py
--rw-r--r--   0        0        0    10150 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_derived_transaction_portfolio_request.py
--rw-r--r--   0        0        0     2364 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_portfolio_details.py
--rw-r--r--   0        0        0     6132 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_portfolio_group_request.py
--rw-r--r--   0        0        0     7429 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_property_definition_request.py
--rw-r--r--   0        0        0     3733 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_recipe_request.py
--rw-r--r--   0        0        0     6391 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_reconciliation_request.py
--rw-r--r--   0        0        0     5018 2024-05-02 08:39:16.589009 lusid_sdk-2.1.79/lusid/models/create_reference_portfolio_request.py
--rw-r--r--   0        0        0     4662 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_relation_definition_request.py
--rw-r--r--   0        0        0     2202 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_relation_request.py
--rw-r--r--   0        0        0     6630 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_relationship_definition_request.py
--rw-r--r--   0        0        0     4060 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_relationship_request.py
--rw-r--r--   0        0        0     4885 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_sequence_request.py
--rw-r--r--   0        0        0     3350 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_staging_rule_set_request.py
--rw-r--r--   0        0        0     3740 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_tax_rule_set_request.py
--rw-r--r--   0        0        0     2961 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_trade_tickets_response.py
--rw-r--r--   0        0        0    10893 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_transaction_portfolio_request.py
--rw-r--r--   0        0        0     3418 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/create_unit_definition.py
--rw-r--r--   0        0        0     8611 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/credit_default_swap.py
--rw-r--r--   0        0        0     3088 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/credit_rating.py
--rw-r--r--   0        0        0     7174 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/credit_spread_curve_data.py
--rw-r--r--   0        0        0     5420 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/credit_support_annex.py
--rw-r--r--   0        0        0      772 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/criterion_type.py
--rw-r--r--   0        0        0     2277 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/currency_and_amount.py
--rw-r--r--   0        0        0     5131 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/curve_options.py
--rw-r--r--   0        0        0     5040 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/custodian_account.py
--rw-r--r--   0        0        0     4363 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/custodian_account_properties.py
--rw-r--r--   0        0        0     6711 2024-05-02 08:39:16.590009 lusid_sdk-2.1.79/lusid/models/custodian_account_request.py
--rw-r--r--   0        0        0     4382 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custodian_accounts_upsert_response.py
--rw-r--r--   0        0        0     4624 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_definition.py
--rw-r--r--   0        0        0     3948 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_definition_request.py
--rw-r--r--   0        0        0     3396 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_field.py
--rw-r--r--   0        0        0     3579 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_field_definition.py
--rw-r--r--   0        0        0     4569 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_id.py
--rw-r--r--   0        0        0     3676 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_request.py
--rw-r--r--   0        0        0     6028 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_response.py
--rw-r--r--   0        0        0     4582 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/custom_entity_type.py
--rw-r--r--   0        0        0     4905 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/cut_label_definition.py
--rw-r--r--   0        0        0     1895 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/cut_local_time.py
--rw-r--r--   0        0        0     5164 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_definition.py
--rw-r--r--   0        0        0     3407 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_map_key.py
--rw-r--r--   0        0        0     3637 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_mapping.py
--rw-r--r--   0        0        0     2324 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_scope.py
--rw-r--r--   0        0        0     7627 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_type.py
--rw-r--r--   0        0        0     6616 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_type_summary.py
--rw-r--r--   0        0        0      722 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/data_type_value_range.py
--rw-r--r--   0        0        0     5794 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/date_attributes.py
--rw-r--r--   0        0        0     2998 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/date_or_diary_entry.py
--rw-r--r--   0        0        0     2176 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/date_range.py
--rw-r--r--   0        0        0      730 2024-05-02 08:39:16.591009 lusid_sdk-2.1.79/lusid/models/date_time_comparison_type.py
--rw-r--r--   0        0        0     5215 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/date_time_compliance_parameter.py
--rw-r--r--   0        0        0     5489 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/date_time_list_compliance_parameter.py
--rw-r--r--   0        0        0     2023 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/day_month.py
--rw-r--r--   0        0        0      756 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/day_of_week.py
--rw-r--r--   0        0        0     5230 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/decimal_compliance_parameter.py
--rw-r--r--   0        0        0     3302 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/decimal_list.py
--rw-r--r--   0        0        0     5481 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/decimal_list_compliance_parameter.py
--rw-r--r--   0        0        0     2830 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/decorated_compliance_run_summary.py
--rw-r--r--   0        0        0     3327 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_accounts_response.py
--rw-r--r--   0        0        0     3992 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_custodian_accounts_response.py
--rw-r--r--   0        0        0     2792 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_instrument_properties_response.py
--rw-r--r--   0        0        0     3136 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_instrument_response.py
--rw-r--r--   0        0        0     3144 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_instruments_response.py
--rw-r--r--   0        0        0      632 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_modes.py
--rw-r--r--   0        0        0     2262 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_relation_request.py
--rw-r--r--   0        0        0     4134 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/delete_relationship_request.py
--rw-r--r--   0        0        0     3643 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/deleted_entity_response.py
--rw-r--r--   0        0        0     3928 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/dependency_source_filter.py
--rw-r--r--   0        0        0     2677 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/described_address_key.py
--rw-r--r--   0        0        0     2995 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/dialect.py
--rw-r--r--   0        0        0     4334 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/dialect_id.py
--rw-r--r--   0        0        0     2368 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/dialect_schema.py
--rw-r--r--   0        0        0     6773 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/diary_entry.py
--rw-r--r--   0        0        0     4564 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/diary_entry_request.py
--rw-r--r--   0        0        0     5522 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/discount_factor_curve_data.py
--rw-r--r--   0        0        0     4377 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/discounting_dependency.py
--rw-r--r--   0        0        0      734 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/discounting_method.py
--rw-r--r--   0        0        0     7454 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/dividend_option_event.py
--rw-r--r--   0        0        0     7340 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/dividend_reinvestment_event.py
--rw-r--r--   0        0        0     6096 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/economic_dependency.py
--rw-r--r--   0        0        0     1290 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/economic_dependency_type.py
--rw-r--r--   0        0        0     3051 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/economic_dependency_with_complex_market_data.py
--rw-r--r--   0        0        0     3358 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/economic_dependency_with_quote.py
--rw-r--r--   0        0        0     2225 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/election_specification.py
--rw-r--r--   0        0        0     2125 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/eligibility_calculation.py
--rw-r--r--   0        0        0     3196 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/empty_model_options.py
--rw-r--r--   0        0        0     2627 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/entity_identifier.py
--rw-r--r--   0        0        0     5752 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/equity.py
--rw-r--r--   0        0        0     3724 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/equity_all_of_identifiers.py
--rw-r--r--   0        0        0     5621 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/equity_curve_by_prices_data.py
--rw-r--r--   0        0        0     5028 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/equity_curve_dependency.py
--rw-r--r--   0        0        0     3698 2024-05-02 08:39:16.593009 lusid_sdk-2.1.79/lusid/models/equity_model_options.py
--rw-r--r--   0        0        0     8709 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/equity_option.py
--rw-r--r--   0        0        0     9341 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/equity_swap.py
--rw-r--r--   0        0        0     4909 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/equity_vol_dependency.py
--rw-r--r--   0        0        0     5865 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/equity_vol_surface_data.py
--rw-r--r--   0        0        0     3279 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/error_detail.py
--rw-r--r--   0        0        0     2252 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/event_date_range.py
--rw-r--r--   0        0        0     3511 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/ex_dividend_configuration.py
--rw-r--r--   0        0        0     6000 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/exchange_traded_option.py
--rw-r--r--   0        0        0     5578 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/exchange_traded_option_contract_details.py
--rw-r--r--   0        0        0     8094 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/execution.py
--rw-r--r--   0        0        0     6720 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/execution_request.py
--rw-r--r--   0        0        0     2672 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/execution_set_request.py
--rw-r--r--   0        0        0     5349 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/exercise_event.py
--rw-r--r--   0        0        0     5705 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/exotic_instrument.py
--rw-r--r--   0        0        0     5931 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/expanded_group.py
--rw-r--r--   0        0        0     4515 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/expiry_event.py
--rw-r--r--   0        0        0     6070 2024-05-02 08:39:16.594009 lusid_sdk-2.1.79/lusid/models/fee_rule.py
--rw-r--r--   0        0        0     6166 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fee_rule_upsert_request.py
--rw-r--r--   0        0        0     3144 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fee_rule_upsert_response.py
--rw-r--r--   0        0        0     2382 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/field_definition.py
--rw-r--r--   0        0        0     4032 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/field_schema.py
--rw-r--r--   0        0        0     2210 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/field_value.py
--rw-r--r--   0        0        0     3006 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/file_response.py
--rw-r--r--   0        0        0     5275 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/filter_predicate_compliance_parameter.py
--rw-r--r--   0        0        0     3857 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/filter_step.py
--rw-r--r--   0        0        0     6618 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fixed_leg.py
--rw-r--r--   0        0        0     2879 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fixed_leg_all_of_overrides.py
--rw-r--r--   0        0        0     7174 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fixed_schedule.py
--rw-r--r--   0        0        0     6252 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/flexible_loan.py
--rw-r--r--   0        0        0     9196 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/float_schedule.py
--rw-r--r--   0        0        0     7558 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/floating_leg.py
--rw-r--r--   0        0        0     2813 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/flow_convention_name.py
--rw-r--r--   0        0        0    10452 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/flow_conventions.py
--rw-r--r--   0        0        0     6589 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/forward_rate_agreement.py
--rw-r--r--   0        0        0     2261 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/from_recipe.py
--rw-r--r--   0        0        0     8478 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fund.py
--rw-r--r--   0        0        0     4242 2024-05-02 08:39:16.595009 lusid_sdk-2.1.79/lusid/models/fund_properties.py
--rw-r--r--   0        0        0     7865 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fund_request.py
--rw-r--r--   0        0        0     6552 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fund_share_class.py
--rw-r--r--   0        0        0     7384 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/funding_leg.py
--rw-r--r--   0        0        0     3515 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/funding_leg_options.py
--rw-r--r--   0        0        0     9013 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/future.py
--rw-r--r--   0        0        0     7336 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/futures_contract_details.py
--rw-r--r--   0        0        0     2612 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_conventions.py
--rw-r--r--   0        0        0     5214 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_dependency.py
--rw-r--r--   0        0        0     8620 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward.py
--rw-r--r--   0        0        0     7865 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_curve_by_quote_reference.py
--rw-r--r--   0        0        0     5758 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_curve_data.py
--rw-r--r--   0        0        0     4864 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_model_options.py
--rw-r--r--   0        0        0     5885 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_pips_curve_data.py
--rw-r--r--   0        0        0     8385 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_settlement_event.py
--rw-r--r--   0        0        0     7547 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_tenor_curve_data.py
--rw-r--r--   0        0        0     7645 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forward_tenor_pips_curve_data.py
--rw-r--r--   0        0        0     5238 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_forwards_dependency.py
--rw-r--r--   0        0        0     5408 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_linked_notional_schedule.py
--rw-r--r--   0        0        0    11849 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_option.py
--rw-r--r--   0        0        0     5183 2024-05-02 08:39:16.596009 lusid_sdk-2.1.79/lusid/models/fx_rate_schedule.py
--rw-r--r--   0        0        0     6948 2024-05-02 08:39:16.592009 lusid_sdk-2.1.79/lusid/models/fx_swap.py
--rw-r--r--   0        0        0     2456 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/fx_tenor_convention.py
--rw-r--r--   0        0        0     4948 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/fx_vol_dependency.py
--rw-r--r--   0        0        0     5832 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/fx_vol_surface_data.py
--rw-r--r--   0        0        0     2723 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/general_ledger_profile_mapping.py
--rw-r--r--   0        0        0     4780 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/general_ledger_profile_request.py
--rw-r--r--   0        0        0     6771 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/general_ledger_profile_response.py
--rw-r--r--   0        0        0     4355 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_cds_flow_conventions_response.py
--rw-r--r--   0        0        0     4940 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_complex_market_data_response.py
--rw-r--r--   0        0        0     4386 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_counterparty_agreement_response.py
--rw-r--r--   0        0        0     4359 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_credit_support_annex_response.py
--rw-r--r--   0        0        0     4832 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_data_map_response.py
--rw-r--r--   0        0        0     4318 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_flow_conventions_response.py
--rw-r--r--   0        0        0     4318 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_index_convention_response.py
--rw-r--r--   0        0        0     4942 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_instruments_response.py
--rw-r--r--   0        0        0     5748 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_quotes_response.py
--rw-r--r--   0        0        0     3323 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_recipe_composer_response.py
--rw-r--r--   0        0        0     3279 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_recipe_response.py
--rw-r--r--   0        0        0     5658 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_reference_portfolio_constituents_response.py
--rw-r--r--   0        0        0     4976 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_structured_result_data_response.py
--rw-r--r--   0        0        0     4912 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/get_virtual_document_response.py
--rw-r--r--   0        0        0     5275 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/group_by_selector_compliance_parameter.py
--rw-r--r--   0        0        0     3865 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/group_by_step.py
--rw-r--r--   0        0        0     5315 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/group_filter_predicate_compliance_parameter.py
--rw-r--r--   0        0        0     4806 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/group_filter_step.py
--rw-r--r--   0        0        0     3322 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/group_of_market_data_key_rules.py
--rw-r--r--   0        0        0     3114 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/grouped_result_of_address_key.py
--rw-r--r--   0        0        0     6451 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holding_adjustment.py
--rw-r--r--   0        0        0     6726 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holding_adjustment_with_date.py
--rw-r--r--   0        0        0     2129 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holding_context.py
--rw-r--r--   0        0        0     2202 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holding_contributor.py
--rw-r--r--   0        0        0     4754 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holdings_adjustment.py
--rw-r--r--   0        0        0     4139 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/holdings_adjustment_header.py
--rw-r--r--   0        0        0     3420 2024-05-02 08:39:16.597009 lusid_sdk-2.1.79/lusid/models/i_unit_definition_dto.py
--rw-r--r--   0        0        0     3158 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/id_selector_definition.py
--rw-r--r--   0        0        0     3083 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/identifier_part_schema.py
--rw-r--r--   0        0        0     5936 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/index_convention.py
--rw-r--r--   0        0        0     3707 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/index_model_options.py
--rw-r--r--   0        0        0     5043 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/index_projection_dependency.py
--rw-r--r--   0        0        0     2860 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/industry_classifier.py
--rw-r--r--   0        0        0     4259 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/inflation_fixing_dependency.py
--rw-r--r--   0        0        0     4811 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inflation_index_conventions.py
--rw-r--r--   0        0        0     9819 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inflation_leg.py
--rw-r--r--   0        0        0    13828 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inflation_linked_bond.py
--rw-r--r--   0        0        0     6839 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inflation_swap.py
--rw-r--r--   0        0        0     4946 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/informational_error_event.py
--rw-r--r--   0        0        0     5959 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/informational_event.py
--rw-r--r--   0        0        0    10449 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inline_valuation_request.py
--rw-r--r--   0        0        0     4749 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/inline_valuations_reconciliation_request.py
--rw-r--r--   0        0        0     2225 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/input_transition.py
--rw-r--r--   0        0        0     8915 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument.py
--rw-r--r--   0        0        0     6377 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_capabilities.py
--rw-r--r--   0        0        0     5438 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_cash_flow.py
--rw-r--r--   0        0        0     4782 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_definition.py
--rw-r--r--   0        0        0     2854 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_definition_format.py
--rw-r--r--   0        0        0      682 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_delete_modes.py
--rw-r--r--   0        0        0     6848 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_event.py
--rw-r--r--   0        0        0     2784 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_event_configuration.py
--rw-r--r--   0        0        0     6994 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_event_holder.py
--rw-r--r--   0        0        0     1698 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_event_type.py
--rw-r--r--   0        0        0     2569 2024-05-02 08:39:16.599009 lusid_sdk-2.1.79/lusid/models/instrument_id_type_descriptor.py
--rw-r--r--   0        0        0     2220 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_id_value.py
--rw-r--r--   0        0        0     5606 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_leg.py
--rw-r--r--   0        0        0     3275 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_list.py
--rw-r--r--   0        0        0     5505 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_list_compliance_parameter.py
--rw-r--r--   0        0        0     3947 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_match.py
--rw-r--r--   0        0        0     3458 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_models.py
--rw-r--r--   0        0        0     5515 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_payment_diary.py
--rw-r--r--   0        0        0     3293 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_payment_diary_leg.py
--rw-r--r--   0        0        0     7048 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_payment_diary_row.py
--rw-r--r--   0        0        0     4302 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_properties.py
--rw-r--r--   0        0        0     3988 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_resolution_detail.py
--rw-r--r--   0        0        0     2297 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_search_property.py
--rw-r--r--   0        0        0     1931 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/instrument_type.py
--rw-r--r--   0        0        0     8820 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/interest_rate_swap.py
--rw-r--r--   0        0        0     6239 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/interest_rate_swaption.py
--rw-r--r--   0        0        0     4403 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/intermediate_compliance_step.py
--rw-r--r--   0        0        0     5867 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/ir_vol_cube_data.py
--rw-r--r--   0        0        0     4523 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/ir_vol_dependency.py
--rw-r--r--   0        0        0     2163 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/is_business_day_response.py
--rw-r--r--   0        0        0    13873 2024-05-02 08:39:16.600009 lusid_sdk-2.1.79/lusid/models/journal_entry_line.py
--rw-r--r--   0        0        0     4647 2024-05-02 08:39:16.580009 lusid_sdk-2.1.79/lusid/models/journal_entry_lines_query_parameters.py
--rw-r--r--   0        0        0     1895 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/label_value_set.py
--rw-r--r--   0        0        0    11100 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/leg_definition.py
--rw-r--r--   0        0        0     8147 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/legal_entity.py
--rw-r--r--   0        0        0     2166 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/level_step.py
--rw-r--r--   0        0        0     3958 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/life_cycle_event_lineage.py
--rw-r--r--   0        0        0     4794 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/life_cycle_event_value.py
--rw-r--r--   0        0        0     3234 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lineage_member.py
--rw-r--r--   0        0        0     2249 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/link.py
--rw-r--r--   0        0        0     3345 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/list_aggregation_reconciliation.py
--rw-r--r--   0        0        0     5412 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/list_aggregation_response.py
--rw-r--r--   0        0        0     3601 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/list_complex_market_data_with_meta_data_response.py
--rw-r--r--   0        0        0     2151 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/loan_period.py
--rw-r--r--   0        0        0     3298 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lock_period_diary_entry_request.py
--rw-r--r--   0        0        0     7466 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lusid_instrument.py
--rw-r--r--   0        0        0     3844 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lusid_problem_details.py
--rw-r--r--   0        0        0     9952 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lusid_trade_ticket.py
--rw-r--r--   0        0        0     2137 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lusid_unique_id.py
--rw-r--r--   0        0        0     4477 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3013 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/mapped_string.py
--rw-r--r--   0        0        0     4180 2024-05-02 08:39:16.601009 lusid_sdk-2.1.79/lusid/models/mapping.py
--rw-r--r--   0        0        0     4965 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/mapping_rule.py
--rw-r--r--   0        0        0     7596 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_context.py
--rw-r--r--   0        0        0     2514 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_context_suppliers.py
--rw-r--r--   0        0        0     9275 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_key_rule.py
--rw-r--r--   0        0        0     3566 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_options.py
--rw-r--r--   0        0        0      697 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_options_type.py
--rw-r--r--   0        0        0     3921 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_overrides.py
--rw-r--r--   0        0        0     8280 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_specific_rule.py
--rw-r--r--   0        0        0     1583 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_data_type.py
--rw-r--r--   0        0        0      801 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_observable_type.py
--rw-r--r--   0        0        0     6247 2024-05-02 08:39:16.598009 lusid_sdk-2.1.79/lusid/models/market_options.py
--rw-r--r--   0        0        0     3145 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/market_quote.py
--rw-r--r--   0        0        0     3568 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/match_criterion.py
--rw-r--r--   0        0        0     4544 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/maturity_event.py
--rw-r--r--   0        0        0     2187 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/metric_value.py
--rw-r--r--   0        0        0     4202 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/model_options.py
--rw-r--r--   0        0        0      931 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/model_options_type.py
--rw-r--r--   0        0        0     3385 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/model_property.py
--rw-r--r--   0        0        0     3861 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/model_schema.py
--rw-r--r--   0        0        0     4086 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/model_selection.py
--rw-r--r--   0        0        0     2568 2024-05-02 08:39:16.602009 lusid_sdk-2.1.79/lusid/models/move_orders_to_different_blocks_request.py
--rw-r--r--   0        0        0     3162 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/moved_order_to_different_block_response.py
--rw-r--r--   0        0        0     1221 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/movement_type.py
--rw-r--r--   0        0        0     2089 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/multi_currency_amounts.py
--rw-r--r--   0        0        0     2718 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/next_value_in_sequence_response.py
--rw-r--r--   0        0        0      772 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/numeric_comparison_type.py
--rw-r--r--   0        0        0     3778 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/opaque_dependency.py
--rw-r--r--   0        0        0     5168 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/opaque_market_data.py
--rw-r--r--   0        0        0     3298 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/opaque_model_options.py
--rw-r--r--   0        0        0     4478 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/open_event.py
--rw-r--r--   0        0        0      648 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/operand_type.py
--rw-r--r--   0        0        0     2546 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/operation.py
--rw-r--r--   0        0        0      622 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/operation_type.py
--rw-r--r--   0        0        0      797 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/operator.py
--rw-r--r--   0        0        0     2136 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/option_entry.py
--rw-r--r--   0        0        0     5425 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/optionality_schedule.py
--rw-r--r--   0        0        0     9659 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order.py
--rw-r--r--   0        0        0     2319 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_by_spec.py
--rw-r--r--   0        0        0     1979 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_flow_configuration.py
--rw-r--r--   0        0        0     5332 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_graph_block.py
--rw-r--r--   0        0        0     2178 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_graph_block_allocation_detail.py
--rw-r--r--   0        0        0     2766 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_graph_block_allocation_synopsis.py
--rw-r--r--   0        0        0     2170 2024-05-02 08:39:16.603009 lusid_sdk-2.1.79/lusid/models/order_graph_block_execution_detail.py
--rw-r--r--   0        0        0     2752 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_execution_synopsis.py
--rw-r--r--   0        0        0     4690 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_order_detail.py
--rw-r--r--   0        0        0     3207 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_order_synopsis.py
--rw-r--r--   0        0        0     2170 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_placement_detail.py
--rw-r--r--   0        0        0     3243 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_placement_synopsis.py
--rw-r--r--   0        0        0     2006 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_transaction_detail.py
--rw-r--r--   0        0        0     2776 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_block_transaction_synopsis.py
--rw-r--r--   0        0        0     5290 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement.py
--rw-r--r--   0        0        0     2210 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_allocation_detail.py
--rw-r--r--   0        0        0     2818 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_allocation_synopsis.py
--rw-r--r--   0        0        0     2242 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_child_placement_detail.py
--rw-r--r--   0        0        0     2202 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_execution_detail.py
--rw-r--r--   0        0        0     2814 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_execution_synopsis.py
--rw-r--r--   0        0        0     2170 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_order_detail.py
--rw-r--r--   0        0        0     2555 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_order_synopsis.py
--rw-r--r--   0        0        0     2830 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_graph_placement_placement_synopsis.py
--rw-r--r--   0        0        0     7187 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_instruction.py
--rw-r--r--   0        0        0     5509 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_instruction_request.py
--rw-r--r--   0        0        0     2764 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_instruction_set_request.py
--rw-r--r--   0        0        0     7833 2024-05-02 08:39:16.604009 lusid_sdk-2.1.79/lusid/models/order_request.py
--rw-r--r--   0        0        0     2716 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/order_set_request.py
--rw-r--r--   0        0        0     2419 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/otc_confirmation.py
--rw-r--r--   0        0        0    13332 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/output_transaction.py
--rw-r--r--   0        0        0     3985 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/output_transition.py
--rw-r--r--   0        0        0     5453 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/package.py
--rw-r--r--   0        0        0     4383 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/package_request.py
--rw-r--r--   0        0        0     2646 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/package_set_request.py
--rw-r--r--   0        0        0     4022 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_abor.py
--rw-r--r--   0        0        0     4179 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_abor_configuration.py
--rw-r--r--   0        0        0     4058 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_account.py
--rw-r--r--   0        0        0     4216 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_address_key_definition.py
--rw-r--r--   0        0        0     4094 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_allocation.py
--rw-r--r--   0        0        0     4204 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_amortisation_rule_set.py
--rw-r--r--   0        0        0     4034 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_block.py
--rw-r--r--   0        0        0     4070 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_calendar.py
--rw-r--r--   0        0        0     4156 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_chart_of_accounts.py
--rw-r--r--   0        0        0     4252 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cleardown_module_response.py
--rw-r--r--   0        0        0     4204 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cleardown_module_rule.py
--rw-r--r--   0        0        0     4240 2024-05-02 08:39:16.605009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_rule_response.py
--rw-r--r--   0        0        0     4205 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_run_info_v2.py
--rw-r--r--   0        0        0     4191 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_template.py
--rw-r--r--   0        0        0     4228 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_corporate_action_source.py
--rw-r--r--   0        0        0     4167 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custodian_account.py
--rw-r--r--   0        0        0     4240 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_definition.py
--rw-r--r--   0        0        0     4216 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_response.py
--rw-r--r--   0        0        0     4168 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_type.py
--rw-r--r--   0        0        0     4192 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cut_label_definition.py
--rw-r--r--   0        0        0     4156 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_data_type_summary.py
--rw-r--r--   0        0        0     4083 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_dialect_id.py
--rw-r--r--   0        0        0     4095 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_diary_entry.py
--rw-r--r--   0        0        0     4082 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_execution.py
--rw-r--r--   0        0        0     4022 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_fund.py
--rw-r--r--   0        0        0     4313 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_general_ledger_profile_response.py
--rw-r--r--   0        0        0     4094 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_instrument.py
--rw-r--r--   0        0        0     4228 2024-05-02 08:39:16.606009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_instrument_event_holder.py
--rw-r--r--   0        0        0     4107 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_legal_entity.py
--rw-r--r--   0        0        0     4034 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order.py
--rw-r--r--   0        0        0     4156 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_graph_block.py
--rw-r--r--   0        0        0     4204 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_graph_placement.py
--rw-r--r--   0        0        0     4167 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_instruction.py
--rw-r--r--   0        0        0     4058 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_package.py
--rw-r--r--   0        0        0     4130 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_participation.py
--rw-r--r--   0        0        0     4046 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_person.py
--rw-r--r--   0        0        0     4082 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_placement.py
--rw-r--r--   0        0        0     4143 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_group.py
--rw-r--r--   0        0        0     4289 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
--rw-r--r--   0        0        0     4228 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_search_result.py
--rw-r--r--   0        0        0     4228 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_posting_module_response.py
--rw-r--r--   0        0        0     4180 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_posting_module_rule.py
--rw-r--r--   0        0        0     4191 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_property_definition.py
--rw-r--r--   0        0        0     4337 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_property_definition_search_result.py
--rw-r--r--   0        0        0     4142 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_reconciliation.py
--rw-r--r--   0        0        0     4228 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_reference_list_response.py
--rw-r--r--   0        0        0     4239 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_relationship_definition.py
--rw-r--r--   0        0        0     4191 2024-05-02 08:39:16.607009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_sequence_definition.py
--rw-r--r--   0        0        0     4144 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_staging_rule_set.py
--rw-r--r--   0        0        0     4203 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_transaction_template.py
--rw-r--r--   0        0        0     4360 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_transaction_template_specification.py
--rw-r--r--   0        0        0     4204 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_translation_script_id.py
--rw-r--r--   0        0        0     4095 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_virtual_row.py
--rw-r--r--   0        0        0     3909 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/participation.py
--rw-r--r--   0        0        0     2858 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/participation_request.py
--rw-r--r--   0        0        0     2724 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/participation_set_request.py
--rw-r--r--   0        0        0     3575 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/performance_return.py
--rw-r--r--   0        0        0     3974 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/performance_returns_metric.py
--rw-r--r--   0        0        0     4527 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/period_diary_entries_reopened_response.py
--rw-r--r--   0        0        0      711 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/period_type.py
--rw-r--r--   0        0        0      713 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/perpetual_entity_state.py
--rw-r--r--   0        0        0     2359 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/perpetual_property.py
--rw-r--r--   0        0        0     6656 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/person.py
--rw-r--r--   0        0        0     2414 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/place_blocks_request.py
--rw-r--r--   0        0        0     9106 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/placement.py
--rw-r--r--   0        0        0     7870 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/placement_request.py
--rw-r--r--   0        0        0     2672 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/placement_set_request.py
--rw-r--r--   0        0        0    12142 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/portfolio.py
--rw-r--r--   0        0        0     8997 2024-05-02 08:39:16.608009 lusid_sdk-2.1.79/lusid/models/portfolio_cash_flow.py
--rw-r--r--   0        0        0     5462 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_cash_ladder.py
--rw-r--r--   0        0        0     9198 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_details.py
--rw-r--r--   0        0        0     4105 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_entity.py
--rw-r--r--   0        0        0     3941 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_entity_id.py
--rw-r--r--   0        0        0     7106 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group.py
--rw-r--r--   0        0        0     5521 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group_id_compliance_parameter.py
--rw-r--r--   0        0        0     3746 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group_id_list.py
--rw-r--r--   0        0        0     5553 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group_id_list_compliance_parameter.py
--rw-r--r--   0        0        0     4343 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group_properties.py
--rw-r--r--   0        0        0     6286 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_group_search_result.py
--rw-r--r--   0        0        0    10562 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_holding.py
--rw-r--r--   0        0        0     5481 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_id_compliance_parameter.py
--rw-r--r--   0        0        0     3706 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_id_list.py
--rw-r--r--   0        0        0     5513 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_id_list_compliance_parameter.py
--rw-r--r--   0        0        0     4292 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_properties.py
--rw-r--r--   0        0        0     2886 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_reconciliation_request.py
--rw-r--r--   0        0        0     6635 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_result_data_key_rule.py
--rw-r--r--   0        0        0     6683 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_return_breakdown.py
--rw-r--r--   0        0        0     6669 2024-05-02 08:39:16.609009 lusid_sdk-2.1.79/lusid/models/portfolio_search_result.py
--rw-r--r--   0        0        0     2780 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/portfolio_trade_ticket.py
--rw-r--r--   0        0        0      712 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/portfolio_type.py
--rw-r--r--   0        0        0    11809 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/portfolio_without_href.py
--rw-r--r--   0        0        0     3001 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/portfolios_reconciliation_request.py
--rw-r--r--   0        0        0     3310 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/posting_module_details.py
--rw-r--r--   0        0        0     4473 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/posting_module_request.py
--rw-r--r--   0        0        0     6104 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/posting_module_response.py
--rw-r--r--   0        0        0     4632 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/posting_module_rule.py
--rw-r--r--   0        0        0     4288 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/posting_module_rules_updated_response.py
--rw-r--r--   0        0        0     2200 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/premium.py
--rw-r--r--   0        0        0     7264 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/pricing_context.py
--rw-r--r--   0        0        0     1447 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/pricing_model.py
--rw-r--r--   0        0        0     7961 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/pricing_options.py
--rw-r--r--   0        0        0     2970 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/processed_command.py
--rw-r--r--   0        0        0    14736 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_definition.py
--rw-r--r--   0        0        0    12851 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_definition_search_result.py
--rw-r--r--   0        0        0      731 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_definition_type.py
--rw-r--r--   0        0        0     2060 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_domain.py
--rw-r--r--   0        0        0     3647 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_filter.py
--rw-r--r--   0        0        0     3221 2024-05-02 08:39:16.610009 lusid_sdk-2.1.79/lusid/models/property_interval.py
--rw-r--r--   0        0        0     5316 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_key_compliance_parameter.py
--rw-r--r--   0        0        0     5513 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_key_list_compliance_parameter.py
--rw-r--r--   0        0        0      681 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_life_time.py
--rw-r--r--   0        0        0     3707 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_list.py
--rw-r--r--   0        0        0     5489 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_list_compliance_parameter.py
--rw-r--r--   0        0        0     3592 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_schema.py
--rw-r--r--   0        0        0      729 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_type.py
--rw-r--r--   0        0        0     3122 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_value.py
--rw-r--r--   0        0        0     3443 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_value_equals.py
--rw-r--r--   0        0        0     3398 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/property_value_in.py
--rw-r--r--   0        0        0    10338 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/query_bucketed_cash_flows_request.py
--rw-r--r--   0        0        0     3986 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/query_cash_flows_request.py
--rw-r--r--   0        0        0     4969 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/query_instrument_events_request.py
--rw-r--r--   0        0        0     4067 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/query_trade_tickets_request.py
--rw-r--r--   0        0        0     8320 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/queryable_key.py
--rw-r--r--   0        0        0     4479 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/quote.py
--rw-r--r--   0        0        0     3179 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/quote_access_metadata_rule.py
--rw-r--r--   0        0        0     6210 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/quote_access_metadata_rule_id.py
--rw-r--r--   0        0        0     4595 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/quote_dependency.py
--rw-r--r--   0        0        0     2419 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/quote_id.py
--rw-r--r--   0        0        0      886 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/quote_instrument_id_type.py
--rw-r--r--   0        0        0     6134 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/quote_series_id.py
--rw-r--r--   0        0        0      958 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/quote_type.py
--rw-r--r--   0        0        0     5358 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/raw_vendor_event.py
--rw-r--r--   0        0        0     2792 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/re_open_period_diary_entry_request.py
--rw-r--r--   0        0        0     7184 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/realised_gain_loss.py
--rw-r--r--   0        0        0     2848 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/recipe_block.py
--rw-r--r--   0        0        0     3703 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/recipe_composer.py
--rw-r--r--   0        0        0     3332 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/recipe_value.py
--rw-r--r--   0        0        0     3881 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/recombine_step.py
--rw-r--r--   0        0        0     4573 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconcile_date_time_rule.py
--rw-r--r--   0        0        0     4606 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconcile_numeric_rule.py
--rw-r--r--   0        0        0     5633 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconcile_string_rule.py
--rw-r--r--   0        0        0     3699 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciled_transaction.py
--rw-r--r--   0        0        0     7603 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation.py
--rw-r--r--   0        0        0     5976 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_break.py
--rw-r--r--   0        0        0     3036 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_configuration.py
--rw-r--r--   0        0        0     2424 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_id.py
--rw-r--r--   0        0        0     2188 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_left_right_address_key_pair.py
--rw-r--r--   0        0        0     3864 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_line.py
--rw-r--r--   0        0        0     6165 2024-05-02 08:39:16.612009 lusid_sdk-2.1.79/lusid/models/reconciliation_request.py
--rw-r--r--   0        0        0     3294 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reconciliation_response.py
--rw-r--r--   0        0        0     4082 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reconciliation_rule.py
--rw-r--r--   0        0        0      856 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reconciliation_rule_type.py
--rw-r--r--   0        0        0     3352 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reconciliation_side_configuration.py
--rw-r--r--   0        0        0     2797 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reconciliation_transactions.py
--rw-r--r--   0        0        0     2927 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_data.py
--rw-r--r--   0        0        0     5288 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_instrument.py
--rw-r--r--   0        0        0     3917 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_list.py
--rw-r--r--   0        0        0     3494 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_list_request.py
--rw-r--r--   0        0        0     4559 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_list_response.py
--rw-r--r--   0        0        0      888 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_list_type.py
--rw-r--r--   0        0        0     4708 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_portfolio_constituent.py
--rw-r--r--   0        0        0     3548 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_portfolio_constituent_request.py
--rw-r--r--   0        0        0      759 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/reference_portfolio_weight_type.py
--rw-r--r--   0        0        0     5522 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/related_entity.py
--rw-r--r--   0        0        0     3418 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/relation.py
--rw-r--r--   0        0        0     6914 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/relation_definition.py
--rw-r--r--   0        0        0     4838 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/relationship.py
--rw-r--r--   0        0        0     6150 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/relationship_definition.py
--rw-r--r--   0        0        0     3016 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/relative_date_offset.py
--rw-r--r--   0        0        0    11323 2024-05-02 08:39:16.613009 lusid_sdk-2.1.79/lusid/models/repo.py
--rw-r--r--   0        0        0     5693 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/reset_event.py
--rw-r--r--   0        0        0     2064 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_id.py
--rw-r--r--   0        0        0     4224 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4395 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_access_metadata_value_of.py
--rw-r--r--   0        0        0     4176 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_address_key_definition.py
--rw-r--r--   0        0        0     4127 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_aggregated_return.py
--rw-r--r--   0        0        0     4127 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_aggregation_query.py
--rw-r--r--   0        0        0     4054 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_allocation.py
--rw-r--r--   0        0        0     3994 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_block.py
--rw-r--r--   0        0        0     4104 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_block_and_orders.py
--rw-r--r--   0        0        0     4079 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_calendar_date.py
--rw-r--r--   0        0        0     4006 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_change.py
--rw-r--r--   0        0        0     4091 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_change_history.py
--rw-r--r--   0        0        0     4261 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_breached_order_info.py
--rw-r--r--   0        0        0     4103 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_rule.py
--rw-r--r--   0        0        0     4176 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_rule_result.py
--rw-r--r--   0        0        0     4140 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_run_info.py
--rw-r--r--   0        0        0     4272 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_constituents_adjustment_header.py
--rw-r--r--   0        0        0     4115 2024-05-02 08:39:16.614009 lusid_sdk-2.1.79/lusid/models/resource_list_of_corporate_action.py
--rw-r--r--   0        0        0     4031 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_data_type.py
--rw-r--r--   0        0        0     4042 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_execution.py
--rw-r--r--   0        0        0     4019 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_fee_rule.py
--rw-r--r--   0        0        0     4286 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_cds_flow_conventions_response.py
--rw-r--r--   0        0        0     4321 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_counterparty_agreement_response.py
--rw-r--r--   0        0        0     4286 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_credit_support_annex_response.py
--rw-r--r--   0        0        0     4249 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_flow_conventions_response.py
--rw-r--r--   0        0        0     4249 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_index_convention_response.py
--rw-r--r--   0        0        0     4237 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_recipe_composer_response.py
--rw-r--r--   0        0        0     4140 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_get_recipe_response.py
--rw-r--r--   0        0        0     4224 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_holdings_adjustment_header.py
--rw-r--r--   0        0        0     4153 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_i_unit_definition_dto.py
--rw-r--r--   0        0        0     4152 2024-05-02 08:39:16.611009 lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_cash_flow.py
--rw-r--r--   0        0        0     4188 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_event_holder.py
--rw-r--r--   0        0        0     4249 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_id_type_descriptor.py
--rw-r--r--   0        0        0     4067 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_legal_entity.py
--rw-r--r--   0        0        0     4433 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py
--rw-r--r--   0        0        0     4018 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_mapping.py
--rw-r--r--   0        0        0     4347 2024-05-02 08:39:16.615009 lusid_sdk-2.1.79/lusid/models/resource_list_of_moved_order_to_different_block_response.py
--rw-r--r--   0        0        0     3994 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_order.py
--rw-r--r--   0        0        0     4127 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_order_instruction.py
--rw-r--r--   0        0        0     4018 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_package.py
--rw-r--r--   0        0        0     4090 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_participation.py
--rw-r--r--   0        0        0     4139 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_performance_return.py
--rw-r--r--   0        0        0     4006 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_person.py
--rw-r--r--   0        0        0     4042 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_placement.py
--rw-r--r--   0        0        0     4042 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio.py
--rw-r--r--   0        0        0     4140 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_cash_flow.py
--rw-r--r--   0        0        0     4164 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_cash_ladder.py
--rw-r--r--   0        0        0     4176 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_trade_ticket.py
--rw-r--r--   0        0        0     4127 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_processed_command.py
--rw-r--r--   0        0        0     4051 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_property.py
--rw-r--r--   0        0        0     4151 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_property_definition.py
--rw-r--r--   0        0        0     4127 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_property_interval.py
--rw-r--r--   0        0        0     4079 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_queryable_key.py
--rw-r--r--   0        0        0     3994 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_quote.py
--rw-r--r--   0        0        0     4213 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_quote_access_metadata_rule.py
--rw-r--r--   0        0        0     4163 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_reconciliation_break.py
--rw-r--r--   0        0        0     4030 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_relation.py
--rw-r--r--   0        0        0     4078 2024-05-02 08:39:16.616009 lusid_sdk-2.1.79/lusid/models/resource_list_of_relationship.py
--rw-r--r--   0        0        0     4115 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_scope_definition.py
--rw-r--r--   0        0        0     4103 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_side_definition.py
--rw-r--r--   0        0        0     3587 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_string.py
--rw-r--r--   0        0        0     4056 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_tax_rule_set.py
--rw-r--r--   0        0        0     4066 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_transaction.py
--rw-r--r--   0        0        0     4115 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_transaction_type.py
--rw-r--r--   0        0        0     3657 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/resource_list_of_value_type.py
--rw-r--r--   0        0        0     3438 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/response_meta_data.py
--rw-r--r--   0        0        0     5434 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_data_key_rule.py
--rw-r--r--   0        0        0     5313 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_data_schema.py
--rw-r--r--   0        0        0     3632 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_key_rule.py
--rw-r--r--   0        0        0      756 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_key_rule_type.py
--rw-r--r--   0        0        0     4898 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value.py
--rw-r--r--   0        0        0     4576 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value0_d.py
--rw-r--r--   0        0        0     3678 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value_bool.py
--rw-r--r--   0        0        0     3893 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value_currency.py
--rw-r--r--   0        0        0     4272 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value_date_time_offset.py
--rw-r--r--   0        0        0     4233 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/result_value_decimal.py
--rw-r--r--   0        0        0     4544 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/result_value_dictionary.py
--rw-r--r--   0        0        0     4173 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/result_value_int.py
--rw-r--r--   0        0        0     3881 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/result_value_string.py
--rw-r--r--   0        0        0     1216 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/result_value_type.py
--rw-r--r--   0        0        0     6187 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/reverse_stock_split_event.py
--rw-r--r--   0        0        0     2297 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/rounding_configuration.py
--rw-r--r--   0        0        0     2111 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/rounding_configuration_component.py
--rw-r--r--   0        0        0     3968 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/rounding_convention.py
--rw-r--r--   0        0        0      699 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/scaling_methodology.py
--rw-r--r--   0        0        0     4032 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/schedule.py
--rw-r--r--   0        0        0      901 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/schedule_type.py
--rw-r--r--   0        0        0     1907 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/scope_definition.py
--rw-r--r--   0        0        0     6145 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/scrip_dividend_event.py
--rw-r--r--   0        0        0     3357 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/script_map_reference.py
--rw-r--r--   0        0        0     3429 2024-05-02 08:39:16.618009 lusid_sdk-2.1.79/lusid/models/security_election.py
--rw-r--r--   0        0        0     4439 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/sequence_definition.py
--rw-r--r--   0        0        0     2945 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_legal_entity_identifiers_request.py
--rw-r--r--   0        0        0     2983 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_legal_entity_properties_request.py
--rw-r--r--   0        0        0     2899 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_person_identifiers_request.py
--rw-r--r--   0        0        0     2697 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_person_properties_request.py
--rw-r--r--   0        0        0     3083 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_share_class_instruments_request.py
--rw-r--r--   0        0        0     2936 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_transaction_configuration_alias.py
--rw-r--r--   0        0        0     4226 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/set_transaction_configuration_source_request.py
--rw-r--r--   0        0        0     3518 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/side_configuration_data.py
--rw-r--r--   0        0        0     2842 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/side_configuration_data_request.py
--rw-r--r--   0        0        0     4149 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/side_definition.py
--rw-r--r--   0        0        0     3310 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/side_definition_request.py
--rw-r--r--   0        0        0     2446 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/sides_definition_request.py
--rw-r--r--   0        0        0     6272 2024-05-02 08:39:16.619009 lusid_sdk-2.1.79/lusid/models/simple_cash_flow_loan.py
--rw-r--r--   0        0        0     6778 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/simple_instrument.py
--rw-r--r--   0        0        0      644 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/sort_order.py
--rw-r--r--   0        0        0     3560 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/staging_rule.py
--rw-r--r--   0        0        0     2687 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/staging_rule_approval_criteria.py
--rw-r--r--   0        0        0     3561 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/staging_rule_match_criteria.py
--rw-r--r--   0        0        0     4196 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/staging_rule_set.py
--rw-r--r--   0        0        0     4504 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/step_schedule.py
--rw-r--r--   0        0        0     6183 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/stock_dividend_event.py
--rw-r--r--   0        0        0     6127 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/stock_split_event.py
--rw-r--r--   0        0        0     2865 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/stream.py
--rw-r--r--   0        0        0      799 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/string_comparison_type.py
--rw-r--r--   0        0        0     5203 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/string_compliance_parameter.py
--rw-r--r--   0        0        0     3243 2024-05-02 08:39:16.620009 lusid_sdk-2.1.79/lusid/models/string_list.py
--rw-r--r--   0        0        0     5473 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/string_list_compliance_parameter.py
--rw-r--r--   0        0        0     3744 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/structured_result_data.py
--rw-r--r--   0        0        0     4411 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/structured_result_data_id.py
--rw-r--r--   0        0        0     3498 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/sub_holding_key_value_equals.py
--rw-r--r--   0        0        0     4296 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/target_tax_lot.py
--rw-r--r--   0        0        0     4290 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/target_tax_lot_request.py
--rw-r--r--   0        0        0     3530 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/tax_rule.py
--rw-r--r--   0        0        0     5007 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/tax_rule_set.py
--rw-r--r--   0        0        0     2339 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/template_field.py
--rw-r--r--   0        0        0     6656 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/term_deposit.py
--rw-r--r--   0        0        0     7051 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/total_return_swap.py
--rw-r--r--   0        0        0     2726 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/touch.py
--rw-r--r--   0        0        0     2320 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/trade_ticket.py
--rw-r--r--   0        0        0      706 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/trade_ticket_type.py
--rw-r--r--   0        0        0    11577 2024-05-02 08:39:16.621009 lusid_sdk-2.1.79/lusid/models/transaction.py
--rw-r--r--   0        0        0     4318 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_configuration_data.py
--rw-r--r--   0        0        0     4398 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_configuration_data_request.py
--rw-r--r--   0        0        0     6984 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_configuration_movement_data.py
--rw-r--r--   0        0        0     6623 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_configuration_movement_data_request.py
--rw-r--r--   0        0        0     4750 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_configuration_type_alias.py
--rw-r--r--   0        0        0     2524 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_currency_and_amount.py
--rw-r--r--   0        0        0     4329 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_field_map.py
--rw-r--r--   0        0        0     2420 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_price.py
--rw-r--r--   0        0        0     2444 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_price_and_type.py
--rw-r--r--   0        0        0      743 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_price_type.py
--rw-r--r--   0        0        0     2607 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_property_map.py
--rw-r--r--   0        0        0     2822 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_property_mapping.py
--rw-r--r--   0        0        0     2877 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_property_mapping_request.py
--rw-r--r--   0        0        0      699 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_query_mode.py
--rw-r--r--   0        0        0     3365 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_query_parameters.py
--rw-r--r--   0        0        0     4294 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_reconciliation_request.py
--rw-r--r--   0        0        0     5946 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_reconciliation_request_v2.py
--rw-r--r--   0        0        0     9335 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_request.py
--rw-r--r--   0        0        0      839 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_roles.py
--rw-r--r--   0        0        0     4411 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_set_configuration_data.py
--rw-r--r--   0        0        0     3947 2024-05-02 08:39:16.622009 lusid_sdk-2.1.79/lusid/models/transaction_set_configuration_data_request.py
--rw-r--r--   0        0        0      700 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_status.py
--rw-r--r--   0        0        0     4175 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_template.py
--rw-r--r--   0        0        0     2874 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_template_request.py
--rw-r--r--   0        0        0     4605 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_template_specification.py
--rw-r--r--   0        0        0     5765 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type.py
--rw-r--r--   0        0        0     3532 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type_alias.py
--rw-r--r--   0        0        0     2451 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type_calculation.py
--rw-r--r--   0        0        0     7324 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type_movement.py
--rw-r--r--   0        0        0     3249 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type_property_mapping.py
--rw-r--r--   0        0        0     5121 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transaction_type_request.py
--rw-r--r--   0        0        0     3083 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transactions_reconciliations_response.py
--rw-r--r--   0        0        0     6703 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/transition_event.py
--rw-r--r--   0        0        0     3576 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_entities_inlined_request.py
--rw-r--r--   0        0        0     3790 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_entities_request.py
--rw-r--r--   0        0        0     4458 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_entities_response.py
--rw-r--r--   0        0        0     3602 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_instrument_definitions_request.py
--rw-r--r--   0        0        0     5063 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_instrument_definitions_response.py
--rw-r--r--   0        0        0     3354 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_trade_ticket_request.py
--rw-r--r--   0        0        0     4984 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translate_trade_tickets_response.py
--rw-r--r--   0        0        0     2507 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translation_context.py
--rw-r--r--   0        0        0     2035 2024-05-02 08:39:16.623009 lusid_sdk-2.1.79/lusid/models/translation_input.py
--rw-r--r--   0        0        0     2747 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/translation_result.py
--rw-r--r--   0        0        0     2684 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/translation_script.py
--rw-r--r--   0        0        0     3279 2024-05-02 08:39:16.617009 lusid_sdk-2.1.79/lusid/models/translation_script_id.py
--rw-r--r--   0        0        0     6216 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/trial_balance.py
--rw-r--r--   0        0        0     4934 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/trial_balance_query_parameters.py
--rw-r--r--   0        0        0     5516 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/trigger_event.py
--rw-r--r--   0        0        0     3908 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/typed_resource_id.py
--rw-r--r--   0        0        0      675 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/unit_schema.py
--rw-r--r--   0        0        0     2154 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/units_ratio.py
--rw-r--r--   0        0        0      870 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/unmatched_holding_method.py
--rw-r--r--   0        0        0     3127 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_amortisation_rule_set_details_request.py
--rw-r--r--   0        0        0     3318 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_calendar_request.py
--rw-r--r--   0        0        0     3640 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_custom_entity_definition_request.py
--rw-r--r--   0        0        0     3592 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_custom_entity_type_request.py
--rw-r--r--   0        0        0     3634 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_cut_label_definition_request.py
--rw-r--r--   0        0        0     4901 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_data_type_request.py
--rw-r--r--   0        0        0     3323 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_derived_property_definition_request.py
--rw-r--r--   0        0        0     3054 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_instrument_identifier_request.py
--rw-r--r--   0        0        0     2454 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_portfolio_group_request.py
--rw-r--r--   0        0        0     2418 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_portfolio_request.py
--rw-r--r--   0        0        0     2575 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_property_definition_request.py
--rw-r--r--   0        0        0     5901 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/update_reconciliation_request.py
--rw-r--r--   0        0        0     3597 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/update_relationship_definition_request.py
--rw-r--r--   0        0        0     3350 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/update_staging_rule_set_request.py
--rw-r--r--   0        0        0     3243 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/update_tax_rule_set_request.py
--rw-r--r--   0        0        0     3889 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/update_unit_request.py
--rw-r--r--   0        0        0     2503 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_cds_flow_conventions_request.py
--rw-r--r--   0        0        0     2830 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_complex_market_data_request.py
--rw-r--r--   0        0        0     5374 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_compliance_rule_request.py
--rw-r--r--   0        0        0     3311 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_compliance_run_summary_request.py
--rw-r--r--   0        0        0     3274 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_compliance_run_summary_result.py
--rw-r--r--   0        0        0     4741 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_corporate_action_request.py
--rw-r--r--   0        0        0     4960 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_corporate_actions_response.py
--rw-r--r--   0        0        0     2548 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_counterparty_agreement_request.py
--rw-r--r--   0        0        0     2531 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_credit_support_annex_request.py
--rw-r--r--   0        0        0     4996 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_custom_entities_response.py
--rw-r--r--   0        0        0     2849 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_custom_entity_access_metadata_request.py
--rw-r--r--   0        0        0     2495 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_dialect_request.py
--rw-r--r--   0        0        0     2431 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_flow_conventions_request.py
--rw-r--r--   0        0        0     2431 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_index_convention_request.py
--rw-r--r--   0        0        0     5820 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_instrument_event_request.py
--rw-r--r--   0        0        0     4985 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_instrument_events_response.py
--rw-r--r--   0        0        0     2825 2024-05-02 08:39:16.625009 lusid_sdk-2.1.79/lusid/models/upsert_instrument_properties_response.py
--rw-r--r--   0        0        0     3347 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_instrument_property_request.py
--rw-r--r--   0        0        0     6089 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_instruments_response.py
--rw-r--r--   0        0        0     4949 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_legal_entities_response.py
--rw-r--r--   0        0        0     2841 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_legal_entity_access_metadata_request.py
--rw-r--r--   0        0        0     5628 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_legal_entity_request.py
--rw-r--r--   0        0        0     2795 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_person_access_metadata_request.py
--rw-r--r--   0        0        0     4278 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_person_request.py
--rw-r--r--   0        0        0     2587 2024-05-02 08:39:16.624009 lusid_sdk-2.1.79/lusid/models/upsert_portfolio_access_metadata_request.py
--rw-r--r--   0        0        0     2633 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_portfolio_group_access_metadata_request.py
--rw-r--r--   0        0        0     4621 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_portfolio_transactions_response.py
--rw-r--r--   0        0        0     3283 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_quote_access_metadata_rule_request.py
--rw-r--r--   0        0        0     4017 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_quote_request.py
--rw-r--r--   0        0        0     4817 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_quotes_response.py
--rw-r--r--   0        0        0     2409 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_recipe_composer_request.py
--rw-r--r--   0        0        0     2423 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_recipe_request.py
--rw-r--r--   0        0        0     4669 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_reference_portfolio_constituents_request.py
--rw-r--r--   0        0        0     3324 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_reference_portfolio_constituents_response.py
--rw-r--r--   0        0        0     3542 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_result_values_data_request.py
--rw-r--r--   0        0        0     4607 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_returns_response.py
--rw-r--r--   0        0        0     3230 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_single_structured_data_response.py
--rw-r--r--   0        0        0     4412 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_structured_data_response.py
--rw-r--r--   0        0        0     2696 2024-05-02 08:39:16.626009 lusid_sdk-2.1.79/lusid/models/upsert_structured_result_data_request.py
--rw-r--r--   0        0        0     4345 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/upsert_transaction_properties_response.py
--rw-r--r--   0        0        0     2417 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/upsert_translation_script_request.py
--rw-r--r--   0        0        0     5323 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/upsert_valuation_point_request.py
--rw-r--r--   0        0        0     2028 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/user.py
--rw-r--r--   0        0        0     2271 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuation_point_data_query_parameters.py
--rw-r--r--   0        0        0     2394 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuation_point_data_request.py
--rw-r--r--   0        0        0     5081 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuation_point_data_response.py
--rw-r--r--   0        0        0    10575 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuation_request.py
--rw-r--r--   0        0        0     6154 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuation_schedule.py
--rw-r--r--   0        0        0     5001 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/valuations_reconciliation_request.py
--rw-r--r--   0        0        0     1241 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/value_type.py
--rw-r--r--   0        0        0     4307 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/vendor_dependency.py
--rw-r--r--   0        0        0      812 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/vendor_library.py
--rw-r--r--   0        0        0     6263 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/vendor_model_rule.py
--rw-r--r--   0        0        0     6496 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/version.py
--rw-r--r--   0        0        0     3584 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/version_summary_dto.py
--rw-r--r--   0        0        0     4522 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_a2_b_data_record.py
--rw-r--r--   0        0        0     4570 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
--rw-r--r--   0        0        0     4580 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_holding_contributor.py
--rw-r--r--   0        0        0     4557 2024-05-02 08:39:16.627009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_journal_entry_line.py
--rw-r--r--   0        0        0     4568 2024-05-02 08:39:16.628009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_output_transaction.py
--rw-r--r--   0        0        0     4556 2024-05-02 08:39:16.628009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_portfolio_holding.py
--rw-r--r--   0        0        0     4495 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_transaction.py
--rw-r--r--   0        0        0     4508 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_trial_balance.py
--rw-r--r--   0        0        0     5579 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py
--rw-r--r--   0        0        0     3256 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/virtual_document.py
--rw-r--r--   0        0        0     2756 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/virtual_document_row.py
--rw-r--r--   0        0        0     3199 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/virtual_row.py
--rw-r--r--   0        0        0     1876 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/warning.py
--rw-r--r--   0        0        0     2315 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/weekend_mask.py
--rw-r--r--   0        0        0     4554 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/weighted_instrument.py
--rw-r--r--   0        0        0     3441 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/weighted_instrument_in_line_lookup_identifiers.py
--rw-r--r--   0        0        0     2543 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/weighted_instruments.py
--rw-r--r--   0        0        0     6330 2024-05-02 08:39:16.629009 lusid_sdk-2.1.79/lusid/models/yield_curve_data.py
--rw-r--r--   0        0        0        0 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/py.typed
--rw-r--r--   0        0        0    10138 2024-05-02 08:39:16.637009 lusid_sdk-2.1.79/lusid/rest.py
--rw-r--r--   0        0        0      791 2024-05-02 08:39:16.688008 lusid_sdk-2.1.79/pyproject.toml
--rw-r--r--   0        0        0   180503 1970-01-01 00:00:00.000000 lusid_sdk-2.1.79/PKG-INFO
+-rw-r--r--   0        0        0   179507 2024-05-02 14:26:01.274234 lusid_sdk-2.1.81/README.md
+-rw-r--r--   0        0        0   104391 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/__init__.py
+-rw-r--r--   0        0        0     5388 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/api/__init__.py
+-rw-r--r--   0        0        0   159655 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/abor_api.py
+-rw-r--r--   0        0        0    64033 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/abor_configuration_api.py
+-rw-r--r--   0        0        0    31640 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/address_key_definition_api.py
+-rw-r--r--   0        0        0    38503 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/aggregation_api.py
+-rw-r--r--   0        0        0    44687 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/allocations_api.py
+-rw-r--r--   0        0        0    54742 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/amortisation_rule_sets_api.py
+-rw-r--r--   0        0        0    23224 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/application_metadata_api.py
+-rw-r--r--   0        0        0    43529 2024-05-02 14:26:01.200235 lusid_sdk-2.1.81/lusid/api/blocks_api.py
+-rw-r--r--   0        0        0   126954 2024-05-02 14:26:01.200235 lusid_sdk-2.1.81/lusid/api/calendars_api.py
+-rw-r--r--   0        0        0   363813 2024-05-02 14:26:01.200235 lusid_sdk-2.1.81/lusid/api/chart_of_accounts_api.py
+-rw-r--r--   0        0        0    48588 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/complex_market_data_api.py
+-rw-r--r--   0        0        0   113825 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/compliance_api.py
+-rw-r--r--   0        0        0   101713 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/configuration_recipe_api.py
+-rw-r--r--   0        0        0   106475 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/conventions_api.py
+-rw-r--r--   0        0        0   102152 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/corporate_action_sources_api.py
+-rw-r--r--   0        0        0    72539 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/counterparties_api.py
+-rw-r--r--   0        0        0   165686 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/custom_entities_api.py
+-rw-r--r--   0        0        0    40849 2024-05-02 14:26:01.201235 lusid_sdk-2.1.81/lusid/api/custom_entity_definitions_api.py
+-rw-r--r--   0        0        0    41503 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/custom_entity_types_api.py
+-rw-r--r--   0        0        0    47049 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/cut_label_definitions_api.py
+-rw-r--r--   0        0        0    77801 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/data_types_api.py
+-rw-r--r--   0        0        0    20227 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/derived_transaction_portfolios_api.py
+-rw-r--r--   0        0        0    21368 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/entities_api.py
+-rw-r--r--   0        0        0    44435 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/executions_api.py
+-rw-r--r--   0        0        0   122388 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/funds_api.py
+-rw-r--r--   0        0        0    81546 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/instrument_event_types_api.py
+-rw-r--r--   0        0        0    45411 2024-05-02 14:26:01.202235 lusid_sdk-2.1.81/lusid/api/instrument_events_api.py
+-rw-r--r--   0        0        0   281333 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/api/instruments_api.py
+-rw-r--r--   0        0        0    96690 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/api/legacy_compliance_api.py
+-rw-r--r--   0        0        0   268154 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/api/legal_entities_api.py
+-rw-r--r--   0        0        0    45280 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/api/order_graph_api.py
+-rw-r--r--   0        0        0    46091 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/api/order_instructions_api.py
+-rw-r--r--   0        0        0    44646 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/order_management_api.py
+-rw-r--r--   0        0        0    43587 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/orders_api.py
+-rw-r--r--   0        0        0    43985 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/packages_api.py
+-rw-r--r--   0        0        0    45263 2024-05-02 14:26:01.199235 lusid_sdk-2.1.81/lusid/api/participations_api.py
+-rw-r--r--   0        0        0   247306 2024-05-02 14:26:01.203235 lusid_sdk-2.1.81/lusid/api/persons_api.py
+-rw-r--r--   0        0        0    45797 2024-05-02 14:26:01.203235 lusid_sdk-2.1.81/lusid/api/placements_api.py
+-rw-r--r--   0        0        0   378953 2024-05-02 14:26:01.203235 lusid_sdk-2.1.81/lusid/api/portfolio_groups_api.py
+-rw-r--r--   0        0        0   366937 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/portfolios_api.py
+-rw-r--r--   0        0        0   140397 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/property_definitions_api.py
+-rw-r--r--   0        0        0    10281 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/queryable_keys_api.py
+-rw-r--r--   0        0        0   115625 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/quotes_api.py
+-rw-r--r--   0        0        0   143284 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/reconciliations_api.py
+-rw-r--r--   0        0        0    39839 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/reference_lists_api.py
+-rw-r--r--   0        0        0    47715 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/reference_portfolio_api.py
+-rw-r--r--   0        0        0    27621 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/relation_definitions_api.py
+-rw-r--r--   0        0        0    22888 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/relations_api.py
+-rw-r--r--   0        0        0    54693 2024-05-02 14:26:01.204235 lusid_sdk-2.1.81/lusid/api/relationship_definitions_api.py
+-rw-r--r--   0        0        0    19986 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/relationships_api.py
+-rw-r--r--   0        0        0    30928 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/schemas_api.py
+-rw-r--r--   0        0        0    16390 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/scopes_api.py
+-rw-r--r--   0        0        0    84048 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/scripted_translation_api.py
+-rw-r--r--   0        0        0    58533 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/search_api.py
+-rw-r--r--   0        0        0    37460 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/sequences_api.py
+-rw-r--r--   0        0        0    49946 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/staging_rule_set_api.py
+-rw-r--r--   0        0        0   112489 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/structured_result_data_api.py
+-rw-r--r--   0        0        0    62054 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/system_configuration_api.py
+-rw-r--r--   0        0        0    50024 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/tax_rule_sets_api.py
+-rw-r--r--   0        0        0   107626 2024-05-02 14:26:01.205235 lusid_sdk-2.1.81/lusid/api/transaction_configuration_api.py
+-rw-r--r--   0        0        0    64512 2024-05-02 14:26:01.206235 lusid_sdk-2.1.81/lusid/api/transaction_fees_api.py
+-rw-r--r--   0        0        0   555070 2024-05-02 14:26:01.206235 lusid_sdk-2.1.81/lusid/api/transaction_portfolios_api.py
+-rw-r--r--   0        0        0    20092 2024-05-02 14:26:01.206235 lusid_sdk-2.1.81/lusid/api/translation_api.py
+-rw-r--r--   0        0        0    30709 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/api_response.py
+-rw-r--r--   0        0        0    14404 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/configuration.py
+-rw-r--r--   0        0        0     5326 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/exceptions.py
+-rw-r--r--   0        0        0      560 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/__init__.py
+-rw-r--r--   0        0        0    30567 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/api_client.py
+-rw-r--r--   0        0        0     9772 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8052 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6760 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12698 2024-05-02 14:26:01.208235 lusid_sdk-2.1.81/lusid/extensions/rest.py
+-rw-r--r--   0        0        0    11564 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-05-02 14:26:01.208235 lusid_sdk-2.1.81/lusid/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3877 2024-05-02 14:26:01.208235 lusid_sdk-2.1.81/lusid/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0    98046 2024-05-02 14:26:01.198235 lusid_sdk-2.1.81/lusid/models/__init__.py
+-rw-r--r--   0        0        0     2947 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/a2_b_breakdown.py
+-rw-r--r--   0        0        0     2725 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/a2_b_category.py
+-rw-r--r--   0        0        0     9737 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/a2_b_data_record.py
+-rw-r--r--   0        0        0    10650 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/a2_b_movement_record.py
+-rw-r--r--   0        0        0     6987 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor.py
+-rw-r--r--   0        0        0     7324 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor_configuration.py
+-rw-r--r--   0        0        0     4373 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor_configuration_properties.py
+-rw-r--r--   0        0        0     6539 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor_configuration_request.py
+-rw-r--r--   0        0        0     4242 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor_properties.py
+-rw-r--r--   0        0        0     5474 2024-05-02 14:26:01.143236 lusid_sdk-2.1.81/lusid/models/abor_request.py
+-rw-r--r--   0        0        0     3863 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4806 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3448 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/access_metadata_operation.py
+-rw-r--r--   0        0        0     2396 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/access_metadata_value.py
+-rw-r--r--   0        0        0     5144 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/account.py
+-rw-r--r--   0        0        0     4272 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/account_properties.py
+-rw-r--r--   0        0        0      837 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/accounting_method.py
+-rw-r--r--   0        0        0     4120 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/accounts_upsert_response.py
+-rw-r--r--   0        0        0     5707 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/accumulation_event.py
+-rw-r--r--   0        0        0     2057 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/action_id.py
+-rw-r--r--   0        0        0     2640 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/add_business_days_to_date_request.py
+-rw-r--r--   0        0        0     2013 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/add_business_days_to_date_response.py
+-rw-r--r--   0        0        0     2534 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/additional_payment.py
+-rw-r--r--   0        0        0     4999 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_definition.py
+-rw-r--r--   0        0        0     5281 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_compliance_parameter.py
+-rw-r--r--   0        0        0     3212 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_definition.py
+-rw-r--r--   0        0        0     2968 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_filter.py
+-rw-r--r--   0        0        0     3275 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_list.py
+-rw-r--r--   0        0        0     5505 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3451 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/address_key_option_definition.py
+-rw-r--r--   0        0        0     4387 2024-05-02 14:26:01.144235 lusid_sdk-2.1.81/lusid/models/adjust_holding.py
+-rw-r--r--   0        0        0     5986 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/adjust_holding_for_date_request.py
+-rw-r--r--   0        0        0     5697 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/adjust_holding_request.py
+-rw-r--r--   0        0        0     3334 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregate_spec.py
+-rw-r--r--   0        0        0     5953 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregated_return.py
+-rw-r--r--   0        0        0     5496 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregated_returns_dispersion_request.py
+-rw-r--r--   0        0        0     7601 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregated_returns_request.py
+-rw-r--r--   0        0        0     4098 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregated_returns_response.py
+-rw-r--r--   0        0        0     5341 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregated_transactions_request.py
+-rw-r--r--   0        0        0     2583 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_context.py
+-rw-r--r--   0        0        0     3190 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_measure_failure_detail.py
+-rw-r--r--   0        0        0     1062 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_op.py
+-rw-r--r--   0        0        0     3128 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_options.py
+-rw-r--r--   0        0        0     8326 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_query.py
+-rw-r--r--   0        0        0      892 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/aggregation_type.py
+-rw-r--r--   0        0        0    11554 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/allocation.py
+-rw-r--r--   0        0        0     9777 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/allocation_request.py
+-rw-r--r--   0        0        0     3454 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/allocation_service_run_response.py
+-rw-r--r--   0        0        0     2851 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/allocation_set_request.py
+-rw-r--r--   0        0        0     5344 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/amortisation_event.py
+-rw-r--r--   0        0        0     3638 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/amortisation_rule.py
+-rw-r--r--   0        0        0     5496 2024-05-02 14:26:01.145235 lusid_sdk-2.1.81/lusid/models/amortisation_rule_set.py
+-rw-r--r--   0        0        0     4347 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/annul_quotes_response.py
+-rw-r--r--   0        0        0     3328 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/annul_single_structured_data_response.py
+-rw-r--r--   0        0        0     4499 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/annul_structured_data_response.py
+-rw-r--r--   0        0        0      793 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/asset_class.py
+-rw-r--r--   0        0        0     2435 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/asset_leg.py
+-rw-r--r--   0        0        0     2745 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/barrier.py
+-rw-r--r--   0        0        0     5886 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/basket.py
+-rw-r--r--   0        0        0     2562 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/basket_identifier.py
+-rw-r--r--   0        0        0     5687 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/batch_adjust_holdings_response.py
+-rw-r--r--   0        0        0     4543 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/batch_upsert_instrument_properties_response.py
+-rw-r--r--   0        0        0     5803 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/batch_upsert_portfolio_transactions_response.py
+-rw-r--r--   0        0        0     4424 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/batch_upsert_property_definition_properties_response.py
+-rw-r--r--   0        0        0     7158 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block.py
+-rw-r--r--   0        0        0     2632 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_and_order_id_request.py
+-rw-r--r--   0        0        0     2573 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_and_orders.py
+-rw-r--r--   0        0        0     2513 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_and_orders_create_request.py
+-rw-r--r--   0        0        0     6319 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_and_orders_request.py
+-rw-r--r--   0        0        0     5797 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_request.py
+-rw-r--r--   0        0        0     2620 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/block_set_request.py
+-rw-r--r--   0        0        0     5839 2024-05-02 14:26:01.146236 lusid_sdk-2.1.81/lusid/models/blocked_order_request.py
+-rw-r--r--   0        0        0    12280 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bond.py
+-rw-r--r--   0        0        0     5121 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bond_coupon_event.py
+-rw-r--r--   0        0        0     4599 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bond_default_event.py
+-rw-r--r--   0        0        0     5156 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bond_principal_event.py
+-rw-r--r--   0        0        0     3719 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/book_transactions_request.py
+-rw-r--r--   0        0        0     3537 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/book_transactions_response.py
+-rw-r--r--   0        0        0     5168 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bool_compliance_parameter.py
+-rw-r--r--   0        0        0     5457 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bool_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3857 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/branch_step.py
+-rw-r--r--   0        0        0    10445 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bucketed_cash_flow_request.py
+-rw-r--r--   0        0        0     5611 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bucketed_cash_flow_response.py
+-rw-r--r--   0        0        0     2100 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/bucketing_schedule.py
+-rw-r--r--   0        0        0     2480 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/calculation_info.py
+-rw-r--r--   0        0        0     3961 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/calendar.py
+-rw-r--r--   0        0        0     3688 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/calendar_date.py
+-rw-r--r--   0        0        0     3871 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/calendar_dependency.py
+-rw-r--r--   0        0        0     5980 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/cap_floor.py
+-rw-r--r--   0        0        0     4182 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/cash_dependency.py
+-rw-r--r--   0        0        0     6410 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/cash_dividend_event.py
+-rw-r--r--   0        0        0     3882 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/cash_election.py
+-rw-r--r--   0        0        0     5119 2024-05-02 14:26:01.147235 lusid_sdk-2.1.81/lusid/models/cash_flow_event.py
+-rw-r--r--   0        0        0     4785 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cash_flow_lineage.py
+-rw-r--r--   0        0        0     5099 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cash_flow_value.py
+-rw-r--r--   0        0        0     4424 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cash_flow_value_set.py
+-rw-r--r--   0        0        0     2285 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cash_ladder_record.py
+-rw-r--r--   0        0        0     5183 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cash_perpetual.py
+-rw-r--r--   0        0        0     8161 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cds_flow_conventions.py
+-rw-r--r--   0        0        0     8115 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cds_index.py
+-rw-r--r--   0        0        0     3213 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cds_protection_detail_specification.py
+-rw-r--r--   0        0        0     5076 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/change.py
+-rw-r--r--   0        0        0     4251 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/change_history.py
+-rw-r--r--   0        0        0      702 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/change_history_action.py
+-rw-r--r--   0        0        0     3837 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/change_item.py
+-rw-r--r--   0        0        0     5391 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/chart_of_accounts.py
+-rw-r--r--   0        0        0     4354 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/chart_of_accounts_properties.py
+-rw-r--r--   0        0        0     4549 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/chart_of_accounts_request.py
+-rw-r--r--   0        0        0     4758 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/check_step.py
+-rw-r--r--   0        0        0     3332 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cleardown_module_details.py
+-rw-r--r--   0        0        0     4507 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cleardown_module_request.py
+-rw-r--r--   0        0        0     6150 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cleardown_module_response.py
+-rw-r--r--   0        0        0     3505 2024-05-02 14:26:01.148235 lusid_sdk-2.1.81/lusid/models/cleardown_module_rule.py
+-rw-r--r--   0        0        0     4316 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/cleardown_module_rules_updated_response.py
+-rw-r--r--   0        0        0     1980 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/client.py
+-rw-r--r--   0        0        0     4801 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/close_event.py
+-rw-r--r--   0        0        0     6413 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/close_period_diary_entry_request.py
+-rw-r--r--   0        0        0     7827 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complete_portfolio.py
+-rw-r--r--   0        0        0     3908 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complete_relation.py
+-rw-r--r--   0        0        0     5168 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complete_relationship.py
+-rw-r--r--   0        0        0     9687 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complex_bond.py
+-rw-r--r--   0        0        0     5865 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complex_market_data.py
+-rw-r--r--   0        0        0     3964 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/complex_market_data_id.py
+-rw-r--r--   0        0        0     2970 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_breached_order_info.py
+-rw-r--r--   0        0        0     8295 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_parameter.py
+-rw-r--r--   0        0        0     2172 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_parameter_type.py
+-rw-r--r--   0        0        0     5581 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule.py
+-rw-r--r--   0        0        0     4285 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_breakdown.py
+-rw-r--r--   0        0        0     3951 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_breakdown_request.py
+-rw-r--r--   0        0        0     6986 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_response.py
+-rw-r--r--   0        0        0     4091 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_result.py
+-rw-r--r--   0        0        0     4937 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_result_detail.py
+-rw-r--r--   0        0        0     2320 2024-05-02 14:26:01.149235 lusid_sdk-2.1.81/lusid/models/compliance_rule_result_portfolio_detail.py
+-rw-r--r--   0        0        0     3061 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_rule_result_v2.py
+-rw-r--r--   0        0        0     7163 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_rule_upsert_request.py
+-rw-r--r--   0        0        0     2503 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_rule_upsert_response.py
+-rw-r--r--   0        0        0     3437 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_run_info.py
+-rw-r--r--   0        0        0     2703 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_run_info_v2.py
+-rw-r--r--   0        0        0     3801 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_step.py
+-rw-r--r--   0        0        0      827 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_step_type.py
+-rw-r--r--   0        0        0     4919 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_summary_rule_result.py
+-rw-r--r--   0        0        0     5038 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_summary_rule_result_request.py
+-rw-r--r--   0        0        0     4039 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_template.py
+-rw-r--r--   0        0        0     2383 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_template_parameter.py
+-rw-r--r--   0        0        0     4961 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compliance_template_variation.py
+-rw-r--r--   0        0        0     3645 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/component_transaction.py
+-rw-r--r--   0        0        0     3350 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/composite_breakdown.py
+-rw-r--r--   0        0        0     5315 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/composite_breakdown_request.py
+-rw-r--r--   0        0        0     3925 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/composite_breakdown_response.py
+-rw-r--r--   0        0        0     6527 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/composite_dispersion.py
+-rw-r--r--   0        0        0     4138 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/composite_dispersion_response.py
+-rw-r--r--   0        0        0     5481 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/compounding.py
+-rw-r--r--   0        0        0     5894 2024-05-02 14:26:01.150236 lusid_sdk-2.1.81/lusid/models/configuration_recipe.py
+-rw-r--r--   0        0        0     5178 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/constant_volatility_surface.py
+-rw-r--r--   0        0        0     3233 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/constituents_adjustment_header.py
+-rw-r--r--   0        0        0     6933 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/contract_for_difference.py
+-rw-r--r--   0        0        0     4151 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action.py
+-rw-r--r--   0        0        0     5011 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action_source.py
+-rw-r--r--   0        0        0     3508 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action_transition.py
+-rw-r--r--   0        0        0     3122 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action_transition_component.py
+-rw-r--r--   0        0        0     2705 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action_transition_component_request.py
+-rw-r--r--   0        0        0     3529 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/corporate_action_transition_request.py
+-rw-r--r--   0        0        0     4158 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/counterparty_agreement.py
+-rw-r--r--   0        0        0     4209 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/counterparty_risk_information.py
+-rw-r--r--   0        0        0     2826 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/counterparty_signatory.py
+-rw-r--r--   0        0        0     2230 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_address_key_definition_request.py
+-rw-r--r--   0        0        0     3478 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_amortisation_rule_set_request.py
+-rw-r--r--   0        0        0     4454 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_calendar_request.py
+-rw-r--r--   0        0        0     4734 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_corporate_action_source_request.py
+-rw-r--r--   0        0        0     3948 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_custom_entity_type_request.py
+-rw-r--r--   0        0        0     3723 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_cut_label_definition_request.py
+-rw-r--r--   0        0        0     2478 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_data_map_request.py
+-rw-r--r--   0        0        0     8058 2024-05-02 14:26:01.151235 lusid_sdk-2.1.81/lusid/models/create_data_type_request.py
+-rw-r--r--   0        0        0     4785 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_date_request.py
+-rw-r--r--   0        0        0     5951 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_derived_property_definition_request.py
+-rw-r--r--   0        0        0    10150 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_derived_transaction_portfolio_request.py
+-rw-r--r--   0        0        0     2364 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_portfolio_details.py
+-rw-r--r--   0        0        0     6132 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_portfolio_group_request.py
+-rw-r--r--   0        0        0     7429 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_property_definition_request.py
+-rw-r--r--   0        0        0     3733 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_recipe_request.py
+-rw-r--r--   0        0        0     6391 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_reconciliation_request.py
+-rw-r--r--   0        0        0     5018 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_reference_portfolio_request.py
+-rw-r--r--   0        0        0     4662 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_relation_definition_request.py
+-rw-r--r--   0        0        0     2202 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_relation_request.py
+-rw-r--r--   0        0        0     6630 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_relationship_definition_request.py
+-rw-r--r--   0        0        0     4060 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_relationship_request.py
+-rw-r--r--   0        0        0     4885 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_sequence_request.py
+-rw-r--r--   0        0        0     3350 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_staging_rule_set_request.py
+-rw-r--r--   0        0        0     3740 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_tax_rule_set_request.py
+-rw-r--r--   0        0        0     2961 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_trade_tickets_response.py
+-rw-r--r--   0        0        0    10893 2024-05-02 14:26:01.152235 lusid_sdk-2.1.81/lusid/models/create_transaction_portfolio_request.py
+-rw-r--r--   0        0        0     3418 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/create_unit_definition.py
+-rw-r--r--   0        0        0     8611 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/credit_default_swap.py
+-rw-r--r--   0        0        0     3088 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/credit_rating.py
+-rw-r--r--   0        0        0     7174 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/credit_spread_curve_data.py
+-rw-r--r--   0        0        0     5420 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/credit_support_annex.py
+-rw-r--r--   0        0        0      772 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/criterion_type.py
+-rw-r--r--   0        0        0     2277 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/currency_and_amount.py
+-rw-r--r--   0        0        0     5131 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/curve_options.py
+-rw-r--r--   0        0        0     5040 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custodian_account.py
+-rw-r--r--   0        0        0     4363 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custodian_account_properties.py
+-rw-r--r--   0        0        0     6711 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custodian_account_request.py
+-rw-r--r--   0        0        0     4382 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custodian_accounts_upsert_response.py
+-rw-r--r--   0        0        0     4624 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_definition.py
+-rw-r--r--   0        0        0     3948 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_definition_request.py
+-rw-r--r--   0        0        0     3396 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_field.py
+-rw-r--r--   0        0        0     3579 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_field_definition.py
+-rw-r--r--   0        0        0     4569 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_id.py
+-rw-r--r--   0        0        0     3676 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_request.py
+-rw-r--r--   0        0        0     6028 2024-05-02 14:26:01.153235 lusid_sdk-2.1.81/lusid/models/custom_entity_response.py
+-rw-r--r--   0        0        0     4582 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/custom_entity_type.py
+-rw-r--r--   0        0        0     4905 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/cut_label_definition.py
+-rw-r--r--   0        0        0     1895 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/cut_local_time.py
+-rw-r--r--   0        0        0     5164 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_definition.py
+-rw-r--r--   0        0        0     3407 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_map_key.py
+-rw-r--r--   0        0        0     3637 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_mapping.py
+-rw-r--r--   0        0        0     2324 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_scope.py
+-rw-r--r--   0        0        0     7627 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_type.py
+-rw-r--r--   0        0        0     6616 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_type_summary.py
+-rw-r--r--   0        0        0      722 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/data_type_value_range.py
+-rw-r--r--   0        0        0     5794 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_attributes.py
+-rw-r--r--   0        0        0     2998 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_or_diary_entry.py
+-rw-r--r--   0        0        0     2176 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_range.py
+-rw-r--r--   0        0        0      730 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_time_comparison_type.py
+-rw-r--r--   0        0        0     5215 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_time_compliance_parameter.py
+-rw-r--r--   0        0        0     5489 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/date_time_list_compliance_parameter.py
+-rw-r--r--   0        0        0     2023 2024-05-02 14:26:01.154235 lusid_sdk-2.1.81/lusid/models/day_month.py
+-rw-r--r--   0        0        0      756 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/day_of_week.py
+-rw-r--r--   0        0        0     5230 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/decimal_compliance_parameter.py
+-rw-r--r--   0        0        0     3302 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/decimal_list.py
+-rw-r--r--   0        0        0     5481 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/decimal_list_compliance_parameter.py
+-rw-r--r--   0        0        0     2830 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/decorated_compliance_run_summary.py
+-rw-r--r--   0        0        0     3327 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_accounts_response.py
+-rw-r--r--   0        0        0     3992 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_custodian_accounts_response.py
+-rw-r--r--   0        0        0     2792 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_instrument_properties_response.py
+-rw-r--r--   0        0        0     3136 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_instrument_response.py
+-rw-r--r--   0        0        0     3144 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_instruments_response.py
+-rw-r--r--   0        0        0      632 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_modes.py
+-rw-r--r--   0        0        0     2262 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_relation_request.py
+-rw-r--r--   0        0        0     4134 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/delete_relationship_request.py
+-rw-r--r--   0        0        0     3643 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     3928 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/dependency_source_filter.py
+-rw-r--r--   0        0        0     2677 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/described_address_key.py
+-rw-r--r--   0        0        0     2995 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/dialect.py
+-rw-r--r--   0        0        0     4334 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/dialect_id.py
+-rw-r--r--   0        0        0     2368 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/dialect_schema.py
+-rw-r--r--   0        0        0     6773 2024-05-02 14:26:01.155235 lusid_sdk-2.1.81/lusid/models/diary_entry.py
+-rw-r--r--   0        0        0     4564 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/diary_entry_request.py
+-rw-r--r--   0        0        0     5522 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/discount_factor_curve_data.py
+-rw-r--r--   0        0        0     4377 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/discounting_dependency.py
+-rw-r--r--   0        0        0      734 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/discounting_method.py
+-rw-r--r--   0        0        0     7454 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/dividend_option_event.py
+-rw-r--r--   0        0        0     7340 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/dividend_reinvestment_event.py
+-rw-r--r--   0        0        0     6096 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/economic_dependency.py
+-rw-r--r--   0        0        0     1290 2024-05-02 14:26:01.156235 lusid_sdk-2.1.81/lusid/models/economic_dependency_type.py
+-rw-r--r--   0        0        0     3051 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/economic_dependency_with_complex_market_data.py
+-rw-r--r--   0        0        0     3358 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/economic_dependency_with_quote.py
+-rw-r--r--   0        0        0     2225 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/election_specification.py
+-rw-r--r--   0        0        0     2125 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/eligibility_calculation.py
+-rw-r--r--   0        0        0     3196 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/empty_model_options.py
+-rw-r--r--   0        0        0     2627 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/entity_identifier.py
+-rw-r--r--   0        0        0     5752 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity.py
+-rw-r--r--   0        0        0     3724 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_all_of_identifiers.py
+-rw-r--r--   0        0        0     5621 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_curve_by_prices_data.py
+-rw-r--r--   0        0        0     5028 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_curve_dependency.py
+-rw-r--r--   0        0        0     3698 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_model_options.py
+-rw-r--r--   0        0        0     8709 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_option.py
+-rw-r--r--   0        0        0     9341 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_swap.py
+-rw-r--r--   0        0        0     4909 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_vol_dependency.py
+-rw-r--r--   0        0        0     5865 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/equity_vol_surface_data.py
+-rw-r--r--   0        0        0     3279 2024-05-02 14:26:01.157235 lusid_sdk-2.1.81/lusid/models/error_detail.py
+-rw-r--r--   0        0        0     2252 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/event_date_range.py
+-rw-r--r--   0        0        0     3511 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/ex_dividend_configuration.py
+-rw-r--r--   0        0        0     6000 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/exchange_traded_option.py
+-rw-r--r--   0        0        0     5578 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/exchange_traded_option_contract_details.py
+-rw-r--r--   0        0        0     8094 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/execution.py
+-rw-r--r--   0        0        0     6720 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/execution_request.py
+-rw-r--r--   0        0        0     2672 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/execution_set_request.py
+-rw-r--r--   0        0        0     5349 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/exercise_event.py
+-rw-r--r--   0        0        0     5705 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/exotic_instrument.py
+-rw-r--r--   0        0        0     5931 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/expanded_group.py
+-rw-r--r--   0        0        0     4515 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/expiry_event.py
+-rw-r--r--   0        0        0     6070 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/fee_rule.py
+-rw-r--r--   0        0        0     6166 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/fee_rule_upsert_request.py
+-rw-r--r--   0        0        0     3144 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/fee_rule_upsert_response.py
+-rw-r--r--   0        0        0     2382 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/field_definition.py
+-rw-r--r--   0        0        0     4032 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/field_schema.py
+-rw-r--r--   0        0        0     2210 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/field_value.py
+-rw-r--r--   0        0        0     3006 2024-05-02 14:26:01.158235 lusid_sdk-2.1.81/lusid/models/file_response.py
+-rw-r--r--   0        0        0     5275 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/filter_predicate_compliance_parameter.py
+-rw-r--r--   0        0        0     3857 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/filter_step.py
+-rw-r--r--   0        0        0     6618 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fixed_leg.py
+-rw-r--r--   0        0        0     2879 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fixed_leg_all_of_overrides.py
+-rw-r--r--   0        0        0     7174 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fixed_schedule.py
+-rw-r--r--   0        0        0     6252 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/flexible_loan.py
+-rw-r--r--   0        0        0     9196 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/float_schedule.py
+-rw-r--r--   0        0        0     7558 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/floating_leg.py
+-rw-r--r--   0        0        0     2813 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/flow_convention_name.py
+-rw-r--r--   0        0        0    10452 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/flow_conventions.py
+-rw-r--r--   0        0        0     6589 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/forward_rate_agreement.py
+-rw-r--r--   0        0        0     2261 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/from_recipe.py
+-rw-r--r--   0        0        0     8478 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fund.py
+-rw-r--r--   0        0        0     4242 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fund_properties.py
+-rw-r--r--   0        0        0     7865 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fund_request.py
+-rw-r--r--   0        0        0     6552 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/fund_share_class.py
+-rw-r--r--   0        0        0     7384 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/funding_leg.py
+-rw-r--r--   0        0        0     3515 2024-05-02 14:26:01.159235 lusid_sdk-2.1.81/lusid/models/funding_leg_options.py
+-rw-r--r--   0        0        0     9013 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/future.py
+-rw-r--r--   0        0        0     7336 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/futures_contract_details.py
+-rw-r--r--   0        0        0     2612 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_conventions.py
+-rw-r--r--   0        0        0     5214 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_dependency.py
+-rw-r--r--   0        0        0     8620 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward.py
+-rw-r--r--   0        0        0     7865 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_curve_by_quote_reference.py
+-rw-r--r--   0        0        0     5758 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_curve_data.py
+-rw-r--r--   0        0        0     4864 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_model_options.py
+-rw-r--r--   0        0        0     5885 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_pips_curve_data.py
+-rw-r--r--   0        0        0     8385 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_settlement_event.py
+-rw-r--r--   0        0        0     7547 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_tenor_curve_data.py
+-rw-r--r--   0        0        0     7645 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forward_tenor_pips_curve_data.py
+-rw-r--r--   0        0        0     5238 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_forwards_dependency.py
+-rw-r--r--   0        0        0     5408 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_linked_notional_schedule.py
+-rw-r--r--   0        0        0    11849 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_option.py
+-rw-r--r--   0        0        0     5183 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_rate_schedule.py
+-rw-r--r--   0        0        0     6948 2024-05-02 14:26:01.160235 lusid_sdk-2.1.81/lusid/models/fx_swap.py
+-rw-r--r--   0        0        0     2456 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/fx_tenor_convention.py
+-rw-r--r--   0        0        0     4948 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/fx_vol_dependency.py
+-rw-r--r--   0        0        0     5832 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/fx_vol_surface_data.py
+-rw-r--r--   0        0        0     2723 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/general_ledger_profile_mapping.py
+-rw-r--r--   0        0        0     4780 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/general_ledger_profile_request.py
+-rw-r--r--   0        0        0     6771 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/general_ledger_profile_response.py
+-rw-r--r--   0        0        0     4355 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_cds_flow_conventions_response.py
+-rw-r--r--   0        0        0     4940 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_complex_market_data_response.py
+-rw-r--r--   0        0        0     4386 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_counterparty_agreement_response.py
+-rw-r--r--   0        0        0     4359 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_credit_support_annex_response.py
+-rw-r--r--   0        0        0     4832 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_data_map_response.py
+-rw-r--r--   0        0        0     4318 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_flow_conventions_response.py
+-rw-r--r--   0        0        0     4318 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_index_convention_response.py
+-rw-r--r--   0        0        0     4942 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_instruments_response.py
+-rw-r--r--   0        0        0     5748 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_quotes_response.py
+-rw-r--r--   0        0        0     3323 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_recipe_composer_response.py
+-rw-r--r--   0        0        0     3279 2024-05-02 14:26:01.161235 lusid_sdk-2.1.81/lusid/models/get_recipe_response.py
+-rw-r--r--   0        0        0     5658 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/get_reference_portfolio_constituents_response.py
+-rw-r--r--   0        0        0     4976 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/get_structured_result_data_response.py
+-rw-r--r--   0        0        0     4912 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/get_virtual_document_response.py
+-rw-r--r--   0        0        0     5275 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/group_by_selector_compliance_parameter.py
+-rw-r--r--   0        0        0     3865 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/group_by_step.py
+-rw-r--r--   0        0        0     5315 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/group_filter_predicate_compliance_parameter.py
+-rw-r--r--   0        0        0     4806 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/group_filter_step.py
+-rw-r--r--   0        0        0     3322 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/group_of_market_data_key_rules.py
+-rw-r--r--   0        0        0     3114 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/grouped_result_of_address_key.py
+-rw-r--r--   0        0        0     6451 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holding_adjustment.py
+-rw-r--r--   0        0        0     6726 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holding_adjustment_with_date.py
+-rw-r--r--   0        0        0     2129 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holding_context.py
+-rw-r--r--   0        0        0     2202 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holding_contributor.py
+-rw-r--r--   0        0        0     4754 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holdings_adjustment.py
+-rw-r--r--   0        0        0     4139 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/holdings_adjustment_header.py
+-rw-r--r--   0        0        0     3420 2024-05-02 14:26:01.162235 lusid_sdk-2.1.81/lusid/models/i_unit_definition_dto.py
+-rw-r--r--   0        0        0     3158 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3083 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     5936 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/index_convention.py
+-rw-r--r--   0        0        0     3707 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/index_model_options.py
+-rw-r--r--   0        0        0     5043 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/index_projection_dependency.py
+-rw-r--r--   0        0        0     2860 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/industry_classifier.py
+-rw-r--r--   0        0        0     4259 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/inflation_fixing_dependency.py
+-rw-r--r--   0        0        0     4811 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/inflation_index_conventions.py
+-rw-r--r--   0        0        0     9819 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/inflation_leg.py
+-rw-r--r--   0        0        0    13828 2024-05-02 14:26:01.163235 lusid_sdk-2.1.81/lusid/models/inflation_linked_bond.py
+-rw-r--r--   0        0        0     6839 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/inflation_swap.py
+-rw-r--r--   0        0        0     4946 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/informational_error_event.py
+-rw-r--r--   0        0        0     5959 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/informational_event.py
+-rw-r--r--   0        0        0    10449 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/inline_valuation_request.py
+-rw-r--r--   0        0        0     4749 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/inline_valuations_reconciliation_request.py
+-rw-r--r--   0        0        0     2225 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/input_transition.py
+-rw-r--r--   0        0        0     8915 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument.py
+-rw-r--r--   0        0        0     6377 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_capabilities.py
+-rw-r--r--   0        0        0     5438 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_cash_flow.py
+-rw-r--r--   0        0        0     4782 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_definition.py
+-rw-r--r--   0        0        0     2854 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_definition_format.py
+-rw-r--r--   0        0        0      682 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_delete_modes.py
+-rw-r--r--   0        0        0     6848 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_event.py
+-rw-r--r--   0        0        0     2784 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_event_configuration.py
+-rw-r--r--   0        0        0     6994 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_event_holder.py
+-rw-r--r--   0        0        0     1698 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_event_type.py
+-rw-r--r--   0        0        0     2569 2024-05-02 14:26:01.164235 lusid_sdk-2.1.81/lusid/models/instrument_id_type_descriptor.py
+-rw-r--r--   0        0        0     2220 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_id_value.py
+-rw-r--r--   0        0        0     5606 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_leg.py
+-rw-r--r--   0        0        0     3275 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_list.py
+-rw-r--r--   0        0        0     5505 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3947 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_match.py
+-rw-r--r--   0        0        0     3458 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_models.py
+-rw-r--r--   0        0        0     5515 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_payment_diary.py
+-rw-r--r--   0        0        0     3293 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_payment_diary_leg.py
+-rw-r--r--   0        0        0     7048 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_payment_diary_row.py
+-rw-r--r--   0        0        0     4302 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_properties.py
+-rw-r--r--   0        0        0     3988 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_resolution_detail.py
+-rw-r--r--   0        0        0     2297 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_search_property.py
+-rw-r--r--   0        0        0     1931 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/instrument_type.py
+-rw-r--r--   0        0        0     8820 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/interest_rate_swap.py
+-rw-r--r--   0        0        0     6239 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/interest_rate_swaption.py
+-rw-r--r--   0        0        0     4403 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/intermediate_compliance_step.py
+-rw-r--r--   0        0        0     5867 2024-05-02 14:26:01.165235 lusid_sdk-2.1.81/lusid/models/ir_vol_cube_data.py
+-rw-r--r--   0        0        0     4523 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/ir_vol_dependency.py
+-rw-r--r--   0        0        0     2163 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/is_business_day_response.py
+-rw-r--r--   0        0        0    13873 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/journal_entry_line.py
+-rw-r--r--   0        0        0     4647 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/journal_entry_lines_query_parameters.py
+-rw-r--r--   0        0        0     1895 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/label_value_set.py
+-rw-r--r--   0        0        0    11100 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/leg_definition.py
+-rw-r--r--   0        0        0     8147 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/legal_entity.py
+-rw-r--r--   0        0        0     2166 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/level_step.py
+-rw-r--r--   0        0        0     3958 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/life_cycle_event_lineage.py
+-rw-r--r--   0        0        0     4794 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/life_cycle_event_value.py
+-rw-r--r--   0        0        0     3234 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/lineage_member.py
+-rw-r--r--   0        0        0     2249 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/link.py
+-rw-r--r--   0        0        0     3345 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/list_aggregation_reconciliation.py
+-rw-r--r--   0        0        0     5412 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/list_aggregation_response.py
+-rw-r--r--   0        0        0     3601 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/list_complex_market_data_with_meta_data_response.py
+-rw-r--r--   0        0        0     2151 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/loan_period.py
+-rw-r--r--   0        0        0     3298 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/lock_period_diary_entry_request.py
+-rw-r--r--   0        0        0     7466 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/lusid_instrument.py
+-rw-r--r--   0        0        0     3844 2024-05-02 14:26:01.166235 lusid_sdk-2.1.81/lusid/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     9952 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/lusid_trade_ticket.py
+-rw-r--r--   0        0        0     2137 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/lusid_unique_id.py
+-rw-r--r--   0        0        0     4477 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3013 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/mapped_string.py
+-rw-r--r--   0        0        0     4180 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/mapping.py
+-rw-r--r--   0        0        0     4965 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/mapping_rule.py
+-rw-r--r--   0        0        0     7596 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_context.py
+-rw-r--r--   0        0        0     2514 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_context_suppliers.py
+-rw-r--r--   0        0        0     9275 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_key_rule.py
+-rw-r--r--   0        0        0     3566 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_options.py
+-rw-r--r--   0        0        0      697 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_options_type.py
+-rw-r--r--   0        0        0     3921 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_overrides.py
+-rw-r--r--   0        0        0     8280 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_specific_rule.py
+-rw-r--r--   0        0        0     1583 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_data_type.py
+-rw-r--r--   0        0        0      801 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_observable_type.py
+-rw-r--r--   0        0        0     6247 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_options.py
+-rw-r--r--   0        0        0     3145 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/market_quote.py
+-rw-r--r--   0        0        0     3568 2024-05-02 14:26:01.167235 lusid_sdk-2.1.81/lusid/models/match_criterion.py
+-rw-r--r--   0        0        0     4544 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/maturity_event.py
+-rw-r--r--   0        0        0     2187 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/metric_value.py
+-rw-r--r--   0        0        0     4202 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/model_options.py
+-rw-r--r--   0        0        0      931 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/model_options_type.py
+-rw-r--r--   0        0        0     3385 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/model_property.py
+-rw-r--r--   0        0        0     3861 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/model_schema.py
+-rw-r--r--   0        0        0     4086 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/model_selection.py
+-rw-r--r--   0        0        0     2568 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/move_orders_to_different_blocks_request.py
+-rw-r--r--   0        0        0     3162 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/moved_order_to_different_block_response.py
+-rw-r--r--   0        0        0     1221 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/movement_type.py
+-rw-r--r--   0        0        0     2089 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/multi_currency_amounts.py
+-rw-r--r--   0        0        0     2718 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/next_value_in_sequence_response.py
+-rw-r--r--   0        0        0      772 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/numeric_comparison_type.py
+-rw-r--r--   0        0        0     3778 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/opaque_dependency.py
+-rw-r--r--   0        0        0     5168 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/opaque_market_data.py
+-rw-r--r--   0        0        0     3298 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/opaque_model_options.py
+-rw-r--r--   0        0        0     4478 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/open_event.py
+-rw-r--r--   0        0        0      648 2024-05-02 14:26:01.168235 lusid_sdk-2.1.81/lusid/models/operand_type.py
+-rw-r--r--   0        0        0     2546 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/operation.py
+-rw-r--r--   0        0        0      622 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/operation_type.py
+-rw-r--r--   0        0        0      797 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/operator.py
+-rw-r--r--   0        0        0     2136 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/option_entry.py
+-rw-r--r--   0        0        0     5425 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/optionality_schedule.py
+-rw-r--r--   0        0        0     9659 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order.py
+-rw-r--r--   0        0        0     2319 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_by_spec.py
+-rw-r--r--   0        0        0     1979 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_flow_configuration.py
+-rw-r--r--   0        0        0     5332 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block.py
+-rw-r--r--   0        0        0     2178 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block_allocation_detail.py
+-rw-r--r--   0        0        0     2766 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block_allocation_synopsis.py
+-rw-r--r--   0        0        0     2170 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block_execution_detail.py
+-rw-r--r--   0        0        0     2752 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block_execution_synopsis.py
+-rw-r--r--   0        0        0     4690 2024-05-02 14:26:01.169235 lusid_sdk-2.1.81/lusid/models/order_graph_block_order_detail.py
+-rw-r--r--   0        0        0     3207 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_block_order_synopsis.py
+-rw-r--r--   0        0        0     2170 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_block_placement_detail.py
+-rw-r--r--   0        0        0     3243 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_block_placement_synopsis.py
+-rw-r--r--   0        0        0     2006 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_block_transaction_detail.py
+-rw-r--r--   0        0        0     2776 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_block_transaction_synopsis.py
+-rw-r--r--   0        0        0     5290 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement.py
+-rw-r--r--   0        0        0     2210 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_allocation_detail.py
+-rw-r--r--   0        0        0     2818 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_allocation_synopsis.py
+-rw-r--r--   0        0        0     2242 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_child_placement_detail.py
+-rw-r--r--   0        0        0     2202 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_execution_detail.py
+-rw-r--r--   0        0        0     2814 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_execution_synopsis.py
+-rw-r--r--   0        0        0     2170 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_order_detail.py
+-rw-r--r--   0        0        0     2555 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_order_synopsis.py
+-rw-r--r--   0        0        0     2830 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_graph_placement_placement_synopsis.py
+-rw-r--r--   0        0        0     7187 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_instruction.py
+-rw-r--r--   0        0        0     5509 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_instruction_request.py
+-rw-r--r--   0        0        0     2764 2024-05-02 14:26:01.170235 lusid_sdk-2.1.81/lusid/models/order_instruction_set_request.py
+-rw-r--r--   0        0        0     7833 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/order_request.py
+-rw-r--r--   0        0        0     2716 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/order_set_request.py
+-rw-r--r--   0        0        0     2419 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/otc_confirmation.py
+-rw-r--r--   0        0        0    13905 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/output_transaction.py
+-rw-r--r--   0        0        0     3985 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/output_transition.py
+-rw-r--r--   0        0        0     5453 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/package.py
+-rw-r--r--   0        0        0     4383 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/package_request.py
+-rw-r--r--   0        0        0     2646 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/package_set_request.py
+-rw-r--r--   0        0        0     4022 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_abor.py
+-rw-r--r--   0        0        0     4179 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_abor_configuration.py
+-rw-r--r--   0        0        0     4058 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_account.py
+-rw-r--r--   0        0        0     4216 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_address_key_definition.py
+-rw-r--r--   0        0        0     4094 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_allocation.py
+-rw-r--r--   0        0        0     4204 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_amortisation_rule_set.py
+-rw-r--r--   0        0        0     4034 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_block.py
+-rw-r--r--   0        0        0     4070 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_calendar.py
+-rw-r--r--   0        0        0     4156 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_chart_of_accounts.py
+-rw-r--r--   0        0        0     4252 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cleardown_module_response.py
+-rw-r--r--   0        0        0     4204 2024-05-02 14:26:01.171235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cleardown_module_rule.py
+-rw-r--r--   0        0        0     4240 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_rule_response.py
+-rw-r--r--   0        0        0     4205 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_run_info_v2.py
+-rw-r--r--   0        0        0     4191 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_template.py
+-rw-r--r--   0        0        0     4228 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_corporate_action_source.py
+-rw-r--r--   0        0        0     4167 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custodian_account.py
+-rw-r--r--   0        0        0     4240 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_definition.py
+-rw-r--r--   0        0        0     4216 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_response.py
+-rw-r--r--   0        0        0     4168 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_type.py
+-rw-r--r--   0        0        0     4192 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cut_label_definition.py
+-rw-r--r--   0        0        0     4156 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_data_type_summary.py
+-rw-r--r--   0        0        0     4083 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_dialect_id.py
+-rw-r--r--   0        0        0     4095 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_diary_entry.py
+-rw-r--r--   0        0        0     4082 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_execution.py
+-rw-r--r--   0        0        0     4022 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_fund.py
+-rw-r--r--   0        0        0     4313 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_general_ledger_profile_response.py
+-rw-r--r--   0        0        0     4094 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_instrument.py
+-rw-r--r--   0        0        0     4228 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_instrument_event_holder.py
+-rw-r--r--   0        0        0     4107 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_legal_entity.py
+-rw-r--r--   0        0        0     4034 2024-05-02 14:26:01.172235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order.py
+-rw-r--r--   0        0        0     4156 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_graph_block.py
+-rw-r--r--   0        0        0     4204 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_graph_placement.py
+-rw-r--r--   0        0        0     4167 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_instruction.py
+-rw-r--r--   0        0        0     4058 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_package.py
+-rw-r--r--   0        0        0     4130 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_participation.py
+-rw-r--r--   0        0        0     4046 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_person.py
+-rw-r--r--   0        0        0     4082 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_placement.py
+-rw-r--r--   0        0        0     4143 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_group.py
+-rw-r--r--   0        0        0     4289 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_group_search_result.py
+-rw-r--r--   0        0        0     4228 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_search_result.py
+-rw-r--r--   0        0        0     4228 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_posting_module_response.py
+-rw-r--r--   0        0        0     4180 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_posting_module_rule.py
+-rw-r--r--   0        0        0     4191 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_property_definition.py
+-rw-r--r--   0        0        0     4337 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_property_definition_search_result.py
+-rw-r--r--   0        0        0     4142 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_reconciliation.py
+-rw-r--r--   0        0        0     4228 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_reference_list_response.py
+-rw-r--r--   0        0        0     4239 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_relationship_definition.py
+-rw-r--r--   0        0        0     4191 2024-05-02 14:26:01.173235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_sequence_definition.py
+-rw-r--r--   0        0        0     4144 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_staging_rule_set.py
+-rw-r--r--   0        0        0     4203 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_transaction_template.py
+-rw-r--r--   0        0        0     4360 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_transaction_template_specification.py
+-rw-r--r--   0        0        0     4204 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_translation_script_id.py
+-rw-r--r--   0        0        0     4095 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_virtual_row.py
+-rw-r--r--   0        0        0     3909 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/participation.py
+-rw-r--r--   0        0        0     2858 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/participation_request.py
+-rw-r--r--   0        0        0     2724 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/participation_set_request.py
+-rw-r--r--   0        0        0     3575 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/performance_return.py
+-rw-r--r--   0        0        0     3974 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/performance_returns_metric.py
+-rw-r--r--   0        0        0     4527 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/period_diary_entries_reopened_response.py
+-rw-r--r--   0        0        0      711 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/period_type.py
+-rw-r--r--   0        0        0      713 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/perpetual_entity_state.py
+-rw-r--r--   0        0        0     2359 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/perpetual_property.py
+-rw-r--r--   0        0        0     6656 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/person.py
+-rw-r--r--   0        0        0     2414 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/place_blocks_request.py
+-rw-r--r--   0        0        0     9106 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/placement.py
+-rw-r--r--   0        0        0     7870 2024-05-02 14:26:01.174235 lusid_sdk-2.1.81/lusid/models/placement_request.py
+-rw-r--r--   0        0        0     2672 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/placement_set_request.py
+-rw-r--r--   0        0        0    12142 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/portfolio.py
+-rw-r--r--   0        0        0     8997 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/portfolio_cash_flow.py
+-rw-r--r--   0        0        0     5462 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/portfolio_cash_ladder.py
+-rw-r--r--   0        0        0     9198 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/portfolio_details.py
+-rw-r--r--   0        0        0     4672 2024-05-02 14:26:01.175235 lusid_sdk-2.1.81/lusid/models/portfolio_entity.py
+-rw-r--r--   0        0        0     3941 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_entity_id.py
+-rw-r--r--   0        0        0     7106 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group.py
+-rw-r--r--   0        0        0     5521 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group_id_compliance_parameter.py
+-rw-r--r--   0        0        0     3746 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group_id_list.py
+-rw-r--r--   0        0        0     5553 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group_id_list_compliance_parameter.py
+-rw-r--r--   0        0        0     4343 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group_properties.py
+-rw-r--r--   0        0        0     6286 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_group_search_result.py
+-rw-r--r--   0        0        0    10562 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_holding.py
+-rw-r--r--   0        0        0     5481 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_id_compliance_parameter.py
+-rw-r--r--   0        0        0     3706 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_id_list.py
+-rw-r--r--   0        0        0     5513 2024-05-02 14:26:01.176235 lusid_sdk-2.1.81/lusid/models/portfolio_id_list_compliance_parameter.py
+-rw-r--r--   0        0        0     4292 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_properties.py
+-rw-r--r--   0        0        0     2886 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_reconciliation_request.py
+-rw-r--r--   0        0        0     6635 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_result_data_key_rule.py
+-rw-r--r--   0        0        0     6683 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_return_breakdown.py
+-rw-r--r--   0        0        0     6669 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_search_result.py
+-rw-r--r--   0        0        0     2780 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_trade_ticket.py
+-rw-r--r--   0        0        0      712 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_type.py
+-rw-r--r--   0        0        0    11809 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolio_without_href.py
+-rw-r--r--   0        0        0     3001 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/portfolios_reconciliation_request.py
+-rw-r--r--   0        0        0     3310 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/posting_module_details.py
+-rw-r--r--   0        0        0     4473 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/posting_module_request.py
+-rw-r--r--   0        0        0     6104 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/posting_module_response.py
+-rw-r--r--   0        0        0     4632 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/posting_module_rule.py
+-rw-r--r--   0        0        0     4288 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/posting_module_rules_updated_response.py
+-rw-r--r--   0        0        0     2200 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/premium.py
+-rw-r--r--   0        0        0     7264 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/pricing_context.py
+-rw-r--r--   0        0        0     1447 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/pricing_model.py
+-rw-r--r--   0        0        0     7961 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/pricing_options.py
+-rw-r--r--   0        0        0     2970 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/processed_command.py
+-rw-r--r--   0        0        0    14736 2024-05-02 14:26:01.177235 lusid_sdk-2.1.81/lusid/models/property_definition.py
+-rw-r--r--   0        0        0    12851 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_definition_search_result.py
+-rw-r--r--   0        0        0      731 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_definition_type.py
+-rw-r--r--   0        0        0     2060 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_domain.py
+-rw-r--r--   0        0        0     3647 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_filter.py
+-rw-r--r--   0        0        0     3221 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_interval.py
+-rw-r--r--   0        0        0     5316 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_key_compliance_parameter.py
+-rw-r--r--   0        0        0     5513 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_key_list_compliance_parameter.py
+-rw-r--r--   0        0        0      681 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_life_time.py
+-rw-r--r--   0        0        0     3707 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_list.py
+-rw-r--r--   0        0        0     5489 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3592 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_schema.py
+-rw-r--r--   0        0        0      729 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_type.py
+-rw-r--r--   0        0        0     3122 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_value.py
+-rw-r--r--   0        0        0     3443 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_value_equals.py
+-rw-r--r--   0        0        0     3398 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/property_value_in.py
+-rw-r--r--   0        0        0    10338 2024-05-02 14:26:01.178235 lusid_sdk-2.1.81/lusid/models/query_bucketed_cash_flows_request.py
+-rw-r--r--   0        0        0     3986 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/query_cash_flows_request.py
+-rw-r--r--   0        0        0     4969 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/query_instrument_events_request.py
+-rw-r--r--   0        0        0     4067 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/query_trade_tickets_request.py
+-rw-r--r--   0        0        0     8320 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/queryable_key.py
+-rw-r--r--   0        0        0     4479 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote.py
+-rw-r--r--   0        0        0     3179 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_access_metadata_rule.py
+-rw-r--r--   0        0        0     6210 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_access_metadata_rule_id.py
+-rw-r--r--   0        0        0     4595 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_dependency.py
+-rw-r--r--   0        0        0     2419 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_id.py
+-rw-r--r--   0        0        0      886 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_instrument_id_type.py
+-rw-r--r--   0        0        0     6134 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_series_id.py
+-rw-r--r--   0        0        0      958 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/quote_type.py
+-rw-r--r--   0        0        0     5358 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/raw_vendor_event.py
+-rw-r--r--   0        0        0     2792 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/re_open_period_diary_entry_request.py
+-rw-r--r--   0        0        0     7184 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/realised_gain_loss.py
+-rw-r--r--   0        0        0     2848 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/recipe_block.py
+-rw-r--r--   0        0        0     3703 2024-05-02 14:26:01.179235 lusid_sdk-2.1.81/lusid/models/recipe_composer.py
+-rw-r--r--   0        0        0     3332 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/recipe_value.py
+-rw-r--r--   0        0        0     3881 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/recombine_step.py
+-rw-r--r--   0        0        0     4573 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconcile_date_time_rule.py
+-rw-r--r--   0        0        0     4606 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconcile_numeric_rule.py
+-rw-r--r--   0        0        0     5633 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconcile_string_rule.py
+-rw-r--r--   0        0        0     3699 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciled_transaction.py
+-rw-r--r--   0        0        0     7603 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation.py
+-rw-r--r--   0        0        0     5976 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation_break.py
+-rw-r--r--   0        0        0     3036 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation_configuration.py
+-rw-r--r--   0        0        0     2424 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation_id.py
+-rw-r--r--   0        0        0     2188 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation_left_right_address_key_pair.py
+-rw-r--r--   0        0        0     3864 2024-05-02 14:26:01.180235 lusid_sdk-2.1.81/lusid/models/reconciliation_line.py
+-rw-r--r--   0        0        0     6165 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_request.py
+-rw-r--r--   0        0        0     3294 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_response.py
+-rw-r--r--   0        0        0     4082 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_rule.py
+-rw-r--r--   0        0        0      856 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_rule_type.py
+-rw-r--r--   0        0        0     3352 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_side_configuration.py
+-rw-r--r--   0        0        0     2797 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reconciliation_transactions.py
+-rw-r--r--   0        0        0     2927 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_data.py
+-rw-r--r--   0        0        0     5288 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_instrument.py
+-rw-r--r--   0        0        0     3917 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_list.py
+-rw-r--r--   0        0        0     3494 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_list_request.py
+-rw-r--r--   0        0        0     4559 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_list_response.py
+-rw-r--r--   0        0        0      888 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_list_type.py
+-rw-r--r--   0        0        0     4708 2024-05-02 14:26:01.181235 lusid_sdk-2.1.81/lusid/models/reference_portfolio_constituent.py
+-rw-r--r--   0        0        0     3548 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/reference_portfolio_constituent_request.py
+-rw-r--r--   0        0        0      759 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/reference_portfolio_weight_type.py
+-rw-r--r--   0        0        0     5522 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/related_entity.py
+-rw-r--r--   0        0        0     3418 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/relation.py
+-rw-r--r--   0        0        0     6914 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/relation_definition.py
+-rw-r--r--   0        0        0     4838 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/relationship.py
+-rw-r--r--   0        0        0     6150 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/relationship_definition.py
+-rw-r--r--   0        0        0     3016 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/relative_date_offset.py
+-rw-r--r--   0        0        0    11323 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/repo.py
+-rw-r--r--   0        0        0     5693 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/reset_event.py
+-rw-r--r--   0        0        0     2064 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/resource_id.py
+-rw-r--r--   0        0        0     4224 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4395 2024-05-02 14:26:01.182235 lusid_sdk-2.1.81/lusid/models/resource_list_of_access_metadata_value_of.py
+-rw-r--r--   0        0        0     4176 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_address_key_definition.py
+-rw-r--r--   0        0        0     4127 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_aggregated_return.py
+-rw-r--r--   0        0        0     4127 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_aggregation_query.py
+-rw-r--r--   0        0        0     4054 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_allocation.py
+-rw-r--r--   0        0        0     3994 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_block.py
+-rw-r--r--   0        0        0     4104 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_block_and_orders.py
+-rw-r--r--   0        0        0     4079 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_calendar_date.py
+-rw-r--r--   0        0        0     4006 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_change.py
+-rw-r--r--   0        0        0     4091 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_change_history.py
+-rw-r--r--   0        0        0     4261 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_breached_order_info.py
+-rw-r--r--   0        0        0     4103 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_rule.py
+-rw-r--r--   0        0        0     4176 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_rule_result.py
+-rw-r--r--   0        0        0     4140 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_run_info.py
+-rw-r--r--   0        0        0     4272 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_constituents_adjustment_header.py
+-rw-r--r--   0        0        0     4115 2024-05-02 14:26:01.183235 lusid_sdk-2.1.81/lusid/models/resource_list_of_corporate_action.py
+-rw-r--r--   0        0        0     4031 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_data_type.py
+-rw-r--r--   0        0        0     4042 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_execution.py
+-rw-r--r--   0        0        0     4019 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_fee_rule.py
+-rw-r--r--   0        0        0     4286 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_cds_flow_conventions_response.py
+-rw-r--r--   0        0        0     4321 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_counterparty_agreement_response.py
+-rw-r--r--   0        0        0     4286 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_credit_support_annex_response.py
+-rw-r--r--   0        0        0     4249 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_flow_conventions_response.py
+-rw-r--r--   0        0        0     4249 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_index_convention_response.py
+-rw-r--r--   0        0        0     4237 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_recipe_composer_response.py
+-rw-r--r--   0        0        0     4140 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_get_recipe_response.py
+-rw-r--r--   0        0        0     4224 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_holdings_adjustment_header.py
+-rw-r--r--   0        0        0     4153 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_i_unit_definition_dto.py
+-rw-r--r--   0        0        0     4152 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_cash_flow.py
+-rw-r--r--   0        0        0     4188 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_event_holder.py
+-rw-r--r--   0        0        0     4249 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_id_type_descriptor.py
+-rw-r--r--   0        0        0     4067 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_legal_entity.py
+-rw-r--r--   0        0        0     4433 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py
+-rw-r--r--   0        0        0     4018 2024-05-02 14:26:01.184235 lusid_sdk-2.1.81/lusid/models/resource_list_of_mapping.py
+-rw-r--r--   0        0        0     4347 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_moved_order_to_different_block_response.py
+-rw-r--r--   0        0        0     3994 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_order.py
+-rw-r--r--   0        0        0     4127 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_order_instruction.py
+-rw-r--r--   0        0        0     4018 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_package.py
+-rw-r--r--   0        0        0     4090 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_participation.py
+-rw-r--r--   0        0        0     4139 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_performance_return.py
+-rw-r--r--   0        0        0     4006 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_person.py
+-rw-r--r--   0        0        0     4042 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_placement.py
+-rw-r--r--   0        0        0     4042 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio.py
+-rw-r--r--   0        0        0     4140 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_cash_flow.py
+-rw-r--r--   0        0        0     4164 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_cash_ladder.py
+-rw-r--r--   0        0        0     4176 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_trade_ticket.py
+-rw-r--r--   0        0        0     4127 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_processed_command.py
+-rw-r--r--   0        0        0     4051 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_property.py
+-rw-r--r--   0        0        0     4151 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_property_definition.py
+-rw-r--r--   0        0        0     4127 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_property_interval.py
+-rw-r--r--   0        0        0     4079 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_queryable_key.py
+-rw-r--r--   0        0        0     3994 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_quote.py
+-rw-r--r--   0        0        0     4213 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_quote_access_metadata_rule.py
+-rw-r--r--   0        0        0     4163 2024-05-02 14:26:01.185235 lusid_sdk-2.1.81/lusid/models/resource_list_of_reconciliation_break.py
+-rw-r--r--   0        0        0     4030 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_relation.py
+-rw-r--r--   0        0        0     4078 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_relationship.py
+-rw-r--r--   0        0        0     4115 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_scope_definition.py
+-rw-r--r--   0        0        0     4103 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_side_definition.py
+-rw-r--r--   0        0        0     3587 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_string.py
+-rw-r--r--   0        0        0     4056 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_tax_rule_set.py
+-rw-r--r--   0        0        0     4066 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_transaction.py
+-rw-r--r--   0        0        0     4115 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_transaction_type.py
+-rw-r--r--   0        0        0     3657 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/resource_list_of_value_type.py
+-rw-r--r--   0        0        0     3438 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/response_meta_data.py
+-rw-r--r--   0        0        0     5434 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_data_key_rule.py
+-rw-r--r--   0        0        0     5313 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_data_schema.py
+-rw-r--r--   0        0        0     3632 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_key_rule.py
+-rw-r--r--   0        0        0      756 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_key_rule_type.py
+-rw-r--r--   0        0        0     4898 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_value.py
+-rw-r--r--   0        0        0     4576 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_value0_d.py
+-rw-r--r--   0        0        0     3678 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_value_bool.py
+-rw-r--r--   0        0        0     3893 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_value_currency.py
+-rw-r--r--   0        0        0     4272 2024-05-02 14:26:01.186235 lusid_sdk-2.1.81/lusid/models/result_value_date_time_offset.py
+-rw-r--r--   0        0        0     4233 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/result_value_decimal.py
+-rw-r--r--   0        0        0     4544 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/result_value_dictionary.py
+-rw-r--r--   0        0        0     4173 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/result_value_int.py
+-rw-r--r--   0        0        0     3881 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/result_value_string.py
+-rw-r--r--   0        0        0     1216 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/result_value_type.py
+-rw-r--r--   0        0        0     6187 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/reverse_stock_split_event.py
+-rw-r--r--   0        0        0     2297 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/rounding_configuration.py
+-rw-r--r--   0        0        0     2111 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/rounding_configuration_component.py
+-rw-r--r--   0        0        0     3968 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/rounding_convention.py
+-rw-r--r--   0        0        0      699 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/scaling_methodology.py
+-rw-r--r--   0        0        0     4032 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/schedule.py
+-rw-r--r--   0        0        0      901 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/schedule_type.py
+-rw-r--r--   0        0        0     1907 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/scope_definition.py
+-rw-r--r--   0        0        0     6145 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/scrip_dividend_event.py
+-rw-r--r--   0        0        0     3357 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/script_map_reference.py
+-rw-r--r--   0        0        0     3429 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/security_election.py
+-rw-r--r--   0        0        0     4439 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/sequence_definition.py
+-rw-r--r--   0        0        0     2945 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/set_legal_entity_identifiers_request.py
+-rw-r--r--   0        0        0     2983 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/set_legal_entity_properties_request.py
+-rw-r--r--   0        0        0     2899 2024-05-02 14:26:01.187235 lusid_sdk-2.1.81/lusid/models/set_person_identifiers_request.py
+-rw-r--r--   0        0        0     2697 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/set_person_properties_request.py
+-rw-r--r--   0        0        0     3083 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/set_share_class_instruments_request.py
+-rw-r--r--   0        0        0     2936 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/set_transaction_configuration_alias.py
+-rw-r--r--   0        0        0     4226 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/set_transaction_configuration_source_request.py
+-rw-r--r--   0        0        0     3518 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/side_configuration_data.py
+-rw-r--r--   0        0        0     2842 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/side_configuration_data_request.py
+-rw-r--r--   0        0        0     4149 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/side_definition.py
+-rw-r--r--   0        0        0     3310 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/side_definition_request.py
+-rw-r--r--   0        0        0     2446 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/sides_definition_request.py
+-rw-r--r--   0        0        0     6272 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/simple_cash_flow_loan.py
+-rw-r--r--   0        0        0     6778 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/simple_instrument.py
+-rw-r--r--   0        0        0      644 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/sort_order.py
+-rw-r--r--   0        0        0     3560 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/staging_rule.py
+-rw-r--r--   0        0        0     2687 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/staging_rule_approval_criteria.py
+-rw-r--r--   0        0        0     3561 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/staging_rule_match_criteria.py
+-rw-r--r--   0        0        0     4196 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/staging_rule_set.py
+-rw-r--r--   0        0        0     4504 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/step_schedule.py
+-rw-r--r--   0        0        0     6183 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/stock_dividend_event.py
+-rw-r--r--   0        0        0     6127 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/stock_split_event.py
+-rw-r--r--   0        0        0     2865 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/stream.py
+-rw-r--r--   0        0        0      799 2024-05-02 14:26:01.188235 lusid_sdk-2.1.81/lusid/models/string_comparison_type.py
+-rw-r--r--   0        0        0     5203 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/string_compliance_parameter.py
+-rw-r--r--   0        0        0     3243 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/string_list.py
+-rw-r--r--   0        0        0     5473 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/string_list_compliance_parameter.py
+-rw-r--r--   0        0        0     3744 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/structured_result_data.py
+-rw-r--r--   0        0        0     4411 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/structured_result_data_id.py
+-rw-r--r--   0        0        0     3498 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/sub_holding_key_value_equals.py
+-rw-r--r--   0        0        0     4296 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/target_tax_lot.py
+-rw-r--r--   0        0        0     4290 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/target_tax_lot_request.py
+-rw-r--r--   0        0        0     3530 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/tax_rule.py
+-rw-r--r--   0        0        0     5007 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/tax_rule_set.py
+-rw-r--r--   0        0        0     2339 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/template_field.py
+-rw-r--r--   0        0        0     6656 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/term_deposit.py
+-rw-r--r--   0        0        0     7051 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/total_return_swap.py
+-rw-r--r--   0        0        0     2726 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/touch.py
+-rw-r--r--   0        0        0     2320 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/trade_ticket.py
+-rw-r--r--   0        0        0      706 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/trade_ticket_type.py
+-rw-r--r--   0        0        0    11577 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/transaction.py
+-rw-r--r--   0        0        0     4318 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/transaction_configuration_data.py
+-rw-r--r--   0        0        0     4398 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/transaction_configuration_data_request.py
+-rw-r--r--   0        0        0     6984 2024-05-02 14:26:01.189235 lusid_sdk-2.1.81/lusid/models/transaction_configuration_movement_data.py
+-rw-r--r--   0        0        0     6623 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_configuration_movement_data_request.py
+-rw-r--r--   0        0        0     4750 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_configuration_type_alias.py
+-rw-r--r--   0        0        0     2524 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_currency_and_amount.py
+-rw-r--r--   0        0        0     4329 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_field_map.py
+-rw-r--r--   0        0        0     2420 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_price.py
+-rw-r--r--   0        0        0     2444 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_price_and_type.py
+-rw-r--r--   0        0        0      743 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_price_type.py
+-rw-r--r--   0        0        0     2607 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_property_map.py
+-rw-r--r--   0        0        0     2822 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_property_mapping.py
+-rw-r--r--   0        0        0     2877 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_property_mapping_request.py
+-rw-r--r--   0        0        0      699 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_query_mode.py
+-rw-r--r--   0        0        0     3365 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_query_parameters.py
+-rw-r--r--   0        0        0     4294 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_reconciliation_request.py
+-rw-r--r--   0        0        0     5946 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_reconciliation_request_v2.py
+-rw-r--r--   0        0        0     9335 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_request.py
+-rw-r--r--   0        0        0      839 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_roles.py
+-rw-r--r--   0        0        0     4411 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_set_configuration_data.py
+-rw-r--r--   0        0        0     3947 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_set_configuration_data_request.py
+-rw-r--r--   0        0        0      700 2024-05-02 14:26:01.190235 lusid_sdk-2.1.81/lusid/models/transaction_status.py
+-rw-r--r--   0        0        0     4175 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_template.py
+-rw-r--r--   0        0        0     2874 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_template_request.py
+-rw-r--r--   0        0        0     4605 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_template_specification.py
+-rw-r--r--   0        0        0     5765 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type.py
+-rw-r--r--   0        0        0     3532 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type_alias.py
+-rw-r--r--   0        0        0     2451 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type_calculation.py
+-rw-r--r--   0        0        0     7324 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type_movement.py
+-rw-r--r--   0        0        0     3249 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type_property_mapping.py
+-rw-r--r--   0        0        0     5121 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transaction_type_request.py
+-rw-r--r--   0        0        0     3083 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transactions_reconciliations_response.py
+-rw-r--r--   0        0        0     6703 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/transition_event.py
+-rw-r--r--   0        0        0     3576 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_entities_inlined_request.py
+-rw-r--r--   0        0        0     3790 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_entities_request.py
+-rw-r--r--   0        0        0     4458 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_entities_response.py
+-rw-r--r--   0        0        0     3602 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_instrument_definitions_request.py
+-rw-r--r--   0        0        0     5063 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_instrument_definitions_response.py
+-rw-r--r--   0        0        0     3354 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_trade_ticket_request.py
+-rw-r--r--   0        0        0     4984 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translate_trade_tickets_response.py
+-rw-r--r--   0        0        0     2507 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translation_context.py
+-rw-r--r--   0        0        0     2035 2024-05-02 14:26:01.191235 lusid_sdk-2.1.81/lusid/models/translation_input.py
+-rw-r--r--   0        0        0     2747 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/translation_result.py
+-rw-r--r--   0        0        0     2684 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/translation_script.py
+-rw-r--r--   0        0        0     3279 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/translation_script_id.py
+-rw-r--r--   0        0        0     6216 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/trial_balance.py
+-rw-r--r--   0        0        0     4934 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/trial_balance_query_parameters.py
+-rw-r--r--   0        0        0     5516 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/trigger_event.py
+-rw-r--r--   0        0        0     3908 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/typed_resource_id.py
+-rw-r--r--   0        0        0      675 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/unit_schema.py
+-rw-r--r--   0        0        0     2154 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/units_ratio.py
+-rw-r--r--   0        0        0      870 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/unmatched_holding_method.py
+-rw-r--r--   0        0        0     3127 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_amortisation_rule_set_details_request.py
+-rw-r--r--   0        0        0     3318 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_calendar_request.py
+-rw-r--r--   0        0        0     3640 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_custom_entity_definition_request.py
+-rw-r--r--   0        0        0     3592 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_custom_entity_type_request.py
+-rw-r--r--   0        0        0     3634 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_cut_label_definition_request.py
+-rw-r--r--   0        0        0     4901 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_data_type_request.py
+-rw-r--r--   0        0        0     3323 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_derived_property_definition_request.py
+-rw-r--r--   0        0        0     3054 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_instrument_identifier_request.py
+-rw-r--r--   0        0        0     2454 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_portfolio_group_request.py
+-rw-r--r--   0        0        0     2418 2024-05-02 14:26:01.192235 lusid_sdk-2.1.81/lusid/models/update_portfolio_request.py
+-rw-r--r--   0        0        0     2575 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_property_definition_request.py
+-rw-r--r--   0        0        0     5901 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_reconciliation_request.py
+-rw-r--r--   0        0        0     3597 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_relationship_definition_request.py
+-rw-r--r--   0        0        0     3350 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_staging_rule_set_request.py
+-rw-r--r--   0        0        0     3243 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_tax_rule_set_request.py
+-rw-r--r--   0        0        0     3889 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/update_unit_request.py
+-rw-r--r--   0        0        0     2503 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_cds_flow_conventions_request.py
+-rw-r--r--   0        0        0     2830 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_complex_market_data_request.py
+-rw-r--r--   0        0        0     5374 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_compliance_rule_request.py
+-rw-r--r--   0        0        0     3311 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_compliance_run_summary_request.py
+-rw-r--r--   0        0        0     3274 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_compliance_run_summary_result.py
+-rw-r--r--   0        0        0     4741 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_corporate_action_request.py
+-rw-r--r--   0        0        0     4960 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_corporate_actions_response.py
+-rw-r--r--   0        0        0     2548 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_counterparty_agreement_request.py
+-rw-r--r--   0        0        0     2531 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_credit_support_annex_request.py
+-rw-r--r--   0        0        0     4996 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_custom_entities_response.py
+-rw-r--r--   0        0        0     2849 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_custom_entity_access_metadata_request.py
+-rw-r--r--   0        0        0     2495 2024-05-02 14:26:01.193235 lusid_sdk-2.1.81/lusid/models/upsert_dialect_request.py
+-rw-r--r--   0        0        0     2431 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_flow_conventions_request.py
+-rw-r--r--   0        0        0     2431 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_index_convention_request.py
+-rw-r--r--   0        0        0     5820 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_instrument_event_request.py
+-rw-r--r--   0        0        0     4985 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_instrument_events_response.py
+-rw-r--r--   0        0        0     2825 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_instrument_properties_response.py
+-rw-r--r--   0        0        0     3347 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_instrument_property_request.py
+-rw-r--r--   0        0        0     6089 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_instruments_response.py
+-rw-r--r--   0        0        0     4949 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_legal_entities_response.py
+-rw-r--r--   0        0        0     2841 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_legal_entity_access_metadata_request.py
+-rw-r--r--   0        0        0     5628 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_legal_entity_request.py
+-rw-r--r--   0        0        0     2795 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_person_access_metadata_request.py
+-rw-r--r--   0        0        0     4278 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_person_request.py
+-rw-r--r--   0        0        0     2587 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_portfolio_access_metadata_request.py
+-rw-r--r--   0        0        0     2633 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_portfolio_group_access_metadata_request.py
+-rw-r--r--   0        0        0     4621 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_portfolio_transactions_response.py
+-rw-r--r--   0        0        0     3283 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_quote_access_metadata_rule_request.py
+-rw-r--r--   0        0        0     4017 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_quote_request.py
+-rw-r--r--   0        0        0     4817 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_quotes_response.py
+-rw-r--r--   0        0        0     2409 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_recipe_composer_request.py
+-rw-r--r--   0        0        0     2423 2024-05-02 14:26:01.194235 lusid_sdk-2.1.81/lusid/models/upsert_recipe_request.py
+-rw-r--r--   0        0        0     4669 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_reference_portfolio_constituents_request.py
+-rw-r--r--   0        0        0     3324 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_reference_portfolio_constituents_response.py
+-rw-r--r--   0        0        0     3542 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_result_values_data_request.py
+-rw-r--r--   0        0        0     4607 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_returns_response.py
+-rw-r--r--   0        0        0     3230 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_single_structured_data_response.py
+-rw-r--r--   0        0        0     4412 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_structured_data_response.py
+-rw-r--r--   0        0        0     2696 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_structured_result_data_request.py
+-rw-r--r--   0        0        0     4345 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_transaction_properties_response.py
+-rw-r--r--   0        0        0     2417 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_translation_script_request.py
+-rw-r--r--   0        0        0     5323 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/upsert_valuation_point_request.py
+-rw-r--r--   0        0        0     2028 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/user.py
+-rw-r--r--   0        0        0     2271 2024-05-02 14:26:01.195235 lusid_sdk-2.1.81/lusid/models/valuation_point_data_query_parameters.py
+-rw-r--r--   0        0        0     2394 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/valuation_point_data_request.py
+-rw-r--r--   0        0        0     5081 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/valuation_point_data_response.py
+-rw-r--r--   0        0        0    10575 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/valuation_request.py
+-rw-r--r--   0        0        0     6154 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/valuation_schedule.py
+-rw-r--r--   0        0        0     5001 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/valuations_reconciliation_request.py
+-rw-r--r--   0        0        0     1241 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/value_type.py
+-rw-r--r--   0        0        0     4307 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/vendor_dependency.py
+-rw-r--r--   0        0        0      812 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/vendor_library.py
+-rw-r--r--   0        0        0     6263 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/vendor_model_rule.py
+-rw-r--r--   0        0        0     6109 2024-05-02 14:26:01.196235 lusid_sdk-2.1.81/lusid/models/version.py
+-rw-r--r--   0        0        0     3584 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/version_summary_dto.py
+-rw-r--r--   0        0        0     4522 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_a2_b_data_record.py
+-rw-r--r--   0        0        0     4570 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_a2_b_movement_record.py
+-rw-r--r--   0        0        0     4580 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_holding_contributor.py
+-rw-r--r--   0        0        0     4557 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_journal_entry_line.py
+-rw-r--r--   0        0        0     4568 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_output_transaction.py
+-rw-r--r--   0        0        0     4556 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_portfolio_holding.py
+-rw-r--r--   0        0        0     4495 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_transaction.py
+-rw-r--r--   0        0        0     4508 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_trial_balance.py
+-rw-r--r--   0        0        0     5579 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py
+-rw-r--r--   0        0        0     3256 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/virtual_document.py
+-rw-r--r--   0        0        0     2756 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/virtual_document_row.py
+-rw-r--r--   0        0        0     3199 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/virtual_row.py
+-rw-r--r--   0        0        0     1876 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/warning.py
+-rw-r--r--   0        0        0     2315 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/weekend_mask.py
+-rw-r--r--   0        0        0     4554 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/weighted_instrument.py
+-rw-r--r--   0        0        0     3441 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/weighted_instrument_in_line_lookup_identifiers.py
+-rw-r--r--   0        0        0     2543 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/weighted_instruments.py
+-rw-r--r--   0        0        0     6330 2024-05-02 14:26:01.197235 lusid_sdk-2.1.81/lusid/models/yield_curve_data.py
+-rw-r--r--   0        0        0        0 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/py.typed
+-rw-r--r--   0        0        0    10138 2024-05-02 14:26:01.207235 lusid_sdk-2.1.81/lusid/rest.py
+-rw-r--r--   0        0        0      791 2024-05-02 14:26:01.275234 lusid_sdk-2.1.81/pyproject.toml
+-rw-r--r--   0        0        0   180503 1970-01-01 00:00:00.000000 lusid_sdk-2.1.81/PKG-INFO
```

### Comparing `lusid_sdk-2.1.79/README.md` & `lusid_sdk-2.1.81/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.11.6513
-- Package version: 2.1.79
+- API version: 0.11.6515
+- Package version: 2.1.81
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_sdk-2.1.79/lusid/__init__.py` & `lusid_sdk-2.1.81/lusid/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/__init__.py` & `lusid_sdk-2.1.81/lusid/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/abor_api.py` & `lusid_sdk-2.1.81/lusid/api/abor_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/abor_configuration_api.py` & `lusid_sdk-2.1.81/lusid/api/abor_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/address_key_definition_api.py` & `lusid_sdk-2.1.81/lusid/api/address_key_definition_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/aggregation_api.py` & `lusid_sdk-2.1.81/lusid/api/aggregation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/allocations_api.py` & `lusid_sdk-2.1.81/lusid/api/allocations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/amortisation_rule_sets_api.py` & `lusid_sdk-2.1.81/lusid/api/amortisation_rule_sets_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/application_metadata_api.py` & `lusid_sdk-2.1.81/lusid/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/blocks_api.py` & `lusid_sdk-2.1.81/lusid/api/blocks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/calendars_api.py` & `lusid_sdk-2.1.81/lusid/api/calendars_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/chart_of_accounts_api.py` & `lusid_sdk-2.1.81/lusid/api/chart_of_accounts_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/complex_market_data_api.py` & `lusid_sdk-2.1.81/lusid/api/complex_market_data_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/compliance_api.py` & `lusid_sdk-2.1.81/lusid/api/compliance_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/configuration_recipe_api.py` & `lusid_sdk-2.1.81/lusid/api/configuration_recipe_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/conventions_api.py` & `lusid_sdk-2.1.81/lusid/api/conventions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/corporate_action_sources_api.py` & `lusid_sdk-2.1.81/lusid/api/corporate_action_sources_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/counterparties_api.py` & `lusid_sdk-2.1.81/lusid/api/counterparties_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/custom_entities_api.py` & `lusid_sdk-2.1.81/lusid/api/custom_entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/custom_entity_definitions_api.py` & `lusid_sdk-2.1.81/lusid/api/custom_entity_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/custom_entity_types_api.py` & `lusid_sdk-2.1.81/lusid/api/custom_entity_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/cut_label_definitions_api.py` & `lusid_sdk-2.1.81/lusid/api/cut_label_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/data_types_api.py` & `lusid_sdk-2.1.81/lusid/api/data_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/derived_transaction_portfolios_api.py` & `lusid_sdk-2.1.81/lusid/api/derived_transaction_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/entities_api.py` & `lusid_sdk-2.1.81/lusid/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/executions_api.py` & `lusid_sdk-2.1.81/lusid/api/executions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/funds_api.py` & `lusid_sdk-2.1.81/lusid/api/funds_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/instrument_event_types_api.py` & `lusid_sdk-2.1.81/lusid/api/instrument_event_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/instrument_events_api.py` & `lusid_sdk-2.1.81/lusid/api/instrument_events_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/instruments_api.py` & `lusid_sdk-2.1.81/lusid/api/instruments_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/legacy_compliance_api.py` & `lusid_sdk-2.1.81/lusid/api/legacy_compliance_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/legal_entities_api.py` & `lusid_sdk-2.1.81/lusid/api/legal_entities_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/order_graph_api.py` & `lusid_sdk-2.1.81/lusid/api/order_graph_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/order_instructions_api.py` & `lusid_sdk-2.1.81/lusid/api/order_instructions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/order_management_api.py` & `lusid_sdk-2.1.81/lusid/api/order_management_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/orders_api.py` & `lusid_sdk-2.1.81/lusid/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/packages_api.py` & `lusid_sdk-2.1.81/lusid/api/packages_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/participations_api.py` & `lusid_sdk-2.1.81/lusid/api/participations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/persons_api.py` & `lusid_sdk-2.1.81/lusid/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/placements_api.py` & `lusid_sdk-2.1.81/lusid/api/placements_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/portfolio_groups_api.py` & `lusid_sdk-2.1.81/lusid/api/portfolio_groups_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/portfolios_api.py` & `lusid_sdk-2.1.81/lusid/api/portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/property_definitions_api.py` & `lusid_sdk-2.1.81/lusid/api/property_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/queryable_keys_api.py` & `lusid_sdk-2.1.81/lusid/api/queryable_keys_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/quotes_api.py` & `lusid_sdk-2.1.81/lusid/api/quotes_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/reconciliations_api.py` & `lusid_sdk-2.1.81/lusid/api/reconciliations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/reference_lists_api.py` & `lusid_sdk-2.1.81/lusid/api/reference_lists_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/reference_portfolio_api.py` & `lusid_sdk-2.1.81/lusid/api/reference_portfolio_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/relation_definitions_api.py` & `lusid_sdk-2.1.81/lusid/api/relation_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/relations_api.py` & `lusid_sdk-2.1.81/lusid/api/relations_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/relationship_definitions_api.py` & `lusid_sdk-2.1.81/lusid/api/relationship_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/relationships_api.py` & `lusid_sdk-2.1.81/lusid/api/relationships_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/schemas_api.py` & `lusid_sdk-2.1.81/lusid/api/schemas_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/scopes_api.py` & `lusid_sdk-2.1.81/lusid/api/scopes_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/scripted_translation_api.py` & `lusid_sdk-2.1.81/lusid/api/scripted_translation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/search_api.py` & `lusid_sdk-2.1.81/lusid/api/search_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/sequences_api.py` & `lusid_sdk-2.1.81/lusid/api/sequences_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/staging_rule_set_api.py` & `lusid_sdk-2.1.81/lusid/api/staging_rule_set_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/structured_result_data_api.py` & `lusid_sdk-2.1.81/lusid/api/structured_result_data_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/system_configuration_api.py` & `lusid_sdk-2.1.81/lusid/api/system_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/tax_rule_sets_api.py` & `lusid_sdk-2.1.81/lusid/api/tax_rule_sets_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/transaction_configuration_api.py` & `lusid_sdk-2.1.81/lusid/api/transaction_configuration_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/transaction_fees_api.py` & `lusid_sdk-2.1.81/lusid/api/transaction_fees_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/transaction_portfolios_api.py` & `lusid_sdk-2.1.81/lusid/api/transaction_portfolios_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api/translation_api.py` & `lusid_sdk-2.1.81/lusid/api/translation_api.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api_client.py` & `lusid_sdk-2.1.81/lusid/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/api_response.py` & `lusid_sdk-2.1.81/lusid/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/configuration.py` & `lusid_sdk-2.1.81/lusid/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.11.6513\n"\
+               "Version of the API: 0.11.6515\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_sdk-2.1.79/lusid/exceptions.py` & `lusid_sdk-2.1.81/lusid/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/__init__.py` & `lusid_sdk-2.1.81/lusid/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/api_client.py` & `lusid_sdk-2.1.81/lusid/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/api_client_factory.py` & `lusid_sdk-2.1.81/lusid/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/api_configuration.py` & `lusid_sdk-2.1.81/lusid/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/configuration_loaders.py` & `lusid_sdk-2.1.81/lusid/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/proxy_config.py` & `lusid_sdk-2.1.81/lusid/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/refreshing_token.py` & `lusid_sdk-2.1.81/lusid/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/rest.py` & `lusid_sdk-2.1.81/lusid/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/retry.py` & `lusid_sdk-2.1.81/lusid/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/socket_keep_alive.py` & `lusid_sdk-2.1.81/lusid/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/extensions/tcp_keep_alive_connector.py` & `lusid_sdk-2.1.81/lusid/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/__init__.py` & `lusid_sdk-2.1.81/lusid/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/a2_b_breakdown.py` & `lusid_sdk-2.1.81/lusid/models/a2_b_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/a2_b_category.py` & `lusid_sdk-2.1.81/lusid/models/a2_b_category.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/a2_b_data_record.py` & `lusid_sdk-2.1.81/lusid/models/a2_b_data_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/a2_b_movement_record.py` & `lusid_sdk-2.1.81/lusid/models/a2_b_movement_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor.py` & `lusid_sdk-2.1.81/lusid/models/abor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor_configuration.py` & `lusid_sdk-2.1.81/lusid/models/abor_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor_configuration_properties.py` & `lusid_sdk-2.1.81/lusid/models/abor_configuration_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor_configuration_request.py` & `lusid_sdk-2.1.81/lusid/models/abor_configuration_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor_properties.py` & `lusid_sdk-2.1.81/lusid/models/abor_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/abor_request.py` & `lusid_sdk-2.1.81/lusid/models/abor_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/access_controlled_action.py` & `lusid_sdk-2.1.81/lusid/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/access_controlled_resource.py` & `lusid_sdk-2.1.81/lusid/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/access_metadata_operation.py` & `lusid_sdk-2.1.81/lusid/models/access_metadata_operation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/access_metadata_value.py` & `lusid_sdk-2.1.81/lusid/models/access_metadata_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/account.py` & `lusid_sdk-2.1.81/lusid/models/account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/account_properties.py` & `lusid_sdk-2.1.81/lusid/models/account_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/accounting_method.py` & `lusid_sdk-2.1.81/lusid/models/accounting_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/accounts_upsert_response.py` & `lusid_sdk-2.1.81/lusid/models/accounts_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/accumulation_event.py` & `lusid_sdk-2.1.81/lusid/models/accumulation_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/action_id.py` & `lusid_sdk-2.1.81/lusid/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/add_business_days_to_date_request.py` & `lusid_sdk-2.1.81/lusid/models/add_business_days_to_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/add_business_days_to_date_response.py` & `lusid_sdk-2.1.81/lusid/models/add_business_days_to_date_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/additional_payment.py` & `lusid_sdk-2.1.81/lusid/models/additional_payment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_definition.py` & `lusid_sdk-2.1.81/lusid/models/address_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/address_key_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_definition.py` & `lusid_sdk-2.1.81/lusid/models/address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_filter.py` & `lusid_sdk-2.1.81/lusid/models/address_key_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_list.py` & `lusid_sdk-2.1.81/lusid/models/address_key_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/address_key_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/address_key_option_definition.py` & `lusid_sdk-2.1.81/lusid/models/address_key_option_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/adjust_holding.py` & `lusid_sdk-2.1.81/lusid/models/adjust_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/adjust_holding_for_date_request.py` & `lusid_sdk-2.1.81/lusid/models/adjust_holding_for_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/adjust_holding_request.py` & `lusid_sdk-2.1.81/lusid/models/adjust_holding_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregate_spec.py` & `lusid_sdk-2.1.81/lusid/models/aggregate_spec.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregated_return.py` & `lusid_sdk-2.1.81/lusid/models/aggregated_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregated_returns_dispersion_request.py` & `lusid_sdk-2.1.81/lusid/models/aggregated_returns_dispersion_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregated_returns_request.py` & `lusid_sdk-2.1.81/lusid/models/aggregated_returns_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregated_returns_response.py` & `lusid_sdk-2.1.81/lusid/models/aggregated_returns_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregated_transactions_request.py` & `lusid_sdk-2.1.81/lusid/models/aggregated_transactions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_context.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_measure_failure_detail.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_measure_failure_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_op.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_op.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_options.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_query.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_query.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/aggregation_type.py` & `lusid_sdk-2.1.81/lusid/models/aggregation_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/allocation.py` & `lusid_sdk-2.1.81/lusid/models/allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/allocation_request.py` & `lusid_sdk-2.1.81/lusid/models/allocation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/allocation_service_run_response.py` & `lusid_sdk-2.1.81/lusid/models/allocation_service_run_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/allocation_set_request.py` & `lusid_sdk-2.1.81/lusid/models/allocation_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/amortisation_event.py` & `lusid_sdk-2.1.81/lusid/models/amortisation_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/amortisation_rule.py` & `lusid_sdk-2.1.81/lusid/models/amortisation_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/amortisation_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/amortisation_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/annul_quotes_response.py` & `lusid_sdk-2.1.81/lusid/models/annul_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/annul_single_structured_data_response.py` & `lusid_sdk-2.1.81/lusid/models/annul_single_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/annul_structured_data_response.py` & `lusid_sdk-2.1.81/lusid/models/annul_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/asset_class.py` & `lusid_sdk-2.1.81/lusid/models/asset_class.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/asset_leg.py` & `lusid_sdk-2.1.81/lusid/models/asset_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/barrier.py` & `lusid_sdk-2.1.81/lusid/models/barrier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/basket.py` & `lusid_sdk-2.1.81/lusid/models/basket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/basket_identifier.py` & `lusid_sdk-2.1.81/lusid/models/basket_identifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/batch_adjust_holdings_response.py` & `lusid_sdk-2.1.81/lusid/models/batch_adjust_holdings_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/batch_upsert_instrument_properties_response.py` & `lusid_sdk-2.1.81/lusid/models/batch_upsert_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/batch_upsert_portfolio_transactions_response.py` & `lusid_sdk-2.1.81/lusid/models/batch_upsert_portfolio_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/batch_upsert_property_definition_properties_response.py` & `lusid_sdk-2.1.81/lusid/models/batch_upsert_property_definition_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block.py` & `lusid_sdk-2.1.81/lusid/models/block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_and_order_id_request.py` & `lusid_sdk-2.1.81/lusid/models/block_and_order_id_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_and_orders.py` & `lusid_sdk-2.1.81/lusid/models/block_and_orders.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_and_orders_create_request.py` & `lusid_sdk-2.1.81/lusid/models/block_and_orders_create_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_and_orders_request.py` & `lusid_sdk-2.1.81/lusid/models/block_and_orders_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_request.py` & `lusid_sdk-2.1.81/lusid/models/block_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/block_set_request.py` & `lusid_sdk-2.1.81/lusid/models/block_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/blocked_order_request.py` & `lusid_sdk-2.1.81/lusid/models/blocked_order_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bond.py` & `lusid_sdk-2.1.81/lusid/models/bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bond_coupon_event.py` & `lusid_sdk-2.1.81/lusid/models/bond_coupon_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bond_default_event.py` & `lusid_sdk-2.1.81/lusid/models/bond_default_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bond_principal_event.py` & `lusid_sdk-2.1.81/lusid/models/bond_principal_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/book_transactions_request.py` & `lusid_sdk-2.1.81/lusid/models/book_transactions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/book_transactions_response.py` & `lusid_sdk-2.1.81/lusid/models/book_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bool_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/bool_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bool_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/bool_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/branch_step.py` & `lusid_sdk-2.1.81/lusid/models/branch_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bucketed_cash_flow_request.py` & `lusid_sdk-2.1.81/lusid/models/bucketed_cash_flow_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bucketed_cash_flow_response.py` & `lusid_sdk-2.1.81/lusid/models/bucketed_cash_flow_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/bucketing_schedule.py` & `lusid_sdk-2.1.81/lusid/models/bucketing_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/calculation_info.py` & `lusid_sdk-2.1.81/lusid/models/calculation_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/calendar.py` & `lusid_sdk-2.1.81/lusid/models/calendar.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/calendar_date.py` & `lusid_sdk-2.1.81/lusid/models/calendar_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/calendar_dependency.py` & `lusid_sdk-2.1.81/lusid/models/calendar_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cap_floor.py` & `lusid_sdk-2.1.81/lusid/models/cap_floor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_dependency.py` & `lusid_sdk-2.1.81/lusid/models/cash_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_dividend_event.py` & `lusid_sdk-2.1.81/lusid/models/cash_dividend_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_election.py` & `lusid_sdk-2.1.81/lusid/models/cash_election.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_flow_event.py` & `lusid_sdk-2.1.81/lusid/models/cash_flow_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_flow_lineage.py` & `lusid_sdk-2.1.81/lusid/models/cash_flow_lineage.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_flow_value.py` & `lusid_sdk-2.1.81/lusid/models/cash_flow_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_flow_value_set.py` & `lusid_sdk-2.1.81/lusid/models/cash_flow_value_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_ladder_record.py` & `lusid_sdk-2.1.81/lusid/models/cash_ladder_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cash_perpetual.py` & `lusid_sdk-2.1.81/lusid/models/cash_perpetual.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cds_flow_conventions.py` & `lusid_sdk-2.1.81/lusid/models/cds_flow_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cds_index.py` & `lusid_sdk-2.1.81/lusid/models/cds_index.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cds_protection_detail_specification.py` & `lusid_sdk-2.1.81/lusid/models/cds_protection_detail_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/change.py` & `lusid_sdk-2.1.81/lusid/models/change.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/change_history.py` & `lusid_sdk-2.1.81/lusid/models/change_history.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/change_history_action.py` & `lusid_sdk-2.1.81/lusid/models/change_history_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/change_item.py` & `lusid_sdk-2.1.81/lusid/models/change_item.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/chart_of_accounts.py` & `lusid_sdk-2.1.81/lusid/models/chart_of_accounts.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/chart_of_accounts_properties.py` & `lusid_sdk-2.1.81/lusid/models/chart_of_accounts_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/chart_of_accounts_request.py` & `lusid_sdk-2.1.81/lusid/models/chart_of_accounts_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/check_step.py` & `lusid_sdk-2.1.81/lusid/models/check_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cleardown_module_details.py` & `lusid_sdk-2.1.81/lusid/models/cleardown_module_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cleardown_module_request.py` & `lusid_sdk-2.1.81/lusid/models/cleardown_module_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cleardown_module_response.py` & `lusid_sdk-2.1.81/lusid/models/cleardown_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cleardown_module_rule.py` & `lusid_sdk-2.1.81/lusid/models/cleardown_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cleardown_module_rules_updated_response.py` & `lusid_sdk-2.1.81/lusid/models/cleardown_module_rules_updated_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/client.py` & `lusid_sdk-2.1.81/lusid/models/client.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/close_event.py` & `lusid_sdk-2.1.81/lusid/models/close_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/close_period_diary_entry_request.py` & `lusid_sdk-2.1.81/lusid/models/close_period_diary_entry_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complete_portfolio.py` & `lusid_sdk-2.1.81/lusid/models/complete_portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complete_relation.py` & `lusid_sdk-2.1.81/lusid/models/complete_relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complete_relationship.py` & `lusid_sdk-2.1.81/lusid/models/complete_relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complex_bond.py` & `lusid_sdk-2.1.81/lusid/models/complex_bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complex_market_data.py` & `lusid_sdk-2.1.81/lusid/models/complex_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/complex_market_data_id.py` & `lusid_sdk-2.1.81/lusid/models/complex_market_data_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_breached_order_info.py` & `lusid_sdk-2.1.81/lusid/models/compliance_breached_order_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_parameter_type.py` & `lusid_sdk-2.1.81/lusid/models/compliance_parameter_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_breakdown.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_breakdown_request.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_breakdown_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_response.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_result.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_result_detail.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_result_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_result_portfolio_detail.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_result_portfolio_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_result_v2.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_result_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_upsert_request.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_upsert_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_rule_upsert_response.py` & `lusid_sdk-2.1.81/lusid/models/compliance_rule_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_run_info.py` & `lusid_sdk-2.1.81/lusid/models/compliance_run_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_run_info_v2.py` & `lusid_sdk-2.1.81/lusid/models/compliance_run_info_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_step.py` & `lusid_sdk-2.1.81/lusid/models/compliance_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_step_type.py` & `lusid_sdk-2.1.81/lusid/models/compliance_step_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_summary_rule_result.py` & `lusid_sdk-2.1.81/lusid/models/compliance_summary_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_summary_rule_result_request.py` & `lusid_sdk-2.1.81/lusid/models/compliance_summary_rule_result_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_template.py` & `lusid_sdk-2.1.81/lusid/models/compliance_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_template_parameter.py` & `lusid_sdk-2.1.81/lusid/models/compliance_template_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compliance_template_variation.py` & `lusid_sdk-2.1.81/lusid/models/compliance_template_variation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/component_transaction.py` & `lusid_sdk-2.1.81/lusid/models/component_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/composite_breakdown.py` & `lusid_sdk-2.1.81/lusid/models/composite_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/composite_breakdown_request.py` & `lusid_sdk-2.1.81/lusid/models/composite_breakdown_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/composite_breakdown_response.py` & `lusid_sdk-2.1.81/lusid/models/composite_breakdown_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/composite_dispersion.py` & `lusid_sdk-2.1.81/lusid/models/composite_dispersion.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/composite_dispersion_response.py` & `lusid_sdk-2.1.81/lusid/models/composite_dispersion_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/compounding.py` & `lusid_sdk-2.1.81/lusid/models/compounding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/configuration_recipe.py` & `lusid_sdk-2.1.81/lusid/models/configuration_recipe.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/constant_volatility_surface.py` & `lusid_sdk-2.1.81/lusid/models/constant_volatility_surface.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/constituents_adjustment_header.py` & `lusid_sdk-2.1.81/lusid/models/constituents_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/contract_for_difference.py` & `lusid_sdk-2.1.81/lusid/models/contract_for_difference.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action_source.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action_source.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action_transition.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action_transition_component.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action_transition_component.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action_transition_component_request.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action_transition_component_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/corporate_action_transition_request.py` & `lusid_sdk-2.1.81/lusid/models/corporate_action_transition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/counterparty_agreement.py` & `lusid_sdk-2.1.81/lusid/models/counterparty_agreement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/counterparty_risk_information.py` & `lusid_sdk-2.1.81/lusid/models/counterparty_risk_information.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/counterparty_signatory.py` & `lusid_sdk-2.1.81/lusid/models/counterparty_signatory.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_address_key_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_address_key_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_amortisation_rule_set_request.py` & `lusid_sdk-2.1.81/lusid/models/create_amortisation_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_calendar_request.py` & `lusid_sdk-2.1.81/lusid/models/create_calendar_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_corporate_action_source_request.py` & `lusid_sdk-2.1.81/lusid/models/create_corporate_action_source_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_custom_entity_type_request.py` & `lusid_sdk-2.1.81/lusid/models/create_custom_entity_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_cut_label_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_cut_label_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_data_map_request.py` & `lusid_sdk-2.1.81/lusid/models/create_data_map_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_data_type_request.py` & `lusid_sdk-2.1.81/lusid/models/create_data_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_date_request.py` & `lusid_sdk-2.1.81/lusid/models/create_date_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_derived_property_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_derived_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_derived_transaction_portfolio_request.py` & `lusid_sdk-2.1.81/lusid/models/create_derived_transaction_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_portfolio_details.py` & `lusid_sdk-2.1.81/lusid/models/create_portfolio_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_portfolio_group_request.py` & `lusid_sdk-2.1.81/lusid/models/create_portfolio_group_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_property_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_recipe_request.py` & `lusid_sdk-2.1.81/lusid/models/create_recipe_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/create_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_reference_portfolio_request.py` & `lusid_sdk-2.1.81/lusid/models/create_reference_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_relation_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_relation_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_relation_request.py` & `lusid_sdk-2.1.81/lusid/models/create_relation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_relationship_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/create_relationship_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_relationship_request.py` & `lusid_sdk-2.1.81/lusid/models/create_relationship_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_sequence_request.py` & `lusid_sdk-2.1.81/lusid/models/create_sequence_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_staging_rule_set_request.py` & `lusid_sdk-2.1.81/lusid/models/create_staging_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_tax_rule_set_request.py` & `lusid_sdk-2.1.81/lusid/models/create_tax_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_trade_tickets_response.py` & `lusid_sdk-2.1.81/lusid/models/create_trade_tickets_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_transaction_portfolio_request.py` & `lusid_sdk-2.1.81/lusid/models/create_transaction_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/create_unit_definition.py` & `lusid_sdk-2.1.81/lusid/models/create_unit_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/credit_default_swap.py` & `lusid_sdk-2.1.81/lusid/models/credit_default_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/credit_rating.py` & `lusid_sdk-2.1.81/lusid/models/credit_rating.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/credit_spread_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/credit_spread_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/credit_support_annex.py` & `lusid_sdk-2.1.81/lusid/models/credit_support_annex.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/criterion_type.py` & `lusid_sdk-2.1.81/lusid/models/criterion_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/currency_and_amount.py` & `lusid_sdk-2.1.81/lusid/models/currency_and_amount.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/curve_options.py` & `lusid_sdk-2.1.81/lusid/models/curve_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custodian_account.py` & `lusid_sdk-2.1.81/lusid/models/custodian_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custodian_account_properties.py` & `lusid_sdk-2.1.81/lusid/models/custodian_account_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custodian_account_request.py` & `lusid_sdk-2.1.81/lusid/models/custodian_account_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custodian_accounts_upsert_response.py` & `lusid_sdk-2.1.81/lusid/models/custodian_accounts_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_definition.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_field.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_field.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_field_definition.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_id.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_request.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_response.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/custom_entity_type.py` & `lusid_sdk-2.1.81/lusid/models/custom_entity_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cut_label_definition.py` & `lusid_sdk-2.1.81/lusid/models/cut_label_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/cut_local_time.py` & `lusid_sdk-2.1.81/lusid/models/cut_local_time.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_definition.py` & `lusid_sdk-2.1.81/lusid/models/data_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_map_key.py` & `lusid_sdk-2.1.81/lusid/models/data_map_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_mapping.py` & `lusid_sdk-2.1.81/lusid/models/data_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_scope.py` & `lusid_sdk-2.1.81/lusid/models/data_scope.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_type.py` & `lusid_sdk-2.1.81/lusid/models/data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_type_summary.py` & `lusid_sdk-2.1.81/lusid/models/data_type_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/data_type_value_range.py` & `lusid_sdk-2.1.81/lusid/models/data_type_value_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_attributes.py` & `lusid_sdk-2.1.81/lusid/models/date_attributes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_or_diary_entry.py` & `lusid_sdk-2.1.81/lusid/models/date_or_diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_range.py` & `lusid_sdk-2.1.81/lusid/models/date_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_time_comparison_type.py` & `lusid_sdk-2.1.81/lusid/models/date_time_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_time_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/date_time_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/date_time_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/date_time_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/day_month.py` & `lusid_sdk-2.1.81/lusid/models/day_month.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/day_of_week.py` & `lusid_sdk-2.1.81/lusid/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/decimal_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/decimal_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/decimal_list.py` & `lusid_sdk-2.1.81/lusid/models/decimal_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/decimal_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/decimal_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/decorated_compliance_run_summary.py` & `lusid_sdk-2.1.81/lusid/models/decorated_compliance_run_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_accounts_response.py` & `lusid_sdk-2.1.81/lusid/models/delete_accounts_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_custodian_accounts_response.py` & `lusid_sdk-2.1.81/lusid/models/delete_custodian_accounts_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_instrument_properties_response.py` & `lusid_sdk-2.1.81/lusid/models/delete_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_instrument_response.py` & `lusid_sdk-2.1.81/lusid/models/delete_instrument_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_instruments_response.py` & `lusid_sdk-2.1.81/lusid/models/delete_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_modes.py` & `lusid_sdk-2.1.81/lusid/models/delete_modes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_relation_request.py` & `lusid_sdk-2.1.81/lusid/models/delete_relation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/delete_relationship_request.py` & `lusid_sdk-2.1.81/lusid/models/delete_relationship_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/deleted_entity_response.py` & `lusid_sdk-2.1.81/lusid/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dependency_source_filter.py` & `lusid_sdk-2.1.81/lusid/models/dependency_source_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/described_address_key.py` & `lusid_sdk-2.1.81/lusid/models/described_address_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dialect.py` & `lusid_sdk-2.1.81/lusid/models/dialect.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dialect_id.py` & `lusid_sdk-2.1.81/lusid/models/dialect_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dialect_schema.py` & `lusid_sdk-2.1.81/lusid/models/dialect_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/diary_entry.py` & `lusid_sdk-2.1.81/lusid/models/diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/diary_entry_request.py` & `lusid_sdk-2.1.81/lusid/models/diary_entry_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/discount_factor_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/discount_factor_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/discounting_dependency.py` & `lusid_sdk-2.1.81/lusid/models/discounting_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/discounting_method.py` & `lusid_sdk-2.1.81/lusid/models/discounting_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dividend_option_event.py` & `lusid_sdk-2.1.81/lusid/models/dividend_option_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/dividend_reinvestment_event.py` & `lusid_sdk-2.1.81/lusid/models/dividend_reinvestment_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/economic_dependency.py` & `lusid_sdk-2.1.81/lusid/models/economic_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/economic_dependency_type.py` & `lusid_sdk-2.1.81/lusid/models/economic_dependency_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/economic_dependency_with_complex_market_data.py` & `lusid_sdk-2.1.81/lusid/models/economic_dependency_with_complex_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/economic_dependency_with_quote.py` & `lusid_sdk-2.1.81/lusid/models/economic_dependency_with_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/election_specification.py` & `lusid_sdk-2.1.81/lusid/models/election_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/eligibility_calculation.py` & `lusid_sdk-2.1.81/lusid/models/eligibility_calculation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/empty_model_options.py` & `lusid_sdk-2.1.81/lusid/models/empty_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/entity_identifier.py` & `lusid_sdk-2.1.81/lusid/models/entity_identifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity.py` & `lusid_sdk-2.1.81/lusid/models/equity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_all_of_identifiers.py` & `lusid_sdk-2.1.81/lusid/models/equity_all_of_identifiers.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_curve_by_prices_data.py` & `lusid_sdk-2.1.81/lusid/models/equity_curve_by_prices_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_curve_dependency.py` & `lusid_sdk-2.1.81/lusid/models/equity_curve_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_model_options.py` & `lusid_sdk-2.1.81/lusid/models/equity_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_option.py` & `lusid_sdk-2.1.81/lusid/models/equity_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_swap.py` & `lusid_sdk-2.1.81/lusid/models/equity_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_vol_dependency.py` & `lusid_sdk-2.1.81/lusid/models/equity_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/equity_vol_surface_data.py` & `lusid_sdk-2.1.81/lusid/models/equity_vol_surface_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/error_detail.py` & `lusid_sdk-2.1.81/lusid/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/event_date_range.py` & `lusid_sdk-2.1.81/lusid/models/event_date_range.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/ex_dividend_configuration.py` & `lusid_sdk-2.1.81/lusid/models/ex_dividend_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/exchange_traded_option.py` & `lusid_sdk-2.1.81/lusid/models/exchange_traded_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/exchange_traded_option_contract_details.py` & `lusid_sdk-2.1.81/lusid/models/exchange_traded_option_contract_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/execution.py` & `lusid_sdk-2.1.81/lusid/models/execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/execution_request.py` & `lusid_sdk-2.1.81/lusid/models/execution_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/execution_set_request.py` & `lusid_sdk-2.1.81/lusid/models/execution_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/exercise_event.py` & `lusid_sdk-2.1.81/lusid/models/exercise_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/exotic_instrument.py` & `lusid_sdk-2.1.81/lusid/models/exotic_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/expanded_group.py` & `lusid_sdk-2.1.81/lusid/models/expanded_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/expiry_event.py` & `lusid_sdk-2.1.81/lusid/models/expiry_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fee_rule.py` & `lusid_sdk-2.1.81/lusid/models/fee_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fee_rule_upsert_request.py` & `lusid_sdk-2.1.81/lusid/models/fee_rule_upsert_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fee_rule_upsert_response.py` & `lusid_sdk-2.1.81/lusid/models/fee_rule_upsert_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/field_definition.py` & `lusid_sdk-2.1.81/lusid/models/field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/field_schema.py` & `lusid_sdk-2.1.81/lusid/models/field_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/field_value.py` & `lusid_sdk-2.1.81/lusid/models/field_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/file_response.py` & `lusid_sdk-2.1.81/lusid/models/file_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/filter_predicate_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/filter_predicate_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/filter_step.py` & `lusid_sdk-2.1.81/lusid/models/filter_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fixed_leg.py` & `lusid_sdk-2.1.81/lusid/models/fixed_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fixed_leg_all_of_overrides.py` & `lusid_sdk-2.1.81/lusid/models/fixed_leg_all_of_overrides.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fixed_schedule.py` & `lusid_sdk-2.1.81/lusid/models/fixed_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/flexible_loan.py` & `lusid_sdk-2.1.81/lusid/models/flexible_loan.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/float_schedule.py` & `lusid_sdk-2.1.81/lusid/models/float_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/floating_leg.py` & `lusid_sdk-2.1.81/lusid/models/floating_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/flow_convention_name.py` & `lusid_sdk-2.1.81/lusid/models/flow_convention_name.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/flow_conventions.py` & `lusid_sdk-2.1.81/lusid/models/flow_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/forward_rate_agreement.py` & `lusid_sdk-2.1.81/lusid/models/forward_rate_agreement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/from_recipe.py` & `lusid_sdk-2.1.81/lusid/models/from_recipe.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fund.py` & `lusid_sdk-2.1.81/lusid/models/fund.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fund_properties.py` & `lusid_sdk-2.1.81/lusid/models/fund_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fund_request.py` & `lusid_sdk-2.1.81/lusid/models/fund_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fund_share_class.py` & `lusid_sdk-2.1.81/lusid/models/fund_share_class.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/funding_leg.py` & `lusid_sdk-2.1.81/lusid/models/funding_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/funding_leg_options.py` & `lusid_sdk-2.1.81/lusid/models/funding_leg_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/future.py` & `lusid_sdk-2.1.81/lusid/models/future.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/futures_contract_details.py` & `lusid_sdk-2.1.81/lusid/models/futures_contract_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_conventions.py` & `lusid_sdk-2.1.81/lusid/models/fx_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_dependency.py` & `lusid_sdk-2.1.81/lusid/models/fx_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_curve_by_quote_reference.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_curve_by_quote_reference.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_model_options.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_pips_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_pips_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_settlement_event.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_settlement_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_tenor_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_tenor_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forward_tenor_pips_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/fx_forward_tenor_pips_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_forwards_dependency.py` & `lusid_sdk-2.1.81/lusid/models/fx_forwards_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_linked_notional_schedule.py` & `lusid_sdk-2.1.81/lusid/models/fx_linked_notional_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_option.py` & `lusid_sdk-2.1.81/lusid/models/fx_option.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_rate_schedule.py` & `lusid_sdk-2.1.81/lusid/models/fx_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_swap.py` & `lusid_sdk-2.1.81/lusid/models/fx_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_tenor_convention.py` & `lusid_sdk-2.1.81/lusid/models/fx_tenor_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_vol_dependency.py` & `lusid_sdk-2.1.81/lusid/models/fx_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/fx_vol_surface_data.py` & `lusid_sdk-2.1.81/lusid/models/fx_vol_surface_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/general_ledger_profile_mapping.py` & `lusid_sdk-2.1.81/lusid/models/general_ledger_profile_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/general_ledger_profile_request.py` & `lusid_sdk-2.1.81/lusid/models/general_ledger_profile_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/general_ledger_profile_response.py` & `lusid_sdk-2.1.81/lusid/models/general_ledger_profile_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_cds_flow_conventions_response.py` & `lusid_sdk-2.1.81/lusid/models/get_cds_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_complex_market_data_response.py` & `lusid_sdk-2.1.81/lusid/models/get_complex_market_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_counterparty_agreement_response.py` & `lusid_sdk-2.1.81/lusid/models/get_counterparty_agreement_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_credit_support_annex_response.py` & `lusid_sdk-2.1.81/lusid/models/get_credit_support_annex_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_data_map_response.py` & `lusid_sdk-2.1.81/lusid/models/get_data_map_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_flow_conventions_response.py` & `lusid_sdk-2.1.81/lusid/models/get_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_index_convention_response.py` & `lusid_sdk-2.1.81/lusid/models/get_index_convention_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_instruments_response.py` & `lusid_sdk-2.1.81/lusid/models/get_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_quotes_response.py` & `lusid_sdk-2.1.81/lusid/models/get_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_recipe_composer_response.py` & `lusid_sdk-2.1.81/lusid/models/get_recipe_composer_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_recipe_response.py` & `lusid_sdk-2.1.81/lusid/models/get_recipe_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_reference_portfolio_constituents_response.py` & `lusid_sdk-2.1.81/lusid/models/get_reference_portfolio_constituents_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_structured_result_data_response.py` & `lusid_sdk-2.1.81/lusid/models/get_structured_result_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/get_virtual_document_response.py` & `lusid_sdk-2.1.81/lusid/models/get_virtual_document_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/group_by_selector_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/group_by_selector_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/group_by_step.py` & `lusid_sdk-2.1.81/lusid/models/group_by_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/group_filter_predicate_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/group_filter_predicate_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/group_filter_step.py` & `lusid_sdk-2.1.81/lusid/models/group_filter_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/group_of_market_data_key_rules.py` & `lusid_sdk-2.1.81/lusid/models/group_of_market_data_key_rules.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/grouped_result_of_address_key.py` & `lusid_sdk-2.1.81/lusid/models/grouped_result_of_address_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holding_adjustment.py` & `lusid_sdk-2.1.81/lusid/models/holding_adjustment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holding_adjustment_with_date.py` & `lusid_sdk-2.1.81/lusid/models/holding_adjustment_with_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holding_context.py` & `lusid_sdk-2.1.81/lusid/models/holding_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holding_contributor.py` & `lusid_sdk-2.1.81/lusid/models/holding_contributor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holdings_adjustment.py` & `lusid_sdk-2.1.81/lusid/models/holdings_adjustment.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/holdings_adjustment_header.py` & `lusid_sdk-2.1.81/lusid/models/holdings_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/i_unit_definition_dto.py` & `lusid_sdk-2.1.81/lusid/models/i_unit_definition_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/id_selector_definition.py` & `lusid_sdk-2.1.81/lusid/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/identifier_part_schema.py` & `lusid_sdk-2.1.81/lusid/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/index_convention.py` & `lusid_sdk-2.1.81/lusid/models/index_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/index_model_options.py` & `lusid_sdk-2.1.81/lusid/models/index_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/index_projection_dependency.py` & `lusid_sdk-2.1.81/lusid/models/index_projection_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/industry_classifier.py` & `lusid_sdk-2.1.81/lusid/models/industry_classifier.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inflation_fixing_dependency.py` & `lusid_sdk-2.1.81/lusid/models/inflation_fixing_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inflation_index_conventions.py` & `lusid_sdk-2.1.81/lusid/models/inflation_index_conventions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inflation_leg.py` & `lusid_sdk-2.1.81/lusid/models/inflation_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inflation_linked_bond.py` & `lusid_sdk-2.1.81/lusid/models/inflation_linked_bond.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inflation_swap.py` & `lusid_sdk-2.1.81/lusid/models/inflation_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/informational_error_event.py` & `lusid_sdk-2.1.81/lusid/models/informational_error_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/informational_event.py` & `lusid_sdk-2.1.81/lusid/models/informational_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inline_valuation_request.py` & `lusid_sdk-2.1.81/lusid/models/inline_valuation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/inline_valuations_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/inline_valuations_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/input_transition.py` & `lusid_sdk-2.1.81/lusid/models/input_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument.py` & `lusid_sdk-2.1.81/lusid/models/instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_capabilities.py` & `lusid_sdk-2.1.81/lusid/models/instrument_capabilities.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_cash_flow.py` & `lusid_sdk-2.1.81/lusid/models/instrument_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_definition.py` & `lusid_sdk-2.1.81/lusid/models/instrument_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_definition_format.py` & `lusid_sdk-2.1.81/lusid/models/instrument_definition_format.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_delete_modes.py` & `lusid_sdk-2.1.81/lusid/models/instrument_delete_modes.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_event.py` & `lusid_sdk-2.1.81/lusid/models/instrument_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_event_configuration.py` & `lusid_sdk-2.1.81/lusid/models/instrument_event_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_event_holder.py` & `lusid_sdk-2.1.81/lusid/models/instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_event_type.py` & `lusid_sdk-2.1.81/lusid/models/instrument_event_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_id_type_descriptor.py` & `lusid_sdk-2.1.81/lusid/models/instrument_id_type_descriptor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_id_value.py` & `lusid_sdk-2.1.81/lusid/models/instrument_id_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_leg.py` & `lusid_sdk-2.1.81/lusid/models/instrument_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_list.py` & `lusid_sdk-2.1.81/lusid/models/instrument_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/instrument_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_match.py` & `lusid_sdk-2.1.81/lusid/models/instrument_match.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_models.py` & `lusid_sdk-2.1.81/lusid/models/instrument_models.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_payment_diary.py` & `lusid_sdk-2.1.81/lusid/models/instrument_payment_diary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_payment_diary_leg.py` & `lusid_sdk-2.1.81/lusid/models/instrument_payment_diary_leg.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_payment_diary_row.py` & `lusid_sdk-2.1.81/lusid/models/instrument_payment_diary_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_properties.py` & `lusid_sdk-2.1.81/lusid/models/instrument_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_resolution_detail.py` & `lusid_sdk-2.1.81/lusid/models/instrument_resolution_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_search_property.py` & `lusid_sdk-2.1.81/lusid/models/instrument_search_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/instrument_type.py` & `lusid_sdk-2.1.81/lusid/models/instrument_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/interest_rate_swap.py` & `lusid_sdk-2.1.81/lusid/models/interest_rate_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/interest_rate_swaption.py` & `lusid_sdk-2.1.81/lusid/models/interest_rate_swaption.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/intermediate_compliance_step.py` & `lusid_sdk-2.1.81/lusid/models/intermediate_compliance_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/ir_vol_cube_data.py` & `lusid_sdk-2.1.81/lusid/models/ir_vol_cube_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/ir_vol_dependency.py` & `lusid_sdk-2.1.81/lusid/models/ir_vol_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/is_business_day_response.py` & `lusid_sdk-2.1.81/lusid/models/is_business_day_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/journal_entry_line.py` & `lusid_sdk-2.1.81/lusid/models/journal_entry_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/journal_entry_lines_query_parameters.py` & `lusid_sdk-2.1.81/lusid/models/journal_entry_lines_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/label_value_set.py` & `lusid_sdk-2.1.81/lusid/models/label_value_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/leg_definition.py` & `lusid_sdk-2.1.81/lusid/models/leg_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/legal_entity.py` & `lusid_sdk-2.1.81/lusid/models/legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/level_step.py` & `lusid_sdk-2.1.81/lusid/models/level_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/life_cycle_event_lineage.py` & `lusid_sdk-2.1.81/lusid/models/life_cycle_event_lineage.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/life_cycle_event_value.py` & `lusid_sdk-2.1.81/lusid/models/life_cycle_event_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lineage_member.py` & `lusid_sdk-2.1.81/lusid/models/lineage_member.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/link.py` & `lusid_sdk-2.1.81/lusid/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/list_aggregation_reconciliation.py` & `lusid_sdk-2.1.81/lusid/models/list_aggregation_reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/list_aggregation_response.py` & `lusid_sdk-2.1.81/lusid/models/list_aggregation_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/list_complex_market_data_with_meta_data_response.py` & `lusid_sdk-2.1.81/lusid/models/list_complex_market_data_with_meta_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/loan_period.py` & `lusid_sdk-2.1.81/lusid/models/loan_period.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lock_period_diary_entry_request.py` & `lusid_sdk-2.1.81/lusid/models/lock_period_diary_entry_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lusid_instrument.py` & `lusid_sdk-2.1.81/lusid/models/lusid_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lusid_problem_details.py` & `lusid_sdk-2.1.81/lusid/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lusid_trade_ticket.py` & `lusid_sdk-2.1.81/lusid/models/lusid_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lusid_unique_id.py` & `lusid_sdk-2.1.81/lusid/models/lusid_unique_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/lusid_validation_problem_details.py` & `lusid_sdk-2.1.81/lusid/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/mapped_string.py` & `lusid_sdk-2.1.81/lusid/models/mapped_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/mapping.py` & `lusid_sdk-2.1.81/lusid/models/mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/mapping_rule.py` & `lusid_sdk-2.1.81/lusid/models/mapping_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_context.py` & `lusid_sdk-2.1.81/lusid/models/market_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_context_suppliers.py` & `lusid_sdk-2.1.81/lusid/models/market_context_suppliers.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_key_rule.py` & `lusid_sdk-2.1.81/lusid/models/market_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_options.py` & `lusid_sdk-2.1.81/lusid/models/market_data_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_options_type.py` & `lusid_sdk-2.1.81/lusid/models/market_data_options_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_overrides.py` & `lusid_sdk-2.1.81/lusid/models/market_data_overrides.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_specific_rule.py` & `lusid_sdk-2.1.81/lusid/models/market_data_specific_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_data_type.py` & `lusid_sdk-2.1.81/lusid/models/market_data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_observable_type.py` & `lusid_sdk-2.1.81/lusid/models/market_observable_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_options.py` & `lusid_sdk-2.1.81/lusid/models/market_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/market_quote.py` & `lusid_sdk-2.1.81/lusid/models/market_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/match_criterion.py` & `lusid_sdk-2.1.81/lusid/models/match_criterion.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/maturity_event.py` & `lusid_sdk-2.1.81/lusid/models/maturity_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/metric_value.py` & `lusid_sdk-2.1.81/lusid/models/metric_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/model_options.py` & `lusid_sdk-2.1.81/lusid/models/model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/model_options_type.py` & `lusid_sdk-2.1.81/lusid/models/model_options_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/model_property.py` & `lusid_sdk-2.1.81/lusid/models/model_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/model_schema.py` & `lusid_sdk-2.1.81/lusid/models/model_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/model_selection.py` & `lusid_sdk-2.1.81/lusid/models/model_selection.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/move_orders_to_different_blocks_request.py` & `lusid_sdk-2.1.81/lusid/models/move_orders_to_different_blocks_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/moved_order_to_different_block_response.py` & `lusid_sdk-2.1.81/lusid/models/moved_order_to_different_block_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/movement_type.py` & `lusid_sdk-2.1.81/lusid/models/movement_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/multi_currency_amounts.py` & `lusid_sdk-2.1.81/lusid/models/multi_currency_amounts.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/next_value_in_sequence_response.py` & `lusid_sdk-2.1.81/lusid/models/next_value_in_sequence_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/numeric_comparison_type.py` & `lusid_sdk-2.1.81/lusid/models/numeric_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/opaque_dependency.py` & `lusid_sdk-2.1.81/lusid/models/opaque_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/opaque_market_data.py` & `lusid_sdk-2.1.81/lusid/models/opaque_market_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/opaque_model_options.py` & `lusid_sdk-2.1.81/lusid/models/opaque_model_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/open_event.py` & `lusid_sdk-2.1.81/lusid/models/open_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/operand_type.py` & `lusid_sdk-2.1.81/lusid/models/operand_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/operation.py` & `lusid_sdk-2.1.81/lusid/models/operation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/operation_type.py` & `lusid_sdk-2.1.81/lusid/models/operation_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/operator.py` & `lusid_sdk-2.1.81/lusid/models/operator.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/option_entry.py` & `lusid_sdk-2.1.81/lusid/models/option_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/optionality_schedule.py` & `lusid_sdk-2.1.81/lusid/models/optionality_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order.py` & `lusid_sdk-2.1.81/lusid/models/order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_by_spec.py` & `lusid_sdk-2.1.81/lusid/models/order_by_spec.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_flow_configuration.py` & `lusid_sdk-2.1.81/lusid/models/order_flow_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_allocation_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_allocation_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_allocation_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_allocation_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_execution_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_execution_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_execution_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_execution_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_order_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_order_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_order_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_order_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_placement_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_placement_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_placement_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_placement_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_transaction_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_block_transaction_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_block_transaction_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_allocation_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_allocation_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_allocation_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_allocation_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_child_placement_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_child_placement_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_execution_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_execution_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_execution_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_execution_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_order_detail.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_order_detail.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_order_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_order_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_graph_placement_placement_synopsis.py` & `lusid_sdk-2.1.81/lusid/models/order_graph_placement_placement_synopsis.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_instruction.py` & `lusid_sdk-2.1.81/lusid/models/order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_instruction_request.py` & `lusid_sdk-2.1.81/lusid/models/order_instruction_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_instruction_set_request.py` & `lusid_sdk-2.1.81/lusid/models/order_instruction_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_request.py` & `lusid_sdk-2.1.81/lusid/models/order_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/order_set_request.py` & `lusid_sdk-2.1.81/lusid/models/order_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/otc_confirmation.py` & `lusid_sdk-2.1.81/lusid/models/otc_confirmation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/output_transaction.py` & `lusid_sdk-2.1.81/lusid/models/output_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     source: Optional[StrictStr] = Field(None, description="The source of the transaction. This is used to look up the appropriate transaction group set in the transaction type configuration.")
     transaction_status: Optional[StrictStr] = Field(None, alias="transactionStatus", description="The status of the transaction. The available values are: Active, Amended, Cancelled")
     entry_date_time: Optional[datetime] = Field(None, alias="entryDateTime", description="The asAt datetime that the transaction was added to LUSID.")
     cancel_date_time: Optional[datetime] = Field(None, alias="cancelDateTime", description="If the transaction has been cancelled, the asAt datetime that the transaction was cancelled.")
     realised_gain_loss: Optional[conlist(RealisedGainLoss)] = Field(None, alias="realisedGainLoss", description="The collection of realised gains or losses resulting from relevant transactions e.g. a sale transaction. The cost used in calculating the realised gain or loss is determined by the accounting method defined when the transaction portfolio is created.")
     holding_ids: Optional[conlist(StrictInt)] = Field(None, alias="holdingIds", description="The collection of single identifiers for the holding within the portfolio. The holdingId is constructed from the LusidInstrumentId, sub-holding keys and currrency and is unique within the portfolio.")
     source_type: Optional[StrictStr] = Field(None, alias="sourceType", description="The type of source that the transaction originated from, eg: InputTransaction, InstrumentEvent, HoldingAdjustment")
-    __properties = ["transactionId", "type", "description", "instrumentIdentifiers", "instrumentScope", "instrumentUid", "transactionDate", "settlementDate", "units", "transactionAmount", "transactionPrice", "totalConsideration", "exchangeRate", "transactionToPortfolioRate", "transactionCurrency", "properties", "counterpartyId", "source", "transactionStatus", "entryDateTime", "cancelDateTime", "realisedGainLoss", "holdingIds", "sourceType"]
+    source_instrument_event_id: Optional[StrictStr] = Field(None, alias="sourceInstrumentEventId", description="The unique ID of the instrument event that the transaction is related to.")
+    __properties = ["transactionId", "type", "description", "instrumentIdentifiers", "instrumentScope", "instrumentUid", "transactionDate", "settlementDate", "units", "transactionAmount", "transactionPrice", "totalConsideration", "exchangeRate", "transactionToPortfolioRate", "transactionCurrency", "properties", "counterpartyId", "source", "transactionStatus", "entryDateTime", "cancelDateTime", "realisedGainLoss", "holdingIds", "sourceType", "sourceInstrumentEventId"]
 
     @validator('transaction_status')
     def transaction_status_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -165,14 +166,19 @@
             _dict['holdingIds'] = None
 
         # set to None if source_type (nullable) is None
         # and __fields_set__ contains the field
         if self.source_type is None and "source_type" in self.__fields_set__:
             _dict['sourceType'] = None
 
+        # set to None if source_instrument_event_id (nullable) is None
+        # and __fields_set__ contains the field
+        if self.source_instrument_event_id is None and "source_instrument_event_id" in self.__fields_set__:
+            _dict['sourceInstrumentEventId'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> OutputTransaction:
         """Create an instance of OutputTransaction from a dict"""
         if obj is None:
             return None
@@ -205,10 +211,11 @@
             "counterparty_id": obj.get("counterpartyId"),
             "source": obj.get("source"),
             "transaction_status": obj.get("transactionStatus"),
             "entry_date_time": obj.get("entryDateTime"),
             "cancel_date_time": obj.get("cancelDateTime"),
             "realised_gain_loss": [RealisedGainLoss.from_dict(_item) for _item in obj.get("realisedGainLoss")] if obj.get("realisedGainLoss") is not None else None,
             "holding_ids": obj.get("holdingIds"),
-            "source_type": obj.get("sourceType")
+            "source_type": obj.get("sourceType"),
+            "source_instrument_event_id": obj.get("sourceInstrumentEventId")
         })
         return _obj
```

### Comparing `lusid_sdk-2.1.79/lusid/models/output_transition.py` & `lusid_sdk-2.1.81/lusid/models/output_transition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/package.py` & `lusid_sdk-2.1.81/lusid/models/package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/package_request.py` & `lusid_sdk-2.1.81/lusid/models/package_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/package_set_request.py` & `lusid_sdk-2.1.81/lusid/models/package_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_abor.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_abor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_abor_configuration.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_abor_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_account.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_address_key_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_allocation.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_amortisation_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_amortisation_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_block.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_calendar.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_calendar.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_chart_of_accounts.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_chart_of_accounts.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cleardown_module_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cleardown_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cleardown_module_rule.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cleardown_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_rule_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_rule_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_run_info_v2.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_run_info_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_compliance_template.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_compliance_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_corporate_action_source.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_corporate_action_source.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custodian_account.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custodian_account.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_custom_entity_type.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_custom_entity_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_cut_label_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_cut_label_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_data_type_summary.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_data_type_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_dialect_id.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_dialect_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_diary_entry.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_diary_entry.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_execution.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_fund.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_fund.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_general_ledger_profile_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_general_ledger_profile_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_instrument.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_instrument_event_holder.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_legal_entity.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_graph_block.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_graph_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_graph_placement.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_graph_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_order_instruction.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_package.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_participation.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_person.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_placement.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_group.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_group_search_result.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_group_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_portfolio_search_result.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_portfolio_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_posting_module_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_posting_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_posting_module_rule.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_posting_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_property_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_property_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_property_definition_search_result.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_property_definition_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_reconciliation.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_reference_list_response.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_reference_list_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_relationship_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_relationship_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_sequence_definition.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_sequence_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_staging_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_staging_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_transaction_template.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_transaction_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_transaction_template_specification.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_transaction_template_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_translation_script_id.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_translation_script_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/paged_resource_list_of_virtual_row.py` & `lusid_sdk-2.1.81/lusid/models/paged_resource_list_of_virtual_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/participation.py` & `lusid_sdk-2.1.81/lusid/models/participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/participation_request.py` & `lusid_sdk-2.1.81/lusid/models/participation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/participation_set_request.py` & `lusid_sdk-2.1.81/lusid/models/participation_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/performance_return.py` & `lusid_sdk-2.1.81/lusid/models/performance_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/performance_returns_metric.py` & `lusid_sdk-2.1.81/lusid/models/performance_returns_metric.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/period_diary_entries_reopened_response.py` & `lusid_sdk-2.1.81/lusid/models/period_diary_entries_reopened_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/period_type.py` & `lusid_sdk-2.1.81/lusid/models/period_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/perpetual_entity_state.py` & `lusid_sdk-2.1.81/lusid/models/perpetual_entity_state.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/perpetual_property.py` & `lusid_sdk-2.1.81/lusid/models/perpetual_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/person.py` & `lusid_sdk-2.1.81/lusid/models/person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/place_blocks_request.py` & `lusid_sdk-2.1.81/lusid/models/place_blocks_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/placement.py` & `lusid_sdk-2.1.81/lusid/models/placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/placement_request.py` & `lusid_sdk-2.1.81/lusid/models/placement_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/placement_set_request.py` & `lusid_sdk-2.1.81/lusid/models/placement_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio.py` & `lusid_sdk-2.1.81/lusid/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_cash_flow.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_cash_ladder.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_cash_ladder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_details.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_entity.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic.v1 import BaseModel, Field, StrictStr, conlist, constr
 from lusid.models.link import Link
 from lusid.models.portfolio_without_href import PortfolioWithoutHref
 
 class PortfolioEntity(BaseModel):
     """
     A list of portfolios.  # noqa: E501
     """
     href: StrictStr = Field(..., description="The specific Uniform Resource Identifier (URI) for this resource at the requested effective and asAt datetime.")
     entity_unique_id: constr(strict=True, min_length=1) = Field(..., alias="entityUniqueId", description="The unique id of the entity")
     status: constr(strict=True, min_length=1) = Field(..., description="The status of the entity at the current time")
+    effective_at_created: Optional[datetime] = Field(None, alias="effectiveAtCreated", description="The EffectiveAt this Entity is created, if entity does not currently exist in EffectiveAt")
     prevailing_portfolio: Optional[PortfolioWithoutHref] = Field(None, alias="prevailingPortfolio")
     deleted_portfolio: Optional[PortfolioWithoutHref] = Field(None, alias="deletedPortfolio")
     links: Optional[conlist(Link)] = None
-    __properties = ["href", "entityUniqueId", "status", "prevailingPortfolio", "deletedPortfolio", "links"]
+    __properties = ["href", "entityUniqueId", "status", "effectiveAtCreated", "prevailingPortfolio", "deletedPortfolio", "links"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -68,14 +69,19 @@
         # override the default output from pydantic by calling `to_dict()` of each item in links (list)
         _items = []
         if self.links:
             for _item in self.links:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['links'] = _items
+        # set to None if effective_at_created (nullable) is None
+        # and __fields_set__ contains the field
+        if self.effective_at_created is None and "effective_at_created" in self.__fields_set__:
+            _dict['effectiveAtCreated'] = None
+
         # set to None if links (nullable) is None
         # and __fields_set__ contains the field
         if self.links is None and "links" in self.__fields_set__:
             _dict['links'] = None
 
         return _dict
 
@@ -88,12 +94,13 @@
         if not isinstance(obj, dict):
             return PortfolioEntity.parse_obj(obj)
 
         _obj = PortfolioEntity.parse_obj({
             "href": obj.get("href"),
             "entity_unique_id": obj.get("entityUniqueId"),
             "status": obj.get("status"),
+            "effective_at_created": obj.get("effectiveAtCreated"),
             "prevailing_portfolio": PortfolioWithoutHref.from_dict(obj.get("prevailingPortfolio")) if obj.get("prevailingPortfolio") is not None else None,
             "deleted_portfolio": PortfolioWithoutHref.from_dict(obj.get("deletedPortfolio")) if obj.get("deletedPortfolio") is not None else None,
             "links": [Link.from_dict(_item) for _item in obj.get("links")] if obj.get("links") is not None else None
         })
         return _obj
```

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_entity_id.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_entity_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group_id_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group_id_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group_id_list.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group_id_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group_id_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group_id_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group_properties.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_group_search_result.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_group_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_holding.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_id_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_id_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_id_list.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_id_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_id_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_id_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_properties.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_properties.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_result_data_key_rule.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_result_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_return_breakdown.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_return_breakdown.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_search_result.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_trade_ticket.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_type.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolio_without_href.py` & `lusid_sdk-2.1.81/lusid/models/portfolio_without_href.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/portfolios_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/portfolios_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/posting_module_details.py` & `lusid_sdk-2.1.81/lusid/models/posting_module_details.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/posting_module_request.py` & `lusid_sdk-2.1.81/lusid/models/posting_module_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/posting_module_response.py` & `lusid_sdk-2.1.81/lusid/models/posting_module_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/posting_module_rule.py` & `lusid_sdk-2.1.81/lusid/models/posting_module_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/posting_module_rules_updated_response.py` & `lusid_sdk-2.1.81/lusid/models/posting_module_rules_updated_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/premium.py` & `lusid_sdk-2.1.81/lusid/models/premium.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/pricing_context.py` & `lusid_sdk-2.1.81/lusid/models/pricing_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/pricing_model.py` & `lusid_sdk-2.1.81/lusid/models/pricing_model.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/pricing_options.py` & `lusid_sdk-2.1.81/lusid/models/pricing_options.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/processed_command.py` & `lusid_sdk-2.1.81/lusid/models/processed_command.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_definition.py` & `lusid_sdk-2.1.81/lusid/models/property_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_definition_search_result.py` & `lusid_sdk-2.1.81/lusid/models/property_definition_search_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_definition_type.py` & `lusid_sdk-2.1.81/lusid/models/property_definition_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_domain.py` & `lusid_sdk-2.1.81/lusid/models/property_domain.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_filter.py` & `lusid_sdk-2.1.81/lusid/models/property_filter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_interval.py` & `lusid_sdk-2.1.81/lusid/models/property_interval.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_key_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/property_key_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_key_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/property_key_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_life_time.py` & `lusid_sdk-2.1.81/lusid/models/property_life_time.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_list.py` & `lusid_sdk-2.1.81/lusid/models/property_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/property_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_schema.py` & `lusid_sdk-2.1.81/lusid/models/property_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_type.py` & `lusid_sdk-2.1.81/lusid/models/property_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_value.py` & `lusid_sdk-2.1.81/lusid/models/property_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_value_equals.py` & `lusid_sdk-2.1.81/lusid/models/property_value_equals.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/property_value_in.py` & `lusid_sdk-2.1.81/lusid/models/property_value_in.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/query_bucketed_cash_flows_request.py` & `lusid_sdk-2.1.81/lusid/models/query_bucketed_cash_flows_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/query_cash_flows_request.py` & `lusid_sdk-2.1.81/lusid/models/query_cash_flows_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/query_instrument_events_request.py` & `lusid_sdk-2.1.81/lusid/models/query_instrument_events_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/query_trade_tickets_request.py` & `lusid_sdk-2.1.81/lusid/models/query_trade_tickets_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/queryable_key.py` & `lusid_sdk-2.1.81/lusid/models/queryable_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote.py` & `lusid_sdk-2.1.81/lusid/models/quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_access_metadata_rule.py` & `lusid_sdk-2.1.81/lusid/models/quote_access_metadata_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_access_metadata_rule_id.py` & `lusid_sdk-2.1.81/lusid/models/quote_access_metadata_rule_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_dependency.py` & `lusid_sdk-2.1.81/lusid/models/quote_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_id.py` & `lusid_sdk-2.1.81/lusid/models/quote_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_instrument_id_type.py` & `lusid_sdk-2.1.81/lusid/models/quote_instrument_id_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_series_id.py` & `lusid_sdk-2.1.81/lusid/models/quote_series_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/quote_type.py` & `lusid_sdk-2.1.81/lusid/models/quote_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/raw_vendor_event.py` & `lusid_sdk-2.1.81/lusid/models/raw_vendor_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/re_open_period_diary_entry_request.py` & `lusid_sdk-2.1.81/lusid/models/re_open_period_diary_entry_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/realised_gain_loss.py` & `lusid_sdk-2.1.81/lusid/models/realised_gain_loss.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/recipe_block.py` & `lusid_sdk-2.1.81/lusid/models/recipe_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/recipe_composer.py` & `lusid_sdk-2.1.81/lusid/models/recipe_composer.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/recipe_value.py` & `lusid_sdk-2.1.81/lusid/models/recipe_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/recombine_step.py` & `lusid_sdk-2.1.81/lusid/models/recombine_step.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconcile_date_time_rule.py` & `lusid_sdk-2.1.81/lusid/models/reconcile_date_time_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconcile_numeric_rule.py` & `lusid_sdk-2.1.81/lusid/models/reconcile_numeric_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconcile_string_rule.py` & `lusid_sdk-2.1.81/lusid/models/reconcile_string_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciled_transaction.py` & `lusid_sdk-2.1.81/lusid/models/reconciled_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_break.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_configuration.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_id.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_left_right_address_key_pair.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_left_right_address_key_pair.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_line.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_response.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_rule.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_rule_type.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_rule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_side_configuration.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_side_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reconciliation_transactions.py` & `lusid_sdk-2.1.81/lusid/models/reconciliation_transactions.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_data.py` & `lusid_sdk-2.1.81/lusid/models/reference_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_instrument.py` & `lusid_sdk-2.1.81/lusid/models/reference_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_list.py` & `lusid_sdk-2.1.81/lusid/models/reference_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_list_request.py` & `lusid_sdk-2.1.81/lusid/models/reference_list_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_list_response.py` & `lusid_sdk-2.1.81/lusid/models/reference_list_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_list_type.py` & `lusid_sdk-2.1.81/lusid/models/reference_list_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_portfolio_constituent.py` & `lusid_sdk-2.1.81/lusid/models/reference_portfolio_constituent.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_portfolio_constituent_request.py` & `lusid_sdk-2.1.81/lusid/models/reference_portfolio_constituent_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reference_portfolio_weight_type.py` & `lusid_sdk-2.1.81/lusid/models/reference_portfolio_weight_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/related_entity.py` & `lusid_sdk-2.1.81/lusid/models/related_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/relation.py` & `lusid_sdk-2.1.81/lusid/models/relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/relation_definition.py` & `lusid_sdk-2.1.81/lusid/models/relation_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/relationship.py` & `lusid_sdk-2.1.81/lusid/models/relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/relationship_definition.py` & `lusid_sdk-2.1.81/lusid/models/relationship_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/relative_date_offset.py` & `lusid_sdk-2.1.81/lusid/models/relative_date_offset.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/repo.py` & `lusid_sdk-2.1.81/lusid/models/repo.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reset_event.py` & `lusid_sdk-2.1.81/lusid/models/reset_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_id.py` & `lusid_sdk-2.1.81/lusid/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_access_controlled_resource.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_access_metadata_value_of.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_access_metadata_value_of.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_address_key_definition.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_address_key_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_aggregated_return.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_aggregated_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_aggregation_query.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_aggregation_query.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_allocation.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_allocation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_block.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_block.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_block_and_orders.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_block_and_orders.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_calendar_date.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_calendar_date.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_change.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_change.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_change_history.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_change_history.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_breached_order_info.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_breached_order_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_rule.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_rule_result.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_rule_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_compliance_run_info.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_compliance_run_info.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_constituents_adjustment_header.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_constituents_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_corporate_action.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_corporate_action.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_data_type.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_data_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_execution.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_execution.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_fee_rule.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_fee_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_cds_flow_conventions_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_cds_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_counterparty_agreement_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_counterparty_agreement_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_credit_support_annex_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_credit_support_annex_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_flow_conventions_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_flow_conventions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_index_convention_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_index_convention_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_recipe_composer_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_recipe_composer_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_get_recipe_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_get_recipe_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_holdings_adjustment_header.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_holdings_adjustment_header.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_i_unit_definition_dto.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_i_unit_definition_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_cash_flow.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_event_holder.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_event_holder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_instrument_id_type_descriptor.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_instrument_id_type_descriptor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_legal_entity.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_legal_entity.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_list_complex_market_data_with_meta_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_mapping.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_moved_order_to_different_block_response.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_moved_order_to_different_block_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_order.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_order_instruction.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_order_instruction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_package.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_package.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_participation.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_participation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_performance_return.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_performance_return.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_person.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_person.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_placement.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_placement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_cash_flow.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_cash_flow.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_cash_ladder.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_cash_ladder.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_portfolio_trade_ticket.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_portfolio_trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_processed_command.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_processed_command.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_property.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_property.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_property_definition.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_property_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_property_interval.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_property_interval.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_queryable_key.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_queryable_key.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_quote.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_quote.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_quote_access_metadata_rule.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_quote_access_metadata_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_reconciliation_break.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_reconciliation_break.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_relation.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_relation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_relationship.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_relationship.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_scope_definition.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_scope_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_side_definition.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_side_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_string.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_tax_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_tax_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_transaction.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_transaction_type.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_transaction_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/resource_list_of_value_type.py` & `lusid_sdk-2.1.81/lusid/models/resource_list_of_value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/response_meta_data.py` & `lusid_sdk-2.1.81/lusid/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_data_key_rule.py` & `lusid_sdk-2.1.81/lusid/models/result_data_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_data_schema.py` & `lusid_sdk-2.1.81/lusid/models/result_data_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_key_rule.py` & `lusid_sdk-2.1.81/lusid/models/result_key_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_key_rule_type.py` & `lusid_sdk-2.1.81/lusid/models/result_key_rule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value.py` & `lusid_sdk-2.1.81/lusid/models/result_value.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value0_d.py` & `lusid_sdk-2.1.81/lusid/models/result_value0_d.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_bool.py` & `lusid_sdk-2.1.81/lusid/models/result_value_bool.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_currency.py` & `lusid_sdk-2.1.81/lusid/models/result_value_currency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_date_time_offset.py` & `lusid_sdk-2.1.81/lusid/models/result_value_date_time_offset.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_decimal.py` & `lusid_sdk-2.1.81/lusid/models/result_value_decimal.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_dictionary.py` & `lusid_sdk-2.1.81/lusid/models/result_value_dictionary.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_int.py` & `lusid_sdk-2.1.81/lusid/models/result_value_int.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_string.py` & `lusid_sdk-2.1.81/lusid/models/result_value_string.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/result_value_type.py` & `lusid_sdk-2.1.81/lusid/models/result_value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/reverse_stock_split_event.py` & `lusid_sdk-2.1.81/lusid/models/reverse_stock_split_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/rounding_configuration.py` & `lusid_sdk-2.1.81/lusid/models/rounding_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/rounding_configuration_component.py` & `lusid_sdk-2.1.81/lusid/models/rounding_configuration_component.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/rounding_convention.py` & `lusid_sdk-2.1.81/lusid/models/rounding_convention.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/scaling_methodology.py` & `lusid_sdk-2.1.81/lusid/models/scaling_methodology.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/schedule.py` & `lusid_sdk-2.1.81/lusid/models/schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/schedule_type.py` & `lusid_sdk-2.1.81/lusid/models/schedule_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/scope_definition.py` & `lusid_sdk-2.1.81/lusid/models/scope_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/scrip_dividend_event.py` & `lusid_sdk-2.1.81/lusid/models/scrip_dividend_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/script_map_reference.py` & `lusid_sdk-2.1.81/lusid/models/script_map_reference.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/security_election.py` & `lusid_sdk-2.1.81/lusid/models/security_election.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/sequence_definition.py` & `lusid_sdk-2.1.81/lusid/models/sequence_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_legal_entity_identifiers_request.py` & `lusid_sdk-2.1.81/lusid/models/set_legal_entity_identifiers_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_legal_entity_properties_request.py` & `lusid_sdk-2.1.81/lusid/models/set_legal_entity_properties_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_person_identifiers_request.py` & `lusid_sdk-2.1.81/lusid/models/set_person_identifiers_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_person_properties_request.py` & `lusid_sdk-2.1.81/lusid/models/set_person_properties_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_share_class_instruments_request.py` & `lusid_sdk-2.1.81/lusid/models/set_share_class_instruments_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_transaction_configuration_alias.py` & `lusid_sdk-2.1.81/lusid/models/set_transaction_configuration_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/set_transaction_configuration_source_request.py` & `lusid_sdk-2.1.81/lusid/models/set_transaction_configuration_source_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/side_configuration_data.py` & `lusid_sdk-2.1.81/lusid/models/side_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/side_configuration_data_request.py` & `lusid_sdk-2.1.81/lusid/models/side_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/side_definition.py` & `lusid_sdk-2.1.81/lusid/models/side_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/side_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/side_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/sides_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/sides_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/simple_cash_flow_loan.py` & `lusid_sdk-2.1.81/lusid/models/simple_cash_flow_loan.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/simple_instrument.py` & `lusid_sdk-2.1.81/lusid/models/simple_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/sort_order.py` & `lusid_sdk-2.1.81/lusid/models/sort_order.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/staging_rule.py` & `lusid_sdk-2.1.81/lusid/models/staging_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/staging_rule_approval_criteria.py` & `lusid_sdk-2.1.81/lusid/models/staging_rule_approval_criteria.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/staging_rule_match_criteria.py` & `lusid_sdk-2.1.81/lusid/models/staging_rule_match_criteria.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/staging_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/staging_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/step_schedule.py` & `lusid_sdk-2.1.81/lusid/models/step_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/stock_dividend_event.py` & `lusid_sdk-2.1.81/lusid/models/stock_dividend_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/stock_split_event.py` & `lusid_sdk-2.1.81/lusid/models/stock_split_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/stream.py` & `lusid_sdk-2.1.81/lusid/models/stream.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/string_comparison_type.py` & `lusid_sdk-2.1.81/lusid/models/string_comparison_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/string_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/string_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/string_list.py` & `lusid_sdk-2.1.81/lusid/models/string_list.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/string_list_compliance_parameter.py` & `lusid_sdk-2.1.81/lusid/models/string_list_compliance_parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/structured_result_data.py` & `lusid_sdk-2.1.81/lusid/models/structured_result_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/structured_result_data_id.py` & `lusid_sdk-2.1.81/lusid/models/structured_result_data_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/sub_holding_key_value_equals.py` & `lusid_sdk-2.1.81/lusid/models/sub_holding_key_value_equals.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/target_tax_lot.py` & `lusid_sdk-2.1.81/lusid/models/target_tax_lot.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/target_tax_lot_request.py` & `lusid_sdk-2.1.81/lusid/models/target_tax_lot_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/tax_rule.py` & `lusid_sdk-2.1.81/lusid/models/tax_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/tax_rule_set.py` & `lusid_sdk-2.1.81/lusid/models/tax_rule_set.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/template_field.py` & `lusid_sdk-2.1.81/lusid/models/template_field.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/term_deposit.py` & `lusid_sdk-2.1.81/lusid/models/term_deposit.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/total_return_swap.py` & `lusid_sdk-2.1.81/lusid/models/total_return_swap.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/touch.py` & `lusid_sdk-2.1.81/lusid/models/touch.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/trade_ticket.py` & `lusid_sdk-2.1.81/lusid/models/trade_ticket.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/trade_ticket_type.py` & `lusid_sdk-2.1.81/lusid/models/trade_ticket_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction.py` & `lusid_sdk-2.1.81/lusid/models/transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_configuration_data.py` & `lusid_sdk-2.1.81/lusid/models/transaction_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_configuration_data_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_configuration_movement_data.py` & `lusid_sdk-2.1.81/lusid/models/transaction_configuration_movement_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_configuration_movement_data_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_configuration_movement_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_configuration_type_alias.py` & `lusid_sdk-2.1.81/lusid/models/transaction_configuration_type_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_currency_and_amount.py` & `lusid_sdk-2.1.81/lusid/models/transaction_currency_and_amount.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_field_map.py` & `lusid_sdk-2.1.81/lusid/models/transaction_field_map.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_price.py` & `lusid_sdk-2.1.81/lusid/models/transaction_price.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_price_and_type.py` & `lusid_sdk-2.1.81/lusid/models/transaction_price_and_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_price_type.py` & `lusid_sdk-2.1.81/lusid/models/transaction_price_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_property_map.py` & `lusid_sdk-2.1.81/lusid/models/transaction_property_map.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_property_mapping.py` & `lusid_sdk-2.1.81/lusid/models/transaction_property_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_property_mapping_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_property_mapping_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_query_mode.py` & `lusid_sdk-2.1.81/lusid/models/transaction_query_mode.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_query_parameters.py` & `lusid_sdk-2.1.81/lusid/models/transaction_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_reconciliation_request_v2.py` & `lusid_sdk-2.1.81/lusid/models/transaction_reconciliation_request_v2.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_roles.py` & `lusid_sdk-2.1.81/lusid/models/transaction_roles.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_set_configuration_data.py` & `lusid_sdk-2.1.81/lusid/models/transaction_set_configuration_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_set_configuration_data_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_set_configuration_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_status.py` & `lusid_sdk-2.1.81/lusid/models/transaction_status.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_template.py` & `lusid_sdk-2.1.81/lusid/models/transaction_template.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_template_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_template_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_template_specification.py` & `lusid_sdk-2.1.81/lusid/models/transaction_template_specification.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type_alias.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type_alias.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type_calculation.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type_calculation.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type_movement.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type_movement.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type_property_mapping.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type_property_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transaction_type_request.py` & `lusid_sdk-2.1.81/lusid/models/transaction_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transactions_reconciliations_response.py` & `lusid_sdk-2.1.81/lusid/models/transactions_reconciliations_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/transition_event.py` & `lusid_sdk-2.1.81/lusid/models/transition_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_entities_inlined_request.py` & `lusid_sdk-2.1.81/lusid/models/translate_entities_inlined_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_entities_request.py` & `lusid_sdk-2.1.81/lusid/models/translate_entities_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_entities_response.py` & `lusid_sdk-2.1.81/lusid/models/translate_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_instrument_definitions_request.py` & `lusid_sdk-2.1.81/lusid/models/translate_instrument_definitions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_instrument_definitions_response.py` & `lusid_sdk-2.1.81/lusid/models/translate_instrument_definitions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_trade_ticket_request.py` & `lusid_sdk-2.1.81/lusid/models/translate_trade_ticket_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translate_trade_tickets_response.py` & `lusid_sdk-2.1.81/lusid/models/translate_trade_tickets_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translation_context.py` & `lusid_sdk-2.1.81/lusid/models/translation_context.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translation_input.py` & `lusid_sdk-2.1.81/lusid/models/translation_input.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translation_result.py` & `lusid_sdk-2.1.81/lusid/models/translation_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translation_script.py` & `lusid_sdk-2.1.81/lusid/models/translation_script.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/translation_script_id.py` & `lusid_sdk-2.1.81/lusid/models/translation_script_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/trial_balance.py` & `lusid_sdk-2.1.81/lusid/models/trial_balance.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/trial_balance_query_parameters.py` & `lusid_sdk-2.1.81/lusid/models/trial_balance_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/trigger_event.py` & `lusid_sdk-2.1.81/lusid/models/trigger_event.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/typed_resource_id.py` & `lusid_sdk-2.1.81/lusid/models/typed_resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/unit_schema.py` & `lusid_sdk-2.1.81/lusid/models/unit_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/units_ratio.py` & `lusid_sdk-2.1.81/lusid/models/units_ratio.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/unmatched_holding_method.py` & `lusid_sdk-2.1.81/lusid/models/unmatched_holding_method.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_amortisation_rule_set_details_request.py` & `lusid_sdk-2.1.81/lusid/models/update_amortisation_rule_set_details_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_calendar_request.py` & `lusid_sdk-2.1.81/lusid/models/update_calendar_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_custom_entity_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/update_custom_entity_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_custom_entity_type_request.py` & `lusid_sdk-2.1.81/lusid/models/update_custom_entity_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_cut_label_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/update_cut_label_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_data_type_request.py` & `lusid_sdk-2.1.81/lusid/models/update_data_type_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_derived_property_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/update_derived_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_instrument_identifier_request.py` & `lusid_sdk-2.1.81/lusid/models/update_instrument_identifier_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_portfolio_group_request.py` & `lusid_sdk-2.1.81/lusid/models/update_portfolio_group_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_portfolio_request.py` & `lusid_sdk-2.1.81/lusid/models/update_portfolio_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_property_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/update_property_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/update_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_relationship_definition_request.py` & `lusid_sdk-2.1.81/lusid/models/update_relationship_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_staging_rule_set_request.py` & `lusid_sdk-2.1.81/lusid/models/update_staging_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_tax_rule_set_request.py` & `lusid_sdk-2.1.81/lusid/models/update_tax_rule_set_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/update_unit_request.py` & `lusid_sdk-2.1.81/lusid/models/update_unit_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_cds_flow_conventions_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_cds_flow_conventions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_complex_market_data_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_complex_market_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_compliance_rule_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_compliance_rule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_compliance_run_summary_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_compliance_run_summary_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_compliance_run_summary_result.py` & `lusid_sdk-2.1.81/lusid/models/upsert_compliance_run_summary_result.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_corporate_action_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_corporate_action_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_corporate_actions_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_corporate_actions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_counterparty_agreement_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_counterparty_agreement_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_credit_support_annex_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_credit_support_annex_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_custom_entities_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_custom_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_custom_entity_access_metadata_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_custom_entity_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_dialect_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_dialect_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_flow_conventions_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_flow_conventions_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_index_convention_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_index_convention_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_instrument_event_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_instrument_event_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_instrument_events_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_instrument_events_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_instrument_properties_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_instrument_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_instrument_property_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_instrument_property_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_instruments_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_instruments_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_legal_entities_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_legal_entities_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_legal_entity_access_metadata_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_legal_entity_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_legal_entity_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_legal_entity_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_person_access_metadata_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_person_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_person_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_person_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_portfolio_access_metadata_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_portfolio_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_portfolio_group_access_metadata_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_portfolio_group_access_metadata_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_portfolio_transactions_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_portfolio_transactions_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_quote_access_metadata_rule_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_quote_access_metadata_rule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_quote_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_quote_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_quotes_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_quotes_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_recipe_composer_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_recipe_composer_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_recipe_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_recipe_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_reference_portfolio_constituents_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_reference_portfolio_constituents_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_reference_portfolio_constituents_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_reference_portfolio_constituents_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_result_values_data_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_result_values_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_returns_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_returns_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_single_structured_data_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_single_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_structured_data_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_structured_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_structured_result_data_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_structured_result_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_transaction_properties_response.py` & `lusid_sdk-2.1.81/lusid/models/upsert_transaction_properties_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_translation_script_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_translation_script_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/upsert_valuation_point_request.py` & `lusid_sdk-2.1.81/lusid/models/upsert_valuation_point_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/user.py` & `lusid_sdk-2.1.81/lusid/models/user.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuation_point_data_query_parameters.py` & `lusid_sdk-2.1.81/lusid/models/valuation_point_data_query_parameters.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuation_point_data_request.py` & `lusid_sdk-2.1.81/lusid/models/valuation_point_data_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuation_point_data_response.py` & `lusid_sdk-2.1.81/lusid/models/valuation_point_data_response.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuation_request.py` & `lusid_sdk-2.1.81/lusid/models/valuation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuation_schedule.py` & `lusid_sdk-2.1.81/lusid/models/valuation_schedule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/valuations_reconciliation_request.py` & `lusid_sdk-2.1.81/lusid/models/valuations_reconciliation_request.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/value_type.py` & `lusid_sdk-2.1.81/lusid/models/value_type.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/vendor_dependency.py` & `lusid_sdk-2.1.81/lusid/models/vendor_dependency.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/vendor_library.py` & `lusid_sdk-2.1.81/lusid/models/vendor_library.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/vendor_model_rule.py` & `lusid_sdk-2.1.81/lusid/models/vendor_model_rule.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/version.py` & `lusid_sdk-2.1.81/lusid/models/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,22 +55,14 @@
         """Create an instance of Version from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
-                            "as_at_created",
-                            "user_id_created",
-                            "request_id_created",
-                            "as_at_modified",
-                            "user_id_modified",
-                            "request_id_modified",
-                            "as_at_version_number",
-                            "entity_unique_id",
                           },
                           exclude_none=True)
         # set to None if as_at_created (nullable) is None
         # and __fields_set__ contains the field
         if self.as_at_created is None and "as_at_created" in self.__fields_set__:
             _dict['asAtCreated'] = None
```

### Comparing `lusid_sdk-2.1.79/lusid/models/version_summary_dto.py` & `lusid_sdk-2.1.81/lusid/models/version_summary_dto.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_a2_b_data_record.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_a2_b_data_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_a2_b_movement_record.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_a2_b_movement_record.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_holding_contributor.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_holding_contributor.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_journal_entry_line.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_journal_entry_line.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_output_transaction.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_output_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_portfolio_holding.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_transaction.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_transaction.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_of_trial_balance.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_of_trial_balance.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py` & `lusid_sdk-2.1.81/lusid/models/versioned_resource_list_with_warnings_of_portfolio_holding.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/virtual_document.py` & `lusid_sdk-2.1.81/lusid/models/virtual_document.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/virtual_document_row.py` & `lusid_sdk-2.1.81/lusid/models/virtual_document_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/virtual_row.py` & `lusid_sdk-2.1.81/lusid/models/virtual_row.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/warning.py` & `lusid_sdk-2.1.81/lusid/models/warning.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/weekend_mask.py` & `lusid_sdk-2.1.81/lusid/models/weekend_mask.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/weighted_instrument.py` & `lusid_sdk-2.1.81/lusid/models/weighted_instrument.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/weighted_instrument_in_line_lookup_identifiers.py` & `lusid_sdk-2.1.81/lusid/models/weighted_instrument_in_line_lookup_identifiers.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/weighted_instruments.py` & `lusid_sdk-2.1.81/lusid/models/weighted_instruments.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/models/yield_curve_data.py` & `lusid_sdk-2.1.81/lusid/models/yield_curve_data.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/lusid/rest.py` & `lusid_sdk-2.1.81/lusid/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_sdk-2.1.79/pyproject.toml` & `lusid_sdk-2.1.81/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-sdk"
-version = "2.1.79"
+version = "2.1.81"
 description = "LUSID API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/lusid-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "LUSID API", "lusid-sdk"]
 packages = [
```

### Comparing `lusid_sdk-2.1.79/PKG-INFO` & `lusid_sdk-2.1.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-sdk
-Version: 2.1.79
+Version: 2.1.81
 Summary: LUSID API
 Home-page: https://github.com/finbourne/lusid-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,LUSID API,lusid-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.11.6513
-- Package version: 2.1.79
+- API version: 0.11.6515
+- Package version: 2.1.81
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

