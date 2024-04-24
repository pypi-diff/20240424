# Comparing `tmp/pinjected-0.2.44.tar.gz` & `tmp/pinjected-0.2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.44.tar", max compression
+gzip compressed data, was "pinjected-0.2.45.tar", max compression
```

## Comparing `pinjected-0.2.44.tar` & `pinjected-0.2.45.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.44/LICENSE
--rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.44/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.44/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.44/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.44/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.44/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.44/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.44/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.44/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.44/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.44/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.44/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.44/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14618 2024-04-23 08:38:19.296348 pinjected-0.2.44/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.44/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.44/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.44/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.44/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.44/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.44/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.44/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.44/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.44/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.44/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.44/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.44/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.44/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.44/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.44/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.44/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.44/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.44/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.44/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.44/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.44/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1500 2024-03-20 13:37:29.443496 pinjected-0.2.44/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.44/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.44/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.44/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.44/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.44/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.44/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.44/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.44/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.44/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.44/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.44/pinjected/global_configs.py
--rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.44/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.44/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.44/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.44/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.44/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.44/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.44/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.44/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.44/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.44/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.44/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.44/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.44/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.44/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.44/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.44/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.44/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.44/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.44/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.44/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.44/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.44/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.44/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.44/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.44/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9546 2024-04-23 08:38:19.299938 pinjected-0.2.44/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.44/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.44/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.44/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.44/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.44/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.44/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.44/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     6128 2024-03-26 02:52:38.850654 pinjected-0.2.44/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.44/pinjected/v2/di.py
--rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.44/pinjected/v2/keys.py
--rw-r--r--   0        0        0      478 2024-03-26 02:52:38.851836 pinjected-0.2.44/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0     9722 2024-04-24 10:51:36.315966 pinjected-0.2.44/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.44/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.44/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.44/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.44/pinjected/with_context.py
--rw-r--r--   0        0        0      627 2024-04-24 10:51:37.617861 pinjected-0.2.44/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.44/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.45/LICENSE
+-rw-r--r--   0        0        0      457 2024-01-10 03:58:40.481212 pinjected-0.2.45/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.45/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.45/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.45/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.45/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.45/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.45/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.45/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.45/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.45/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.45/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.45/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14786 2024-04-24 11:20:36.713957 pinjected-0.2.45/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.45/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.45/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.45/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.45/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.45/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54209 2024-04-16 06:03:24.715277 pinjected-0.2.45/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.45/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.45/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.45/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.45/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.45/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.45/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.45/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.45/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.45/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.45/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.45/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.45/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.45/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.45/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.45/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.45/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.45/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.45/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.45/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.45/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15106 2024-03-26 02:52:38.846281 pinjected-0.2.45/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.45/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.45/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.45/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31540 2024-04-16 12:32:23.061374 pinjected-0.2.45/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.45/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.45/pinjected/global_configs.py
+-rw-r--r--   0        0        0     2927 2024-03-26 02:52:38.847411 pinjected-0.2.45/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.45/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.45/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.45/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.45/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.45/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.45/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.45/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.45/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.45/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.45/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.45/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.45/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.45/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.45/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.45/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.45/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.45/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.45/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.45/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.45/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.45/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.45/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.45/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.45/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9546 2024-04-23 08:38:19.299938 pinjected-0.2.45/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.45/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.45/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.45/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.45/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.45/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.45/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.45/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7086 2024-04-24 11:25:34.881010 pinjected-0.2.45/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.45/pinjected/v2/di.py
+-rw-r--r--   0        0        0      358 2024-03-26 02:52:38.851474 pinjected-0.2.45/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      507 2024-04-24 11:15:46.603608 pinjected-0.2.45/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0     9332 2024-04-24 11:45:09.926974 pinjected-0.2.45/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.45/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.45/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.45/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.45/pinjected/with_context.py
+-rw-r--r--   0        0        0      656 2024-04-24 11:45:30.023899 pinjected-0.2.45/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.45/PKG-INFO
```

### Comparing `pinjected-0.2.44/LICENSE` & `pinjected-0.2.45/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/decoration.py` & `pinjected-0.2.45/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/demo.py` & `pinjected-0.2.45/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/app_designed.py` & `pinjected-0.2.45/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/app_injected.py` & `pinjected-0.2.45/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/applicative.py` & `pinjected-0.2.45/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/ast.py` & `pinjected-0.2.45/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/decorators.py` & `pinjected-0.2.45/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/design.py` & `pinjected-0.2.45/pinjected/di/design.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from pathlib import Path
 from pprint import pformat
 from typing import TypeVar, List, Dict, Union, Callable, Type, Self
 
 from cytoolz import merge
 from makefun import create_function
 
