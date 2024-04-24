# Comparing `tmp/orchestrator_core-2.2.2rc1.tar.gz` & `tmp/orchestrator_core-2.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-2.2.2rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-2.2.2rc2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-2.2.2rc1.tar` & `orchestrator_core-2.2.2rc2.tar`

### file list

```diff
@@ -1,543 +1,543 @@
--rw-r--r--   0        0        0      342 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.coveragerc
--rw-r--r--   0        0        0     1564 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0     1149 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0      502 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     2620 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      346 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      583 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/issues.yml
--rw-r--r--   0        0        0      550 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1215 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2255 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.gitignore
--rw-r--r--   0        0        0     2599 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/.stignore
--rw-r--r--   0        0        0    30927 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/CHANGELOG.md
--rw-r--r--   0        0        0      333 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/Dockerfile
--rw-r--r--   0        0        0    11409 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/LICENSE
--rw-r--r--   0        0        0      150 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/NOTICE
--rw-r--r--   0        0        0     5595 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/README.md
--rw-r--r--   0        0        0      196 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/codecov.yml
--rw-r--r--   0        0        0       45 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/api.md
--rw-r--r--   0        0        0     5505 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/callbacks.md
--rw-r--r--   0        0        0    30737 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13882 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    24522 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/graphql.md
--rw-r--r--   0        0        0    48994 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2500 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11462 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0      668 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/context.md
--rw-r--r--   0        0        0      802 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/introduction.md
--rw-r--r--   0        0        0     1671 2024-04-17 11:53:37.400903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.md
--rw-r--r--   0        0        0    84576 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.png
--rw-r--r--   0        0        0     1311 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.md
--rw-r--r--   0        0        0    55937 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.png
--rw-r--r--   0        0        0      854 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.md
--rw-r--r--   0        0        0    29551 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.png
--rw-r--r--   0        0        0     1398 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/modelling.md
--rw-r--r--   0        0        0     1138 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.md
--rw-r--r--   0        0        0    23110 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.png
--rw-r--r--   0        0        0     1147 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.md
--rw-r--r--   0        0        0    37248 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.png
--rw-r--r--   0        0        0     1694 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.md
--rw-r--r--   0        0        0    78824 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.png
--rw-r--r--   0        0        0      989 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/standards.md
--rw-r--r--   0        0        0     1114 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/terminology.md
--rw-r--r--   0        0        0     2080 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/contributing/guidelines.md
--rw-r--r--   0        0        0     9997 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/custom.css
--rw-r--r--   0        0        0      656 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/style.css
--rw-r--r--   0        0        0     2165 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/development.md
--rw-r--r--   0        0        0     3438 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/getting-started/prepare-source-folder.md
--rw-r--r--   0        0        0    17905 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/img/WFO-Emblem-White.png
--rw-r--r--   0        0        0      842 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/img/favicon.ico
--rw-r--r--   0        0        0     4020 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/index.md
--rw-r--r--   0        0        0     3897 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/js/termynal.js
--rw-r--r--   0        0        0    11084 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/migration-guide/2.0.md
--rw-r--r--   0        0        0     9063 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3719 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     6048 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3087 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5602 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4623 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7447 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3697 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3051 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6156 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1953 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3991 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3596 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2141 2024-04-17 11:53:37.404903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2878 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      785 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3632 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2024-04-17 11:53:37.408903 orchestrator_core-2.2.2rc1/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0     5478 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/mkdocs.yml
--rw-r--r--   0        0        0     1262 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/mutmut_config.py
--rw-r--r--   0        0        0       70 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/nitpick-style.toml
--rw-r--r--   0        0        0     1098 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     3145 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     1034 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1284 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    14585 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     4021 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     4806 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     3657 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     6106 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     3081 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    15675 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      963 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1827 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     2563 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1722 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/ws.py
--rw-r--r--   0        0        0     1502 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    10612 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5996 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/api/models.py
--rw-r--r--   0        0        0     8416 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/app.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13792 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6775 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     2172 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10474 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9379 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    23981 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1399 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     7377 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0      173 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/README
--rw-r--r--   0        0        0      307 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
--rw-r--r--   0        0        0      115 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
--rw-r--r--   0        0        0      307 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
--rw-r--r--   0        0        0      115 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
--rw-r--r--   0        0        0      234 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
--rw-r--r--   0        0        0      131 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
--rw-r--r--   0        0        0       82 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     2007 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/enums.py
--rw-r--r--   0        0        0     5452 2024-04-17 11:53:37.412903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     6341 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2073 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5285 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1379 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1878 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4541 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1815 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     8026 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      759 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      538 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      532 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      361 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      431 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_create_imports.j2
--rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_create_steps.j2
--rw-r--r--   0        0        0      394 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_modify_imports.j2
--rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_modify_steps.j2
--rw-r--r--   0        0        0       25 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/additional_terminate_steps.j2
--rw-r--r--   0        0        0      282 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0      361 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_data_head.j2
--rw-r--r--   0        0        0     4806 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      298 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/enums.j2
--rw-r--r--   0        0        0      523 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
--rw-r--r--   0        0        0      277 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      904 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4719 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2901 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1365 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2454 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      545 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     1274 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_workflows.j2
--rw-r--r--   0        0        0      291 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/subscription_model_registry.j2
--rw-r--r--   0        0        0     1883 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1802 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1677 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      985 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2315 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      857 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20371 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8979 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4110 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2970 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10269 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/database.py
--rw-r--r--   0        0        0      371 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     5020 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4098 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0      899 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     1089 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/product_block.py
--rw-r--r--   0        0        0      889 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/resource_type.py
--rw-r--r--   0        0        0      562 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/__init__.py
--rw-r--r--   0        0        0     5170 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/inferred_filter.py
--rw-r--r--   0        0        0     1466 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0     1276 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/filters/workflow.py
--rw-r--r--   0        0        0      283 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/helpers.py
--rw-r--r--   0        0        0    24840 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/models.py
--rw-r--r--   0        0        0      162 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     2175 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      353 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0     1987 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      570 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0      617 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product_block.py
--rw-r--r--   0        0        0      617 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/resource_type.py
--rw-r--r--   0        0        0     4455 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0     1441 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0      576 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/db/sorting/workflow.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    18847 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/__init__.py
--rw-r--r--   0        0        0     8359 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/migrate_20.py
--rw-r--r--   0        0        0     2494 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2508 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3271 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      894 2024-04-17 11:53:37.416903 orchestrator_core-2.2.2rc1/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    59246 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2732 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/customer_description.py
--rw-r--r--   0        0        0      989 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/helpers.py
--rw-r--r--   0        0        0     2882 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     1268 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0      892 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     1906 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/__init__.py
--rw-r--r--   0        0        0     1505 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_contact_list.py
--rw-r--r--   0        0        0      708 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_id.py
--rw-r--r--   0        0        0      779 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/display_subscription.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/network_type_validators.py
--rw-r--r--   0        0        0     2114 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/forms/validators/product_id.py
--rw-r--r--   0        0        0     1378 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     6161 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/autoregistration.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4304 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1746 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     5826 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_handler_extension.py
--rw-r--r--   0        0        0     3100 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/customer_description.py
--rw-r--r--   0        0        0     1553 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/start_process.py
--rw-r--r--   0        0        0     2413 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      851 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0      934 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/customer.py
--rw-r--r--   0        0        0      636 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/helpers.py
--rw-r--r--   0        0        0     4491 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2562 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     2748 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product_block.py
--rw-r--r--   0        0        0     2741 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/resource_type.py
--rw-r--r--   0        0        0     3700 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     5531 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0     2681 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/workflow.py
--rw-r--r--   0        0        0     7403 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schema.py
--rw-r--r--   0        0        0     1003 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/__init__.py
--rw-r--r--   0        0        0      115 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/customer.py
--rw-r--r--   0        0        0      213 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/customer_description.py
--rw-r--r--   0        0        0      203 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3475 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2134 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0     1203 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      755 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      999 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7838 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0     1140 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     4470 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      524 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1191 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0     1002 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0     3897 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py
--rw-r--r--   0        0        0     2156 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/is_query_detailed.py
--rw-r--r--   0        0        0     1370 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/override_class.py
--rw-r--r--   0        0        0      902 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/to_graphql_result_page.py
--rw-r--r--   0        0        0       39 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3382 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40911 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2698 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1265 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    39307 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      950 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1214 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1603 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5106 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7964 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0     1014 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0      591 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
--rw-r--r--   0        0        0      755 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
--rw-r--r--   0        0        0      967 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
--rw-r--r--   0        0        0     4491 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
--rw-r--r--   0        0        0     1036 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
--rw-r--r--   0        0        0     5480 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
--rw-r--r--   0        0        0     2246 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/py.typed
--rw-r--r--   0        0        0     1066 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1526 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1234 2024-04-17 11:53:37.420903 orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2195 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2708 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      888 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1286 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1356 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      802 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     2693 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1698 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1792 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      973 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3366 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1030 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1977 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1744 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/security.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3635 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/celery.py
--rw-r--r--   0        0        0      876 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/fixed_inputs.py
--rw-r--r--   0        0        0     3710 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/process_broadcast_thread.py
--rw-r--r--   0        0        0    26253 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1933 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/products.py
--rw-r--r--   0        0        0      884 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/resource_types.py
--rw-r--r--   0        0        0     2723 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/settings.py
--rw-r--r--   0        0        0    25733 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5867 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1713 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/translations.py
--rw-r--r--   0        0        0     1638 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/services/workflows.py
--rw-r--r--   0        0        0     3634 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/targets.py
--rw-r--r--   0        0        0    16236 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/types.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5584 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0      875 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/deprecation_logger.py
--rw-r--r--   0        0        0     6172 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     4658 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/enrich_process.py
--rw-r--r--   0        0        0     4250 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     2665 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/fixed_inputs.py
--rw-r--r--   0        0        0     8063 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     1322 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/get_updated_properties.py
--rw-r--r--   0        0        0     3212 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8341 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/json.py
--rw-r--r--   0        0        0     6378 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/redis.py
--rw-r--r--   0        0        0    15801 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/search_query.py
--rw-r--r--   0        0        0    12998 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     1366 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/version.py
--rw-r--r--   0        0        0     4828 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3324 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2924 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    42689 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflow.py
--rw-r--r--   0        0        0     4048 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2164 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9528 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2349 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8511 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12929 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     5073 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0     2725 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/setup.cfg
--rw-r--r--   0        0        0      665 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/setup.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1851 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2024-04-17 11:53:37.424903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2887 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5160 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1626 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1139 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3055 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    21379 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15509 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3863 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     8209 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2614 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     3000 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     3038 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    41173 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     3457 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0     3777 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/api/test_ws.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/__init__.py
--rw-r--r--   0        0        0      744 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate.sh
--rw-r--r--   0        0        0      885 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/alembic.ini
--rw-r--r--   0        0        0      233 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/main.py
--rw-r--r--   0        0        0     2821 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/env.py
--rw-r--r--   0        0        0       98 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/helpers.py
--rw-r--r--   0        0        0      510 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/script.py.mako
--rw-r--r--   0        0        0      315 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
--rw-r--r--   0        0        0     2227 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
--rw-r--r--   0        0        0     3852 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
--rw-r--r--   0        0        0      467 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
--rw-r--r--   0        0        0      812 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/__init__.py
--rw-r--r--   0        0        0      764 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py
--rw-r--r--   0        0        0      559 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py
--rw-r--r--   0        0        0     1499 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
--rw-r--r--   0        0        0     1499 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
--rw-r--r--   0        0        0     2442 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
--rw-r--r--   0        0        0     2014 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
--rw-r--r--   0        0        0     1345 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
--rw-r--r--   0        0        0     1010 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
--rw-r--r--   0        0        0      902 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
--rw-r--r--   0        0        0      872 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
--rw-r--r--   0        0        0      755 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
--rw-r--r--   0        0        0      405 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
--rw-r--r--   0        0        0      415 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/translations/en-GB.json
--rw-r--r--   0        0        0      701 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/__init__.py
--rw-r--r--   0        0        0     3940 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
--rw-r--r--   0        0        0     3602 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
--rw-r--r--   0        0        0      620 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
--rw-r--r--   0        0        0     1560 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
--rw-r--r--   0        0        0     1025 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
--rw-r--r--   0        0        0     2683 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
--rw-r--r--   0        0        0     2508 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
--rw-r--r--   0        0        0        1 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
--rw-r--r--   0        0        0     1220 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
--rw-r--r--   0        0        0     1273 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/shared.py
--rw-r--r--   0        0        0     2656 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config1.yaml
--rw-r--r--   0        0        0      549 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config2.yaml
--rw-r--r--   0        0        0      590 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config3.yaml
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/__init__.py
--rw-r--r--   0        0        0      812 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/test_enums.py
--rw-r--r--   0        0        0     2509 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_cli_generate.py
--rw-r--r--   0        0        0     2930 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_generate_code.py
--rw-r--r--   0        0        0    26343 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27644 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/config.py
--rw-r--r--   0        0        0    23677 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.428903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    53002 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8230 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4670 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     1992 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_lifecycle.py
--rw-r--r--   0        0        0     2841 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7794 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1645 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2970 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1606 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2573 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2518 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1194 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1123 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2172 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4217 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3428 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2951 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2272 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2256 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1639 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1838 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      644 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0      451 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/workflows.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     4706 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_contact_list.py
--rw-r--r--   0        0        0      495 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_id.py
--rw-r--r--   0        0        0     1746 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_display_subscription.py
--rw-r--r--   0        0        0     4109 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/__init__.py
--rw-r--r--   0        0        0      690 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/conftest.py
--rw-r--r--   0        0        0      488 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/helpers.py
--rw-r--r--   0        0        0     6235 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_customer_description.py
--rw-r--r--   0        0        0     2449 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_start_process.py
--rw-r--r--   0        0        0     2316 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_customer.py
--rw-r--r--   0        0        0    18677 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     8514 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0    10211 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product_blocks.py
--rw-r--r--   0        0        0     5635 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_resource_types.py
--rw-r--r--   0        0        0     5179 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0     2939 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py
--rw-r--r--   0        0        0     3239 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscription.py
--rw-r--r--   0        0        0    48810 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0     6682 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_workflows.py
--rw-r--r--   0        0        0      608 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_autoregistration.py
--rw-r--r--   0        0        0     7669 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py
--rw-r--r--   0        0        0     3042 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py
--rw-r--r--   0        0        0     8760 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_override_class.py
--rw-r--r--   0        0        0      631 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/helpers.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    28556 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1155 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     6171 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     6650 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      379 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    17406 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1891 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3486 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3529 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_get_updated_properties.py
--rw-r--r--   0        0        0     3052 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     4613 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_search_query.py
--rw-r--r--   0        0        0    11471 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/websocket/__init__.py
--rw-r--r--   0        0        0     3561 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/websocket/test_broadcast.py
--rw-r--r--   0        0        0    14040 2024-04-17 11:53:37.432903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2746 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     5378 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_async_workflow.py
--rw-r--r--   0        0        0     3495 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1884 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2024-04-17 11:53:37.436903 orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 orchestrator_core-2.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.coveragerc
+-rw-r--r--   0        0        0     1564 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0     1149 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0      502 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2620 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      346 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      583 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/issues.yml
+-rw-r--r--   0        0        0      550 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1215 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2426 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.gitignore
+-rw-r--r--   0        0        0     2599 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2024-04-24 12:09:00.578062 orchestrator_core-2.2.2rc2/.stignore
+-rw-r--r--   0        0        0    30927 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/Dockerfile
+-rw-r--r--   0        0        0    11409 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/LICENSE
+-rw-r--r--   0        0        0      150 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/NOTICE
+-rw-r--r--   0        0        0     5595 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/README.md
+-rw-r--r--   0        0        0      196 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/codecov.yml
+-rw-r--r--   0        0        0       45 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/api.md
+-rw-r--r--   0        0        0     5505 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/callbacks.md
+-rw-r--r--   0        0        0    30737 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13882 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    28254 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/graphql.md
+-rw-r--r--   0        0        0    48994 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2500 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11462 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0      802 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1311 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1398 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1138 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0     9997 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/custom.css
+-rw-r--r--   0        0        0      656 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/style.css
+-rw-r--r--   0        0        0     2165 2024-04-24 12:09:00.582062 orchestrator_core-2.2.2rc2/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/development.md
+-rw-r--r--   0        0        0     3438 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/getting-started/prepare-source-folder.md
+-rw-r--r--   0        0        0    17905 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/img/WFO-Emblem-White.png
+-rw-r--r--   0        0        0      842 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/img/favicon.ico
+-rw-r--r--   0        0        0     4020 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/index.md
+-rw-r--r--   0        0        0     3897 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/js/termynal.js
+-rw-r--r--   0        0        0    11084 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/migration-guide/2.0.md
+-rw-r--r--   0        0        0     9063 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3719 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     6048 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3087 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5602 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4623 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7447 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3697 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3051 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6156 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1953 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3991 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3596 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2141 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2878 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      785 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3632 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2024-04-24 12:09:00.586062 orchestrator_core-2.2.2rc2/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0     5478 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/mutmut_config.py
+-rw-r--r--   0        0        0       70 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/nitpick-style.toml
+-rw-r--r--   0        0        0     1098 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     3145 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1284 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    14585 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     4021 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     4806 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     3657 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     6106 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     3081 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    15675 2024-04-24 12:09:00.590062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      963 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1827 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     2563 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1722 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/ws.py
+-rw-r--r--   0        0        0     1502 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    10612 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5996 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/api/models.py
+-rw-r--r--   0        0        0     8721 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13792 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6775 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     2172 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10474 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9379 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    23981 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1399 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     7377 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/README
+-rw-r--r--   0        0        0      307 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      307 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0      115 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0      234 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_imports.j2
+-rw-r--r--   0        0        0      131 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_input_fields.j2
+-rw-r--r--   0        0        0       82 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/custom_templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     2007 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/enums.py
+-rw-r--r--   0        0        0     5452 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     6341 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2073 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5285 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1379 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1878 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4541 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1815 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     8026 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      759 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      538 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      532 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      361 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      431 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_create_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_create_steps.j2
+-rw-r--r--   0        0        0      394 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_modify_imports.j2
+-rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_modify_steps.j2
+-rw-r--r--   0        0        0       25 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/additional_terminate_steps.j2
+-rw-r--r--   0        0        0      282 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0      361 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_data_head.j2
+-rw-r--r--   0        0        0     4806 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      298 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/enums.j2
+-rw-r--r--   0        0        0      523 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2
+-rw-r--r--   0        0        0      277 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      904 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4719 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2901 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1365 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2454 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      545 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     1274 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_workflows.j2
+-rw-r--r--   0        0        0      291 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/subscription_model_registry.j2
+-rw-r--r--   0        0        0     1883 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1802 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1677 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      985 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2315 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      857 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20371 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8979 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4110 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2970 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10269 2024-04-24 12:09:00.594062 orchestrator_core-2.2.2rc2/orchestrator/db/database.py
+-rw-r--r--   0        0        0      371 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     5020 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4144 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0      899 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     1089 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/product_block.py
+-rw-r--r--   0        0        0      889 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/resource_type.py
+-rw-r--r--   0        0        0      562 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/__init__.py
+-rw-r--r--   0        0        0     5591 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/inferred_filter.py
+-rw-r--r--   0        0        0     1466 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0     1276 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/filters/workflow.py
+-rw-r--r--   0        0        0      831 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/helpers.py
+-rw-r--r--   0        0        0    24900 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/models.py
+-rw-r--r--   0        0        0      162 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     2175 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      353 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0     1987 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      570 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0      617 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product_block.py
+-rw-r--r--   0        0        0      617 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/resource_type.py
+-rw-r--r--   0        0        0     4455 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0     1441 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0      576 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/db/sorting/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    18847 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/__init__.py
+-rw-r--r--   0        0        0     8359 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/migrate_20.py
+-rw-r--r--   0        0        0     2494 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2508 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3271 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      894 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    59246 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2732 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/customer_description.py
+-rw-r--r--   0        0        0      989 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/helpers.py
+-rw-r--r--   0        0        0     2882 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     1268 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0      892 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     1906 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/__init__.py
+-rw-r--r--   0        0        0     1505 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_contact_list.py
+-rw-r--r--   0        0        0      708 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_id.py
+-rw-r--r--   0        0        0      779 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/display_subscription.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/network_type_validators.py
+-rw-r--r--   0        0        0     2114 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/forms/validators/product_id.py
+-rw-r--r--   0        0        0     1482 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     6159 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/autoregistration.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4304 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1746 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     5826 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_handler_extension.py
+-rw-r--r--   0        0        0     3100 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/customer_description.py
+-rw-r--r--   0        0        0     1553 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/start_process.py
+-rw-r--r--   0        0        0     2413 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      851 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/customer.py
+-rw-r--r--   0        0        0      636 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/helpers.py
+-rw-r--r--   0        0        0     4491 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2562 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     2748 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product_block.py
+-rw-r--r--   0        0        0     2741 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/resource_type.py
+-rw-r--r--   0        0        0     3700 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     5888 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0     2681 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/workflow.py
+-rw-r--r--   0        0        0     7736 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schema.py
+-rw-r--r--   0        0        0      798 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/customer.py
+-rw-r--r--   0        0        0      213 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/customer_description.py
+-rw-r--r--   0        0        0      203 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3482 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2134 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0     1203 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      755 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      999 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7838 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0     1140 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     4905 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      524 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1191 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0     1002 2024-04-24 12:09:00.598062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0     3897 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py
+-rw-r--r--   0        0        0     2156 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/is_query_detailed.py
+-rw-r--r--   0        0        0     1370 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/override_class.py
+-rw-r--r--   0        0        0      902 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/to_graphql_result_page.py
+-rw-r--r--   0        0        0       39 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3382 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40911 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2698 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1265 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    39307 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      950 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1214 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1603 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5106 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7964 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0     1014 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0      591 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py
+-rw-r--r--   0        0        0      755 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql
+-rw-r--r--   0        0        0      967 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py
+-rw-r--r--   0        0        0     4491 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql
+-rw-r--r--   0        0        0     1036 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py
+-rw-r--r--   0        0        0     5383 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql
+-rw-r--r--   0        0        0     2246 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/py.typed
+-rw-r--r--   0        0        0     1066 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1526 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1234 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2195 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2708 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1286 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1356 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      802 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     2693 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1698 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1792 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      973 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3366 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1030 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1977 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1744 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3635 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/celery.py
+-rw-r--r--   0        0        0      876 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/fixed_inputs.py
+-rw-r--r--   0        0        0     3710 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/process_broadcast_thread.py
+-rw-r--r--   0        0        0    26253 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1933 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/products.py
+-rw-r--r--   0        0        0      884 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/resource_types.py
+-rw-r--r--   0        0        0     2723 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    25733 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5867 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1713 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     1638 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/services/workflows.py
+-rw-r--r--   0        0        0     3634 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/targets.py
+-rw-r--r--   0        0        0    16236 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5584 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0      875 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/deprecation_logger.py
+-rw-r--r--   0        0        0     6172 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4658 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/enrich_process.py
+-rw-r--r--   0        0        0     4250 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     2665 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/fixed_inputs.py
+-rw-r--r--   0        0        0     8063 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     1322 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/get_updated_properties.py
+-rw-r--r--   0        0        0     3212 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8341 2024-04-24 12:09:00.602062 orchestrator_core-2.2.2rc2/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     6378 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0    17039 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/search_query.py
+-rw-r--r--   0        0        0    12998 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     1366 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/version.py
+-rw-r--r--   0        0        0     4828 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     4596 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3324 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2924 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    42689 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4048 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9528 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2349 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8511 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12929 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     5073 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     2725 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/setup.cfg
+-rw-r--r--   0        0        0      665 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/setup.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1529 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2887 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5160 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1626 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1139 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3055 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    21379 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15509 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3787 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     8209 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2530 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     3000 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     3038 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    41173 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     3457 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0     3777 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/api/test_ws.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate.sh
+-rw-r--r--   0        0        0      885 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/alembic.ini
+-rw-r--r--   0        0        0      233 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/main.py
+-rw-r--r--   0        0        0     2821 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/env.py
+-rw-r--r--   0        0        0       98 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/script.py.mako
+-rw-r--r--   0        0        0      315 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_59e1199aff7f_create_data_head.py
+-rw-r--r--   0        0        0     2227 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py
+-rw-r--r--   0        0        0     3852 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py
+-rw-r--r--   0        0        0      467 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py
+-rw-r--r--   0        0        0      812 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py
+-rw-r--r--   0        0        0      559 2024-04-24 12:09:00.606062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py
+-rw-r--r--   0        0        0     1499 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py
+-rw-r--r--   0        0        0     1499 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py
+-rw-r--r--   0        0        0     2442 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py
+-rw-r--r--   0        0        0     2014 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py
+-rw-r--r--   0        0        0     1345 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py
+-rw-r--r--   0        0        0     1010 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py
+-rw-r--r--   0        0        0      902 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py
+-rw-r--r--   0        0        0      872 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py
+-rw-r--r--   0        0        0      755 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py
+-rw-r--r--   0        0        0      405 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_validate_example2.py
+-rw-r--r--   0        0        0      415 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/translations/en-GB.json
+-rw-r--r--   0        0        0      701 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/__init__.py
+-rw-r--r--   0        0        0     3940 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py
+-rw-r--r--   0        0        0     3602 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py
+-rw-r--r--   0        0        0      620 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py
+-rw-r--r--   0        0        0     1560 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py
+-rw-r--r--   0        0        0     1025 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py
+-rw-r--r--   0        0        0     2683 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py
+-rw-r--r--   0        0        0     2508 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py
+-rw-r--r--   0        0        0        1 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/shared/forms.py
+-rw-r--r--   0        0        0     1220 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py
+-rw-r--r--   0        0        0     1273 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/shared.py
+-rw-r--r--   0        0        0     2656 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config1.yaml
+-rw-r--r--   0        0        0      549 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config2.yaml
+-rw-r--r--   0        0        0      590 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config3.yaml
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/test_enums.py
+-rw-r--r--   0        0        0     2509 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_cli_generate.py
+-rw-r--r--   0        0        0     2930 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_generate_code.py
+-rw-r--r--   0        0        0    26343 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27644 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/config.py
+-rw-r--r--   0        0        0    23677 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    53002 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8230 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4670 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     1992 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_lifecycle.py
+-rw-r--r--   0        0        0     2841 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2970 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1606 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2573 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2518 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1194 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1123 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2172 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4217 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3428 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2951 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2272 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2256 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1639 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1838 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      644 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0      451 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     4706 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_contact_list.py
+-rw-r--r--   0        0        0      495 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_id.py
+-rw-r--r--   0        0        0     1746 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_display_subscription.py
+-rw-r--r--   0        0        0     4109 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/__init__.py
+-rw-r--r--   0        0        0     1424 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/conftest.py
+-rw-r--r--   0        0        0      488 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/helpers.py
+-rw-r--r--   0        0        0     6235 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_customer_description.py
+-rw-r--r--   0        0        0     2449 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_start_process.py
+-rw-r--r--   0        0        0     2316 2024-04-24 12:09:00.610062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_customer.py
+-rw-r--r--   0        0        0    18677 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     8514 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0    10211 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product_blocks.py
+-rw-r--r--   0        0        0     5635 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_resource_types.py
+-rw-r--r--   0        0        0     5179 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0     2939 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py
+-rw-r--r--   0        0        0     3239 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscription.py
+-rw-r--r--   0        0        0    48770 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0     6682 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_workflows.py
+-rw-r--r--   0        0        0      608 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_autoregistration.py
+-rw-r--r--   0        0        0     7669 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py
+-rw-r--r--   0        0        0     3042 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py
+-rw-r--r--   0        0        0     8760 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_override_class.py
+-rw-r--r--   0        0        0      631 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    28556 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1155 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     6171 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     6852 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      379 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    17406 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3486 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3529 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_get_updated_properties.py
+-rw-r--r--   0        0        0     3052 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     5867 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_search_query.py
+-rw-r--r--   0        0        0    11471 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/websocket/__init__.py
+-rw-r--r--   0        0        0     3561 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/websocket/test_broadcast.py
+-rw-r--r--   0        0        0    14040 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2443 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2746 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     5378 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_async_workflow.py
+-rw-r--r--   0        0        0     3495 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1884 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2024-04-24 12:09:00.614062 orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4574 1970-01-01 00:00:00.000000 orchestrator_core-2.2.2rc2/PKG-INFO
```

