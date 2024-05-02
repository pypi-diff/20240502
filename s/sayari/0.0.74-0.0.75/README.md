# Comparing `tmp/sayari-0.0.74.tar.gz` & `tmp/sayari-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayari-0.0.74.tar", max compression
+gzip compressed data, was "sayari-0.0.75.tar", max compression
```

## Comparing `sayari-0.0.74.tar` & `sayari-0.0.75.tar`

### file list

```diff
@@ -1,304 +1,304 @@
--rw-r--r--   0        0        0     1401 2024-05-02 15:56:27.171642 sayari-0.0.74/README.md
--rw-r--r--   0        0        0      590 2024-05-02 15:56:27.171642 sayari-0.0.74/pyproject.toml
--rw-r--r--   0        0        0    11506 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/__init__.py
--rw-r--r--   0        0        0      293 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/__init__.py
--rw-r--r--   0        0        0    27153 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/client.py
--rw-r--r--   0        0        0      430 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/__init__.py
--rw-r--r--   0        0        0     1905 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/add_attribute.py
--rw-r--r--   0        0        0      897 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/attribute_properties.py
--rw-r--r--   0        0        0     1648 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/attribute_response.py
--rw-r--r--   0        0        0      971 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/attribute_response_data.py
--rw-r--r--   0        0        0     1692 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/attributes/types/update_attribute.py
--rw-r--r--   0        0        0      125 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/auth/__init__.py
--rw-r--r--   0        0        0     8440 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/auth/client.py
--rw-r--r--   0        0        0      133 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/auth/types/__init__.py
--rw-r--r--   0        0        0     1191 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/auth/types/auth_response.py
--rw-r--r--   0        0        0     9571 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_client.py
--rw-r--r--   0        0        0      203 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_types/__init__.py
--rw-r--r--   0        0        0      272 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_types/types/__init__.py
--rw-r--r--   0        0        0      151 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_types/types/count_qualifier.py
--rw-r--r--   0        0        0     1210 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_types/types/paginated_response.py
--rw-r--r--   0        0        0      928 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/base_types/types/qualified_count.py
--rw-r--r--   0        0        0     9751 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/client.py
--rw-r--r--   0        0        0      853 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/api_error.py
--rw-r--r--   0        0        0     2275 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/jsonable_encoder.py
--rw-r--r--   0        0        0     1374 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/oauth_token_provider.py
--rw-r--r--   0        0        0      329 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/core/request_options.py
--rw-r--r--   0        0        0      183 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/entity/__init__.py
--rw-r--r--   0        0        0    34320 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/entity/client.py
--rw-r--r--   0        0        0      233 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/entity/types/__init__.py
--rw-r--r--   0        0        0     1084 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/entity/types/entity_summary_response.py
--rw-r--r--   0        0        0     1072 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/entity/types/get_entity_response.py
--rw-r--r--   0        0        0      201 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/environment.py
--rw-r--r--   0        0        0     4187 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/__init__.py
--rw-r--r--   0        0        0     6509 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/additional_information_data.py
--rw-r--r--   0        0        0     1478 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/additional_information_info.py
--rw-r--r--   0        0        0     1409 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/additional_information_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/address_data.py
--rw-r--r--   0        0        0     1567 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/address_info.py
--rw-r--r--   0        0        0     5771 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/address_properties.py
--rw-r--r--   0        0        0      214 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/address_type.py
--rw-r--r--   0        0        0      932 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/attribute_data.py
--rw-r--r--   0        0        0     3055 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/attribute_details.py
--rw-r--r--   0        0        0      650 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/attributes.py
--rw-r--r--   0        0        0      249 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/both_identifier_types.py
--rw-r--r--   0        0        0     1065 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/business_purpose_data.py
--rw-r--r--   0        0        0     1302 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/business_purpose_info.py
--rw-r--r--   0        0        0     1560 2024-05-02 15:56:27.171642 sayari-0.0.74/src/sayari/generated_types/types/business_purpose_properties.py
--rw-r--r--   0        0        0      649 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/business_purpose_standard.py
--rw-r--r--   0        0        0      488 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/company_status.py
--rw-r--r--   0        0        0     1049 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/company_type_data.py
--rw-r--r--   0        0        0     1293 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/company_type_info.py
--rw-r--r--   0        0        0     1182 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/company_type_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/contact_data.py
--rw-r--r--   0        0        0     1192 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/contact_info.py
--rw-r--r--   0        0        0     1429 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/contact_properties.py
--rw-r--r--   0        0        0      174 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/contact_type.py
--rw-r--r--   0        0        0     3929 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/country.py
--rw-r--r--   0        0        0      443 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/country_context.py
--rw-r--r--   0        0        0     1032 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/country_data.py
--rw-r--r--   0        0        0     1244 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/country_info.py
--rw-r--r--   0        0        0     1580 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/country_properties.py
--rw-r--r--   0        0        0     2940 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/currency.py
--rw-r--r--   0        0        0     1050 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_data.py
--rw-r--r--   0        0        0     1199 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_info.py
--rw-r--r--   0        0        0     1257 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_properties.py
--rw-r--r--   0        0        0      401 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/entities.py
--rw-r--r--   0        0        0      322 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/finance_type.py
--rw-r--r--   0        0        0     1036 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/finances_data.py
--rw-r--r--   0        0        0     1206 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/finances_info.py
--rw-r--r--   0        0        0     1649 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/finances_properties.py
--rw-r--r--   0        0        0     1044 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/financials_data.py
--rw-r--r--   0        0        0     1226 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/financials_info.py
--rw-r--r--   0        0        0     2406 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/financials_properties.py
--rw-r--r--   0        0        0      157 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/gender.py
--rw-r--r--   0        0        0     1028 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/gender_data.py
--rw-r--r--   0        0        0     1172 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/gender_info.py
--rw-r--r--   0        0        0     1274 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/gender_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/generic_data.py
--rw-r--r--   0        0        0     1265 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/generic_info.py
--rw-r--r--   0        0        0     1418 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/generic_properties.py
--rw-r--r--   0        0        0     1044 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/identifier_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/identifier_info.py
--rw-r--r--   0        0        0     1324 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/identifier_properties.py
--rw-r--r--   0        0        0    16828 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/identifier_type.py
--rw-r--r--   0        0        0     2726 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/language.py
--rw-r--r--   0        0        0     1048 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/measurement_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/measurement_info.py
--rw-r--r--   0        0        0     1479 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/measurement_properties.py
--rw-r--r--   0        0        0      181 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/measurement_type.py
--rw-r--r--   0        0        0      191 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/monetary_value_context.py
--rw-r--r--   0        0        0     1057 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/monetary_value_data.py
--rw-r--r--   0        0        0     1232 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/monetary_value_info.py
--rw-r--r--   0        0        0     1542 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/monetary_value_properties.py
--rw-r--r--   0        0        0      222 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/name_context.py
--rw-r--r--   0        0        0     1020 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/name_data.py
--rw-r--r--   0        0        0     1297 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/name_info.py
--rw-r--r--   0        0        0     1677 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/name_properties.py
--rw-r--r--   0        0        0      163 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/person_status.py
--rw-r--r--   0        0        0     1053 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/person_status_data.py
--rw-r--r--   0        0        0     1238 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/person_status_info.py
--rw-r--r--   0        0        0     1260 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/person_status_properties.py
--rw-r--r--   0        0        0     1036 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/position_data.py
--rw-r--r--   0        0        0     1393 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/position_info.py
--rw-r--r--   0        0        0     1218 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/position_properties.py
--rw-r--r--   0        0        0     1995 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/relationships.py
--rw-r--r--   0        0        0     4122 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/risk.py
--rw-r--r--   0        0        0     1069 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_data.py
--rw-r--r--   0        0        0     1239 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_info.py
--rw-r--r--   0        0        0     1992 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_properties.py
--rw-r--r--   0        0        0     1028 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/shares_data.py
--rw-r--r--   0        0        0     1274 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/shares_info.py
--rw-r--r--   0        0        0     1862 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/shares_properties.py
--rw-r--r--   0        0        0      343 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/status_context.py
--rw-r--r--   0        0        0     1028 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/status_data.py
--rw-r--r--   0        0        0     1339 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/status_info.py
--rw-r--r--   0        0        0     1629 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/status_properties.py
--rw-r--r--   0        0        0      848 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/tag.py
--rw-r--r--   0        0        0     1061 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/translated_name_data.py
--rw-r--r--   0        0        0     1230 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/translated_name_info.py
--rw-r--r--   0        0        0     1509 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/translated_name_properties.py
--rw-r--r--   0        0        0      208 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/translation_context.py
--rw-r--r--   0        0        0      157 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/unit.py
--rw-r--r--   0        0        0     1061 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_data.py
--rw-r--r--   0        0        0     1326 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_info.py
--rw-r--r--   0        0        0     1439 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_properties.py
--rw-r--r--   0        0        0     3356 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_type.py
--rw-r--r--   0        0        0      239 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/__init__.py
--rw-r--r--   0        0        0    18664 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/client.py
--rw-r--r--   0        0        0      348 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/__init__.py
--rw-r--r--   0        0        0      121 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/event_info.py
--rw-r--r--   0        0        0      959 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/history_info.py
--rw-r--r--   0        0        0      949 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/history_response.py
--rw-r--r--   0        0        0     1189 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/usage_info.py
--rw-r--r--   0        0        0     1272 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/info/types/usage_response.py
--rw-r--r--   0        0        0      531 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/__init__.py
--rw-r--r--   0        0        0    19516 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/client.py
--rw-r--r--   0        0        0      747 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/__init__.py
--rw-r--r--   0        0        0     1584 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/notification.py
--rw-r--r--   0        0        0     1086 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/notification_additional_information.py
--rw-r--r--   0        0        0      148 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/notification_type.py
--rw-r--r--   0        0        0     1296 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/project_notification_data.py
--rw-r--r--   0        0        0     3380 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/project_notifications_response.py
--rw-r--r--   0        0        0     1835 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/resource_notification_data.py
--rw-r--r--   0        0        0     1627 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/notifications/types/resource_notifications_response.py
--rw-r--r--   0        0        0     1179 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/__init__.py
--rw-r--r--   0        0        0    32266 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/client.py
--rw-r--r--   0        0        0     1785 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/__init__.py
--rw-r--r--   0        0        0     1107 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/bucket_agg.py
--rw-r--r--   0        0        0      985 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/create_project_request.py
--rw-r--r--   0        0        0     1390 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/create_project_response.py
--rw-r--r--   0        0        0      852 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/doc_count.py
--rw-r--r--   0        0        0      220 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/get_project_entities_accept_header.py
--rw-r--r--   0        0        0    14401 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/get_project_entities_response.py
--rw-r--r--   0        0        0     3197 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/get_projects_response.py
--rw-r--r--   0        0        0      933 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/hs_code_agg.py
--rw-r--r--   0        0        0      965 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/hs_code_agg_bucket.py
--rw-r--r--   0        0        0      995 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/hs_code_agg_terms.py
--rw-r--r--   0        0        0      851 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/int_key_value.py
--rw-r--r--   0        0        0     1236 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project.py
--rw-r--r--   0        0        0     1084 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_counts.py
--rw-r--r--   0        0        0     1980 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_entities_aggs.py
--rw-r--r--   0        0        0      101 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_entities_aggs_definition.py
--rw-r--r--   0        0        0       93 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_entities_filter.py
--rw-r--r--   0        0        0     1755 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_entity.py
--rw-r--r--   0        0        0     1010 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_entity_upstream.py
--rw-r--r--   0        0        0     1009 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/project_with_members.py
--rw-r--r--   0        0        0     1014 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/psa_summary.py
--rw-r--r--   0        0        0      157 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/role.py
--rw-r--r--   0        0        0      989 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/role_member.py
--rw-r--r--   0        0        0      155 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/role_member_type.py
--rw-r--r--   0        0        0      517 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/project/types/sort_field.py
--rw-r--r--   0        0        0        0 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/py.typed
--rw-r--r--   0        0        0      173 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/record/__init__.py
--rw-r--r--   0        0        0     9509 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/record/client.py
--rw-r--r--   0        0        0      217 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/record/types/__init__.py
--rw-r--r--   0        0        0    10699 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/record/types/get_record_response.py
--rw-r--r--   0        0        0     1036 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/record/types/record_references.py
--rw-r--r--   0        0        0      267 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/__init__.py
--rw-r--r--   0        0        0    13242 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/client.py
--rw-r--r--   0        0        0      380 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/types/__init__.py
--rw-r--r--   0        0        0     1234 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/types/match_explanation.py
--rw-r--r--   0        0        0     4632 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/types/resolution_response.py
--rw-r--r--   0        0        0     1725 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/types/resolution_response_fields.py
--rw-r--r--   0        0        0     1501 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resolution/types/resolution_result.py
--rw-r--r--   0        0        0      257 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/__init__.py
--rw-r--r--   0        0        0     9347 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/client.py
--rw-r--r--   0        0        0      368 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/types/__init__.py
--rw-r--r--   0        0        0      146 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/types/resource_type.py
--rw-r--r--   0        0        0     1254 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/types/save_entity_request.py
--rw-r--r--   0        0        0     1528 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/types/save_entity_response.py
--rw-r--r--   0        0        0     1095 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/resource/types/save_entity_response_data.py
--rw-r--r--   0        0        0      295 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/__init__.py
--rw-r--r--   0        0        0    45037 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/client.py
--rw-r--r--   0        0        0      444 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/__init__.py
--rw-r--r--   0        0        0      883 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/coordinates.py
--rw-r--r--   0        0        0     6193 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/entity_search_response.py
--rw-r--r--   0        0        0     1478 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/filter_list.py
--rw-r--r--   0        0        0     3434 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/record_search_response.py
--rw-r--r--   0        0        0     1140 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/search_results.py
--rw-r--r--   0        0        0       80 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/search/types/source_id.py
--rw-r--r--   0        0        0      987 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/__init__.py
--rw-r--r--   0        0        0      658 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/__init__.py
--rw-r--r--   0        0        0      297 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/bad_gateway.py
--rw-r--r--   0        0        0      297 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/bad_request.py
--rw-r--r--   0        0        0      317 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/connection_error.py
--rw-r--r--   0        0        0      334 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/internal_server_error.py
--rw-r--r--   0        0        0      322 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/method_not_allowed.py
--rw-r--r--   0        0        0      309 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/not_acceptable.py
--rw-r--r--   0        0        0      289 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/not_found.py
--rw-r--r--   0        0        0      301 2024-05-02 15:56:27.175642 sayari-0.0.74/src/sayari/shared_errors/errors/rate_limit_exceeded.py
--rw-r--r--   0        0        0      304 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/errors/unauthorized.py
--rw-r--r--   0        0        0      858 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/__init__.py
--rw-r--r--   0        0        0      112 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/bad_gateway_response.py
--rw-r--r--   0        0        0      112 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/bad_request_response.py
--rw-r--r--   0        0        0      117 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/connection_error_response.py
--rw-r--r--   0        0        0      121 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/internal_server_error_response.py
--rw-r--r--   0        0        0      972 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/method_not_allowed_response.py
--rw-r--r--   0        0        0     1028 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/not_acceptable_response.py
--rw-r--r--   0        0        0      972 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/not_found_response.py
--rw-r--r--   0        0        0      111 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/rate_limit_response.py
--rw-r--r--   0        0        0      114 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_errors/types/unauthorized_response.py
--rw-r--r--   0        0        0     1519 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/client_name.py
--rw-r--r--   0        0        0       83 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/company_type.py
--rw-r--r--   0        0        0      882 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/coordinate.py
--rw-r--r--   0        0        0     4362 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/core_entity.py
--rw-r--r--   0        0        0     3746 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/embedded_entity.py
--rw-r--r--   0        0        0     2776 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_details.py
--rw-r--r--   0        0        0       84 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_hs_code.py
--rw-r--r--   0        0        0      131 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_matches.py
--rw-r--r--   0        0        0       94 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_registration_date.py
--rw-r--r--   0        0        0     1279 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_relationships.py
--rw-r--r--   0        0        0      201 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_risk.py
--rw-r--r--   0        0        0      962 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_summary.py
--rw-r--r--   0        0        0       93 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/entity_translated_label.py
--rw-r--r--   0        0        0     1245 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/identifier.py
--rw-r--r--   0        0        0     1249 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as.py
--rw-r--r--   0        0        0     1062 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as_data.py
--rw-r--r--   0        0        0      876 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as_match.py
--rw-r--r--   0        0        0      981 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/psa.py
--rw-r--r--   0        0        0     1386 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/psa_entity.py
--rw-r--r--   0        0        0      888 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/psa_match_keys.py
--rw-r--r--   0        0        0     1785 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/record_details.py
--rw-r--r--   0        0        0     1218 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/referenced_by.py
--rw-r--r--   0        0        0      998 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/referenced_by_data.py
--rw-r--r--   0        0        0      165 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/referenced_by_data_type.py
--rw-r--r--   0        0        0      198 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/relationship_count.py
--rw-r--r--   0        0        0     1569 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/relationship_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/relationship_info.py
--rw-r--r--   0        0        0     1054 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/risk_data.py
--rw-r--r--   0        0        0      177 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/risk_level.py
--rw-r--r--   0        0        0      123 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/risk_value.py
--rw-r--r--   0        0        0      222 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/search_field.py
--rw-r--r--   0        0        0       87 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/shipment_arrival.py
--rw-r--r--   0        0        0       89 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/shipment_departure.py
--rw-r--r--   0        0        0      948 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/source_count_info.py
--rw-r--r--   0        0        0      977 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/shared_types/types/status.py
--rw-r--r--   0        0        0      197 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/__init__.py
--rw-r--r--   0        0        0    15172 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/client.py
--rw-r--r--   0        0        0      264 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/types/__init__.py
--rw-r--r--   0        0        0     1029 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/types/get_source_response.py
--rw-r--r--   0        0        0     2882 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/types/list_sources_response.py
--rw-r--r--   0        0        0     1318 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/source/types/source.py
--rw-r--r--   0        0        0      887 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/__init__.py
--rw-r--r--   0        0        0    31333 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/client.py
--rw-r--r--   0        0        0     1316 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/__init__.py
--rw-r--r--   0        0        0      917 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/business_purpose.py
--rw-r--r--   0        0        0     7236 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/buyer_search_response.py
--rw-r--r--   0        0        0      956 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/data_source.py
--rw-r--r--   0        0        0      924 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/hs_code.py
--rw-r--r--   0        0        0      870 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/hs_code_info.py
--rw-r--r--   0        0        0      998 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/monetary_value.py
--rw-r--r--   0        0        0     1842 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment.py
--rw-r--r--   0        0        0     1071 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment_address.py
--rw-r--r--   0        0        0      912 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment_country.py
--rw-r--r--   0        0        0      967 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment_identifier.py
--rw-r--r--   0        0        0     1318 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment_metadata.py
--rw-r--r--   0        0        0     3778 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/shipment_search_response.py
--rw-r--r--   0        0        0     1565 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/source_or_destination_entity.py
--rw-r--r--   0        0        0     1146 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/supplier_metadata.py
--rw-r--r--   0        0        0     1052 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/supplier_or_buyer.py
--rw-r--r--   0        0        0     4760 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/supplier_search_response.py
--rw-r--r--   0        0        0     5181 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/trade_filter_list.py
--rw-r--r--   0        0        0      876 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/trade/types/weight.py
--rw-r--r--   0        0        0      395 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/__init__.py
--rw-r--r--   0        0        0   104903 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/client.py
--rw-r--r--   0        0        0      539 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/__init__.py
--rw-r--r--   0        0        0     1025 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/shortest_path_data.py
--rw-r--r--   0        0        0    20912 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/shortest_path_response.py
--rw-r--r--   0        0        0     1022 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/traversal_data.py
--rw-r--r--   0        0        0     1147 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/traversal_path.py
--rw-r--r--   0        0        0     1135 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/traversal_relationship_data.py
--rw-r--r--   0        0        0     7818 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/traversal/types/traversal_response.py
--rw-r--r--   0        0        0       74 2024-05-02 15:56:27.179642 sayari-0.0.74/src/sayari/version.py
--rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 sayari-0.0.74/PKG-INFO
+-rw-r--r--   0        0        0     1401 2024-05-02 16:24:17.902155 sayari-0.0.75/README.md
+-rw-r--r--   0        0        0      613 2024-05-02 16:24:17.902155 sayari-0.0.75/pyproject.toml
+-rw-r--r--   0        0        0    11506 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/__init__.py
+-rw-r--r--   0        0        0    27153 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/client.py
+-rw-r--r--   0        0        0      430 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/__init__.py
+-rw-r--r--   0        0        0     1905 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/add_attribute.py
+-rw-r--r--   0        0        0      897 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_properties.py
+-rw-r--r--   0        0        0     1648 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_response.py
+-rw-r--r--   0        0        0      971 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_response_data.py
+-rw-r--r--   0        0        0     1692 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/update_attribute.py
+-rw-r--r--   0        0        0      125 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/__init__.py
+-rw-r--r--   0        0        0     8440 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/client.py
+-rw-r--r--   0        0        0      133 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/types/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/types/auth_response.py
+-rw-r--r--   0        0        0     9571 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_client.py
+-rw-r--r--   0        0        0      203 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/__init__.py
+-rw-r--r--   0        0        0      272 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/count_qualifier.py
+-rw-r--r--   0        0        0     1210 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/paginated_response.py
+-rw-r--r--   0        0        0      928 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/qualified_count.py
+-rw-r--r--   0        0        0     9751 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/client.py
+-rw-r--r--   0        0        0      853 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/api_error.py
+-rw-r--r--   0        0        0     2275 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/jsonable_encoder.py
+-rw-r--r--   0        0        0     1374 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/oauth_token_provider.py
+-rw-r--r--   0        0        0      329 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/request_options.py
+-rw-r--r--   0        0        0      183 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/__init__.py
+-rw-r--r--   0        0        0    34320 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/client.py
+-rw-r--r--   0        0        0      233 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/entity_summary_response.py
+-rw-r--r--   0        0        0     1072 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/get_entity_response.py
+-rw-r--r--   0        0        0      201 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/environment.py
+-rw-r--r--   0        0        0     4187 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/__init__.py
+-rw-r--r--   0        0        0     6509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/__init__.py
+-rw-r--r--   0        0        0     1089 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_data.py
+-rw-r--r--   0        0        0     1478 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_info.py
+-rw-r--r--   0        0        0     1409 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_data.py
+-rw-r--r--   0        0        0     1567 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_info.py
+-rw-r--r--   0        0        0     5771 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_properties.py
+-rw-r--r--   0        0        0      214 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_type.py
+-rw-r--r--   0        0        0      932 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attribute_data.py
+-rw-r--r--   0        0        0     3055 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attribute_details.py
+-rw-r--r--   0        0        0      650 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attributes.py
+-rw-r--r--   0        0        0      249 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/both_identifier_types.py
+-rw-r--r--   0        0        0     1065 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_data.py
+-rw-r--r--   0        0        0     1302 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_info.py
+-rw-r--r--   0        0        0     1560 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_properties.py
+-rw-r--r--   0        0        0      649 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_standard.py
+-rw-r--r--   0        0        0      488 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_status.py
+-rw-r--r--   0        0        0     1049 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_data.py
+-rw-r--r--   0        0        0     1293 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_info.py
+-rw-r--r--   0        0        0     1182 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_data.py
+-rw-r--r--   0        0        0     1192 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_info.py
+-rw-r--r--   0        0        0     1429 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_properties.py
+-rw-r--r--   0        0        0      174 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_type.py
+-rw-r--r--   0        0        0     3929 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country.py
+-rw-r--r--   0        0        0      443 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_context.py
+-rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_data.py
+-rw-r--r--   0        0        0     1244 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_info.py
+-rw-r--r--   0        0        0     1580 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_properties.py
+-rw-r--r--   0        0        0     2940 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/currency.py
+-rw-r--r--   0        0        0     1050 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_data.py
+-rw-r--r--   0        0        0     1199 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_info.py
+-rw-r--r--   0        0        0     1257 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_properties.py
+-rw-r--r--   0        0        0      401 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/entities.py
+-rw-r--r--   0        0        0      322 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finance_type.py
+-rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_data.py
+-rw-r--r--   0        0        0     1206 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_info.py
+-rw-r--r--   0        0        0     1649 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_properties.py
+-rw-r--r--   0        0        0     1044 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_data.py
+-rw-r--r--   0        0        0     1226 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_info.py
+-rw-r--r--   0        0        0     2406 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_properties.py
+-rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender.py
+-rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_data.py
+-rw-r--r--   0        0        0     1172 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_info.py
+-rw-r--r--   0        0        0     1274 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_data.py
+-rw-r--r--   0        0        0     1265 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_info.py
+-rw-r--r--   0        0        0     1418 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_properties.py
+-rw-r--r--   0        0        0     1044 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_info.py
+-rw-r--r--   0        0        0     1324 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_properties.py
+-rw-r--r--   0        0        0    16828 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_type.py
+-rw-r--r--   0        0        0     2726 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/language.py
+-rw-r--r--   0        0        0     1048 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_info.py
+-rw-r--r--   0        0        0     1479 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_properties.py
+-rw-r--r--   0        0        0      181 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_type.py
+-rw-r--r--   0        0        0      191 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_context.py
+-rw-r--r--   0        0        0     1057 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_data.py
+-rw-r--r--   0        0        0     1232 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_info.py
+-rw-r--r--   0        0        0     1542 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_properties.py
+-rw-r--r--   0        0        0      222 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_context.py
+-rw-r--r--   0        0        0     1020 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_data.py
+-rw-r--r--   0        0        0     1297 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_info.py
+-rw-r--r--   0        0        0     1677 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_properties.py
+-rw-r--r--   0        0        0      163 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status.py
+-rw-r--r--   0        0        0     1053 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_data.py
+-rw-r--r--   0        0        0     1238 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_info.py
+-rw-r--r--   0        0        0     1260 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_properties.py
+-rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_data.py
+-rw-r--r--   0        0        0     1393 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_info.py
+-rw-r--r--   0        0        0     1218 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_properties.py
+-rw-r--r--   0        0        0     1995 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/relationships.py
+-rw-r--r--   0        0        0     4122 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk.py
+-rw-r--r--   0        0        0     1069 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_data.py
+-rw-r--r--   0        0        0     1239 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_info.py
+-rw-r--r--   0        0        0     1992 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_properties.py
+-rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_data.py
+-rw-r--r--   0        0        0     1274 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_info.py
+-rw-r--r--   0        0        0     1862 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_properties.py
+-rw-r--r--   0        0        0      343 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_context.py
+-rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_data.py
+-rw-r--r--   0        0        0     1339 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_info.py
+-rw-r--r--   0        0        0     1629 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_properties.py
+-rw-r--r--   0        0        0      848 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/tag.py
+-rw-r--r--   0        0        0     1061 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_data.py
+-rw-r--r--   0        0        0     1230 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_info.py
+-rw-r--r--   0        0        0     1509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_properties.py
+-rw-r--r--   0        0        0      208 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translation_context.py
+-rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/unit.py
+-rw-r--r--   0        0        0     1061 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_data.py
+-rw-r--r--   0        0        0     1326 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_info.py
+-rw-r--r--   0        0        0     1439 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_properties.py
+-rw-r--r--   0        0        0     3356 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_type.py
+-rw-r--r--   0        0        0      239 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/__init__.py
+-rw-r--r--   0        0        0    18664 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/client.py
+-rw-r--r--   0        0        0      348 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/event_info.py
+-rw-r--r--   0        0        0      959 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/history_info.py
+-rw-r--r--   0        0        0      949 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/history_response.py
+-rw-r--r--   0        0        0     1189 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/usage_info.py
+-rw-r--r--   0        0        0     1272 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/usage_response.py
+-rw-r--r--   0        0        0      531 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/__init__.py
+-rw-r--r--   0        0        0    19516 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/client.py
+-rw-r--r--   0        0        0      747 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification.py
+-rw-r--r--   0        0        0     1086 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification_additional_information.py
+-rw-r--r--   0        0        0      148 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification_type.py
+-rw-r--r--   0        0        0     1296 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/project_notification_data.py
+-rw-r--r--   0        0        0     3380 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/project_notifications_response.py
+-rw-r--r--   0        0        0     1835 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/resource_notification_data.py
+-rw-r--r--   0        0        0     1627 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/resource_notifications_response.py
+-rw-r--r--   0        0        0     1179 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/__init__.py
+-rw-r--r--   0        0        0    32266 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/client.py
+-rw-r--r--   0        0        0     1785 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/__init__.py
+-rw-r--r--   0        0        0     1107 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/bucket_agg.py
+-rw-r--r--   0        0        0      985 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/create_project_request.py
+-rw-r--r--   0        0        0     1390 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/create_project_response.py
+-rw-r--r--   0        0        0      852 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/doc_count.py
+-rw-r--r--   0        0        0      220 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_project_entities_accept_header.py
+-rw-r--r--   0        0        0    14401 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_project_entities_response.py
+-rw-r--r--   0        0        0     3197 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_projects_response.py
+-rw-r--r--   0        0        0      933 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg.py
+-rw-r--r--   0        0        0      965 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg_bucket.py
+-rw-r--r--   0        0        0      995 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg_terms.py
+-rw-r--r--   0        0        0      851 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/int_key_value.py
+-rw-r--r--   0        0        0     1236 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project.py
+-rw-r--r--   0        0        0     1084 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_counts.py
+-rw-r--r--   0        0        0     1980 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_aggs.py
+-rw-r--r--   0        0        0      101 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_aggs_definition.py
+-rw-r--r--   0        0        0       93 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_filter.py
+-rw-r--r--   0        0        0     1755 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entity.py
+-rw-r--r--   0        0        0     1010 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entity_upstream.py
+-rw-r--r--   0        0        0     1009 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_with_members.py
+-rw-r--r--   0        0        0     1014 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/psa_summary.py
+-rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role.py
+-rw-r--r--   0        0        0      989 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role_member.py
+-rw-r--r--   0        0        0      155 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role_member_type.py
+-rw-r--r--   0        0        0      517 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/sort_field.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/py.typed
+-rw-r--r--   0        0        0      173 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/__init__.py
+-rw-r--r--   0        0        0     9509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/client.py
+-rw-r--r--   0        0        0      217 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/__init__.py
+-rw-r--r--   0        0        0    10699 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/get_record_response.py
+-rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/record_references.py
+-rw-r--r--   0        0        0      267 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/__init__.py
+-rw-r--r--   0        0        0    13242 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/client.py
+-rw-r--r--   0        0        0      380 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/__init__.py
+-rw-r--r--   0        0        0     1234 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/match_explanation.py
+-rw-r--r--   0        0        0     4632 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_response.py
+-rw-r--r--   0        0        0     1725 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_response_fields.py
+-rw-r--r--   0        0        0     1501 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_result.py
+-rw-r--r--   0        0        0      257 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/__init__.py
+-rw-r--r--   0        0        0     9347 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/client.py
+-rw-r--r--   0        0        0      368 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/resource_type.py
+-rw-r--r--   0        0        0     1254 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_request.py
+-rw-r--r--   0        0        0     1528 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_response.py
+-rw-r--r--   0        0        0     1095 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_response_data.py
+-rw-r--r--   0        0        0      295 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/__init__.py
+-rw-r--r--   0        0        0    45037 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/client.py
+-rw-r--r--   0        0        0      444 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/coordinates.py
+-rw-r--r--   0        0        0     6193 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/entity_search_response.py
+-rw-r--r--   0        0        0     1478 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/filter_list.py
+-rw-r--r--   0        0        0     3434 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/record_search_response.py
+-rw-r--r--   0        0        0     1140 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/search_results.py
+-rw-r--r--   0        0        0       80 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/source_id.py
+-rw-r--r--   0        0        0      987 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/bad_gateway.py
+-rw-r--r--   0        0        0      297 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/bad_request.py
+-rw-r--r--   0        0        0      317 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/connection_error.py
+-rw-r--r--   0        0        0      334 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/internal_server_error.py
+-rw-r--r--   0        0        0      322 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/method_not_allowed.py
+-rw-r--r--   0        0        0      309 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/not_acceptable.py
+-rw-r--r--   0        0        0      289 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/not_found.py
+-rw-r--r--   0        0        0      301 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/rate_limit_exceeded.py
+-rw-r--r--   0        0        0      304 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/unauthorized.py
+-rw-r--r--   0        0        0      858 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/bad_gateway_response.py
+-rw-r--r--   0        0        0      112 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/bad_request_response.py
+-rw-r--r--   0        0        0      117 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/connection_error_response.py
+-rw-r--r--   0        0        0      121 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/internal_server_error_response.py
+-rw-r--r--   0        0        0      972 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/method_not_allowed_response.py
+-rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/not_acceptable_response.py
+-rw-r--r--   0        0        0      972 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/not_found_response.py
+-rw-r--r--   0        0        0      111 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/rate_limit_response.py
+-rw-r--r--   0        0        0      114 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/unauthorized_response.py
+-rw-r--r--   0        0        0     1519 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/client_name.py
+-rw-r--r--   0        0        0       83 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/company_type.py
+-rw-r--r--   0        0        0      882 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/coordinate.py
+-rw-r--r--   0        0        0     4362 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/core_entity.py
+-rw-r--r--   0        0        0     3746 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/embedded_entity.py
+-rw-r--r--   0        0        0     2776 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_details.py
+-rw-r--r--   0        0        0       84 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_hs_code.py
+-rw-r--r--   0        0        0      131 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_matches.py
+-rw-r--r--   0        0        0       94 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_registration_date.py
+-rw-r--r--   0        0        0     1279 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_relationships.py
+-rw-r--r--   0        0        0      201 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_risk.py
+-rw-r--r--   0        0        0      962 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_summary.py
+-rw-r--r--   0        0        0       93 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_translated_label.py
+-rw-r--r--   0        0        0     1245 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/identifier.py
+-rw-r--r--   0        0        0     1249 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as.py
+-rw-r--r--   0        0        0     1062 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_data.py
+-rw-r--r--   0        0        0      876 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_match.py
+-rw-r--r--   0        0        0      981 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa.py
+-rw-r--r--   0        0        0     1386 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa_entity.py
+-rw-r--r--   0        0        0      888 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa_match_keys.py
+-rw-r--r--   0        0        0     1785 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/record_details.py
+-rw-r--r--   0        0        0     1218 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by.py
+-rw-r--r--   0        0        0      998 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data.py
+-rw-r--r--   0        0        0      165 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data_type.py
+-rw-r--r--   0        0        0      198 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_count.py
+-rw-r--r--   0        0        0     1569 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_info.py
+-rw-r--r--   0        0        0     1054 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_data.py
+-rw-r--r--   0        0        0      177 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_level.py
+-rw-r--r--   0        0        0      123 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_value.py
+-rw-r--r--   0        0        0      222 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/search_field.py
+-rw-r--r--   0        0        0       87 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/shipment_arrival.py
+-rw-r--r--   0        0        0       89 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/shipment_departure.py
+-rw-r--r--   0        0        0      948 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/source_count_info.py
+-rw-r--r--   0        0        0      977 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/status.py
+-rw-r--r--   0        0        0      197 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/__init__.py
+-rw-r--r--   0        0        0    15172 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/client.py
+-rw-r--r--   0        0        0      264 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/get_source_response.py
+-rw-r--r--   0        0        0     2882 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/list_sources_response.py
+-rw-r--r--   0        0        0     1318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/source.py
+-rw-r--r--   0        0        0      887 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/__init__.py
+-rw-r--r--   0        0        0    31333 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/client.py
+-rw-r--r--   0        0        0     1316 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/business_purpose.py
+-rw-r--r--   0        0        0     7236 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/buyer_search_response.py
+-rw-r--r--   0        0        0      956 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/data_source.py
+-rw-r--r--   0        0        0      924 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/hs_code.py
+-rw-r--r--   0        0        0      870 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/hs_code_info.py
+-rw-r--r--   0        0        0      998 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/monetary_value.py
+-rw-r--r--   0        0        0     1842 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment.py
+-rw-r--r--   0        0        0     1071 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_address.py
+-rw-r--r--   0        0        0      912 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_country.py
+-rw-r--r--   0        0        0      967 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_identifier.py
+-rw-r--r--   0        0        0     1318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_metadata.py
+-rw-r--r--   0        0        0     3778 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_search_response.py
+-rw-r--r--   0        0        0     1565 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/source_or_destination_entity.py
+-rw-r--r--   0        0        0     1146 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_metadata.py
+-rw-r--r--   0        0        0     1052 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_or_buyer.py
+-rw-r--r--   0        0        0     4760 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_search_response.py
+-rw-r--r--   0        0        0     5181 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/trade_filter_list.py
+-rw-r--r--   0        0        0      876 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/weight.py
+-rw-r--r--   0        0        0      395 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/__init__.py
+-rw-r--r--   0        0        0   104903 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/client.py
+-rw-r--r--   0        0        0      539 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/__init__.py
+-rw-r--r--   0        0        0     1025 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/shortest_path_data.py
+-rw-r--r--   0        0        0    20912 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/shortest_path_response.py
+-rw-r--r--   0        0        0     1022 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_data.py
+-rw-r--r--   0        0        0     1147 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_path.py
+-rw-r--r--   0        0        0     1135 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_relationship_data.py
+-rw-r--r--   0        0        0     7818 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_response.py
+-rw-r--r--   0        0        0       74 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/version.py
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 sayari-0.0.75/PKG-INFO
```

### Comparing `sayari-0.0.74/README.md` & `sayari-0.0.75/README.md`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/pyproject.toml` & `sayari-0.0.75/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sayari"
-version = "0.0.74"
-description = ""
+version = "0.0.75"
+description = "A Python SDK for Sayari"
 readme = "README.md"
 authors = []
 packages = [
     { include = "sayari", from = "src"}
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `sayari-0.0.74/src/sayari/__init__.py` & `sayari-0.0.75/src/sayari/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/client.py` & `sayari-0.0.75/src/sayari/attributes/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/types/add_attribute.py` & `sayari-0.0.75/src/sayari/attributes/types/add_attribute.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/types/attribute_properties.py` & `sayari-0.0.75/src/sayari/attributes/types/attribute_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/types/attribute_response.py` & `sayari-0.0.75/src/sayari/attributes/types/attribute_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/types/attribute_response_data.py` & `sayari-0.0.75/src/sayari/attributes/types/attribute_response_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/attributes/types/update_attribute.py` & `sayari-0.0.75/src/sayari/attributes/types/update_attribute.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/auth/client.py` & `sayari-0.0.75/src/sayari/auth/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/auth/types/auth_response.py` & `sayari-0.0.75/src/sayari/auth/types/auth_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/base_client.py` & `sayari-0.0.75/src/sayari/base_client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/base_types/types/paginated_response.py` & `sayari-0.0.75/src/sayari/base_types/types/paginated_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/base_types/types/qualified_count.py` & `sayari-0.0.75/src/sayari/base_types/types/qualified_count.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/client.py` & `sayari-0.0.75/src/sayari/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/__init__.py` & `sayari-0.0.75/src/sayari/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/client_wrapper.py` & `sayari-0.0.75/src/sayari/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "sayari",
-            "X-Fern-SDK-Version": "0.0.74",
+            "X-Fern-SDK-Version": "0.0.75",
         }
         headers["client-name"] = self._client_name
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
```

### Comparing `sayari-0.0.74/src/sayari/core/datetime_utils.py` & `sayari-0.0.75/src/sayari/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/file.py` & `sayari-0.0.75/src/sayari/core/file.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/http_client.py` & `sayari-0.0.75/src/sayari/core/http_client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/jsonable_encoder.py` & `sayari-0.0.75/src/sayari/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/oauth_token_provider.py` & `sayari-0.0.75/src/sayari/core/oauth_token_provider.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/core/request_options.py` & `sayari-0.0.75/src/sayari/core/request_options.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/entity/client.py` & `sayari-0.0.75/src/sayari/entity/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/entity/types/entity_summary_response.py` & `sayari-0.0.75/src/sayari/entity/types/entity_summary_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/entity/types/get_entity_response.py` & `sayari-0.0.75/src/sayari/entity/types/get_entity_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/__init__.py` & `sayari-0.0.75/src/sayari/generated_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/__init__.py` & `sayari-0.0.75/src/sayari/generated_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/additional_information_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/additional_information_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/additional_information_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/additional_information_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/additional_information_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/additional_information_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/address_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/address_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/address_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/address_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/address_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/address_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/attribute_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/attribute_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/attribute_details.py` & `sayari-0.0.75/src/sayari/generated_types/types/attribute_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/attributes.py` & `sayari-0.0.75/src/sayari/generated_types/types/attributes.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/business_purpose_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/business_purpose_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/business_purpose_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/business_purpose_standard.py` & `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_standard.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/company_type_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/company_type_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/company_type_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/company_type_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/company_type_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/company_type_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/contact_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/contact_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/contact_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/contact_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/contact_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/contact_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/country.py` & `sayari-0.0.75/src/sayari/generated_types/types/country.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/country_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/country_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/country_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/country_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/country_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/country_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/currency.py` & `sayari-0.0.75/src/sayari/generated_types/types/currency.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/date_of_birth_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/finances_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/finances_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/finances_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/finances_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/finances_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/finances_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/financials_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/financials_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/financials_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/financials_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/financials_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/financials_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/gender_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/gender_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/gender_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/gender_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/gender_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/gender_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/generic_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/generic_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/generic_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/generic_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/generic_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/generic_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/identifier_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/identifier_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/identifier_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/identifier_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/identifier_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/identifier_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/identifier_type.py` & `sayari-0.0.75/src/sayari/generated_types/types/identifier_type.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/language.py` & `sayari-0.0.75/src/sayari/generated_types/types/language.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/measurement_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/measurement_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/measurement_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/measurement_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/measurement_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/measurement_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/monetary_value_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/monetary_value_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/monetary_value_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/name_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/name_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/name_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/name_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/name_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/name_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/person_status_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/person_status_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/person_status_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/person_status_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/person_status_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/person_status_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/position_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/position_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/position_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/position_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/position_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/position_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/relationships.py` & `sayari-0.0.75/src/sayari/generated_types/types/relationships.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/risk.py` & `sayari-0.0.75/src/sayari/generated_types/types/risk.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/risk_intelligence_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/shares_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/shares_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/shares_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/shares_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/shares_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/shares_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/status_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/status_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/status_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/status_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/status_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/status_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/tag.py` & `sayari-0.0.75/src/sayari/generated_types/types/tag.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/translated_name_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/translated_name_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/translated_name_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/translated_name_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/translated_name_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/translated_name_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_data.py` & `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_info.py` & `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_properties.py` & `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/generated_types/types/weak_identifier_type.py` & `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_type.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/info/client.py` & `sayari-0.0.75/src/sayari/info/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/info/types/history_info.py` & `sayari-0.0.75/src/sayari/info/types/history_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/info/types/history_response.py` & `sayari-0.0.75/src/sayari/info/types/history_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/info/types/usage_info.py` & `sayari-0.0.75/src/sayari/info/types/usage_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/info/types/usage_response.py` & `sayari-0.0.75/src/sayari/info/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/__init__.py` & `sayari-0.0.75/src/sayari/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/client.py` & `sayari-0.0.75/src/sayari/notifications/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/__init__.py` & `sayari-0.0.75/src/sayari/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/notification.py` & `sayari-0.0.75/src/sayari/notifications/types/notification.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/notification_additional_information.py` & `sayari-0.0.75/src/sayari/notifications/types/notification_additional_information.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/project_notification_data.py` & `sayari-0.0.75/src/sayari/notifications/types/project_notification_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/project_notifications_response.py` & `sayari-0.0.75/src/sayari/notifications/types/project_notifications_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/resource_notification_data.py` & `sayari-0.0.75/src/sayari/notifications/types/resource_notification_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/notifications/types/resource_notifications_response.py` & `sayari-0.0.75/src/sayari/notifications/types/resource_notifications_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/__init__.py` & `sayari-0.0.75/src/sayari/project/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/client.py` & `sayari-0.0.75/src/sayari/project/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/__init__.py` & `sayari-0.0.75/src/sayari/project/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/bucket_agg.py` & `sayari-0.0.75/src/sayari/project/types/bucket_agg.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/create_project_request.py` & `sayari-0.0.75/src/sayari/project/types/create_project_request.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/create_project_response.py` & `sayari-0.0.75/src/sayari/project/types/create_project_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/doc_count.py` & `sayari-0.0.75/src/sayari/project/types/doc_count.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/get_project_entities_response.py` & `sayari-0.0.75/src/sayari/project/types/get_project_entities_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/get_projects_response.py` & `sayari-0.0.75/src/sayari/project/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/hs_code_agg.py` & `sayari-0.0.75/src/sayari/project/types/hs_code_agg.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/hs_code_agg_bucket.py` & `sayari-0.0.75/src/sayari/project/types/hs_code_agg_bucket.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/hs_code_agg_terms.py` & `sayari-0.0.75/src/sayari/project/types/hs_code_agg_terms.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/int_key_value.py` & `sayari-0.0.75/src/sayari/project/types/int_key_value.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project.py` & `sayari-0.0.75/src/sayari/project/types/project.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project_counts.py` & `sayari-0.0.75/src/sayari/project/types/project_counts.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project_entities_aggs.py` & `sayari-0.0.75/src/sayari/project/types/project_entities_aggs.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project_entity.py` & `sayari-0.0.75/src/sayari/project/types/project_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project_entity_upstream.py` & `sayari-0.0.75/src/sayari/project/types/project_entity_upstream.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/project_with_members.py` & `sayari-0.0.75/src/sayari/project/types/project_with_members.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/psa_summary.py` & `sayari-0.0.75/src/sayari/project/types/psa_summary.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/role_member.py` & `sayari-0.0.75/src/sayari/project/types/role_member.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/project/types/sort_field.py` & `sayari-0.0.75/src/sayari/project/types/sort_field.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/record/client.py` & `sayari-0.0.75/src/sayari/record/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/record/types/get_record_response.py` & `sayari-0.0.75/src/sayari/record/types/get_record_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/record/types/record_references.py` & `sayari-0.0.75/src/sayari/record/types/record_references.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resolution/client.py` & `sayari-0.0.75/src/sayari/resolution/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resolution/types/match_explanation.py` & `sayari-0.0.75/src/sayari/resolution/types/match_explanation.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resolution/types/resolution_response.py` & `sayari-0.0.75/src/sayari/resolution/types/resolution_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resolution/types/resolution_response_fields.py` & `sayari-0.0.75/src/sayari/resolution/types/resolution_response_fields.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resolution/types/resolution_result.py` & `sayari-0.0.75/src/sayari/resolution/types/resolution_result.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resource/client.py` & `sayari-0.0.75/src/sayari/resource/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resource/types/save_entity_request.py` & `sayari-0.0.75/src/sayari/resource/types/save_entity_request.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resource/types/save_entity_response.py` & `sayari-0.0.75/src/sayari/resource/types/save_entity_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/resource/types/save_entity_response_data.py` & `sayari-0.0.75/src/sayari/resource/types/save_entity_response_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/client.py` & `sayari-0.0.75/src/sayari/search/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/types/coordinates.py` & `sayari-0.0.75/src/sayari/search/types/coordinates.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/types/entity_search_response.py` & `sayari-0.0.75/src/sayari/search/types/entity_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/types/filter_list.py` & `sayari-0.0.75/src/sayari/search/types/filter_list.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/types/record_search_response.py` & `sayari-0.0.75/src/sayari/search/types/record_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/search/types/search_results.py` & `sayari-0.0.75/src/sayari/search/types/search_results.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/__init__.py` & `sayari-0.0.75/src/sayari/shared_errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/errors/__init__.py` & `sayari-0.0.75/src/sayari/shared_errors/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/types/__init__.py` & `sayari-0.0.75/src/sayari/shared_errors/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/types/method_not_allowed_response.py` & `sayari-0.0.75/src/sayari/shared_errors/types/method_not_allowed_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/types/not_acceptable_response.py` & `sayari-0.0.75/src/sayari/shared_errors/types/not_acceptable_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_errors/types/not_found_response.py` & `sayari-0.0.75/src/sayari/shared_errors/types/not_found_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/__init__.py` & `sayari-0.0.75/src/sayari/shared_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/__init__.py` & `sayari-0.0.75/src/sayari/shared_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/coordinate.py` & `sayari-0.0.75/src/sayari/shared_types/types/coordinate.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/core_entity.py` & `sayari-0.0.75/src/sayari/shared_types/types/core_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/embedded_entity.py` & `sayari-0.0.75/src/sayari/shared_types/types/embedded_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/entity_details.py` & `sayari-0.0.75/src/sayari/shared_types/types/entity_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/entity_relationships.py` & `sayari-0.0.75/src/sayari/shared_types/types/entity_relationships.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/entity_summary.py` & `sayari-0.0.75/src/sayari/shared_types/types/entity_summary.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/identifier.py` & `sayari-0.0.75/src/sayari/shared_types/types/identifier.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as.py` & `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as_data.py` & `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/possibly_same_as_match.py` & `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_match.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/psa.py` & `sayari-0.0.75/src/sayari/shared_types/types/psa.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/psa_entity.py` & `sayari-0.0.75/src/sayari/shared_types/types/psa_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/psa_match_keys.py` & `sayari-0.0.75/src/sayari/shared_types/types/psa_match_keys.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/record_details.py` & `sayari-0.0.75/src/sayari/shared_types/types/record_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/referenced_by.py` & `sayari-0.0.75/src/sayari/shared_types/types/referenced_by.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/referenced_by_data.py` & `sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/relationship_data.py` & `sayari-0.0.75/src/sayari/shared_types/types/relationship_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/relationship_info.py` & `sayari-0.0.75/src/sayari/shared_types/types/relationship_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/risk_data.py` & `sayari-0.0.75/src/sayari/shared_types/types/risk_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/source_count_info.py` & `sayari-0.0.75/src/sayari/shared_types/types/source_count_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/shared_types/types/status.py` & `sayari-0.0.75/src/sayari/shared_types/types/status.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/source/client.py` & `sayari-0.0.75/src/sayari/source/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/source/types/get_source_response.py` & `sayari-0.0.75/src/sayari/source/types/get_source_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/source/types/list_sources_response.py` & `sayari-0.0.75/src/sayari/source/types/list_sources_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/source/types/source.py` & `sayari-0.0.75/src/sayari/source/types/source.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/__init__.py` & `sayari-0.0.75/src/sayari/trade/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/client.py` & `sayari-0.0.75/src/sayari/trade/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/__init__.py` & `sayari-0.0.75/src/sayari/trade/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/business_purpose.py` & `sayari-0.0.75/src/sayari/trade/types/business_purpose.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/buyer_search_response.py` & `sayari-0.0.75/src/sayari/trade/types/buyer_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/data_source.py` & `sayari-0.0.75/src/sayari/trade/types/data_source.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/hs_code.py` & `sayari-0.0.75/src/sayari/trade/types/hs_code.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/hs_code_info.py` & `sayari-0.0.75/src/sayari/trade/types/hs_code_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/monetary_value.py` & `sayari-0.0.75/src/sayari/trade/types/monetary_value.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment.py` & `sayari-0.0.75/src/sayari/trade/types/shipment.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment_address.py` & `sayari-0.0.75/src/sayari/trade/types/shipment_address.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment_country.py` & `sayari-0.0.75/src/sayari/trade/types/shipment_country.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment_identifier.py` & `sayari-0.0.75/src/sayari/trade/types/shipment_identifier.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment_metadata.py` & `sayari-0.0.75/src/sayari/trade/types/shipment_metadata.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/shipment_search_response.py` & `sayari-0.0.75/src/sayari/trade/types/shipment_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/source_or_destination_entity.py` & `sayari-0.0.75/src/sayari/trade/types/source_or_destination_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/supplier_metadata.py` & `sayari-0.0.75/src/sayari/trade/types/supplier_metadata.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/supplier_or_buyer.py` & `sayari-0.0.75/src/sayari/trade/types/supplier_or_buyer.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/supplier_search_response.py` & `sayari-0.0.75/src/sayari/trade/types/supplier_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/trade_filter_list.py` & `sayari-0.0.75/src/sayari/trade/types/trade_filter_list.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/trade/types/weight.py` & `sayari-0.0.75/src/sayari/trade/types/weight.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/client.py` & `sayari-0.0.75/src/sayari/traversal/client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/__init__.py` & `sayari-0.0.75/src/sayari/traversal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/shortest_path_data.py` & `sayari-0.0.75/src/sayari/traversal/types/shortest_path_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/shortest_path_response.py` & `sayari-0.0.75/src/sayari/traversal/types/shortest_path_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/traversal_data.py` & `sayari-0.0.75/src/sayari/traversal/types/traversal_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/traversal_path.py` & `sayari-0.0.75/src/sayari/traversal/types/traversal_path.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/traversal_relationship_data.py` & `sayari-0.0.75/src/sayari/traversal/types/traversal_relationship_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/src/sayari/traversal/types/traversal_response.py` & `sayari-0.0.75/src/sayari/traversal/types/traversal_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.74/PKG-INFO` & `sayari-0.0.75/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sayari
-Version: 0.0.74
-Summary: 
+Version: 0.0.75
+Summary: A Python SDK for Sayari
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
```

