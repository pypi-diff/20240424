# Comparing `tmp/cognite_neat-0.75.4.tar.gz` & `tmp/cognite_neat-0.75.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.75.4.tar", max compression
+gzip compressed data, was "cognite_neat-0.75.5.tar", max compression
```

## Comparing `cognite_neat-0.75.4.tar` & `cognite_neat-0.75.5.tar`

### file list

```diff
@@ -1,257 +1,257 @@
--rw-r--r--   0        0        0    11351 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/README.md
--rw-r--r--   0        0        0       61 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1891 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     3529 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13661 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     8107 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    12402 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0    10756 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
--rw-r--r--   0        0        0     8374 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
--rw-r--r--   0        0        0     5333 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
--rw-r--r--   0        0        0      629 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-04-24 10:08:28.254683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1423704 2024-04-24 10:08:28.262683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
--rw-r--r--   0        0        0     2667 2024-04-24 10:08:28.262683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
--rw-r--r--   0        0        0  6282865 2024-04-24 10:08:28.290683 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
--rw-r--r--   0        0        0   240334 2024-04-24 10:08:28.294684 cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-24 10:08:28.302683 cognite_neat-0.75.4/cognite/neat/config.py
--rw-r--r--   0        0        0     1227 2024-04-24 10:08:28.302683 cognite_neat-0.75.4/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-24 10:08:28.302683 cognite_neat-0.75.4/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-24 10:08:28.302683 cognite_neat-0.75.4/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-24 10:08:28.302683 cognite_neat-0.75.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14947 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      149 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-24 10:08:28.306684 cognite_neat-0.75.4/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    13473 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/__init__.py
--rw-r--r--   0        0        0       73 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-24 10:08:28.310684 cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/__init__.py
--rw-r--r--   0        0        0      363 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_base.py
--rw-r--r--   0        0        0    11734 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_dexpi.py
--rw-r--r--   0        0        0    17695 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14909 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      701 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/__init__.py
--rw-r--r--   0        0        0    23859 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_asset_loader.py
--rw-r--r--   0        0        0     2399 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_base.py
--rw-r--r--   0        0        0     2837 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/__init__.py
--rw-r--r--   0        0        0     2321 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/labels.py
--rw-r--r--   0        0        0     5023 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/models.py
--rw-r--r--   0        0        0    40480 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22715 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12995 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/validator.py
--rw-r--r--   0        0        0      149 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/__init__.py
--rw-r--r--   0        0        0    14289 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5448 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/__init__.py
--rw-r--r--   0        0        0     4765 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
--rw-r--r--   0        0        0    18719 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
--rw-r--r--   0        0        0    14738 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/transformer.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/__init__.py
--rw-r--r--   0        0        0     8610 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/__init__.py
--rw-r--r--   0        0        0     2598 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5567 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-24 10:08:28.314684 cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1453 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_base.py
--rw-r--r--   0        0        0      102 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
--rw-r--r--   0        0        0    36814 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8312 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0     6251 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2graphql.py
--rw-r--r--   0        0        0    18458 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0    28805 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3881 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     1085 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2triples.py
--rw-r--r--   0        0        0     5783 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/__init__.py
--rw-r--r--   0        0        0     2330 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_base.py
--rw-r--r--   0        0        0     6476 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_dict2rules.py
--rw-r--r--   0        0        0     7727 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0    12093 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9407 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10557 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1502 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0      421 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_xsd2rules.py
--rw-r--r--   0        0        0     1601 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      127 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/_base.py
--rw-r--r--   0        0        0    12382 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7351 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51091 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/tables.py
--rw-r--r--   0        0        0     4402 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/legacy/rules/models/value_types.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0      176 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0      115 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/analysis/__init__.py
--rw-r--r--   0        0        0      673 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/analysis/_base.py
--rw-r--r--   0        0        0    19612 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/analysis/_information_rules.py
--rw-r--r--   0        0        0      374 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0    65934 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      413 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1517 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    11853 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0    13145 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19900 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4090 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      408 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4267 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0    10553 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-24 10:08:28.318684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12553 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6924 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11925 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7597 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7804 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7443 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     7110 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    11480 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4197 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     6158 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    15323 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0     4893 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/_entity.py
--rw-r--r--   0        0        0     7228 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0      522 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/__init__.py
--rw-r--r--   0        0        0    11024 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_base.py
--rw-r--r--   0        0        0    56292 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_dms_architect_rules.py
--rw-r--r--   0        0        0    30789 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_dms_schema.py
--rw-r--r--   0        0        0     2567 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_domain_rules.py
--rw-r--r--   0        0        0    21658 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_information_rules.py
--rw-r--r--   0        0        0     1299 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/__init__.py
--rw-r--r--   0        0        0    12212 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_field.py
--rw-r--r--   0        0        0     6308 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_value.py
--rw-r--r--   0        0        0       68 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2722 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26857 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
--rw-r--r--   0        0        0    13659 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.322684 cognite_neat-0.75.4/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6568 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     3015 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6295 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18678 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0    10812 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4784 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29416 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27324 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12728 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2361 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20706 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28111 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-24 10:08:28.326684 cognite_neat-0.75.4/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4540 2024-04-24 10:08:28.710687 cognite_neat-0.75.4/pyproject.toml
--rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.4/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/README.md
+-rw-r--r--   0        0        0       61 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1891 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     3529 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13661 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     8107 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    12402 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0    10756 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg
+-rw-r--r--   0        0        0     8374 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg
+-rw-r--r--   0        0        0     5333 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg
+-rw-r--r--   0        0        0      629 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-24 13:14:46.784801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1423704 2024-04-24 13:14:46.792801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js
+-rw-r--r--   0        0        0     2667 2024-04-24 13:14:46.792801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt
+-rw-r--r--   0        0        0  6282865 2024-04-24 13:14:46.816801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map
+-rw-r--r--   0        0        0   240334 2024-04-24 13:14:46.820801 cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/config.py
+-rw-r--r--   0        0        0     1227 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-24 13:14:46.824801 cognite_neat-0.75.5/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-24 13:14:46.828801 cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14947 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      149 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    13473 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/legacy/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-24 13:14:46.832801 cognite_neat-0.75.5/cognite/neat/legacy/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_base.py
+-rw-r--r--   0        0        0    11734 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_dexpi.py
+-rw-r--r--   0        0        0    17695 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14909 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      701 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/__init__.py
+-rw-r--r--   0        0        0    23859 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_asset_loader.py
+-rw-r--r--   0        0        0     2399 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/__init__.py
+-rw-r--r--   0        0        0     2321 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/labels.py
+-rw-r--r--   0        0        0     5023 2024-04-24 13:14:46.836801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/models.py
+-rw-r--r--   0        0        0    40480 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22715 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12995 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/validator.py
+-rw-r--r--   0        0        0      149 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14289 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5448 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/__init__.py
+-rw-r--r--   0        0        0     4765 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/__init__.py
+-rw-r--r--   0        0        0    18719 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/sparql.py
+-rw-r--r--   0        0        0    14738 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/__init__.py
+-rw-r--r--   0        0        0     8610 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2598 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5567 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1453 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_base.py
+-rw-r--r--   0        0        0      102 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/rules2labels.py
+-rw-r--r--   0        0        0    36814 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8312 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0     6251 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2graphql.py
+-rw-r--r--   0        0        0    18458 2024-04-24 13:14:46.840801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0    28805 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3881 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     1085 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2triples.py
+-rw-r--r--   0        0        0     5783 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_base.py
+-rw-r--r--   0        0        0     6476 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dict2rules.py
+-rw-r--r--   0        0        0     7727 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0    12093 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9407 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10557 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1502 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      421 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_xsd2rules.py
+-rw-r--r--   0        0        0     1601 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      127 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/_base.py
+-rw-r--r--   0        0        0    12382 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7351 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51091 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/tables.py
+-rw-r--r--   0        0        0     4402 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/legacy/rules/models/value_types.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0      115 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/__init__.py
+-rw-r--r--   0        0        0      673 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/_base.py
+-rw-r--r--   0        0        0    19612 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/analysis/_information_rules.py
+-rw-r--r--   0        0        0      374 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0    65934 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      413 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1517 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    11853 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0    13145 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19900 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4090 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      408 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4267 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0    10553 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12553 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6924 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11925 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7597 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7804 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7443 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     7110 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    11480 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4197 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     6158 2024-04-24 13:14:46.844801 cognite_neat-0.75.5/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    15323 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0     4893 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/_entity.py
+-rw-r--r--   0        0        0     7228 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0      522 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/__init__.py
+-rw-r--r--   0        0        0    11024 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_base.py
+-rw-r--r--   0        0        0    56312 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_architect_rules.py
+-rw-r--r--   0        0        0    30789 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_schema.py
+-rw-r--r--   0        0        0     2567 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_domain_rules.py
+-rw-r--r--   0        0        0    21658 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_information_rules.py
+-rw-r--r--   0        0        0     1299 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/__init__.py
+-rw-r--r--   0        0        0    12233 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_field.py
+-rw-r--r--   0        0        0     6308 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_value.py
+-rw-r--r--   0        0        0       68 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2722 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26857 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Import_DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml
+-rw-r--r--   0        0        0    13659 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6568 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     3015 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6295 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18678 2024-04-24 13:14:46.848801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0    10812 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4784 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29416 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27324 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12728 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2361 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20706 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28111 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-24 13:14:46.852801 cognite_neat-0.75.5/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4540 2024-04-24 13:14:47.236803 cognite_neat-0.75.5/pyproject.toml
+-rw-r--r--   0        0        0     9316 1970-01-01 00:00:00.000000 cognite_neat-0.75.5/PKG-INFO
```

### Comparing `cognite_neat-0.75.4/LICENSE` & `cognite_neat-0.75.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/README.md` & `cognite_neat-0.75.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/configuration.py` & `cognite_neat-0.75.5/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.75.5/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.75.5/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/explorer.py` & `cognite_neat-0.75.5/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.75.5/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.75.5/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.75.5/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.75.5/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.75.5/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/architect-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/developer-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/img/sme-icon.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/js/main.4345d42f.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.75.5/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/config.py` & `cognite_neat-0.75.5/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/constants.py` & `cognite_neat-0.75.5/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.5/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.5/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.5/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.5/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_dexpi.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/__init__.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_asset_loader.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_base.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/_exceptions.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/labels.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/models.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/rdf_to_dms.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/loaders/validator.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/loaders/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/__init__.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_base.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_graphdb_store.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_memory_store.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_oxigraph_store.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_oxrdflib.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/entity_matcher.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/query_generator/sparql.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/graph/transformations/transformer.py` & `cognite_neat-0.75.5/cognite/neat/legacy/graph/transformations/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/analysis.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/__init__.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/power-grid-model.yaml` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/rules-template.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/skos-rules.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/examples/wind-energy.owl` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/__init__.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_base.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_core/rules2labels.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2graphql.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_rules2triples.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/exporters/_validation.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/__init__.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_base.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_dict2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_dms2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_graph2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_json2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/models/_base.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/models/raw_rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/models/rdfpath.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/models/rules.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/legacy/rules/models/value_types.py` & `cognite_neat-0.75.5/cognite/neat/legacy/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/analysis/_base.py` & `cognite_neat-0.75.5/cognite/neat/rules/analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/analysis/_information_rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.75.5/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.75.5/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/base.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.75.5/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/_entity.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/_entity.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/__init__.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_base.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_dms_architect_rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_architect_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -758,15 +758,16 @@
     ) -> dm.SpaceApplyList:
         used_spaces = {container.space for container in containers} | {view.space for view in views}
         if len(used_spaces) == 1:
             # We skip the default space and only use this space for the data model
             data_model.space = used_spaces.pop()
             spaces = dm.SpaceApplyList([dm.SpaceApply(space=data_model.space)])
         else:
-            spaces = dm.SpaceApplyList([metadata.as_space()] + [dm.SpaceApply(space=space) for space in used_spaces])
+            used_spaces.add(metadata.space)
+            spaces = dm.SpaceApplyList([dm.SpaceApply(space=space) for space in used_spaces])
         if self.instance_space and self.instance_space not in {space.space for space in spaces}:
             spaces.append(dm.SpaceApply(space=self.instance_space, name=self.instance_space))
         return spaces
 
     def _create_views_with_node_types(
         self,
         dms_views: SheetList[DMSView],
```

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_dms_schema.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_dms_schema.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_domain_rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_information_rules.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/__init__.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_base.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 
 if sys.version_info >= (3, 11):
     from typing import Self
 else:
     from typing_extensions import Self
 
-
+# mypy: ignore-errors
 VERSION_ID_REGEX = rf"\(version=(?P<version>{VERSION_REGEX})\)"
 
 
 PROPERTY_ENTITY_REGEX_COMPILED = re.compile(
     rf"^((?P<prefix>{PREFIX_REGEX}):)?(?P<suffix>{SUFFIX_REGEX})"
     rf"\((version=(?P<version>{VERSION_REGEX}), )?property=(?P<property>{PROPERTY_REGEX})\)$"
 )
```

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_field.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/rules/models/rules/_types/_value.py` & `cognite_neat-0.75.5/cognite/neat/rules/models/rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/cdf.py` & `cognite_neat-0.75.5/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.75.5/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/exceptions.py` & `cognite_neat-0.75.5/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.75.5/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/text.py` & `cognite_neat-0.75.5/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/utils.py` & `cognite_neat-0.75.5/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/utils/xml.py` & `cognite_neat-0.75.5/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.75.5/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/base.py` & `cognite_neat-0.75.5/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.75.5/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Export_DMS/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Export_Rules_to_Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_DEXPI_Graph_and_Export_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Extract_RDF_Graph_and_Generate_Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Import_DMS/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Import_DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Ontology_to_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Validate_Solution_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Data_Model_Using_Mock_Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml` & `cognite_neat-0.75.5/cognite/neat/workflows/examples/Visualize_Semantic_Data_Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/manager.py` & `cognite_neat-0.75.5/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.75.5/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.75.5/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/model.py` & `cognite_neat-0.75.5/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.75.5/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/tasks.py` & `cognite_neat-0.75.5/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/cognite/neat/workflows/triggers.py` & `cognite_neat-0.75.5/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.75.4/pyproject.toml` & `cognite_neat-0.75.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.75.4"
+version = "0.75.5"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.75.4/PKG-INFO` & `cognite_neat-0.75.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.75.4
+Version: 0.75.5
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