### Comparing `orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `orchestrator_core-2.2.2rc2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/README.md` & `orchestrator_core-2.2.2rc2/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/build-push-container.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/codeql-analysis.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/issues.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/issues.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/publish-package.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/run-linting-tests.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/run-unit-tests.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/run-unit-tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 name: Unit tests
 on:
   push:
   workflow_call:
 
 jobs:
   container_job:
-    name: Unit tests
+    name: Unit tests Python (${{ matrix.python-version }}) Postgres (${{ matrix.postgres-version }})
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.11', '3.12']
+        postgres-version: ['11', '12', '13', '14', '15', '16']
       fail-fast: false
     container: python:${{ matrix.python-version }}-slim
     services:
       postgres:
-        image: postgres:15-alpine
+        image: postgres:${{ matrix.postgres-version }}-alpine
         # Provide the password for postgres
         env:
           POSTGRES_PASSWORD: nwa
           POSTGRES_USER: nwa
         # Set health checks to wait until postgres has started
         options: >-
           --health-cmd pg_isready
```

### Comparing `orchestrator_core-2.2.2rc1/.github/workflows/scheduled-build.yml` & `orchestrator_core-2.2.2rc2/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.gitignore` & `orchestrator_core-2.2.2rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.pre-commit-config.yaml` & `orchestrator_core-2.2.2rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/.stignore` & `orchestrator_core-2.2.2rc2/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/CHANGELOG.md` & `orchestrator_core-2.2.2rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/LICENSE` & `orchestrator_core-2.2.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/README.md` & `orchestrator_core-2.2.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/callbacks.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/callbacks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/cli.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/domainmodels.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/forms.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/graphql.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/graphql.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,40 +23,106 @@
 app = OrchestratorCore(base_settings=AppSettings())
 # register SUBSCRIPTION_MODEL_REGISTRY
 app.register_graphql()
 ```
 
 ## Extending the Query and Mutation
 
+You are not able to remove resolvers from a Query, so we split the Query into 2 and merged them back for a default Query.
+Our usecase for this is that we use an external graphql source as our customers root.
+
+- `OrchestratorQuery` all resolvers except for customers.
+- `CustomerQuery` only has `customers` resolver.
+- `Query` Merges of `OrchestratorQuery` and `CustomerQuery` and serves as the default.
+
 This is an basic example of how to extend the query.
 You can do the same to extend Mutation.
 
 ```python
