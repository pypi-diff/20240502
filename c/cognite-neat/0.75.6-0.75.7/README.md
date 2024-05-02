# Comparing `tmp/cognite_neat-0.75.6.tar.gz` & `tmp/cognite_neat-0.75.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.75.6.tar", max compression
+gzip compressed data, was "cognite_neat-0.75.7.tar", max compression
```

## Comparing `cognite_neat-0.75.6.tar` & `cognite_neat-0.75.7.tar`

### file list

```diff
@@ -1,257 +1,259 @@
--rw-r--r--   0        0        0    11351 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/README.md
--rw-r--r--   0        0        0       61 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3529 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13661 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8107 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-04-26 08:02:28.900058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-26 08:02:28.904058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423704 2024-04-26 08:02:28.908058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
--rw-r--r--   0        0        0     2667 2024-04-26 08:02:28.912058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
--rw-r--r--   0        0        0  6282865 2024-04-26 08:02:28.936058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
--rw-r--r--   0        0        0   240334 2024-04-26 08:02:28.936058 cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/config.py
--rw-r--r--   0        0        0     1227 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-26 08:02:28.944058 cognite_neat-0.75.6/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-26 08:02:28.948058 cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14947 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-26 08:02:28.952058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14909 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23859 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2399 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2837 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40480 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22715 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12995 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14738 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-26 08:02:28.956058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36814 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5783 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2330 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7727 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      176 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-04-26 08:02:28.960058 cognite_neat-0.75.6/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      673 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19612 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1517 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11893 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13767 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19900 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4090 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4057 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10405 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12553 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6801 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11925 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7804 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     6987 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11085 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4074 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15323 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0     4893 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/_entity.py
--rw-r--r--   0        0        0     7228 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0      522 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/__init__.py
--rw-r--r--   0        0        0    11024 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_base.py
--rw-r--r--   0        0        0    56198 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_architect_rules.py
--rw-r--r--   0        0        0    30789 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_schema.py
--rw-r--r--   0        0        0     2542 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_domain_rules.py
--rw-r--r--   0        0        0    21577 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_information_rules.py
--rw-r--r--   0        0        0     1299 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/__init__.py
--rw-r--r--   0        0        0    12233 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_value.py
--rw-r--r--   0        0        0       68 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-26 08:02:28.964058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3015 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18678 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0    10384 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4784 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29416 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27324 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12728 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2361 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20706 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28111 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-26 08:02:28.968058 cognite_neat-0.75.6/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4540 2024-04-26 08:02:29.356060 cognite_neat-0.75.6/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.6/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/LICENSE
+-rw-r--r--   0        0        0     6775 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/README.md
+-rw-r--r--   0        0        0       61 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3529 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13661 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8107 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-05-02 10:32:57.718098 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423704 2024-05-02 10:32:57.726099 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
+-rw-r--r--   0        0        0     2667 2024-05-02 10:32:57.726099 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282865 2024-05-02 10:32:57.750103 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
+-rw-r--r--   0        0        0   240334 2024-05-02 10:32:57.754104 cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/config.py
+-rw-r--r--   0        0        0     1227 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-05-02 10:32:57.758105 cognite_neat-0.75.7/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-02 10:32:57.762105 cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14947 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-02 10:32:57.766106 cognite_neat-0.75.7/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14909 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-05-02 10:32:57.770107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23859 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2399 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2837 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40480 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22715 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12995 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14738 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-02 10:32:57.774107 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36814 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5783 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2330 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7727 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19612 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1870 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    14231 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13767 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19900 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4090 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4057 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10405 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12553 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6801 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11925 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-05-02 10:32:57.778108 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     6987 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11085 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4074 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15323 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     4893 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/_entity.py
+-rw-r--r--   0        0        0     5308 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/data_types.py
+-rw-r--r--   0        0        0     9885 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/entities.py
+-rw-r--r--   0        0        0     7228 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    11024 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    56198 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    30789 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2542 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    21577 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0     1299 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0    12233 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_value.py
+-rw-r--r--   0        0        0       68 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11304 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-05-02 10:32:57.782109 cognite_neat-0.75.7/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    22585 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0    10384 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3929 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29416 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27324 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12728 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2361 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20706 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28111 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-05-02 10:32:57.786109 cognite_neat-0.75.7/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4540 2024-05-02 10:32:58.170174 cognite_neat-0.75.7/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.7/PKG-INFO
```

### Comparing `cognite_neat-0.75.6/LICENSE` & `cognite_neat-0.75.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/README.md` & `cognite_neat-0.75.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/configuration.py` & `cognite_neat-0.75.7/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.75.7/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.75.7/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/explorer.py` & `cognite_neat-0.75.7/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.75.7/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.75.7/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.75.7/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.75.7/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.75.7/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.75.7/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/config.py` & `cognite_neat-0.75.7/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/constants.py` & `cognite_neat-0.75.7/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.7/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.7/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.7/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.7/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.75.7/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.75.7/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.75.7/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.75.7/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,33 +26,38 @@
     created: int = 0
     deleted: int = 0
     changed: int = 0
     unchanged: int = 0
     skipped: int = 0
     failed_created: int = 0
     failed_changed: int = 0
