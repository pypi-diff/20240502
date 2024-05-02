# Comparing `tmp/patent_client-5.0.0.tar.gz` & `tmp/patent_client-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patent_client-5.0.0.tar", max compression
+gzip compressed data, was "patent_client-5.0.1.tar", max compression
```

## Comparing `patent_client-5.0.0.tar` & `patent_client-5.0.1.tar`

### file list

```diff
@@ -1,409 +1,408 @@
--rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.0/LICENSE
--rw-r--r--   0        0        0     6104 2024-04-25 19:50:46.499667 patent_client-5.0.0/README.md
--rw-r--r--   0        0        0     1708 2024-04-25 19:50:46.516333 patent_client-5.0.0/patent_client/__init__.py
--rw-r--r--   0        0        0      839 2024-04-25 19:50:46.516665 patent_client-5.0.0/patent_client/_async/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.0/patent_client/_async/epo/__init__.py
--rw-r--r--   0        0        0      214 2024-04-25 19:50:46.517020 patent_client-5.0.0/patent_client/_async/epo/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.0/patent_client/_async/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      386 2024-04-25 19:50:46.517267 patent_client-5.0.0/patent_client/_async/epo/ops/family/api.py
--rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.0/patent_client/_async/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      378 2024-04-25 19:50:46.518752 patent_client-5.0.0/patent_client/_async/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1119 2024-04-25 19:50:46.519067 patent_client-5.0.0/patent_client/_async/epo/ops/family/model.py
--rw-r--r--   0        0        0      519 2024-04-25 19:50:46.519341 patent_client-5.0.0/patent_client/_async/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1545 2024-04-25 19:50:46.519652 patent_client-5.0.0/patent_client/_async/epo/ops/family/schema.py
--rw-r--r--   0        0        0      527 2024-04-25 19:50:46.520362 patent_client-5.0.0/patent_client/_async/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.0/patent_client/_async/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      361 2024-04-25 19:50:46.520529 patent_client-5.0.0/patent_client/_async/epo/ops/legal/api.py
--rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.0/patent_client/_async/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0      489 2024-04-25 19:50:46.528737 patent_client-5.0.0/patent_client/_async/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2375 2024-04-25 19:50:46.528871 patent_client-5.0.0/patent_client/_async/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5399 2024-04-25 19:50:46.529038 patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4062 2024-04-25 19:50:46.529393 patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1216 2024-04-25 19:50:46.529507 patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.0/patent_client/_async/epo/ops/legal/util.py
--rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1417 2024-04-25 19:50:46.529887 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     1806 2024-04-25 19:50:46.530201 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1117 2024-04-25 19:50:46.530931 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0      763 2024-04-25 19:50:46.531354 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/model.py
--rw-r--r--   0        0        0      952 2024-04-25 19:50:46.531484 patent_client-5.0.0/patent_client/_async/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.0/patent_client/_async/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5650 2024-04-25 19:50:46.531713 patent_client-5.0.0/patent_client/_async/epo/ops/published/api.py
--rw-r--r--   0        0        0     2849 2024-04-25 19:50:46.531966 patent_client-5.0.0/patent_client/_async/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.0/patent_client/_async/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6195 2024-04-25 19:50:46.535765 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.536077 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18516 2024-04-25 19:50:46.536175 patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3261 2024-04-25 19:50:46.536305 patent_client-5.0.0/patent_client/_async/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2212 2024-04-25 19:50:46.536541 patent_client-5.0.0/patent_client/_async/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      321 2024-04-25 19:50:46.536782 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     2754 2024-04-25 19:50:46.536911 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1050 2024-04-25 19:50:46.537030 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2084 2024-04-25 19:50:46.537277 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/images.py
--rw-r--r--   0        0        0      843 2024-04-25 19:50:46.537418 patent_client-5.0.0/patent_client/_async/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      285 2024-04-25 19:50:46.537840 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     3962 2024-04-25 19:50:46.538098 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0      874 2024-04-25 19:50:46.538325 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     1668 2024-04-25 19:50:46.538535 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3193 2024-04-25 19:50:46.539173 patent_client-5.0.0/patent_client/_async/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-04-25 19:50:46.539913 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-04-25 19:50:46.540088 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.0/patent_client/_async/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3482 2024-04-25 19:50:46.541813 patent_client-5.0.0/patent_client/_async/epo/ops/session.py
--rw-r--r--   0        0        0     2741 2024-04-25 19:50:46.541992 patent_client-5.0.0/patent_client/_async/epo/ops/util.py
--rw-r--r--   0        0        0     3230 2024-04-25 19:50:46.542440 patent_client-5.0.0/patent_client/_async/http_client.py
--rw-r--r--   0        0        0      202 2024-04-25 19:50:46.542670 patent_client-5.0.0/patent_client/_async/odp.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.0/patent_client/_async/uspto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.0/patent_client/_async/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-25 19:50:46.542893 patent_client-5.0.0/patent_client/_async/uspto/assignment/api.py
--rw-r--r--   0        0        0      934 2024-04-25 19:50:46.543014 patent_client-5.0.0/patent_client/_async/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     3633 2024-04-25 19:50:46.559627 patent_client-5.0.0/patent_client/_async/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.0/patent_client/_async/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3445 2024-04-25 19:50:46.562396 patent_client-5.0.0/patent_client/_async/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4202 2024-04-25 19:50:46.562667 patent_client-5.0.0/patent_client/_async/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5466 2024-04-25 19:50:46.562938 patent_client-5.0.0/patent_client/_async/uspto/assignment/model.py
--rw-r--r--   0        0        0     1932 2024-04-25 19:50:46.563119 patent_client-5.0.0/patent_client/_async/uspto/assignment/model_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3208 2024-04-25 19:50:46.563555 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1100 2024-04-25 19:50:46.563680 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     2781 2024-04-25 19:50:46.566025 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1707 2024-04-25 19:50:46.566134 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1558 2024-04-25 19:50:46.566440 patent_client-5.0.0/patent_client/_async/uspto/bulk_data/model.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-25 19:50:46.566609 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1143 2024-04-25 19:50:46.566720 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     1902 2024-04-25 19:50:46.606761 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7111 2024-04-25 19:50:46.610118 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3738 2024-04-25 19:50:46.611808 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6063 2024-04-25 19:50:46.613527 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5252 2024-04-25 19:50:46.613926 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0        1 2024-04-25 19:50:46.614640 patent_client-5.0.0/patent_client/_async/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5524 2024-04-25 19:50:46.615019 patent_client-5.0.0/patent_client/_async/uspto/odp/api.py
--rw-r--r--   0        0        0     2834 2024-04-25 19:50:46.615152 patent_client-5.0.0/patent_client/_async/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     4863 2024-04-25 19:50:46.624619 patent_client-5.0.0/patent_client/_async/uspto/odp/manager.py
--rw-r--r--   0        0        0     1895 2024-04-25 19:50:46.624873 patent_client-5.0.0/patent_client/_async/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    16311 2024-04-25 19:50:46.625251 patent_client-5.0.0/patent_client/_async/uspto/odp/model.py
--rw-r--r--   0        0        0    12253 2024-04-25 19:50:46.625468 patent_client-5.0.0/patent_client/_async/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2396 2024-04-25 19:50:46.625599 patent_client-5.0.0/patent_client/_async/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.0/patent_client/_async/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      475 2024-04-25 19:50:46.628424 patent_client-5.0.0/patent_client/_async/uspto/odp/util.py
--rw-r--r--   0        0        0      132 2024-04-25 19:50:46.628549 patent_client-5.0.0/patent_client/_async/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4501 2024-04-25 19:50:46.628716 patent_client-5.0.0/patent_client/_async/uspto/peds/api.py
--rw-r--r--   0        0        0      711 2024-04-25 19:50:46.629004 patent_client-5.0.0/patent_client/_async/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0    18324 2024-04-25 19:50:46.659745 patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8360 2024-04-25 19:50:46.659927 patent_client-5.0.0/patent_client/_async/uspto/peds/manager.py
--rw-r--r--   0        0        0     9792 2024-04-25 19:50:46.660088 patent_client-5.0.0/patent_client/_async/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    16990 2024-04-25 19:50:46.664359 patent_client-5.0.0/patent_client/_async/uspto/peds/model.py
--rw-r--r--   0        0        0     6116 2024-04-25 19:50:46.664816 patent_client-5.0.0/patent_client/_async/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.0/patent_client/_async/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      149 2024-04-25 19:50:46.665140 patent_client-5.0.0/patent_client/_async/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10200 2024-04-25 19:50:46.665671 patent_client-5.0.0/patent_client/_async/uspto/ptab/api.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.0/patent_client/_async/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2085 2024-04-25 19:50:46.669191 patent_client-5.0.0/patent_client/_async/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2311 2024-04-25 19:50:46.669333 patent_client-5.0.0/patent_client/_async/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8117 2024-04-25 19:50:46.669591 patent_client-5.0.0/patent_client/_async/uspto/ptab/model.py
--rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.0/patent_client/_async/uspto/ptab/util.py
--rw-r--r--   0        0        0      161 2024-04-25 19:50:46.669818 patent_client-5.0.0/patent_client/_async/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6700 2024-04-25 19:50:46.670036 patent_client-5.0.0/patent_client/_async/uspto/public_search/api.py
--rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.0/patent_client/_async/uspto/public_search/api_test.py
--rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2066 2024-04-25 19:50:46.694995 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     6678 2024-04-25 19:50:46.698061 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     1594 2024-04-25 19:50:46.698401 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1035 2024-04-25 19:50:46.698472 patent_client-5.0.0/patent_client/_async/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.0/patent_client/_async/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-04-25 19:50:46.706321 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4144 2024-04-25 19:50:46.712656 patent_client-5.0.0/patent_client/_async/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7743 2024-04-25 19:50:46.716625 patent_client-5.0.0/patent_client/_async/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      330 2024-04-25 19:50:46.716790 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-25 19:50:46.716934 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7574 2024-04-25 19:50:46.717130 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2249 2024-04-25 19:50:46.719323 patent_client-5.0.0/patent_client/_async/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1537 2024-04-25 19:50:46.719456 patent_client-5.0.0/patent_client/_async/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4520 2024-04-25 19:50:46.722417 patent_client-5.0.0/patent_client/_async/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.0/patent_client/_async/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4313 2024-04-25 19:50:46.722791 patent_client-5.0.0/patent_client/_async/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.0/patent_client/_async/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.0/patent_client/_async/uspto/public_search/util.py
--rw-r--r--   0        0        0     1255 2024-04-25 19:50:46.723166 patent_client-5.0.0/patent_client/_sync/__init__.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.723379 patent_client-5.0.0/patent_client/_sync/epo/__init__.py
--rw-r--r--   0        0        0      630 2024-04-25 19:50:46.723511 patent_client-5.0.0/patent_client/_sync/epo/ops/__init__.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.723823 patent_client-5.0.0/patent_client/_sync/epo/ops/family/__init__.py
--rw-r--r--   0        0        0      790 2024-04-25 19:50:46.724222 patent_client-5.0.0/patent_client/_sync/epo/ops/family/api.py
--rw-r--r--   0        0        0      855 2024-04-25 19:50:46.724547 patent_client-5.0.0/patent_client/_sync/epo/ops/family/api_test.py
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.725140 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
--rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.725251 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
--rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.725360 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
--rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.725470 patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
--rw-r--r--   0        0        0      772 2024-04-25 19:50:46.725581 patent_client-5.0.0/patent_client/_sync/epo/ops/family/manager.py
--rw-r--r--   0        0        0     1535 2024-04-25 19:50:46.725776 patent_client-5.0.0/patent_client/_sync/epo/ops/family/model.py
--rw-r--r--   0        0        0      903 2024-04-25 19:50:46.725892 patent_client-5.0.0/patent_client/_sync/epo/ops/family/model_test.py
--rw-r--r--   0        0        0     1961 2024-04-25 19:50:46.725998 patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema.py
--rw-r--r--   0        0        0      943 2024-04-25 19:50:46.726102 patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema_test.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.726325 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/__init__.py
--rw-r--r--   0        0        0      765 2024-04-25 19:50:46.726444 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/api.py
--rw-r--r--   0        0        0      704 2024-04-25 19:50:46.726566 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/api_test.py
--rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.731050 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
--rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.731151 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
--rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.731269 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
--rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.731525 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
--rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.731642 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
--rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.731778 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
--rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.732730 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
--rw-r--r--   0        0        0   291881 2024-04-25 19:50:46.733722 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/legal_code_descriptions_2023-44-0.xlsx
--rw-r--r--   0        0        0      883 2024-04-25 19:50:46.733910 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/manager.py
--rw-r--r--   0        0        0     2791 2024-04-25 19:50:46.735502 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/model.py
--rw-r--r--   0        0        0     5753 2024-04-25 19:50:46.735838 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes.py
--rw-r--r--   0        0        0      882 2024-04-25 19:50:46.735986 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes_test.py
--rw-r--r--   0        0        0     4478 2024-04-25 19:50:46.736419 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema.py
--rw-r--r--   0        0        0     1632 2024-04-25 19:50:46.736570 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema_test.py
--rw-r--r--   0        0        0      530 2024-04-25 19:50:46.736711 patent_client-5.0.0/patent_client/_sync/epo/ops/legal/util.py
--rw-r--r--   0        0        0      483 2024-04-25 19:50:46.736849 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-25 19:50:46.736982 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api.py
--rw-r--r--   0        0        0     2062 2024-04-25 19:50:46.737103 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api_test.py
--rw-r--r--   0        0        0     1533 2024-04-25 19:50:46.738134 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.py
--rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.738251 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.txt
--rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.738313 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/messages.txt
--rw-r--r--   0        0        0     1179 2024-04-25 19:50:46.738445 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/model.py
--rw-r--r--   0        0        0     1368 2024-04-25 19:50:46.738569 patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/schema.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.738708 patent_client-5.0.0/patent_client/_sync/epo/ops/published/__init__.py
--rw-r--r--   0        0        0     5934 2024-04-25 19:50:46.739051 patent_client-5.0.0/patent_client/_sync/epo/ops/published/api.py
--rw-r--r--   0        0        0     3073 2024-04-25 19:50:46.739287 patent_client-5.0.0/patent_client/_sync/epo/ops/published/api_test.py
--rw-r--r--   0        0        0     1917 2024-04-25 19:50:46.750057 patent_client-5.0.0/patent_client/_sync/epo/ops/published/cql.py
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.750171 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0     6174 2024-04-25 19:50:46.750486 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
--rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.750620 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
--rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.750740 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
--rw-r--r--   0        0        0    20102 2024-04-25 19:50:46.750995 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0    18510 2024-04-25 19:50:46.751449 patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
--rw-r--r--   0        0        0     3551 2024-04-25 19:50:46.751824 patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager.py
--rw-r--r--   0        0        0     2286 2024-04-25 19:50:46.752196 patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager_test.py
--rw-r--r--   0        0        0      737 2024-04-25 19:50:46.752406 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/__init__.py
--rw-r--r--   0        0        0     3170 2024-04-25 19:50:46.753562 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/biblio.py
--rw-r--r--   0        0        0     1466 2024-04-25 19:50:46.753818 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/fulltext.py
--rw-r--r--   0        0        0     2500 2024-04-25 19:50:46.754620 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/images.py
--rw-r--r--   0        0        0     1259 2024-04-25 19:50:46.755053 patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/search.py
--rw-r--r--   0        0        0      701 2024-04-25 19:50:46.755310 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/__init__.py
--rw-r--r--   0        0        0     4378 2024-04-25 19:50:46.756124 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/biblio.py
--rw-r--r--   0        0        0     1290 2024-04-25 19:50:46.756266 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/fulltext.py
--rw-r--r--   0        0        0     2084 2024-04-25 19:50:46.756499 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/images.py
--rw-r--r--   0        0        0     1066 2024-04-25 19:50:46.756981 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/search.py
--rw-r--r--   0        0        0     3609 2024-04-25 19:50:46.757116 patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema_test.py
--rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.757289 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example.xml
--rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.757399 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
--rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.757681 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
--rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.757775 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
--rw-r--r--   0        0        0     7251 2024-04-25 19:50:46.757901 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.json
--rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.757965 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.xml
--rw-r--r--   0        0        0    13020 2024-04-25 19:50:46.758078 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.json
--rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.758194 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
--rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.758423 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/description_example.xml
--rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.758601 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
--rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.758726 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
--rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.758859 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
--rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.758949 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
--rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.759057 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
--rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.759123 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
--rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.759232 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
--rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.759296 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
--rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.759369 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/image_example.json
--rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.759484 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
--rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.759585 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
--rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.759654 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/image_example.xml
--rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.759897 patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/search_example.xml
--rw-r--r--   0        0        0     3876 2024-04-25 19:50:46.760034 patent_client-5.0.0/patent_client/_sync/epo/ops/session.py
--rw-r--r--   0        0        0     3008 2024-04-25 19:50:46.760181 patent_client-5.0.0/patent_client/_sync/epo/ops/util.py
--rw-r--r--   0        0        0     3607 2024-04-25 19:50:46.760452 patent_client-5.0.0/patent_client/_sync/http_client.py
--rw-r--r--   0        0        0      617 2024-04-25 19:50:46.760692 patent_client-5.0.0/patent_client/_sync/odp.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.760938 patent_client-5.0.0/patent_client/_sync/uspto/__init__.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.761073 patent_client-5.0.0/patent_client/_sync/uspto/assignment/__init__.py
--rw-r--r--   0        0        0     2936 2024-04-25 19:50:46.761193 patent_client-5.0.0/patent_client/_sync/uspto/assignment/api.py
--rw-r--r--   0        0        0     1286 2024-04-25 19:50:46.761308 patent_client-5.0.0/patent_client/_sync/uspto/assignment/api_test.py
--rw-r--r--   0        0        0     4049 2024-04-25 19:50:46.771159 patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert.py
--rw-r--r--   0        0        0     1565 2024-04-25 19:50:46.772719 patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert_test.py
--rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.772880 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
--rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.773005 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
--rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.773107 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
--rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.773225 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
--rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.773450 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
--rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.773639 patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
--rw-r--r--   0        0        0     3817 2024-04-25 19:50:46.773871 patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager.py
--rw-r--r--   0        0        0     4308 2024-04-25 19:50:46.774130 patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager_test.py
--rw-r--r--   0        0        0     5870 2024-04-25 19:50:46.774420 patent_client-5.0.0/patent_client/_sync/uspto/assignment/model.py
--rw-r--r--   0        0        0     2348 2024-04-25 19:50:46.774671 patent_client-5.0.0/patent_client/_sync/uspto/assignment/model_test.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.774789 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/__init__.py
--rw-r--r--   0        0        0     3575 2024-04-25 19:50:46.774902 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api.py
--rw-r--r--   0        0        0     1382 2024-04-25 19:50:46.775011 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api_test.py
--rw-r--r--   0        0        0     3113 2024-04-25 19:50:46.776499 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager.py
--rw-r--r--   0        0        0     1963 2024-04-25 19:50:46.776623 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager_test.py
--rw-r--r--   0        0        0     1962 2024-04-25 19:50:46.776743 patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/model.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.776873 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-25 19:50:46.776992 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api.py
--rw-r--r--   0        0        0     1463 2024-04-25 19:50:46.777323 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api_test.py
--rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.819170 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/gd_input.csv
--rw-r--r--   0        0        0     2272 2024-04-25 19:50:46.819397 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/manager.py
--rw-r--r--   0        0        0     7354 2024-04-25 19:50:46.820973 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model.py
--rw-r--r--   0        0        0     3853 2024-04-25 19:50:46.821302 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model_test.py
--rw-r--r--   0        0        0     6479 2024-04-25 19:50:46.822907 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query.py
--rw-r--r--   0        0        0     5668 2024-04-25 19:50:46.823088 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query_test.py
--rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.823233 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app.json
--rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.823291 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app_expected.json
--rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.823387 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list.json
--rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.823499 patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
--rw-r--r--   0        0        0      417 2024-04-25 19:50:46.823618 patent_client-5.0.0/patent_client/_sync/uspto/odp/__init__.py
--rw-r--r--   0        0        0     5822 2024-04-25 19:50:46.823779 patent_client-5.0.0/patent_client/_sync/uspto/odp/api.py
--rw-r--r--   0        0        0     2898 2024-04-25 19:50:46.824087 patent_client-5.0.0/patent_client/_sync/uspto/odp/api_test.py
--rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.830209 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/adjustment.json
--rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.830453 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/application.json
--rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.830552 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/assignment.json
--rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.830776 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/attorney.json
--rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.830907 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/biblio.json
--rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.830994 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/continuity.json
--rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.831136 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/documents.json
--rw-r--r--   0        0        0      317 2024-04-25 19:50:46.831239 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
--rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.831429 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/search.json
--rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.831608 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
--rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.831762 patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/transactions.json
--rw-r--r--   0        0        0     5082 2024-04-25 19:50:46.833233 patent_client-5.0.0/patent_client/_sync/uspto/odp/manager.py
--rw-r--r--   0        0        0     1973 2024-04-25 19:50:46.833456 patent_client-5.0.0/patent_client/_sync/uspto/odp/manager_test.py
--rw-r--r--   0        0        0    15504 2024-04-25 19:50:46.833707 patent_client-5.0.0/patent_client/_sync/uspto/odp/model.py
--rw-r--r--   0        0        0    12669 2024-04-25 19:50:46.834120 patent_client-5.0.0/patent_client/_sync/uspto/odp/model_test.py
--rw-r--r--   0        0        0     2812 2024-04-25 19:50:46.834328 patent_client-5.0.0/patent_client/_sync/uspto/odp/query.py
--rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.834414 patent_client-5.0.0/patent_client/_sync/uspto/odp/query_fields.csv
--rw-r--r--   0        0        0      891 2024-04-25 19:50:46.834544 patent_client-5.0.0/patent_client/_sync/uspto/odp/util.py
--rw-r--r--   0        0        0      548 2024-04-25 19:50:46.834685 patent_client-5.0.0/patent_client/_sync/uspto/peds/__init__.py
--rw-r--r--   0        0        0     4838 2024-04-25 19:50:46.834873 patent_client-5.0.0/patent_client/_sync/uspto/peds/api.py
--rw-r--r--   0        0        0     1031 2024-04-25 19:50:46.835135 patent_client-5.0.0/patent_client/_sync/uspto/peds/api_test.py
--rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.853167 patent_client-5.0.0/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
--rw-r--r--   0        0        0    18324 2024-04-25 19:50:46.853244 patent_client-5.0.0/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
--rw-r--r--   0        0        0     8674 2024-04-25 19:50:46.855392 patent_client-5.0.0/patent_client/_sync/uspto/peds/manager.py
--rw-r--r--   0        0        0     9528 2024-04-25 19:50:46.855604 patent_client-5.0.0/patent_client/_sync/uspto/peds/manager_test.py
--rw-r--r--   0        0        0    17335 2024-04-25 19:50:46.856041 patent_client-5.0.0/patent_client/_sync/uspto/peds/model.py
--rw-r--r--   0        0        0     6532 2024-04-25 19:50:46.856238 patent_client-5.0.0/patent_client/_sync/uspto/peds/query.py
--rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.856357 patent_client-5.0.0/patent_client/_sync/uspto/peds/search_index.csv
--rw-r--r--   0        0        0      565 2024-04-25 19:50:46.856654 patent_client-5.0.0/patent_client/_sync/uspto/ptab/__init__.py
--rw-r--r--   0        0        0    10579 2024-04-25 19:50:46.856830 patent_client-5.0.0/patent_client/_sync/uspto/ptab/api.py
--rw-r--r--   0        0        0     1021 2024-04-25 19:50:46.857052 patent_client-5.0.0/patent_client/_sync/uspto/ptab/api_test.py
--rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.859921 patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
--rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.859981 patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
--rw-r--r--   0        0        0     2467 2024-04-25 19:50:46.860111 patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager.py
--rw-r--r--   0        0        0     2415 2024-04-25 19:50:46.860301 patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager_test.py
--rw-r--r--   0        0        0     8521 2024-04-25 19:50:46.860476 patent_client-5.0.0/patent_client/_sync/uspto/ptab/model.py
--rw-r--r--   0        0        0      658 2024-04-25 19:50:46.860666 patent_client-5.0.0/patent_client/_sync/uspto/ptab/util.py
--rw-r--r--   0        0        0      577 2024-04-25 19:50:46.860801 patent_client-5.0.0/patent_client/_sync/uspto/public_search/__init__.py
--rw-r--r--   0        0        0     6951 2024-04-25 19:50:46.860978 patent_client-5.0.0/patent_client/_sync/uspto/public_search/api.py
--rw-r--r--   0        0        0      682 2024-04-25 19:50:46.861094 patent_client-5.0.0/patent_client/_sync/uspto/public_search/api_test.py
--rw-r--r--   0        0        0      416 2024-04-25 19:50:46.877927 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/__init__.py
--rw-r--r--   0        0        0     2482 2024-04-25 19:50:46.879710 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/biblio.py
--rw-r--r--   0        0        0     7094 2024-04-25 19:50:46.881142 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/document.py
--rw-r--r--   0        0        0     2010 2024-04-25 19:50:46.881444 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/shared.py
--rw-r--r--   0        0        0     1451 2024-04-25 19:50:46.881652 patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert_test.py
--rw-r--r--   0        0        0      576 2024-04-25 19:50:46.881727 patent_client-5.0.0/patent_client/_sync/uspto/public_search/count_query.json
--rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.882601 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio.json
--rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.883125 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
--rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.883285 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
--rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.885243 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc.json
--rw-r--r--   0        0        0  2225007 2024-04-25 19:50:46.886477 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
--rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.888518 patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
--rw-r--r--   0        0        0     4487 2024-04-25 19:50:46.889539 patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager.py
--rw-r--r--   0        0        0     7339 2024-04-25 19:50:46.889731 patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager_test.py
--rw-r--r--   0        0        0      746 2024-04-25 19:50:46.889860 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/__init__.py
--rw-r--r--   0        0        0     3548 2024-04-25 19:50:46.889976 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/biblio.py
--rw-r--r--   0        0        0     7978 2024-04-25 19:50:46.890155 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/document.py
--rw-r--r--   0        0        0     2665 2024-04-25 19:50:46.890280 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/shared.py
--rw-r--r--   0        0        0     1953 2024-04-25 19:50:46.890406 patent_client-5.0.0/patent_client/_sync/uspto/public_search/model_test.py
--rw-r--r--   0        0        0     4936 2024-04-25 19:50:46.892506 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query.py
--rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.892581 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_config.csv
--rw-r--r--   0        0        0     4729 2024-04-25 19:50:46.894147 patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_test.py
--rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.894230 patent_client-5.0.0/patent_client/_sync/uspto/public_search/search_query.json
--rw-r--r--   0        0        0      689 2024-04-25 19:50:46.894466 patent_client-5.0.0/patent_client/_sync/uspto/public_search/util.py
--rw-r--r--   0        0        0     6043 2024-04-25 19:50:46.896118 patent_client-5.0.0/patent_client/parser.py
--rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.0/patent_client/patches.py
--rw-r--r--   0        0        0     3272 2024-04-25 19:50:46.897434 patent_client-5.0.0/patent_client/session.py
--rw-r--r--   0        0        0      685 2024-04-25 19:50:46.897630 patent_client-5.0.0/patent_client/settings.py
--rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.0/patent_client/test_parser.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.0/patent_client/util/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.0/patent_client/util/asyncio_util.py
--rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.0/patent_client/util/claims/__init__.py
--rw-r--r--   0        0        0     4313 2024-04-25 19:37:51.159560 patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.json
--rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.txt
--rw-r--r--   0        0        0     6924 2024-04-25 19:37:51.166864 patent_client-5.0.0/patent_client/util/claims/examples/published_claims.json
--rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.0/patent_client/util/claims/examples/published_claims.txt
--rw-r--r--   0        0        0      732 2024-04-03 19:26:37.308282 patent_client-5.0.0/patent_client/util/claims/model.py
--rw-r--r--   0        0        0     3546 2024-04-25 19:50:46.899557 patent_client-5.0.0/patent_client/util/claims/parser.py
--rw-r--r--   0        0        0      939 2024-04-25 19:50:46.899709 patent_client-5.0.0/patent_client/util/claims/parser_test.py
--rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.0/patent_client/util/format.py
--rw-r--r--   0        0        0     9464 2024-04-25 19:50:46.899927 patent_client-5.0.0/patent_client/util/manager.py
--rw-r--r--   0        0        0     3038 2024-04-25 19:50:46.900084 patent_client-5.0.0/patent_client/util/pydantic_util.py
--rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.0/patent_client/util/request_util.py
--rw-r--r--   0        0        0     1256 2024-04-25 19:50:46.900223 patent_client-5.0.0/patent_client/util/test.py
--rw-r--r--   0        0        0       22 2024-04-25 19:50:46.900461 patent_client-5.0.0/patent_client/version.py
--rw-r--r--   0        0        0     3376 2024-04-25 19:50:46.901426 patent_client-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     7701 1970-01-01 00:00:00.000000 patent_client-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      593 2024-04-03 19:26:37.145253 patent_client-5.0.1/LICENSE
+-rw-r--r--   0        0        0     6283 2024-05-02 16:19:13.662029 patent_client-5.0.1/README.md
+-rw-r--r--   0        0        0     1745 2024-05-01 18:31:51.839413 patent_client-5.0.1/patent_client/__init__.py
+-rw-r--r--   0        0        0      833 2024-05-01 18:11:58.854819 patent_client-5.0.1/patent_client/_async/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.516700 patent_client-5.0.1/patent_client/_async/epo/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-01 18:05:47.951425 patent_client-5.0.1/patent_client/_async/epo/ops/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.517050 patent_client-5.0.1/patent_client/_async/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      384 2024-05-02 16:38:02.138419 patent_client-5.0.1/patent_client/_async/epo/ops/family/api.py
+-rw-r--r--   0        0        0      471 2024-04-25 19:50:46.517324 patent_client-5.0.1/patent_client/_async/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518230 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-04-25 19:50:46.518338 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-04-25 19:50:46.518473 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-04-25 19:50:46.518568 patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      378 2024-05-01 18:05:47.952110 patent_client-5.0.1/patent_client/_async/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1119 2024-05-01 18:05:47.952437 patent_client-5.0.1/patent_client/_async/epo/ops/family/model.py
+-rw-r--r--   0        0        0      519 2024-05-01 18:05:47.952767 patent_client-5.0.1/patent_client/_async/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1545 2024-05-01 18:05:47.953175 patent_client-5.0.1/patent_client/_async/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      527 2024-05-01 18:05:47.953647 patent_client-5.0.1/patent_client/_async/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.520397 patent_client-5.0.1/patent_client/_async/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 16:38:02.129547 patent_client-5.0.1/patent_client/_async/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      320 2024-04-25 19:50:46.520929 patent_client-5.0.1/patent_client/_async/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-04-25 19:50:46.522112 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-04-25 19:50:46.522207 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-04-25 19:50:46.522310 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-04-25 19:50:46.522377 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-04-25 19:50:46.522453 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-04-25 19:50:46.522568 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-04-25 19:50:46.528538 patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      489 2024-05-01 18:05:47.953918 patent_client-5.0.1/patent_client/_async/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2375 2024-05-01 18:05:47.954191 patent_client-5.0.1/patent_client/_async/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5554 2024-05-01 18:49:55.209500 patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      498 2024-04-25 19:50:46.529161 patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4062 2024-05-01 18:05:47.954735 patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1216 2024-05-01 18:05:47.954968 patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      114 2024-04-25 19:50:46.529573 patent_client-5.0.1/patent_client/_async/epo/ops/legal/util.py
+-rw-r--r--   0        0        0       67 2024-04-25 19:50:46.529635 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1415 2024-05-02 16:38:02.133836 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     1806 2024-05-01 18:05:47.955307 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1117 2024-05-01 18:05:47.955516 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-04-25 19:50:46.531046 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-04-25 19:50:46.531107 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0      763 2024-05-01 18:05:47.955715 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0      952 2024-05-01 18:05:47.955921 patent_client-5.0.1/patent_client/_async/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.531523 patent_client-5.0.1/patent_client/_async/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5542 2024-05-02 16:38:45.106304 patent_client-5.0.1/patent_client/_async/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2743 2024-05-02 16:55:55.950023 patent_client-5.0.1/patent_client/_async/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1501 2024-04-25 19:50:46.535532 patent_client-5.0.1/patent_client/_async/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.535641 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-02 16:54:56.798037 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-04-25 19:50:46.535884 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-04-25 19:50:46.536001 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-02 16:54:56.801597 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18516 2024-05-02 16:54:56.812017 patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3226 2024-05-02 16:37:07.255945 patent_client-5.0.1/patent_client/_async/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2433 2024-05-02 16:55:55.950077 patent_client-5.0.1/patent_client/_async/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      321 2024-05-01 18:05:47.957189 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     2754 2024-05-01 18:05:47.957413 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1050 2024-05-01 18:05:47.957672 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2108 2024-05-02 16:32:37.841594 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0      843 2024-05-01 18:05:47.958081 patent_client-5.0.1/patent_client/_async/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      285 2024-05-01 18:05:47.958344 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     3962 2024-05-01 18:05:47.958633 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0      874 2024-05-01 18:05:47.958917 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     1668 2024-05-01 18:05:47.959251 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0      650 2024-04-25 19:50:46.538723 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3193 2024-05-01 18:16:57.840152 patent_client-5.0.1/patent_client/_async/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-04-25 19:50:46.539395 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-04-25 19:50:46.539578 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-04-25 19:50:46.539698 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-04-25 19:50:46.539787 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-02 16:54:56.944056 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-04-25 19:50:46.539986 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-02 16:54:56.947909 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-04-25 19:50:46.540212 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-04-25 19:50:46.540329 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-04-25 19:50:46.540478 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-04-25 19:50:46.540611 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-04-25 19:50:46.540733 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-04-25 19:50:46.540800 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-04-25 19:50:46.540898 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-04-25 19:50:46.540961 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-04-25 19:50:46.541071 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-04-25 19:50:46.541138 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-04-25 19:50:46.541208 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-04-25 19:50:46.541291 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-04-25 19:50:46.541397 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-04-25 19:50:46.541481 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-04-25 19:50:46.541601 patent_client-5.0.1/patent_client/_async/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3478 2024-05-02 16:38:02.129285 patent_client-5.0.1/patent_client/_async/epo/ops/session.py
+-rw-r--r--   0        0        0     2881 2024-05-02 16:55:55.950107 patent_client-5.0.1/patent_client/_async/epo/ops/util.py
+-rw-r--r--   0        0        0     3234 2024-05-01 18:32:10.993912 patent_client-5.0.1/patent_client/_async/http_client.py
+-rw-r--r--   0        0        0      201 2024-05-01 18:11:58.854920 patent_client-5.0.1/patent_client/_async/odp.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542707 patent_client-5.0.1/patent_client/_async/uspto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.542758 patent_client-5.0.1/patent_client/_async/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-01 18:05:47.961041 patent_client-5.0.1/patent_client/_async/uspto/assignment/api.py
+-rw-r--r--   0        0        0      921 2024-05-01 18:11:58.854972 patent_client-5.0.1/patent_client/_async/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     3633 2024-05-01 18:05:47.961566 patent_client-5.0.1/patent_client/_async/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1149 2024-04-25 19:50:46.559695 patent_client-5.0.1/patent_client/_async/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-04-25 19:50:46.559866 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-04-25 19:50:46.560112 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-04-25 19:50:46.560215 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-04-25 19:50:46.560334 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-04-25 19:50:46.560560 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-04-25 19:50:46.560745 patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3454 2024-05-01 18:15:07.226884 patent_client-5.0.1/patent_client/_async/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4202 2024-05-01 18:14:52.417225 patent_client-5.0.1/patent_client/_async/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5506 2024-05-01 18:33:09.323130 patent_client-5.0.1/patent_client/_async/uspto/assignment/model.py
+-rw-r--r--   0        0        0     1932 2024-05-01 18:05:47.962761 patent_client-5.0.1/patent_client/_async/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.563151 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3226 2024-05-01 18:37:44.350189 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1100 2024-05-01 18:05:47.963236 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     2781 2024-05-01 18:05:47.963445 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1707 2024-05-01 18:05:47.963660 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1567 2024-05-01 18:37:29.912372 patent_client-5.0.1/patent_client/_async/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.566476 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2109 2024-05-01 18:05:47.964054 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1143 2024-05-01 18:05:47.964243 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-04-25 19:50:46.606532 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     1902 2024-05-01 18:05:47.969601 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7111 2024-05-01 18:11:58.855043 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3738 2024-05-01 18:05:47.970105 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6063 2024-05-01 18:05:47.970370 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5252 2024-05-01 18:05:47.970651 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-04-25 19:50:46.614090 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-04-25 19:50:46.614159 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-04-25 19:50:46.614257 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-04-25 19:50:46.614376 patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0        1 2024-05-01 18:05:47.970962 patent_client-5.0.1/patent_client/_async/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5502 2024-05-01 18:11:58.855103 patent_client-5.0.1/patent_client/_async/uspto/odp/api.py
+-rw-r--r--   0        0        0     2834 2024-05-01 18:05:47.971502 patent_client-5.0.1/patent_client/_async/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-04-25 19:50:46.622009 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-04-25 19:50:46.622371 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-04-25 19:50:46.622570 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-04-25 19:50:46.622985 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-04-25 19:50:46.623140 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-04-25 19:50:46.623322 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-04-25 19:50:46.623651 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-04-25 19:50:46.623819 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-04-25 19:50:46.623951 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-04-25 19:50:46.624215 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-04-25 19:50:46.624391 patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     4834 2024-05-01 18:11:58.855157 patent_client-5.0.1/patent_client/_async/uspto/odp/manager.py
+-rw-r--r--   0        0        0     1895 2024-05-01 18:11:58.855213 patent_client-5.0.1/patent_client/_async/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16427 2024-05-01 18:11:58.855271 patent_client-5.0.1/patent_client/_async/uspto/odp/model.py
+-rw-r--r--   0        0        0    12253 2024-05-01 18:05:47.972423 patent_client-5.0.1/patent_client/_async/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2396 2024-05-01 18:05:47.972634 patent_client-5.0.1/patent_client/_async/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-04-25 19:50:46.625967 patent_client-5.0.1/patent_client/_async/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      475 2024-05-01 18:05:47.972937 patent_client-5.0.1/patent_client/_async/uspto/odp/util.py
+-rw-r--r--   0        0        0      132 2024-05-01 18:05:47.973121 patent_client-5.0.1/patent_client/_async/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-01 18:05:47.973352 patent_client-5.0.1/patent_client/_async/uspto/peds/api.py
+-rw-r--r--   0        0        0      711 2024-05-01 18:05:47.973610 patent_client-5.0.1/patent_client/_async/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-04-25 19:50:46.659667 patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8585 2024-05-02 16:13:03.406844 patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8495 2024-05-02 16:01:44.826324 patent_client-5.0.1/patent_client/_async/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9726 2024-05-02 16:13:06.160175 patent_client-5.0.1/patent_client/_async/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    14987 2024-05-02 16:10:44.102210 patent_client-5.0.1/patent_client/_async/uspto/peds/model.py
+-rw-r--r--   0        0        0     6116 2024-05-01 18:05:47.974623 patent_client-5.0.1/patent_client/_async/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-04-25 19:50:46.665065 patent_client-5.0.1/patent_client/_async/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      188 2024-05-01 18:14:39.938865 patent_client-5.0.1/patent_client/_async/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10200 2024-05-01 18:05:47.974861 patent_client-5.0.1/patent_client/_async/uspto/ptab/api.py
+-rw-r--r--   0        0        0      701 2024-04-25 19:50:46.666047 patent_client-5.0.1/patent_client/_async/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-04-25 19:50:46.668915 patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-04-25 19:50:46.668975 patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2085 2024-05-01 18:05:47.975042 patent_client-5.0.1/patent_client/_async/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2311 2024-05-01 18:05:47.975211 patent_client-5.0.1/patent_client/_async/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8358 2024-05-01 18:37:03.633749 patent_client-5.0.1/patent_client/_async/uspto/ptab/model.py
+-rw-r--r--   0        0        0      242 2024-04-25 19:50:46.669654 patent_client-5.0.1/patent_client/_async/uspto/ptab/util.py
+-rw-r--r--   0        0        0      326 2024-05-01 18:14:14.991401 patent_client-5.0.1/patent_client/_async/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6701 2024-05-01 18:38:39.241032 patent_client-5.0.1/patent_client/_async/uspto/public_search/api.py
+-rw-r--r--   0        0        0      298 2024-04-25 19:50:46.670256 patent_client-5.0.1/patent_client/_async/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0        0 2024-04-25 19:50:46.692132 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2066 2024-05-01 18:05:47.981591 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     6678 2024-05-01 18:05:47.983341 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     1594 2024-05-01 18:05:47.983719 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1035 2024-05-01 18:13:57.304685 patent_client-5.0.1/patent_client/_async/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-04-25 19:50:46.698650 patent_client-5.0.1/patent_client/_async/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-04-25 19:50:46.699482 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-04-25 19:50:46.699909 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-04-25 19:50:46.700055 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-04-25 19:50:46.704774 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-02 16:54:59.151394 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-04-25 19:50:46.708274 patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4144 2024-05-01 18:05:47.983936 patent_client-5.0.1/patent_client/_async/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7743 2024-05-01 18:05:47.984232 patent_client-5.0.1/patent_client/_async/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      524 2024-05-01 18:40:07.745391 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3144 2024-05-01 18:16:57.840869 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7574 2024-05-01 18:05:47.984820 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2249 2024-05-01 18:05:47.984983 patent_client-5.0.1/patent_client/_async/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1535 2024-05-01 18:13:46.898757 patent_client-5.0.1/patent_client/_async/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4520 2024-05-01 18:05:47.985447 patent_client-5.0.1/patent_client/_async/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-04-25 19:50:46.722489 patent_client-5.0.1/patent_client/_async/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4313 2024-05-01 18:12:45.762919 patent_client-5.0.1/patent_client/_async/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-04-25 19:50:46.722977 patent_client-5.0.1/patent_client/_async/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      273 2024-04-25 19:50:46.723043 patent_client-5.0.1/patent_client/_async/uspto/public_search/util.py
+-rw-r--r--   0        0        0     1249 2024-05-02 16:54:49.273351 patent_client-5.0.1/patent_client/_sync/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.680949 patent_client-5.0.1/patent_client/_sync/epo/__init__.py
+-rw-r--r--   0        0        0      630 2024-05-02 16:54:49.692358 patent_client-5.0.1/patent_client/_sync/epo/ops/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.706525 patent_client-5.0.1/patent_client/_sync/epo/ops/family/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-02 16:54:49.709397 patent_client-5.0.1/patent_client/_sync/epo/ops/family/api.py
+-rw-r--r--   0        0        0      855 2024-05-02 16:54:49.710444 patent_client-5.0.1/patent_client/_sync/epo/ops/family/api_test.py
+-rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714131 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json
+-rw-r--r--   0        0        0     7247 2024-05-02 16:54:49.714466 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_convert.json
+-rw-r--r--   0        0        0     8854 2024-05-02 16:54:49.714990 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_input.xml
+-rw-r--r--   0        0        0     7445 2024-05-02 16:54:49.714682 patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json
+-rw-r--r--   0        0        0      772 2024-05-02 16:54:49.711289 patent_client-5.0.1/patent_client/_sync/epo/ops/family/manager.py
+-rw-r--r--   0        0        0     1535 2024-05-02 16:54:49.708518 patent_client-5.0.1/patent_client/_sync/epo/ops/family/model.py
+-rw-r--r--   0        0        0      903 2024-05-02 16:54:49.705264 patent_client-5.0.1/patent_client/_sync/epo/ops/family/model_test.py
+-rw-r--r--   0        0        0     1961 2024-05-02 16:54:49.713729 patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema.py
+-rw-r--r--   0        0        0      943 2024-05-02 16:54:49.706394 patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.784538 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-02 16:54:49.789201 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api.py
+-rw-r--r--   0        0        0      704 2024-05-02 16:54:49.799011 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api_test.py
+-rw-r--r--   0        0        0    76105 2024-05-02 16:54:49.811517 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml
+-rw-r--r--   0        0        0    44094 2024-05-02 16:54:49.808791 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json
+-rw-r--r--   0        0        0    78351 2024-05-02 16:54:49.811216 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml
+-rw-r--r--   0        0        0    45316 2024-05-02 16:54:49.810170 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json
+-rw-r--r--   0        0        0    22970 2024-05-02 16:54:49.810402 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml
+-rw-r--r--   0        0        0    11923 2024-05-02 16:54:49.810723 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json
+-rw-r--r--   0        0        0   292939 2024-05-02 16:54:49.808401 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx
+-rw-r--r--   0        0        0      883 2024-05-02 16:54:49.800072 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/manager.py
+-rw-r--r--   0        0        0     2791 2024-05-02 16:54:49.788392 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/model.py
+-rw-r--r--   0        0        0     5908 2024-05-02 16:54:49.798143 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes.py
+-rw-r--r--   0        0        0      882 2024-05-02 16:54:49.781664 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes_test.py
+-rw-r--r--   0        0        0     4478 2024-05-02 16:54:49.806767 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema.py
+-rw-r--r--   0        0        0     1632 2024-05-02 16:54:49.783877 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema_test.py
+-rw-r--r--   0        0        0      530 2024-05-02 16:54:49.784387 patent_client-5.0.1/patent_client/_sync/epo/ops/legal/util.py
+-rw-r--r--   0        0        0      483 2024-05-02 16:54:49.693120 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/__init__.py
+-rw-r--r--   0        0        0     1819 2024-05-02 16:54:49.696999 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api.py
+-rw-r--r--   0        0        0     2062 2024-05-02 16:54:49.702142 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api_test.py
+-rw-r--r--   0        0        0     1533 2024-05-02 16:54:49.699423 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.py
+-rw-r--r--   0        0        0     5589 2024-05-02 16:54:49.692702 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.txt
+-rw-r--r--   0        0        0     2086 2024-05-02 16:54:49.697276 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/messages.txt
+-rw-r--r--   0        0        0     1179 2024-05-02 16:54:49.694652 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/model.py
+-rw-r--r--   0        0        0     1368 2024-05-02 16:54:49.703985 patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/schema.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.724238 patent_client-5.0.1/patent_client/_sync/epo/ops/published/__init__.py
+-rw-r--r--   0        0        0     5746 2024-05-02 16:55:55.949498 patent_client-5.0.1/patent_client/_sync/epo/ops/published/api.py
+-rw-r--r--   0        0        0     2878 2024-05-02 16:55:55.949751 patent_client-5.0.1/patent_client/_sync/epo/ops/published/api_test.py
+-rw-r--r--   0        0        0     1917 2024-05-02 16:54:49.726807 patent_client-5.0.1/patent_client/_sync/epo/ops/published/cql.py
+-rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.780449 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0     6174 2024-05-02 16:55:18.406245 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json
+-rw-r--r--   0        0        0     5148 2024-05-02 16:54:49.779487 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json
+-rw-r--r--   0        0        0    10706 2024-05-02 16:54:49.779804 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    20102 2024-05-02 16:55:18.590618 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0    18448 2024-05-02 16:55:18.792704 patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/search_result.xml
+-rw-r--r--   0        0        0     3516 2024-05-02 16:54:49.745375 patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager.py
+-rw-r--r--   0        0        0     2383 2024-05-02 16:55:55.949242 patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager_test.py
+-rw-r--r--   0        0        0      737 2024-05-02 16:54:49.766843 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-02 16:54:49.771074 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/biblio.py
+-rw-r--r--   0        0        0     1466 2024-05-02 16:54:49.778409 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/fulltext.py
+-rw-r--r--   0        0        0     2500 2024-05-02 16:54:49.774783 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/images.py
+-rw-r--r--   0        0        0     1259 2024-05-02 16:54:49.776390 patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/search.py
+-rw-r--r--   0        0        0      701 2024-05-02 16:54:49.753627 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/__init__.py
+-rw-r--r--   0        0        0     4378 2024-05-02 16:54:49.760006 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/biblio.py
+-rw-r--r--   0        0        0     1290 2024-05-02 16:54:49.765780 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/fulltext.py
+-rw-r--r--   0        0        0     2084 2024-05-02 16:54:49.762883 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/images.py
+-rw-r--r--   0        0        0     1066 2024-05-02 16:54:49.764083 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/search.py
+-rw-r--r--   0        0        0     3609 2024-05-02 16:54:49.724096 patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema_test.py
+-rw-r--r--   0        0        0   105372 2024-05-02 16:54:49.746815 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example.xml
+-rw-r--r--   0        0        0    27945 2024-05-02 16:54:49.747751 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml
+-rw-r--r--   0        0        0    13833 2024-05-02 16:54:49.747456 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml
+-rw-r--r--   0        0        0    51036 2024-05-02 16:54:49.747138 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml
+-rw-r--r--   0        0        0     7251 2024-05-02 16:55:22.225396 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.json
+-rw-r--r--   0        0        0     3973 2024-05-02 16:54:49.749328 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.xml
+-rw-r--r--   0        0        0    13020 2024-05-02 16:55:22.229990 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.json
+-rw-r--r--   0        0        0     5916 2024-05-02 16:54:49.748436 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.xml
+-rw-r--r--   0        0        0    12044 2024-05-02 16:54:49.746102 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/description_example.xml
+-rw-r--r--   0        0        0     9211 2024-05-02 16:54:49.750694 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json
+-rw-r--r--   0        0        0     8815 2024-05-02 16:54:49.750054 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json
+-rw-r--r--   0        0        0     7197 2024-05-02 16:54:49.751835 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/claims_example.json
+-rw-r--r--   0        0        0     1956 2024-05-02 16:54:49.752720 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml
+-rw-r--r--   0        0        0    13035 2024-05-02 16:54:49.751111 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml
+-rw-r--r--   0        0        0     3459 2024-05-02 16:54:49.751285 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml
+-rw-r--r--   0        0        0    11421 2024-05-02 16:54:49.751611 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml
+-rw-r--r--   0        0        0    21196 2024-05-02 16:54:49.750350 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml
+-rw-r--r--   0        0        0     1076 2024-05-02 16:54:49.749720 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/image_example.json
+-rw-r--r--   0        0        0    34696 2024-05-02 16:54:49.752544 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/search_result.xml
+-rw-r--r--   0        0        0    21197 2024-05-02 16:54:49.745766 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml
+-rw-r--r--   0        0        0     3059 2024-05-02 16:54:49.748069 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/image_example.xml
+-rw-r--r--   0        0        0     5642 2024-05-02 16:54:49.749004 patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/search_example.xml
+-rw-r--r--   0        0        0     3872 2024-05-02 16:54:49.691686 patent_client-5.0.1/patent_client/_sync/epo/ops/session.py
+-rw-r--r--   0        0        0     3129 2024-05-02 16:55:55.949894 patent_client-5.0.1/patent_client/_sync/epo/ops/util.py
+-rw-r--r--   0        0        0     3611 2024-05-02 16:54:49.271384 patent_client-5.0.1/patent_client/_sync/http_client.py
+-rw-r--r--   0        0        0      616 2024-05-02 16:54:49.274025 patent_client-5.0.1/patent_client/_sync/odp.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.274313 patent_client-5.0.1/patent_client/_sync/uspto/__init__.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.422160 patent_client-5.0.1/patent_client/_sync/uspto/assignment/__init__.py
+-rw-r--r--   0        0        0     2936 2024-05-02 16:54:49.435281 patent_client-5.0.1/patent_client/_sync/uspto/assignment/api.py
+-rw-r--r--   0        0        0     1273 2024-05-02 16:54:49.436962 patent_client-5.0.1/patent_client/_sync/uspto/assignment/api_test.py
+-rw-r--r--   0        0        0     4049 2024-05-02 16:54:49.422016 patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert.py
+-rw-r--r--   0        0        0     1565 2024-05-02 16:54:49.439130 patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert_test.py
+-rw-r--r--   0        0        0     5926 2024-05-02 16:54:49.448163 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json
+-rw-r--r--   0        0        0    13274 2024-05-02 16:54:49.448757 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml
+-rw-r--r--   0        0        0     4573 2024-05-02 16:54:49.445263 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json
+-rw-r--r--   0        0        0    11638 2024-05-02 16:54:49.446731 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml
+-rw-r--r--   0        0        0   243532 2024-05-02 16:54:49.446163 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json
+-rw-r--r--   0        0        0   277704 2024-05-02 16:54:49.447858 patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml
+-rw-r--r--   0        0        0     3826 2024-05-02 16:54:49.444752 patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager.py
+-rw-r--r--   0        0        0     4308 2024-05-02 16:54:49.413378 patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager_test.py
+-rw-r--r--   0        0        0     5910 2024-05-02 16:54:49.431060 patent_client-5.0.1/patent_client/_sync/uspto/assignment/model.py
+-rw-r--r--   0        0        0     2348 2024-05-02 16:54:49.416385 patent_client-5.0.1/patent_client/_sync/uspto/assignment/model_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.277934 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/__init__.py
+-rw-r--r--   0        0        0     3593 2024-05-02 16:54:49.286527 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api.py
+-rw-r--r--   0        0        0     1382 2024-05-02 16:54:49.288731 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api_test.py
+-rw-r--r--   0        0        0     3113 2024-05-02 16:54:49.293522 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager.py
+-rw-r--r--   0        0        0     1963 2024-05-02 16:54:49.277782 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager_test.py
+-rw-r--r--   0        0        0     1971 2024-05-02 16:54:49.280906 patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/model.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.620966 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/__init__.py
+-rw-r--r--   0        0        0     2446 2024-05-02 16:54:49.635557 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api.py
+-rw-r--r--   0        0        0     1463 2024-05-02 16:54:49.637862 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api_test.py
+-rw-r--r--   0        0        0     2983 2024-05-02 16:54:49.620829 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/gd_input.csv
+-rw-r--r--   0        0        0     2272 2024-05-02 16:54:49.641199 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/manager.py
+-rw-r--r--   0        0        0     7354 2024-05-02 16:54:49.632107 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model.py
+-rw-r--r--   0        0        0     3853 2024-05-02 16:54:49.602482 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model_test.py
+-rw-r--r--   0        0        0     6479 2024-05-02 16:54:49.620511 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query.py
+-rw-r--r--   0        0        0     5668 2024-05-02 16:54:49.611314 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query_test.py
+-rw-r--r--   0        0        0     4134 2024-05-02 16:54:49.641637 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app.json
+-rw-r--r--   0        0        0     2527 2024-05-02 16:54:49.642377 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app_expected.json
+-rw-r--r--   0        0        0    12360 2024-05-02 16:54:49.642679 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list.json
+-rw-r--r--   0        0        0    10994 2024-05-02 16:54:49.642129 patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json
+-rw-r--r--   0        0        0      417 2024-05-02 16:54:49.474650 patent_client-5.0.1/patent_client/_sync/uspto/odp/__init__.py
+-rw-r--r--   0        0        0     5786 2024-05-02 16:54:49.507980 patent_client-5.0.1/patent_client/_sync/uspto/odp/api.py
+-rw-r--r--   0        0        0     2898 2024-05-02 16:54:49.512417 patent_client-5.0.1/patent_client/_sync/uspto/odp/api_test.py
+-rw-r--r--   0        0        0    16485 2024-05-02 16:54:49.523098 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/adjustment.json
+-rw-r--r--   0        0        0   187414 2024-05-02 16:54:49.524963 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/application.json
+-rw-r--r--   0        0        0     1479 2024-05-02 16:54:49.522829 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/assignment.json
+-rw-r--r--   0        0        0   172204 2024-05-02 16:54:49.524478 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/attorney.json
+-rw-r--r--   0        0        0     2697 2024-05-02 16:54:49.522678 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/biblio.json
+-rw-r--r--   0        0        0     1650 2024-05-02 16:54:49.520625 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/continuity.json
+-rw-r--r--   0        0        0    72937 2024-05-02 16:54:49.523412 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/documents.json
+-rw-r--r--   0        0        0      317 2024-05-02 16:54:49.525169 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/foreign_priority.json
+-rw-r--r--   0        0        0     4077 2024-05-02 16:54:49.520959 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/search.json
+-rw-r--r--   0        0        0    84893 2024-05-02 16:54:49.522498 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/swagger.yaml
+-rw-r--r--   0        0        0     8767 2024-05-02 16:54:49.523715 patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/transactions.json
+-rw-r--r--   0        0        0     5053 2024-05-02 16:54:49.520104 patent_client-5.0.1/patent_client/_sync/uspto/odp/manager.py
+-rw-r--r--   0        0        0     2025 2024-05-02 16:54:49.451871 patent_client-5.0.1/patent_client/_sync/uspto/odp/manager_test.py
+-rw-r--r--   0        0        0    16610 2024-05-02 16:54:49.499830 patent_client-5.0.1/patent_client/_sync/uspto/odp/model.py
+-rw-r--r--   0        0        0    12669 2024-05-02 16:54:49.469166 patent_client-5.0.1/patent_client/_sync/uspto/odp/model_test.py
+-rw-r--r--   0        0        0     2812 2024-05-02 16:54:49.473108 patent_client-5.0.1/patent_client/_sync/uspto/odp/query.py
+-rw-r--r--   0        0        0     2531 2024-05-02 16:54:49.474462 patent_client-5.0.1/patent_client/_sync/uspto/odp/query_fields.csv
+-rw-r--r--   0        0        0      891 2024-05-02 16:54:49.474154 patent_client-5.0.1/patent_client/_sync/uspto/odp/util.py
+-rw-r--r--   0        0        0      548 2024-05-02 16:54:49.549313 patent_client-5.0.1/patent_client/_sync/uspto/peds/__init__.py
+-rw-r--r--   0        0        0     4838 2024-05-02 16:54:49.579007 patent_client-5.0.1/patent_client/_sync/uspto/peds/api.py
+-rw-r--r--   0        0        0     1031 2024-05-02 16:54:49.580486 patent_client-5.0.1/patent_client/_sync/uspto/peds/api_test.py
+-rw-r--r--   0        0        0    94707 2024-05-02 16:54:49.595544 patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_input.json
+-rw-r--r--   0        0        0     8585 2024-05-02 16:54:49.594371 patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_output.json
+-rw-r--r--   0        0        0     8814 2024-05-02 16:54:49.593537 patent_client-5.0.1/patent_client/_sync/uspto/peds/manager.py
+-rw-r--r--   0        0        0     9448 2024-05-02 16:54:49.539641 patent_client-5.0.1/patent_client/_sync/uspto/peds/manager_test.py
+-rw-r--r--   0        0        0    15332 2024-05-02 16:54:49.571891 patent_client-5.0.1/patent_client/_sync/uspto/peds/model.py
+-rw-r--r--   0        0        0     6532 2024-05-02 16:54:49.548772 patent_client-5.0.1/patent_client/_sync/uspto/peds/query.py
+-rw-r--r--   0        0        0     4469 2024-05-02 16:54:49.540007 patent_client-5.0.1/patent_client/_sync/uspto/peds/search_index.csv
+-rw-r--r--   0        0        0      604 2024-05-02 16:54:49.647690 patent_client-5.0.1/patent_client/_sync/uspto/ptab/__init__.py
+-rw-r--r--   0        0        0    10579 2024-05-02 16:54:49.674786 patent_client-5.0.1/patent_client/_sync/uspto/ptab/api.py
+-rw-r--r--   0        0        0     1021 2024-05-02 16:54:49.676210 patent_client-5.0.1/patent_client/_sync/uspto/ptab/api_test.py
+-rw-r--r--   0        0        0     1300 2024-05-02 16:54:49.680173 patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/documents_input.json
+-rw-r--r--   0        0        0     1057 2024-05-02 16:54:49.680705 patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json
+-rw-r--r--   0        0        0     2467 2024-05-02 16:54:49.679688 patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager.py
+-rw-r--r--   0        0        0     2415 2024-05-02 16:54:49.646348 patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager_test.py
+-rw-r--r--   0        0        0     8762 2024-05-02 16:54:49.660127 patent_client-5.0.1/patent_client/_sync/uspto/ptab/model.py
+-rw-r--r--   0        0        0      658 2024-05-02 16:54:49.647071 patent_client-5.0.1/patent_client/_sync/uspto/ptab/util.py
+-rw-r--r--   0        0        0      742 2024-05-02 16:54:49.325197 patent_client-5.0.1/patent_client/_sync/uspto/public_search/__init__.py
+-rw-r--r--   0        0        0     6952 2024-05-02 16:54:49.335229 patent_client-5.0.1/patent_client/_sync/uspto/public_search/api.py
+-rw-r--r--   0        0        0      682 2024-05-02 16:54:49.335976 patent_client-5.0.1/patent_client/_sync/uspto/public_search/api_test.py
+-rw-r--r--   0        0        0      416 2024-05-02 16:54:49.389789 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-02 16:54:49.394364 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/biblio.py
+-rw-r--r--   0        0        0     7094 2024-05-02 16:54:49.407282 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/document.py
+-rw-r--r--   0        0        0     2010 2024-05-02 16:54:49.396701 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/shared.py
+-rw-r--r--   0        0        0     1451 2024-05-02 16:54:49.337751 patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert_test.py
+-rw-r--r--   0        0        0      576 2024-05-02 16:54:49.324277 patent_client-5.0.1/patent_client/_sync/uspto/public_search/count_query.json
+-rw-r--r--   0        0        0   867778 2024-05-02 16:54:49.379455 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio.json
+-rw-r--r--   0        0        0   270895 2024-05-02 16:54:49.385172 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json
+-rw-r--r--   0        0        0   220128 2024-05-02 16:54:49.389523 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json
+-rw-r--r--   0        0        0  2431829 2024-05-02 16:54:49.387433 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc.json
+-rw-r--r--   0        0        0  2225007 2024-05-02 16:55:24.352861 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json
+-rw-r--r--   0        0        0  3962033 2024-05-02 16:54:49.370527 patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_output.json
+-rw-r--r--   0        0        0     4487 2024-05-02 16:54:49.344979 patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager.py
+-rw-r--r--   0        0        0     7339 2024-05-02 16:54:49.306132 patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager_test.py
+-rw-r--r--   0        0        0      940 2024-05-02 16:54:49.346685 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/__init__.py
+-rw-r--r--   0        0        0     3548 2024-05-02 16:54:49.351720 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/biblio.py
+-rw-r--r--   0        0        0     7978 2024-05-02 16:54:49.367308 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/document.py
+-rw-r--r--   0        0        0     2665 2024-05-02 16:54:49.355383 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/shared.py
+-rw-r--r--   0        0        0     1951 2024-05-02 16:54:49.308937 patent_client-5.0.1/patent_client/_sync/uspto/public_search/model_test.py
+-rw-r--r--   0        0        0     4936 2024-05-02 16:54:49.323048 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query.py
+-rw-r--r--   0        0        0     1344 2024-05-02 16:54:49.293946 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_config.csv
+-rw-r--r--   0        0        0     4729 2024-05-02 16:54:49.316153 patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_test.py
+-rw-r--r--   0        0        0     1049 2024-05-02 16:54:49.345205 patent_client-5.0.1/patent_client/_sync/uspto/public_search/search_query.json
+-rw-r--r--   0        0        0      689 2024-05-02 16:54:49.323888 patent_client-5.0.1/patent_client/_sync/uspto/public_search/util.py
+-rw-r--r--   0        0        0     6043 2024-05-01 18:05:48.009638 patent_client-5.0.1/patent_client/parser.py
+-rw-r--r--   0        0        0      331 2024-04-03 19:26:37.191135 patent_client-5.0.1/patent_client/patches.py
+-rw-r--r--   0        0        0     3276 2024-05-01 18:37:20.358790 patent_client-5.0.1/patent_client/session.py
+-rw-r--r--   0        0        0      685 2024-05-01 18:05:48.010111 patent_client-5.0.1/patent_client/settings.py
+-rw-r--r--   0        0        0     8162 2024-04-03 19:26:37.191401 patent_client-5.0.1/patent_client/test_parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306255 patent_client-5.0.1/patent_client/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-25 19:50:46.899374 patent_client-5.0.1/patent_client/util/asyncio_util.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:26:37.306393 patent_client-5.0.1/patent_client/util/claims/__init__.py
+-rw-r--r--   0        0        0     4313 2024-05-02 16:55:25.224279 patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.json
+-rw-r--r--   0        0        0     2456 2024-04-03 19:26:37.308088 patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.txt
+-rw-r--r--   0        0        0     6924 2024-05-02 16:55:25.227038 patent_client-5.0.1/patent_client/util/claims/examples/published_claims.json
+-rw-r--r--   0        0        0     3719 2024-04-03 19:26:37.308219 patent_client-5.0.1/patent_client/util/claims/examples/published_claims.txt
+-rw-r--r--   0        0        0      735 2024-05-01 18:11:58.857909 patent_client-5.0.1/patent_client/util/claims/model.py
+-rw-r--r--   0        0        0     3554 2024-05-01 18:11:58.857956 patent_client-5.0.1/patent_client/util/claims/parser.py
+-rw-r--r--   0        0        0      939 2024-05-01 18:05:48.010826 patent_client-5.0.1/patent_client/util/claims/parser_test.py
+-rw-r--r--   0        0        0      611 2024-04-03 19:26:37.308464 patent_client-5.0.1/patent_client/util/format.py
+-rw-r--r--   0        0        0     9728 2024-05-02 16:55:55.950403 patent_client-5.0.1/patent_client/util/manager.py
+-rw-r--r--   0        0        0     3035 2024-05-01 18:29:51.038167 patent_client-5.0.1/patent_client/util/pydantic_util.py
+-rw-r--r--   0        0        0      861 2024-04-03 19:26:37.308765 patent_client-5.0.1/patent_client/util/request_util.py
+-rw-r--r--   0        0        0     1255 2024-05-01 18:11:58.858129 patent_client-5.0.1/patent_client/util/test.py
+-rw-r--r--   0        0        0       22 2024-05-02 16:56:44.518693 patent_client-5.0.1/patent_client/version.py
+-rw-r--r--   0        0        0     3376 2024-05-02 16:56:44.518941 patent_client-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7880 1970-01-01 00:00:00.000000 patent_client-5.0.1/PKG-INFO
```

### Comparing `patent_client-5.0.0/LICENSE` & `patent_client-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/README.md` & `patent_client-5.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: patent-client
+Version: 5.0.1
+Summary: A set of ORM-style clients for publicly available intellectual property data
+Home-page: https://github.com/parkerhancock/patent_client
+License: Apache Software License 2.0
+Keywords: patent,intellectual property,usitc,epo,ops,trademark,inpadoc,337
+Author: Parker Hancock
+Author-email: 633163+parkerhancock@users.noreply.github.com
+Requires-Python: >=3.9,<3.13
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Legal Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: async-property (>=0.2.2,<0.3.0)
+Requires-Dist: hishel (>=0.0.20,<0.0.21)
+Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
+Requires-Dist: lxml (>=4.9.0,<5.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pydantic (>=2.4.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
+Requires-Dist: pypdf (>=3.17.0,<4.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: yankee (>=0.1.43,<0.2.0)
+Project-URL: Documentation, https://patent-client.readthedocs.io
+Project-URL: Repository, https://github.com/parkerhancock/patent_client
+Description-Content-Type: text/markdown
+
 [![patent_client_logo](https://raw.githubusercontent.com/parkerhancock/patent_client/master/docs/_static/patent_client_logo.svg)](https://patent-client.readthedocs.io)
 
 [![Build](https://github.com/parkerhancock/patent_client/actions/workflows/build.yaml/badge.svg)](https://github.com/parkerhancock/patent_client/actions/workflows/build.yaml)
 [![codecov](https://codecov.io/gh/parkerhancock/patent_client/branch/master/graph/badge.svg?token=pWsiQLHi6r)](https://codecov.io/gh/parkerhancock/patent_client)
 [![Documentation](https://img.shields.io/readthedocs/patent-client/stable)](https://patent-client.readthedocs.io/en/stable/)
 
 
@@ -54,24 +89,24 @@
 * Free software: Apache Software License 2.0
 
 [DORM]: https://docs.djangoproject.com/en/4.0/topics/db/queries/
 [PANDAS]: https://pandas.pydata.org/docs/
 [httpx]: https://www.python-httpx.org/
 [hishel]: https://hishel.com/
 [yankee]: https://github.com/parkerhancock/yankee
-[Assignment]: https://developer.uspto.gov/api-catalog/patent-assignment-search-beta
-[OPS]: http://ops.epo.org
-[PPS]:  https://ppubs.uspto.gov/pubwebapp/static/pages/landing.html
-[PEDS]: https://developer.uspto.gov/api-catalog/ped
-[PTAB]: https://developer.uspto.gov/api-catalog/ptab-api-v2
+[Assignment]: user_guide/assignments.html
+[OPS]: https://patent-client.readthedocs.io/en/latest/user_guide/epo.html
+[PPS]:  https://patent-client.readthedocs.io/en/latest/user_guide/fulltext.html
+[PEDS]: https://patent-client.readthedocs.io/en/latest/user_guide/peds.html
+[PTAB]: https://patent-client.readthedocs.io/en/latest/user_guide/ptab.html
 [USPTO]: http://developer.uspto.gov
-[BDSS]: https://developer.uspto.gov/api-catalog/bdss
-[GD]: https://globaldossier.uspto.gov
+[BDSS]: https://patent-client.readthedocs.io/en/latest/user_guide/bulk_data.html
+[GD]: https://patent-client.readthedocs.io/en/latest/user_guide/global_dossier.html
 [pydantic]: https://docs.pydantic.dev/latest/
-[ODP]: https://beta-data.uspto.gov/home
+[ODP]: https://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html
 
 
 ## Installation
 
 ```
 pip install patent_client
 ```
@@ -146,7 +181,8 @@
 # Related projects
 
 - [Python EPO OPS Client](https://github.com/55minutes/python-epo-ops-client)
 - [Google Public Patent Data](https://github.com/google/patents-public-data)
 - [PatentsView API Wrapper](https://github.com/mikeym88/PatentsView-API-Wrapper)
 - [USPTO Scrapy Scraper](https://github.com/blazers08/USPTO)
 
+
```

### Comparing `patent_client-5.0.0/patent_client/__init__.py` & `patent_client-5.0.1/patent_client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,16 +45,18 @@
 handler.setFormatter(
     logging.Formatter("%(asctime)s:%(levelname)s:%(name)s:%(message)s")
 )
 logger.addHandler(handler)
 
 logger.info(f"Starting Patent Client with log level {SETTINGS.log_level}")
 
-
-from ._sync import *
+try:
+    from ._sync import *
+except ImportError:
+    pass
 
 elapsed = time.time() - start
 logger.info(f"Startup Complete!, took {elapsed:.3f} seconds")
 
 cache_dir = Path("~/.patent_client/cache").expanduser()
 cache_dir.parent.mkdir(exist_ok=True, parents=True)
```

### Comparing `patent_client-5.0.0/patent_client/_async/__init__.py` & `patent_client-5.0.1/patent_client/_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+from . import odp
 from .epo.ops.published.model import Inpadoc
 from .uspto.assignment.model import Assignment
 from .uspto.global_dossier.model import GlobalDossier, GlobalDossierApplication
 from .uspto.peds.model import USApplication
 from .uspto.ptab.model import PtabDecision, PtabDocument, PtabProceeding
 from .uspto.public_search.model import (
     Patent,
     PatentBiblio,
     PublicSearchBiblio,
     PublicSearchDocument,
     PublishedApplication,
     PublishedApplicationBiblio,
 )
 
-from . import odp
-    
-
 __all__ = [
     "Inpadoc",
     "Assignment",
     "USApplication",
     "PtabDecision",
     "PtabDocument",
     "PtabProceeding",
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/model.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/model_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/schema.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/family/schema_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/model.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/national_codes.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/national_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,23 +139,29 @@
         "INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows
     )
     con.commit()
 
 
 class LegalCodes:
     def __init__(self):
+        self.initialized = False
+
+    def initialize(self):
         if not code_database_current:
             logger.info(
                 "Legal Code Database is out of date - creating legal code database. Note this only happens once!"
             )
             asyncio.run(generate_legal_code_db())
         self.connection = sqlite3.connect(db_location, timeout=30)
         self.connection.row_factory = sqlite3.Row
+        self.initialized = True
 
     def get_code_data(self, country_code, legal_code):
+        if not self.initialized:
+            self.initialize()
         cur = self.connection.cursor()
         try:
             return dict(
                 cur.execute(
                     "SELECT * FROM legal_codes WHERE country_code = ? AND event_code = ?",
                     (country_code, legal_code),
                 ).fetchone()
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/legal/schema_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..session import asession
+from ..session import session
 from .model import NumberServiceResult
 
 
 class NumberServiceException(Exception):
     pass
 
 
@@ -25,15 +25,15 @@
             JP.2006147056.A.20060526
             US.(08/921,321).A.19970829
         doc_type: type of document (publication / application / priority)
         input_format: input type (original / docdb / epodoc)
         output_format: output type (original / docdb / epodoc)
 
         """
-        response = await asession.get(
+        response = await session.get(
             f"http://ops.epo.org/3.2/rest-services/number-service/{doc_type}/{input_format}/{number}/{output_format}",
             extensions={"force_cache": True},
         )
         result = NumberServiceResult.model_validate(response.text)
         errors = [m for m in result.messages if m["kind"] == "ERROR"]
         if errors:
             raise NumberServiceException("\n".join(str(e) for e in errors))
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/api_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/errors.txt` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/messages.txt` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/model.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/number_service/schema.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/api.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from io import BytesIO
 
 from yankee.data import AttrDict
 
-from ..session import asession
+from ..session import session
 from .model.biblio import BiblioResult
 from .model.fulltext import Claims, Description
 from .model.images import Images
 from .model.search import Search
 
 logger = logging.getLogger(__name__)
 
 
-class PublishedBiblioAsyncApi:
+class PublishedBiblioApi:
     @classmethod
     async def get_constituents(
         cls, number, doc_type="publication", format="docdb", constituents=("biblio",)
     ):
         """Published Data Constituents API
         number: document number to search
         doc_type: document type (application / publication)
@@ -24,15 +24,15 @@
         constituents: what data to retrieve. Can be combined. (biblio / abstract / full-cycle)
 
         """
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
         if isinstance(constituents, str):
             constituents = (constituents,)
         url = base_url + ",".join(constituents)
-        response = await asession.get(url)
+        response = await session.get(url)
         return response.text
 
     @classmethod
     async def get_biblio(
         cls, number, doc_type="publication", format="docdb"
     ) -> "BiblioResult":
         text = await cls.get_constituents(
@@ -49,15 +49,15 @@
     @classmethod
     async def get_full_cycle(cls, number, doc_type="publication", format="docdb"):
         return await cls.get_constituents(
             number, doc_type, format, constituents="full-cycle"
         )
 
 
-class PublishedFulltextAsyncApi:
+class PublishedFulltextApi:
     fulltext_jurisdictions = "EP, WO, AT, BE, BG, CA, CH, CY, CZ, DK, EE, ES, FR, GB, GR, HR, IE, IT, LT, LU, MC, MD, ME, NO, PL, PT, RO, RS, SE, SK".split(
         ", "
     )
 
     @classmethod
     async def get_fulltext_result(
         cls, number, doc_type="publication", format="docdb", inquiry="fulltext"
@@ -70,15 +70,15 @@
 
         """
         url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/{inquiry}"
         if number[:2] not in cls.fulltext_jurisdictions:
             raise ValueError(
                 f"Fulltext Is Not Available For Country Code {number[:2]}. Fulltext is only available in {', '.join(cls.fulltext_jurisdictions)}"
             )
-        response = await asession.get(url)
+        response = await session.get(url)
         response.raise_for_status
         return response.text
 
     @classmethod
     async def get_description(cls, number, doc_type="publication", format="docdb"):
         text = await cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="description"
@@ -91,63 +91,61 @@
     ) -> "Claims":
         text = await cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="claims"
         )
         return Claims.model_validate(text)
 
 
-class PublishedSearchAsyncApi:
+class PublishedSearchApi:
     @classmethod
     async def search(cls, query, start=1, end=100):
         base_url = "http://ops.epo.org/3.2/rest-services/published-data/search"
         range = f"{start}-{end}"
         logger.debug(f"OPS Search Endpoint - Query: {query}\nRange: {start}-{end}")
-        response = await asession.get(base_url, params={"Range": range, "q": query})
+        response = await session.get(base_url, params={"Range": range, "q": query})
         if response.status_code == 404:
             return AttrDict.convert(
                 {
                     "query": "query",
                     "num_results": 0,
                     "begin": start,
                     "end": end,
                     "results": list(),
                 }
             )
 
         return Search.model_validate(response.text)
 
 
-class PublishedImagesAsyncApi:
+class PublishedImagesApi:
     @classmethod
     async def get_images(cls, number, doc_type="publication", format="docdb"):
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/images"
-        response = await asession.get(base_url)
+        response = await session.get(base_url)
         return Images.model_validate(response.text)
 
     @classmethod
     async def get_page_image(
         cls, country, number, kind, image_type, page_number, image_format="pdf"
     ):
-        response = await asession.get(
+        response = await session.get(
             f"https://ops.epo.org/3.2/rest-services/published-data/images/{country}/{number}/{kind}/{image_type}.{image_format}",
             params={"Range": page_number},
-            stream=True,
             extensions={"force_cache": True},
         )
-        return BytesIO(response.raw.read())
+        return BytesIO(response.content)
 
     @classmethod
     async def get_page_image_from_link(cls, link, page_number, image_format="pdf"):
-        response = await asession.get(
+        response = await session.get(
             f"https://ops.epo.org/3.2/rest-services/{link}.{image_format}",
             params={"Range": page_number},
-            stream=True,
             extensions={"force_cache": True},
         )
-        return BytesIO(response.raw.read())
+        return BytesIO(response.content)
 
 
-class PublishedAsyncApi:
-    biblio = PublishedBiblioAsyncApi
-    fulltext = PublishedFulltextAsyncApi
-    search = PublishedSearchAsyncApi
-    images = PublishedImagesAsyncApi
+class PublishedApi:
+    biblio = PublishedBiblioApi
+    fulltext = PublishedFulltextApi
+    search = PublishedSearchApi
+    images = PublishedImagesApi
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/api_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,70 @@
 import json
 from pathlib import Path
 
 import pytest
 
-from .api import PublishedAsyncApi
+from .api import PublishedApi
 
 fixture_dir = Path(__file__).parent / "fixtures"
 
 
-class TestPublishedBiblioAsyncApi:
+class TestPublishedBiblioApi:
     @pytest.mark.asyncio
     async def test_doc_example_biblio(self):
-        result = await PublishedAsyncApi.biblio.get_biblio(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = await PublishedApi.biblio.get_biblio("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_biblio_result.json"
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_full_cycle(self):
-        result = await PublishedAsyncApi.biblio.get_full_cycle(
+        result = await PublishedApi.biblio.get_full_cycle(
             "EP1000000.A1", format="epodoc"
         )
         expected_file = fixture_dir / "ep1000000_full_cycle_result.xml"
         expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
     @pytest.mark.asyncio
     async def test_doc_example_abstract(self):
-        result = await PublishedAsyncApi.biblio.get_abstract(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = await PublishedApi.biblio.get_abstract("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_abstract_result.xml"
         # expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
 
 class TestSearchApi:
     @pytest.mark.asyncio
     async def test_search(self):
-        result = await PublishedAsyncApi.search.search("ti=plastic")
+        result = await PublishedApi.search.search("ti=plastic")
         expected_file = fixture_dir / "search_result.xml"
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
 
 class TestFullTextAsyncApi:
     @pytest.mark.asyncio
     async def test_description(self):
-        result = await PublishedAsyncApi.fulltext.get_description(
+        result = await PublishedApi.fulltext.get_description(
             "EP1000000.A1", format="epodoc"
         )
         expected_file = fixture_dir / "ep1000000_description_result.xml"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
     @pytest.mark.asyncio
     async def test_claims(self):
-        result = await PublishedAsyncApi.fulltext.get_claims(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = await PublishedApi.fulltext.get_claims("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_claims_result.json"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/cql.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957142857142858%*

 * *Differences: {"'documents'": "{0: {'cpc_class': {insert: [(2, 'B28B 5/025')], delete: [2, 0]}}}"}*

```diff
@@ -109,17 +109,16 @@
                     },
                     "original": null
                 }
             ],
             "country": "EP",
             "cpc_class": [
                 "B28B 1/29",
-                "B28B 1/29",
-                "B28B 5/022",
                 "B28B 5/022",
+                "B28B 5/025",
                 "B28B 7/0064",
                 "B28B 7/0064"
             ],
             "doc_number": "1000000",
             "docdb_number": "EP1000000.A1",
             "family_id": "19768124",
             "intl_class": [
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/manager.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 from patent_client.util.manager import AsyncManager
 
-from .api import PublishedAsyncApi
+from .api import PublishedApi
 from .cql import generate_query
 from .model.biblio import BiblioResult
 from .model.fulltext import Claims, Description
 from .model.images import ImageDocument
 
 
 def get_ranges(limit=None, offset=0, page_size=100):
@@ -34,15 +34,15 @@
     primary_key = "publication"
 
     async def _get_search_results_range(self, start=1, end=100):
         if "cql_query" in self.config.filter:
             query = self.config.filter["cql_query"]
         else:
             query = generate_query(**self.config.filter)
-        return await PublishedAsyncApi.search.search(query, start, end)
+        return await PublishedApi.search.search(query, start, end)
 
     async def count(self) -> int:
         page = await self._get_search_results_range(1, 100)
         offset = self.config.offset or 0
         limit = self.config.limit or page.num_results - offset
         num_results = page.num_results
         num_results -= offset
@@ -56,41 +56,41 @@
             page = await self._get_search_results_range(start, end)
             for result in page.results:
                 yield result
             if len(page.results) < self.result_size:
                 break
 
     async def get(self, number, doc_type="publication", format="docdb") -> BiblioResult:
-        result = await PublishedAsyncApi.biblio.get_biblio(number, doc_type, format)
+        result = await PublishedApi.biblio.get_biblio(number, doc_type, format)
         if len(result.documents) > 1:
             raise Exception("More than one result found! Try another query")
         return result.documents[0]
 
 
 class BiblioManager(AsyncManager):
     async def get(self, doc_number) -> "BiblioResult":
-        result = await PublishedAsyncApi.biblio.get_biblio(doc_number)
+        result = await PublishedApi.biblio.get_biblio(doc_number)
         if len(result.documents) > 1:
             raise ValueError(f"More than one result found for {doc_number}!")
         return result.documents[0]
 
 
 class ClaimsManager(AsyncManager):
     async def get(self, doc_number) -> "Claims":
-        return await PublishedAsyncApi.fulltext.get_claims(doc_number)
+        return await PublishedApi.fulltext.get_claims(doc_number)
 
 
 class DescriptionManager(AsyncManager):
     async def get(self, doc_number) -> Description:
-        return await PublishedAsyncApi.fulltext.get_description(doc_number)
+        return await PublishedApi.fulltext.get_description(doc_number)
 
 
 class ImagesManager(AsyncManager):
     async def get(self, doc_number) -> ImageDocument:
-        return await PublishedAsyncApi.images.get_images(doc_number)
+        return await PublishedApi.images.get_images(doc_number)
 
 
 class InpadocManager(SearchManager):
     pass
 
 
 class InpadocBiblioManager(BiblioManager):
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/manager_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/manager_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,7 +58,13 @@
         assert biblio.intl_class is not None
 
     @pytest.mark.asyncio
     async def test_issue_41(self):
         result = await Inpadoc.objects.get("JP2005533465A")
         biblio = await result.biblio
         assert biblio.title is None
+
+    @pytest.mark.asyncio
+    async def test_document_downloading(self, tmpdir):
+        result = await Inpadoc.objects.get("WO2010050748A2")
+        await result.download(tmpdir)
+        assert len(tmpdir.listdir()) > 0
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/biblio.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/fulltext.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/images.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/images.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,40 +17,40 @@
     num_pages: Optional[int] = None
     description: Optional[str] = None
     link: Optional[str] = None
     formats: List[str] = Field(default_factory=list)
     sections: List[Section] = Field(default_factory=list)
     doc_number: Optional[str] = None
 
-    def download(self, path="."):
+    async def download(self, path="."):
         from ..api import PublishedImagesApi
 
         out_file = Path(path) / f"{self.doc_number}.pdf"
         writer = PdfWriter()
         for i in range(1, self.num_pages + 1):
-            page_data = PublishedImagesApi.get_page_image_from_link(
+            page_data = await PublishedImagesApi.get_page_image_from_link(
                 self.link, page_number=i
             )
             page = PdfReader(page_data).pages[0]
             if page["/Rotate"] == 90:
                 page.rotate_clockwise(-90)
             writer.add_page(page)
 
         for section in self.sections:
             writer.add_outline_item(section.name.capitalize(), section.start_page)
 
         with out_file.open("wb") as f:
             writer.write(f)
 
-    def download_image(self, path=".", image_format="tif", page_number=1):
+    async def download_image(self, path=".", image_format="tif", page_number=1):
         from ..api import PublishedImagesApi
 
         out_file = Path(path) / f"{self.doc_number}.{image_format}"
 
-        image = PublishedImagesApi.get_page_image_from_link(
+        image = await PublishedImagesApi.get_page_image_from_link(
             self.link, page_number=page_number, image_format=image_format
         )
 
         with out_file.open("wb") as f:
             f.write(image.read())
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/model/search.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/biblio.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/images.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema/search.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/schema_test.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/description_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/full_cycle_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/image_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/published/test/search_example.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/session.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import base64
 import datetime as dt
+import logging
 from typing import Sequence
 
 import hishel
 import httpx
 from httpcore import Request, Response
 
 from patent_client import SETTINGS
 from patent_client._async.http_client import PatentClientSession
 from patent_client.session import CACHE_DIR
 
-import logging
-
 logger = logging.getLogger(__name__)
 
 NS = {
     "http://ops.epo.org": None,
     "http://www.epo.org/exchange": None,
     "http://www.epo.org/fulltext": None,
     "http://www.epo.org/register": None,
 }
 
 
-
-
 class OpsAuthenticationError(Exception):
     pass
 
 
 class OpsForbiddenError(Exception):
     pass
 
@@ -107,15 +104,15 @@
 
 async def handle_response(response):
     if response.status_code == 403:
         raise OpsForbiddenError("Forbidden")
     return response
 
 
-asession = PatentClientSession(
+session = PatentClientSession(
     transport=ops_transport,
     auth=OpsAuth(key=SETTINGS.epo_api_key, secret=SETTINGS.epo_api_secret),
     event_hooks={
         "response": [
             handle_response,
         ]
     },
```

### Comparing `patent_client-5.0.0/patent_client/_async/epo/ops/util.py` & `patent_client-5.0.1/patent_client/_async/epo/ops/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,7 +82,11 @@
         self,
     ) -> List["FamilyMember"]:
         return (
             await self._get_model(
                 ".family.model.Family", base_class=InpadocModel
             ).objects.get(self.docdb_number)
         ).family_members
+
+    async def download(self, path: str = "."):
+        images = await self.images
+        return await images.full_document.download(path)
```

### Comparing `patent_client-5.0.0/patent_client/_async/http_client.py` & `patent_client-5.0.1/patent_client/_async/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-from typing import Optional
+import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -63,15 +63,15 @@
             path = path / filename if path else Path.cwd() / filename
         return path
 
     async def download(
         self,
         url,
         method: str = "GET",
-        path: Optional[str | Path] = None,
+        path: tp.Optional[tp.Union[str, Path]] = None,
         **kwargs,
     ):
         # Ensure we skip the cache for file downloads
         kwargs["extensions"] = kwargs.get("extensions", dict())
         if "force_cache" in kwargs["extensions"]:
             raise ValueError("force_cache is not supported for file downloads")
         kwargs["extensions"]["cache_disabled"] = True
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 
-import httpx
 import pytest
 
 from .api import AssignmentApi
 
 
 @pytest.mark.asyncio
 async def test_alookup():
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/convert.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/convert_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
 from .api import AssignmentApi
 from .model import Assignment
 
 warnings.filterwarnings("ignore", category=InsecureRequestWarning)
 
 NUMBER_CLEAN_RE = re.compile(r"[^\d]")
-clean_number = lambda x: NUMBER_CLEAN_RE.sub("", str(x))
+
+
+def clean_number(x):
+    return NUMBER_CLEAN_RE.sub("", str(x))
 
 
 logger = logging.getLogger(__name__)
 
 
 class AssignmentManager(AsyncManager["Assignment"]):
     fields = {
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/manager_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         assert len(a.properties) == 5
         assert (
             a.properties[0].invention_title
             == "SYSTEM AND METHODS FOR ACCELERATED DATA STORAGE AND RETRIEVAL"
         )
         assert a.properties[0].appl_num == "10628795"
         assert a.properties[0].filing_date.isoformat() == "2003-07-28"
-        assert a.properties[0].intl_publ_date == None
-        assert a.properties[0].intl_reg_num == None
+        assert a.properties[0].intl_publ_date is None
+        assert a.properties[0].intl_reg_num is None
         assert a.properties[0].inventors == "James J. Fallon"
         assert a.properties[0].issue_date.isoformat() == "2006-10-31"
         assert a.properties[0].pat_num == "7130913"
-        assert a.properties[0].pct_num == None
+        assert a.properties[0].pct_num is None
         assert a.properties[0].publ_date.isoformat() == "2004-04-15"
         assert a.properties[0].publ_num == "20040073746"
 
     @pytest.mark.asyncio
     async def test_fetch_assignments_by_assignee(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
         assert await assignments.count() >= 22
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+import typing as tp
 
 from dateutil.parser import isoparse
 from pydantic import BeforeValidator, ConfigDict, Field, field_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from ..peds.model import USApplication
     from ..public_search.model import Patent, PublishedApplication
 
 UsptoDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%Y%m%d").date()),
 ]
@@ -32,15 +32,15 @@
     dt = parse_datetime(string)
     if dt is None:
         return None
     return dt.date()
 
 
 DatetimeAsDate = Annotated[
-    Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
+    tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
 ]
 
 
 class AbstractAssignmentModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
@@ -58,26 +58,26 @@
     address: str = Field(alias="patAssigneeAddress")
 
 
 class Property(AbstractAssignmentModel):
     invention_title: str
     invention_title_lang: str
     appl_num: str
-    filing_date: Optional[DatetimeAsDate] = None
-    intl_publ_date: Optional[DatetimeAsDate] = None
-    intl_reg_num: Optional[str] = None
-    inventors: Optional[str] = None
-    issue_date: Optional[DatetimeAsDate] = None
-    pat_num: Optional[str] = None
-    pct_num: Optional[str] = None
-    publ_date: Optional[DatetimeAsDate] = None
-    publ_num: Optional[str] = None
+    filing_date: tp.Optional[DatetimeAsDate] = None
+    intl_publ_date: tp.Optional[DatetimeAsDate] = None
+    intl_reg_num: tp.Optional[str] = None
+    inventors: tp.Optional[str] = None
+    issue_date: tp.Optional[DatetimeAsDate] = None
+    pat_num: tp.Optional[str] = None
+    pct_num: tp.Optional[str] = None
+    publ_date: tp.Optional[DatetimeAsDate] = None
+    publ_num: tp.Optional[str] = None
 
     @property
-    def application(self) -> Optional["USApplication"]:
+    def application(self) -> tp.Optional["USApplication"]:
         """The related US Application"""
         try:
             appl_id = getattr(self, "appl_id", None)
             if appl_id is not None:
                 return self._get_model(
                     "patent_client.uspto.peds.model.USApplication"
                 ).objects.get(appl_id=appl_id)
@@ -121,29 +121,29 @@
 class Correspondent(AbstractAssignmentModel):
     name: str
     address: str
 
 
 class Assignment(AbstractAssignmentModel["AssignmentManager"]):
     id: str
-    date_produced: Optional[UsptoDate] = None
-    action_key_code: Optional[str] = None
-    transaction_date: Optional[DatetimeAsDate] = None
+    date_produced: tp.Optional[UsptoDate] = None
+    action_key_code: tp.Optional[str] = None
+    transaction_date: tp.Optional[DatetimeAsDate] = None
     last_update_date: DatetimeAsDate
     purge_indicator: YNBool
     recorded_date: DatetimeAsDate
     page_count: int
     conveyance_text: str
     assignment_record_has_images: YNBool
-    attorney_dock_num: Optional[str] = None
+    attorney_dock_num: tp.Optional[str] = None
     pat_assignor_earliest_ex_date: DatetimeAsDate
     correspondent: Correspondent
-    assignors: List[Assignor]
-    assignees: List[Assignee]
-    properties: List[Property]
+    assignors: tp.List[Assignor]
+    assignees: tp.List[Assignee]
+    properties: tp.List[Property]
 
     @field_validator("conveyance_text")
     @classmethod
     def remove_see_document(cls, v) -> str:
         return v.replace(" (SEE DOCUMENT FOR DETAILS).", "").strip()
 
     @property
@@ -153,15 +153,15 @@
     @property
     def image_url(self):
         reel, frame = self.reel_frame
         reel = reel.rjust(6, "0")
         frame = frame.rjust(4, "0")
         return f"http://legacy-assignments.uspto.gov/assignments/assignment-pat-{reel}-{frame}.pdf"
 
-    async def download(self, path: Optional[str | Path] = None):
+    async def download(self, path: tp.Optional[tp.Union[str, Path]] = None):
         """asynchronously downloads the PDF associated with the assignment to the current working directory"""
         from .api import client
 
         return await client.download(self.image_url, path=path)
 
 
 class AssignmentPage(AbstractAssignmentModel):
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/assignment/model_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         )
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     async def get_by_short_name(
         cls,
         product_name: str,
-        from_date: tp.Optional[datetime.date | str] = None,
-        to_date: tp.Optional[datetime.date | str] = None,
+        from_date: tp.Optional[tp.Union[datetime.date, str]] = None,
+        to_date: tp.Optional[tp.Union[datetime.date, str]] = None,
         max_files: int = 20,
     ) -> tp.List[Product]:
         """Returns files associated with products (of level PRODUCT) based on their full or partial names."""
         params = dict()
         if from_date:
             if isinstance(from_date, str):
                 from_date = datetime.date.fromisoformat(from_date)
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/bulk_data/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/bulk_data/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     size: int = Field(alias="fileSize")
     download_url: str = Field(alias="fileDownloadUrl")
     from_date: datetime.date = Field(alias="fileFromTime")
     to_date: datetime.date = Field(alias="fileToTime")
     type: str = Field(alias="fileType")
     release_date: datetime.date = Field(alias="fileReleaseDate")
 
-    async def download(self, path: tp.Optional[str | Path]):
+    async def download(self, path: tp.Optional[tp.Union[str, Path]]):
         from .api import client
 
         return await client.download(self.download_url, path=path)
 
 
 class Product(BaseModel):
     link_path: str = Field(alias="productLinkPath")
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from pydantic import BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
 if tp.TYPE_CHECKING:
+    from ..assignment.model import Assignment
     from ..peds.model import USApplication
     from ..public_search.model import Patent, PublishedApplication
-    from ..assignment.model import Assignment
 
 MDYDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m/%d/%Y").date()),
 ]
 OptionalStrList = Annotated[
     tp.List[str], BeforeValidator(lambda x: x if isinstance(x, list) else list())
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/model_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/query_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app.json` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.1/patent_client/_async/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing as tp
 
 from patent_client import SETTINGS
-from ...http_client import PatentClientSession
 
+from ...http_client import PatentClientSession
 from .model import (
     Assignment,
     Continuity,
     CustomerNumber,
     Document,
     ForeignPriority,
     SearchGetRequest,
@@ -19,17 +19,15 @@
 from .util import prune
 
 
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
-        self.client = PatentClientSession(
-            headers={"X-API-KEY": SETTINGS.odp_api_key}
-        )
+        self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
 
     async def post_search(
         self, search_request: SearchRequest = SearchRequest()
     ) -> tp.Dict:
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = await self.client.post(
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/application.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/documents.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/search.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.1/patent_client/_async/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from .api import ODPApi
 from .model import SearchRequest, USApplication, USApplicationBiblio
 from .query import create_post_search_obj
 
 if tp.TYPE_CHECKING:
     from .model import (
+        Assignment,
         Continuity,
+        CustomerNumber,
         Document,
+        ForeignPriority,
         SearchResult,
+        TermAdjustment,
+        Transaction,
         USApplication,
         USApplicationBiblio,
-        TermAdjustment,
-        Assignment,
-        CustomerNumber,
-        ForeignPriority,
-        Transaction
     )
 
 
 api = ODPApi()
 
 
 class USApplicationManager(AsyncManager):
@@ -103,47 +103,53 @@
 
     async def count(self):
         return len(await api.get_documents(self.config.filter["appl_id"][0]))
 
     async def _get_results(self) -> tp.AsyncIterator["Document"]:
         for doc in await api.get_documents(self.config.filter["appl_id"][0]):
             yield doc
-            
+
+
 class TermAdjustmentManager(AsyncManager):
     default_filter = "appl_id"
-    
+
     async def _get_results(self) -> "TermAdjustment":
         return await api.get_term_adjustments(self.config.filter["appl_id"][0])
-    
+
+
 class AssignmentManager(AsyncManager):
     default_filter = "appl_id"
-    
+
     async def _get_results(self) -> tp.AsyncIterator["Assignment"]:
         for doc in await api.get_assignments(self.config.filter["appl_id"][0]):
             yield doc
-    
+
     async def count(self):
         return len(await api.get_assignments(self.config.filter["appl_id"][0]))
-    
+
+
 class CustomerNumberManager(AsyncManager):
     default_filter = "appl_id"
-    
+
     async def _get_results(self) -> "CustomerNumber":
         return await api.get_customer_numbers(self.config.filter["appl_id"][0])
-    
+
+
 class ForeignPriorityManager(AsyncManager):
     default_filter = "appl_id"
-    
+
     async def _get_results(self) -> "ForeignPriority":
-        for doc in await api.get_foreign_priority_data(self.config.filter["appl_id"][0]):
+        for doc in await api.get_foreign_priority_data(
+            self.config.filter["appl_id"][0]
+        ):
             yield doc
-    
+
+
 class TransactionManager(AsyncManager):
     default_filter = "appl_id"
-    
+
     async def _get_results(self) -> tp.AsyncIterator["Transaction"]:
         for doc in await api.get_transactions(self.config.filter["appl_id"][0]):
             yield doc
-    
+
     async def count(self):
         return len(await api.get_transactions(self.config.filter["appl_id"][0]))
-
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/manager_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from .manager import USApplicationManager, USApplicationBiblioManager
+from .manager import USApplicationBiblioManager, USApplicationManager
 
 
 @pytest.mark.asyncio
 async def test_all_apps():
     manager = USApplicationManager().filter(query=dict())
     assert await manager.count() > 1000
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,28 @@
     appl_id: str = Field(alias="applicationNumberText")
     mail_date: datetime.datetime = Field(alias="officialDate")
     document_identifier: str = Field(alias="documentIdentifier")
     document_code: str = Field(alias="documentCode")
     document_code_description: str = Field(alias="documentCodeDescriptionText")
     direction_category: str = Field(alias="directionCategory")
     download_option_bag: list[dict] = Field(alias="downloadOptionBag")
-    
+
     async def download(self, type="PDF", out_path=None):
         from .manager import api
+
         try:
-            url = next(u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type)["downloadUrl"]
+            url = next(
+                u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type
+            )["downloadUrl"]
         except StopIteration:
             raise ValueError(f"No download URL found for this document type: {type}")
         if out_path is None:
-            out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace("/", "-")
+            out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace(
+                "/", "-"
+            )
         return await api.client.download(url, "GET", path=out_path)
 
 
 # Assignment
 
 
 class Assignor(BaseODPModel):
@@ -277,34 +282,42 @@
         return await self._get_model(".model.Continuity").objects.get(
             appl_id=self.appl_id
         )
 
     @async_property
     async def documents(self) -> list[Document]:
         return self._get_model(".model.Document").objects.filter(appl_id=self.appl_id)
-    
+
     @async_property
     async def term_adjustment(self) -> TermAdjustment:
-        return self._get_model(".model.TermAdjustment").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.TermAdjustment").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @async_property
     async def assignments(self) -> list[Assignment]:
         return self._get_model(".model.Assignment").objects.filter(appl_id=self.appl_id)
-    
+
     @async_property
     async def customer_number(self) -> CustomerNumber:
-        return self._get_model(".model.CustomerNumber").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.CustomerNumber").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @async_property
     async def foreign_priority(self) -> ForeignPriority:
-        return self._get_model(".model.ForeignPriority").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.ForeignPriority").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @async_property
     async def transactions(self) -> list[Transaction]:
-        return self._get_model(".model.Transaction").objects.filter(appl_id=self.appl_id)
+        return self._get_model(".model.Transaction").objects.filter(
+            appl_id=self.appl_id
+        )
 
     # Aliases
 
     @async_property
     async def biblio(self) -> "USApplicationBiblio":
         return await self.bibliographic_data
 
@@ -329,16 +342,15 @@
     atty_docket_num: str = Field(alias="docketNumber")
     appl_id: str = Field(alias="applicationNumberText")
     first_inventor_name: str = Field(alias="firstInventorName")
     first_applicant_name: str = Field(alias="firstApplicantName")
     cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
     entity_status: str = Field(alias="businessEntityStatusCategory")
     app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
-    
-    
+
     app_type_code: str = Field(alias="applicationTypeCode")
     national_stage_indicator: YNBool = Field(alias="nationalStageIndicator")
 
     effective_filing_date: datetime.date = Field(alias="effectiveFilingDate")
     cls_sub_cls: str = Field(alias="class/subclass")
     assignments: list[Assignment] = Field(alias="assignmentBag")
     attorneys: CustomerNumber = Field(alias="recordAttorney")
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/model_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/query.py` & `patent_client-5.0.1/patent_client/_async/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/odp/query_fields.csv` & `patent_client-5.0.1/patent_client/_async/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.1/patent_client/_async/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import datetime
 import logging
 from collections.abc import Sequence
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, AsyncIterator
+import typing as tp
 
 from dateutil.parser import parse as dt_parse
 from pypdf import PdfMerger
 
 from patent_client.util.manager import AsyncManager
 from patent_client.util.request_util import get_start_and_row_count
 
 from .api import PatentExaminationDataSystemApi
 from .query import QueryFields
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from .model import Document, USApplication
 
 logger = logging.getLogger(__name__)
 
 
 class HttpException(Exception):
     pass
 
 
 def cast_as_datetime(
-    date: str | datetime.datetime | datetime.date, end_of_day=False
+    date: tp.Union[str, datetime.datetime, datetime.date], end_of_day=False
 ) -> datetime.datetime:
     if isinstance(date, datetime.datetime):
         pass
     elif isinstance(date, str):
         date = dt_parse(date)
     elif isinstance(date, datetime.date):
         date = datetime.datetime.combine(date, datetime.datetime.min.time())
@@ -50,25 +50,29 @@
     default_filter = "appl_id"
 
     async def count(self):
         api = PatentExaminationDataSystemApi()
         max_length = (await api.create_query(**self.get_query_params())).num_found
         return min(max_length, self.config.limit) if self.config.limit else max_length
 
-    async def _get_results(self) -> AsyncIterator["USApplication"]:
+    async def _get_results(self) -> tp.AsyncIterator["USApplication"]:
         query_params = self.get_query_params()
         api = PatentExaminationDataSystemApi()
+        counter = 0
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, page_size=20
         ):
             page = await api.create_query(
                 **{**query_params, "start": start, "rows": rows}
             )
             for app in page.applications:
                 yield app
+                counter += 1
+                if self.config.limit and counter >= self.config.limit:
+                    break
             if len(page.applications) < rows:
                 break
 
     def get_query_params(self):
         # Short circuit processing logic if the "query" filter is specified
         if "query" in self.config.filter:
             query_text = self.config.filter["query"]
@@ -186,15 +190,15 @@
 
 class DocumentManager(AsyncManager["Document"]):
     default_filter = "appl_id"
 
     async def count(self):
         return len([i async for i in self])
 
-    async def _get_results(self) -> AsyncIterator["Document"]:
+    async def _get_results(self) -> tp.AsyncIterator["Document"]:
         api = PatentExaminationDataSystemApi()
         docs = await api.get_documents(self.config.filter["appl_id"][0])
         for doc in docs:
             yield doc
 
     async def download(self, docs, path="."):
         if str(path)[-4:].lower() == ".pdf":
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/manager_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from collections import OrderedDict
 from pathlib import Path
 
 import pytest
 from pypdf import PdfReader
 
-from .model import PedsPage, USApplication
+from .model import PedsPage, USApplication, RemovedDataException
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
 class TestPatentExaminationDataDeserialization:
     def test_application(self):
         input_file = fixtures / "app_1_input.json"
@@ -90,37 +90,41 @@
             "US20050120054A1",
             "US20050188423A1",
         ]
         data = USApplication.objects.filter(app_early_pub_number=nos)
         assert await data.count() == 5
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("Continuity information has been removed from PEDS")
     async def test_get_child_data(self):
         parent = await USApplication.objects.get("14018930")
         child = parent.child_continuity[0]
         assert child.child_appl_id == "14919159"
         assert child.relationship == "claims the benefit of"
         # assert child.child.patent_title == "LEAPFROG TREE-JOIN"
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("Continuity information has been removed from PEDS")
     async def test_get_parent_data(self):
         child = await USApplication.objects.get("14018930")
         parent = child.parent_continuity[0]
         assert parent.parent_appl_id == "61706484"
         assert parent.relationship == "Claims Priority from Provisional Application"
         assert parent.parent_app_filing_date is not None
         # assert parent.parent.patent_title == "Leapfrog Tree-Join"
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     async def test_pta_history(self):
         app = await USApplication.objects.get("14095073")
         pta_history = app.pta_pte_tran_history
         assert len(pta_history) > 10
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     async def test_pta_summary(self):
         app = await USApplication.objects.get("14095073")
         expected = OrderedDict(
             [
                 ("kind", "PTA"),
                 ("a_delay", 169),
                 ("pto_delay", 169),
@@ -146,14 +150,15 @@
             "corr_address",
         ]
 
         for k in expected_keys:
             assert getattr(app, k, None) is not None
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("Attorney information has been removed from PEDS")
     async def test_attorneys(self):
         app = await USApplication.objects.get("14095073")
         assert len(app.attorneys) > 1
         actual = app.attorneys[0].model_dump()
         assert int(actual["registration_no"]) > 1000
         expected_keys = [
             "registration_no",
@@ -172,14 +177,15 @@
             async for a in apps:
                 counter += 1
         except KeyError as e:
             raise e
         assert await apps.count() == counter
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     async def test_expiration_date(self):
         app = await USApplication.objects.get("15384723")
         expected = {
             "parent_appl_id": "12322218",
             "parent_app_filing_date": datetime.date(2009, 1, 29),
             "parent_relationship": "is a Continuation in part of",
             "initial_term": datetime.date(2029, 1, 29),
@@ -202,14 +208,15 @@
             "terminal_disclaimer_filed": False,
         }
         actual = dict(app.expiration)
         for k in expected.keys():
             assert expected[k] == actual[k]
 
     @pytest.mark.asyncio
+    @pytest.mark.skip("Expiration date is not supported for PCT applications")
     async def test_expiration_date_for_pct_apps(self):
         app = await USApplication.objects.get("PCT/US2014/020588")
         with pytest.raises(Exception) as exc:
             _ = app.expiration
         assert exc.match("Expiration date not supported for PCT Applications")
 
     @pytest.mark.asyncio
@@ -219,14 +226,35 @@
         assert isinstance(fp, list)
         app = fp[0]
         assert app.country_name == "NORWAY"
         assert app.filing_date == datetime.date(2017, 2, 15)
         assert app.priority_claim == "20170229"
 
 
+    @pytest.mark.asyncio
+    async def test_raises_warning_on_missing_information(self):
+        app = await USApplication.objects.get(patent_number=10000000)
+        with pytest.raises(RemovedDataException):
+            _ = app.expiration
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.attorneys
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.pta_pte_summary
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.pta_pte_tran_history
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.parent_continuity
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.child_continuity
+
 class TestDocuments:
     @pytest.mark.vcr
     async def test_can_get_document_listing(self):
         app = await USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         assert await docs.count() > 50
 
@@ -234,36 +262,9 @@
     async def test_can_get_application_from_document(self):
         app = await USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         doc = await docs[5]
         backref_app = await doc.application
         assert app.appl_id == backref_app.appl_id
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    async def test_can_download_document(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        doc = app.documents.to_list()[-1]
-        result = doc.download(path=tmp_path)
-        assert "14643719 - 2015-03-10 - IDS" in str(result)
-        assert result.exists()
-        assert len(list(tmp_path.glob("*.pdf"))) == 1
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    async def test_can_download_document_without_appl_id(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        doc = app.documents.to_list()[-1]
-        result = doc.download(path=tmp_path, include_appl_id=False)
-        assert "2015-03-10 - IDS" in str(result)
-        assert "14643719" not in str(result)
-        assert result.exists()
-        assert len(list(tmp_path.glob("*.pdf"))) == 1
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    async def test_multiple_document_download(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        docs = app.documents.to_list()[-2:]
-        result = app.documents.download(docs, path=tmp_path)
-        reader = PdfReader(str(result))
-        assert reader.numPages == 8
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, List, Optional
+import typing as tp
 
 from async_property import async_property
 from dateutil.relativedelta import relativedelta
 from pydantic import (
     AliasPath,
     BeforeValidator,
     ConfigDict,
@@ -13,30 +13,34 @@
     model_validator,
 )
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated, Self
 
 from patent_client.util.pydantic_util import BaseModel, Date, DateTime
 
-if TYPE_CHECKING:
-    from ..public_search.model import Patent, PublishedApplication
-    from ..ptab.model import PtabProceeding
+if tp.TYPE_CHECKING:
     from ...epo.ops.published.model import InpadocBiblio
+    from ..ptab.model import PtabProceeding
+    from ..public_search.model import Patent, PublishedApplication
 
 
 def parse_mdy_date(string: str) -> datetime.date:
     try:
         return datetime.datetime.strptime(string, "%m-%d-%Y").date()
     except ValueError:
         return None
 
 
-MDYDate = Annotated[Optional[datetime.date], BeforeValidator(parse_mdy_date)]
+class RemovedDataException(Exception):
+    pass
+
+
+MDYDate = Annotated[tp.Optional[datetime.date], BeforeValidator(parse_mdy_date)]
 YNBool = Annotated[bool, BeforeValidator(lambda x: x == "Y")]
-OptionalInt = Annotated[Optional[int], BeforeValidator(lambda x: int(x) if x else None)]
+OptionalInt = Annotated[tp.Optional[int], BeforeValidator(lambda x: int(x) if x else None)]
 RelationshipStr = Annotated[
     str, BeforeValidator(lambda x: x.replace("This application ", "").strip())
 ]
 ConveyanceStr = Annotated[
     str, BeforeValidator(lambda x: x.replace(" (SEE DOCUMENT FOR DETAILS).", ""))
 ]
 
@@ -50,62 +54,23 @@
 
 class Transactions(PEDSBaseModel):
     record_date: Date
     code: str
     description: str
 
 
-class PtaOrPteTransactionHistory(PEDSBaseModel):
-    number: float
-    pta_or_pte_date: MDYDate
-    contents_description: str
-    pto_days: OptionalInt
-    appl_days: OptionalInt
-    start: float
-
-
-class PtaOrPteSummary(PEDSBaseModel):
-    a_delay: int
-    b_delay: int
-    c_delay: int
-    pto_adjustments: int
-    total_days: int = Field(alias="totalPtoDays")
-    kind: str = Field(alias="ptaPteInd")
-    pto_delay: int
-    applicant_delay: int = Field(alias="applDelay")
-    overlap_delay: int
-
-
-class ParentApplication(PEDSBaseModel):
-    parent_appl_id: str = Field(alias="claimApplicationNumberText")
-    child_appl_id: str = Field(alias="applicationNumberText")
-    parent_app_filing_date: MDYDate = Field(alias="filingDate")
-    parent_patent_number: str = Field(alias="patentNumberText")
-    parent_status: str = Field(alias="applicationStatus")
-    relationship: RelationshipStr = Field(alias="applicationStatusDescription")
-
-
-class ChildApplication(PEDSBaseModel):
-    child_appl_id: str = Field(alias="claimApplicationNumberText")
-    parent_appl_id: str = Field(alias="applicationNumberText")
-    child_app_filing_date: MDYDate = Field(alias="filingDate")
-    child_patent_number: str = Field(alias="patentNumberText")
-    child_status: str = Field(alias="applicationStatus")
-    relationship: RelationshipStr = Field(alias="applicationStatusDescription")
-
-
 class ForeignPriority(PEDSBaseModel):
     priority_claim: str
     country_name: str
     filing_date: MDYDate
 
 
 class AttorneyOrAgent(PEDSBaseModel):
-    application_id: Optional[str] = None
-    registration_no: Optional[str] = None
+    application_id: tp.Optional[str] = None
+    registration_no: tp.Optional[str] = None
     full_name: str
     phone_num: str
     reg_status: str
 
 
 class Inventor(PEDSBaseModel):
     name: str
@@ -132,76 +97,97 @@
     correspondent_name: str = Field(alias="addressNameText")
     mail_date: MDYDate
     received_date: MDYDate
     recorded_date: MDYDate
     pages: OptionalInt = Field(alias="pagesCount", default=None)
     conveyance: ConveyanceStr = Field(alias="converyanceName")
     sequence_number: int
-    assignors: Optional[List[Assignor]] = Field(alias="assignors", default_factory=list)
-    assignees: Optional[List[Assignee]] = Field(alias="assignee", default_factory=list)
+    assignors: tp.Optional[tp.List[Assignor]] = Field(alias="assignors", default_factory=list)
+    assignees: tp.Optional[tp.List[Assignee]] = Field(alias="assignee", default_factory=list)
 
     @computed_field
     @property
     def reel_frame(self) -> str:
         return f"{self.reel_number}/{self.frame_number}"
 
 
 class USApplication(PEDSBaseModel):
     appl_id: str
     app_filing_date: Date
-    app_exam_name: Optional[str] = None
+    app_exam_name: tp.Optional[str] = None
     public_ind: YNBool
-    inventor_name: Optional[str] = None
-    app_early_pub_number: Optional[str] = None
-    app_early_pub_date: Optional[Date] = None
-    patent_number: Optional[str] = None
-    patent_issue_date: Optional[Date] = None
-    app_location: Optional[str] = None
-    app_grp_art_number: Optional[str] = None
+    inventor_name: tp.Optional[str] = None
+    app_early_pub_number: tp.Optional[str] = None
+    app_early_pub_date: tp.Optional[Date] = None
+    patent_number: tp.Optional[str] = None
+    patent_issue_date: tp.Optional[Date] = None
+    app_location: tp.Optional[str] = None
+    app_grp_art_number: tp.Optional[str] = None
     last_modified: DateTime = Field(alias="LAST_MOD_TS")
     last_insert_time: DateTime = Field(alias="LAST_INSERT_TIME")
-    patent_title: Optional[str] = None
-
-    app_attr_dock_number: Optional[str] = None
-    app_status: Optional[str] = None
-    app_status_date: Optional[Date] = None
-    app_type: Optional[str] = None
-    app_cls_sub_cls: Optional[str] = None
-    corr_name: Optional[str] = None
-    corr_address: Optional[str] = None
-    corr_cust_no: Optional[str] = Field(alias="corrAddrCustNo", default=None)
-    transactions: List[Transactions]
-    attorneys: List[AttorneyOrAgent] = Field(alias="attrnyAddr", default_factory=list)
-    inventors: List[Inventor] = Field(default_factory=list)
-    applicants: List[Applicant] = Field(default_factory=list)
-    pta_pte_summary: Optional[PtaOrPteSummary] = None
-    pta_pte_tran_history: List[PtaOrPteTransactionHistory] = Field(default_factory=list)
-    parent_continuity: List[ParentApplication] = Field(default_factory=list)
-    child_continuity: List[ChildApplication] = Field(default_factory=list)
-    foreign_priority: List[ForeignPriority] = Field(default_factory=list)
-    assignments: List[Assignment] = Field(default_factory=list)
+    patent_title: tp.Optional[str] = None
+    app_attr_dock_number: tp.Optional[str] = None
+    app_status: tp.Optional[str] = None
+    app_status_date: tp.Optional[Date] = None
+    app_type: tp.Optional[str] = None
+    app_cls_sub_cls: tp.Optional[str] = None
+    corr_name: tp.Optional[str] = None
+    corr_address: tp.Optional[str] = None
+    corr_cust_no: tp.Optional[str] = Field(alias="corrAddrCustNo", default=None)
+    transactions: tp.List[Transactions]
+    inventors: tp.List[Inventor] = Field(default_factory=list)
+    applicants: tp.List[Applicant] = Field(default_factory=list)
+    foreign_priority: tp.List[ForeignPriority] = Field(default_factory=list)
+    assignments: tp.List[Assignment] = Field(default_factory=list)
 
     def __repr__(self):
         return f"USApplication(appl_id='{self.appl_id}', patent_title='{self.patent_title}', app_status='{self.app_status}')"
 
+    # Data removed by USPTO
+
+    @property
+    def attorneys(self):
+        raise RemovedDataException("Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+
+    @property
+    def expiration(self):
+        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def pta_pte_summary(self):
+        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def pta_pte_tran_history(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def parent_continuity(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def child_continuity(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+
+
     @property
     def patent_center_link(self) -> str:
         return f"https://patentcenter.uspto.gov/applications/{self.appl_id}"
 
     @property
-    def google_patents_link(self) -> Optional[str]:
+    def google_patents_link(self) -> tp.Optional[str]:
         if self.patent_number is not None:
             return f"https://patents.google.com/patent/US{self.patent_number}/en"
         elif self.app_early_pub_number is not None:
             return f"https://patents.google.com/patent/{self.app_early_pub_number}/en"
         else:
             return None
 
     @property
-    def continuity(self) -> List[Self]:
+    def continuity(self) -> tp.List["Self"]:
         """Returns a complete set of parents, self, and children"""
         return list(
             [
                 *self.child_continuity.values_list("child", flat=True),
                 self,
                 *self.parent_continuity.values_list("parent", flat=True),
             ]
@@ -217,127 +203,79 @@
         return "Nonprovisional"
 
     @property
     def publication_number(self):
         return self.app_early_pub_number[2:-2]
 
     @property
-    def priority_date(self) -> Optional[datetime.date]:
+    def priority_date(self) -> tp.Optional[datetime.date]:
         """Attempts to return the priority date of the application, calculated as
         the earliest application filing date among the application's parents, or
         its own filing date if it has no parents. Does not include foreign priority
         """
         if not self.parent_continuity:
             return self.app_filing_date
         else:
             return sorted(p.parent_app_filing_date for p in self.parent_continuity)[0]
 
-    @property
-    def expiration(self) -> Optional["Expiration"]:
-        """Calculates expiration data from which the expiration date can be calculated. See
-        help information for the resulting Expiration model.
-        """
-        if "PCT" in self.appl_id:
-            raise NotImplementedError(
-                "Expiration date not supported for PCT Applications"
-            )
-        if not self.patent_number:
-            return None
-        expiration_data = dict()
-        term_parents = [
-            p
-            for p in self.parent_continuity
-            if p.relationship
-            not in ["Claims Priority from Provisional Application", "is a Reissue of"]
-        ]
-        if term_parents:
-            term_parent = sorted(term_parents, key=lambda x: x.parent_app_filing_date)[
-                0
-            ]
-            relationship = term_parent.relationship
-            parent_filing_date = term_parent.parent_app_filing_date
-            parent_appl_id = term_parent.parent_appl_id
-        else:
-            relationship = "self"
-            parent_appl_id = self.appl_id
-            parent_filing_date = self.app_filing_date
-
-        expiration_data["parent_appl_id"] = parent_appl_id
-        expiration_data["parent_app_filing_date"] = parent_filing_date
-        expiration_data["parent_relationship"] = relationship
-        expiration_data["initial_term"] = parent_filing_date + relativedelta(years=20)  # type: ignore
-        expiration_data["pta_or_pte"] = self.pta_pte_summary.total_days or 0  # type: ignore
-        expiration_data["extended_term"] = expiration_data[
-            "initial_term"
-        ] + relativedelta(days=expiration_data["pta_or_pte"])  # type: ignore
-
-        transactions = self.transactions
-        try:
-            _ = next(t for t in transactions if t.code == "DIST")
-            expiration_data["terminal_disclaimer_filed"] = True
-        except StopIteration:
-            expiration_data["terminal_disclaimer_filed"] = False
-
-        return Expiration(**expiration_data)  # type: ignore
-
     # Related objects
     @property
-    def documents(self) -> "Iterable[Document]":
+    def documents(self) -> tp.Iterable["Document"]:
         """File History Documents from PEDS CMS"""
         return self._get_model(".Document").objects.filter(appl_id=self.appl_id)
 
     @property
     def related_assignments(
         self,
-    ) -> "Iterable[Assignment]":
+    ) -> tp.Iterable["Assignment"]:
         """Related Assignments from the Assignments API"""
         return self._get_model("..assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
 
     @property
     def ptab_proceedings(
         self,
-    ) -> "Iterable[PtabProceeding]":
+    ) -> tp.Iterable["PtabProceeding"]:
         """Related PtabProceedings for this application"""
         return self._get_model("..ptab.model.PtabProceeding").objects.filter(
             appl_id=self.appl_id
         )
 
     @property
-    def patent(self) -> "Optional[Patent]":
+    def patent(self) -> tp.Optional["Patent"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("..public_search.model.Patent").objects.get(
             publication_number=self.patent_number
         )
 
     @property
     def publication(
         self,
-    ) -> "Optional[PublishedApplication]":
+    ) -> tp.Optional["PublishedApplication"]:
         """Fulltext version of the Publication - If Available"""
         return self._get_model(
             "..public_search.model.PublishedApplication"
         ).objects.get(
             publication_number=self.publication_number,
         )
 
     @property
     def inpadoc_patent(
         self,
-    ) -> "Optional[InpadocBiblio]":
+    ) -> tp.Optional["InpadocBiblio"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=f"US{self.patent_number}",
         )
 
     @property
     def inpadoc_publication(
         self,
-    ) -> "Optional[InpadocBiblio]":
+    ) -> tp.Optional["InpadocBiblio"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=self.app_early_pub_number,
         )
 
     @model_validator(mode="before")
     @classmethod
@@ -434,17 +372,17 @@
     mail_room_date: Date
     document_code: str
     document_description: str
     document_category: str
     access_level_category: str
     document_identifier: str
     page_count: int
-    pdf_url: Optional[str] = None
+    pdf_url: tp.Optional[str] = None
 
-    async def download(self, path: Optional[str | Path]) -> Path:
+    async def download(self, path: tp.Optional[tp.Union[str, Path]] = None) -> Path:
         from .api import client
 
         if self.pdf_url is None:
             raise ValueError("No PDF URL available")
         full_url = f"https://ped.uspto.gov/api/queries/cms/{self.pdf_url}"
         out_path = await client.download(full_url, path=path)
         return out_path
@@ -459,10 +397,10 @@
 
 class PedsPage(PEDSBaseModel):
     num_found: int = Field(
         validation_alias=AliasPath(
             "queryResults", "searchResponse", "response", "numFound"
         )
     )
-    applications: List[USApplication] = Field(
+    applications: tp.List[USApplication] = Field(
         validation_alias=AliasPath("queryResults", "searchResponse", "response", "docs")
     )
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/query.py` & `patent_client-5.0.1/patent_client/_async/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/peds/search_index.csv` & `patent_client-5.0.1/patent_client/_async/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/api_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/ptab/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+# ********************************************************************************
+# *         WARNING: This file is automatically generated by unasync.py.         *
+# *                             DO NOT MANUALLY EDIT                             *
+# *            Source File: patent_client/_async/uspto/ptab/model.py             *
+# ********************************************************************************
+
 import datetime
 import re
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+import typing as tp
 
 from pydantic import BeforeValidator, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel, DateTime
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from ..peds.model import USApplication
 
 MDYDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m-%d-%Y").date()),
 ]
 
@@ -22,96 +28,96 @@
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
 
 
 class AdditionalRespondent(PtabBaseModel):
-    application_number_text: Optional[str] = None
-    inventor_name: Optional[str] = None
-    patent_number: Optional[str] = None
-    party_name: Optional[str] = None
+    application_number_text: tp.Optional[str] = None
+    inventor_name: tp.Optional[str] = None
+    patent_number: tp.Optional[str] = None
+    party_name: tp.Optional[str] = None
 
 
 class PtabProceeding(PtabBaseModel):
     """A PTAB Proceeding - e.g. IPR/CBM/DER Trial, Patent Appeal, Interference, etc.
 
     All fields are query-able. Date ranges can be formed by inserting "from" or "to" on a query
     for a date range.
 
     """
 
     # Proceeding Metadata
-    last_modified_date: Optional[DateTime] = None
-    last_modified_user_id: Optional[DateTime] = None
-    institution_decision_date: Optional[MDYDate] = None
-    proceeding_filing_date: Optional[MDYDate] = None
-    accorded_filing_date: Optional[MDYDate] = None
-    proceeding_status_category: Optional[str] = None
-    proceeding_number: Optional[str] = None
-    proceeding_last_modified_date: Optional[MDYDate] = None
-    proceeding_type_category: Optional[str] = None
-    subproceeding_type_category: Optional[str] = None
-    decision_date: Optional[MDYDate] = None
-    docket_notice_mail_date: Optional[MDYDate] = None
-    declaration_date: Optional[MDYDate] = None
-    style_name_text: Optional[str] = None
+    last_modified_date: tp.Optional[DateTime] = None
+    last_modified_user_id: tp.Optional[DateTime] = None
+    institution_decision_date: tp.Optional[MDYDate] = None
+    proceeding_filing_date: tp.Optional[MDYDate] = None
+    accorded_filing_date: tp.Optional[MDYDate] = None
+    proceeding_status_category: tp.Optional[str] = None
+    proceeding_number: tp.Optional[str] = None
+    proceeding_last_modified_date: tp.Optional[MDYDate] = None
+    proceeding_type_category: tp.Optional[str] = None
+    subproceeding_type_category: tp.Optional[str] = None
+    decision_date: tp.Optional[MDYDate] = None
+    docket_notice_mail_date: tp.Optional[MDYDate] = None
+    declaration_date: tp.Optional[MDYDate] = None
+    style_name_text: tp.Optional[str] = None
 
     # Respondent Information
-    respondent_technology_center_number: Optional[str] = None
-    respondent_patent_owner_name: Optional[str] = None
-    respondent_party_name: Optional[str] = None
-    respondent_group_art_unit_number: Optional[str] = None
-    respondent_inventor_name: Optional[str] = None
-    respondent_counsel_name: Optional[str] = None
-    respondent_grant_date: Optional[MDYDate] = None
-    respondent_patent_number: Optional[str] = None
-    respondent_application_number_text: Optional[str] = None
-    respondent_publication_number: Optional[str] = None
-    respondent_publication_date: Optional[MDYDate] = None
+    respondent_technology_center_number: tp.Optional[str] = None
+    respondent_patent_owner_name: tp.Optional[str] = None
+    respondent_party_name: tp.Optional[str] = None
+    respondent_group_art_unit_number: tp.Optional[str] = None
+    respondent_inventor_name: tp.Optional[str] = None
+    respondent_counsel_name: tp.Optional[str] = None
+    respondent_grant_date: tp.Optional[MDYDate] = None
+    respondent_patent_number: tp.Optional[str] = None
+    respondent_application_number_text: tp.Optional[str] = None
+    respondent_publication_number: tp.Optional[str] = None
+    respondent_publication_date: tp.Optional[MDYDate] = None
 
     # Petitioner Information
-    petitioner_technology_center_number: Optional[str] = None
-    petitioner_patent_owner_name: Optional[str] = None
-    petitioner_party_name: Optional[str] = None
-    petitioner_group_art_unit_number: Optional[str] = None
-    petitioner_inventor_name: Optional[str] = None
-    petitioner_counsel_name: Optional[str] = None
-    petitioner_grant_date: Optional[MDYDate] = None
-    petitioner_patent_number: Optional[str] = None
-    petitioner_application_number_text: Optional[str] = None
+    petitioner_technology_center_number: tp.Optional[str] = None
+    petitioner_patent_owner_name: tp.Optional[str] = None
+    petitioner_party_name: tp.Optional[str] = None
+    petitioner_group_art_unit_number: tp.Optional[str] = None
+    petitioner_inventor_name: tp.Optional[str] = None
+    petitioner_counsel_name: tp.Optional[str] = None
+    petitioner_grant_date: tp.Optional[MDYDate] = None
+    petitioner_patent_number: tp.Optional[str] = None
+    petitioner_application_number_text: tp.Optional[str] = None
 
     # Appellant Information
-    appellant_technology_center_number: Optional[str] = None
-    appellant_patent_owner_name: Optional[str] = None
-    appellant_party_name: Optional[str] = None
-    appellant_group_art_unit_number: Optional[str] = None
-    appellant_inventor_name: Optional[str] = None
-    appellant_counsel_name: Optional[str] = None
-    appellant_grant_date: Optional[MDYDate] = None
-    appellant_patent_number: Optional[str] = None
-    appellant_application_number_text: Optional[str] = None
-    appellant_publication_date: Optional[MDYDate] = None
-    appellant_publication_number: Optional[str] = None
-    third_party_name: Optional[str] = None
+    appellant_technology_center_number: tp.Optional[str] = None
+    appellant_patent_owner_name: tp.Optional[str] = None
+    appellant_party_name: tp.Optional[str] = None
+    appellant_group_art_unit_number: tp.Optional[str] = None
+    appellant_inventor_name: tp.Optional[str] = None
+    appellant_counsel_name: tp.Optional[str] = None
+    appellant_grant_date: tp.Optional[MDYDate] = None
+    appellant_patent_number: tp.Optional[str] = None
+    appellant_application_number_text: tp.Optional[str] = None
+    appellant_publication_date: tp.Optional[MDYDate] = None
+    appellant_publication_number: tp.Optional[str] = None
+    third_party_name: tp.Optional[str] = None
 
     # Second Respondent (if any)
-    second_respondent_party_name: Optional[str] = None
-    second_respondent_appl_number_text: Optional[str] = None
-    second_respondent_patent_number: Optional[str] = None
-    second_respondent_grant_date: Optional[MDYDate] = None
-    second_respondent_patent_owner_name: Optional[str] = None
-    second_respondent_inventor_name: Optional[str] = None
-    second_respondent_counsel_name: Optional[str] = None
-    second_respondent_g_a_u_number: Optional[str] = None
-    second_respondent_tech_center_number: Optional[str] = None
-    second_respondent_pub_number: Optional[str] = None
-    second_respondent_publication_date: Optional[MDYDate] = None
+    second_respondent_party_name: tp.Optional[str] = None
+    second_respondent_appl_number_text: tp.Optional[str] = None
+    second_respondent_patent_number: tp.Optional[str] = None
+    second_respondent_grant_date: tp.Optional[MDYDate] = None
+    second_respondent_patent_owner_name: tp.Optional[str] = None
+    second_respondent_inventor_name: tp.Optional[str] = None
+    second_respondent_counsel_name: tp.Optional[str] = None
+    second_respondent_g_a_u_number: tp.Optional[str] = None
+    second_respondent_tech_center_number: tp.Optional[str] = None
+    second_respondent_pub_number: tp.Optional[str] = None
+    second_respondent_publication_date: tp.Optional[MDYDate] = None
 
-    additional_respondents: List[str] = Field(default_factory=list)
+    additional_respondents: tp.List[str] = Field(default_factory=list)
 
     @property
     def documents(
         self,
     ) -> "list[PtabDocument]":
         """Documents associated with the Proceeding"""
         return self._get_model(".model.PtabDocument").objects.filter(
@@ -138,73 +144,73 @@
 
 
 fname_re = re.compile(r"[<>:\"/\|?*]")
 
 
 class PtabDocument(PtabBaseModel):
     document_identifier: str = Field(repr=False, default=None)
-    document_category: Optional[str] = None
-    document_type_name: Optional[str] = None
-    document_number: Optional[int] = None
-    document_name: Optional[str] = None
-    document_filing_date: Optional[MDYDate] = None
-    proceeding_number: Optional[str] = None
-    proceeding_type_category: Optional[str] = Field(repr=False, default=None)
-    title: Optional[str] = None
+    document_category: tp.Optional[str] = None
+    document_type_name: tp.Optional[str] = None
+    document_number: tp.Optional[int] = None
+    document_name: tp.Optional[str] = None
+    document_filing_date: tp.Optional[MDYDate] = None
+    proceeding_number: tp.Optional[str] = None
+    proceeding_type_category: tp.Optional[str] = Field(repr=False, default=None)
+    title: tp.Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
         return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
-    async def download(self, path: Optional[str | Path]) -> Path:
+    def download(self, path: tp.Optional[tp.Union[str, Path]]) -> Path:
         from .api import client
 
         name, ext = self.document_name.rsplit(".", 1)
         name = name[:100] + "." + ext
         filename = f"[{str(self.document_number).rjust(4, '0')}] {self.document_filing_date.isoformat()} - {name}"
         filename = filename.encode(encoding="ascii", errors="ignore").decode("ascii")
         filename = fname_re.sub("", filename)
         out_path = Path(path) if path else Path.cwd()
         if out_path.is_dir():
             out_path = Path(path) / filename
         else:
             out_path = out_path
         download_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
-        return await client.download(download_url, path=out_path)
+        return client.download(download_url, path=out_path)
 
 
 class PtabDecision(PtabBaseModel):
     proceeding_number: str
-    board_rulings: List[str] = Field(default_factory=list)
-    decision_type_category: Optional[str] = None
-    document_identifier: Optional[str] = None
-    document_name: Optional[str] = None
-    identifier: Optional[str] = None
-    subdecision_type_category: Optional[str] = None
-    issue_type: List[str] = Field(default_factory=list)
-    object_uu_id: Optional[str] = None
-    petitioner_technology_center_number: Optional[str] = None
+    board_rulings: tp.List[str] = Field(default_factory=list)
+    decision_type_category: tp.Optional[str] = None
+    document_identifier: tp.Optional[str] = None
+    document_name: tp.Optional[str] = None
+    identifier: tp.Optional[str] = None
+    subdecision_type_category: tp.Optional[str] = None
+    issue_type: tp.List[str] = Field(default_factory=list)
+    object_uu_id: tp.Optional[str] = None
+    petitioner_technology_center_number: tp.Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
         return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
 
 class PtabDocumentPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabDocument] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabDocument] = Field(alias="results", default_factory=list)
 
 
 class PtabProceedingPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabProceeding] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabProceeding] = Field(alias="results", default_factory=list)
 
 
 class PtabDecisionPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabDecision] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabDecision] = Field(alias="results", default_factory=list)
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/api.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import json
 from copy import deepcopy
 from pathlib import Path
+
 import httpx
 
 from patent_client._async.http_client import PatentClientSession
 
 from .model import PublicSearchBiblioPage, PublicSearchDocument
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/biblio.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/document.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert/shared.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/convert_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/convert_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from pathlib import Path
 
-fixtures = Path(__file__).parent / "fixtures"
-
 from .convert.biblio import PublicSearchBiblioPageSchema
 from .convert.document import PublicSearchDocumentSchema
 
+fixtures = Path(__file__).parent / "fixtures"
+
 
 def test_convert_biblio():
     input_file = fixtures / "biblio.json"
     output_file = fixtures / "biblio_convert.json"
     input_data = json.loads(input_file.read_text())
     output_data = PublicSearchBiblioPageSchema().deserialize(input_data)
     # output_file.write_text(output_data.to_json(indent=2))
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/count_query.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/manager.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/manager_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/biblio.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/document.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/model/shared.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/model_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
+import datetime
 import json
 from pathlib import Path
 
 from patent_client.util.test import compare_dicts, compare_lists
 
 from .model.biblio import PublicSearchBiblioPage
 from .model.document import PublicSearchDocument
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
-import datetime
-
-
 def json_serial(obj):
     """JSON serializer for objects not serializable by default json code"""
 
     if isinstance(obj, (datetime.datetime, datetime.date)):
         return obj.isoformat()
     raise TypeError("Type %s not serializable" % type(obj))
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/query.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/query_config.csv` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/query_test.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/query_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,17 +84,17 @@
 
     def test_error_query(self):
         with pytest.raises(QueryException):
             PatentBiblioManager().filter(blargh="2021-01-01")._query
 
     def test_error_date_query(self):
         with pytest.raises(QueryException):
-            q = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
+            _ = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
         with pytest.raises(QueryException):
-            q = PatentBiblioManager().filter(app_filing_date=False)._query
+            _ = PatentBiblioManager().filter(app_filing_date=False)._query
 
     def test_multiple_fields(self):
         assert (
             PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
             == '@APD="20210101" AND "6103599".PN.'
         )
         assert (
```

### Comparing `patent_client-5.0.0/patent_client/_async/uspto/public_search/search_query.json` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/__init__.py` & `patent_client-5.0.1/patent_client/_sync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *                Source File: patent_client/_async/__init__.py                 *
 # ********************************************************************************
 
+from . import odp
 from .epo.ops.published.model import Inpadoc
 from .uspto.assignment.model import Assignment
 from .uspto.global_dossier.model import GlobalDossier, GlobalDossierApplication
 from .uspto.peds.model import USApplication
 from .uspto.ptab.model import PtabDecision, PtabDocument, PtabProceeding
 from .uspto.public_search.model import (
     Patent,
     PatentBiblio,
     PublicSearchBiblio,
     PublicSearchDocument,
     PublishedApplication,
     PublishedApplicationBiblio,
 )
 
-from . import odp
-    
-
 __all__ = [
     "Inpadoc",
     "Assignment",
     "USApplication",
     "PtabDecision",
     "PtabDocument",
     "PtabProceeding",
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/__init__.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/api.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
-# *           Source File: patent_client/_async/epo/ops/family/api.py            *
+# *            Source File: patent_client/_async/epo/ops/legal/api.py            *
 # ********************************************************************************
 
-from ..session import asession
-from .model import Family
+from ..session import session
+from .model import Legal
 
 
-class FamilyAsyncApi:
+class LegalApi:
     @classmethod
-    def get_family(cls, number, doc_type="publication", format="docdb"):
-        url = (
-            f"http://ops.epo.org/3.2/rest-services/family/{doc_type}/{format}/{number}"
-        )
-        response = asession.get(url)
-        return Family.model_validate(response.text)
+    def get_legal(cls, doc_number, doc_type="publication", format="docdb"):
+        url = f"http://ops.epo.org/3.2/rest-services/legal/{doc_type}/{format}/{doc_number}"
+        response = session.get(url)
+
+        return Legal.model_validate(response.text)
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/api_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_api_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_convert.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_input.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_input.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/fixtures/family_model_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/manager.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/model.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/model_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/family/schema_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/family/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/api_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_1_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_2_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/example_3_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/fixtures/legal_code_descriptions_202417.xlsx`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/manager.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/model.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,23 +145,29 @@
         "INSERT INTO legal_codes values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", rows
     )
     con.commit()
 
 
 class LegalCodes:
     def __init__(self):
+        self.initialized = False
+
+    def initialize(self):
         if not code_database_current:
             logger.info(
                 "Legal Code Database is out of date - creating legal code database. Note this only happens once!"
             )
             generate_legal_code_db()
         self.connection = sqlite3.connect(db_location, timeout=30)
         self.connection.row_factory = sqlite3.Row
+        self.initialized = True
 
     def get_code_data(self, country_code, legal_code):
+        if not self.initialized:
+            self.initialize()
         cur = self.connection.cursor()
         try:
             return dict(
                 cur.execute(
                     "SELECT * FROM legal_codes WHERE country_code = ? AND event_code = ?",
                     (country_code, legal_code),
                 ).fetchone()
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/national_codes_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/national_codes_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/schema_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/legal/util.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/legal/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *       Source File: patent_client/_async/epo/ops/number_service/api.py        *
 # ********************************************************************************
 
-from ..session import asession
+from ..session import session
 from .model import NumberServiceResult
 
 
 class NumberServiceException(Exception):
     pass
 
 
@@ -31,15 +31,15 @@
             JP.2006147056.A.20060526
             US.(08/921,321).A.19970829
         doc_type: type of document (publication / application / priority)
         input_format: input type (original / docdb / epodoc)
         output_format: output type (original / docdb / epodoc)
 
         """
-        response = asession.get(
+        response = session.get(
             f"http://ops.epo.org/3.2/rest-services/number-service/{doc_type}/{input_format}/{number}/{output_format}",
             extensions={"force_cache": True},
         )
         result = NumberServiceResult.model_validate(response.text)
         errors = [m for m in result.messages if m["kind"] == "ERROR"]
         if errors:
             raise NumberServiceException("\n".join(str(e) for e in errors))
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/api_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/errors.txt` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/errors.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/messages.txt` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/messages.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/model.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/model.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/number_service/schema.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/number_service/schema.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/api.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # ********************************************************************************
 
 import logging
 from io import BytesIO
 
 from yankee.data import AttrDict
 
-from ..session import asession
+from ..session import session
 from .model.biblio import BiblioResult
 from .model.fulltext import Claims, Description
 from .model.images import Images
 from .model.search import Search
 
 logger = logging.getLogger(__name__)
 
 
-class PublishedBiblioAsyncApi:
+class PublishedBiblioApi:
     @classmethod
     def get_constituents(
         cls, number, doc_type="publication", format="docdb", constituents=("biblio",)
     ):
         """Published Data Constituents API
         number: document number to search
         doc_type: document type (application / publication)
@@ -30,40 +30,34 @@
         constituents: what data to retrieve. Can be combined. (biblio / abstract / full-cycle)
 
         """
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/"
         if isinstance(constituents, str):
             constituents = (constituents,)
         url = base_url + ",".join(constituents)
-        response = asession.get(url)
+        response = session.get(url)
         return response.text
 
     @classmethod
     def get_biblio(
         cls, number, doc_type="publication", format="docdb"
     ) -> "BiblioResult":
-        text = cls.get_constituents(
-            number, doc_type, format, constituents="biblio"
-        )
+        text = cls.get_constituents(number, doc_type, format, constituents="biblio")
         return BiblioResult.model_validate(text)
 
     @classmethod
     def get_abstract(cls, number, doc_type="publication", format="docdb"):
-        return cls.get_constituents(
-            number, doc_type, format, constituents="abstract"
-        )
+        return cls.get_constituents(number, doc_type, format, constituents="abstract")
 
     @classmethod
     def get_full_cycle(cls, number, doc_type="publication", format="docdb"):
-        return cls.get_constituents(
-            number, doc_type, format, constituents="full-cycle"
-        )
+        return cls.get_constituents(number, doc_type, format, constituents="full-cycle")
 
 
-class PublishedFulltextAsyncApi:
+class PublishedFulltextApi:
     fulltext_jurisdictions = "EP, WO, AT, BE, BG, CA, CH, CY, CZ, DK, EE, ES, FR, GB, GR, HR, IE, IT, LT, LU, MC, MD, ME, NO, PL, PT, RO, RS, SE, SK".split(
         ", "
     )
 
     @classmethod
     def get_fulltext_result(
         cls, number, doc_type="publication", format="docdb", inquiry="fulltext"
@@ -76,84 +70,80 @@
 
         """
         url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/{inquiry}"
         if number[:2] not in cls.fulltext_jurisdictions:
             raise ValueError(
                 f"Fulltext Is Not Available For Country Code {number[:2]}. Fulltext is only available in {', '.join(cls.fulltext_jurisdictions)}"
             )
-        response = asession.get(url)
+        response = session.get(url)
         response.raise_for_status
         return response.text
 
     @classmethod
     def get_description(cls, number, doc_type="publication", format="docdb"):
         text = cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="description"
         )
         return Description.model_validate(text)
 
     @classmethod
-    def get_claims(
-        cls, number, doc_type="publication", format="docdb"
-    ) -> "Claims":
+    def get_claims(cls, number, doc_type="publication", format="docdb") -> "Claims":
         text = cls.get_fulltext_result(
             number, doc_type="publication", format="docdb", inquiry="claims"
         )
         return Claims.model_validate(text)
 
 
-class PublishedSearchAsyncApi:
+class PublishedSearchApi:
     @classmethod
     def search(cls, query, start=1, end=100):
         base_url = "http://ops.epo.org/3.2/rest-services/published-data/search"
         range = f"{start}-{end}"
         logger.debug(f"OPS Search Endpoint - Query: {query}\nRange: {start}-{end}")
-        response = asession.get(base_url, params={"Range": range, "q": query})
+        response = session.get(base_url, params={"Range": range, "q": query})
         if response.status_code == 404:
             return AttrDict.convert(
                 {
                     "query": "query",
                     "num_results": 0,
                     "begin": start,
                     "end": end,
                     "results": list(),
                 }
             )
 
         return Search.model_validate(response.text)
 
 
-class PublishedImagesAsyncApi:
+class PublishedImagesApi:
     @classmethod
     def get_images(cls, number, doc_type="publication", format="docdb"):
         base_url = f"http://ops.epo.org/3.2/rest-services/published-data/{doc_type}/{format}/{number}/images"
-        response = asession.get(base_url)
+        response = session.get(base_url)
         return Images.model_validate(response.text)
 
     @classmethod
     def get_page_image(
         cls, country, number, kind, image_type, page_number, image_format="pdf"
     ):
-        response = asession.get(
+        response = session.get(
             f"https://ops.epo.org/3.2/rest-services/published-data/images/{country}/{number}/{kind}/{image_type}.{image_format}",
             params={"Range": page_number},
-            stream=True,
             extensions={"force_cache": True},
         )
-        return BytesIO(response.raw.read())
+        return BytesIO(response.content)
 
     @classmethod
     def get_page_image_from_link(cls, link, page_number, image_format="pdf"):
-        response = asession.get(
+        response = session.get(
             f"https://ops.epo.org/3.2/rest-services/{link}.{image_format}",
             params={"Range": page_number},
-            stream=True,
             extensions={"force_cache": True},
         )
-        return BytesIO(response.raw.read())
+        return BytesIO(response.content)
 
 
-class PublishedAsyncApi:
-    biblio = PublishedBiblioAsyncApi
-    fulltext = PublishedFulltextAsyncApi
-    search = PublishedSearchAsyncApi
-    images = PublishedImagesAsyncApi
+class PublishedApi:
+    biblio = PublishedBiblioApi
+    fulltext = PublishedFulltextApi
+    search = PublishedSearchApi
+    images = PublishedImagesApi
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/api_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,80 +3,62 @@
 # *                             DO NOT MANUALLY EDIT                             *
 # *       Source File: patent_client/_async/epo/ops/published/api_test.py        *
 # ********************************************************************************
 
 import json
 from pathlib import Path
 
-import pytest
-
-from .api import PublishedAsyncApi
+from .api import PublishedApi
 
 fixture_dir = Path(__file__).parent / "fixtures"
 
 
-class TestPublishedBiblioAsyncApi:
-    
+class TestPublishedBiblioApi:
     def test_doc_example_biblio(self):
-        result = PublishedAsyncApi.biblio.get_biblio(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = PublishedApi.biblio.get_biblio("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_biblio_result.json"
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
-    
     def test_doc_example_full_cycle(self):
-        result = PublishedAsyncApi.biblio.get_full_cycle(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = PublishedApi.biblio.get_full_cycle("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_full_cycle_result.xml"
         expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
-    
     def test_doc_example_abstract(self):
-        result = PublishedAsyncApi.biblio.get_abstract(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = PublishedApi.biblio.get_abstract("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_abstract_result.xml"
         # expected_file.write_text(result, encoding="utf8")
         expected = expected_file.read_text(encoding="utf8")
         assert result == expected
 
 
 class TestSearchApi:
-    
     def test_search(self):
-        result = PublishedAsyncApi.search.search("ti=plastic")
+        result = PublishedApi.search.search("ti=plastic")
         expected_file = fixture_dir / "search_result.xml"
         expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
 
 class TestFullTextAsyncApi:
-    
     def test_description(self):
-        result = PublishedAsyncApi.fulltext.get_description(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = PublishedApi.fulltext.get_description("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_description_result.xml"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
 
-    
     def test_claims(self):
-        result = PublishedAsyncApi.fulltext.get_claims(
-            "EP1000000.A1", format="epodoc"
-        )
+        result = PublishedApi.fulltext.get_claims("EP1000000.A1", format="epodoc")
         expected_file = fixture_dir / "ep1000000_claims_result.json"
         # expected_file.write_text(result.model_dump_json(indent=2))
         expected = json.loads(expected_file.read_text())
         actual = json.loads(result.model_dump_json())
         assert actual == expected
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/cql.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/cql.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_biblio_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_claims_result.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml` & `patent_client-5.0.1/patent_client/_async/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/fixtures/search_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/search_result.xml`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9587301587301587%*

 * *Differences: {"'results'": "{insert: [(0, OrderedDict([('family_id', '90825108'), ('id_type', 'docdb'), "*

 * *              "('country', 'TW'), ('doc_number', 'I833656'), ('kind', 'B'), ('docdb_number', "*

 * *              "'TWI833656B')])), (1, OrderedDict([('family_id', '90627870'), ('id_type', 'docdb'), "*

 * *              "('country', 'TW'), ('doc_number', 'I833389'), ('kind', 'B'), ('docdb_number', "*

 * *              "'TWI833389B')])), (2, OrderedDict([('family_id', '90823799'), ('id_type', 'docdb'), "*

 * *              "('country',  […]*

```diff
@@ -1,14 +1,222 @@
 {
     "begin": 1,
     "end": 100,
     "num_results": 10000,
     "query": "ti = plastic",
     "results": [
         {
+            "country": "TW",
+            "doc_number": "I833656",
+            "docdb_number": "TWI833656B",
+            "family_id": "90825108",
+            "id_type": "docdb",
+            "kind": "B"
+        },
+        {
+            "country": "TW",
+            "doc_number": "I833389",
+            "docdb_number": "TWI833389B",
+            "family_id": "90627870",
+            "id_type": "docdb",
+            "kind": "B"
+        },
+        {
+            "country": "TW",
+            "doc_number": "M651695",
+            "docdb_number": "TWM651695U",
+            "family_id": "90823799",
+            "id_type": "docdb",
+            "kind": "U"
+        },
+        {
+            "country": "TW",
+            "doc_number": "M651049",
+            "docdb_number": "TWM651049U",
+            "family_id": "88753474",
+            "id_type": "docdb",
+            "kind": "U"
+        },
+        {
+            "country": "TW",
+            "doc_number": "M651104",
+            "docdb_number": "TWM651104U",
+            "family_id": "90823348",
+            "id_type": "docdb",
+            "kind": "U"
+        },
+        {
+            "country": "TW",
+            "doc_number": "M651078",
+            "docdb_number": "TWM651078U",
+            "family_id": "90823290",
+            "id_type": "docdb",
+            "kind": "U"
+        },
+        {
+            "country": "TW",
+            "doc_number": "M651068",
+            "docdb_number": "TWM651068U",
+            "family_id": "90823284",
+            "id_type": "docdb",
+            "kind": "U"
+        },
+        {
+            "country": "CA",
+            "doc_number": "3235790",
+            "docdb_number": "CA3235790A1",
+            "family_id": "84363069",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "CA",
+            "doc_number": "3236276",
+            "docdb_number": "CA3236276A1",
+            "family_id": "80446795",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "TW",
+            "doc_number": "202405064",
+            "docdb_number": "TW202405064A",
+            "family_id": "90822854",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "TW",
+            "doc_number": "202404853",
+            "docdb_number": "TW202404853A",
+            "family_id": "86732062",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "TW",
+            "doc_number": "202404813",
+            "docdb_number": "TW202404813A",
+            "family_id": "90822810",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "PL",
+            "doc_number": "4103490",
+            "docdb_number": "PL4103490T3",
+            "family_id": "74550685",
+            "id_type": "docdb",
+            "kind": "T3"
+        },
+        {
+            "country": "PL",
+            "doc_number": "131036",
+            "docdb_number": "PL131036U1",
+            "family_id": "90790628",
+            "id_type": "docdb",
+            "kind": "U1"
+        },
+        {
+            "country": "PL",
+            "doc_number": "442543",
+            "docdb_number": "PL442543A1",
+            "family_id": "90790589",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024086147",
+            "docdb_number": "WO2024086147A1",
+            "family_id": "90738205",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024085310",
+            "docdb_number": "WO2024085310A1",
+            "family_id": "90737986",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024085218",
+            "docdb_number": "WO2024085218A1",
+            "family_id": "90737902",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024085131",
+            "docdb_number": "WO2024085131A1",
+            "family_id": "90737893",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024085217",
+            "docdb_number": "WO2024085217A1",
+            "family_id": "90737625",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "WO",
+            "doc_number": "2024085001",
+            "docdb_number": "WO2024085001A1",
+            "family_id": "90737463",
+            "id_type": "docdb",
+            "kind": "A1"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2023008483",
+            "docdb_number": "MX2023008483A",
+            "family_id": "76525546",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2023008484",
+            "docdb_number": "MX2023008484A",
+            "family_id": "77076147",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2023006430",
+            "docdb_number": "MX2023006430A",
+            "family_id": "74003695",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "MX",
+            "doc_number": "2023007539",
+            "docdb_number": "MX2023007539A",
+            "family_id": "60663297",
+            "id_type": "docdb",
+            "kind": "A"
+        },
+        {
+            "country": "CZ",
+            "doc_number": "37828",
+            "docdb_number": "CZ37828U1",
+            "family_id": "90730538",
+            "id_type": "docdb",
+            "kind": "U1"
+        },
+        {
             "country": "CA",
             "doc_number": "3234950",
             "docdb_number": "CA3234950A1",
             "family_id": "78516473",
             "id_type": "docdb",
             "kind": "A1"
         },
@@ -591,218 +799,10 @@
         {
             "country": "WO",
             "doc_number": "2024071139",
             "docdb_number": "WO2024071139A1",
             "family_id": "90478038",
             "id_type": "docdb",
             "kind": "A1"
-        },
-        {
-            "country": "WO",
-            "doc_number": "2024067879",
-            "docdb_number": "WO2024067879A1",
-            "family_id": "84905305",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "WO",
-            "doc_number": "2024066118",
-            "docdb_number": "WO2024066118A1",
-            "family_id": "84393933",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "WO",
-            "doc_number": "2024066107",
-            "docdb_number": "WO2024066107A1",
-            "family_id": "89573406",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "WO",
-            "doc_number": "2024066099",
-            "docdb_number": "WO2024066099A1",
-            "family_id": "89164385",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "WO",
-            "doc_number": "2024065084",
-            "docdb_number": "WO2024065084A1",
-            "family_id": "90475169",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "ZA",
-            "doc_number": "202106922",
-            "docdb_number": "ZA202106922B",
-            "family_id": "73045953",
-            "id_type": "docdb",
-            "kind": "B"
-        },
-        {
-            "country": "KR",
-            "doc_number": "102648713",
-            "docdb_number": "KR102648713B1",
-            "family_id": "90473961",
-            "id_type": "docdb",
-            "kind": "B1"
-        },
-        {
-            "country": "KR",
-            "doc_number": "20240038308",
-            "docdb_number": "KR20240038308A",
-            "family_id": "90473953",
-            "id_type": "docdb",
-            "kind": "A"
-        },
-        {
-            "country": "KR",
-            "doc_number": "20240038197",
-            "docdb_number": "KR20240038197A",
-            "family_id": "90473917",
-            "id_type": "docdb",
-            "kind": "A"
-        },
-        {
-            "country": "KR",
-            "doc_number": "20240039096",
-            "docdb_number": "KR20240039096A",
-            "family_id": "90473039",
-            "id_type": "docdb",
-            "kind": "A"
-        },
-        {
-            "country": "KR",
-            "doc_number": "20240037213",
-            "docdb_number": "KR20240037213A",
-            "family_id": "66846582",
-            "id_type": "docdb",
-            "kind": "A"
-        },
-        {
-            "country": "PT",
-            "doc_number": "3660189",
-            "docdb_number": "PT3660189T",
-            "family_id": "50434027",
-            "id_type": "docdb",
-            "kind": "T"
-        },
-        {
-            "country": "PL",
-            "doc_number": "3837112",
-            "docdb_number": "PL3837112T3",
-            "family_id": "63962763",
-            "id_type": "docdb",
-            "kind": "T3"
-        },
-        {
-            "country": "PL",
-            "doc_number": "4079488",
-            "docdb_number": "PL4079488T3",
-            "family_id": "75625462",
-            "id_type": "docdb",
-            "kind": "T3"
-        },
-        {
-            "country": "PL",
-            "doc_number": "442333",
-            "docdb_number": "PL442333A1",
-            "family_id": "90471944",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "PL",
-            "doc_number": "446313",
-            "docdb_number": "PL446313A1",
-            "family_id": "90471934",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024110577",
-            "docdb_number": "US2024110577A1",
-            "family_id": "90471670",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024110109",
-            "docdb_number": "US2024110109A1",
-            "family_id": "73344141",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024109682",
-            "docdb_number": "US2024109682A1",
-            "family_id": "90471433",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024109220",
-            "docdb_number": "US2024109220A1",
-            "family_id": "88197191",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024109239",
-            "docdb_number": "US2024109239A1",
-            "family_id": "87933698",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024109090",
-            "docdb_number": "US2024109090A1",
-            "family_id": "90471290",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024109047",
-            "docdb_number": "US2024109047A1",
-            "family_id": "90471235",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "US",
-            "doc_number": "2024110860",
-            "docdb_number": "US2024110860A1",
-            "family_id": "77928972",
-            "id_type": "docdb",
-            "kind": "A1"
-        },
-        {
-            "country": "FI",
-            "doc_number": "3946667",
-            "docdb_number": "FI3946667T3",
-            "family_id": "73781005",
-            "id_type": "docdb",
-            "kind": "T3"
-        },
-        {
-            "country": "CZ",
-            "doc_number": "37788",
-            "docdb_number": "CZ37788U1",
-            "family_id": "90459351",
-            "id_type": "docdb",
-            "kind": "U1"
         }
     ]
 }
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # *        Source File: patent_client/_async/epo/ops/published/manager.py        *
 # ********************************************************************************
 
 import math
 
 from patent_client.util.manager import Manager
 
-from .api import PublishedAsyncApi
+from .api import PublishedApi
 from .cql import generate_query
 from .model.biblio import BiblioResult
 from .model.fulltext import Claims, Description
 from .model.images import ImageDocument
 
 
 def get_ranges(limit=None, offset=0, page_size=100):
@@ -40,15 +40,15 @@
     primary_key = "publication"
 
     def _get_search_results_range(self, start=1, end=100):
         if "cql_query" in self.config.filter:
             query = self.config.filter["cql_query"]
         else:
             query = generate_query(**self.config.filter)
-        return PublishedAsyncApi.search.search(query, start, end)
+        return PublishedApi.search.search(query, start, end)
 
     def count(self) -> int:
         page = self._get_search_results_range(1, 100)
         offset = self.config.offset or 0
         limit = self.config.limit or page.num_results - offset
         num_results = page.num_results
         num_results -= offset
@@ -62,41 +62,41 @@
             page = self._get_search_results_range(start, end)
             for result in page.results:
                 yield result
             if len(page.results) < self.result_size:
                 break
 
     def get(self, number, doc_type="publication", format="docdb") -> BiblioResult:
-        result = PublishedAsyncApi.biblio.get_biblio(number, doc_type, format)
+        result = PublishedApi.biblio.get_biblio(number, doc_type, format)
         if len(result.documents) > 1:
             raise Exception("More than one result found! Try another query")
         return result.documents[0]
 
 
 class BiblioManager(Manager):
     def get(self, doc_number) -> "BiblioResult":
-        result = PublishedAsyncApi.biblio.get_biblio(doc_number)
+        result = PublishedApi.biblio.get_biblio(doc_number)
         if len(result.documents) > 1:
             raise ValueError(f"More than one result found for {doc_number}!")
         return result.documents[0]
 
 
 class ClaimsManager(Manager):
     def get(self, doc_number) -> "Claims":
-        return PublishedAsyncApi.fulltext.get_claims(doc_number)
+        return PublishedApi.fulltext.get_claims(doc_number)
 
 
 class DescriptionManager(Manager):
     def get(self, doc_number) -> Description:
-        return PublishedAsyncApi.fulltext.get_description(doc_number)
+        return PublishedApi.fulltext.get_description(doc_number)
 
 
 class ImagesManager(Manager):
     def get(self, doc_number) -> ImageDocument:
-        return PublishedAsyncApi.images.get_images(doc_number)
+        return PublishedApi.images.get_images(doc_number)
 
 
 class InpadocManager(SearchManager):
     pass
 
 
 class InpadocBiblioManager(BiblioManager):
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/manager_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *     Source File: patent_client/_async/epo/ops/published/manager_test.py      *
 # ********************************************************************************
 
-import pytest
 
 from .model.search import Inpadoc
 
 
 class TestPublished:
-    
     def test_inpadoc_manager(self):
         result = Inpadoc.objects.filter(applicant="Microsoft")
         assert result.count() > 20
-        countries = [
-            c for c in result.limit(20).values_list("country", flat=True)
-        ]
+        countries = [c for c in result.limit(20).values_list("country", flat=True)]
         assert sum(1 for c in countries if c == "US") >= 1
 
-    
     def test_get_biblio_from_result(self):
         doc = Inpadoc.objects.filter(applicant="Google").first()
         result = doc.biblio
         assert len(result.titles) > 0
 
-    
     def test_get_claims_from_result(self):
         result = Inpadoc.objects.get("WO2009085664A2")
         claims = result.claims
         assert len(claims.claims) == 20
         assert len(claims.claim_text) == 4830
 
-    
     def test_get_description_from_result(self):
         result = Inpadoc.objects.get("WO2009085664A2")
         description = result.description
         assert len(description) == 47955
 
-    
     def test_get_family_from_result(self):
         result = Inpadoc.objects.get("WO2009085664A2")
         family = result.family
         assert len(family) >= 20
 
-    
     def test_get_biblio_from_wo(self):
         result = Inpadoc.objects.get("WO2009085664A2")
         biblio = result.biblio
         assert biblio.abstract is not None
 
-    
     def test_can_index_inpadoc_result(self):
         result = Inpadoc.objects.filter(applicant="Tesla")
         first = result.first()
         second = result.offset(1).first()
         assert first != second
 
-    
     def test_can_handle_single_item_ipc_classes(self):
         result = Inpadoc.objects.get("WO2020081771")
         biblio = result.biblio
         assert biblio.intl_class is not None
 
-    
     def test_issue_41(self):
         result = Inpadoc.objects.get("JP2005533465A")
         biblio = result.biblio
         assert biblio.title is None
+
+    def test_document_downloading(self, tmpdir):
+        result = Inpadoc.objects.get("WO2010050748A2")
+        result.download(tmpdir)
+        assert len(tmpdir.listdir()) > 0
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/__init__.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/biblio.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/fulltext.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/images.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/model/search.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/model/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/__init__.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/biblio.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/fulltext.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/fulltext.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/images.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/images.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema/search.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema/search.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/schema_test.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/schema_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/biblio_example_4.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/claims_example_2.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/claims_example_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/description_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/description_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/biblio_example_4.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/claims_example.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/claims_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_abstract_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_biblio_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_claims_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/ep1000000_description_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/ep1000000_full_cycle_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (826)*

 * *Files 0% similar despite different names*

```diff
@@ -1318,8 +1318,8 @@
 00005250: 696f 6e2d 7469 746c 653e 0a20 2020 2020  ion-title>.     
 00005260: 2020 2020 2020 203c 2f62 6962 6c69 6f67         </bibliog
 00005270: 7261 7068 6963 2d64 6174 613e 0a20 2020  raphic-data>.   
 00005280: 2020 2020 203c 2f65 7863 6861 6e67 652d       </exchange-
 00005290: 646f 6375 6d65 6e74 3e0a 2020 2020 3c2f  document>.    </
 000052a0: 6578 6368 616e 6765 2d64 6f63 756d 656e  exchange-documen
 000052b0: 7473 3e0a 3c2f 6f70 733a 776f 726c 642d  ts>.</ops:world-
-000052c0: 7061 7465 6e74 2d64 6174 613e            patent-data>
+000052c0: 7061 7465 6e74 2d64 6174 613e 0a         patent-data>.
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/image_example.json` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/image_example.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/expected/search_result.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/expected/search_result.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

 * *Files 8% similar despite different names*

#### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/full_cycle_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/fixtures/ep1000000_full_cycle_result.xml`

```diff
@@ -47,50 +47,40 @@
             <generating-office>US</generating-office>
           </patent-classification>
           <patent-classification sequence="2">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
-            <main-group>1</main-group>
-            <subgroup>29</subgroup>
-            <classification-value>I</classification-value>
-            <generating-office>EP</generating-office>
-          </patent-classification>
-          <patent-classification sequence="3">
-            <classification-scheme office="EP" scheme="CPCI"/>
-            <section>B</section>
-            <class>28</class>
-            <subclass>B</subclass>
             <main-group>5</main-group>
             <subgroup>022</subgroup>
             <classification-value>I</classification-value>
             <generating-office>US</generating-office>
           </patent-classification>
-          <patent-classification sequence="4">
+          <patent-classification sequence="3">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>5</main-group>
-            <subgroup>022</subgroup>
+            <subgroup>025</subgroup>
             <classification-value>I</classification-value>
             <generating-office>EP</generating-office>
           </patent-classification>
-          <patent-classification sequence="5">
+          <patent-classification sequence="4">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>7</main-group>
             <subgroup>0064</subgroup>
             <classification-value>I</classification-value>
             <generating-office>US</generating-office>
           </patent-classification>
-          <patent-classification sequence="6">
+          <patent-classification sequence="5">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>7</main-group>
             <subgroup>0064</subgroup>
             <classification-value>I</classification-value>
@@ -266,50 +256,40 @@
             <generating-office>US</generating-office>
           </patent-classification>
           <patent-classification sequence="2">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
-            <main-group>1</main-group>
-            <subgroup>29</subgroup>
-            <classification-value>I</classification-value>
-            <generating-office>EP</generating-office>
-          </patent-classification>
-          <patent-classification sequence="3">
-            <classification-scheme office="EP" scheme="CPCI"/>
-            <section>B</section>
-            <class>28</class>
-            <subclass>B</subclass>
             <main-group>5</main-group>
             <subgroup>022</subgroup>
             <classification-value>I</classification-value>
             <generating-office>US</generating-office>
           </patent-classification>
-          <patent-classification sequence="4">
+          <patent-classification sequence="3">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>5</main-group>
-            <subgroup>022</subgroup>
+            <subgroup>025</subgroup>
             <classification-value>I</classification-value>
             <generating-office>EP</generating-office>
           </patent-classification>
-          <patent-classification sequence="5">
+          <patent-classification sequence="4">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>7</main-group>
             <subgroup>0064</subgroup>
             <classification-value>I</classification-value>
             <generating-office>US</generating-office>
           </patent-classification>
-          <patent-classification sequence="6">
+          <patent-classification sequence="5">
             <classification-scheme office="EP" scheme="CPCI"/>
             <section>B</section>
             <class>28</class>
             <subclass>B</subclass>
             <main-group>7</main-group>
             <subgroup>0064</subgroup>
             <classification-value>I</classification-value>
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/image_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/image_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/published/test/search_example.xml` & `patent_client-5.0.1/patent_client/_sync/epo/ops/published/test/search_example.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/session.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,35 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *             Source File: patent_client/_async/epo/ops/session.py             *
 # ********************************************************************************
 
 import base64
 import datetime as dt
+import logging
 from typing import Sequence
 
 import hishel
 import httpx
 from httpcore import Request, Response
 
 from patent_client import SETTINGS
 from patent_client._sync.http_client import PatentClientSession
 from patent_client.session import CACHE_DIR
 
-import logging
-
 logger = logging.getLogger(__name__)
 
 NS = {
     "http://ops.epo.org": None,
     "http://www.epo.org/exchange": None,
     "http://www.epo.org/fulltext": None,
     "http://www.epo.org/register": None,
 }
 
 
-
-
 class OpsAuthenticationError(Exception):
     pass
 
 
 class OpsForbiddenError(Exception):
     pass
 
@@ -113,15 +110,15 @@
 
 def handle_response(response):
     if response.status_code == 403:
         raise OpsForbiddenError("Forbidden")
     return response
 
 
-asession = PatentClientSession(
+session = PatentClientSession(
     transport=ops_transport,
     auth=OpsAuth(key=SETTINGS.epo_api_key, secret=SETTINGS.epo_api_secret),
     event_hooks={
         "response": [
             handle_response,
         ]
     },
```

### Comparing `patent_client-5.0.0/patent_client/_sync/epo/ops/util.py` & `patent_client-5.0.1/patent_client/_sync/epo/ops/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *              Source File: patent_client/_async/epo/ops/util.py               *
 # ********************************************************************************
 
 from typing import TYPE_CHECKING, List, Optional
 
-
 from async_property.base import AsyncPropertyDescriptor
 from pydantic import ConfigDict, computed_field, model_validator
 from yankee.xml.schema import Schema as XmlSchema
 
 from patent_client.util.pydantic_util import BaseModel
 
 if TYPE_CHECKING:
@@ -74,21 +73,25 @@
         return self._get_model(
             ".published.model.Claims", base_class=InpadocModel
         ).objects.get(self.docdb_number)
 
     @property
     def legal(self) -> List["LegalEvent"]:
         return (
-            self._get_model(
-                ".legal.model.Legal", base_class=InpadocModel
-            ).objects.get(self.docdb_number)
+            self._get_model(".legal.model.Legal", base_class=InpadocModel).objects.get(
+                self.docdb_number
+            )
         ).events
 
     @property
     def family(
         self,
     ) -> List["FamilyMember"]:
         return (
             self._get_model(
                 ".family.model.Family", base_class=InpadocModel
             ).objects.get(self.docdb_number)
         ).family_members
+
+    def download(self, path: str = "."):
+        images = self.images
+        return images.full_document.download(path)
```

### Comparing `patent_client-5.0.0/patent_client/_sync/http_client.py` & `patent_client-5.0.1/patent_client/_sync/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # *               Source File: patent_client/_async/http_client.py               *
 # ********************************************************************************
 
 import re
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-from typing import Optional
+import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -69,15 +69,15 @@
             path = path / filename if path else Path.cwd() / filename
         return path
 
     def download(
         self,
         url,
         method: str = "GET",
-        path: Optional[str | Path] = None,
+        path: tp.Optional[tp.Union[str, Path]] = None,
         **kwargs,
     ):
         # Ensure we skip the cache for file downloads
         kwargs["extensions"] = kwargs.get("extensions", dict())
         if "force_cache" in kwargs["extensions"]:
             raise ValueError("force_cache is not supported for file downloads")
         kwargs["extensions"]["cache_disabled"] = True
```

### Comparing `patent_client-5.0.0/patent_client/_sync/odp.py` & `patent_client-5.0.1/patent_client/_sync/odp.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,7 @@
 # ********************************************************************************
 
 # A simple separate namespace for the USPTO's Open Data Portal.
 
 from patent_client._sync.uspto.odp.model import USApplication, USApplicationBiblio
 
 __all__ = ["USApplication", "USApplicationBiblio"]
-
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/api_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *        Source File: patent_client/_async/uspto/assignment/api_test.py        *
 # ********************************************************************************
 
 from pathlib import Path
 
-import httpx
 import pytest
 
 from .api import AssignmentApi
 
 
 
 def test_alookup():
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/convert_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/convert_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_1.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_2.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/fixtures/assignment_3.xml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 from .api import AssignmentApi
 from .model import Assignment
 
 warnings.filterwarnings("ignore", category=InsecureRequestWarning)
 
 NUMBER_CLEAN_RE = re.compile(r"[^\d]")
-clean_number = lambda x: NUMBER_CLEAN_RE.sub("", str(x))
+
+
+def clean_number(x):
+    return NUMBER_CLEAN_RE.sub("", str(x))
 
 
 logger = logging.getLogger(__name__)
 
 
 class AssignmentManager(Manager["Assignment"]):
     fields = {
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/manager_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,20 +34,20 @@
         assert len(a.properties) == 5
         assert (
             a.properties[0].invention_title
             == "SYSTEM AND METHODS FOR ACCELERATED DATA STORAGE AND RETRIEVAL"
         )
         assert a.properties[0].appl_num == "10628795"
         assert a.properties[0].filing_date.isoformat() == "2003-07-28"
-        assert a.properties[0].intl_publ_date == None
-        assert a.properties[0].intl_reg_num == None
+        assert a.properties[0].intl_publ_date is None
+        assert a.properties[0].intl_reg_num is None
         assert a.properties[0].inventors == "James J. Fallon"
         assert a.properties[0].issue_date.isoformat() == "2006-10-31"
         assert a.properties[0].pat_num == "7130913"
-        assert a.properties[0].pct_num == None
+        assert a.properties[0].pct_num is None
         assert a.properties[0].publ_date.isoformat() == "2004-04-15"
         assert a.properties[0].publ_num == "20040073746"
 
     
     def test_fetch_assignments_by_assignee(self):
         assignments = Assignment.objects.filter(assignee="US Well Services")
         assert assignments.count() >= 22
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/uspto/assignment/model.py          *
 # ********************************************************************************
 
 import datetime
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+import typing as tp
 
 from dateutil.parser import isoparse
 from pydantic import BeforeValidator, ConfigDict, Field, field_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from ..peds.model import USApplication
     from ..public_search.model import Patent, PublishedApplication
 
 UsptoDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%Y%m%d").date()),
 ]
@@ -38,15 +38,15 @@
     dt = parse_datetime(string)
     if dt is None:
         return None
     return dt.date()
 
 
 DatetimeAsDate = Annotated[
-    Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
+    tp.Optional[datetime.date], BeforeValidator(lambda x: parse_date(x))
 ]
 
 
 class AbstractAssignmentModel(BaseModel):
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
@@ -64,26 +64,26 @@
     address: str = Field(alias="patAssigneeAddress")
 
 
 class Property(AbstractAssignmentModel):
     invention_title: str
     invention_title_lang: str
     appl_num: str
-    filing_date: Optional[DatetimeAsDate] = None
-    intl_publ_date: Optional[DatetimeAsDate] = None
-    intl_reg_num: Optional[str] = None
-    inventors: Optional[str] = None
-    issue_date: Optional[DatetimeAsDate] = None
-    pat_num: Optional[str] = None
-    pct_num: Optional[str] = None
-    publ_date: Optional[DatetimeAsDate] = None
-    publ_num: Optional[str] = None
+    filing_date: tp.Optional[DatetimeAsDate] = None
+    intl_publ_date: tp.Optional[DatetimeAsDate] = None
+    intl_reg_num: tp.Optional[str] = None
+    inventors: tp.Optional[str] = None
+    issue_date: tp.Optional[DatetimeAsDate] = None
+    pat_num: tp.Optional[str] = None
+    pct_num: tp.Optional[str] = None
+    publ_date: tp.Optional[DatetimeAsDate] = None
+    publ_num: tp.Optional[str] = None
 
     @property
-    def application(self) -> Optional["USApplication"]:
+    def application(self) -> tp.Optional["USApplication"]:
         """The related US Application"""
         try:
             appl_id = getattr(self, "appl_id", None)
             if appl_id is not None:
                 return self._get_model(
                     "patent_client.uspto.peds.model.USApplication"
                 ).objects.get(appl_id=appl_id)
@@ -127,29 +127,29 @@
 class Correspondent(AbstractAssignmentModel):
     name: str
     address: str
 
 
 class Assignment(AbstractAssignmentModel["AssignmentManager"]):
     id: str
-    date_produced: Optional[UsptoDate] = None
-    action_key_code: Optional[str] = None
-    transaction_date: Optional[DatetimeAsDate] = None
+    date_produced: tp.Optional[UsptoDate] = None
+    action_key_code: tp.Optional[str] = None
+    transaction_date: tp.Optional[DatetimeAsDate] = None
     last_update_date: DatetimeAsDate
     purge_indicator: YNBool
     recorded_date: DatetimeAsDate
     page_count: int
     conveyance_text: str
     assignment_record_has_images: YNBool
-    attorney_dock_num: Optional[str] = None
+    attorney_dock_num: tp.Optional[str] = None
     pat_assignor_earliest_ex_date: DatetimeAsDate
     correspondent: Correspondent
-    assignors: List[Assignor]
-    assignees: List[Assignee]
-    properties: List[Property]
+    assignors: tp.List[Assignor]
+    assignees: tp.List[Assignee]
+    properties: tp.List[Property]
 
     @field_validator("conveyance_text")
     @classmethod
     def remove_see_document(cls, v) -> str:
         return v.replace(" (SEE DOCUMENT FOR DETAILS).", "").strip()
 
     @property
@@ -159,15 +159,15 @@
     @property
     def image_url(self):
         reel, frame = self.reel_frame
         reel = reel.rjust(6, "0")
         frame = frame.rjust(4, "0")
         return f"http://legacy-assignments.uspto.gov/assignments/assignment-pat-{reel}-{frame}.pdf"
 
-    def download(self, path: Optional[str | Path] = None):
+    def download(self, path: tp.Optional[tp.Union[str, Path]] = None):
         """asynchronously downloads the PDF associated with the assignment to the current working directory"""
         from .api import client
 
         return client.download(self.image_url, path=path)
 
 
 class AssignmentPage(AbstractAssignmentModel):
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/assignment/model_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/assignment/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         )
         return [Product.model_validate(product) for product in response.json()]
 
     @classmethod
     def get_by_short_name(
         cls,
         product_name: str,
-        from_date: tp.Optional[datetime.date | str] = None,
-        to_date: tp.Optional[datetime.date | str] = None,
+        from_date: tp.Optional[tp.Union[datetime.date, str]] = None,
+        to_date: tp.Optional[tp.Union[datetime.date, str]] = None,
         max_files: int = 20,
     ) -> tp.List[Product]:
         """Returns files associated with products (of level PRODUCT) based on their full or partial names."""
         params = dict()
         if from_date:
             if isinstance(from_date, str):
                 from_date = datetime.date.fromisoformat(from_date)
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/bulk_data/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/bulk_data/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     size: int = Field(alias="fileSize")
     download_url: str = Field(alias="fileDownloadUrl")
     from_date: datetime.date = Field(alias="fileFromTime")
     to_date: datetime.date = Field(alias="fileToTime")
     type: str = Field(alias="fileType")
     release_date: datetime.date = Field(alias="fileReleaseDate")
 
-    def download(self, path: tp.Optional[str | Path]):
+    def download(self, path: tp.Optional[tp.Union[str, Path]]):
         from .api import client
 
         return client.download(self.download_url, path=path)
 
 
 class Product(BaseModel):
     link_path: str = Field(alias="productLinkPath")
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/gd_input.csv` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/gd_input.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from pydantic import BeforeValidator, ConfigDict, Field, model_validator
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel
 
 if tp.TYPE_CHECKING:
+    from ..assignment.model import Assignment
     from ..peds.model import USApplication
     from ..public_search.model import Patent, PublishedApplication
-    from ..assignment.model import Assignment
 
 MDYDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m/%d/%Y").date()),
 ]
 OptionalStrList = Annotated[
     tp.List[str], BeforeValidator(lambda x: x if isinstance(x, list) else list())
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/model_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/query_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/query_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app.json` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/app_expected.json` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/app_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list.json` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json` & `patent_client-5.0.1/patent_client/_sync/uspto/global_dossier/test/doc_list_expected.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *              Source File: patent_client/_async/uspto/odp/api.py              *
 # ********************************************************************************
 
 import typing as tp
 
-import httpx
-
 from patent_client import SETTINGS
-from ...http_client import PatentClientSession
 
+from ...http_client import PatentClientSession
 from .model import (
     Assignment,
     Continuity,
     CustomerNumber,
     Document,
     ForeignPriority,
     SearchGetRequest,
@@ -27,17 +25,15 @@
 from .util import prune
 
 
 class ODPApi:
     base_url = "https://beta-api.uspto.gov"
 
     def __init__(self):
-        self.client = PatentClientSession(
-            headers={"X-API-KEY": SETTINGS.odp_api_key}
-        )
+        self.client = PatentClientSession(headers={"X-API-KEY": SETTINGS.odp_api_key})
 
     def post_search(
         self, search_request: SearchRequest = SearchRequest()
     ) -> tp.Dict:
         url = self.base_url + "/api/v1/patent/applications/search"
         search_data = prune(search_request.model_dump())
         response = self.client.post(
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/adjustment.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/adjustment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/application.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/application.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/assignment.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/assignment.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/attorney.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/attorney.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/biblio.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/continuity.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/continuity.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/documents.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/documents.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/search.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/search.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/swagger.yaml` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/swagger.yaml`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/fixtures/transactions.json` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/fixtures/transactions.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 
 from .api import ODPApi
 from .model import SearchRequest, USApplication, USApplicationBiblio
 from .query import create_post_search_obj
 
 if tp.TYPE_CHECKING:
     from .model import (
+        Assignment,
         Continuity,
+        CustomerNumber,
         Document,
+        ForeignPriority,
         SearchResult,
+        TermAdjustment,
+        Transaction,
         USApplication,
         USApplicationBiblio,
-        TermAdjustment,
-        Assignment,
-        CustomerNumber,
-        ForeignPriority,
-        Transaction
     )
 
 
 api = ODPApi()
 
 
 class USApplicationManager(Manager):
@@ -109,47 +109,53 @@
 
     def count(self):
         return len(api.get_documents(self.config.filter["appl_id"][0]))
 
     def _get_results(self) -> tp.Iterator["Document"]:
         for doc in api.get_documents(self.config.filter["appl_id"][0]):
             yield doc
-            
+
+
 class TermAdjustmentManager(Manager):
     default_filter = "appl_id"
-    
+
     def _get_results(self) -> "TermAdjustment":
         return api.get_term_adjustments(self.config.filter["appl_id"][0])
-    
+
+
 class AssignmentManager(Manager):
     default_filter = "appl_id"
-    
+
     def _get_results(self) -> tp.Iterator["Assignment"]:
         for doc in api.get_assignments(self.config.filter["appl_id"][0]):
             yield doc
-    
+
     def count(self):
         return len(api.get_assignments(self.config.filter["appl_id"][0]))
-    
+
+
 class CustomerNumberManager(Manager):
     default_filter = "appl_id"
-    
+
     def _get_results(self) -> "CustomerNumber":
         return api.get_customer_numbers(self.config.filter["appl_id"][0])
-    
+
+
 class ForeignPriorityManager(Manager):
     default_filter = "appl_id"
-    
+
     def _get_results(self) -> "ForeignPriority":
-        for doc in api.get_foreign_priority_data(self.config.filter["appl_id"][0]):
+        for doc in api.get_foreign_priority_data(
+            self.config.filter["appl_id"][0]
+        ):
             yield doc
-    
+
+
 class TransactionManager(Manager):
     default_filter = "appl_id"
-    
+
     def _get_results(self) -> tp.Iterator["Transaction"]:
         for doc in api.get_transactions(self.config.filter["appl_id"][0]):
             yield doc
-    
+
     def count(self):
         return len(api.get_transactions(self.config.filter["appl_id"][0]))
-
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/manager_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *         Source File: patent_client/_async/uspto/odp/manager_test.py          *
 # ********************************************************************************
 
 import pytest
 
-from .manager import USApplicationManager
+from .manager import USApplicationBiblioManager, USApplicationManager
 
 
 
 def test_all_apps():
     manager = USApplicationManager().filter(query=dict())
     assert manager.count() > 1000
 
@@ -20,39 +20,39 @@
     app = USApplicationManager().get(q="applicationNumberText:16123456")
     assert app is not None
     assert app.appl_id == "16123456"
 
 
 
 def test_get_app_from_search_result():
-    manager = USApplicationManager()
+    manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     application = result.application
     assert application.appl_id == "16123456"
 
 
 
 def test_get_app_biblio_from_search_result():
-    manager = USApplicationManager()
+    manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     biblio = result.biblio
     assert biblio.appl_id == "16123456"
 
 
 
 def test_get_continuity_from_search_result():
-    manager = USApplicationManager()
+    manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     continuity = result.continuity
     assert len(continuity.child_continuity) > 0
 
 
 
 def test_get_documents_from_search_result():
-    manager = USApplicationManager()
+    manager = USApplicationBiblioManager()
     result = manager.get(q="applicationNumberText:16123456")
     documents = result.documents
     assert documents.count() > 0
 
 
 
 def test_simple_keyword_searches():
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,23 +94,28 @@
     appl_id: str = Field(alias="applicationNumberText")
     mail_date: datetime.datetime = Field(alias="officialDate")
     document_identifier: str = Field(alias="documentIdentifier")
     document_code: str = Field(alias="documentCode")
     document_code_description: str = Field(alias="documentCodeDescriptionText")
     direction_category: str = Field(alias="directionCategory")
     download_option_bag: list[dict] = Field(alias="downloadOptionBag")
-    
+
     def download(self, type="PDF", out_path=None):
         from .manager import api
+
         try:
-            url = next(u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type)["downloadUrl"]
+            url = next(
+                u for u in self.download_option_bag if u["mimeTypeIdentifier"] == type
+            )["downloadUrl"]
         except StopIteration:
             raise ValueError(f"No download URL found for this document type: {type}")
         if out_path is None:
-            out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace("/", "-")
+            out_path = f"{self.appl_id} - {self.mail_date.date()} - {self.document_code} - {self.document_code_description}.{type.lower()}".replace(
+                "/", "-"
+            )
         return api.client.download(url, "GET", path=out_path)
 
 
 # Assignment
 
 
 class Assignor(BaseODPModel):
@@ -283,34 +288,42 @@
         return self._get_model(".model.Continuity").objects.get(
             appl_id=self.appl_id
         )
 
     @property
     def documents(self) -> list[Document]:
         return self._get_model(".model.Document").objects.filter(appl_id=self.appl_id)
-    
+
     @property
     def term_adjustment(self) -> TermAdjustment:
-        return self._get_model(".model.TermAdjustment").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.TermAdjustment").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @property
     def assignments(self) -> list[Assignment]:
         return self._get_model(".model.Assignment").objects.filter(appl_id=self.appl_id)
-    
+
     @property
     def customer_number(self) -> CustomerNumber:
-        return self._get_model(".model.CustomerNumber").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.CustomerNumber").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @property
     def foreign_priority(self) -> ForeignPriority:
-        return self._get_model(".model.ForeignPriority").objects.filter(appl_id=self.appl_id)
-    
+        return self._get_model(".model.ForeignPriority").objects.filter(
+            appl_id=self.appl_id
+        )
+
     @property
     def transactions(self) -> list[Transaction]:
-        return self._get_model(".model.Transaction").objects.filter(appl_id=self.appl_id)
+        return self._get_model(".model.Transaction").objects.filter(
+            appl_id=self.appl_id
+        )
 
     # Aliases
 
     @property
     def biblio(self) -> "USApplicationBiblio":
         return self.bibliographic_data
 
@@ -319,15 +332,31 @@
         return self.application
 
     @property
     def docs(self) -> list[Document]:
         return self.documents
 
 
-class USApplication(USApplicationBiblio):
+class USApplication(BaseODPModel):
+    aia_indicator: YNBool = Field(alias="firstInventorToFileIndicator")
+    app_filing_date: datetime.date = Field(alias="filingDate")
+    inventors: list[Inventor] = Field(alias="inventorBag")
+    customer_number: int = Field(alias="customerNumber")
+    group_art_unit: str = Field(alias="groupArtUnitNumber")
+    invention_title: str = Field(alias="inventionTitle")
+    correspondence_address: list[Address] = Field(alias="correspondenceAddressBag")
+    app_conf_num: int = Field(alias="applicationConfirmationNumber")
+    atty_docket_num: str = Field(alias="docketNumber")
+    appl_id: str = Field(alias="applicationNumberText")
+    first_inventor_name: str = Field(alias="firstInventorName")
+    first_applicant_name: str = Field(alias="firstApplicantName")
+    cpc_classifications: list[str] = Field(alias="cpcClassificationBag")
+    entity_status: str = Field(alias="businessEntityStatusCategory")
+    app_early_pub_number: Optional[str] = Field(alias="earliestPublicationNumber")
+
     app_type_code: str = Field(alias="applicationTypeCode")
     national_stage_indicator: YNBool = Field(alias="nationalStageIndicator")
 
     effective_filing_date: datetime.date = Field(alias="effectiveFilingDate")
     cls_sub_cls: str = Field(alias="class/subclass")
     assignments: list[Assignment] = Field(alias="assignmentBag")
     attorneys: CustomerNumber = Field(alias="recordAttorney")
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/model_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/model_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/query.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/query_fields.csv` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/query_fields.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/odp/util.py` & `patent_client-5.0.1/patent_client/_sync/uspto/odp/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/__init__.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/__init__.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/fixtures/app_1_input.json` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/fixtures/app_1_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 # ********************************************************************************
 
 import datetime
 import logging
 from collections.abc import Sequence
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import TYPE_CHECKING, Iterator
+import typing as tp
 
 from dateutil.parser import parse as dt_parse
 from pypdf import PdfMerger
 
 from patent_client.util.manager import Manager
 from patent_client.util.request_util import get_start_and_row_count
 
 from .api import PatentExaminationDataSystemApi
 from .query import QueryFields
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from .model import Document, USApplication
 
 logger = logging.getLogger(__name__)
 
 
 class HttpException(Exception):
     pass
 
 
 def cast_as_datetime(
-    date: str | datetime.datetime | datetime.date, end_of_day=False
+    date: tp.Union[str, datetime.datetime, datetime.date], end_of_day=False
 ) -> datetime.datetime:
     if isinstance(date, datetime.datetime):
         pass
     elif isinstance(date, str):
         date = dt_parse(date)
     elif isinstance(date, datetime.date):
         date = datetime.datetime.combine(date, datetime.datetime.min.time())
@@ -56,25 +56,29 @@
     default_filter = "appl_id"
 
     def count(self):
         api = PatentExaminationDataSystemApi()
         max_length = (api.create_query(**self.get_query_params())).num_found
         return min(max_length, self.config.limit) if self.config.limit else max_length
 
-    def _get_results(self) -> Iterator["USApplication"]:
+    def _get_results(self) -> tp.Iterator["USApplication"]:
         query_params = self.get_query_params()
         api = PatentExaminationDataSystemApi()
+        counter = 0
         for start, rows in get_start_and_row_count(
             self.config.limit, self.config.offset, page_size=20
         ):
             page = api.create_query(
                 **{**query_params, "start": start, "rows": rows}
             )
             for app in page.applications:
                 yield app
+                counter += 1
+                if self.config.limit and counter >= self.config.limit:
+                    break
             if len(page.applications) < rows:
                 break
 
     def get_query_params(self):
         # Short circuit processing logic if the "query" filter is specified
         if "query" in self.config.filter:
             query_text = self.config.filter["query"]
@@ -192,15 +196,15 @@
 
 class DocumentManager(Manager["Document"]):
     default_filter = "appl_id"
 
     def count(self):
         return len([i for i in self])
 
-    def _get_results(self) -> Iterator["Document"]:
+    def _get_results(self) -> tp.Iterator["Document"]:
         api = PatentExaminationDataSystemApi()
         docs = api.get_documents(self.config.filter["appl_id"][0])
         for doc in docs:
             yield doc
 
     def download(self, docs, path="."):
         if str(path)[-4:].lower() == ".pdf":
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/manager_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 from collections import OrderedDict
 from pathlib import Path
 
 import pytest
 from pypdf import PdfReader
 
-from .model import PedsPage, USApplication
+from .model import PedsPage, USApplication, RemovedDataException
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
 class TestPatentExaminationDataDeserialization:
     def test_application(self):
         input_file = fixtures / "app_1_input.json"
@@ -96,37 +96,41 @@
             "US20050120054A1",
             "US20050188423A1",
         ]
         data = USApplication.objects.filter(app_early_pub_number=nos)
         assert data.count() == 5
 
     
+    @pytest.mark.skip("Continuity information has been removed from PEDS")
     def test_get_child_data(self):
         parent = USApplication.objects.get("14018930")
         child = parent.child_continuity[0]
         assert child.child_appl_id == "14919159"
         assert child.relationship == "claims the benefit of"
         # assert child.child.patent_title == "LEAPFROG TREE-JOIN"
 
     
+    @pytest.mark.skip("Continuity information has been removed from PEDS")
     def test_get_parent_data(self):
         child = USApplication.objects.get("14018930")
         parent = child.parent_continuity[0]
         assert parent.parent_appl_id == "61706484"
         assert parent.relationship == "Claims Priority from Provisional Application"
         assert parent.parent_app_filing_date is not None
         # assert parent.parent.patent_title == "Leapfrog Tree-Join"
 
     
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_pta_history(self):
         app = USApplication.objects.get("14095073")
         pta_history = app.pta_pte_tran_history
         assert len(pta_history) > 10
 
     
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_pta_summary(self):
         app = USApplication.objects.get("14095073")
         expected = OrderedDict(
             [
                 ("kind", "PTA"),
                 ("a_delay", 169),
                 ("pto_delay", 169),
@@ -152,14 +156,15 @@
             "corr_address",
         ]
 
         for k in expected_keys:
             assert getattr(app, k, None) is not None
 
     
+    @pytest.mark.skip("Attorney information has been removed from PEDS")
     def test_attorneys(self):
         app = USApplication.objects.get("14095073")
         assert len(app.attorneys) > 1
         actual = app.attorneys[0].model_dump()
         assert int(actual["registration_no"]) > 1000
         expected_keys = [
             "registration_no",
@@ -178,14 +183,15 @@
             for a in apps:
                 counter += 1
         except KeyError as e:
             raise e
         assert apps.count() == counter
 
     
+    @pytest.mark.skip("PTA information has been removed from PEDS")
     def test_expiration_date(self):
         app = USApplication.objects.get("15384723")
         expected = {
             "parent_appl_id": "12322218",
             "parent_app_filing_date": datetime.date(2009, 1, 29),
             "parent_relationship": "is a Continuation in part of",
             "initial_term": datetime.date(2029, 1, 29),
@@ -208,14 +214,15 @@
             "terminal_disclaimer_filed": False,
         }
         actual = dict(app.expiration)
         for k in expected.keys():
             assert expected[k] == actual[k]
 
     
+    @pytest.mark.skip("Expiration date is not supported for PCT applications")
     def test_expiration_date_for_pct_apps(self):
         app = USApplication.objects.get("PCT/US2014/020588")
         with pytest.raises(Exception) as exc:
             _ = app.expiration
         assert exc.match("Expiration date not supported for PCT Applications")
 
     
@@ -225,14 +232,35 @@
         assert isinstance(fp, list)
         app = fp[0]
         assert app.country_name == "NORWAY"
         assert app.filing_date == datetime.date(2017, 2, 15)
         assert app.priority_claim == "20170229"
 
 
+    
+    def test_raises_warning_on_missing_information(self):
+        app = USApplication.objects.get(patent_number=10000000)
+        with pytest.raises(RemovedDataException):
+            _ = app.expiration
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.attorneys
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.pta_pte_summary
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.pta_pte_tran_history
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.parent_continuity
+            
+        with pytest.raises(RemovedDataException):
+            _ = app.child_continuity
+
 class TestDocuments:
     @pytest.mark.vcr
     def test_can_get_document_listing(self):
         app = USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         assert docs.count() > 50
 
@@ -240,36 +268,9 @@
     def test_can_get_application_from_document(self):
         app = USApplication.objects.get(patent_number=10000000)
         docs = app.documents
         doc = docs[5]
         backref_app = doc.application
         assert app.appl_id == backref_app.appl_id
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    def test_can_download_document(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        doc = app.documents.to_list()[-1]
-        result = doc.download(path=tmp_path)
-        assert "14643719 - 2015-03-10 - IDS" in str(result)
-        assert result.exists()
-        assert len(list(tmp_path.glob("*.pdf"))) == 1
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    def test_can_download_document_without_appl_id(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        doc = app.documents.to_list()[-1]
-        result = doc.download(path=tmp_path, include_appl_id=False)
-        assert "2015-03-10 - IDS" in str(result)
-        assert "14643719" not in str(result)
-        assert result.exists()
-        assert len(list(tmp_path.glob("*.pdf"))) == 1
 
-    @pytest.mark.skip("Downloading currently doesn't work")
-    @pytest.mark.vcr
-    def test_multiple_document_download(self, tmp_path):
-        app = USApplication.objects.get(patent_number=10000000)
-        docs = app.documents.to_list()[-2:]
-        result = app.documents.download(docs, path=tmp_path)
-        reader = PdfReader(str(result))
-        assert reader.numPages == 8
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/model.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *            Source File: patent_client/_async/uspto/peds/model.py             *
 # ********************************************************************************
 
 import datetime
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, List, Optional
+import typing as tp
 
 
 from dateutil.relativedelta import relativedelta
 from pydantic import (
     AliasPath,
     BeforeValidator,
     ConfigDict,
@@ -19,30 +19,34 @@
     model_validator,
 )
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated, Self
 
 from patent_client.util.pydantic_util import BaseModel, Date, DateTime
 
-if TYPE_CHECKING:
-    from ..public_search.model import Patent, PublishedApplication
-    from ..ptab.model import PtabProceeding
+if tp.TYPE_CHECKING:
     from ...epo.ops.published.model import InpadocBiblio
+    from ..ptab.model import PtabProceeding
+    from ..public_search.model import Patent, PublishedApplication
 
 
 def parse_mdy_date(string: str) -> datetime.date:
     try:
         return datetime.datetime.strptime(string, "%m-%d-%Y").date()
     except ValueError:
         return None
 
 
-MDYDate = Annotated[Optional[datetime.date], BeforeValidator(parse_mdy_date)]
+class RemovedDataException(Exception):
+    pass
+
+
+MDYDate = Annotated[tp.Optional[datetime.date], BeforeValidator(parse_mdy_date)]
 YNBool = Annotated[bool, BeforeValidator(lambda x: x == "Y")]
-OptionalInt = Annotated[Optional[int], BeforeValidator(lambda x: int(x) if x else None)]
+OptionalInt = Annotated[tp.Optional[int], BeforeValidator(lambda x: int(x) if x else None)]
 RelationshipStr = Annotated[
     str, BeforeValidator(lambda x: x.replace("This application ", "").strip())
 ]
 ConveyanceStr = Annotated[
     str, BeforeValidator(lambda x: x.replace(" (SEE DOCUMENT FOR DETAILS).", ""))
 ]
 
@@ -56,62 +60,23 @@
 
 class Transactions(PEDSBaseModel):
     record_date: Date
     code: str
     description: str
 
 
-class PtaOrPteTransactionHistory(PEDSBaseModel):
-    number: float
-    pta_or_pte_date: MDYDate
-    contents_description: str
-    pto_days: OptionalInt
-    appl_days: OptionalInt
-    start: float
-
-
-class PtaOrPteSummary(PEDSBaseModel):
-    a_delay: int
-    b_delay: int
-    c_delay: int
-    pto_adjustments: int
-    total_days: int = Field(alias="totalPtoDays")
-    kind: str = Field(alias="ptaPteInd")
-    pto_delay: int
-    applicant_delay: int = Field(alias="applDelay")
-    overlap_delay: int
-
-
-class ParentApplication(PEDSBaseModel):
-    parent_appl_id: str = Field(alias="claimApplicationNumberText")
-    child_appl_id: str = Field(alias="applicationNumberText")
-    parent_app_filing_date: MDYDate = Field(alias="filingDate")
-    parent_patent_number: str = Field(alias="patentNumberText")
-    parent_status: str = Field(alias="applicationStatus")
-    relationship: RelationshipStr = Field(alias="applicationStatusDescription")
-
-
-class ChildApplication(PEDSBaseModel):
-    child_appl_id: str = Field(alias="claimApplicationNumberText")
-    parent_appl_id: str = Field(alias="applicationNumberText")
-    child_app_filing_date: MDYDate = Field(alias="filingDate")
-    child_patent_number: str = Field(alias="patentNumberText")
-    child_status: str = Field(alias="applicationStatus")
-    relationship: RelationshipStr = Field(alias="applicationStatusDescription")
-
-
 class ForeignPriority(PEDSBaseModel):
     priority_claim: str
     country_name: str
     filing_date: MDYDate
 
 
 class AttorneyOrAgent(PEDSBaseModel):
-    application_id: Optional[str] = None
-    registration_no: Optional[str] = None
+    application_id: tp.Optional[str] = None
+    registration_no: tp.Optional[str] = None
     full_name: str
     phone_num: str
     reg_status: str
 
 
 class Inventor(PEDSBaseModel):
     name: str
@@ -138,76 +103,97 @@
     correspondent_name: str = Field(alias="addressNameText")
     mail_date: MDYDate
     received_date: MDYDate
     recorded_date: MDYDate
     pages: OptionalInt = Field(alias="pagesCount", default=None)
     conveyance: ConveyanceStr = Field(alias="converyanceName")
     sequence_number: int
-    assignors: Optional[List[Assignor]] = Field(alias="assignors", default_factory=list)
-    assignees: Optional[List[Assignee]] = Field(alias="assignee", default_factory=list)
+    assignors: tp.Optional[tp.List[Assignor]] = Field(alias="assignors", default_factory=list)
+    assignees: tp.Optional[tp.List[Assignee]] = Field(alias="assignee", default_factory=list)
 
     @computed_field
     @property
     def reel_frame(self) -> str:
         return f"{self.reel_number}/{self.frame_number}"
 
 
 class USApplication(PEDSBaseModel):
     appl_id: str
     app_filing_date: Date
-    app_exam_name: Optional[str] = None
+    app_exam_name: tp.Optional[str] = None
     public_ind: YNBool
-    inventor_name: Optional[str] = None
-    app_early_pub_number: Optional[str] = None
-    app_early_pub_date: Optional[Date] = None
-    patent_number: Optional[str] = None
-    patent_issue_date: Optional[Date] = None
-    app_location: Optional[str] = None
-    app_grp_art_number: Optional[str] = None
+    inventor_name: tp.Optional[str] = None
+    app_early_pub_number: tp.Optional[str] = None
+    app_early_pub_date: tp.Optional[Date] = None
+    patent_number: tp.Optional[str] = None
+    patent_issue_date: tp.Optional[Date] = None
+    app_location: tp.Optional[str] = None
+    app_grp_art_number: tp.Optional[str] = None
     last_modified: DateTime = Field(alias="LAST_MOD_TS")
     last_insert_time: DateTime = Field(alias="LAST_INSERT_TIME")
-    patent_title: Optional[str] = None
-
-    app_attr_dock_number: Optional[str] = None
-    app_status: Optional[str] = None
-    app_status_date: Optional[Date] = None
-    app_type: Optional[str] = None
-    app_cls_sub_cls: Optional[str] = None
-    corr_name: Optional[str] = None
-    corr_address: Optional[str] = None
-    corr_cust_no: Optional[str] = Field(alias="corrAddrCustNo", default=None)
-    transactions: List[Transactions]
-    attorneys: List[AttorneyOrAgent] = Field(alias="attrnyAddr", default_factory=list)
-    inventors: List[Inventor] = Field(default_factory=list)
-    applicants: List[Applicant] = Field(default_factory=list)
-    pta_pte_summary: Optional[PtaOrPteSummary] = None
-    pta_pte_tran_history: List[PtaOrPteTransactionHistory] = Field(default_factory=list)
-    parent_continuity: List[ParentApplication] = Field(default_factory=list)
-    child_continuity: List[ChildApplication] = Field(default_factory=list)
-    foreign_priority: List[ForeignPriority] = Field(default_factory=list)
-    assignments: List[Assignment] = Field(default_factory=list)
+    patent_title: tp.Optional[str] = None
+    app_attr_dock_number: tp.Optional[str] = None
+    app_status: tp.Optional[str] = None
+    app_status_date: tp.Optional[Date] = None
+    app_type: tp.Optional[str] = None
+    app_cls_sub_cls: tp.Optional[str] = None
+    corr_name: tp.Optional[str] = None
+    corr_address: tp.Optional[str] = None
+    corr_cust_no: tp.Optional[str] = Field(alias="corrAddrCustNo", default=None)
+    transactions: tp.List[Transactions]
+    inventors: tp.List[Inventor] = Field(default_factory=list)
+    applicants: tp.List[Applicant] = Field(default_factory=list)
+    foreign_priority: tp.List[ForeignPriority] = Field(default_factory=list)
+    assignments: tp.List[Assignment] = Field(default_factory=list)
 
     def __repr__(self):
         return f"USApplication(appl_id='{self.appl_id}', patent_title='{self.patent_title}', app_status='{self.app_status}')"
 
+    # Data removed by USPTO
+
+    @property
+    def attorneys(self):
+        raise RemovedDataException("Attorney information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+
+    @property
+    def expiration(self):
+        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def pta_pte_summary(self):
+        raise RemovedDataException("PTA information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def pta_pte_tran_history(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def parent_continuity(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+    
+    @property
+    def child_continuity(self):
+        raise RemovedDataException("Continuity information is no longer available in PEDS. Use the ODP client to retrieve this information:\nhttps://patent-client.readthedocs.io/en/latest/user_guide/open_data_portal.html")
+
+
     @property
     def patent_center_link(self) -> str:
         return f"https://patentcenter.uspto.gov/applications/{self.appl_id}"
 
     @property
-    def google_patents_link(self) -> Optional[str]:
+    def google_patents_link(self) -> tp.Optional[str]:
         if self.patent_number is not None:
             return f"https://patents.google.com/patent/US{self.patent_number}/en"
         elif self.app_early_pub_number is not None:
             return f"https://patents.google.com/patent/{self.app_early_pub_number}/en"
         else:
             return None
 
     @property
-    def continuity(self) -> List[Self]:
+    def continuity(self) -> tp.List["Self"]:
         """Returns a complete set of parents, self, and children"""
         return list(
             [
                 *self.child_continuity.values_list("child", flat=True),
                 self,
                 *self.parent_continuity.values_list("parent", flat=True),
             ]
@@ -223,127 +209,79 @@
         return "Nonprovisional"
 
     @property
     def publication_number(self):
         return self.app_early_pub_number[2:-2]
 
     @property
-    def priority_date(self) -> Optional[datetime.date]:
+    def priority_date(self) -> tp.Optional[datetime.date]:
         """Attempts to return the priority date of the application, calculated as
         the earliest application filing date among the application's parents, or
         its own filing date if it has no parents. Does not include foreign priority
         """
         if not self.parent_continuity:
             return self.app_filing_date
         else:
             return sorted(p.parent_app_filing_date for p in self.parent_continuity)[0]
 
-    @property
-    def expiration(self) -> Optional["Expiration"]:
-        """Calculates expiration data from which the expiration date can be calculated. See
-        help information for the resulting Expiration model.
-        """
-        if "PCT" in self.appl_id:
-            raise NotImplementedError(
-                "Expiration date not supported for PCT Applications"
-            )
-        if not self.patent_number:
-            return None
-        expiration_data = dict()
-        term_parents = [
-            p
-            for p in self.parent_continuity
-            if p.relationship
-            not in ["Claims Priority from Provisional Application", "is a Reissue of"]
-        ]
-        if term_parents:
-            term_parent = sorted(term_parents, key=lambda x: x.parent_app_filing_date)[
-                0
-            ]
-            relationship = term_parent.relationship
-            parent_filing_date = term_parent.parent_app_filing_date
-            parent_appl_id = term_parent.parent_appl_id
-        else:
-            relationship = "self"
-            parent_appl_id = self.appl_id
-            parent_filing_date = self.app_filing_date
-
-        expiration_data["parent_appl_id"] = parent_appl_id
-        expiration_data["parent_app_filing_date"] = parent_filing_date
-        expiration_data["parent_relationship"] = relationship
-        expiration_data["initial_term"] = parent_filing_date + relativedelta(years=20)  # type: ignore
-        expiration_data["pta_or_pte"] = self.pta_pte_summary.total_days or 0  # type: ignore
-        expiration_data["extended_term"] = expiration_data[
-            "initial_term"
-        ] + relativedelta(days=expiration_data["pta_or_pte"])  # type: ignore
-
-        transactions = self.transactions
-        try:
-            _ = next(t for t in transactions if t.code == "DIST")
-            expiration_data["terminal_disclaimer_filed"] = True
-        except StopIteration:
-            expiration_data["terminal_disclaimer_filed"] = False
-
-        return Expiration(**expiration_data)  # type: ignore
-
     # Related objects
     @property
-    def documents(self) -> "Iterable[Document]":
+    def documents(self) -> tp.Iterable["Document"]:
         """File History Documents from PEDS CMS"""
         return self._get_model(".Document").objects.filter(appl_id=self.appl_id)
 
     @property
     def related_assignments(
         self,
-    ) -> "Iterable[Assignment]":
+    ) -> tp.Iterable["Assignment"]:
         """Related Assignments from the Assignments API"""
         return self._get_model("..assignment.model.Assignment").objects.filter(
             appl_id=self.appl_id
         )
 
     @property
     def ptab_proceedings(
         self,
-    ) -> "Iterable[PtabProceeding]":
+    ) -> tp.Iterable["PtabProceeding"]:
         """Related PtabProceedings for this application"""
         return self._get_model("..ptab.model.PtabProceeding").objects.filter(
             appl_id=self.appl_id
         )
 
     @property
-    def patent(self) -> "Optional[Patent]":
+    def patent(self) -> tp.Optional["Patent"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("..public_search.model.Patent").objects.get(
             publication_number=self.patent_number
         )
 
     @property
     def publication(
         self,
-    ) -> "Optional[PublishedApplication]":
+    ) -> tp.Optional["PublishedApplication"]:
         """Fulltext version of the Publication - If Available"""
         return self._get_model(
             "..public_search.model.PublishedApplication"
         ).objects.get(
             publication_number=self.publication_number,
         )
 
     @property
     def inpadoc_patent(
         self,
-    ) -> "Optional[InpadocBiblio]":
+    ) -> tp.Optional["InpadocBiblio"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=f"US{self.patent_number}",
         )
 
     @property
     def inpadoc_publication(
         self,
-    ) -> "Optional[InpadocBiblio]":
+    ) -> tp.Optional["InpadocBiblio"]:
         """Fulltext version of the patent - If Available"""
         return self._get_model("...epo.ops.published.model.InpadocBiblio").objects.get(
             publication_number=self.app_early_pub_number,
         )
 
     @model_validator(mode="before")
     @classmethod
@@ -440,17 +378,17 @@
     mail_room_date: Date
     document_code: str
     document_description: str
     document_category: str
     access_level_category: str
     document_identifier: str
     page_count: int
-    pdf_url: Optional[str] = None
+    pdf_url: tp.Optional[str] = None
 
-    def download(self, path: Optional[str | Path]) -> Path:
+    def download(self, path: tp.Optional[tp.Union[str, Path]] = None) -> Path:
         from .api import client
 
         if self.pdf_url is None:
             raise ValueError("No PDF URL available")
         full_url = f"https://ped.uspto.gov/api/queries/cms/{self.pdf_url}"
         out_path = client.download(full_url, path=path)
         return out_path
@@ -465,10 +403,10 @@
 
 class PedsPage(PEDSBaseModel):
     num_found: int = Field(
         validation_alias=AliasPath(
             "queryResults", "searchResponse", "response", "numFound"
         )
     )
-    applications: List[USApplication] = Field(
+    applications: tp.List[USApplication] = Field(
         validation_alias=AliasPath("queryResults", "searchResponse", "response", "docs")
     )
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/query.py` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/peds/search_index.csv` & `patent_client-5.0.1/patent_client/_sync/uspto/peds/search_index.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/__init__.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *           Source File: patent_client/_async/uspto/ptab/__init__.py           *
 # ********************************************************************************
 
-import json
-from pathlib import Path
-
 __api_name__ = "PTAB API v2"
 
 from .model import PtabDecision, PtabDocument, PtabProceeding  # noqa: F401,E402
+
+__all__ = [
+    "PtabDecision",
+    "PtabDocument",
+    "PtabProceeding",
+]
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/api.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/documents_input.json` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/documents_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/fixtures/proceeding_input.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/model.py` & `patent_client-5.0.1/patent_client/_async/uspto/ptab/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-# ********************************************************************************
-# *         WARNING: This file is automatically generated by unasync.py.         *
-# *                             DO NOT MANUALLY EDIT                             *
-# *            Source File: patent_client/_async/uspto/ptab/model.py             *
-# ********************************************************************************
-
 import datetime
 import re
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional
+import typing as tp
 
 from pydantic import BeforeValidator, ConfigDict, Field
 from pydantic.alias_generators import to_camel
 from typing_extensions import Annotated
 
 from patent_client.util.pydantic_util import BaseModel, DateTime
 
-if TYPE_CHECKING:
+if tp.TYPE_CHECKING:
     from ..peds.model import USApplication
 
 MDYDate = Annotated[
     datetime.date,
     BeforeValidator(lambda x: datetime.datetime.strptime(x, "%m-%d-%Y").date()),
 ]
 
@@ -28,96 +22,96 @@
     model_config = ConfigDict(
         alias_generator=to_camel,
         str_strip_whitespace=True,
     )
 
 
 class AdditionalRespondent(PtabBaseModel):
-    application_number_text: Optional[str] = None
-    inventor_name: Optional[str] = None
-    patent_number: Optional[str] = None
-    party_name: Optional[str] = None
+    application_number_text: tp.Optional[str] = None
+    inventor_name: tp.Optional[str] = None
+    patent_number: tp.Optional[str] = None
+    party_name: tp.Optional[str] = None
 
 
 class PtabProceeding(PtabBaseModel):
     """A PTAB Proceeding - e.g. IPR/CBM/DER Trial, Patent Appeal, Interference, etc.
 
     All fields are query-able. Date ranges can be formed by inserting "from" or "to" on a query
     for a date range.
 
     """
 
     # Proceeding Metadata
-    last_modified_date: Optional[DateTime] = None
-    last_modified_user_id: Optional[DateTime] = None
-    institution_decision_date: Optional[MDYDate] = None
-    proceeding_filing_date: Optional[MDYDate] = None
-    accorded_filing_date: Optional[MDYDate] = None
-    proceeding_status_category: Optional[str] = None
-    proceeding_number: Optional[str] = None
-    proceeding_last_modified_date: Optional[MDYDate] = None
-    proceeding_type_category: Optional[str] = None
-    subproceeding_type_category: Optional[str] = None
-    decision_date: Optional[MDYDate] = None
-    docket_notice_mail_date: Optional[MDYDate] = None
-    declaration_date: Optional[MDYDate] = None
-    style_name_text: Optional[str] = None
+    last_modified_date: tp.Optional[DateTime] = None
+    last_modified_user_id: tp.Optional[DateTime] = None
+    institution_decision_date: tp.Optional[MDYDate] = None
+    proceeding_filing_date: tp.Optional[MDYDate] = None
+    accorded_filing_date: tp.Optional[MDYDate] = None
+    proceeding_status_category: tp.Optional[str] = None
+    proceeding_number: tp.Optional[str] = None
+    proceeding_last_modified_date: tp.Optional[MDYDate] = None
+    proceeding_type_category: tp.Optional[str] = None
+    subproceeding_type_category: tp.Optional[str] = None
+    decision_date: tp.Optional[MDYDate] = None
+    docket_notice_mail_date: tp.Optional[MDYDate] = None
+    declaration_date: tp.Optional[MDYDate] = None
+    style_name_text: tp.Optional[str] = None
 
     # Respondent Information
-    respondent_technology_center_number: Optional[str] = None
-    respondent_patent_owner_name: Optional[str] = None
-    respondent_party_name: Optional[str] = None
-    respondent_group_art_unit_number: Optional[str] = None
-    respondent_inventor_name: Optional[str] = None
-    respondent_counsel_name: Optional[str] = None
-    respondent_grant_date: Optional[MDYDate] = None
-    respondent_patent_number: Optional[str] = None
-    respondent_application_number_text: Optional[str] = None
-    respondent_publication_number: Optional[str] = None
-    respondent_publication_date: Optional[MDYDate] = None
+    respondent_technology_center_number: tp.Optional[str] = None
+    respondent_patent_owner_name: tp.Optional[str] = None
+    respondent_party_name: tp.Optional[str] = None
+    respondent_group_art_unit_number: tp.Optional[str] = None
+    respondent_inventor_name: tp.Optional[str] = None
+    respondent_counsel_name: tp.Optional[str] = None
+    respondent_grant_date: tp.Optional[MDYDate] = None
+    respondent_patent_number: tp.Optional[str] = None
+    respondent_application_number_text: tp.Optional[str] = None
+    respondent_publication_number: tp.Optional[str] = None
+    respondent_publication_date: tp.Optional[MDYDate] = None
 
     # Petitioner Information
-    petitioner_technology_center_number: Optional[str] = None
-    petitioner_patent_owner_name: Optional[str] = None
-    petitioner_party_name: Optional[str] = None
-    petitioner_group_art_unit_number: Optional[str] = None
-    petitioner_inventor_name: Optional[str] = None
-    petitioner_counsel_name: Optional[str] = None
-    petitioner_grant_date: Optional[MDYDate] = None
-    petitioner_patent_number: Optional[str] = None
-    petitioner_application_number_text: Optional[str] = None
+    petitioner_technology_center_number: tp.Optional[str] = None
+    petitioner_patent_owner_name: tp.Optional[str] = None
+    petitioner_party_name: tp.Optional[str] = None
+    petitioner_group_art_unit_number: tp.Optional[str] = None
+    petitioner_inventor_name: tp.Optional[str] = None
+    petitioner_counsel_name: tp.Optional[str] = None
+    petitioner_grant_date: tp.Optional[MDYDate] = None
+    petitioner_patent_number: tp.Optional[str] = None
+    petitioner_application_number_text: tp.Optional[str] = None
 
     # Appellant Information
-    appellant_technology_center_number: Optional[str] = None
-    appellant_patent_owner_name: Optional[str] = None
-    appellant_party_name: Optional[str] = None
-    appellant_group_art_unit_number: Optional[str] = None
-    appellant_inventor_name: Optional[str] = None
-    appellant_counsel_name: Optional[str] = None
-    appellant_grant_date: Optional[MDYDate] = None
-    appellant_patent_number: Optional[str] = None
-    appellant_application_number_text: Optional[str] = None
-    appellant_publication_date: Optional[MDYDate] = None
-    appellant_publication_number: Optional[str] = None
-    third_party_name: Optional[str] = None
+    appellant_technology_center_number: tp.Optional[str] = None
+    appellant_patent_owner_name: tp.Optional[str] = None
+    appellant_party_name: tp.Optional[str] = None
+    appellant_group_art_unit_number: tp.Optional[str] = None
+    appellant_inventor_name: tp.Optional[str] = None
+    appellant_counsel_name: tp.Optional[str] = None
+    appellant_grant_date: tp.Optional[MDYDate] = None
+    appellant_patent_number: tp.Optional[str] = None
+    appellant_application_number_text: tp.Optional[str] = None
+    appellant_publication_date: tp.Optional[MDYDate] = None
+    appellant_publication_number: tp.Optional[str] = None
+    third_party_name: tp.Optional[str] = None
 
     # Second Respondent (if any)
-    second_respondent_party_name: Optional[str] = None
-    second_respondent_appl_number_text: Optional[str] = None
-    second_respondent_patent_number: Optional[str] = None
-    second_respondent_grant_date: Optional[MDYDate] = None
-    second_respondent_patent_owner_name: Optional[str] = None
-    second_respondent_inventor_name: Optional[str] = None
-    second_respondent_counsel_name: Optional[str] = None
-    second_respondent_g_a_u_number: Optional[str] = None
-    second_respondent_tech_center_number: Optional[str] = None
-    second_respondent_pub_number: Optional[str] = None
-    second_respondent_publication_date: Optional[MDYDate] = None
+    second_respondent_party_name: tp.Optional[str] = None
+    second_respondent_appl_number_text: tp.Optional[str] = None
+    second_respondent_patent_number: tp.Optional[str] = None
+    second_respondent_grant_date: tp.Optional[MDYDate] = None
+    second_respondent_patent_owner_name: tp.Optional[str] = None
+    second_respondent_inventor_name: tp.Optional[str] = None
+    second_respondent_counsel_name: tp.Optional[str] = None
+    second_respondent_g_a_u_number: tp.Optional[str] = None
+    second_respondent_tech_center_number: tp.Optional[str] = None
+    second_respondent_pub_number: tp.Optional[str] = None
+    second_respondent_publication_date: tp.Optional[MDYDate] = None
 
-    additional_respondents: List[str] = Field(default_factory=list)
+    additional_respondents: tp.List[str] = Field(default_factory=list)
 
     @property
     def documents(
         self,
     ) -> "list[PtabDocument]":
         """Documents associated with the Proceeding"""
         return self._get_model(".model.PtabDocument").objects.filter(
@@ -144,73 +138,73 @@
 
 
 fname_re = re.compile(r"[<>:\"/\|?*]")
 
 
 class PtabDocument(PtabBaseModel):
     document_identifier: str = Field(repr=False, default=None)
-    document_category: Optional[str] = None
-    document_type_name: Optional[str] = None
-    document_number: Optional[int] = None
-    document_name: Optional[str] = None
-    document_filing_date: Optional[MDYDate] = None
-    proceeding_number: Optional[str] = None
-    proceeding_type_category: Optional[str] = Field(repr=False, default=None)
-    title: Optional[str] = None
+    document_category: tp.Optional[str] = None
+    document_type_name: tp.Optional[str] = None
+    document_number: tp.Optional[int] = None
+    document_name: tp.Optional[str] = None
+    document_filing_date: tp.Optional[MDYDate] = None
+    proceeding_number: tp.Optional[str] = None
+    proceeding_type_category: tp.Optional[str] = Field(repr=False, default=None)
+    title: tp.Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
         return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
-    def download(self, path: Optional[str | Path]) -> Path:
+    async def download(self, path: tp.Optional[tp.Union[str, Path]]) -> Path:
         from .api import client
 
         name, ext = self.document_name.rsplit(".", 1)
         name = name[:100] + "." + ext
         filename = f"[{str(self.document_number).rjust(4, '0')}] {self.document_filing_date.isoformat()} - {name}"
         filename = filename.encode(encoding="ascii", errors="ignore").decode("ascii")
         filename = fname_re.sub("", filename)
         out_path = Path(path) if path else Path.cwd()
         if out_path.is_dir():
             out_path = Path(path) / filename
         else:
             out_path = out_path
         download_url = f"https://developer.uspto.gov/ptab-api/documents/{self.document_identifier}/download"
-        return client.download(download_url, path=out_path)
+        return await client.download(download_url, path=out_path)
 
 
 class PtabDecision(PtabBaseModel):
     proceeding_number: str
-    board_rulings: List[str] = Field(default_factory=list)
-    decision_type_category: Optional[str] = None
-    document_identifier: Optional[str] = None
-    document_name: Optional[str] = None
-    identifier: Optional[str] = None
-    subdecision_type_category: Optional[str] = None
-    issue_type: List[str] = Field(default_factory=list)
-    object_uu_id: Optional[str] = None
-    petitioner_technology_center_number: Optional[str] = None
+    board_rulings: tp.List[str] = Field(default_factory=list)
+    decision_type_category: tp.Optional[str] = None
+    document_identifier: tp.Optional[str] = None
+    document_name: tp.Optional[str] = None
+    identifier: tp.Optional[str] = None
+    subdecision_type_category: tp.Optional[str] = None
+    issue_type: tp.List[str] = Field(default_factory=list)
+    object_uu_id: tp.Optional[str] = None
+    petitioner_technology_center_number: tp.Optional[str] = None
 
     @property
     def proceeding(self) -> "PtabProceeding":
         """The PTAB proceeding associated with the document"""
         return self._get_model(".model.PtabProceeding").objects.get(
             proceeding_number=self.proceeding_number
         )
 
 
 class PtabDocumentPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabDocument] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabDocument] = Field(alias="results", default_factory=list)
 
 
 class PtabProceedingPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabProceeding] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabProceeding] = Field(alias="results", default_factory=list)
 
 
 class PtabDecisionPage(PtabBaseModel):
-    num_found: Optional[int] = Field(alias="recordTotalQuantity")
-    docs: List[PtabDecision] = Field(alias="results", default_factory=list)
+    num_found: tp.Optional[int] = Field(alias="recordTotalQuantity")
+    docs: tp.List[PtabDecision] = Field(alias="results", default_factory=list)
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/ptab/util.py` & `patent_client-5.0.1/patent_client/_sync/uspto/ptab/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/__init__.py` & `patent_client-5.0.1/patent_client/_async/uspto/public_search/model/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,29 @@
-# ********************************************************************************
-# *         WARNING: This file is automatically generated by unasync.py.         *
-# *                             DO NOT MANUALLY EDIT                             *
-# *      Source File: patent_client/_async/uspto/public_search/__init__.py       *
-# ********************************************************************************
-
-from .model import (
-    Patent,
-    PatentBiblio,
-    PublicSearchBiblio,
-    PublicSearchDocument,
-    PublishedApplication,
-    PublishedApplicationBiblio,
-)
+from .biblio import PublicSearchBiblio, PublicSearchBiblioPage
+from .document import PublicSearchDocument
+
+
+class PatentBiblio(PublicSearchBiblio):
+    pass
+
+
+class Patent(PublicSearchDocument):
+    pass
+
+
+class PublishedApplicationBiblio(PublicSearchBiblio):
+    pass
+
+
+class PublishedApplication(PublicSearchDocument):
+    pass
+
+
+__all__ = [
+    "PatentBiblio",
+    "Patent",
+    "PublishedApplicationBiblio",
+    "PublishedApplication",
+    "PublicSearchBiblio",
+    "PublicSearchDocument",
+    "PublicSearchDocument",
+]
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/api.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # *         Source File: patent_client/_async/uspto/public_search/api.py         *
 # ********************************************************************************
 
 import asyncio
 import json
 from copy import deepcopy
 from pathlib import Path
+
 import httpx
 
 from patent_client._sync.http_client import PatentClientSession
 
 from .model import PublicSearchBiblioPage, PublicSearchDocument
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/api_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/api_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/biblio.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/document.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert/shared.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/convert_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/convert_test.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # *                             DO NOT MANUALLY EDIT                             *
 # *    Source File: patent_client/_async/uspto/public_search/convert_test.py     *
 # ********************************************************************************
 
 import json
 from pathlib import Path
 
-fixtures = Path(__file__).parent / "fixtures"
-
 from .convert.biblio import PublicSearchBiblioPageSchema
 from .convert.document import PublicSearchDocumentSchema
 
+fixtures = Path(__file__).parent / "fixtures"
+
 
 def test_convert_biblio():
     input_file = fixtures / "biblio.json"
     output_file = fixtures / "biblio_convert.json"
     input_data = json.loads(input_file.read_text())
     output_data = PublicSearchBiblioPageSchema().deserialize(input_data)
     # output_file.write_text(output_data.to_json(indent=2))
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/count_query.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/count_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/biblio_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_convert.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/fixtures/doc_output.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/fixtures/doc_output.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/manager_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/manager_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/biblio.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/biblio.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/document.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/document.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/model/shared.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model/shared.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/model_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # ********************************************************************************
 # *         WARNING: This file is automatically generated by unasync.py.         *
 # *                             DO NOT MANUALLY EDIT                             *
 # *     Source File: patent_client/_async/uspto/public_search/model_test.py      *
 # ********************************************************************************
 
+import datetime
 import json
 from pathlib import Path
 
 from patent_client.util.test import compare_dicts, compare_lists
 
 from .model.biblio import PublicSearchBiblioPage
 from .model.document import PublicSearchDocument
 
 fixtures = Path(__file__).parent / "fixtures"
 
 
-import datetime
-
-
 def json_serial(obj):
     """JSON serializer for objects not serializable by default json code"""
 
     if isinstance(obj, (datetime.datetime, datetime.date)):
         return obj.isoformat()
     raise TypeError("Type %s not serializable" % type(obj))
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/query.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_config.csv` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_config.csv`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/query_test.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/query_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 
     def test_error_query(self):
         with pytest.raises(QueryException):
             PatentBiblioManager().filter(blargh="2021-01-01")._query
 
     def test_error_date_query(self):
         with pytest.raises(QueryException):
-            q = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
+            _ = PatentBiblioManager().filter(app_filing_date="2021-00-01")._query
         with pytest.raises(QueryException):
-            q = PatentBiblioManager().filter(app_filing_date=False)._query
+            _ = PatentBiblioManager().filter(app_filing_date=False)._query
 
     def test_multiple_fields(self):
         assert (
             PatentBiblioManager().filter("6103599", app_filing_date="2021-01-01")._query
             == '@APD="20210101" AND "6103599".PN.'
         )
         assert (
```

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/search_query.json` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/search_query.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/_sync/uspto/public_search/util.py` & `patent_client-5.0.1/patent_client/_sync/uspto/public_search/util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/parser.py` & `patent_client-5.0.1/patent_client/parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/session.py` & `patent_client-5.0.1/patent_client/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import warnings
 from hashlib import blake2b
 from pathlib import Path
-from typing import Optional
+import typing as tp
 
 import hishel
 import httpcore
 import httpx
 from hishel._utils import normalized_url
 
 from patent_client import CACHE_DIR
@@ -63,15 +63,15 @@
             path = path / filename if path else Path.cwd() / filename
         return path
 
     async def download(
         self,
         url,
         method: str = "GET",
-        path: Optional[str | Path] = None,
+        path: tp.Optional[tp.Union[str, Path]] = None,
         show_progress: bool = False,
         **kwargs,
     ):
         # Ensure we skip the cache for file downloads
         kwargs["extensions"] = kwargs.get("extensions", dict())
         if "force_cache" in kwargs["extensions"]:
             raise ValueError("force_cache is not supported for file downloads")
```

### Comparing `patent_client-5.0.0/patent_client/settings.py` & `patent_client-5.0.1/patent_client/settings.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/test_parser.py` & `patent_client-5.0.1/patent_client/test_parser.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/asyncio_util.py` & `patent_client-5.0.1/patent_client/util/asyncio_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.json` & `patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/claims/examples/multiple_dependent.txt` & `patent_client-5.0.1/patent_client/util/claims/examples/multiple_dependent.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/claims/examples/published_claims.json` & `patent_client-5.0.1/patent_client/util/claims/examples/published_claims.json`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/claims/examples/published_claims.txt` & `patent_client-5.0.1/patent_client/util/claims/examples/published_claims.txt`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/claims/model.py` & `patent_client-5.0.1/patent_client/util/claims/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import textwrap
-from typing import *
+from typing import List
 
 from pydantic import Field
 
 from ..pydantic_util import BaseModel
 
 
 class Claim(BaseModel):
```

### Comparing `patent_client-5.0.0/patent_client/util/claims/parser.py` & `patent_client-5.0.1/patent_client/util/claims/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 
 DEPENDENCY_RE = re.compile(r"claims? (?P<number>[\d,or ]+)", flags=re.IGNORECASE)
 DEPENDENT_CLAIMS_RE = re.compile(r"(?P<number>\d+)([^\d]|$)")
 DEPEND_ALL_RE = re.compile(
     r"(any of the foregoing claims|any of the previous claims)", flags=re.IGNORECASE
 )
 
-clean_text = lambda text: WHITESPACE_RE.sub(" ", text).strip()
+
+def clean_text(text):
+    return WHITESPACE_RE.sub(" ", text).strip()
 
 
 def grouper(iterable, n, fillvalue=None):
     "Collect data into fixed-length chunks or blocks"
     # grouper('ABCDEFG', 3, 'x') --> ABC DEF Gxx"
     args = [iter(iterable)] * n
     return zip_longest(*args, fillvalue=fillvalue)
```

### Comparing `patent_client-5.0.0/patent_client/util/claims/parser_test.py` & `patent_client-5.0.1/patent_client/util/claims/parser_test.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/format.py` & `patent_client-5.0.1/patent_client/util/format.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/manager.py` & `patent_client-5.0.1/patent_client/util/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from copy import deepcopy
 from enum import Enum
 from itertools import chain
-from typing import (
-    TYPE_CHECKING,
-    AsyncIterator,
-    Generic,
-    Iterator,
-    TypeVar,
-    Union,
-)
+from typing import TYPE_CHECKING, AsyncIterator, Generic, Iterator, TypeVar, Union
 
 from typing_extensions import Self
 from yankee.data import Collection
 
 if TYPE_CHECKING:
     pass
 
@@ -251,18 +244,26 @@
 
     async def len(self) -> int:
         """Returns number of records in the QuerySet. Alias for self.count()"""
         return await self.count()
 
     async def first(self) -> ModelType:
         """Get the first object in the manager"""
-        return await anext(self.limit(1).__aiter__())
+        try:
+            return await anext(self.limit(1).__aiter__())
+        except NameError:  # anext was added in 3.10
+            async for doc in self.limit(1):
+                return doc
 
     async def get(self, *args, **kwargs) -> ModelType:
         """If the critera results in a single record, return it, else raise an exception"""
         mger = self.filter(*args, **kwargs)
         length = await mger.count()
         if length > 1:
             raise ValueError("More than one document found!")
         if length == 0:
             raise ValueError("No documents found!")
         return await mger.first()
+
+    async def to_list(self) -> list[ModelType]:
+        """Return a list of all objects in the manager"""
+        return [item async for item in self]
```

### Comparing `patent_client-5.0.0/patent_client/util/pydantic_util.py` & `patent_client-5.0.1/patent_client/util/pydantic_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 import importlib
 import re
 import typing as tp
 
 from async_property.base import AsyncPropertyDescriptor
 from dateutil.parser import isoparse
 from dateutil.parser import parse as parse_dt
-from pydantic import BaseModel as PydanticBaseModel
-from pydantic import BeforeValidator, ConfigDict
+from pydantic import BaseModel as PydanticBaseModel, BeforeValidator, ConfigDict
 from typing_extensions import Annotated
 
 from patent_client.util.manager import Manager
 
 
-def parse_datetime(date_obj: str | datetime.datetime) -> datetime.datetime:
+def parse_datetime(date_obj: tp.Union[str, datetime.datetime]) -> datetime.datetime:
     if isinstance(date_obj, datetime.datetime):
         return date_obj
     try:
         return isoparse(date_obj)
     except ValueError:
         return parse_dt(date_obj)
 
 
-def parse_date(date_obj: str | datetime.datetime | datetime.date) -> datetime.date:
+def parse_date(date_obj: tp.Union[str, datetime.datetime, datetime.date]) -> datetime.date:
     if isinstance(date_obj, datetime.date):
         return date_obj
     elif isinstance(date_obj, datetime.datetime):
         return date_obj.date()
     try:
         return isoparse(date_obj).date()
     except ValueError:
```

### Comparing `patent_client-5.0.0/patent_client/util/request_util.py` & `patent_client-5.0.1/patent_client/util/request_util.py`

 * *Files identical despite different names*

### Comparing `patent_client-5.0.0/patent_client/util/test.py` & `patent_client-5.0.1/patent_client/util/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,7 @@
     for k, v in dict_1.items():
         if isinstance(v, list) and not isinstance(v, str):
             return compare_lists(v, dict_2[k], key=f"{key}.{k}")
         elif isinstance(v, dict):
             return compare_dicts(v, dict_2[k], key=f"{key}.{k}")
         else:
             assert v == dict_2[k], f"At key {key}.{k}, {v} != {dict_2[k]}"
-
```

### Comparing `patent_client-5.0.0/pyproject.toml` & `patent_client-5.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patent_client"
-version = "5.0.0"
+version = "5.0.1"
 description = "A set of ORM-style clients for publicly available intellectual property data"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 documentation = "https://patent-client.readthedocs.io"
 homepage = "https://github.com/parkerhancock/patent_client"
 repository = "https://github.com/parkerhancock/patent_client"
```