-from orchestrator.graphql import Query, Mutation
+from orchestrator.graphql import Query, Mutation, OrchestratorQuery
 
 
 # Queries
 def resolve_new(info) -> str:
     return "resolve new..."
 
 
+# with customers.
 @strawberry.federation.type(description="Orchestrator queries")
 class NewQuery(Query):
     other_processes: Connection[ProcessType] = authenticated_field(
         resolver=resolve_processes,
         description="resolve_processes used for another field",
     )
     new: str = strawberry.field(resolve_new, description="new resolver")
 
+# without customers.
+@strawberry.federation.type(description="Orchestrator queries")
+class NewQueryWithoutCustomers(OrchestratorQuery):
+    other_processes: Connection[ProcessType] = authenticated_field(
+        resolver=resolve_processes,
+        description="resolve_processes used for another field",
+    )
+    new: str = strawberry.field(resolve_new, description="new resolver")
+
 
 app = OrchestratorCore(base_settings=AppSettings())
 # register SUBSCRIPTION_MODEL_REGISTRY
 app.register_graphql(query=NewQuery)
 ```
 
+## Adding federated types to the graphql
+
+federation introduction: https://strawberry.rocks/docs/federation/introduction
+
+Within a federation, it is possible to add orchestrator data to graphql types from other sources by extending the `DEFAULT_GRAPHL_MODELS` dictionary with your own federated classes and adding them as parameter to `app.register_graphql(graphql_models={})`. Here is an example for when instead of overriding the customers resolver, you instead use a different graphql source (know that not storing any customer data in the orchestator will make filtering and sorting unavailable and very tricky to implement):
+
+```python
+import strawberry
+from sqlalchemy import select
+
+from oauth2_lib.strawberry import authenticated_field
+from orchestrator.db import db
+from orchestrator.graphql.pagination import Connection
+from orchestrator.graphql.schemas.subscription import SubscriptionInterface
+from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
+
+
+@strawberry.federation.type(description="Customer", keys=["customer_id"])
+class Customer:
+    customer_id: str
+
+    @classmethod
+    async def resolve_reference(cls, customer_id: str) -> "Customer":  # noqa: N803
+        return Customer(customer_id=customer_id)
+
+    @authenticated_field(description="Returns subscriptions of a customer")  # type: ignore
+    async def subscriptions(
+        self,
+        info: OrchestratorInfo,
+        filter_by: list[GraphqlFilter] | None = None,
+        sort_by: list[GraphqlSort] | None = None,
+        first: int = 10,
+        after: int = 0,
+    ) -> Connection[SubscriptionInterface]:
+        from orchestrator.graphql.resolvers.subscription import resolve_subscriptions
+
+        filter_by_customer_id = (filter_by or []) + [GraphqlFilter(field="customerId", value=str(self.uuid))]  # type: ignore
+        return await resolve_subscriptions(info, filter_by_customer_id, sort_by, first, after)
+
+UPDATED_GRAPHQL_MODELS = DEFAULT_GRAPHQL_MODELS | {
+    "Customer": Customer,
+}
+
+app.register_graphql(query=OrchestratorQuery, graphql_models=UPDATED_GRAPHQL_MODELS)
+```
+
+Types that are added in this way but aren't used in a resolver, will be viewable outside of a federation inside the types in the graphql ui interface.
+Adding product or product block strawberry types to the `graphql_models` will skip their generation inside `register_domain_models`. More info [here](#domain-models-auto-registration-for-graphql)
+
 ## Add Json schema for metadata
 
 The metadata in a subscription is completely unrestricted and can have anything.
 This functionality is to make metadata descriptive in a `__schema__` for the frontend to be able to render the metadata and know what to do with typing.
 
 example how to update the `__schema__`:
 
@@ -90,57 +156,62 @@
         "some_metadata_prop"
     ]
 }
 ```
 
 ## Domain Models Auto Registration for GraphQL
 
-When using the `register_graphql()` function, all products in the `SUBSCRIPTION_MODEL_REGISTRY` will be automatically converted into GraphQL types.
+When using the `app.register_graphql()` function, all products in the `SUBSCRIPTION_MODEL_REGISTRY` will be automatically converted into GraphQL types.
+You are able to turn this off with `app.register_graphql(register_models=False)`, but then you can only query fields from the default `SubscriptionModel`.
 The registration process iterates through the list, starting from the deepest product block and working its way back up to the product level.
 