+from pinjected.di.app_injected import EvaledInjected
 from pinjected.di.graph import DependencyResolver
 from pinjected.di.implicit_globals import IMPLICIT_BINDINGS
 from pinjected.di.injected import Injected
 from pinjected.di.injected import extract_dependency_including_self, InjectedPure, InjectedFunction
 # from pinjected.di.util import get_class_aware_args, get_dict_diff, check_picklable
 from pinjected.di.proxiable import DelegatedVar
 from pinjected.module_var_path import ModuleVarPath
-from pinjected.v2.binds import IBind, BindInjected
+from pinjected.v2.binds import IBind, BindInjected, ExprBind
 from pinjected.v2.keys import IBindKey, StrBindKey
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 def map_wrap(src, f):
@@ -179,18 +180,20 @@
         for k, v in kwargs.items():
             # logger.info(f"binding provider:{k}=>{v}")
             from loguru import logger
             match v:
                 case type():
                     # logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
                     bindings[StrBindKey(k)] = BindInjected(Injected.bind(v))
+                case EvaledInjected():
+                    bindings[StrBindKey(k)] = ExprBind(v)
+                case DelegatedVar():
+                    bindings[StrBindKey(k)] = ExprBind(v.eval())
                 case Injected():
                     bindings[StrBindKey(k)] = BindInjected(v)
-                case DelegatedVar():
-                    bindings[StrBindKey(k)] = BindInjected(v.eval())
                 case non_func if not callable(non_func):
                     logger.warning(
                         f"{k}->{v}: non-callable or non-injected is passed to bind_provider. fixing automatically.")
                     bindings[StrBindKey(k)] = BindInjected(Injected.pure(v))
                 case func if callable(func):
                     bindings[StrBindKey(k)] = BindInjected(Injected.bind(func))
                 case _:
@@ -365,16 +368,16 @@
         cxt = self.stack.pop()
         acc_d = sum([cxt.src for cxt in self.stack], start=Design()) + cxt.src
         target_vars = cxt.exit(frame)
         for mvp in target_vars:
             if mvp not in self.bindings:
                 self.bindings[mvp] = acc_d
 
-    def get_overrides(self,tgt:ModuleVarPath):
-        return self.bindings.get(tgt,Design())
+    def get_overrides(self, tgt: ModuleVarPath):
+        return self.bindings.get(tgt, Design())
 
 
 DESIGN_OVERRIDES_STORE = DesignOverridesStore()
 
 
 @dataclass
 class DesignOverrideContext:
@@ -382,36 +385,36 @@
     init_frame: inspect.FrameInfo
 
     def __post_init__(self):
         # get parent global variables
         parent_globals = self.init_frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
         from loguru import logger
-        #logger.debug(f"enter->\n"+pformat(global_ids))
+        # logger.debug(f"enter->\n"+pformat(global_ids))
         self.last_global_ids = global_ids
 
-    def exit(self, frame:inspect.FrameInfo) -> list[ModuleVarPath]:
+    def exit(self, frame: inspect.FrameInfo) -> list[ModuleVarPath]:
         from loguru import logger
         # get parent global variables
         parent_globals = frame.f_globals
         global_ids = {k: id(v) for k, v in parent_globals.items()}
         from loguru import logger
