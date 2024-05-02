# Comparing `tmp/sayari-0.0.75.tar.gz` & `tmp/sayari-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayari-0.0.75.tar", max compression
+gzip compressed data, was "sayari-0.0.76.tar", max compression
```

## Comparing `sayari-0.0.75.tar` & `sayari-0.0.76.tar`

### file list

```diff
@@ -1,304 +1,304 @@
--rw-r--r--   0        0        0     1401 2024-05-02 16:24:17.902155 sayari-0.0.75/README.md
--rw-r--r--   0        0        0      613 2024-05-02 16:24:17.902155 sayari-0.0.75/pyproject.toml
--rw-r--r--   0        0        0    11506 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/__init__.py
--rw-r--r--   0        0        0      293 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/__init__.py
--rw-r--r--   0        0        0    27153 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/client.py
--rw-r--r--   0        0        0      430 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/__init__.py
--rw-r--r--   0        0        0     1905 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/add_attribute.py
--rw-r--r--   0        0        0      897 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_properties.py
--rw-r--r--   0        0        0     1648 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_response.py
--rw-r--r--   0        0        0      971 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/attribute_response_data.py
--rw-r--r--   0        0        0     1692 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/attributes/types/update_attribute.py
--rw-r--r--   0        0        0      125 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/__init__.py
--rw-r--r--   0        0        0     8440 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/client.py
--rw-r--r--   0        0        0      133 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/types/__init__.py
--rw-r--r--   0        0        0     1191 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/auth/types/auth_response.py
--rw-r--r--   0        0        0     9571 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_client.py
--rw-r--r--   0        0        0      203 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/__init__.py
--rw-r--r--   0        0        0      272 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/__init__.py
--rw-r--r--   0        0        0      151 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/count_qualifier.py
--rw-r--r--   0        0        0     1210 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/paginated_response.py
--rw-r--r--   0        0        0      928 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/base_types/types/qualified_count.py
--rw-r--r--   0        0        0     9751 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/client.py
--rw-r--r--   0        0        0      853 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/api_error.py
--rw-r--r--   0        0        0     2275 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/jsonable_encoder.py
--rw-r--r--   0        0        0     1374 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/oauth_token_provider.py
--rw-r--r--   0        0        0      329 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/core/request_options.py
--rw-r--r--   0        0        0      183 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/__init__.py
--rw-r--r--   0        0        0    34320 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/client.py
--rw-r--r--   0        0        0      233 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/__init__.py
--rw-r--r--   0        0        0     1084 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/entity_summary_response.py
--rw-r--r--   0        0        0     1072 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/entity/types/get_entity_response.py
--rw-r--r--   0        0        0      201 2024-05-02 16:24:17.902155 sayari-0.0.75/src/sayari/environment.py
--rw-r--r--   0        0        0     4187 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/__init__.py
--rw-r--r--   0        0        0     6509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_data.py
--rw-r--r--   0        0        0     1478 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_info.py
--rw-r--r--   0        0        0     1409 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/additional_information_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_data.py
--rw-r--r--   0        0        0     1567 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_info.py
--rw-r--r--   0        0        0     5771 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_properties.py
--rw-r--r--   0        0        0      214 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/address_type.py
--rw-r--r--   0        0        0      932 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attribute_data.py
--rw-r--r--   0        0        0     3055 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attribute_details.py
--rw-r--r--   0        0        0      650 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/attributes.py
--rw-r--r--   0        0        0      249 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/both_identifier_types.py
--rw-r--r--   0        0        0     1065 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_data.py
--rw-r--r--   0        0        0     1302 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_info.py
--rw-r--r--   0        0        0     1560 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_properties.py
--rw-r--r--   0        0        0      649 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/business_purpose_standard.py
--rw-r--r--   0        0        0      488 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_status.py
--rw-r--r--   0        0        0     1049 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_data.py
--rw-r--r--   0        0        0     1293 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_info.py
--rw-r--r--   0        0        0     1182 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/company_type_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_data.py
--rw-r--r--   0        0        0     1192 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_info.py
--rw-r--r--   0        0        0     1429 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_properties.py
--rw-r--r--   0        0        0      174 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/contact_type.py
--rw-r--r--   0        0        0     3929 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country.py
--rw-r--r--   0        0        0      443 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_context.py
--rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_data.py
--rw-r--r--   0        0        0     1244 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_info.py
--rw-r--r--   0        0        0     1580 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/country_properties.py
--rw-r--r--   0        0        0     2940 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/currency.py
--rw-r--r--   0        0        0     1050 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_data.py
--rw-r--r--   0        0        0     1199 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_info.py
--rw-r--r--   0        0        0     1257 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_properties.py
--rw-r--r--   0        0        0      401 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/entities.py
--rw-r--r--   0        0        0      322 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finance_type.py
--rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_data.py
--rw-r--r--   0        0        0     1206 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_info.py
--rw-r--r--   0        0        0     1649 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/finances_properties.py
--rw-r--r--   0        0        0     1044 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_data.py
--rw-r--r--   0        0        0     1226 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_info.py
--rw-r--r--   0        0        0     2406 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/financials_properties.py
--rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender.py
--rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_data.py
--rw-r--r--   0        0        0     1172 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_info.py
--rw-r--r--   0        0        0     1274 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/gender_properties.py
--rw-r--r--   0        0        0     1032 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_data.py
--rw-r--r--   0        0        0     1265 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_info.py
--rw-r--r--   0        0        0     1418 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/generic_properties.py
--rw-r--r--   0        0        0     1044 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_info.py
--rw-r--r--   0        0        0     1324 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_properties.py
--rw-r--r--   0        0        0    16828 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/identifier_type.py
--rw-r--r--   0        0        0     2726 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/language.py
--rw-r--r--   0        0        0     1048 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_info.py
--rw-r--r--   0        0        0     1479 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_properties.py
--rw-r--r--   0        0        0      181 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/measurement_type.py
--rw-r--r--   0        0        0      191 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_context.py
--rw-r--r--   0        0        0     1057 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_data.py
--rw-r--r--   0        0        0     1232 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_info.py
--rw-r--r--   0        0        0     1542 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/monetary_value_properties.py
--rw-r--r--   0        0        0      222 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_context.py
--rw-r--r--   0        0        0     1020 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_data.py
--rw-r--r--   0        0        0     1297 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_info.py
--rw-r--r--   0        0        0     1677 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/name_properties.py
--rw-r--r--   0        0        0      163 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status.py
--rw-r--r--   0        0        0     1053 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_data.py
--rw-r--r--   0        0        0     1238 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_info.py
--rw-r--r--   0        0        0     1260 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/person_status_properties.py
--rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_data.py
--rw-r--r--   0        0        0     1393 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_info.py
--rw-r--r--   0        0        0     1218 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/position_properties.py
--rw-r--r--   0        0        0     1995 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/relationships.py
--rw-r--r--   0        0        0     4122 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk.py
--rw-r--r--   0        0        0     1069 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_data.py
--rw-r--r--   0        0        0     1239 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_info.py
--rw-r--r--   0        0        0     1992 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_properties.py
--rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_data.py
--rw-r--r--   0        0        0     1274 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_info.py
--rw-r--r--   0        0        0     1862 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/shares_properties.py
--rw-r--r--   0        0        0      343 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_context.py
--rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_data.py
--rw-r--r--   0        0        0     1339 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_info.py
--rw-r--r--   0        0        0     1629 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/status_properties.py
--rw-r--r--   0        0        0      848 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/tag.py
--rw-r--r--   0        0        0     1061 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_data.py
--rw-r--r--   0        0        0     1230 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_info.py
--rw-r--r--   0        0        0     1509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translated_name_properties.py
--rw-r--r--   0        0        0      208 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/translation_context.py
--rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/unit.py
--rw-r--r--   0        0        0     1061 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_data.py
--rw-r--r--   0        0        0     1326 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_info.py
--rw-r--r--   0        0        0     1439 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_properties.py
--rw-r--r--   0        0        0     3356 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_type.py
--rw-r--r--   0        0        0      239 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/__init__.py
--rw-r--r--   0        0        0    18664 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/client.py
--rw-r--r--   0        0        0      348 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/__init__.py
--rw-r--r--   0        0        0      121 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/event_info.py
--rw-r--r--   0        0        0      959 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/history_info.py
--rw-r--r--   0        0        0      949 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/history_response.py
--rw-r--r--   0        0        0     1189 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/usage_info.py
--rw-r--r--   0        0        0     1272 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/info/types/usage_response.py
--rw-r--r--   0        0        0      531 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/__init__.py
--rw-r--r--   0        0        0    19516 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/client.py
--rw-r--r--   0        0        0      747 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/__init__.py
--rw-r--r--   0        0        0     1584 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification.py
--rw-r--r--   0        0        0     1086 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification_additional_information.py
--rw-r--r--   0        0        0      148 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/notification_type.py
--rw-r--r--   0        0        0     1296 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/project_notification_data.py
--rw-r--r--   0        0        0     3380 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/project_notifications_response.py
--rw-r--r--   0        0        0     1835 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/resource_notification_data.py
--rw-r--r--   0        0        0     1627 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/notifications/types/resource_notifications_response.py
--rw-r--r--   0        0        0     1179 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/__init__.py
--rw-r--r--   0        0        0    32266 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/client.py
--rw-r--r--   0        0        0     1785 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/__init__.py
--rw-r--r--   0        0        0     1107 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/bucket_agg.py
--rw-r--r--   0        0        0      985 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/create_project_request.py
--rw-r--r--   0        0        0     1390 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/create_project_response.py
--rw-r--r--   0        0        0      852 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/doc_count.py
--rw-r--r--   0        0        0      220 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_project_entities_accept_header.py
--rw-r--r--   0        0        0    14401 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_project_entities_response.py
--rw-r--r--   0        0        0     3197 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/get_projects_response.py
--rw-r--r--   0        0        0      933 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg.py
--rw-r--r--   0        0        0      965 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg_bucket.py
--rw-r--r--   0        0        0      995 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/hs_code_agg_terms.py
--rw-r--r--   0        0        0      851 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/int_key_value.py
--rw-r--r--   0        0        0     1236 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project.py
--rw-r--r--   0        0        0     1084 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_counts.py
--rw-r--r--   0        0        0     1980 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_aggs.py
--rw-r--r--   0        0        0      101 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_aggs_definition.py
--rw-r--r--   0        0        0       93 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entities_filter.py
--rw-r--r--   0        0        0     1755 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entity.py
--rw-r--r--   0        0        0     1010 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_entity_upstream.py
--rw-r--r--   0        0        0     1009 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/project_with_members.py
--rw-r--r--   0        0        0     1014 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/psa_summary.py
--rw-r--r--   0        0        0      157 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role.py
--rw-r--r--   0        0        0      989 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role_member.py
--rw-r--r--   0        0        0      155 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/role_member_type.py
--rw-r--r--   0        0        0      517 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/project/types/sort_field.py
--rw-r--r--   0        0        0        0 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/py.typed
--rw-r--r--   0        0        0      173 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/__init__.py
--rw-r--r--   0        0        0     9509 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/client.py
--rw-r--r--   0        0        0      217 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/__init__.py
--rw-r--r--   0        0        0    10699 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/get_record_response.py
--rw-r--r--   0        0        0     1036 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/record/types/record_references.py
--rw-r--r--   0        0        0      267 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/__init__.py
--rw-r--r--   0        0        0    13242 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/client.py
--rw-r--r--   0        0        0      380 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/__init__.py
--rw-r--r--   0        0        0     1234 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/match_explanation.py
--rw-r--r--   0        0        0     4632 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_response.py
--rw-r--r--   0        0        0     1725 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_response_fields.py
--rw-r--r--   0        0        0     1501 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resolution/types/resolution_result.py
--rw-r--r--   0        0        0      257 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/__init__.py
--rw-r--r--   0        0        0     9347 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/client.py
--rw-r--r--   0        0        0      368 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/__init__.py
--rw-r--r--   0        0        0      146 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/resource_type.py
--rw-r--r--   0        0        0     1254 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_request.py
--rw-r--r--   0        0        0     1528 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_response.py
--rw-r--r--   0        0        0     1095 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/resource/types/save_entity_response_data.py
--rw-r--r--   0        0        0      295 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/__init__.py
--rw-r--r--   0        0        0    45037 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/client.py
--rw-r--r--   0        0        0      444 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/__init__.py
--rw-r--r--   0        0        0      883 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/coordinates.py
--rw-r--r--   0        0        0     6193 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/entity_search_response.py
--rw-r--r--   0        0        0     1478 2024-05-02 16:24:17.906155 sayari-0.0.75/src/sayari/search/types/filter_list.py
--rw-r--r--   0        0        0     3434 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/record_search_response.py
--rw-r--r--   0        0        0     1140 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/search_results.py
--rw-r--r--   0        0        0       80 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/search/types/source_id.py
--rw-r--r--   0        0        0      987 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/__init__.py
--rw-r--r--   0        0        0      658 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/__init__.py
--rw-r--r--   0        0        0      297 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/bad_gateway.py
--rw-r--r--   0        0        0      297 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/bad_request.py
--rw-r--r--   0        0        0      317 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/connection_error.py
--rw-r--r--   0        0        0      334 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/internal_server_error.py
--rw-r--r--   0        0        0      322 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/method_not_allowed.py
--rw-r--r--   0        0        0      309 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/not_acceptable.py
--rw-r--r--   0        0        0      289 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/not_found.py
--rw-r--r--   0        0        0      301 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/rate_limit_exceeded.py
--rw-r--r--   0        0        0      304 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/errors/unauthorized.py
--rw-r--r--   0        0        0      858 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/__init__.py
--rw-r--r--   0        0        0      112 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/bad_gateway_response.py
--rw-r--r--   0        0        0      112 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/bad_request_response.py
--rw-r--r--   0        0        0      117 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/connection_error_response.py
--rw-r--r--   0        0        0      121 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/internal_server_error_response.py
--rw-r--r--   0        0        0      972 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/method_not_allowed_response.py
--rw-r--r--   0        0        0     1028 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/not_acceptable_response.py
--rw-r--r--   0        0        0      972 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/not_found_response.py
--rw-r--r--   0        0        0      111 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/rate_limit_response.py
--rw-r--r--   0        0        0      114 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_errors/types/unauthorized_response.py
--rw-r--r--   0        0        0     1519 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/client_name.py
--rw-r--r--   0        0        0       83 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/company_type.py
--rw-r--r--   0        0        0      882 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/coordinate.py
--rw-r--r--   0        0        0     4362 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/core_entity.py
--rw-r--r--   0        0        0     3746 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/embedded_entity.py
--rw-r--r--   0        0        0     2776 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_details.py
--rw-r--r--   0        0        0       84 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_hs_code.py
--rw-r--r--   0        0        0      131 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_matches.py
--rw-r--r--   0        0        0       94 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_registration_date.py
--rw-r--r--   0        0        0     1279 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_relationships.py
--rw-r--r--   0        0        0      201 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_risk.py
--rw-r--r--   0        0        0      962 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_summary.py
--rw-r--r--   0        0        0       93 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/entity_translated_label.py
--rw-r--r--   0        0        0     1245 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/identifier.py
--rw-r--r--   0        0        0     1249 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as.py
--rw-r--r--   0        0        0     1062 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_data.py
--rw-r--r--   0        0        0      876 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_match.py
--rw-r--r--   0        0        0      981 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa.py
--rw-r--r--   0        0        0     1386 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa_entity.py
--rw-r--r--   0        0        0      888 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/psa_match_keys.py
--rw-r--r--   0        0        0     1785 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/record_details.py
--rw-r--r--   0        0        0     1218 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by.py
--rw-r--r--   0        0        0      998 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data.py
--rw-r--r--   0        0        0      165 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data_type.py
--rw-r--r--   0        0        0      198 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_count.py
--rw-r--r--   0        0        0     1569 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_data.py
--rw-r--r--   0        0        0     1263 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/relationship_info.py
--rw-r--r--   0        0        0     1054 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_data.py
--rw-r--r--   0        0        0      177 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_level.py
--rw-r--r--   0        0        0      123 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/risk_value.py
--rw-r--r--   0        0        0      222 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/search_field.py
--rw-r--r--   0        0        0       87 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/shipment_arrival.py
--rw-r--r--   0        0        0       89 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/shipment_departure.py
--rw-r--r--   0        0        0      948 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/source_count_info.py
--rw-r--r--   0        0        0      977 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/shared_types/types/status.py
--rw-r--r--   0        0        0      197 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/__init__.py
--rw-r--r--   0        0        0    15172 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/client.py
--rw-r--r--   0        0        0      264 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/__init__.py
--rw-r--r--   0        0        0     1029 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/get_source_response.py
--rw-r--r--   0        0        0     2882 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/list_sources_response.py
--rw-r--r--   0        0        0     1318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/source/types/source.py
--rw-r--r--   0        0        0      887 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/__init__.py
--rw-r--r--   0        0        0    31333 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/client.py
--rw-r--r--   0        0        0     1316 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/__init__.py
--rw-r--r--   0        0        0      917 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/business_purpose.py
--rw-r--r--   0        0        0     7236 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/buyer_search_response.py
--rw-r--r--   0        0        0      956 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/data_source.py
--rw-r--r--   0        0        0      924 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/hs_code.py
--rw-r--r--   0        0        0      870 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/hs_code_info.py
--rw-r--r--   0        0        0      998 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/monetary_value.py
--rw-r--r--   0        0        0     1842 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment.py
--rw-r--r--   0        0        0     1071 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_address.py
--rw-r--r--   0        0        0      912 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_country.py
--rw-r--r--   0        0        0      967 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_identifier.py
--rw-r--r--   0        0        0     1318 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_metadata.py
--rw-r--r--   0        0        0     3778 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/shipment_search_response.py
--rw-r--r--   0        0        0     1565 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/source_or_destination_entity.py
--rw-r--r--   0        0        0     1146 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_metadata.py
--rw-r--r--   0        0        0     1052 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_or_buyer.py
--rw-r--r--   0        0        0     4760 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/supplier_search_response.py
--rw-r--r--   0        0        0     5181 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/trade_filter_list.py
--rw-r--r--   0        0        0      876 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/trade/types/weight.py
--rw-r--r--   0        0        0      395 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/__init__.py
--rw-r--r--   0        0        0   104903 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/client.py
--rw-r--r--   0        0        0      539 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/__init__.py
--rw-r--r--   0        0        0     1025 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/shortest_path_data.py
--rw-r--r--   0        0        0    20912 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/shortest_path_response.py
--rw-r--r--   0        0        0     1022 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_data.py
--rw-r--r--   0        0        0     1147 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_path.py
--rw-r--r--   0        0        0     1135 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_relationship_data.py
--rw-r--r--   0        0        0     7818 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/traversal/types/traversal_response.py
--rw-r--r--   0        0        0       74 2024-05-02 16:24:17.910155 sayari-0.0.75/src/sayari/version.py
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 sayari-0.0.75/PKG-INFO
+-rw-r--r--   0        0        0     1401 2024-05-02 17:34:42.339619 sayari-0.0.76/README.md
+-rw-r--r--   0        0        0      613 2024-05-02 17:34:42.339619 sayari-0.0.76/pyproject.toml
+-rw-r--r--   0        0        0    11506 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/__init__.py
+-rw-r--r--   0        0        0    26889 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/client.py
+-rw-r--r--   0        0        0      430 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/__init__.py
+-rw-r--r--   0        0        0     1905 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/add_attribute.py
+-rw-r--r--   0        0        0      897 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/attribute_properties.py
+-rw-r--r--   0        0        0     1648 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/attribute_response.py
+-rw-r--r--   0        0        0      971 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/attribute_response_data.py
+-rw-r--r--   0        0        0     1692 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/attributes/types/update_attribute.py
+-rw-r--r--   0        0        0      125 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/auth/__init__.py
+-rw-r--r--   0        0        0     8352 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/auth/client.py
+-rw-r--r--   0        0        0      133 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/auth/types/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/auth/types/auth_response.py
+-rw-r--r--   0        0        0     9225 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_client.py
+-rw-r--r--   0        0        0      203 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_types/__init__.py
+-rw-r--r--   0        0        0      272 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_types/types/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_types/types/count_qualifier.py
+-rw-r--r--   0        0        0     1210 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_types/types/paginated_response.py
+-rw-r--r--   0        0        0      928 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/base_types/types/qualified_count.py
+-rw-r--r--   0        0        0     9583 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/client.py
+-rw-r--r--   0        0        0      853 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/api_error.py
+-rw-r--r--   0        0        0     2056 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/jsonable_encoder.py
+-rw-r--r--   0        0        0     1374 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/oauth_token_provider.py
+-rw-r--r--   0        0        0      329 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/core/request_options.py
+-rw-r--r--   0        0        0      183 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/entity/__init__.py
+-rw-r--r--   0        0        0    34144 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/entity/client.py
+-rw-r--r--   0        0        0      233 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/entity/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/entity/types/entity_summary_response.py
+-rw-r--r--   0        0        0     1072 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/entity/types/get_entity_response.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/environment.py
+-rw-r--r--   0        0        0     4187 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/__init__.py
+-rw-r--r--   0        0        0     6509 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/__init__.py
+-rw-r--r--   0        0        0     1089 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/additional_information_data.py
+-rw-r--r--   0        0        0     1478 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/additional_information_info.py
+-rw-r--r--   0        0        0     1409 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/additional_information_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/address_data.py
+-rw-r--r--   0        0        0     1567 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/address_info.py
+-rw-r--r--   0        0        0     5771 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/address_properties.py
+-rw-r--r--   0        0        0      214 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/address_type.py
+-rw-r--r--   0        0        0      932 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/attribute_data.py
+-rw-r--r--   0        0        0     3055 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/attribute_details.py
+-rw-r--r--   0        0        0      650 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/attributes.py
+-rw-r--r--   0        0        0      249 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/both_identifier_types.py
+-rw-r--r--   0        0        0     1065 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/business_purpose_data.py
+-rw-r--r--   0        0        0     1302 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/business_purpose_info.py
+-rw-r--r--   0        0        0     1560 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/business_purpose_properties.py
+-rw-r--r--   0        0        0      649 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/business_purpose_standard.py
+-rw-r--r--   0        0        0      488 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/company_status.py
+-rw-r--r--   0        0        0     1049 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/company_type_data.py
+-rw-r--r--   0        0        0     1293 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/company_type_info.py
+-rw-r--r--   0        0        0     1182 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/company_type_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/contact_data.py
+-rw-r--r--   0        0        0     1192 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/contact_info.py
+-rw-r--r--   0        0        0     1429 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/contact_properties.py
+-rw-r--r--   0        0        0      174 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/contact_type.py
+-rw-r--r--   0        0        0     3929 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/country.py
+-rw-r--r--   0        0        0      443 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/country_context.py
+-rw-r--r--   0        0        0     1032 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/country_data.py
+-rw-r--r--   0        0        0     1244 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/country_info.py
+-rw-r--r--   0        0        0     1580 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/country_properties.py
+-rw-r--r--   0        0        0     2940 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/currency.py
+-rw-r--r--   0        0        0     1050 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_data.py
+-rw-r--r--   0        0        0     1199 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_info.py
+-rw-r--r--   0        0        0     1257 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_properties.py
+-rw-r--r--   0        0        0      401 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/entities.py
+-rw-r--r--   0        0        0      322 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/finance_type.py
+-rw-r--r--   0        0        0     1036 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/finances_data.py
+-rw-r--r--   0        0        0     1206 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/finances_info.py
+-rw-r--r--   0        0        0     1649 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/finances_properties.py
+-rw-r--r--   0        0        0     1044 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/financials_data.py
+-rw-r--r--   0        0        0     1226 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/financials_info.py
+-rw-r--r--   0        0        0     2406 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/financials_properties.py
+-rw-r--r--   0        0        0      157 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/gender.py
+-rw-r--r--   0        0        0     1028 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/gender_data.py
+-rw-r--r--   0        0        0     1172 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/gender_info.py
+-rw-r--r--   0        0        0     1274 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/gender_properties.py
+-rw-r--r--   0        0        0     1032 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/generic_data.py
+-rw-r--r--   0        0        0     1265 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/generic_info.py
+-rw-r--r--   0        0        0     1418 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/generic_properties.py
+-rw-r--r--   0        0        0     1044 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/identifier_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/identifier_info.py
+-rw-r--r--   0        0        0     1324 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/identifier_properties.py
+-rw-r--r--   0        0        0    16828 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/identifier_type.py
+-rw-r--r--   0        0        0     2726 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/language.py
+-rw-r--r--   0        0        0     1048 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/measurement_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/measurement_info.py
+-rw-r--r--   0        0        0     1479 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/measurement_properties.py
+-rw-r--r--   0        0        0      181 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/measurement_type.py
+-rw-r--r--   0        0        0      191 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/monetary_value_context.py
+-rw-r--r--   0        0        0     1057 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/monetary_value_data.py
+-rw-r--r--   0        0        0     1232 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/monetary_value_info.py
+-rw-r--r--   0        0        0     1542 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/monetary_value_properties.py
+-rw-r--r--   0        0        0      222 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/name_context.py
+-rw-r--r--   0        0        0     1020 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/name_data.py
+-rw-r--r--   0        0        0     1297 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/name_info.py
+-rw-r--r--   0        0        0     1677 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/name_properties.py
+-rw-r--r--   0        0        0      163 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/person_status.py
+-rw-r--r--   0        0        0     1053 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/person_status_data.py
+-rw-r--r--   0        0        0     1238 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/person_status_info.py
+-rw-r--r--   0        0        0     1260 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/person_status_properties.py
+-rw-r--r--   0        0        0     1036 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/position_data.py
+-rw-r--r--   0        0        0     1393 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/position_info.py
+-rw-r--r--   0        0        0     1218 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/position_properties.py
+-rw-r--r--   0        0        0     1995 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/relationships.py
+-rw-r--r--   0        0        0     4122 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/risk.py
+-rw-r--r--   0        0        0     1069 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_data.py
+-rw-r--r--   0        0        0     1239 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_info.py
+-rw-r--r--   0        0        0     1992 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_properties.py
+-rw-r--r--   0        0        0     1028 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/shares_data.py
+-rw-r--r--   0        0        0     1274 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/shares_info.py
+-rw-r--r--   0        0        0     1862 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/shares_properties.py
+-rw-r--r--   0        0        0      343 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/status_context.py
+-rw-r--r--   0        0        0     1028 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/status_data.py
+-rw-r--r--   0        0        0     1339 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/status_info.py
+-rw-r--r--   0        0        0     1629 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/status_properties.py
+-rw-r--r--   0        0        0      848 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/tag.py
+-rw-r--r--   0        0        0     1061 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/translated_name_data.py
+-rw-r--r--   0        0        0     1230 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/translated_name_info.py
+-rw-r--r--   0        0        0     1509 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/translated_name_properties.py
+-rw-r--r--   0        0        0      208 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/translation_context.py
+-rw-r--r--   0        0        0      157 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/unit.py
+-rw-r--r--   0        0        0     1061 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_data.py
+-rw-r--r--   0        0        0     1326 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_info.py
+-rw-r--r--   0        0        0     1439 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_properties.py
+-rw-r--r--   0        0        0     3356 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_type.py
+-rw-r--r--   0        0        0      239 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/__init__.py
+-rw-r--r--   0        0        0    18488 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/client.py
+-rw-r--r--   0        0        0      348 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/__init__.py
+-rw-r--r--   0        0        0      121 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/event_info.py
+-rw-r--r--   0        0        0      959 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/history_info.py
+-rw-r--r--   0        0        0      949 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/history_response.py
+-rw-r--r--   0        0        0     1189 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/usage_info.py
+-rw-r--r--   0        0        0     1272 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/info/types/usage_response.py
+-rw-r--r--   0        0        0      531 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/__init__.py
+-rw-r--r--   0        0        0    19340 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/client.py
+-rw-r--r--   0        0        0      747 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/types/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/types/notification.py
+-rw-r--r--   0        0        0     1086 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/types/notification_additional_information.py
+-rw-r--r--   0        0        0      148 2024-05-02 17:34:42.343619 sayari-0.0.76/src/sayari/notifications/types/notification_type.py
+-rw-r--r--   0        0        0     1296 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/notifications/types/project_notification_data.py
+-rw-r--r--   0        0        0     3380 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/notifications/types/project_notifications_response.py
+-rw-r--r--   0        0        0     1835 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/notifications/types/resource_notification_data.py
+-rw-r--r--   0        0        0     1627 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/notifications/types/resource_notifications_response.py
+-rw-r--r--   0        0        0     1179 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/__init__.py
+-rw-r--r--   0        0        0    32002 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/client.py
+-rw-r--r--   0        0        0     1785 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/__init__.py
+-rw-r--r--   0        0        0     1107 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/bucket_agg.py
+-rw-r--r--   0        0        0      985 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/create_project_request.py
+-rw-r--r--   0        0        0     1390 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/create_project_response.py
+-rw-r--r--   0        0        0      852 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/doc_count.py
+-rw-r--r--   0        0        0      220 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/get_project_entities_accept_header.py
+-rw-r--r--   0        0        0    14401 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/get_project_entities_response.py
+-rw-r--r--   0        0        0     3197 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/get_projects_response.py
+-rw-r--r--   0        0        0      933 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/hs_code_agg.py
+-rw-r--r--   0        0        0      965 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/hs_code_agg_bucket.py
+-rw-r--r--   0        0        0      995 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/hs_code_agg_terms.py
+-rw-r--r--   0        0        0      851 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/int_key_value.py
+-rw-r--r--   0        0        0     1236 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project.py
+-rw-r--r--   0        0        0     1084 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_counts.py
+-rw-r--r--   0        0        0     1980 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_entities_aggs.py
+-rw-r--r--   0        0        0      101 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_entities_aggs_definition.py
+-rw-r--r--   0        0        0       93 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_entities_filter.py
+-rw-r--r--   0        0        0     1755 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_entity.py
+-rw-r--r--   0        0        0     1010 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_entity_upstream.py
+-rw-r--r--   0        0        0     1009 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/project_with_members.py
+-rw-r--r--   0        0        0     1014 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/psa_summary.py
+-rw-r--r--   0        0        0      157 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/role.py
+-rw-r--r--   0        0        0      989 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/role_member.py
+-rw-r--r--   0        0        0      155 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/role_member_type.py
+-rw-r--r--   0        0        0      517 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/project/types/sort_field.py
+-rw-r--r--   0        0        0        0 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/py.typed
+-rw-r--r--   0        0        0      173 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/record/__init__.py
+-rw-r--r--   0        0        0     9421 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/record/client.py
+-rw-r--r--   0        0        0      217 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/record/types/__init__.py
+-rw-r--r--   0        0        0    10699 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/record/types/get_record_response.py
+-rw-r--r--   0        0        0     1036 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/record/types/record_references.py
+-rw-r--r--   0        0        0      267 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/__init__.py
+-rw-r--r--   0        0        0    13154 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/client.py
+-rw-r--r--   0        0        0      380 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/types/__init__.py
+-rw-r--r--   0        0        0     1234 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/types/match_explanation.py
+-rw-r--r--   0        0        0     4632 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/types/resolution_response.py
+-rw-r--r--   0        0        0     1725 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/types/resolution_response_fields.py
+-rw-r--r--   0        0        0     1501 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resolution/types/resolution_result.py
+-rw-r--r--   0        0        0      257 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/__init__.py
+-rw-r--r--   0        0        0     9259 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/client.py
+-rw-r--r--   0        0        0      368 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/types/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/types/resource_type.py
+-rw-r--r--   0        0        0     1254 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/types/save_entity_request.py
+-rw-r--r--   0        0        0     1528 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/types/save_entity_response.py
+-rw-r--r--   0        0        0     1095 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/resource/types/save_entity_response_data.py
+-rw-r--r--   0        0        0      295 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/__init__.py
+-rw-r--r--   0        0        0    44685 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/client.py
+-rw-r--r--   0        0        0      444 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/coordinates.py
+-rw-r--r--   0        0        0     6193 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/entity_search_response.py
+-rw-r--r--   0        0        0     1478 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/filter_list.py
+-rw-r--r--   0        0        0     3434 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/record_search_response.py
+-rw-r--r--   0        0        0     1140 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/search_results.py
+-rw-r--r--   0        0        0       80 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/search/types/source_id.py
+-rw-r--r--   0        0        0      987 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/__init__.py
+-rw-r--r--   0        0        0      658 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/bad_gateway.py
+-rw-r--r--   0        0        0      297 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/bad_request.py
+-rw-r--r--   0        0        0      317 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/connection_error.py
+-rw-r--r--   0        0        0      334 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/internal_server_error.py
+-rw-r--r--   0        0        0      322 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/method_not_allowed.py
+-rw-r--r--   0        0        0      309 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/not_acceptable.py
+-rw-r--r--   0        0        0      289 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/not_found.py
+-rw-r--r--   0        0        0      301 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/rate_limit_exceeded.py
+-rw-r--r--   0        0        0      304 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/errors/unauthorized.py
+-rw-r--r--   0        0        0      858 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/bad_gateway_response.py
+-rw-r--r--   0        0        0      112 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/bad_request_response.py
+-rw-r--r--   0        0        0      117 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/connection_error_response.py
+-rw-r--r--   0        0        0      121 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/internal_server_error_response.py
+-rw-r--r--   0        0        0      972 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/method_not_allowed_response.py
+-rw-r--r--   0        0        0     1028 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/not_acceptable_response.py
+-rw-r--r--   0        0        0      972 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/not_found_response.py
+-rw-r--r--   0        0        0      111 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/rate_limit_response.py
+-rw-r--r--   0        0        0      114 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_errors/types/unauthorized_response.py
+-rw-r--r--   0        0        0     1519 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/client_name.py
+-rw-r--r--   0        0        0       83 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/company_type.py
+-rw-r--r--   0        0        0      882 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/coordinate.py
+-rw-r--r--   0        0        0     4362 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/core_entity.py
+-rw-r--r--   0        0        0     3746 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/embedded_entity.py
+-rw-r--r--   0        0        0     2776 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_details.py
+-rw-r--r--   0        0        0       84 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_hs_code.py
+-rw-r--r--   0        0        0      131 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_matches.py
+-rw-r--r--   0        0        0       94 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_registration_date.py
+-rw-r--r--   0        0        0     1279 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_relationships.py
+-rw-r--r--   0        0        0      201 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_risk.py
+-rw-r--r--   0        0        0      962 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_summary.py
+-rw-r--r--   0        0        0       93 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/entity_translated_label.py
+-rw-r--r--   0        0        0     1245 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/identifier.py
+-rw-r--r--   0        0        0     1249 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as.py
+-rw-r--r--   0        0        0     1062 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as_data.py
+-rw-r--r--   0        0        0      876 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as_match.py
+-rw-r--r--   0        0        0      981 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/psa.py
+-rw-r--r--   0        0        0     1386 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/psa_entity.py
+-rw-r--r--   0        0        0      888 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/psa_match_keys.py
+-rw-r--r--   0        0        0     1785 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/record_details.py
+-rw-r--r--   0        0        0     1218 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/referenced_by.py
+-rw-r--r--   0        0        0      998 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/referenced_by_data.py
+-rw-r--r--   0        0        0      165 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/referenced_by_data_type.py
+-rw-r--r--   0        0        0      198 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/relationship_count.py
+-rw-r--r--   0        0        0     1569 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/relationship_data.py
+-rw-r--r--   0        0        0     1263 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/relationship_info.py
+-rw-r--r--   0        0        0     1054 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/risk_data.py
+-rw-r--r--   0        0        0      177 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/risk_level.py
+-rw-r--r--   0        0        0      123 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/risk_value.py
+-rw-r--r--   0        0        0      222 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/search_field.py
+-rw-r--r--   0        0        0       87 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/shipment_arrival.py
+-rw-r--r--   0        0        0       89 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/shipment_departure.py
+-rw-r--r--   0        0        0      948 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/source_count_info.py
+-rw-r--r--   0        0        0      977 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/shared_types/types/status.py
+-rw-r--r--   0        0        0      197 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/__init__.py
+-rw-r--r--   0        0        0    14996 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/client.py
+-rw-r--r--   0        0        0      264 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/types/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/types/get_source_response.py
+-rw-r--r--   0        0        0     2882 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/types/list_sources_response.py
+-rw-r--r--   0        0        0     1318 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/source/types/source.py
+-rw-r--r--   0        0        0      887 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/__init__.py
+-rw-r--r--   0        0        0    31069 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/client.py
+-rw-r--r--   0        0        0     1316 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/__init__.py
+-rw-r--r--   0        0        0      917 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/business_purpose.py
+-rw-r--r--   0        0        0     7236 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/buyer_search_response.py
+-rw-r--r--   0        0        0      956 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/data_source.py
+-rw-r--r--   0        0        0      924 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/hs_code.py
+-rw-r--r--   0        0        0      870 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/hs_code_info.py
+-rw-r--r--   0        0        0      998 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/monetary_value.py
+-rw-r--r--   0        0        0     1842 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment.py
+-rw-r--r--   0        0        0     1071 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment_address.py
+-rw-r--r--   0        0        0      912 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment_country.py
+-rw-r--r--   0        0        0      967 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment_identifier.py
+-rw-r--r--   0        0        0     1318 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment_metadata.py
+-rw-r--r--   0        0        0     3778 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/shipment_search_response.py
+-rw-r--r--   0        0        0     1565 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/source_or_destination_entity.py
+-rw-r--r--   0        0        0     1146 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/supplier_metadata.py
+-rw-r--r--   0        0        0     1052 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/supplier_or_buyer.py
+-rw-r--r--   0        0        0     4760 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/supplier_search_response.py
+-rw-r--r--   0        0        0     5181 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/trade_filter_list.py
+-rw-r--r--   0        0        0      876 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/trade/types/weight.py
+-rw-r--r--   0        0        0      395 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/__init__.py
+-rw-r--r--   0        0        0   104463 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/client.py
+-rw-r--r--   0        0        0      539 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/__init__.py
+-rw-r--r--   0        0        0     1025 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/shortest_path_data.py
+-rw-r--r--   0        0        0    20912 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/shortest_path_response.py
+-rw-r--r--   0        0        0     1022 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/traversal_data.py
+-rw-r--r--   0        0        0     1147 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/traversal_path.py
+-rw-r--r--   0        0        0     1135 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/traversal_relationship_data.py
+-rw-r--r--   0        0        0     7818 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/traversal/types/traversal_response.py
+-rw-r--r--   0        0        0       74 2024-05-02 17:34:42.347619 sayari-0.0.76/src/sayari/version.py
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 sayari-0.0.76/PKG-INFO
```

### Comparing `sayari-0.0.75/README.md` & `sayari-0.0.76/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 ```
 <!-- End Installation  -->
 
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
-from sayari.client import Client
+from sayari.client import Sayari
 
-client = Client(
+client = Sayari(
     client_id="YOUR_CLIENT_ID",
     client_secret="YOUR_CLIENT_SECRET",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
-from sayari.client import AsyncClient
+from sayari.client import AsyncSayari
 
-client = AsyncClient(
+client = AsyncSayari(
     client_id="YOUR_CLIENT_ID",
     client_secret="YOUR_CLIENT_SECRET",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
```