-However, there is a potential issue when dealing with a `ProductBlock` that references itself, as it leads to an error expecting the `ProductBlock` type to exist.
+However, there is a potential issue when dealing with a `ProductBlock` that references itself, as it could lead to an error expecting the `ProductBlock` type to exist.
 
 Here is an example of the expected error with a self referenced `ProductBlock`:
 
 ```
 strawberry.experimental.pydantic.exceptions.UnregisteredTypeException: Cannot find a Strawberry Type for <class 'products.product_blocks.product_block_file.ProductBlock'> did you forget to register it?
 ```
 
-To handle this situation, you must manually create the GraphQL type for that `ProductBlock` and add it to the `GRAPHQL_MODELS` list.
+To handle this situation, you must manually create the GraphQL type for that `ProductBlock` and add it to the `DEFAULT_GRAPHQL_MODELS` list.
 
 Here's an example of how to do it:
 
 ```python
 # product_block_file.py
 import strawberry
 from typing import Annotated
 from app.product_blocks import ProductBlock
-from orchestrator.graphql import GRAPHQL_MODELS
+from orchestrator.graphql import DEFAULT_GRAPHQL_MODELS
 
 
 # It is necessary to use pydantic type, so that other product blocks can recognize it when typing to GraphQL.
 @strawberry.experimental.pydantic.type(model=ProductBlock)
 class ProductBlockGraphql:
     name: strawberry.auto
     self_reference_block: Annotated[
         "ProductBlockGraphql", strawberry.lazy(".product_block_file")
     ] | None = None
     ...
 
 
-# Add the ProductBlockGraphql type to GRAPHQL_MODELS, which is used in auto-registration for already created product blocks.
-GRAPHQL_MODELS.update({"ProductBlockGraphql": ProductBlockGraphql})
+# Add the ProductBlockGraphql type to GRAPHQL_MODELS, which skips its auto-register and used for products or product blocks dependant on it.
+UPDATED_GRAPHQL_MODELS = DEFAULT_GRAPHQL_MODELS | {
+    "ProductBlockGraphql": ProductBlockGraphql,
+}
+
+app.register_graphql(query=OrchestratorQuery, graphql_models=UPDATED_GRAPHQL_MODELS)
 ```
 
-By following this example, you can effectively create the necessary GraphQL type for `ProductBlock` and ensure proper registration with `register_graphql()`. This will help you avoid any `Cannot find a Strawberry Type` scenarios and enable smooth integration of domain models with GraphQL.
+By following this example, you can effectively create the necessary GraphQL type for `ProductBlock` and ensure proper registration with `app.register_graphql()`. This will help you avoid any `Cannot find a Strawberry Type` scenarios and enable smooth integration of domain models with GraphQL.
 
 ### Scalars for Auto Registration
 
 When working with special types such as `VlanRanges` or `IPv4Interface` in the core module, scalar types are essential for the auto registration process.
-Scalar types enable smooth integration of these special types into the GraphQL schema, They need to be initialized before `register_graphql()`.
+Scalar types enable smooth integration of these special types into the GraphQL schema, They need to be initialized and can be added with a dict to `app.register_graphql(scalar_overrides={})`.
 
 Here's an example of how to add a new scalar:
 
 ```python
 import strawberry
 from typing import NewType
 from orchestrator.graphql import SCALAR_OVERRIDES
@@ -149,28 +220,27 @@
     NewType("VlanRangesType", str),
     description="Represent the Orchestrator VlanRanges data type",
     serialize=lambda v: v.to_list_of_tuples(),
     parse_value=lambda v: v,
 )
 
 # Add the scalar to the SCALAR_OVERRIDES dictionary, with the type in the product block as the key and the scalar as the value
-SCALAR_OVERRIDES.update(
-    {
-        VlanRanges: VlanRangesType,
-    }
-)
+UPDATED_SCALAR_OVERRIDES = SCALAR_OVERRIDES | {
+    VlanRanges: VlanRangesType,
+}
+
+app.register_graphql(other_params..., scalar_overrides=UPDATED_SCALAR_OVERRIDES)
 ```
 
 You can find more examples of scalar usage in the `orchestrator/graphql/types.py` file.
 For additional information on Scalars, please refer to the Strawberry documentation on Scalars: https://strawberry.rocks/docs/types/scalars.
 
 By using scalar types for auto registration, you can seamlessly incorporate special types into your GraphQL schema, making it easier to work with complex data in the Orchestrator application.
 
 
-
 ### Federating with Autogenerated Types
 
 To enable federation, set the `FEDERATION_ENABLED` environment variable to `True`.
 
 Federation allows you to federate with subscriptions using the `subscriptionId` and with product blocks inside the subscription by utilizing any property that includes `_id` in its name.
 
 Below is an example of a GraphQL app that extends the `SubscriptionInterface`:
@@ -371,15 +441,15 @@
 Overriding strawberry types can be achieved through various methods. One less desirable approach involves extending classes using class inheritance.
 However, this method becomes cumbersome when updating a single class, as it necessitates updating all associated types and their corresponding resolvers, essentially impacting the entire structure.
 
 For instance, consider the scenario of overriding the `CustomerType`. you would need to update the related `SubscriptionInterface`, `ProcessType` and their respective resolvers. due to these modifications, all their related types and resolvers would also require updates, resulting in a tedious and error-prone process.
 
 To enhance the override process, we created a helper function `override_class` to override fields. It takes the base class as well as a list of fields that will replace their counterparts within the class or add new fields.
 