+    failed_deleted: int = 0
     error_messages: list[str] = field(default_factory=list)
 
     @property
     def total(self) -> int:
         return self.created + self.deleted + self.changed + self.unchanged
 
     @property
     def failed(self) -> int:
-        return self.failed_created + self.failed_changed
+        return self.failed_created + self.failed_changed + self.failed_deleted
 
     def as_report_str(self) -> str:
         line = []
         if self.created:
             line.append(f"created {self.created}")
         if self.changed:
             line.append(f"updated {self.changed}")
         if self.skipped:
             line.append(f"skipped {self.skipped}")
         if self.unchanged:
             line.append(f"unchanged {self.unchanged}")
+        if self.deleted:
+            line.append(f"deleted {self.deleted}")
         if self.failed_created:
             line.append(f"failed to create {self.failed_created}")
         if self.failed_changed:
             line.append(f"failed to update {self.failed_changed}")
+        if self.failed_deleted:
+            line.append(f"failed to delete {self.failed_deleted}")
 
         return f"{self.name.title()}: {', '.join(line)}"
```

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,29 +147,63 @@
         if dms_rules.metadata.extension in (ExtensionCategory.addition, ExtensionCategory.reshape):
             # We do not freeze views as they might be changed, even for addition,
             # in case, for example, new properties are added. The validation will catch this.
             schema.frozen_ids.update(set(reference_schema.containers.as_ids()))
             schema.frozen_ids.update(set(reference_schema.node_types.as_ids()))
         return schema
 
+    def delete_from_cdf(self, rules: Rules, client: CogniteClient, dry_run: bool = False) -> Iterable[UploadResult]:
+        schema, to_export = self._prepare_schema_and_exporters(rules, client)
+
+        # we need to reverse order in which we are picking up the items to delete
+        # as they are sorted in the order of creation and we need to delete them in reverse order
+        for all_items, loader in reversed(to_export):
+            all_item_ids = loader.get_ids(all_items)
+            skipped = sum(1 for item_id in all_item_ids if item_id in schema.frozen_ids)
+            item_ids = [item_id for item_id in all_item_ids if item_id not in schema.frozen_ids]
+            cdf_items = loader.retrieve(item_ids)
+            cdf_item_by_id = {loader.get_id(item): item for item in cdf_items}
+            items = [item for item in all_items if loader.get_id(item) in item_ids]
+            to_delete = []
+
+            for item in items:
+                if (
+                    isinstance(loader, DataModelingLoader)
+                    and self.include_space is not None
+                    and not loader.in_space(item, self.include_space)
+                ):
+                    continue
+
+                cdf_item = cdf_item_by_id.get(loader.get_id(item))
+                if cdf_item:
+                    to_delete.append(cdf_item)
+
+            deleted = len(to_delete)
+            failed_deleted = 0
+
+            error_messages: list[str] = []
+            if not dry_run:
+                if to_delete:
+                    try:
+                        loader.delete(to_delete)
+                    except CogniteAPIError as e:
+                        failed_deleted = len(e.failed) + len(e.unknown)
+                        deleted -= failed_deleted
+                        error_messages.append(f"Failed delete: {e.message}")
+
+            yield UploadResult(
+                name=loader.resource_name,
+                deleted=deleted,
+                skipped=skipped,
+                failed_deleted=failed_deleted,
+                error_messages=error_messages,
+            )
+
     def export_to_cdf(self, rules: Rules, client: CogniteClient, dry_run: bool = False) -> Iterable[UploadResult]:
-        schema = self.export(rules)
-        to_export: list[tuple[CogniteResourceList, ResourceLoader]] = []
-        if self.export_components.intersection({"all", "spaces"}):
-            to_export.append((schema.spaces, SpaceLoader(client)))
-        if self.export_components.intersection({"all", "containers"}):
-            to_export.append((schema.containers, ContainerLoader(client)))
-        if self.export_components.intersection({"all", "views"}):
-            to_export.append((schema.views, ViewLoader(client, self.existing_handling)))
-        if self.export_components.intersection({"all", "data_models"}):
-            to_export.append((schema.data_models, DataModelLoader(client)))
-        if isinstance(schema, PipelineSchema):
-            to_export.append((schema.databases, RawDatabaseLoader(client)))
-            to_export.append((schema.raw_tables, RawTableLoader(client)))
-            to_export.append((schema.transformations, TransformationLoader(client)))
+        schema, to_export = self._prepare_schema_and_exporters(rules, client)
 
         # The conversion from DMS to GraphQL does not seem to be triggered even if the views
         # are changed. This is a workaround to force the conversion.
         redeploy_data_model = False
 
         for all_items, loader in to_export:
             all_item_ids = loader.get_ids(all_items)
@@ -250,7 +284,26 @@
                 failed_created=failed_created,
                 failed_changed=failed_changed,
                 error_messages=error_messages,
             )
 
             if loader.resource_name == "views" and (created or changed) and not redeploy_data_model:
                 redeploy_data_model = True
+
+    def _prepare_schema_and_exporters(
+        self, rules, client
+    ) -> tuple[DMSSchema, list[tuple[CogniteResourceList, ResourceLoader]]]:
+        schema = self.export(rules)
+        to_export: list[tuple[CogniteResourceList, ResourceLoader]] = []
+        if self.export_components.intersection({"all", "spaces"}):
+            to_export.append((schema.spaces, SpaceLoader(client)))
+        if self.export_components.intersection({"all", "containers"}):
+            to_export.append((schema.containers, ContainerLoader(client)))
+        if self.export_components.intersection({"all", "views"}):
+            to_export.append((schema.views, ViewLoader(client, self.existing_handling)))
+        if self.export_components.intersection({"all", "data_models"}):
+            to_export.append((schema.data_models, DataModelLoader(client)))
+        if isinstance(schema, PipelineSchema):
+            to_export.append((schema.databases, RawDatabaseLoader(client)))
+            to_export.append((schema.raw_tables, RawTableLoader(client)))
+            to_export.append((schema.transformations, TransformationLoader(client)))
+        return schema, to_export
```

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.75.7/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/base.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.75.7/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/_entity.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/_entity.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/__init__.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_base.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_architect_rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_dms_schema.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_domain_rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_information_rules.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/__init__.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_base.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_field.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/rules/models/rules/_types/_value.py` & `cognite_neat-0.75.7/cognite/neat/rules/models/rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/cdf.py` & `cognite_neat-0.75.7/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,16 +83,18 @@
 
     def retrieve(self, ids: SequenceNotStr[str]) -> SpaceList:
         return self.client.data_modeling.spaces.retrieve(ids)
 
     def update(self, items: Sequence[SpaceApply]) -> SpaceList:
         return self.create(items)
 