-        #logger.debug("exit->\n"+pformat(global_ids))
+        # logger.debug("exit->\n"+pformat(global_ids))
         changed_keys = []
         for k in global_ids:
             if k in self.last_global_ids:
                 if global_ids[k] != self.last_global_ids[k]:
                     changed_keys.append(k)
             else:
                 changed_keys.append(k)
-        #logger.debug(f"global_ids:{global_ids}")
+        # logger.debug(f"global_ids:{global_ids}")
         # find instance of DelegatedVar and Injected in the changed globals
         target_vars = dict()
         for k in changed_keys:
             v = parent_globals[k]
             if isinstance(v, DelegatedVar):
                 target_vars[k] = v
             if isinstance(v, Injected):
                 target_vars[k] = v
         mod_name = inspect.getmodule(frame).__name__
-        #logger.info(f"found targets:\n{pformat(target_vars)}")
-        return [ModuleVarPath(mod_name+"."+v) for v in target_vars.keys()]
+        # logger.info(f"found targets:\n{pformat(target_vars)}")
+        return [ModuleVarPath(mod_name + "." + v) for v in target_vars.keys()]
```

### Comparing `pinjected-0.2.44/pinjected/di/designed.py` & `pinjected-0.2.45/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.45/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/graph.py` & `pinjected-0.2.45/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/injected.py` & `pinjected-0.2.45/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/injected_analysis.py` & `pinjected-0.2.45/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/modular_injected.py` & `pinjected-0.2.45/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/overload_experimental.py` & `pinjected-0.2.45/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/proxiable.py` & `pinjected-0.2.45/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/session.py` & `pinjected-0.2.45/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/sessioned.py` & `pinjected-0.2.45/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/static_proxy.py` & `pinjected-0.2.45/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.45/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/test_graph.py` & `pinjected-0.2.45/pinjected/di/test_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def test_provide_session():
     d = Design().bind_instance(
         a=0
     )
     g = d.to_graph()