-It's worth noting that `SubscriptionInterface` poses a unique challenge due to its auto-generated types. The issue arises from the fact that the models inherited from `SubscriptionInterface` do not automatically update. This can be addressed by utilizing the `override_class` function and incorporating the returned class into the `register_graphql` function. This ensures that the updated class, with overridden fields, becomes the basis for generating the auto-generated models.
+It's worth noting that `SubscriptionInterface` poses a unique challenge due to its auto-generated types. The issue arises from the fact that the models inherited from `SubscriptionInterface` do not automatically update. This can be addressed by utilizing the `override_class` function and incorporating the returned class into the `app.register_graphql` function. This ensures that the updated class, with overridden fields, becomes the basis for generating the auto-generated models.
 
 ```python
 # Define a custom subscription interface using the `override_class` function, incorporating specified override fields.
 custom_subscription_interface = override_class(SubscriptionInterface, override_fields)
 
 # Register the customized subscription interface when setting up GraphQL in your application.
 app.register_graphql(subscription_interface=custom_subscription_interface)
```

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/openapi.json` & `orchestrator_core-2.2.2rc2/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/python.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/scaling.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/tasks.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/websockets.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/application/workflow.md` & `orchestrator_core-2.2.2rc2/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/context.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/context.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/introduction.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/ip_static.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/ip_static.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_point_to_point.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_point_to_point.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/l2_vpn.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/l2_vpn.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/modelling.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/modelling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/node.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/node.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/port.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/port.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/product_block_graph.png` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/product_block_graph.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/standards.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/standards.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/product_modelling/terminology.md` & `orchestrator_core-2.2.2rc2/docs/architecture/product_modelling/terminology.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/architecture/tldr.md` & `orchestrator_core-2.2.2rc2/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/contributing/guidelines.md` & `orchestrator_core-2.2.2rc2/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/contributing/testing.md` & `orchestrator_core-2.2.2rc2/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/css/style.css` & `orchestrator_core-2.2.2rc2/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/css/termynal.css` & `orchestrator_core-2.2.2rc2/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/getting-started/base.md` & `orchestrator_core-2.2.2rc2/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/getting-started/development.md` & `orchestrator_core-2.2.2rc2/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/getting-started/prepare-source-folder.md` & `orchestrator_core-2.2.2rc2/docs/getting-started/prepare-source-folder.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/img/WFO-Emblem-White.png` & `orchestrator_core-2.2.2rc2/docs/img/WFO-Emblem-White.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/img/favicon.ico` & `orchestrator_core-2.2.2rc2/docs/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/index.md` & `orchestrator_core-2.2.2rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/js/custom.js` & `orchestrator_core-2.2.2rc2/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/js/termynal.js` & `orchestrator_core-2.2.2rc2/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/migration-guide/2.0.md` & `orchestrator_core-2.2.2rc2/docs/migration-guide/2.0.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/domain-models.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/overview.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/scenario.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-2.2.2rc2/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/create-user.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/database-migration.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/debian.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/docker.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/domain-models.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/explore.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/input-forms.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/macos.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/modify-user.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/overview.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/scenario.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/start-applications.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-2.2.2rc2/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/images/metadata_products.png` & `orchestrator_core-2.2.2rc2/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-2.2.2rc2/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/mkdocs.yml` & `orchestrator_core-2.2.2rc2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/mutmut_config.py` & `orchestrator_core-2.2.2rc2/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "2.2.2rc1"
+__version__ = "2.2.2rc2"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/api.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/api_v1/endpoints/ws.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/api_v1/endpoints/ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/error_handling.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/api/models.py` & `orchestrator_core-2.2.2rc2/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/app.py` & `orchestrator_core-2.2.2rc2/orchestrator/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from orchestrator.db import db, init_database
 from orchestrator.db.database import DBSessionMiddleware
 from orchestrator.distlock import init_distlock_manager
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY, SubscriptionModel
 from orchestrator.exception_handlers import problem_detail_handler
 from orchestrator.graphql import Mutation, Query, create_graphql_router
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface
+from orchestrator.graphql.types import ScalarOverrideType, StrawberryModelType
 from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 from orchestrator.settings import AppSettings, ExecutorType, app_settings
 from orchestrator.version import GIT_COMMIT_HASH
 from orchestrator.websocket import init_websocket_manager
 from pydantic_forms.exception_handlers.fastapi import form_error_handler
 from pydantic_forms.exceptions import FormException
 
@@ -184,17 +185,25 @@
 
     def register_graphql(
         self: "OrchestratorCore",
         query: Any = Query,
         mutation: Any = Mutation,
         register_models: bool = True,
         subscription_interface: Any = SubscriptionInterface,
+        graphql_models: StrawberryModelType | None = None,
+        scalar_overrides: ScalarOverrideType | None = None,
     ) -> None:
         new_router = create_graphql_router(
-            query, mutation, register_models, subscription_interface, self.broadcast_thread
+            query,
+            mutation,
+            register_models,
+            subscription_interface,
+            self.broadcast_thread,
+            graphql_models,
+            scalar_overrides,
         )
         if not self.graphql_router:
             self.graphql_router = new_router
             self.include_router(new_router, prefix="/api/graphql")
         else:
             self.graphql_router.schema = new_router.schema
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/database.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generate.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/enums.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/generator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/lazy_workflow_instance.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/lazy_workflow_instance.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/shared_workflows.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/shared_workflows.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-2.2.2rc2/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/main.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/migration_helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/cli/scheduler.py` & `orchestrator_core-2.2.2rc2/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/config/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/config/assignee.py` & `orchestrator_core-2.2.2rc2/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/database.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/filters.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/process.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from orchestrator.db.filters import create_memoized_field_list, generic_filter_from_clauses
 from orchestrator.db.filters.search_filters import (
     default_inferred_column_clauses,
     filter_exact,
     inferred_filter,
     node_to_str_val,
 )
+from orchestrator.db.filters.search_filters.inferred_filter import filter_uuid_exact
 from orchestrator.utils.search_query import Node, WhereCondGenerator
 
 logger = structlog.get_logger(__name__)
 
 
 def make_product_clause(filter_generator: WhereCondGenerator) -> WhereCondGenerator:
     """The passed filter_generator takes a Node and returns a where clause acting on a ProductTable column."""
@@ -61,17 +62,15 @@
     )
     return ProcessTable.process_id.in_(process_subscriptions)
 
 
 def make_subscription_id_clause(filter_generator: WhereCondGenerator) -> WhereCondGenerator:
     def subscription_id_clause(node: Node) -> BinaryExpression:
 
-        process_subscriptions = (
-            select(ProcessSubscriptionTable.process_id).join(SubscriptionTable).where(filter_generator(node)).subquery()
-        )
+        process_subscriptions = select(ProcessSubscriptionTable.process_id).where(filter_generator(node)).subquery()
 
         return ProcessTable.process_id.in_(process_subscriptions)
 
     return subscription_id_clause
 
 
 def workflow_name_clause(node: Node) -> BinaryExpression:
@@ -96,15 +95,15 @@
     return ProcessTable.process_id.in_(process_workflows)
 
 
 PROCESS_TABLE_COLUMN_CLAUSES = default_inferred_column_clauses(ProcessTable) | {
     "customer": customer_clause,
     "product": make_product_clause(inferred_filter(ProductTable.name)),
     "product_description": make_product_clause(inferred_filter(ProductTable.description)),
-    "subscription_id": make_subscription_id_clause(inferred_filter(SubscriptionTable.subscription_id)),
+    "subscription_id": make_subscription_id_clause(filter_uuid_exact(ProcessSubscriptionTable.subscription_id)),
     "tag": make_product_clause(filter_exact(ProductTable.tag)),
     "target": workflow_targets_clause,
     "workflow_name": workflow_name_clause,
 }
 
 
 process_filter_fields = create_memoized_field_list(PROCESS_TABLE_COLUMN_CLAUSES)
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/resource_type.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/search_filters/inferred_filter.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/search_filters/inferred_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,7 +148,21 @@
         if node[0] == "Word":
             return field.ilike(f"{node[1]}")
         if node[0] == "PrefixWord":
             return field.ilike(f"{node[1]}%")
         return _filter_string(field)(node)
 
     return _clause_gen
+
+
+def filter_uuid_exact(field: ColumnClause) -> WhereCondGenerator:
+    assert field.type.python_type == uuid.UUID  # noqa: S101
+
+    def _clause_gen(node: Node) -> BinaryExpression[bool] | ColumnElement[bool]:
+        try:
+            v = uuid.UUID(node_to_str_val(node))
+        except ValueError:
+            # Not a valid uuid
+            return sqlalchemy.false()
+        return eq(field, v)
+
+    return _clause_gen
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/filters/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/filters/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/models.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,17 @@
     commit_hash = mapped_column(String(40), nullable=True, default=GIT_COMMIT_HASH)
 
 
 class ProcessSubscriptionTable(BaseModel):
     __tablename__ = "processes_subscriptions"
 
     id = mapped_column(UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True)
-    process_id = mapped_column("pid", UUIDType, ForeignKey("processes.pid", ondelete="CASCADE"), index=True)
+    process_id = mapped_column(
+        "pid", UUIDType, ForeignKey("processes.pid", ondelete="CASCADE"), index=True, nullable=False
+    )
     process = relationship("ProcessTable", back_populates="process_subscriptions")
     subscription_id = mapped_column(UUIDType, ForeignKey("subscriptions.subscription_id"), nullable=False, index=True)
     subscription = relationship("SubscriptionTable", lazy=True)
     created_at = mapped_column(UtcTimestamp, server_default=text("current_timestamp()"), nullable=False)
     workflow_target = mapped_column(String(255), nullable=False, server_default=Target.CREATE)
 
 
@@ -533,15 +535,17 @@
         UniqueConstraint("customer_id", "subscription_id", name="uniq_customer_subscription_description"),
     )
 
 
 class SubscriptionTable(BaseModel):
     __tablename__ = "subscriptions"
 
-    subscription_id = mapped_column(UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True)
+    subscription_id = mapped_column(
+        UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True, nullable=False
+    )
     description = mapped_column(Text(), nullable=False)
     status = mapped_column(String(STATUS_LENGTH), nullable=False, index=True)
     product_id = mapped_column(UUIDType, ForeignKey("products.product_id"), nullable=False, index=True)
     product = relationship("ProductTable")
     customer_id = mapped_column(String, index=True, nullable=False)
     insync = mapped_column(Boolean())
     start_date = mapped_column(UtcTimestamp, nullable=True)
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/range/range.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/process.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/resource_type.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/sorting.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/db/sorting/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/db/sorting/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/devtools/populator.py` & `orchestrator_core-2.2.2rc2/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/devtools/scripts/migrate_20.py` & `orchestrator_core-2.2.2rc2/orchestrator/devtools/scripts/migrate_20.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/distlock/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/domain/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/domain/base.py` & `orchestrator_core-2.2.2rc2/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/domain/customer_description.py` & `orchestrator_core-2.2.2rc2/orchestrator/domain/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/domain/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/domain/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/domain/lifecycle.py` & `orchestrator_core-2.2.2rc2/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/exception_handlers.py` & `orchestrator_core-2.2.2rc2/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_contact_list.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/customer_id.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/customer_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/display_subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/network_type_validators.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/forms/validators/product_id.py` & `orchestrator_core-2.2.2rc2/orchestrator/forms/validators/product_id.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,33 @@
 from orchestrator.graphql.autoregistration import (
     EnumDict,
     add_class_to_strawberry,
     graphql_subscription_name,
     register_domain_models,
 )
 from orchestrator.graphql.schema import (
+    CustomerQuery,
     Mutation,
     OrchestratorGraphqlRouter,
+    OrchestratorQuery,
     OrchestratorSchema,
     Query,
     create_graphql_router,
     custom_context_dependency,
     get_context,
 )
-from orchestrator.graphql.schemas import GRAPHQL_MODELS
+from orchestrator.graphql.schemas import DEFAULT_GRAPHQL_MODELS
 from orchestrator.graphql.types import SCALAR_OVERRIDES
 
 __all__ = [
-    "GRAPHQL_MODELS",
+    "DEFAULT_GRAPHQL_MODELS",
     "SCALAR_OVERRIDES",
     "Query",
+    "OrchestratorQuery",
+    "CustomerQuery",
     "Mutation",
     "OrchestratorGraphqlRouter",
     "OrchestratorSchema",
     "custom_context_dependency",
     "get_context",
     "create_graphql_router",
     "EnumDict",
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/autoregistration.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/autoregistration.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from more_itertools import one
 from strawberry.experimental.pydantic.conversion_types import StrawberryTypeFromPydantic
 from strawberry.federation.schema_directives import Key
 from strawberry.unset import UNSET
 
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY
 from orchestrator.domain.base import DomainModel, get_depends_on_product_block_type_list
-from orchestrator.graphql.schemas import StrawberryModelType
+from orchestrator.graphql.types import StrawberryModelType
 from orchestrator.types import filter_nonetype, is_of_type, is_optional_type
 from orchestrator.utils.helpers import to_camel
 
 logger = structlog.get_logger(__name__)
 
 EnumDict = dict[str, EnumMeta]
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/extensions/error_handler_extension.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/extensions/error_handler_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/customer_description.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/mutations/start_process.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/mutations/start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/pagination.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/customer.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/resource_type.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import cast
 from uuid import UUID
 
 import structlog
+from graphql import GraphQLError
 from pydantic.alias_generators import to_camel as to_lower_camel
 from sqlalchemy import Select, func, select
+from strawberry.experimental.pydantic.conversion_types import StrawberryTypeFromPydantic
 
 from orchestrator.db import ProductTable, SubscriptionTable, db
 from orchestrator.db.filters import Filter
 from orchestrator.db.filters.subscription import (
     filter_by_query_string,
     filter_subscriptions,
     subscription_filter_fields,
@@ -31,15 +33,19 @@
     sort_subscriptions,
     subscription_sort_fields,
 )
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.schemas.product import ProductModelGraphql
 from orchestrator.graphql.schemas.subscription import SubscriptionInterface
-from orchestrator.graphql.types import GraphqlFilter, GraphqlSort, OrchestratorInfo
+from orchestrator.graphql.types import (
+    GraphqlFilter,
+    GraphqlSort,
+    OrchestratorInfo,
+)
 from orchestrator.graphql.utils import (
     create_resolver_error_handler,
     is_query_detailed,
     is_querying_page_data,
     to_graphql_result_page,
 )
 from orchestrator.types import SubscriptionLifecycle
@@ -52,42 +58,47 @@
     + [to_lower_camel(key) for key in ProductModelGraphql.__annotations__]
     + ["__typename"]
 )
 
 _is_subscription_detailed = is_query_detailed(base_sub_props, ("SubscriptionInterface",))
 
 
-def get_subscription_details(subscription: SubscriptionTable) -> SubscriptionInterface:
-    from orchestrator.graphql import GRAPHQL_MODELS
+def get_subscription_graphql_type(info: OrchestratorInfo, subscription_name: str) -> StrawberryTypeFromPydantic:
+    subscription_graphql_type = info.context.graphql_models.get(subscription_name)
+    if not subscription_graphql_type:
+        raise GraphQLError(message=f"No graphql type found for {subscription_name}")
+    return subscription_graphql_type
+
+
+def get_subscription_details(info: OrchestratorInfo, subscription: SubscriptionTable) -> SubscriptionInterface:
     from orchestrator.graphql.autoregistration import graphql_subscription_name
 
     subscription_details = SubscriptionModel.from_subscription(subscription.subscription_id)
     base_model = subscription_details.__base_type__ if subscription_details.__base_type__ else subscription_details
     base_subscription_details = base_model.from_other_lifecycle(  # type: ignore
         subscription_details, SubscriptionLifecycle.INITIAL, skip_validation=True
     )
     base_subscription_details.status = subscription_details.status
-    strawberry_type = GRAPHQL_MODELS[graphql_subscription_name(base_model.__name__)]  # type: ignore
-    return strawberry_type.from_pydantic(base_subscription_details)
+    strawberry_type = get_subscription_graphql_type(info, graphql_subscription_name(base_model.__name__))  # type: ignore
+    return strawberry_type.from_pydantic(base_subscription_details)  # type:ignore
 
 
-def format_base_subscription(subscription: SubscriptionTable) -> SubscriptionInterface:
-    from orchestrator.graphql import GRAPHQL_MODELS
+def format_subscription(info: OrchestratorInfo, subscription: SubscriptionTable) -> SubscriptionInterface:
+    if _is_subscription_detailed(info):
+        return get_subscription_details(info, subscription)
 
-    strawberry_type = GRAPHQL_MODELS["subscription"]
-    return strawberry_type.from_pydantic(subscription)
+    strawberry_type = get_subscription_graphql_type(info, "subscription")
+    return strawberry_type.from_pydantic(subscription)  # type:ignore
 
 
 async def resolve_subscription(info: OrchestratorInfo, id: UUID) -> SubscriptionInterface | None:
     stmt = select(SubscriptionTable).where(SubscriptionTable.subscription_id == id)
 
     if subscription := db.session.scalar(stmt):
-        if _is_subscription_detailed(info):
-            return get_subscription_details(subscription)
-        return format_base_subscription(subscription)
+        return format_subscription(info, subscription)
     return None
 
 
 async def resolve_subscriptions(
     info: OrchestratorInfo,
     filter_by: list[GraphqlFilter] | None = None,
     sort_by: list[GraphqlSort] | None = None,
@@ -115,16 +126,13 @@
     stmt = cast(Select, sort_subscriptions(stmt, pydantic_sort_by, _error_handler))
     total = db.session.scalar(select(func.count()).select_from(stmt.subquery()))
     stmt = apply_range_to_statement(stmt, after, after + first + 1)
 
     graphql_subscriptions = []
     if is_querying_page_data(info):
         subscriptions = db.session.scalars(stmt).all()
-        if _is_subscription_detailed(info):
-            graphql_subscriptions = [get_subscription_details(p) for p in subscriptions]
-        else:
-            graphql_subscriptions = [format_base_subscription(p) for p in subscriptions]
+        graphql_subscriptions = [format_subscription(info, p) for p in subscriptions]
     logger.info("Resolve subscriptions", filter_by=filter_by, total=graphql_subscriptions)
 
     return to_graphql_result_page(
         graphql_subscriptions, first, after, total, subscription_sort_fields(), subscription_filter_fields()
     )
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/resolvers/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/resolvers/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schema.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from strawberry.fastapi import GraphQLRouter
 from strawberry.tools import merge_types
 from strawberry.types import ExecutionContext
 from strawberry.utils.logging import StrawberryLogger
 
 from oauth2_lib.strawberry import authenticated_field
 from orchestrator.domain.base import SubscriptionModel
-from orchestrator.graphql.autoregistration import register_domain_models
+from orchestrator.graphql.autoregistration import create_subscription_strawberry_type, register_domain_models
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
 from orchestrator.graphql.extensions.error_handler_extension import ErrorHandlerExtension
 from orchestrator.graphql.mutations.customer_description import CustomerSubscriptionDescriptionMutation
 from orchestrator.graphql.mutations.start_process import ProcessMutation
 from orchestrator.graphql.pagination import Connection
 from orchestrator.graphql.resolvers import (
     SettingsMutation,
@@ -41,35 +41,35 @@
     resolve_products,
     resolve_resource_types,
     resolve_settings,
     resolve_subscriptions,
     resolve_workflows,
 )
 from orchestrator.graphql.resolvers.subscription import resolve_subscription
-from orchestrator.graphql.schemas import GRAPHQL_MODELS
+from orchestrator.graphql.schemas import DEFAULT_GRAPHQL_MODELS
 from orchestrator.graphql.schemas.customer import CustomerType
 from orchestrator.graphql.schemas.process import ProcessType
 from orchestrator.graphql.schemas.product import ProductType
 from orchestrator.graphql.schemas.product_block import ProductBlock
 from orchestrator.graphql.schemas.resource_type import ResourceType
 from orchestrator.graphql.schemas.settings import StatusType
-from orchestrator.graphql.schemas.subscription import SubscriptionInterface, federation_key_directives
+from orchestrator.graphql.schemas.subscription import SubscriptionInterface
 from orchestrator.graphql.schemas.workflow import Workflow
-from orchestrator.graphql.types import SCALAR_OVERRIDES, OrchestratorContext
+from orchestrator.graphql.types import SCALAR_OVERRIDES, OrchestratorContext, ScalarOverrideType, StrawberryModelType
 from orchestrator.security import get_oidc_user, get_opa_security_graphql
 from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 from orchestrator.settings import app_settings
 
 api_router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
 
 @strawberry.federation.type(description="Orchestrator queries")
-class Query:
+class OrchestratorQuery:
     processes: Connection[ProcessType] = authenticated_field(
         resolver=resolve_processes, description="Returns list of processes"
     )
     products: Connection[ProductType] = authenticated_field(
         resolver=resolve_products, description="Returns list of products"
     )
     product_blocks: Connection[ProductBlock] = authenticated_field(
@@ -87,19 +87,24 @@
     subscriptions: Connection[SubscriptionInterface] = authenticated_field(
         resolver=resolve_subscriptions, description="Returns list of subscriptions"
     )
     settings: StatusType = authenticated_field(
         resolver=resolve_settings,
         description="Returns information about cache, workers, and global engine settings",
     )
+
+
+@strawberry.federation.type(description="Orchestrator customer Query")
+class CustomerQuery:
     customers: Connection[CustomerType] = authenticated_field(
         resolver=resolve_customer, description="Returns default customer information"
     )
 
 
+Query = merge_types("Query", (OrchestratorQuery, CustomerQuery))
 Mutation = merge_types("Mutation", (SettingsMutation, CustomerSubscriptionDescriptionMutation, ProcessMutation))
 
 OrchestratorGraphqlRouter = GraphQLRouter
 
 
 class OrchestratorSchema(strawberry.federation.Schema):
     def process_errors(
@@ -126,56 +131,50 @@
     get_current_user: Callable = Depends(get_oidc_user),  # noqa: B008
     get_opa_decision: Callable = Depends(get_opa_security_graphql),  # noqa: B008
 ) -> OrchestratorContext:
     return OrchestratorContext(get_current_user=get_current_user, get_opa_decision=get_opa_decision)
 
 
 def get_context(
+    graphql_models: StrawberryModelType,
     broadcast_thread: ProcessDataBroadcastThread | None = None,
 ) -> Callable[[OrchestratorContext], Coroutine[Any, Any, OrchestratorContext]]:
     async def _get_context(
         custom_context: OrchestratorContext = Depends(custom_context_dependency),  # noqa: B008
     ) -> OrchestratorContext:
         custom_context.broadcast_thread = broadcast_thread
+        custom_context.graphql_models = graphql_models
         return custom_context
 
     return _get_context
 
 
-GRAPHQL_MODELS_INITIAL = dict(GRAPHQL_MODELS)
-
-
 def create_graphql_router(
     query: Any = Query,
     mutation: Any = Mutation,
     register_models: bool = True,
-    subscription_interface: type | None = SubscriptionInterface,
+    subscription_interface: type = SubscriptionInterface,
     broadcast_thread: ProcessDataBroadcastThread | None = None,
+    graphql_models: StrawberryModelType | None = None,
+    scalar_overrides: ScalarOverrideType | None = None,
 ) -> OrchestratorGraphqlRouter:
-    @strawberry.experimental.pydantic.type(
-        model=SubscriptionModel, all_fields=True, directives=federation_key_directives
+    scalar_overrides = scalar_overrides if scalar_overrides else dict(SCALAR_OVERRIDES)
+    models = graphql_models if graphql_models else dict(DEFAULT_GRAPHQL_MODELS)
+    models["subscription"] = create_subscription_strawberry_type(
+        "Subscription", SubscriptionModel, subscription_interface
     )
-    class Subscription(SubscriptionInterface):
-        pass
-
-    models = dict(GRAPHQL_MODELS_INITIAL)
-    models["subscription"] = Subscription
 
     if register_models:
         models = register_domain_models(subscription_interface, existing_models=models)
-        GRAPHQL_MODELS.update(models)
 
     schema = OrchestratorSchema(
         query=query,
         mutation=mutation,
         enable_federation_2=app_settings.FEDERATION_ENABLED,
         types=tuple(models.values()),
         extensions=[ErrorHandlerExtension, make_deprecation_checker_extension(query=query)],
-        scalar_overrides=SCALAR_OVERRIDES,
+        scalar_overrides=scalar_overrides,
     )
 
     return OrchestratorGraphqlRouter(
-        schema, context_getter=get_context(broadcast_thread), graphiql=app_settings.SERVE_GRAPHQL_UI
+        schema, context_getter=get_context(models, broadcast_thread), graphiql=app_settings.SERVE_GRAPHQL_UI
     )
-
-
-graphql_router = create_graphql_router()
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/process.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from orchestrator.schemas.process import ProcessSchema, ProcessStepSchema
 from orchestrator.settings import app_settings
 
 if TYPE_CHECKING:
     from orchestrator.graphql.schemas.subscription import SubscriptionInterface
 
 
-federation_key_directives = [Key(fields="id", resolvable=UNSET)]
+federation_key_directives = [Key(fields="processId", resolvable=UNSET)]
 
 
 @strawberry.experimental.pydantic.type(model=ProcessStepSchema)
 class ProcessStepType:
     step_id: strawberry.auto
     name: strawberry.auto
     status: strawberry.auto
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/resource_type.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/schemas/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/types.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,51 +11,58 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Awaitable, Callable
 from ipaddress import IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 
 # Map some Orchestrator types to scalars
-from typing import Any, NewType
+from typing import Any, NewType, TypeVar
 
 import strawberry
 from graphql import GraphQLError
 from starlette.requests import Request
 from strawberry.custom_scalar import ScalarDefinition, ScalarWrapper
+from strawberry.experimental.pydantic.conversion_types import StrawberryTypeFromPydantic
 from strawberry.scalars import JSON
 from strawberry.types import Info
 from strawberry.types.info import RootValueType
 
 from nwastdlib.vlans import VlanRanges
 from oauth2_lib.fastapi import OIDCUserModel
 from oauth2_lib.strawberry import OauthContext
 from orchestrator.db.filters import Filter
 from orchestrator.db.sorting import Sort, SortOrder
 from orchestrator.services.process_broadcast_thread import ProcessDataBroadcastThread
 
+StrawberryPydanticModel = TypeVar("StrawberryPydanticModel", bound=StrawberryTypeFromPydantic)
+StrawberryModelType = dict[str, StrawberryPydanticModel]
+
 
 def serialize_to_string(value: Any) -> str:
     return str(value)
 
 
 def serialize_vlan(vlan: VlanRanges) -> list[tuple[int, int]]:
     return vlan.to_list_of_tuples()
 
 
 class OrchestratorContext(OauthContext):
-    broadcast_thread: ProcessDataBroadcastThread | None = None
+    broadcast_thread: ProcessDataBroadcastThread | None
+    graphql_models: StrawberryModelType
 
     def __init__(
         self,
         get_current_user: Callable[[Request], Awaitable[OIDCUserModel]],
         get_opa_decision: Callable[[str, OIDCUserModel], Awaitable[bool | None]],
         broadcast_thread: ProcessDataBroadcastThread | None = None,
+        graphql_models: StrawberryModelType | None = None,
     ):
         self.errors: list[GraphQLError] = []
         self.broadcast_thread = broadcast_thread
+        self.graphql_models = graphql_models or {}
         super().__init__(get_current_user, get_opa_decision)
 
 
 OrchestratorInfo = Info[OrchestratorContext, RootValueType]
 
 
 @strawberry.experimental.pydantic.input(model=Sort)
@@ -108,15 +115,16 @@
 IntType = strawberry.scalar(
     NewType("Int", int),
     description="An arbitrary precision integer",
     serialize=lambda v: v,
     parse_value=lambda v: v,
 )
 
-SCALAR_OVERRIDES: dict[object, Any | ScalarWrapper | ScalarDefinition] = {
+ScalarOverrideType = dict[object, type | ScalarWrapper | ScalarDefinition]
+SCALAR_OVERRIDES: ScalarOverrideType = {
     dict: JSON,
     VlanRanges: VlanRangesType,
     IPv4Address: IPv4AddressType,
     IPv6Address: IPv6AddressType,
     IPv4Interface: IPv4InterfaceType,
     IPv6Interface: IPv6InterfaceType,
     int: IntType,
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/get_subscription_product_blocks.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/get_subscription_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/is_query_detailed.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/override_class.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/graphql/utils/to_graphql_result_page.py` & `orchestrator_core-2.2.2rc2/orchestrator/graphql/utils/to_graphql_result_page.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/alembic.ini` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/env.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-06-28_a09ac125ea73_add_throttling_to_refresh_subscriptions.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-07-17_165303a20fb1_customer_id_to_varchar.sql`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-09-25_da5c9f4cce1c_add_subscription_metadata_to_fulltext_.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,72 @@
 -- Must drop the materialized view and recreate, as you cannot edit it directly/any of its dependencies
 DROP MATERIALIZED VIEW IF EXISTS subscriptions_search;
 
 -- Recreate the view
 CREATE MATERIALIZED VIEW IF NOT EXISTS subscriptions_search AS
 WITH rt_info AS (SELECT s.subscription_id,
                         concat_ws(
-                                ', ',
-                                string_agg(
-                                                rt.resource_type || ':' || siv.value,
-                                                ', '
-                                                ORDER BY rt.resource_type
-                                    ),
-                                string_agg(
-                                        distinct 'subscription_instance_id' || ':' || si.subscription_instance_id,
-                                        ', '
-                                    )
-                            ) AS rt_info
+                                ' ',
+                                string_agg(rt.resource_type || ' ' || siv.value, ' '),
+                                string_agg(distinct 'subscription_instance_id' || ':' || si.subscription_instance_id, ' ')
+                        ) AS rt_info
                  FROM subscription_instance_values siv
                           JOIN resource_types rt ON siv.resource_type_id = rt.resource_type_id
                           JOIN subscription_instances si ON siv.subscription_instance_id = si.subscription_instance_id
                           JOIN subscriptions s ON si.subscription_id = s.subscription_id
                  GROUP BY s.subscription_id),
      sub_prod_info AS (SELECT s.subscription_id,
                               array_to_string(
                                       ARRAY ['subscription_id:' || s.subscription_id,
                                           'status:' || s.status,
                                           'insync:' || s.insync,
                                           'subscription_description:' || s.description,
                                           'note:' || coalesce(s.note, ''),
                                           'customer_id:' || s.customer_id,
                                           'product_id:' || s.product_id],
-                                      ', '
-                                  ) AS sub_info,
+                                      ' '
+                              ) AS sub_info,
                               array_to_string(
                                       ARRAY ['product_name:' || p.name,
                                           'product_description:' || p.description,
                                           'tag:' || p.tag,
                                           'product_type:', p.product_type],
-                                      ', '
-                                  ) AS prod_info
+                                      ' '
+                              ) AS prod_info
                        FROM subscriptions s
                                 JOIN products p ON s.product_id = p.product_id),
      fi_info AS (SELECT s.subscription_id,
-                        string_agg(
-                                        fi.name || ':' || fi.value,
-                                        ', '
-                                        ORDER BY fi.name
-                            ) AS fi_info
+                        string_agg(fi.name || ':' || fi.value, ' ') AS fi_info
                  FROM subscriptions s
                           JOIN products p ON s.product_id = p.product_id
                           JOIN fixed_inputs fi ON p.product_id = fi.product_id
                  GROUP BY s.subscription_id),
      cust_info AS (SELECT s.subscription_id,
-                          string_agg(
-                                      'customer_description: ' || scd.description,
-                                      ', '
-                              ) AS cust_info
+                          string_agg('customer_description: ' || scd.description, ' ') AS cust_info
                    FROM subscriptions s
                             JOIN subscription_customer_descriptions scd ON s.subscription_id = scd.subscription_id
                    GROUP BY s.subscription_id)
+-- to_tsvector handles parsing of hyphened words in a peculiar way and is inconsistent with how to_tsquery parses it in Postgres <14
+-- Replacing all hyphens with underscores makes the parsing more predictable and removes some issues arising when searching for subscription ids for example
+-- See: https://git.postgresql.org/gitweb/?p=postgresql.git;a=commit;h=0c4f355c6a5fd437f71349f2f3d5d491382572b7
 SELECT s.subscription_id,
        to_tsvector(
                'simple',
-               concat_ws(
-                       ', ',
-                       spi.sub_info,
-                       spi.prod_info,
-                       fi.fi_info,
-                       rti.rt_info,
-                       ci.cust_info,
-                       md.metadata::text
-                   )
-           ) as tsv
+               replace(
+                       concat_ws(
+                               ' ',
+                               spi.sub_info,
+                               spi.prod_info,
+                               fi.fi_info,
+                               rti.rt_info,
+                               ci.cust_info,
+                               md.metadata::text
+                       ),
+                       '-', '_')
+       ) as tsv
 FROM subscriptions s
          LEFT JOIN sub_prod_info spi ON s.subscription_id = spi.subscription_id
          LEFT JOIN fi_info fi ON s.subscription_id = fi.subscription_id
          LEFT JOIN rt_info rti ON s.subscription_id = rti.subscription_id
          LEFT JOIN cust_info ci ON s.subscription_id = ci.subscription_id
          LEFT JOIN subscription_metadata md ON s.subscription_id = md.subscription_id;
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py` & `orchestrator_core-2.2.2rc2/orchestrator/migrations/versions/schema/2023-12-06_048219045729_add_workflow_id_to_processes_table.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/scheduling.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_products.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/base.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/engine_settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/fixed_input.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/problem_detail.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/process.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/product.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/product_block.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/resource_type.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/schemas/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/security.py` & `orchestrator_core-2.2.2rc2/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/celery.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/fixed_inputs.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/process_broadcast_thread.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/process_broadcast_thread.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/processes.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/products.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/resource_types.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/subscriptions.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/tasks.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/tasks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/translations.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/services/workflows.py` & `orchestrator_core-2.2.2rc2/orchestrator/services/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/settings.py` & `orchestrator_core-2.2.2rc2/orchestrator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/targets.py` & `orchestrator_core-2.2.2rc2/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/types.py` & `orchestrator_core-2.2.2rc2/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/crypt.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/datetime.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/deprecation_logger.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/deprecation_logger.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/docs.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/enrich_process.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/enrich_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/errors.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/fixed_inputs.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/functional.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/get_updated_properties.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/helpers.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/json.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/redis.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/search_query.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/search_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import re
 from collections.abc import Callable, Iterable, Iterator
 from enum import Enum
 from itertools import chain
 from typing import Any, Union, cast
 
 import structlog
-from sqlalchemy import BinaryExpression, ColumnElement, CompoundSelect, Select, false, not_, or_
+from sqlalchemy import BinaryExpression, ColumnElement, CompoundSelect, Select, column, false, func, not_, or_, select
 from sqlalchemy.orm import InstrumentedAttribute, MappedColumn
 
+from orchestrator.db import db
 from orchestrator.db.database import BaseModel
+from orchestrator.db.helpers import get_postgres_version
 from orchestrator.utils.helpers import camel_to_snake
 
 logger = structlog.getLogger(__name__)
 
 
 class Token(Enum):
     WORD = "WORD"
@@ -251,14 +253,38 @@
         self.it = iter(self.tokens)
         query = self.parse_query()
         self.expect(Token.END)
         return query
 
 
 class TSQueryVisitor:
+
+    _glue_chars = re.compile(r"[-_@#$%^&]")
+
+    @staticmethod
+    def _split_term(term: str) -> list[str]:
+        """Workaround for the way Postgres <14 parses text with to_tsquery.
+
+        For Postgres <14, we issue a database query to parse the text for us in a way that is compatible with to_tsvector. This is the same behavior as Postgres >=14.
+        """
+
+        # TODO: Remove this workaround when support for Postgres <14 is dropped
+        # https://github.com/workfloworchestrator/orchestrator-core/issues/621
+
+        if get_postgres_version() < 14:
+            # tokid 12 is the space separator token
+            stmt = (
+                select(func.array_agg(column("token")))
+                .select_from(func.ts_parse("default", func.replace(term, "-", "_")))
+                .where(column("tokid") != 12)
+            )
+            return db.session.scalar(stmt) or []
+
+        return TSQueryVisitor._glue_chars.split(term)
+
     @staticmethod
     def visit_group(node: Node, acc: list[str]) -> None:
         acc.append("(")
         for expr in node[1]:
             TSQueryVisitor.visit_and_expression(expr, acc)
             acc.append(" | ")
         acc.pop()
@@ -283,24 +309,36 @@
             acc.pop()
             acc.append(")")
         else:
             TSQueryVisitor.visit_term(value_node, acc)
 
     @staticmethod
     def visit_search_word(node: Node, acc: list[str]) -> None:
+
+        if node[0] not in ["Word", "PrefixWord"]:
+            raise Exception(f"Invalid SearchWord type {node[0]}")
+
         # Postgres is finicky with single quotes in the query. In some situations it throws an error.
         # To avoid the special handling of ' by PG, we replace it with double quotes.
-        # We also replace underscores with the 'followed by' operator
-        text = node[1].replace("'", '"').replace("_", " <-> ")
-        if node[0] == "Word":
-            acc.append(text)
-        elif node[0] == "PrefixWord":
-            acc.append(f"{text}:*")
-        else:
-            raise Exception(f"Invalid SearchWord type {node[0]}")
+
+        text = node[1].replace("'", '"')
+
+        parts = TSQueryVisitor._split_term(text)
+
+        if not parts:
+            return
+
+        text = " <-> ".join(parts)
+
+        if node[0] == "PrefixWord":
+            text = f"{text}:*"
+
+        # Wrap parentheses for clarity, even though <-> has the highest operator precedence
+        text = f"({text})" if len(parts) > 1 else text
+        acc.append(text)
 
     @staticmethod
     def visit_phrase(node: Node, acc: list[str]) -> None:
         for search_word in node[1]:
             TSQueryVisitor.visit_search_word(search_word, acc)
             acc.append(" <-> ")
```

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/state.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/utils/strings.py` & `orchestrator_core-2.2.2rc2/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/version.py` & `orchestrator_core-2.2.2rc2/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/websocket/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-2.2.2rc2/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/modify_note.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/steps.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/orchestrator/workflows/utils.py` & `orchestrator_core-2.2.2rc2/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/pyproject.toml` & `orchestrator_core-2.2.2rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/setup.cfg` & `orchestrator_core-2.2.2rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/setup.py` & `orchestrator_core-2.2.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/conftest.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/acceptance_tests/test_test_product.py` & `orchestrator_core-2.2.2rc2/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_caching.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_health.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_helpers.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_models.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_product_blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from uuid import uuid4
 
 import pytest
 from sqlalchemy import delete
 
 from orchestrator.db import ProductBlockTable, ProductTable, ResourceTypeTable, db
 from test.unit_tests.config import IMS_CIRCUIT_ID