-    def delete(self, ids: SequenceNotStr[str]) -> list[str]:
-        return self.client.data_modeling.spaces.delete(ids)
+    def delete(self, ids: SequenceNotStr[str] | Sequence[Space | SpaceApply]) -> list[str]:
+        if all(isinstance(item, Space) for item in ids) or all(isinstance(item, SpaceApply) for item in ids):
+            ids = [cast(Space | SpaceApply, item).space for item in ids]
+        return self.client.data_modeling.spaces.delete(cast(SequenceNotStr[str], ids))
 
 
 class ViewLoader(DataModelingLoader[ViewId, ViewApply, View, ViewApplyList, ViewList]):
     resource_name = "views"
 
     def __init__(self, client: CogniteClient, existing_handling: Literal["fail", "skip", "update", "force"] = "fail"):
         super().__init__(client)
```

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.75.7/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/exceptions.py` & `cognite_neat-0.75.7/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.75.7/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/text.py` & `cognite_neat-0.75.7/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/utils.py` & `cognite_neat-0.75.7/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/utils/xml.py` & `cognite_neat-0.75.7/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.75.7/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/base.py` & `cognite_neat-0.75.7/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.75.7/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.75.7/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/manager.py` & `cognite_neat-0.75.7/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.75.7/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.75.7/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/model.py` & `cognite_neat-0.75.7/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,117 @@
 __all__ = [
     "RulesToDMS",
     "RulesToExcel",
     "RulesToOntology",
     "RulesToSHACL",
     "RulesToSemanticDataModel",
     "RulesToCDFTransformations",
+    "DeleteDataModelFromCDF",
 ]
 
 
 CATEGORY = __name__.split(".")[-1].replace("_", " ").title()
 
 
+class DeleteDataModelFromCDF(Step):
+    """
+    This step deletes data model and its components from CDF
+    """
+
+    description = "This step deletes data model and its components from CDF."
+    version = "private-beta"
+    category = CATEGORY
+
+    configurables: ClassVar[list[Configurable]] = [
+        Configurable(
+            name="Dry run",
+            value="False",
+            label=("Whether to perform a dry run of the deleter. "),
+            options=["True", "False"],
+        ),
+        Configurable(
+            name="Components",
+            type="multi_select",
+            value="",
+            label="Select which DMS schema component(s) to be deleted from CDF",
+            options=["spaces", "containers", "views", "data_models"],
+        ),
+        Configurable(
+            name="Multi-space components deletion",
+            value="False",
+            label=(
+                "Whether to delete only components belonging to the data model space"
+                " (i.e. space define under Metadata sheet of Rules), "
+                "or also additionally delete components outside of the data model space."
+            ),
+            options=["True", "False"],
+        ),
+    ]
+
+    def run(self, rules: MultiRuleData, cdf_client: CogniteClient) -> FlowMessage:  # type: ignore[override]
+        if self.configs is None or self.data_store_path is None:
+            raise StepNotInitialized(type(self).__name__)
+        components_to_delete = {
+            cast(Literal["all", "spaces", "data_models", "views", "containers"], key)
+            for key, value in self.complex_configs["Components"].items()
+            if value
+        }
+        dry_run = self.configs["Dry run"] == "True"
+        multi_space_components_delete: bool = self.configs["Multi-space components deletion"] == "True"
+
+        if not components_to_delete:
+            return FlowMessage(
+                error_text="No DMS Schema components selected for removal! Please select minimum one!",
+                step_execution_status=StepExecutionStatus.ABORT_AND_FAIL,
+            )
+        input_rules = rules.dms or rules.information
+        if input_rules is None:
+            return FlowMessage(
+                error_text="Missing DMS or Information rules in the input data! "
+                "Please ensure that a DMS or Information rules is provided!",
+                step_execution_status=StepExecutionStatus.ABORT_AND_FAIL,
+            )
+
+        dms_exporter = exporters.DMSExporter(
+            export_components=frozenset(components_to_delete),
+            include_space=(
+                None
+                if multi_space_components_delete
+                else {input_rules.metadata.space if isinstance(input_rules, DMSRules) else input_rules.metadata.prefix}
+            ),
+        )
+
+        report_lines = ["# Data Model Deletion from CDF\n\n"]
+        errors = []
+        for result in dms_exporter.delete_from_cdf(rules=input_rules, client=cdf_client, dry_run=dry_run):
+            report_lines.append(result.as_report_str())
+            errors.extend(result.error_messages)
+
+        report_lines.append("\n\n# ERRORS\n\n")
+        report_lines.extend(errors)
+
+        output_dir = self.data_store_path / Path("staging")
+        output_dir.mkdir(parents=True, exist_ok=True)
+        report_file = "dms_component_creation_report.txt"
+        report_full_path = output_dir / report_file
+        report_full_path.write_text("\n".join(report_lines))
+
+        output_text = (
+            "<p></p>"
+            "Download Data Model Deletion "
+            f'<a href="/data/staging/{report_file}?{time.time()}" '
+            f'target="_blank">Report</a>'
+        )
+
+        if errors:
+            return FlowMessage(error_text=output_text, step_execution_status=StepExecutionStatus.ABORT_AND_FAIL)
+        else:
+            return FlowMessage(output_text=output_text)
+
+
 class RulesToDMS(Step):
     """
     This step exports Rules to DMS Schema components in CDF
     """
 
     description = "This step exports Rules to DMS Schema components in CDF."
     version = "private-beta"
```

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.75.7/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/tasks.py` & `cognite_neat-0.75.7/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/cognite/neat/workflows/triggers.py` & `cognite_neat-0.75.7/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.6/pyproject.toml` & `cognite_neat-0.75.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.75.6"
+version = "0.75.7"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.75.6/PKG-INFO` & `cognite_neat-0.75.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.75.6
+Version: 0.75.7
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