### Comparing `sayari-0.0.75/pyproject.toml` & `sayari-0.0.76/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sayari"
-version = "0.0.75"
 description = "A Python SDK for Sayari"
+version = "0.0.76"
 readme = "README.md"
 authors = []
 packages = [
     { include = "sayari", from = "src"}
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `sayari-0.0.75/src/sayari/__init__.py` & `sayari-0.0.76/src/sayari/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     trade,
     traversal,
 )
 from .attributes import AddAttribute, AttributeProperties, AttributeResponse, AttributeResponseData, UpdateAttribute
 from .auth import AuthResponse
 from .base_types import CountQualifier, PaginatedResponse, QualifiedCount
 from .entity import EntitySummaryResponse, GetEntityResponse
-from .environment import ClientEnvironment
+from .environment import SayariEnvironment
 from .generated_types import (
     AdditionalInformationData,
     AdditionalInformationInfo,
     AdditionalInformationProperties,
     AddressData,
     AddressInfo,
     AddressProperties,
@@ -271,15 +271,14 @@
     "BucketAgg",
     "BusinessPurpose",
     "BusinessPurposeData",
     "BusinessPurposeInfo",
     "BusinessPurposeProperties",
     "BusinessPurposeStandard",
     "BuyerSearchResponse",
-    "ClientEnvironment",
     "ClientName",
     "CompanyStatus",
     "CompanyType",
     "CompanyTypeData",
     "CompanyTypeInfo",
     "CompanyTypeProperties",
     "ConnectionError",
@@ -432,14 +431,15 @@
     "RiskValue",
     "Role",
     "RoleMember",
     "RoleMemberType",
     "SaveEntityRequest",
     "SaveEntityResponse",
     "SaveEntityResponseData",
+    "SayariEnvironment",
     "SearchField",
     "SearchResults",
     "SharesData",
     "SharesInfo",
     "SharesProperties",
     "Shipment",
     "ShipmentAddress",
```

### Comparing `sayari-0.0.75/src/sayari/attributes/client.py` & `sayari-0.0.76/src/sayari/attributes/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,17 @@
 
         Parameters:
             - request: AddAttribute.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import AddAttribute
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.attributes.post_attribute(
             request=AddAttribute(
                 entity="zq04axX2dLn9tE6W6Q8Qhg",
                 type="address",
@@ -134,18 +133,17 @@
             - attribute_id: str.
 
             - request: UpdateAttribute.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import UpdateAttribute
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.attributes.patch_attribute(
             attribute_id="enEwNGF4WDJkTG45dEU2VzZROFFoZ3xhZGRyZXNzfDBwbEVCMHxVNzhzN21yOUVFTThIZ3pwREM3UDFB",
             request=UpdateAttribute(
                 value={
@@ -222,18 +220,17 @@
         <Callout intent="warning">This endpoint is in beta and is subject to change. It is provided for early access and testing purposes only.</Callout> Delete an existing Attribute
 
         Parameters:
             - attribute_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.attributes.delete_attribute(
             attribute_id="enEwNGF4WDJkTG45dEU2VzZROFFoZ3xhZGRyZXNzfDBwbEVCMHxVNzhzN21yOUVFTThIZ3pwREM3UDFB",
         )
         """
@@ -298,18 +295,17 @@
 
         Parameters:
             - request: AddAttribute.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import AddAttribute
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.attributes.post_attribute(
             request=AddAttribute(
                 entity="zq04axX2dLn9tE6W6Q8Qhg",
                 type="address",
@@ -386,18 +382,17 @@
             - attribute_id: str.
 
             - request: UpdateAttribute.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import UpdateAttribute
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.attributes.patch_attribute(
             attribute_id="enEwNGF4WDJkTG45dEU2VzZROFFoZ3xhZGRyZXNzfDBwbEVCMHxVNzhzN21yOUVFTThIZ3pwREM3UDFB",
             request=UpdateAttribute(
                 value={
@@ -474,18 +469,17 @@
         <Callout intent="warning">This endpoint is in beta and is subject to change. It is provided for early access and testing purposes only.</Callout> Delete an existing Attribute
 
         Parameters:
             - attribute_id: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.attributes.delete_attribute(
             attribute_id="enEwNGF4WDJkTG45dEU2VzZROFFoZ3xhZGRyZXNzfDBwbEVCMHxVNzhzN21yOUVFTThIZ3pwREM3UDFB",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/attributes/types/add_attribute.py` & `sayari-0.0.76/src/sayari/attributes/types/add_attribute.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/attributes/types/attribute_properties.py` & `sayari-0.0.76/src/sayari/attributes/types/attribute_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/attributes/types/attribute_response.py` & `sayari-0.0.76/src/sayari/attributes/types/attribute_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/attributes/types/attribute_response_data.py` & `sayari-0.0.76/src/sayari/attributes/types/attribute_response_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/attributes/types/update_attribute.py` & `sayari-0.0.76/src/sayari/attributes/types/update_attribute.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/auth/client.py` & `sayari-0.0.76/src/sayari/auth/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,17 @@
         Parameters:
             - client_id: str.
 
             - client_secret: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.auth.get_token(
             client_id="your client_id here",
             client_secret="your client_secret here",
         )
@@ -121,18 +120,17 @@
         Parameters:
             - client_id: str.
 
             - client_secret: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.auth.get_token(
             client_id="your client_id here",
             client_secret="your client_secret here",
         )
```

### Comparing `sayari-0.0.75/src/sayari/auth/types/auth_response.py` & `sayari-0.0.76/src/sayari/auth/types/auth_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/base_client.py` & `sayari-0.0.76/src/sayari/base_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import httpx
 
 from .attributes.client import AsyncAttributesClient, AttributesClient
 from .auth.client import AsyncAuthClient, AuthClient
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.oauth_token_provider import OAuthTokenProvider
 from .entity.client import AsyncEntityClient, EntityClient
-from .environment import ClientEnvironment
+from .environment import SayariEnvironment
 from .info.client import AsyncInfoClient, InfoClient
 from .notifications.client import AsyncNotificationsClient, NotificationsClient
 from .project.client import AsyncProjectClient, ProjectClient
 from .record.client import AsyncRecordClient, RecordClient
 from .resolution.client import AsyncResolutionClient, ResolutionClient
 from .resource.client import AsyncResourceClient, ResourceClient
 from .search.client import AsyncSearchClient, SearchClient
@@ -25,67 +25,61 @@
 class BaseClient:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
         - base_url: typing.Optional[str]. The base url to use for requests from the client.
 
-        - environment: ClientEnvironment. The environment to use for requests from the client. from .environment import ClientEnvironment
+        - environment: SayariEnvironment. The environment to use for requests from the client. from .environment import SayariEnvironment
 
-                                          Defaults to ClientEnvironment.PRODUCTION
-
-        - client_name: str.
+                                          Defaults to SayariEnvironment.PRODUCTION
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
         - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
         - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
         - client_id: str.
 
         - client_secret: str.
     ---
-    from sayari.client import Client
+    from sayari.client import Sayari
 
-    client = Client(
-        client_name="YOUR_CLIENT_NAME",
+    client = Sayari(
         client_id="YOUR_CLIENT_ID",
         client_secret="YOUR_CLIENT_SECRET",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
-        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
-        client_name: str,
+        environment: SayariEnvironment = SayariEnvironment.PRODUCTION,
         timeout: typing.Optional[float] = None,
         follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None,
         client_id: str,
         client_secret: str
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         oauth_token_provider = OAuthTokenProvider(
             client_id=client_id,
             client_secret=client_secret,
             client_wrapper=SyncClientWrapper(
                 base_url=_get_base_url(base_url=base_url, environment=environment),
-                client_name=client_name,
                 httpx_client=httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
                 if follow_redirects is not None
                 else httpx.Client(timeout=_defaulted_timeout),
                 timeout=_defaulted_timeout,
             ),
         )
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
-            client_name=client_name,
             token=oauth_token_provider.get_token,
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
@@ -108,67 +102,61 @@
 class AsyncBaseClient:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
     Parameters:
         - base_url: typing.Optional[str]. The base url to use for requests from the client.
 
-        - environment: ClientEnvironment. The environment to use for requests from the client. from .environment import ClientEnvironment
-
-                                          Defaults to ClientEnvironment.PRODUCTION
+        - environment: SayariEnvironment. The environment to use for requests from the client. from .environment import SayariEnvironment
 
-        - client_name: str.
+                                          Defaults to SayariEnvironment.PRODUCTION
 
         - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
         - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
         - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
         - client_id: str.
 
         - client_secret: str.
     ---
-    from sayari.client import AsyncClient
+    from sayari.client import AsyncSayari
 
-    client = AsyncClient(
-        client_name="YOUR_CLIENT_NAME",
+    client = AsyncSayari(
         client_id="YOUR_CLIENT_ID",
         client_secret="YOUR_CLIENT_SECRET",
     )
     """
 
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
-        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
-        client_name: str,
+        environment: SayariEnvironment = SayariEnvironment.PRODUCTION,
         timeout: typing.Optional[float] = None,
         follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
         client_id: str,
         client_secret: str
     ):
         _defaulted_timeout = timeout if timeout is not None else 60 if httpx_client is None else None
         oauth_token_provider = OAuthTokenProvider(
             client_id=client_id,
             client_secret=client_secret,
             client_wrapper=SyncClientWrapper(
                 base_url=_get_base_url(base_url=base_url, environment=environment),
-                client_name=client_name,
                 httpx_client=httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
                 if follow_redirects is not None
                 else httpx.Client(timeout=_defaulted_timeout),
                 timeout=_defaulted_timeout,
             ),
         )
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
-            client_name=client_name,
             token=oauth_token_provider.get_token,
             httpx_client=httpx_client
             if httpx_client is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
@@ -184,14 +172,14 @@
         self.resource = AsyncResourceClient(client_wrapper=self._client_wrapper)
         self.search = AsyncSearchClient(client_wrapper=self._client_wrapper)
         self.source = AsyncSourceClient(client_wrapper=self._client_wrapper)
         self.trade = AsyncTradeClient(client_wrapper=self._client_wrapper)
         self.traversal = AsyncTraversalClient(client_wrapper=self._client_wrapper)
 
 
-def _get_base_url(*, base_url: typing.Optional[str] = None, environment: ClientEnvironment) -> str:
+def _get_base_url(*, base_url: typing.Optional[str] = None, environment: SayariEnvironment) -> str:
     if base_url is not None:
         return base_url
     elif environment is not None:
         return environment.value
     else:
         raise Exception("Please pass in either base_url or environment to construct the client")
```

### Comparing `sayari-0.0.75/src/sayari/base_types/types/paginated_response.py` & `sayari-0.0.76/src/sayari/base_types/types/paginated_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/base_types/types/qualified_count.py` & `sayari-0.0.76/src/sayari/base_types/types/qualified_count.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/client.py` & `sayari-0.0.76/src/sayari/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import httpx
 import urllib.parse
 import csv
 import queue
 import time
 from multiprocessing import Process, Queue, set_start_method
 from .base_client import BaseClient, AsyncBaseClient
-from .environment import ClientEnvironment
+from .environment import SayariEnvironment
 
 # resolution attributes
 Name = "name"
 Identifier = "identifier"
 Country = "country"
 Address = "address"
 DOB = "dateofbirth"
@@ -60,26 +60,24 @@
         client_secret="YOUR_CLIENT_SECRET",
     )
     """
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
-        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
+        environment: SayariEnvironment = SayariEnvironment.PRODUCTION,
         timeout: typing.Optional[float] = None,
         follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None,
         client_id: str,
         client_secret: str
     ):
         super().__init__(
             base_url=base_url,
             environment=environment,
-            # TODO: capture version info here
-            client_name="python_sdk",
             timeout=timeout,
             follow_redirects=follow_redirects,
             httpx_client=httpx_client,
             client_id=client_id,
             client_secret=client_secret
         )
 
@@ -163,26 +161,24 @@
         client_secret="YOUR_CLIENT_SECRET",
     )
     """
     def __init__(
         self,
         *,
         base_url: typing.Optional[str] = None,
-        environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
+        environment: SayariEnvironment = SayariEnvironment.PRODUCTION,
         timeout: typing.Optional[float] = None,
         follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
         client_id: str,
         client_secret: str
     ):
         super().__init__(
             base_url=base_url,
             environment=environment,
-            # TODO: capture version info here
-            client_name="python_sdk",
             timeout=timeout,
             follow_redirects=follow_redirects,
             httpx_client=httpx_client,
             client_id=client_id,
             client_secret=client_secret
         )
```

### Comparing `sayari-0.0.75/src/sayari/core/__init__.py` & `sayari-0.0.76/src/sayari/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/client_wrapper.py` & `sayari-0.0.76/src/sayari/core/client_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,28 @@
 from .http_client import AsyncHttpClient, HttpClient
 
 
 class BaseClientWrapper:
     def __init__(
         self,
         *,
-        client_name: str,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         base_url: str,
         timeout: typing.Optional[float] = None,
     ):
-        self._client_name = client_name
         self._token = token
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "sayari",
-            "X-Fern-SDK-Version": "0.0.75",
+            "X-Fern-SDK-Version": "0.0.76",
         }
-        headers["client-name"] = self._client_name
         token = self._get_token()
         if token is not None:
             headers["Authorization"] = f"Bearer {token}"
         return headers
 
     def _get_token(self) -> typing.Optional[str]:
         if isinstance(self._token, str) or self._token is None:
@@ -46,29 +43,27 @@
         return self._timeout
 
 
 class SyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
-        client_name: str,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         base_url: str,
         timeout: typing.Optional[float] = None,
         httpx_client: httpx.Client,
     ):
-        super().__init__(client_name=client_name, token=token, base_url=base_url, timeout=timeout)
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
         self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
-        client_name: str,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = None,
         base_url: str,
         timeout: typing.Optional[float] = None,
         httpx_client: httpx.AsyncClient,
     ):
-        super().__init__(client_name=client_name, token=token, base_url=base_url, timeout=timeout)
+        super().__init__(token=token, base_url=base_url, timeout=timeout)
         self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `sayari-0.0.75/src/sayari/core/datetime_utils.py` & `sayari-0.0.76/src/sayari/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/file.py` & `sayari-0.0.76/src/sayari/core/file.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/http_client.py` & `sayari-0.0.76/src/sayari/core/http_client.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/jsonable_encoder.py` & `sayari-0.0.76/src/sayari/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/oauth_token_provider.py` & `sayari-0.0.76/src/sayari/core/oauth_token_provider.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/core/request_options.py` & `sayari-0.0.76/src/sayari/core/request_options.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/entity/client.py` & `sayari-0.0.76/src/sayari/entity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,17 @@
 
             - referenced_by_prev: typing.Optional[str]. The pagination token for the previous page of the entity's referencing records
 
             - referenced_by_limit: typing.Optional[int]. Limit totals values returned for entity's referencing records. Defaults to 100.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.entity.get_entity(
             id="mGq1lpuqKssNWTjIokuPeA",
             attributes_name_limit=1,
             attributes_address_limit=1,
@@ -258,18 +257,17 @@
         The Entity Summary endpoint returns a smaller entity payload
 
         Parameters:
             - id: str. Unique identifier of the entity
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.entity.entity_summary(
             id="mGq1lpuqKssNWTjIokuPeA",
         )
         """
@@ -431,18 +429,17 @@
 
             - referenced_by_prev: typing.Optional[str]. The pagination token for the previous page of the entity's referencing records
 
             - referenced_by_limit: typing.Optional[int]. Limit totals values returned for entity's referencing records. Defaults to 100.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.entity.get_entity(
             id="mGq1lpuqKssNWTjIokuPeA",
             attributes_name_limit=1,
             attributes_address_limit=1,
@@ -546,18 +543,17 @@
         The Entity Summary endpoint returns a smaller entity payload
 
         Parameters:
             - id: str. Unique identifier of the entity
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.entity.entity_summary(
             id="mGq1lpuqKssNWTjIokuPeA",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/entity/types/entity_summary_response.py` & `sayari-0.0.76/src/sayari/entity/types/entity_summary_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/entity/types/get_entity_response.py` & `sayari-0.0.76/src/sayari/entity/types/get_entity_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/__init__.py` & `sayari-0.0.76/src/sayari/generated_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/__init__.py` & `sayari-0.0.76/src/sayari/generated_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/additional_information_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/additional_information_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/additional_information_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/additional_information_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/additional_information_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/additional_information_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/address_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/address_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/address_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/address_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/address_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/address_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/attribute_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/attribute_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/attribute_details.py` & `sayari-0.0.76/src/sayari/generated_types/types/attribute_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/attributes.py` & `sayari-0.0.76/src/sayari/generated_types/types/attributes.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/business_purpose_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/business_purpose_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/business_purpose_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/business_purpose_standard.py` & `sayari-0.0.76/src/sayari/generated_types/types/business_purpose_standard.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/company_type_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/company_type_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/company_type_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/company_type_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/company_type_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/company_type_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/contact_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/contact_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/contact_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/contact_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/contact_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/contact_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/country.py` & `sayari-0.0.76/src/sayari/generated_types/types/country.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/country_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/country_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/country_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/country_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/country_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/country_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/currency.py` & `sayari-0.0.76/src/sayari/generated_types/types/currency.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/date_of_birth_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/date_of_birth_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/finances_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/finances_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/finances_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/finances_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/finances_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/finances_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/financials_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/financials_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/financials_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/financials_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/financials_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/financials_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/gender_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/gender_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/gender_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/gender_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/gender_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/gender_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/generic_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/generic_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/generic_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/generic_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/generic_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/generic_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/identifier_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/identifier_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/identifier_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/identifier_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/identifier_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/identifier_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/identifier_type.py` & `sayari-0.0.76/src/sayari/generated_types/types/identifier_type.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/language.py` & `sayari-0.0.76/src/sayari/generated_types/types/language.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/measurement_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/measurement_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/measurement_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/measurement_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/measurement_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/measurement_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/monetary_value_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/monetary_value_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/monetary_value_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/monetary_value_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/name_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/name_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/name_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/name_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/name_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/name_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/person_status_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/person_status_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/person_status_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/person_status_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/person_status_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/person_status_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/position_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/position_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/position_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/position_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/position_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/position_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/relationships.py` & `sayari-0.0.76/src/sayari/generated_types/types/relationships.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/risk.py` & `sayari-0.0.76/src/sayari/generated_types/types/risk.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/risk_intelligence_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/risk_intelligence_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/shares_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/shares_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/shares_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/shares_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/shares_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/shares_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/status_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/status_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/status_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/status_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/status_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/status_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/tag.py` & `sayari-0.0.76/src/sayari/generated_types/types/tag.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/translated_name_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/translated_name_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/translated_name_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/translated_name_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/translated_name_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/translated_name_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_data.py` & `sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_info.py` & `sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_properties.py` & `sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_properties.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/generated_types/types/weak_identifier_type.py` & `sayari-0.0.76/src/sayari/generated_types/types/weak_identifier_type.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/info/client.py` & `sayari-0.0.76/src/sayari/info/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,17 @@
 
             - to: typing.Optional[dt.date]. An ISO 8601 encoded date string indicating the ending time period to obtain usage stats. In the format YYYY-MM-DD
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.info.get_usage(
             from_=datetime.date.fromisoformat(
                 "2023-01-15",
             ),
@@ -138,18 +137,17 @@
 
             - token: typing.Optional[str]. Pagination token to retrieve the next page of results
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.info.get_history(
             events="string",
             from_=datetime.date.fromisoformat(
                 "2023-01-15",
@@ -234,18 +232,17 @@
 
             - to: typing.Optional[dt.date]. An ISO 8601 encoded date string indicating the ending time period to obtain usage stats. In the format YYYY-MM-DD
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.info.get_usage(
             from_=datetime.date.fromisoformat(
                 "2023-01-15",
             ),
@@ -328,18 +325,17 @@
 
             - token: typing.Optional[str]. Pagination token to retrieve the next page of results
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         import datetime
 
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.info.get_history(
             events="string",
             from_=datetime.date.fromisoformat(
                 "2023-01-15",
```

### Comparing `sayari-0.0.75/src/sayari/info/types/history_info.py` & `sayari-0.0.76/src/sayari/info/types/history_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/info/types/history_response.py` & `sayari-0.0.76/src/sayari/info/types/history_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/info/types/usage_info.py` & `sayari-0.0.76/src/sayari/info/types/usage_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/info/types/usage_response.py` & `sayari-0.0.76/src/sayari/info/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/__init__.py` & `sayari-0.0.76/src/sayari/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/client.py` & `sayari-0.0.76/src/sayari/notifications/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,18 +50,17 @@
 
             - limit: typing.Optional[int]. Limit total notifications in the response. Defaults to 100.
 
             - offset: typing.Optional[int]. Offset which notifications are returned. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.notifications.project_notifications(
             id="0oZnoG",
             limit=20,
         )
@@ -140,18 +139,17 @@
 
             - limit: typing.Optional[int]. Limit total notifications in the response. Defaults to 100.
 
             - offset: typing.Optional[int]. Offset which notifications are returned. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.notifications.resource_notifications(
             id="03ePyj",
             limit=20,
         )
@@ -235,18 +233,17 @@
 
             - limit: typing.Optional[int]. Limit total notifications in the response. Defaults to 100.
 
             - offset: typing.Optional[int]. Offset which notifications are returned. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.notifications.project_notifications(
             id="0oZnoG",
             limit=20,
         )
@@ -325,18 +322,17 @@
 
             - limit: typing.Optional[int]. Limit total notifications in the response. Defaults to 100.
 
             - offset: typing.Optional[int]. Offset which notifications are returned. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.notifications.resource_notifications(
             id="03ePyj",
             limit=20,
         )
```

### Comparing `sayari-0.0.75/src/sayari/notifications/types/__init__.py` & `sayari-0.0.76/src/sayari/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/notification.py` & `sayari-0.0.76/src/sayari/notifications/types/notification.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/notification_additional_information.py` & `sayari-0.0.76/src/sayari/notifications/types/notification_additional_information.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/project_notification_data.py` & `sayari-0.0.76/src/sayari/notifications/types/project_notification_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/project_notifications_response.py` & `sayari-0.0.76/src/sayari/notifications/types/project_notifications_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/resource_notification_data.py` & `sayari-0.0.76/src/sayari/notifications/types/resource_notification_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/notifications/types/resource_notifications_response.py` & `sayari-0.0.76/src/sayari/notifications/types/resource_notifications_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/__init__.py` & `sayari-0.0.76/src/sayari/project/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/client.py` & `sayari-0.0.76/src/sayari/project/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,18 +50,17 @@
 
         Parameters:
             - request: CreateProjectRequest.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import CreateProjectRequest
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.project.create_project(
             request=CreateProjectRequest(
                 label="Project Alpha",
             ),
@@ -134,18 +133,17 @@
 
             - limit: typing.Optional[int]. Limit total values returned for projects. Defaults to 100. Max 100.
 
             - archived: typing.Optional[bool]. Toggle between projects that have been archived (true) or not (false). Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.project.get_projects(
             archived=False,
             limit=8,
         )
@@ -255,18 +253,17 @@
 
             - aggregations: typing.Optional[typing.Union[ProjectEntitiesAggsDefinition, typing.Sequence[ProjectEntitiesAggsDefinition]]]. Aggregations for entities in a project.
 
             - accept: GetProjectEntitiesAcceptHeader. The response format. Defaults to application/json.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.project.get_project_entities(
             id="gPq6EY",
             accept="application/json",
         )
@@ -349,18 +346,17 @@
 
         Parameters:
             - request: CreateProjectRequest.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import CreateProjectRequest
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.project.create_project(
             request=CreateProjectRequest(
                 label="Project Alpha",
             ),
@@ -433,18 +429,17 @@
 
             - limit: typing.Optional[int]. Limit total values returned for projects. Defaults to 100. Max 100.
 
             - archived: typing.Optional[bool]. Toggle between projects that have been archived (true) or not (false). Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.project.get_projects(
             archived=False,
             limit=8,
         )
@@ -554,18 +549,17 @@
 
             - aggregations: typing.Optional[typing.Union[ProjectEntitiesAggsDefinition, typing.Sequence[ProjectEntitiesAggsDefinition]]]. Aggregations for entities in a project.
 
             - accept: GetProjectEntitiesAcceptHeader. The response format. Defaults to application/json.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.project.get_project_entities(
             id="gPq6EY",
             accept="application/json",
         )
```

### Comparing `sayari-0.0.75/src/sayari/project/types/__init__.py` & `sayari-0.0.76/src/sayari/project/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/bucket_agg.py` & `sayari-0.0.76/src/sayari/project/types/bucket_agg.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/create_project_request.py` & `sayari-0.0.76/src/sayari/project/types/create_project_request.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/create_project_response.py` & `sayari-0.0.76/src/sayari/project/types/create_project_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/doc_count.py` & `sayari-0.0.76/src/sayari/project/types/doc_count.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/get_project_entities_response.py` & `sayari-0.0.76/src/sayari/project/types/get_project_entities_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/get_projects_response.py` & `sayari-0.0.76/src/sayari/project/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/hs_code_agg.py` & `sayari-0.0.76/src/sayari/project/types/hs_code_agg.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/hs_code_agg_bucket.py` & `sayari-0.0.76/src/sayari/project/types/hs_code_agg_bucket.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/hs_code_agg_terms.py` & `sayari-0.0.76/src/sayari/project/types/hs_code_agg_terms.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/int_key_value.py` & `sayari-0.0.76/src/sayari/project/types/int_key_value.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project.py` & `sayari-0.0.76/src/sayari/project/types/project.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project_counts.py` & `sayari-0.0.76/src/sayari/project/types/project_counts.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project_entities_aggs.py` & `sayari-0.0.76/src/sayari/project/types/project_entities_aggs.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project_entity.py` & `sayari-0.0.76/src/sayari/project/types/project_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project_entity_upstream.py` & `sayari-0.0.76/src/sayari/project/types/project_entity_upstream.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/project_with_members.py` & `sayari-0.0.76/src/sayari/project/types/project_with_members.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/psa_summary.py` & `sayari-0.0.76/src/sayari/project/types/psa_summary.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/role_member.py` & `sayari-0.0.76/src/sayari/project/types/role_member.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/project/types/sort_field.py` & `sayari-0.0.76/src/sayari/project/types/sort_field.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/record/client.py` & `sayari-0.0.76/src/sayari/record/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,17 @@
 
             - references_limit: typing.Optional[int]. A limit on the number of references to be returned. Defaults to 100.
 
             - references_offset: typing.Optional[int]. Number of references to skip before returning response. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.record.get_record(
             id="74cf0fc2a62f9c8f4e88f8a0b3ffcca4%2FF0000110%2F1682970471254",
         )
         """
@@ -133,18 +132,17 @@
 
             - references_limit: typing.Optional[int]. A limit on the number of references to be returned. Defaults to 100.
 
             - references_offset: typing.Optional[int]. Number of references to skip before returning response. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.record.get_record(
             id="74cf0fc2a62f9c8f4e88f8a0b3ffcca4%2FF0000110%2F1682970471254",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/record/types/get_record_response.py` & `sayari-0.0.76/src/sayari/record/types/get_record_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/record/types/record_references.py` & `sayari-0.0.76/src/sayari/record/types/record_references.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resolution/client.py` & `sayari-0.0.76/src/sayari/resolution/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,17 @@
 
             - contact: typing.Optional[typing.Union[str, typing.Sequence[str]]]. Entity contact
 
             - type: typing.Optional[typing.Union[Entities, typing.Sequence[Entities]]]. [Entity type](/sayari-library/ontology/entities). If multiple values are passed for any field, the endpoint will match entities with ANY of the values.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.resolution.resolution(
             name="victoria beckham limited",
         )
         """
@@ -165,18 +164,17 @@
 
             - contact: typing.Optional[typing.Union[str, typing.Sequence[str]]]. Entity contact
 
             - type: typing.Optional[typing.Union[Entities, typing.Sequence[Entities]]]. [Entity type](/sayari-library/ontology/entities). If multiple values are passed for any field, the endpoint will match entities with ANY of the values.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.resolution.resolution(
             name="victoria beckham limited",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/resolution/types/match_explanation.py` & `sayari-0.0.76/src/sayari/resolution/types/match_explanation.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resolution/types/resolution_response.py` & `sayari-0.0.76/src/sayari/resolution/types/resolution_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resolution/types/resolution_response_fields.py` & `sayari-0.0.76/src/sayari/resolution/types/resolution_response_fields.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resolution/types/resolution_result.py` & `sayari-0.0.76/src/sayari/resolution/types/resolution_result.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resource/client.py` & `sayari-0.0.76/src/sayari/resource/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 
         Parameters:
             - request: SaveEntityRequest.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import SaveEntityRequest
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.resource.save_entity(
             request=SaveEntityRequest(
                 type="entity",
                 project="GNJbkG",
@@ -121,18 +120,17 @@
 
         Parameters:
             - request: SaveEntityRequest.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from sayari import SaveEntityRequest
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.resource.save_entity(
             request=SaveEntityRequest(
                 type="entity",
                 project="GNJbkG",
```

### Comparing `sayari-0.0.75/src/sayari/resource/types/save_entity_request.py` & `sayari-0.0.76/src/sayari/resource/types/save_entity_request.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resource/types/save_entity_response.py` & `sayari-0.0.76/src/sayari/resource/types/save_entity_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/resource/types/save_entity_response_data.py` & `sayari-0.0.76/src/sayari/resource/types/save_entity_response_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/search/client.py` & `sayari-0.0.76/src/sayari/search/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,17 @@
 
             - geo_facets: typing.Optional[bool]. Whether or not to return search geo bound facets in results giving counts by geo tile. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.search.search_entity(
             limit=1,
             q="victoria beckham limited",
         )
@@ -179,18 +178,17 @@
 
             - geo_facets: typing.Optional[bool]. Whether or not to return search geo bound facets in results giving counts by geo tile. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.search.search_entity_get(
             limit=1,
             q="victoria beckham limited",
         )
@@ -280,18 +278,17 @@
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.search.search_record(
             limit=1,
             q="victoria beckham limited",
         )
@@ -388,18 +385,17 @@
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.search.search_record_get(
             q="victoria beckham limited",
             limit=1,
         )
@@ -496,18 +492,17 @@
 
             - geo_facets: typing.Optional[bool]. Whether or not to return search geo bound facets in results giving counts by geo tile. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.search.search_entity(
             limit=1,
             q="victoria beckham limited",
         )
@@ -609,18 +604,17 @@
 
             - geo_facets: typing.Optional[bool]. Whether or not to return search geo bound facets in results giving counts by geo tile. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.search.search_entity_get(
             limit=1,
             q="victoria beckham limited",
         )
@@ -710,18 +704,17 @@
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.search.search_record(
             limit=1,
             q="victoria beckham limited",
         )
@@ -818,18 +811,17 @@
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - advanced: typing.Optional[bool]. Set to true to enable full elasticsearch query string syntax which allows for fielded search and more complex operators. Note that the syntax is more strict and can result in empty result-sets. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.search.search_record_get(
             q="victoria beckham limited",
             limit=1,
         )
```

### Comparing `sayari-0.0.75/src/sayari/search/types/coordinates.py` & `sayari-0.0.76/src/sayari/search/types/coordinates.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/search/types/entity_search_response.py` & `sayari-0.0.76/src/sayari/search/types/entity_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/search/types/filter_list.py` & `sayari-0.0.76/src/sayari/search/types/filter_list.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/search/types/record_search_response.py` & `sayari-0.0.76/src/sayari/search/types/record_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/search/types/search_results.py` & `sayari-0.0.76/src/sayari/search/types/search_results.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/__init__.py` & `sayari-0.0.76/src/sayari/shared_errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/errors/__init__.py` & `sayari-0.0.76/src/sayari/shared_errors/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/types/__init__.py` & `sayari-0.0.76/src/sayari/shared_errors/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/types/method_not_allowed_response.py` & `sayari-0.0.76/src/sayari/shared_errors/types/method_not_allowed_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/types/not_acceptable_response.py` & `sayari-0.0.76/src/sayari/shared_errors/types/not_acceptable_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_errors/types/not_found_response.py` & `sayari-0.0.76/src/sayari/shared_errors/types/not_found_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/__init__.py` & `sayari-0.0.76/src/sayari/shared_types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/__init__.py` & `sayari-0.0.76/src/sayari/shared_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/coordinate.py` & `sayari-0.0.76/src/sayari/shared_types/types/coordinate.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/core_entity.py` & `sayari-0.0.76/src/sayari/shared_types/types/core_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/embedded_entity.py` & `sayari-0.0.76/src/sayari/shared_types/types/embedded_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/entity_details.py` & `sayari-0.0.76/src/sayari/shared_types/types/entity_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/entity_relationships.py` & `sayari-0.0.76/src/sayari/shared_types/types/entity_relationships.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/entity_summary.py` & `sayari-0.0.76/src/sayari/shared_types/types/entity_summary.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/identifier.py` & `sayari-0.0.76/src/sayari/shared_types/types/identifier.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as.py` & `sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_data.py` & `sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/possibly_same_as_match.py` & `sayari-0.0.76/src/sayari/shared_types/types/possibly_same_as_match.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/psa.py` & `sayari-0.0.76/src/sayari/shared_types/types/psa.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/psa_entity.py` & `sayari-0.0.76/src/sayari/shared_types/types/psa_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/psa_match_keys.py` & `sayari-0.0.76/src/sayari/shared_types/types/psa_match_keys.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/record_details.py` & `sayari-0.0.76/src/sayari/shared_types/types/record_details.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/referenced_by.py` & `sayari-0.0.76/src/sayari/shared_types/types/referenced_by.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/referenced_by_data.py` & `sayari-0.0.76/src/sayari/shared_types/types/referenced_by_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/relationship_data.py` & `sayari-0.0.76/src/sayari/shared_types/types/relationship_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/relationship_info.py` & `sayari-0.0.76/src/sayari/shared_types/types/relationship_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/risk_data.py` & `sayari-0.0.76/src/sayari/shared_types/types/risk_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/source_count_info.py` & `sayari-0.0.76/src/sayari/shared_types/types/source_count_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/shared_types/types/status.py` & `sayari-0.0.76/src/sayari/shared_types/types/status.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/source/client.py` & `sayari-0.0.76/src/sayari/source/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,17 @@
         Parameters:
             - limit: typing.Optional[int]. A limit on the number of objects to be returned with a range between 1 and 100. Defaults to 100.
 
             - offset: typing.Optional[int]. Number of results to skip before returning response. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.source.list_sources(
             limit=2,
         )
         """
@@ -113,18 +112,17 @@
         Returns metadata for a source that Sayari collects data from
 
         Parameters:
             - id: str. The unique identifier for a source in the database
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.source.get_source(
             id="f4396e4b8a41d1fd9f09ea94d2ebedb9",
         )
         """
@@ -188,18 +186,17 @@
         Parameters:
             - limit: typing.Optional[int]. A limit on the number of objects to be returned with a range between 1 and 100. Defaults to 100.
 
             - offset: typing.Optional[int]. Number of results to skip before returning response. Defaults to 0.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.source.list_sources(
             limit=2,
         )
         """
@@ -260,18 +257,17 @@
         Returns metadata for a source that Sayari collects data from
 
         Parameters:
             - id: str. The unique identifier for a source in the database
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.source.get_source(
             id="f4396e4b8a41d1fd9f09ea94d2ebedb9",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/source/types/get_source_response.py` & `sayari-0.0.76/src/sayari/source/types/get_source_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/source/types/list_sources_response.py` & `sayari-0.0.76/src/sayari/source/types/list_sources_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/source/types/source.py` & `sayari-0.0.76/src/sayari/source/types/source.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/__init__.py` & `sayari-0.0.76/src/sayari/trade/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/client.py` & `sayari-0.0.76/src/sayari/trade/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.trade.search_shipments(
             limit=1,
             q="rum",
         )
@@ -154,18 +153,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.trade.search_suppliers(
             limit=1,
             q="rum",
         )
@@ -253,18 +251,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.trade.search_buyers(
             limit=1,
             q="rum",
         )
@@ -357,18 +354,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.trade.search_shipments(
             limit=1,
             q="rum",
         )
@@ -456,18 +452,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.trade.search_suppliers(
             limit=1,
             q="rum",
         )
@@ -555,18 +550,17 @@
 
             - filter: typing.Optional[TradeFilterList]. Filters to be applied to search query to limit the result-set.
 
             - facets: typing.Optional[bool]. Whether or not to return search facets in results giving counts by field. Defaults to false.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.trade.search_buyers(
             limit=1,
             q="rum",
         )
```

### Comparing `sayari-0.0.75/src/sayari/trade/types/__init__.py` & `sayari-0.0.76/src/sayari/trade/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/business_purpose.py` & `sayari-0.0.76/src/sayari/trade/types/business_purpose.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/buyer_search_response.py` & `sayari-0.0.76/src/sayari/trade/types/buyer_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/data_source.py` & `sayari-0.0.76/src/sayari/trade/types/data_source.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/hs_code.py` & `sayari-0.0.76/src/sayari/trade/types/hs_code.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/hs_code_info.py` & `sayari-0.0.76/src/sayari/trade/types/hs_code_info.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/monetary_value.py` & `sayari-0.0.76/src/sayari/trade/types/monetary_value.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment.py` & `sayari-0.0.76/src/sayari/trade/types/shipment.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment_address.py` & `sayari-0.0.76/src/sayari/trade/types/shipment_address.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment_country.py` & `sayari-0.0.76/src/sayari/trade/types/shipment_country.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment_identifier.py` & `sayari-0.0.76/src/sayari/trade/types/shipment_identifier.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment_metadata.py` & `sayari-0.0.76/src/sayari/trade/types/shipment_metadata.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/shipment_search_response.py` & `sayari-0.0.76/src/sayari/trade/types/shipment_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/source_or_destination_entity.py` & `sayari-0.0.76/src/sayari/trade/types/source_or_destination_entity.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/supplier_metadata.py` & `sayari-0.0.76/src/sayari/trade/types/supplier_metadata.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/supplier_or_buyer.py` & `sayari-0.0.76/src/sayari/trade/types/supplier_or_buyer.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/supplier_search_response.py` & `sayari-0.0.76/src/sayari/trade/types/supplier_search_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/trade_filter_list.py` & `sayari-0.0.76/src/sayari/trade/types/trade_filter_list.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/trade/types/weight.py` & `sayari-0.0.76/src/sayari/trade/types/weight.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/client.py` & `sayari-0.0.76/src/sayari/traversal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,18 +128,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.traversal.traversal(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -316,18 +315,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.traversal.ubo(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -504,18 +502,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.traversal.ownership(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -694,18 +691,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.traversal.watchlist(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -801,18 +797,17 @@
         The Shortest Path endpoint returns a response identifying the shortest traversal path connecting each pair of entities.
 
         Parameters:
             - entities: typing.Union[str, typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import Client
+        from sayari.client import Sayari
 
-        client = Client(
-            client_name="YOUR_CLIENT_NAME",
+        client = Sayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         client.traversal.shortest_path(
             entities="string",
         )
         """
@@ -967,18 +962,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.traversal.traversal(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -1155,18 +1149,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.traversal.ubo(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -1343,18 +1336,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.traversal.ownership(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -1533,18 +1525,17 @@
 
             - law_enforcement_action: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - xinjiang_geospatial: typing.Optional[bool]. Filter paths to only those that entity with an entity that we have flagged with this risk factor
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.traversal.watchlist(
             id="mGq1lpuqKssNWTjIokuPeA",
             limit=1,
         )
@@ -1640,18 +1631,17 @@
         The Shortest Path endpoint returns a response identifying the shortest traversal path connecting each pair of entities.
 
         Parameters:
             - entities: typing.Union[str, typing.Sequence[str]].
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
-        from sayari.client import AsyncClient
+        from sayari.client import AsyncSayari
 
-        client = AsyncClient(
-            client_name="YOUR_CLIENT_NAME",
+        client = AsyncSayari(
             client_id="YOUR_CLIENT_ID",
             client_secret="YOUR_CLIENT_SECRET",
         )
         await client.traversal.shortest_path(
             entities="string",
         )
         """
```

### Comparing `sayari-0.0.75/src/sayari/traversal/types/__init__.py` & `sayari-0.0.76/src/sayari/traversal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/shortest_path_data.py` & `sayari-0.0.76/src/sayari/traversal/types/shortest_path_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/shortest_path_response.py` & `sayari-0.0.76/src/sayari/traversal/types/shortest_path_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/traversal_data.py` & `sayari-0.0.76/src/sayari/traversal/types/traversal_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/traversal_path.py` & `sayari-0.0.76/src/sayari/traversal/types/traversal_path.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/traversal_relationship_data.py` & `sayari-0.0.76/src/sayari/traversal/types/traversal_relationship_data.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/src/sayari/traversal/types/traversal_response.py` & `sayari-0.0.76/src/sayari/traversal/types/traversal_response.py`

 * *Files identical despite different names*

### Comparing `sayari-0.0.75/PKG-INFO` & `sayari-0.0.76/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayari
-Version: 0.0.75
+Version: 0.0.76
 Summary: A Python SDK for Sayari
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,30 +29,30 @@
 ```
 <!-- End Installation  -->
 
 <!-- Begin Usage, generated by Fern  -->
 # Usage
 
 ```python
-from sayari.client import Client
+from sayari.client import Sayari
 
-client = Client(
+client = Sayari(
     client_id="YOUR_CLIENT_ID",
     client_secret="YOUR_CLIENT_SECRET",
 )
 ```
 <!-- End Usage  -->
 
 <!-- Begin Async Usage, generated by Fern  -->
 # Async Client
 
 ```python
-from sayari.client import AsyncClient
+from sayari.client import AsyncSayari
 
-client = AsyncClient(
+client = AsyncSayari(
     client_id="YOUR_CLIENT_ID",
     client_secret="YOUR_CLIENT_SECRET",
 )
 ```
 <!-- End Async Usage  -->
 
 <!-- Begin Status, generated by Fern  -->
```