-from test.unit_tests.helpers import URL_MISSING
 
 PRODUCT_BLOCK_ID = "f51f9542-e83f-42e5-a590-0284dd5493e4"
 
 
 @pytest.fixture
 def seed():
     db.session.execute(delete(ProductBlockTable))
@@ -71,16 +70,16 @@
 
 def test_save_invalid_product_block(seed, test_client):
     response = test_client.post("/api/product_blocks/", json=({}))
 
     assert HTTPStatus.UNPROCESSABLE_ENTITY == response.status_code
     assert {
         "detail": [
-            {"type": "missing", "loc": ["body", "name"], "msg": "Field required", "input": {}} | URL_MISSING,
-            {"type": "missing", "loc": ["body", "description"], "msg": "Field required", "input": {}} | URL_MISSING,
+            {"type": "missing", "loc": ["body", "name"], "msg": "Field required", "input": {}},
+            {"type": "missing", "loc": ["body", "description"], "msg": "Field required", "input": {}},
         ]
     } == response.json()
 
 
 def test_update_product_block(seed, test_client):
     body = {"product_block_id": PRODUCT_BLOCK_ID, "name": "Circuit", "description": "desc", "status": "end of life"}
     response = test_client.put("/api/product_blocks/", json=body)
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_products.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_resource_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from http import HTTPStatus
 from uuid import uuid4
 
 import pytest
 from sqlalchemy import delete
 
 from orchestrator.db import ProductBlockTable, ResourceTypeTable, db