-    assert g["session"] == g
+    assert g["__resolver__"] == g.resolver
 
 
 def test_child_session():
     d = Design().bind_instance(
         a=0
     ).bind_provider(
         x=lambda a: a
```

### Comparing `pinjected-0.2.44/pinjected/di/test_injected.py` & `pinjected-0.2.45/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/tools/add_overload.py` & `pinjected-0.2.45/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/di/util.py` & `pinjected-0.2.45/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/exceptions.py` & `pinjected-0.2.45/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.45/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.45/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/graph_inspection.py` & `pinjected-0.2.45/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/helper_structure.py` & `pinjected-0.2.45/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/helpers.py` & `pinjected-0.2.45/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.45/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.45/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/ide_supports/default_design.py` & `pinjected-0.2.45/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.45/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.45/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/main_impl.py` & `pinjected-0.2.45/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/maybe_patch.py` & `pinjected-0.2.45/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/module_helper.py` & `pinjected-0.2.45/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/module_inspector.py` & `pinjected-0.2.45/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/module_var_path.py` & `pinjected-0.2.45/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/notification.py` & `pinjected-0.2.45/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/nx_graph_util.py` & `pinjected-0.2.45/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/run_config_utils.py` & `pinjected-0.2.45/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/run_config_utils_v2.py` & `pinjected-0.2.45/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/run_helpers/config.py` & `pinjected-0.2.45/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.45/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/runnables.py` & `pinjected-0.2.45/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/test_package/__init__.py` & `pinjected-0.2.45/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/test_package/child/module1.py` & `pinjected-0.2.45/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/v2/ainjected.py` & `pinjected-0.2.45/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/v2/binds.py` & `pinjected-0.2.45/pinjected/v2/binds.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 import asyncio
 import inspect
 from abc import ABC
 from dataclasses import dataclass, field, replace
 from typing import Generic, Dict, Any, Callable, Awaitable, TypeVar
 
 from pinjected import Injected
+from pinjected.di.app_injected import EvaledInjected
+from pinjected.di.ast import Expr
 from pinjected.di.metadata.bind_metadata import BindMetadata
 from pinjected.v2.keys import IBindKey, StrBindKey
 from pinjected.v2.provide_context import ProvideContext
 from returns.maybe import Maybe, Nothing, Some
 
 T = TypeVar('T')
 U = TypeVar('U')
 
+
 class IBind(Generic[T], ABC):
     """
     hold a provider and metadata
     """
+
     @abc.abstractmethod
     async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
         pass
 
     @property
     @abc.abstractmethod
     def dependencies(self) -> set[IBindKey]:
@@ -76,19 +80,18 @@
 
     @property
     @abc.abstractmethod
     def metadata(self) -> Maybe[BindMetadata]:
         raise NotImplementedError("metadata must be implemented")
 
     @abc.abstractmethod
-    def update_metadata(self, metadata: BindMetadata)->"IBind":
+    def update_metadata(self, metadata: BindMetadata) -> "IBind":
         raise NotImplementedError("update_metadata must be implemented")
 
 
-
 @dataclass
 class JustBind(IBind[T]):
     impl: Callable[[ProvideContext, Dict[IBindKey, Any]], Awaitable[T]]
     deps: set[IBindKey]
 
     async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
         return await self.impl(cxt, deps)
@@ -144,33 +147,33 @@
     def bind(cls, func: Callable[..., T]) -> 'StrBind[T]':
         if inspect.iscoroutinefunction(func):
             return cls.async_bind(func)
         else:
             return cls.func_bind(func)
 
 
-
 @dataclass
 class BindInjected(IBind[T]):
-
     from pinjected import Injected
     src: Injected
     _metadata: Maybe[BindMetadata] = field(default=Nothing)
+
     def __post_init__(self):
         assert isinstance(self.src, Injected), f"src must be an Injected, got {self.src}"
 
     async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
         from loguru import logger
         keys = {StrBindKey(d) for d in self.src.dependencies()}
         dep_dict = {d.name: deps[d] for d in keys}
         func = self.src.get_provider()
         logger.trace(f"provider:{func}")
-        assert inspect.iscoroutinefunction(func), f"provider of an Injected({self.src}) must be a coroutine function, got {func}"
+        assert inspect.iscoroutinefunction(
+            func), f"provider of an Injected({self.src}) must be a coroutine function, got {func}"
         data = await func(**dep_dict)
-        #assert not inspect.isawaitable(data), f"provider of an Injected({self.src}) must return a non-awaitable, got {data}"
+        # assert not inspect.isawaitable(data), f"provider of an Injected({self.src}) must return a non-awaitable, got {data}"
         return data
 
     @property
     def dependencies(self) -> set[IBindKey]:
         return {StrBindKey(d) for d in self.src.dependencies()}
 
     @property
@@ -182,14 +185,41 @@
         return self._metadata
 
     def update_metadata(self, metadata: BindMetadata) -> "IBind":
         return replace(self, _metadata=Some(metadata))
 
 
 @dataclass
+class ExprBind(IBind):
+    src: EvaledInjected
+    _metadata: Maybe[BindMetadata] = field(default=Nothing)
+
+    @property
+    def dependencies(self) -> set[IBindKey]:
+        return {StrBindKey(d) for d in self.src.dependencies()}
+
+    @property
+    def dynamic_dependencies(self) -> set[IBindKey]:
+        return {StrBindKey(d) for d in self.src.dynamic_dependencies()}
+
+    @property
+    def metadata(self) -> Maybe[BindMetadata]:
+        return self._metadata
+
+    def update_metadata(self, metadata: BindMetadata) -> "IBind":
+        return replace(self, _metadata=Some(metadata))
+
+    def __post_init__(self):
+        assert isinstance(self.src, EvaledInjected), f"src must be an Expr, got {self.src}"
+
+    async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
+        return await cxt.resolver.provide(self.src)
+
+
+@dataclass
 class MappedBind(IBind[U]):
     src: IBind[T]
     async_f: Callable[[T], Awaitable[U]]
 
     async def provide(self, cxt: ProvideContext, deps: Dict[IBindKey, Any]) -> T:
         data = self.src.provide(cxt, deps)
         return await self.async_f(data)
```

### Comparing `pinjected-0.2.44/pinjected/v2/di.py` & `pinjected-0.2.45/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pinjected/v2/resolver.py` & `pinjected-0.2.45/pinjected/v2/resolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     def __getstate__(self):
         return self.src
 
     def __setstate__(self, state):
         self.src = state
 
     def __hash__(self):
-        return hash(self.src)
+        return hash(f"cached") + hash(self.src)
 
 
 @dataclass
 class AsyncResolver:
     design: "Design"
     parent: Optional["AsyncResolver"] = None
     objects: Dict[IBindKey, Any] = field(default_factory=dict)
@@ -115,69 +115,55 @@
         self.eval_memos = {}
         self.eval_locks = defaultdict(asyncio.Lock)
 
     async def _optimize(self, expr: Expr):
         """
         this finds duplicated expr in the node and replace it with Cache Node.
         """
-        expr_table = defaultdict(list)
-        logger.debug(f'optimizing:{expr}')
+        return walk_replace(expr, lambda x: Cache(x))
 
-        def update_table(expr):
-            expr_table[hash(expr)] += [expr]
-            return expr
-
-        walk_replace(expr, update_table)
-        for k, v in expr_table.items():
-            # logger.info(f"expr {k} has {len(v)} duplicates ->: {v[0]}")
-            cache = Cache(src=v[0])
-            if len(v) > 1:
-                expr = walk_replace(expr, lambda x: cache if hash(x) == k else x)
-        logger.debug(f"optimized expr:{expr}")
-        return expr
-
-    async def _eval(self, expr: Expr):
+    async def eval_expr(self, expr: Expr):
         assert isinstance(expr, Expr), f"expr must be Expr, got {expr} of type {type(expr)}"
         match expr:
             case Cache(src):
                 k = hash(src)
                 async with self.eval_locks[k]:
                     if k in self.eval_memos:
                         res = self.eval_memos[k]
                     else:
-                        res = await self._eval(src)
+                        res = await self.eval_expr(src)
                         self.eval_memos[k] = res
 
             case Object(DelegatedVar(value, cxt)):
-                res = await self._eval(value)
+                res = await self.eval_expr(value)
             case Object(Injected() as _injected):
                 res = await self._provide_providable(_injected)
             case Object(x):
                 res = x
             case Call(f, args, kwargs):
-                args = asyncio.gather(*[self._eval(a) for a in args])
+                args = asyncio.gather(*[self.eval_expr(a) for a in args])
                 keys = list(kwargs.keys())
-                values = asyncio.gather(*[self._eval(v) for v in kwargs.values()])
-                f, args, values = await asyncio.gather(self._eval(f), args, values)
+                values = asyncio.gather(*[self.eval_expr(v) for v in kwargs.values()])
+                f, args, values = await asyncio.gather(self.eval_expr(f), args, values)
                 kwargs = dict(zip(keys, values))
                 res = f(*args, **kwargs)
             case BiOp(op, left, right):
-                left, right = await asyncio.gather(self._eval(left), self._eval(right))
+                left, right = await asyncio.gather(self.eval_expr(left), self.eval_expr(right))
                 res = OPERATORS[op](left, right)
             case UnaryOp('await', data):
-                data = await self._eval(data)
+                data = await self.eval_expr(data)
                 res = await data
             case UnaryOp(name, data):
-                data = await self._eval(data)
+                data = await self.eval_expr(data)
                 res = UNARY_OPS[name](data)
             case Attr(data, name):
-                data = await self._eval(data)
+                data = await self.eval_expr(data)
                 res = getattr(data, name)
             case GetItem(data, key):
-                data, key = await asyncio.gather(self._eval(data), self._eval(key))
+                data, key = await asyncio.gather(self.eval_expr(data), self.eval_expr(key))
                 res = data[key]
             case _:
                 raise TypeError(
                     f"expr must be Object, Call, BiOp, UnaryOp, Attr or GetItem, got {expr} of type {type(expr)}")
         return res
 
     async def _provide(self, key: IBindKey, cxt: ProvideContext):
@@ -190,15 +176,15 @@
             elif key in self.design:
                 logger.info(f"{cxt.trace_str}")
                 # we are responsible for providing this
                 bind = self.design.bindings[key]
                 dep_keys = list(bind.dependencies)
                 tasks = []
                 for dep_key in dep_keys:
-                    n_cxt = ProvideContext(key=dep_key, parent=cxt)
+                    n_cxt = ProvideContext(self, key=dep_key, parent=cxt)
                     tasks.append(self._provide(dep_key, n_cxt))
                 res = await asyncio.gather(*tasks)
                 deps = dict(zip(dep_keys, res))
                 data = await bind.provide(cxt, deps)
                 self.objects[key] = data
                 show_data = str(data)[:100]
                 logger.info(f"{cxt.trace_str} := {show_data}")
@@ -210,34 +196,34 @@
                     raise KeyError(f"Key {key} not found in design in {cxt.trace_str}")
 
     def child_session(self, overrides: "Design"):
         return AsyncResolver(overrides, parent=self)
 
     async def _provide_providable(self, tgt: Providable):
         async def resolve_deps(keys: set[IBindKey]):
-            tasks = [self._provide(k, ProvideContext(key=k, parent=None)) for k in keys]
+            tasks = [self._provide(k, ProvideContext(self, key=k, parent=None)) for k in keys]
             return {k: v for k, v in zip(keys, await asyncio.gather(*tasks))}
 
         match tgt:
             case str():
-                return await self._provide(StrBindKey(tgt), ProvideContext(key=StrBindKey(tgt), parent=None))
+                return await self._provide(StrBindKey(tgt), ProvideContext(self, key=StrBindKey(tgt), parent=None))
             case IBindKey():
-                return await self._provide(tgt, ProvideContext(key=tgt, parent=None))
+                return await self._provide(tgt, ProvideContext(self, key=tgt, parent=None))
             case DelegatedVar(value, cxt) as dv:
                 # return await self._provide_providable(tgt.eval())
                 expr = await self._optimize(dv.eval().ast)
-                return await self._eval(expr)
+                return await self.eval_expr(expr)
             case EvaledInjected(val, ast):
                 expr = await self._optimize(ast)
-                return await self._eval(expr)
+                return await self.eval_expr(expr)
             case Injected() as i_tgt:
                 return await self._provide_providable(BindInjected(i_tgt))
             case IBind():
                 deps = await resolve_deps(tgt.dependencies)
-                return await tgt.provide(ProvideContext(key=tgt, parent=None), deps)
+                return await tgt.provide(ProvideContext(self, key=tgt, parent=None), deps)
             case func if inspect.isfunction:
                 deps = extract_dependency(func)
                 logger.info(f"Resolving deps for {func} -> {deps}")
                 keys = {StrBindKey(d) for d in deps}
                 deps = await resolve_deps(keys)
                 kwargs = {k.name: v for k, v in deps.items()}
                 data = tgt(**kwargs)
```

### Comparing `pinjected-0.2.44/pinjected/visualize_di.py` & `pinjected-0.2.45/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.44/pyproject.toml` & `pinjected-0.2.45/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+[project]
+dependencies = []
+
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.44"
+version = "0.2.45"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.44/PKG-INFO` & `pinjected-0.2.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.44
+Version: 0.2.45
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