-from test.unit_tests.helpers import URL_MISSING
 
 RESOURCE_TYPE_ID = "f51f9542-e83f-42e5-a590-0284dd5493e4"
 
 
 @pytest.fixture
 def seed():
     # Delete current resource types
@@ -40,17 +39,15 @@
 
 
 def test_save_invalid_resource_type(seed, test_client):
     response = test_client.post("/api/resource_types/", json={})
 
     assert HTTPStatus.UNPROCESSABLE_ENTITY == response.status_code
     assert {
-        "detail": [
-            {"type": "missing", "loc": ["body", "resource_type"], "msg": "Field required", "input": {}} | URL_MISSING
-        ]
+        "detail": [{"type": "missing", "loc": ["body", "resource_type"], "msg": "Field required", "input": {}}]
     } == response.json()
 
 
 def test_update_resource_type(seed, test_client):
     body = {"resource_type_id": RESOURCE_TYPE_ID, "resource_type": "changed"}
     response = test_client.put("/api/resource_types/", json=body)
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_settings.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_workflows.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/api/test_ws.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate.sh` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate.sh`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/alembic.ini` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/env.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_85be1c80731c_add_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/migrations/versions/schema/2024-02-20_ea9e6c9de75c_add_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_blocks/example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_blocks/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/products/product_types/example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/products/product_types/example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/domain/product_types/test_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example1/test_validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/test/unit_tests/workflows/example2/test_terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/__init__.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/create_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/modify_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/shared/forms.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/terminate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example1/validate_example1.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/create_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/modify_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/example2/terminate_example2.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/generate/workflows/shared.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/generate/workflows/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config1.yaml` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config1.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config2.yaml` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config2.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/data/product_config3.yaml` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/data/product_config3.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/generator/test_enums.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/generator/test_enums.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_cli_generate.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_cli_generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_generate_code.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_generate_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/conftest.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/domain/test_lifecycle.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/domain/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/processes.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/processes.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         mock_process(None, "running", first_datetime + timedelta(days=4), is_task=True),
         mock_process(None, "resumed", first_datetime + timedelta(days=5), is_task=True),
     ]
 
 
 @pytest.fixture
 def mocked_processes_resumeall(test_workflow, generic_subscription_1, generic_subscription_2):
-    first_datetime = datetime(2020, 1, 14, 9, 30, tzinfo=pytz.utc)
+    first_datetime = datetime(2020, 2, 14, 9, 30, tzinfo=pytz.utc)
 
     def mock_process(subscription_id, status, started, assignee=Assignee.SYSTEM, is_task=False):
         process_id = uuid4()
         process = ProcessTable(
             process_id=process_id,
             workflow_id=test_workflow.workflow_id,
             last_status=status,
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_customer_contact_list.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_customer_contact_list.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_display_subscription.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_display_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_customer_description.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_customer_description.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/mutations/test_start_process.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/mutations/test_start_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_customer.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_customer.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         "hasNextPage": True,
         "startCursor": 0,
         "endCursor": 9,
         "totalItems": 19,
     }
 
     assert processes[0]["startedAt"] == "2020-01-14T09:30:00+00:00"
-    assert processes[1]["startedAt"] == "2020-01-14T09:30:00+00:00"
+    assert processes[1]["startedAt"] == "2020-01-15T09:30:00+00:00"
     assert processes[2]["startedAt"] == "2020-01-15T09:30:00+00:00"
 
 
 def test_processes_sorting_desc(
     test_client,
     mocked_processes,
     mocked_processes_resumeall,
@@ -325,19 +325,19 @@
         "hasPreviousPage": False,
         "hasNextPage": True,
         "startCursor": 0,
         "endCursor": 9,
         "totalItems": 19,
     }
 
-    assert processes[0]["startedAt"] == "2020-01-19T09:30:00+00:00"
-    assert processes[1]["startedAt"] == "2020-01-19T09:30:00+00:00"
-    assert processes[2]["startedAt"] == "2020-01-19T09:30:00+00:00"
-    assert processes[3]["startedAt"] == "2020-01-19T09:30:00+00:00"
-    assert processes[4]["startedAt"] == "2020-01-18T09:30:00+00:00"
+    assert processes[0]["startedAt"] == "2020-02-19T09:30:00+00:00"
+    assert processes[1]["startedAt"] == "2020-02-19T09:30:00+00:00"
+    assert processes[2]["startedAt"] == "2020-02-18T09:30:00+00:00"
+    assert processes[3]["startedAt"] == "2020-02-17T09:30:00+00:00"
+    assert processes[4]["startedAt"] == "2020-02-16T09:30:00+00:00"
 
 
 @pytest.mark.parametrize(
     "query_args",
     [
         {"filter_by": [{"field": "lastStatus", "value": "completed"}]},
         {"query_string": "lastStatus:completed"},
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_product_blocks.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_resource_types.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_sort_and_filter_fields.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_sort_and_filter_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscription.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -975,14 +975,15 @@
     generic_subscription_1,
     query_args,
 ):
     # when
 
     product_type_1_subscriptions_factory(30)
     subscription_id = generic_subscription_1
+
     do_refresh_subscriptions_search_view()
 
     data = get_subscriptions_query_with_relations(**query_args(subscription_id))
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
@@ -1012,14 +1013,15 @@
     sub_one_subscription_1,
     sub_two_subscription_1,
     product_sub_list_union_subscription_1,
 ):
     # when
 
     product_type_1_subscriptions_factory(30)
+
     do_refresh_subscriptions_search_view()
 
     subscription_id = str(product_sub_list_union_subscription_1)
     data = get_subscriptions_query_with_relations(query_string=subscription_id)
     response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     expected_depends_on_ids = {
@@ -1056,15 +1058,15 @@
     product_type_1_subscriptions_factory,
     sub_one_subscription_1,
     product_sub_list_union_subscription_1,
 ):
     # when
 
     product_type_1_subscriptions_factory(30)
-    do_refresh_subscriptions_search_view()
+
     subscription_id = str(sub_one_subscription_1.subscription_id)
     subscription_query = get_subscriptions_query_with_relations(
         filter_by=[{"field": "subscriptionId", "value": subscription_id}]
     )
 
     response = test_client.post(
         "/api/graphql", content=subscription_query, headers={"Content-Type": "application/json"}
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/test_workflows.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_autoregistration.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_autoregistration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_query_detailed.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_query_detailed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_is_querying_page_data.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_is_querying_page_data.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/graphql/utils/test_override_class.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/graphql/utils/test_override_class.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/helpers.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_processes.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_products.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/services/test_translations.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/test_db.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/test_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from unittest import mock
 
 import pytest
 from sqlalchemy import select
 from sqlalchemy.exc import NoResultFound
 
 from orchestrator.db import ResourceTypeTable, SubscriptionTable, WorkflowTable, db, transactional
+from orchestrator.db.helpers import get_postgres_version
 from orchestrator.targets import Target
 
 
 def test_transactional():
     def insert_wf(state):
         wf = WorkflowTable(name="Test transactional", target=Target.CREATE, description="Testing 1, 2, 3!")
         db.session.add(wf)
@@ -170,7 +171,13 @@
 
 
 def test_str_method():
     assert (
         str(SubscriptionTable())
         == "SubscriptionTable(subscription_id=None, description=None, status=None, product_id=None, customer_id=None, insync=None, start_date=None, end_date=None, note=None)"
     )
+
+
+def test_get_postgres_version():
+    pg_version = get_postgres_version()
+    assert isinstance(pg_version, int)
+    assert 0 < pg_version < 20
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/test_workflow.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_errors.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_functional.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_get_updated_properties.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_get_updated_properties.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_json.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_search_query.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_search_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import uuid
+
 import pytest
-from sqlalchemy import Column, Integer, String, select
+from sqlalchemy import Column, Integer, String, func, select
 
+from orchestrator.db import db
 from orchestrator.db.database import BaseModel
 from orchestrator.db.helpers import to_sql_string
 from orchestrator.utils.search_query import Lexer, ParseError, Parser, TSQueryVisitor, create_sqlalchemy_select
 
 
 def _parse_tree_and_tsquery(q: str) -> tuple[tuple, str]:
     tokens = Lexer(q).lex()
@@ -56,18 +59,35 @@
 def test_parse_errors(query, msg):
     with pytest.raises(ParseError):
         _parse_tree_and_tsquery(query)
 
 
 def test_parse_edge_cases():
     # Just test whether this parses without error
-    q = "aa*bb@cc?dd>ee'ff_g<g[hh]ij$kk%;\\=+12`3€crazy!text kk|ll:''"
+    q = "aa*bb@cc?dd>ee'ff_g<g[hh]ij$kk%;\\=+12`3€crazy!text kk|ll:m"
     parse_tree, tsquery = _parse_tree_and_tsquery(q)
     assert tsquery.startswith("aa:*")
-    assert tsquery.endswith('| ll <-> ""')
+    assert tsquery.endswith("| ll <-> m")
+
+
+@pytest.mark.parametrize(
+    "query,expected_tsquery",
+    [
+        ("basic query example", "basic & query & example"),
+        ("example status:(suspended | terminated)", "example & status <-> (suspended | terminated)"),
+        (
+            "subscription_id:849fb72a-4366-4d41-9d37-3821d73e4dd4",
+            "(subscription <-> id) <-> (849fb72a <-> 4366 <-> 4d41 <-> 9d37 <-> 3821d73e4dd4)",
+        ),
+        ("something aaa_bbb else", "something & (aaa <-> bbb) & else"),
+    ],
+)
+def test_common_queries(query, expected_tsquery):
+    _, tsquery = _parse_tree_and_tsquery(query)
+    assert tsquery == expected_tsquery
 
 
 def test_parse_complex_query():
     q = "".join(
         [
             '"phrase1 phrase2 phrase3" word1 word2 prefixword* field1:(val1 | val2* | "val3 val4*")',
             " | ",
@@ -88,19 +108,19 @@
             "phrase21 <-> phrase22 & ((klm & tag <-> lp) | (sinica & tag <-> fw))",
             " & !(not <-> this & or <-> this) & something & else",
         ]
     )
 
 
 def test_query_with_underscores():
-    q = 'word_with_underscores prefix_word* key_value:term_1 key_value2:(val_1 | "val_2" | val_3*)'
+    q = 'word_with_underscores prefix_word* key_value:term_1 key_value2:(val1 | "val2" | val3*)'
     parse_tree, tsquery = _parse_tree_and_tsquery(q)
     assert (
         tsquery
-        == "word <-> with <-> underscores & prefix <-> word:* & key <-> value <-> term <-> 1 & key <-> value2 <-> (val <-> 1 | val <-> 2 | val <-> 3:*)"
+        == "(word <-> with <-> underscores) & (prefix <-> word:*) & (key <-> value) <-> (term <-> 1) & (key <-> value2) <-> (val1 | val2 | val3:*)"
     )
 
 
 def test_query_kv_camelcasing():
     q = "productTag:myTag"
     q2 = "product_tag:myTag"
     assert _parse_tree_and_tsquery(q)[1] == _parse_tree_and_tsquery(q2)[1]
@@ -125,7 +145,26 @@
     mappings = {"name": lambda node: MyTable.name.like(node[1].lower())}
     stmt = select(MyTable)
     stmt = create_sqlalchemy_select(stmt, search_query, mappings, MyTable, MyTable.id)
     for substring in substrings:
         assert substring in to_sql_string(stmt)
 
     MyTable.metadata.clear()
+
+
+@pytest.mark.parametrize("i", range(100))
+def test_uuid_queries(i):
+    # Tests whether a text search vector containing a UUID can be successfully queried
+    # This used to fail sometimes in Postgres <14 versions.
+
+    # TODO: Remove when support for Postgres <14 is dropped
+    uid = uuid.uuid4()
+
+    query = f"subscription_id:{uid}"
+    tsv = func.to_tsvector("simple", func.replace(query, "-", "_"))
+
+    _, ts_query = _parse_tree_and_tsquery(query)
+
+    stmt = select(tsv.op("@@")(func.to_tsquery("simple", ts_query)))
+
+    matches = db.session.scalar(stmt)
+    assert matches
```

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/utils/test_state.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/websocket/test_broadcast.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/websocket/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/__init__.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_async_workflow.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_async_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-2.2.2rc2/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-2.2.2rc1/PKG-INFO` & `orchestrator_core-2.2.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 2.2.2rc1
+Version: 2.2.2rc2
 Summary: This is the orchestrator workflow engine.
 Requires-Python: >=3.11,<3.13
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
```

