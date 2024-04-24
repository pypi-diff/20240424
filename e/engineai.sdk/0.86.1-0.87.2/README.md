# Comparing `tmp/engineai_sdk-0.86.1.tar.gz` & `tmp/engineai_sdk-0.87.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engineai_sdk-0.86.1.tar", max compression
+gzip compressed data, was "engineai_sdk-0.87.2.tar", max compression
```

## Comparing `engineai_sdk-0.86.1.tar` & `engineai_sdk-0.87.2.tar`

### file list

```diff
@@ -1,366 +1,366 @@
--rw-r--r--   0        0        0     1065 2024-04-18 10:02:32.115517 engineai_sdk-0.86.1/LICENSE
--rw-r--r--   0        0        0      987 2024-04-18 10:02:32.115517 engineai_sdk-0.86.1/README.md
--rw-r--r--   0        0        0      435 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/__init__.py
--rw-r--r--   0        0        0       28 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/__init__.py
--rw-r--r--   0        0        0       33 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/__init__.py
--rw-r--r--   0        0        0     2541 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/app.py
--rw-r--r--   0        0        0    14251 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/commands/dashboard.py
--rw-r--r--   0        0        0     1379 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/console.py
--rw-r--r--   0        0        0     4806 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/generator.py
--rw-r--r--   0        0        0       43 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/.env.sample
--rw-r--r--   0        0        0     5396 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/data/example.json
--rw-r--r--   0        0        0      411 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/template/content/main.py
--rw-r--r--   0        0        0    10363 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/cli/utils.py
--rw-r--r--   0        0        0       38 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/__init__.py
--rw-r--r--   0        0        0      121 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/__init__.py
--rw-r--r--   0        0        0     2181 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/layout.py
--rw-r--r--   0        0        0      207 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/selectable_widgets.py
--rw-r--r--   0        0        0      570 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/typing.py
--rw-r--r--   0        0        0     1600 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/base.py
--rw-r--r--   0        0        0       96 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/__init__.py
--rw-r--r--   0        0        0     3574 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/activate_dashboard.py
--rw-r--r--   0        0        0     7670 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/api.py
--rw-r--r--   0        0        0     1451 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/exceptions.py
--rw-r--r--   0        0        0      217 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/__init__.py
--rw-r--r--   0        0        0      472 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/py.typed
--rw-r--r--   0        0        0      207 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
--rw-r--r--   0        0        0     6861 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
--rw-r--r--   0        0        0     3134 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/json.py
--rw-r--r--   0        0        0     4618 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/storage.py
--rw-r--r--   0        0        0      515 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/config.py
--rw-r--r--   0        0        0      310 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/__init__.py
--rw-r--r--   0        0        0    13364 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/dashboard.py
--rw-r--r--   0        0        0      140 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/enums.py
--rw-r--r--   0        0        0     4691 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/exceptions.py
--rw-r--r--   0        0        0       27 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/__init__.py
--rw-r--r--   0        0        0     2417 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py
--rw-r--r--   0        0        0     8389 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/instance.py
--rw-r--r--   0        0        0     1231 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/node.py
--rw-r--r--   0        0        0     2586 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/utils.py
--rw-r--r--   0        0        0       41 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/__init__.py
--rw-r--r--   0        0        0     1431 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/dependency.py
--rw-r--r--   0        0        0     5667 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/page.py
--rw-r--r--   0        0        0     1909 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/root.py
--rw-r--r--   0        0        0     2932 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/route.py
--rw-r--r--   0        0        0      345 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/typings.py
--rw-r--r--   0        0        0       33 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/__init__.py
--rw-r--r--   0        0        0     5105 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/version.py
--rw-r--r--   0        0        0      185 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/__init__.py
--rw-r--r--   0        0        0    12893 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/decorator.py
--rw-r--r--   0        0        0     1822 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/duplicated.py
--rw-r--r--   0        0        0     1047 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/enums.py
--rw-r--r--   0        0        0     4676 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/exceptions.py
--rw-r--r--   0        0        0     1996 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/http.py
--rw-r--r--   0        0        0     3616 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/io_handler.py
--rw-r--r--   0        0        0     1306 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/interface.py
--rw-r--r--   0        0        0     9994 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/manager.py
--rw-r--r--   0        0        0     2892 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/decorator.py
--rw-r--r--   0        0        0      441 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/__init__.py
--rw-r--r--   0        0        0     3521 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/datastore.py
--rw-r--r--   0        0        0      141 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/__init__.py
--rw-r--r--   0        0        0      966 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/header.py
--rw-r--r--   0        0        0     2555 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/http.py
--rw-r--r--   0        0        0     2026 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/route.py
--rw-r--r--   0        0        0     2518 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/widget.py
--rw-r--r--   0        0        0      369 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/__init__.py
--rw-r--r--   0        0        0     1112 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/align.py
--rw-r--r--   0        0        0      741 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/legend_position.py
--rw-r--r--   0        0        0     5156 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/exceptions.py
--rw-r--r--   0        0        0      569 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/__init__.py
--rw-r--r--   0        0        0     3817 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/axis.py
--rw-r--r--   0        0        0     1888 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/datetime.py
--rw-r--r--   0        0        0      661 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/exceptions.py
--rw-r--r--   0        0        0     1331 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/mapper.py
--rw-r--r--   0        0        0     5254 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/number.py
--rw-r--r--   0        0        0     1421 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/text.py
--rw-r--r--   0        0        0      331 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/typing.py
--rw-r--r--   0        0        0      985 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/validator.py
--rw-r--r--   0        0        0     1056 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/interface.py
--rw-r--r--   0        0        0      825 2024-04-18 10:02:32.119517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/__init__.py
--rw-r--r--   0        0        0      417 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/build_item.py
--rw-r--r--   0        0        0       28 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/__init__.py
--rw-r--r--   0        0        0     5990 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/card.py
--rw-r--r--   0        0        0     2889 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/chip.py
--rw-r--r--   0        0        0     1679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/header.py
--rw-r--r--   0        0        0       55 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/__init__.py
--rw-r--r--   0        0        0     3082 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/chip.py
--rw-r--r--   0        0        0     1968 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/header.py
--rw-r--r--   0        0        0     6641 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/section.py
--rw-r--r--   0        0        0     5999 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/column.py
--rw-r--r--   0        0        0     2679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/chip.py
--rw-r--r--   0        0        0     2165 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/header.py
--rw-r--r--   0        0        0     2385 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/label.py
--rw-r--r--   0        0        0     4695 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/__init__.py
--rw-r--r--   0        0        0     5791 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
--rw-r--r--   0        0        0     1921 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py
--rw-r--r--   0        0        0     7313 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/grid.py
--rw-r--r--   0        0        0    10423 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/row.py
--rw-r--r--   0        0        0       36 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/__init__.py
--rw-r--r--   0        0        0     7582 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/base.py
--rw-r--r--   0        0        0     2171 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/exceptions.py
--rw-r--r--   0        0        0     4397 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/tab.py
--rw-r--r--   0        0        0      676 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/typings.py
--rw-r--r--   0        0        0      244 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/__init__.py
--rw-r--r--   0        0        0     6016 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/abstract.py
--rw-r--r--   0        0        0     2201 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/route_link.py
--rw-r--r--   0        0        0     2576 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/template_string_link.py
--rw-r--r--   0        0        0      202 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/typing.py
--rw-r--r--   0        0        0     1427 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/url.py
--rw-r--r--   0        0        0      934 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_dependency.py
--rw-r--r--   0        0        0     3039 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_field.py
--rw-r--r--   0        0        0        0 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/py.typed
--rw-r--r--   0        0        0     2020 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/selected.py
--rw-r--r--   0        0        0      100 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/__init__.py
--rw-r--r--   0        0        0      744 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/__init__.py
--rw-r--r--   0        0        0     5872 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/default_specs.py
--rw-r--r--   0        0        0     6985 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/discrete_map.py
--rw-r--r--   0        0        0     1679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/divergent.py
--rw-r--r--   0        0        0     4055 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/gradient.py
--rw-r--r--   0        0        0     5949 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/palette.py
--rw-r--r--   0        0        0      920 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/single.py
--rw-r--r--   0        0        0      946 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/spec.py
--rw-r--r--   0        0        0      436 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/typing.py
--rw-r--r--   0        0        0     3436 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/icons.py
--rw-r--r--   0        0        0     8298 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/templated_string.py
--rw-r--r--   0        0        0     3514 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/utils.py
--rw-r--r--   0        0        0       25 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/__init__.py
--rw-r--r--   0        0        0     8541 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/base.py
--rw-r--r--   0        0        0     2647 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py
--rw-r--r--   0        0        0       44 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
--rw-r--r--   0        0        0     3566 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
--rw-r--r--   0        0        0      365 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
--rw-r--r--   0        0        0     2149 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
--rw-r--r--   0        0        0     5237 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
--rw-r--r--   0        0        0     4410 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
--rw-r--r--   0        0        0     4481 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/chart.py
--rw-r--r--   0        0        0     1468 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
--rw-r--r--   0        0        0      987 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/legend.py
--rw-r--r--   0        0        0       45 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
--rw-r--r--   0        0        0     2640 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py
--rw-r--r--   0        0        0     4026 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
--rw-r--r--   0        0        0     7256 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py
--rw-r--r--   0        0        0     5303 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
--rw-r--r--   0        0        0     2660 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py
--rw-r--r--   0        0        0     2640 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py
--rw-r--r--   0        0        0     2679 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
--rw-r--r--   0        0        0      573 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
--rw-r--r--   0        0        0     4957 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/chart_utils.py
--rw-r--r--   0        0        0       39 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/__init__.py
--rw-r--r--   0        0        0       87 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py
--rw-r--r--   0        0        0     1475 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
--rw-r--r--   0        0        0     1910 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
--rw-r--r--   0        0        0       47 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/__init__.py
--rw-r--r--   0        0        0       56 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
--rw-r--r--   0        0        0      416 2024-04-18 10:02:32.123517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
--rw-r--r--   0        0        0     1764 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
--rw-r--r--   0        0        0     1764 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
--rw-r--r--   0        0        0     1117 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
--rw-r--r--   0        0        0     2785 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
--rw-r--r--   0        0        0      338 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
--rw-r--r--   0        0        0      151 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/consts.py
--rw-r--r--   0        0        0     7162 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
--rw-r--r--   0        0        0     2787 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py
--rw-r--r--   0        0        0       23 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
--rw-r--r--   0        0        0      955 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
--rw-r--r--   0        0        0     2138 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
--rw-r--r--   0        0        0      806 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
--rw-r--r--   0        0        0      314 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
--rw-r--r--   0        0        0      696 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
--rw-r--r--   0        0        0     1491 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
--rw-r--r--   0        0        0     1573 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
--rw-r--r--   0        0        0     4041 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
--rw-r--r--   0        0        0     3527 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
--rw-r--r--   0        0        0     3132 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
--rw-r--r--   0        0        0     1484 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
--rw-r--r--   0        0        0     1047 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
--rw-r--r--   0        0        0     1540 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
--rw-r--r--   0        0        0     3635 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
--rw-r--r--   0        0        0     1473 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
--rw-r--r--   0        0        0     1514 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
--rw-r--r--   0        0        0      802 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
--rw-r--r--   0        0        0      282 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
--rw-r--r--   0        0        0      319 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
--rw-r--r--   0        0        0     3647 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
--rw-r--r--   0        0        0     1490 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
--rw-r--r--   0        0        0     1641 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
--rw-r--r--   0        0        0      617 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
--rw-r--r--   0        0        0     1102 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
--rw-r--r--   0        0        0     1526 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
--rw-r--r--   0        0        0     1594 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
--rw-r--r--   0        0        0      647 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/typing.py
--rw-r--r--   0        0        0       29 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/__init__.py
--rw-r--r--   0        0        0     1192 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py
--rw-r--r--   0        0        0       35 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
--rw-r--r--   0        0        0      228 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
--rw-r--r--   0        0        0      236 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
--rw-r--r--   0        0        0      228 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
--rw-r--r--   0        0        0     1184 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
--rw-r--r--   0        0        0      379 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
--rw-r--r--   0        0        0      974 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
--rw-r--r--   0        0        0       36 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
--rw-r--r--   0        0        0      902 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
--rw-r--r--   0        0        0      893 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
--rw-r--r--   0        0        0      906 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
--rw-r--r--   0        0        0     1263 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
--rw-r--r--   0        0        0      339 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
--rw-r--r--   0        0        0       34 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
--rw-r--r--   0        0        0      879 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
--rw-r--r--   0        0        0     1388 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
--rw-r--r--   0        0        0      943 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
--rw-r--r--   0        0        0      903 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
--rw-r--r--   0        0        0      331 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
--rw-r--r--   0        0        0     1313 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
--rw-r--r--   0        0        0     2014 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
--rw-r--r--   0        0        0     2003 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
--rw-r--r--   0        0        0      136 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/__init__.py
--rw-r--r--   0        0        0     2890 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/content.py
--rw-r--r--   0        0        0     1265 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/exceptions.py
--rw-r--r--   0        0        0      613 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/item.py
--rw-r--r--   0        0        0     1431 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/markdown.py
--rw-r--r--   0        0        0     3756 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/exceptions.py
--rw-r--r--   0        0        0      573 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/__init__.py
--rw-r--r--   0        0        0     1369 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/color_axis.py
--rw-r--r--   0        0        0     1043 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/enums.py
--rw-r--r--   0        0        0      980 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/exceptions.py
--rw-r--r--   0        0        0       25 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
--rw-r--r--   0        0        0     8048 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/base.py
--rw-r--r--   0        0        0     4272 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py
--rw-r--r--   0        0        0       29 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/__init__.py
--rw-r--r--   0        0        0      832 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py
--rw-r--r--   0        0        0      988 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py
--rw-r--r--   0        0        0      954 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/legend.py
--rw-r--r--   0        0        0       42 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/__init__.py
--rw-r--r--   0        0        0     4887 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py
--rw-r--r--   0        0        0      625 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/series.py
--rw-r--r--   0        0        0     2937 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/styling.py
--rw-r--r--   0        0        0     2113 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pandas_utils.py
--rw-r--r--   0        0        0      672 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/__init__.py
--rw-r--r--   0        0        0     1949 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/chart.py
--rw-r--r--   0        0        0      852 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/exceptions.py
--rw-r--r--   0        0        0      851 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/legend.py
--rw-r--r--   0        0        0     6296 2024-04-18 10:02:32.127517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/pie.py
--rw-r--r--   0        0        0       35 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/__init__.py
--rw-r--r--   0        0        0     6044 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/base.py
--rw-r--r--   0        0        0     3413 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/country.py
--rw-r--r--   0        0        0     3059 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/series.py
--rw-r--r--   0        0        0     3185 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/styling.py
--rw-r--r--   0        0        0      165 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/typings.py
--rw-r--r--   0        0        0     2402 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/tooltip.py
--rw-r--r--   0        0        0      391 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/__init__.py
--rw-r--r--   0        0        0     3415 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/base.py
--rw-r--r--   0        0        0      900 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/build_result.py
--rw-r--r--   0        0        0     3470 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/number.py
--rw-r--r--   0        0        0       21 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
--rw-r--r--   0        0        0     3252 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
--rw-r--r--   0        0        0     1523 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py
--rw-r--r--   0        0        0     1712 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py
--rw-r--r--   0        0        0     2432 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/text.py
--rw-r--r--   0        0        0      280 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/typing.py
--rw-r--r--   0        0        0     8158 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/search.py
--rw-r--r--   0        0        0       79 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/exceptions.py
--rw-r--r--   0        0        0     1783 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/group.py
--rw-r--r--   0        0        0     6575 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/select.py
--rw-r--r--   0        0        0     2453 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/__init__.py
--rw-r--r--   0        0        0       50 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/__init__.py
--rw-r--r--   0        0        0       26 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
--rw-r--r--   0        0        0     6147 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py
--rw-r--r--   0        0        0     6201 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py
--rw-r--r--   0        0        0       46 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
--rw-r--r--   0        0        0     5611 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
--rw-r--r--   0        0        0     6726 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
--rw-r--r--   0        0        0     5672 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
--rw-r--r--   0        0        0     5669 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
--rw-r--r--   0        0        0     5330 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
--rw-r--r--   0        0        0     5103 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py
--rw-r--r--   0        0        0     5869 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
--rw-r--r--   0        0        0     4011 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
--rw-r--r--   0        0        0     6105 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py
--rw-r--r--   0        0        0     5601 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py
--rw-r--r--   0        0        0     5419 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py
--rw-r--r--   0        0        0     3727 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
--rw-r--r--   0        0        0       49 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
--rw-r--r--   0        0        0     1146 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
--rw-r--r--   0        0        0     1659 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
--rw-r--r--   0        0        0     5055 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
--rw-r--r--   0        0        0     1541 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
--rw-r--r--   0        0        0     2510 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
--rw-r--r--   0        0        0     1161 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
--rw-r--r--   0        0        0     1321 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
--rw-r--r--   0        0        0     1271 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
--rw-r--r--   0        0        0     1537 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
--rw-r--r--   0        0        0     1418 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
--rw-r--r--   0        0        0     1233 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
--rw-r--r--   0        0        0     1147 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
--rw-r--r--   0        0        0     1494 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
--rw-r--r--   0        0        0     2723 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
--rw-r--r--   0        0        0     1727 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
--rw-r--r--   0        0        0     1779 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
--rw-r--r--   0        0        0      473 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/enums.py
--rw-r--r--   0        0        0     5447 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/exceptions.py
--rw-r--r--   0        0        0     1864 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/group.py
--rw-r--r--   0        0        0     9162 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/header.py
--rw-r--r--   0        0        0     2713 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/initial_state.py
--rw-r--r--   0        0        0     2046 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/styling.py
--rw-r--r--   0        0        0    17305 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/table.py
--rw-r--r--   0        0        0     3155 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py
--rw-r--r--   0        0        0       45 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
--rw-r--r--   0        0        0     1722 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
--rw-r--r--   0        0        0      381 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
--rw-r--r--   0        0        0       35 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
--rw-r--r--   0        0        0     4983 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
--rw-r--r--   0        0        0      902 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
--rw-r--r--   0        0        0     3279 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
--rw-r--r--   0        0        0     4413 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
--rw-r--r--   0        0        0     9066 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/chart.py
--rw-r--r--   0        0        0      513 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/consts.py
--rw-r--r--   0        0        0     1562 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/enums.py
--rw-r--r--   0        0        0    12101 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
--rw-r--r--   0        0        0     1126 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/legend.py
--rw-r--r--   0        0        0     3322 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py
--rw-r--r--   0        0        0       56 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
--rw-r--r--   0        0        0     1051 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
--rw-r--r--   0        0        0     5436 2024-04-18 10:02:32.131517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
--rw-r--r--   0        0        0     1339 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
--rw-r--r--   0        0        0       46 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
--rw-r--r--   0        0        0     3472 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py
--rw-r--r--   0        0        0     4698 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
--rw-r--r--   0        0        0     7615 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py
--rw-r--r--   0        0        0     6061 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
--rw-r--r--   0        0        0     3621 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py
--rw-r--r--   0        0        0     4728 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
--rw-r--r--   0        0        0     3637 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py
--rw-r--r--   0        0        0     3623 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py
--rw-r--r--   0        0        0     3654 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
--rw-r--r--   0        0        0      618 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
--rw-r--r--   0        0        0    23062 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
--rw-r--r--   0        0        0     2038 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/transform.py
--rw-r--r--   0        0        0       87 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/__init__.py
--rw-r--r--   0        0        0      543 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py
--rw-r--r--   0        0        0     5107 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/toggle.py
--rw-r--r--   0        0        0     2755 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/utils.py
--rw-r--r--   0        0        0       33 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/authentication/auth0.py
--rw-r--r--   0        0        0     5852 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/authentication/utils.py
--rw-r--r--   0        0        0       92 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/__init__.py
--rw-r--r--   0        0        0     5003 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/api.py
--rw-r--r--   0        0        0     1195 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/clients/exceptions.py
--rw-r--r--   0        0        0      482 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/exceptions.py
--rw-r--r--   0        0        0      432 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/__init__.py
--rw-r--r--   0        0        0      348 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/py.typed
--rw-r--r--   0        0        0     3169 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/schema.py
--rw-r--r--   0        0        0     6996 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/types.py
--rw-r--r--   0        0        0      319 2024-04-18 10:02:32.135517 engineai_sdk-0.86.1/engineai/sdk/internal/url_config.py
--rw-r--r--   0        0        0     1841 2024-04-18 10:02:47.779638 engineai_sdk-0.86.1/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 engineai_sdk-0.86.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/LICENSE
+-rw-r--r--   0        0        0      987 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/README.md
+-rw-r--r--   0        0        0      435 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/app.py
+-rw-r--r--   0        0        0    14251 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/commands/dashboard.py
+-rw-r--r--   0        0        0     1379 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/console.py
+-rw-r--r--   0        0        0     4806 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/generator.py
+-rw-r--r--   0        0        0       43 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/.env.sample
+-rw-r--r--   0        0        0     5396 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/data/example.json
+-rw-r--r--   0        0        0      411 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/template/content/main.py
+-rw-r--r--   0        0        0    10363 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/cli/utils.py
+-rw-r--r--   0        0        0       38 2024-04-24 14:07:11.083692 engineai_sdk-0.87.2/engineai/sdk/dashboard/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/__init__.py
+-rw-r--r--   0        0        0     2181 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/layout.py
+-rw-r--r--   0        0        0      207 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/selectable_widgets.py
+-rw-r--r--   0        0        0      570 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/typing.py
+-rw-r--r--   0        0        0     1600 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/base.py
+-rw-r--r--   0        0        0       96 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/__init__.py
+-rw-r--r--   0        0        0     3574 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/activate_dashboard.py
+-rw-r--r--   0        0        0     7670 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/api.py
+-rw-r--r--   0        0        0     1451 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/exceptions.py
+-rw-r--r--   0        0        0      217 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/py.typed
+-rw-r--r--   0        0        0      207 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/__init__.py
+-rw-r--r--   0        0        0     6861 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py
+-rw-r--r--   0        0        0     3134 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/json.py
+-rw-r--r--   0        0        0     4618 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/storage.py
+-rw-r--r--   0        0        0      515 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/config.py
+-rw-r--r--   0        0        0      310 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/__init__.py
+-rw-r--r--   0        0        0    13364 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/dashboard.py
+-rw-r--r--   0        0        0      140 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/enums.py
+-rw-r--r--   0        0        0     4691 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/exceptions.py
+-rw-r--r--   0        0        0       27 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/__init__.py
+-rw-r--r--   0        0        0     2417 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/executor_config.py
+-rw-r--r--   0        0        0     8389 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/instance.py
+-rw-r--r--   0        0        0     1231 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/node.py
+-rw-r--r--   0        0        0     2586 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/utils.py
+-rw-r--r--   0        0        0       41 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/__init__.py
+-rw-r--r--   0        0        0     1431 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/dependency.py
+-rw-r--r--   0        0        0     5667 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/page.py
+-rw-r--r--   0        0        0     1909 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/root.py
+-rw-r--r--   0        0        0     2932 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/route.py
+-rw-r--r--   0        0        0      345 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/typings.py
+-rw-r--r--   0        0        0       33 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/__init__.py
+-rw-r--r--   0        0        0     5105 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/version.py
+-rw-r--r--   0        0        0      185 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/__init__.py
+-rw-r--r--   0        0        0    12893 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/decorator.py
+-rw-r--r--   0        0        0     1822 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/duplicated.py
+-rw-r--r--   0        0        0     1047 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/enums.py
+-rw-r--r--   0        0        0     4676 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/exceptions.py
+-rw-r--r--   0        0        0     1996 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/http.py
+-rw-r--r--   0        0        0     3616 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/io_handler.py
+-rw-r--r--   0        0        0     1306 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/interface.py
+-rw-r--r--   0        0        0     9994 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/manager.py
+-rw-r--r--   0        0        0     2892 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/decorator.py
+-rw-r--r--   0        0        0      441 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/__init__.py
+-rw-r--r--   0        0        0     3521 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/datastore.py
+-rw-r--r--   0        0        0      141 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/__init__.py
+-rw-r--r--   0        0        0      966 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/header.py
+-rw-r--r--   0        0        0     2555 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/http.py
+-rw-r--r--   0        0        0     2026 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/route.py
+-rw-r--r--   0        0        0     2518 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/widget.py
+-rw-r--r--   0        0        0      369 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/__init__.py
+-rw-r--r--   0        0        0     1112 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/align.py
+-rw-r--r--   0        0        0      741 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/legend_position.py
+-rw-r--r--   0        0        0     5156 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/exceptions.py
+-rw-r--r--   0        0        0      569 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/axis.py
+-rw-r--r--   0        0        0     1888 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/datetime.py
+-rw-r--r--   0        0        0      661 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/exceptions.py
+-rw-r--r--   0        0        0     1331 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/mapper.py
+-rw-r--r--   0        0        0     5254 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/number.py
+-rw-r--r--   0        0        0     1421 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/text.py
+-rw-r--r--   0        0        0      331 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/typing.py
+-rw-r--r--   0        0        0      985 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/validator.py
+-rw-r--r--   0        0        0     1056 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/interface.py
+-rw-r--r--   0        0        0      825 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/build_item.py
+-rw-r--r--   0        0        0       28 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/__init__.py
+-rw-r--r--   0        0        0     5990 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/card.py
+-rw-r--r--   0        0        0     2889 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/chip.py
+-rw-r--r--   0        0        0     1679 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/header.py
+-rw-r--r--   0        0        0       55 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/__init__.py
+-rw-r--r--   0        0        0     3082 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/chip.py
+-rw-r--r--   0        0        0     1968 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/header.py
+-rw-r--r--   0        0        0     6641 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/section.py
+-rw-r--r--   0        0        0     5999 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/column.py
+-rw-r--r--   0        0        0     2679 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/chip.py
+-rw-r--r--   0        0        0     2165 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/header.py
+-rw-r--r--   0        0        0     2385 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/label.py
+-rw-r--r--   0        0        0     4695 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-24 14:07:11.087693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/__init__.py
+-rw-r--r--   0        0        0     5791 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py
+-rw-r--r--   0        0        0     1921 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/items_build.py
+-rw-r--r--   0        0        0     7313 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/grid.py
+-rw-r--r--   0        0        0    10423 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/row.py
+-rw-r--r--   0        0        0       36 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/__init__.py
+-rw-r--r--   0        0        0     7582 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/base.py
+-rw-r--r--   0        0        0     2171 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/exceptions.py
+-rw-r--r--   0        0        0     4397 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/tab.py
+-rw-r--r--   0        0        0      676 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/typings.py
+-rw-r--r--   0        0        0      244 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/__init__.py
+-rw-r--r--   0        0        0     6016 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/abstract.py
+-rw-r--r--   0        0        0     2201 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/route_link.py
+-rw-r--r--   0        0        0     2576 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/template_string_link.py
+-rw-r--r--   0        0        0      202 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/typing.py
+-rw-r--r--   0        0        0     1427 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/url.py
+-rw-r--r--   0        0        0      934 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_dependency.py
+-rw-r--r--   0        0        0     3039 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_field.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/py.typed
+-rw-r--r--   0        0        0     2020 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/selected.py
+-rw-r--r--   0        0        0      100 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/__init__.py
+-rw-r--r--   0        0        0     5872 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/default_specs.py
+-rw-r--r--   0        0        0     6985 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/discrete_map.py
+-rw-r--r--   0        0        0     1679 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/divergent.py
+-rw-r--r--   0        0        0     4055 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/gradient.py
+-rw-r--r--   0        0        0     5949 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/palette.py
+-rw-r--r--   0        0        0      920 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/single.py
+-rw-r--r--   0        0        0      946 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/spec.py
+-rw-r--r--   0        0        0      436 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/typing.py
+-rw-r--r--   0        0        0     3436 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/icons.py
+-rw-r--r--   0        0        0     8298 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/templated_string.py
+-rw-r--r--   0        0        0     3514 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/utils.py
+-rw-r--r--   0        0        0       25 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/__init__.py
+-rw-r--r--   0        0        0     8541 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/base.py
+-rw-r--r--   0        0        0     2647 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/__init__.py
+-rw-r--r--   0        0        0     3566 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py
+-rw-r--r--   0        0        0      365 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/typing.py
+-rw-r--r--   0        0        0     2149 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py
+-rw-r--r--   0        0        0     5237 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py
+-rw-r--r--   0        0        0     4410 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py
+-rw-r--r--   0        0        0     4481 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/chart.py
+-rw-r--r--   0        0        0     1468 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py
+-rw-r--r--   0        0        0      987 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/legend.py
+-rw-r--r--   0        0        0       45 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py
+-rw-r--r--   0        0        0     4026 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py
+-rw-r--r--   0        0        0     7256 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py
+-rw-r--r--   0        0        0     5303 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py
+-rw-r--r--   0        0        0     2660 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py
+-rw-r--r--   0        0        0     2640 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py
+-rw-r--r--   0        0        0     2679 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py
+-rw-r--r--   0        0        0      573 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py
+-rw-r--r--   0        0        0     4957 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/chart_utils.py
+-rw-r--r--   0        0        0       39 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py
+-rw-r--r--   0        0        0     1475 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py
+-rw-r--r--   0        0        0     1910 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py
+-rw-r--r--   0        0        0       47 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/__init__.py
+-rw-r--r--   0        0        0      416 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py
+-rw-r--r--   0        0        0     1764 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py
+-rw-r--r--   0        0        0     1764 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py
+-rw-r--r--   0        0        0     1117 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py
+-rw-r--r--   0        0        0     2785 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py
+-rw-r--r--   0        0        0      338 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/typing.py
+-rw-r--r--   0        0        0      151 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/consts.py
+-rw-r--r--   0        0        0     7162 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/__init__.py
+-rw-r--r--   0        0        0     2787 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py
+-rw-r--r--   0        0        0       23 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/__init__.py
+-rw-r--r--   0        0        0      955 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py
+-rw-r--r--   0        0        0     2138 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py
+-rw-r--r--   0        0        0      806 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py
+-rw-r--r--   0        0        0      314 2024-04-24 14:07:11.091693 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/typing.py
+-rw-r--r--   0        0        0      696 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py
+-rw-r--r--   0        0        0     1491 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py
+-rw-r--r--   0        0        0     1573 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py
+-rw-r--r--   0        0        0     4041 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py
+-rw-r--r--   0        0        0     3527 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py
+-rw-r--r--   0        0        0     3132 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py
+-rw-r--r--   0        0        0     1484 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py
+-rw-r--r--   0        0        0     1047 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py
+-rw-r--r--   0        0        0     1540 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py
+-rw-r--r--   0        0        0     3635 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py
+-rw-r--r--   0        0        0     1473 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py
+-rw-r--r--   0        0        0     1514 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py
+-rw-r--r--   0        0        0      802 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py
+-rw-r--r--   0        0        0      282 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/toolbar.py
+-rw-r--r--   0        0        0      319 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/__init__.py
+-rw-r--r--   0        0        0     3647 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py
+-rw-r--r--   0        0        0     1490 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py
+-rw-r--r--   0        0        0     1641 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py
+-rw-r--r--   0        0        0      617 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py
+-rw-r--r--   0        0        0     1102 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py
+-rw-r--r--   0        0        0     1526 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py
+-rw-r--r--   0        0        0     1594 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py
+-rw-r--r--   0        0        0      647 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/typing.py
+-rw-r--r--   0        0        0       29 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py
+-rw-r--r--   0        0        0       35 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/__init__.py
+-rw-r--r--   0        0        0      228 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/area.py
+-rw-r--r--   0        0        0      236 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/column.py
+-rw-r--r--   0        0        0      228 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/line.py
+-rw-r--r--   0        0        0     1184 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py
+-rw-r--r--   0        0        0      379 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/typing.py
+-rw-r--r--   0        0        0      974 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py
+-rw-r--r--   0        0        0       36 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py
+-rw-r--r--   0        0        0      902 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py
+-rw-r--r--   0        0        0      893 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py
+-rw-r--r--   0        0        0      906 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py
+-rw-r--r--   0        0        0     1263 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py
+-rw-r--r--   0        0        0      339 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/typing.py
+-rw-r--r--   0        0        0       34 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py
+-rw-r--r--   0        0        0     1388 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py
+-rw-r--r--   0        0        0      943 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py
+-rw-r--r--   0        0        0      903 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py
+-rw-r--r--   0        0        0      331 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/typing.py
+-rw-r--r--   0        0        0     1313 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py
+-rw-r--r--   0        0        0     2014 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py
+-rw-r--r--   0        0        0     2003 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py
+-rw-r--r--   0        0        0      136 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/__init__.py
+-rw-r--r--   0        0        0     2890 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/content.py
+-rw-r--r--   0        0        0     1265 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/exceptions.py
+-rw-r--r--   0        0        0      613 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/item.py
+-rw-r--r--   0        0        0     1431 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/markdown.py
+-rw-r--r--   0        0        0     3756 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/exceptions.py
+-rw-r--r--   0        0        0      573 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/__init__.py
+-rw-r--r--   0        0        0     1369 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/color_axis.py
+-rw-r--r--   0        0        0     1043 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/enums.py
+-rw-r--r--   0        0        0      980 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/exceptions.py
+-rw-r--r--   0        0        0       25 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/__init__.py
+-rw-r--r--   0        0        0     8048 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/base.py
+-rw-r--r--   0        0        0     4272 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py
+-rw-r--r--   0        0        0       29 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py
+-rw-r--r--   0        0        0      988 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py
+-rw-r--r--   0        0        0      954 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/legend.py
+-rw-r--r--   0        0        0       42 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/__init__.py
+-rw-r--r--   0        0        0     4887 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py
+-rw-r--r--   0        0        0      625 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/series.py
+-rw-r--r--   0        0        0     2937 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/styling.py
+-rw-r--r--   0        0        0     2113 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pandas_utils.py
+-rw-r--r--   0        0        0      672 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/__init__.py
+-rw-r--r--   0        0        0     1949 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/chart.py
+-rw-r--r--   0        0        0      852 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/exceptions.py
+-rw-r--r--   0        0        0      851 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/legend.py
+-rw-r--r--   0        0        0     6296 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/pie.py
+-rw-r--r--   0        0        0       35 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/__init__.py
+-rw-r--r--   0        0        0     6044 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/base.py
+-rw-r--r--   0        0        0     3413 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/country.py
+-rw-r--r--   0        0        0     3059 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/series.py
+-rw-r--r--   0        0        0     3185 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/styling.py
+-rw-r--r--   0        0        0      165 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/typings.py
+-rw-r--r--   0        0        0     2402 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/tooltip.py
+-rw-r--r--   0        0        0      391 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/__init__.py
+-rw-r--r--   0        0        0     3415 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/base.py
+-rw-r--r--   0        0        0      900 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/build_result.py
+-rw-r--r--   0        0        0     3470 2024-04-24 14:07:11.095692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/number.py
+-rw-r--r--   0        0        0       21 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/__init__.py
+-rw-r--r--   0        0        0     3252 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py
+-rw-r--r--   0        0        0     1523 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py
+-rw-r--r--   0        0        0     1712 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py
+-rw-r--r--   0        0        0     2432 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/text.py
+-rw-r--r--   0        0        0      280 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/typing.py
+-rw-r--r--   0        0        0     8158 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/search.py
+-rw-r--r--   0        0        0       79 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/exceptions.py
+-rw-r--r--   0        0        0     1783 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/group.py
+-rw-r--r--   0        0        0     6575 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/select.py
+-rw-r--r--   0        0        0     2453 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/__init__.py
+-rw-r--r--   0        0        0     6147 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py
+-rw-r--r--   0        0        0     6201 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py
+-rw-r--r--   0        0        0       46 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/__init__.py
+-rw-r--r--   0        0        0     5611 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py
+-rw-r--r--   0        0        0     6726 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py
+-rw-r--r--   0        0        0     5672 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py
+-rw-r--r--   0        0        0     5669 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py
+-rw-r--r--   0        0        0     5330 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py
+-rw-r--r--   0        0        0     5103 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py
+-rw-r--r--   0        0        0     5869 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py
+-rw-r--r--   0        0        0     4011 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py
+-rw-r--r--   0        0        0     6105 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py
+-rw-r--r--   0        0        0     5601 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py
+-rw-r--r--   0        0        0     5419 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py
+-rw-r--r--   0        0        0     3727 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py
+-rw-r--r--   0        0        0       49 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/__init__.py
+-rw-r--r--   0        0        0     1146 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py
+-rw-r--r--   0        0        0     1659 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py
+-rw-r--r--   0        0        0     5055 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py
+-rw-r--r--   0        0        0     1541 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py
+-rw-r--r--   0        0        0     2510 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py
+-rw-r--r--   0        0        0     1161 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py
+-rw-r--r--   0        0        0     1321 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py
+-rw-r--r--   0        0        0     1271 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py
+-rw-r--r--   0        0        0     1537 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py
+-rw-r--r--   0        0        0     1418 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py
+-rw-r--r--   0        0        0     1233 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py
+-rw-r--r--   0        0        0     1147 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py
+-rw-r--r--   0        0        0     1494 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/range.py
+-rw-r--r--   0        0        0     2723 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py
+-rw-r--r--   0        0        0     1727 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py
+-rw-r--r--   0        0        0     1779 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py
+-rw-r--r--   0        0        0      473 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/enums.py
+-rw-r--r--   0        0        0     5447 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/exceptions.py
+-rw-r--r--   0        0        0     1864 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/group.py
+-rw-r--r--   0        0        0     9162 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/header.py
+-rw-r--r--   0        0        0     2713 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/initial_state.py
+-rw-r--r--   0        0        0     2046 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/styling.py
+-rw-r--r--   0        0        0    17305 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/table.py
+-rw-r--r--   0        0        0     3155 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/__init__.py
+-rw-r--r--   0        0        0     1722 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/base.py
+-rw-r--r--   0        0        0      381 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/x_axis.py
+-rw-r--r--   0        0        0       35 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/__init__.py
+-rw-r--r--   0        0        0     4983 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py
+-rw-r--r--   0        0        0      902 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py
+-rw-r--r--   0        0        0     3279 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py
+-rw-r--r--   0        0        0     4413 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py
+-rw-r--r--   0        0        0     9066 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/chart.py
+-rw-r--r--   0        0        0      513 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/consts.py
+-rw-r--r--   0        0        0     1562 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/enums.py
+-rw-r--r--   0        0        0    12101 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py
+-rw-r--r--   0        0        0     1126 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/legend.py
+-rw-r--r--   0        0        0     3322 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py
+-rw-r--r--   0        0        0       56 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py
+-rw-r--r--   0        0        0     1051 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py
+-rw-r--r--   0        0        0     5436 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py
+-rw-r--r--   0        0        0     1339 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py
+-rw-r--r--   0        0        0       46 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/__init__.py
+-rw-r--r--   0        0        0     3472 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py
+-rw-r--r--   0        0        0     4698 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py
+-rw-r--r--   0        0        0     7615 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py
+-rw-r--r--   0        0        0     6061 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py
+-rw-r--r--   0        0        0     3621 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py
+-rw-r--r--   0        0        0     4728 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py
+-rw-r--r--   0        0        0     3637 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py
+-rw-r--r--   0        0        0     3623 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py
+-rw-r--r--   0        0        0     3654 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py
+-rw-r--r--   0        0        0      618 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py
+-rw-r--r--   0        0        0    23062 2024-04-24 14:07:11.099692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py
+-rw-r--r--   0        0        0     2038 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/transform.py
+-rw-r--r--   0        0        0       87 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/__init__.py
+-rw-r--r--   0        0        0      543 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py
+-rw-r--r--   0        0        0     5107 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/toggle.py
+-rw-r--r--   0        0        0     2755 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/utils.py
+-rw-r--r--   0        0        0       33 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/__init__.py
+-rw-r--r--   0        0        0     1336 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/authentication/auth0.py
+-rw-r--r--   0        0        0     5852 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/authentication/utils.py
+-rw-r--r--   0        0        0       92 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/__init__.py
+-rw-r--r--   0        0        0     5038 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/api.py
+-rw-r--r--   0        0        0     1195 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/clients/exceptions.py
+-rw-r--r--   0        0        0      482 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/exceptions.py
+-rw-r--r--   0        0        0      432 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/py.typed
+-rw-r--r--   0        0        0     3169 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/schema.py
+-rw-r--r--   0        0        0     6996 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/types.py
+-rw-r--r--   0        0        0      319 2024-04-24 14:07:11.103692 engineai_sdk-0.87.2/engineai/sdk/internal/url_config.py
+-rw-r--r--   0        0        0     1841 2024-04-24 14:07:29.015686 engineai_sdk-0.87.2/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 engineai_sdk-0.87.2/PKG-INFO
```

### Comparing `engineai_sdk-0.86.1/LICENSE` & `engineai_sdk-0.87.2/LICENSE`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/README.md` & `engineai_sdk-0.87.2/README.md`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/commands/app.py` & `engineai_sdk-0.87.2/engineai/sdk/cli/commands/app.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/commands/dashboard.py` & `engineai_sdk-0.87.2/engineai/sdk/cli/commands/dashboard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/console.py` & `engineai_sdk-0.87.2/engineai/sdk/cli/console.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/generator.py` & `engineai_sdk-0.87.2/engineai/sdk/cli/generator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/template/content/data/example.json` & `engineai_sdk-0.87.2/engineai/sdk/cli/template/content/data/example.json`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/cli/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/layout.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/layout.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/abstract/typing.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/abstract/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/activate_dashboard.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/activate_dashboard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/api.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/api.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/serialization/json.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/serialization/json.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/clients/storage/storage.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/clients/storage/storage.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/config.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/dashboard.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/executor_config.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/executor_config.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/instance.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/instance.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/node.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/node.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/graph/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/graph/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/dependency.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/dependency.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/page.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/page.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/root.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/root.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/page/route.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/page/route.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dashboard/version/version.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dashboard/version/version.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/decorator.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/duplicated.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/duplicated.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/enums.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/http.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/http.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/io_handler.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/io_handler.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/interface.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/data/manager/manager.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/data/manager/manager.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/decorator.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/decorator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/datastore.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/datastore.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/http/http.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/http/http.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/route.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/route.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/dependencies/widget.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/dependencies/widget.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/align.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/align.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/enum/legend_position.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/enum/legend_position.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/datetime.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/datetime.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/mapper.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/mapper.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/number.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/text.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/formatting/validator.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/formatting/validator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/interface.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/interface.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/card.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/card.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/chip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/card/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/card/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/chip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/collapsible/section.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/collapsible/section.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/chip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/components/label.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/components/label.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/fluid_row.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/fluid_row/items_build.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/fluid_row/items_build.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/grid.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/grid.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/row.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/row.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/selectable/tab.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/selectable/tab.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/layout/typings.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/layout/typings.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/abstract.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/abstract.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/route_link.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/route_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/template_string_link.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/template_string_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/url.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/url.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_dependency.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_dependency.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/links/widget_field.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/links/widget_field.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/selected.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/selected.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/default_specs.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/default_specs.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/discrete_map.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/discrete_map.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/divergent.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/divergent.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/gradient.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/gradient.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/palette.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/palette.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/single.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/single.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/color/spec.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/color/spec.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/styling/icons.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/styling/icons.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/templated_string.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/templated_string.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/x_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/axis/y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/cartesian.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/cartesian.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/chart.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/chart.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/legend.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/area_range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/bubble.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/line.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/scatter.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/cartesian/series/typing.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/cartesian/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/chart_utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/chart_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/actions/links/url_link.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/dynamic.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/negative.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/positive.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/scale.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/axis/scale/symmetric.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/series/entities/custom.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/area_range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_circle.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/bubble_country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/error_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/line.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/point.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/point.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/scatter.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/styling/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/category.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/datetime.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/tooltip/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/charts/typing.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/charts/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/chart/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/arrow.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/dot.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/font.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/number/progress_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/chip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/country_flag.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/dot.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/styling/text/font.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/format_build.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/components/items/tooltip/tooltip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/content.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/content.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/item.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/item.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/content/markdown.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/content/markdown.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/color_axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/color_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/enums.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/geo.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/geo.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/label.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/geo/styling/styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/legend.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/numeric.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/numeric.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/series.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/series.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/maps/series/styling.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/maps/series/styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pandas_utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/chart.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/chart.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/legend.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/pie.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/pie.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/country.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/series.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/series.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/series/styling.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/series/styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/pie/tooltip.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/pie/tooltip.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/build_result.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/build_result.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/number.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/base_styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/number.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/styling/text.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/styling/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/results/text.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/results/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/search/search.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/search/search.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/group.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/group.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/select/select.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/select/select.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/category.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/category.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/charts/stack_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/country.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/country.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/datetime.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/number.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/number.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/range.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/text.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/text.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/items/url_column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/area.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/arrow.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/cell.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/color_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/country_flag.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/dot.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/font.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/font.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/icon.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/line.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/range.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/split_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/stacked_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/columns/styling/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/group.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/group.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/header.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/header.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/initial_state.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/initial_state.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/styling.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/styling.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/table/table.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/table/table.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/__init__.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/build_y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/axis/y_axis/y_axis_mirror.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/chart.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/chart.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/consts.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/consts.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/enums.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/enums.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/legend.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/legend.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/navigator.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/navigator.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/custom_period.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/period.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/selector.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/period_selector/standard.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/area_range.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/base.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/base.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/bubble.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/column.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/column.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/error_bar.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/line.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/line.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/point.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/point.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/scatter.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/series/typing.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/series/typing.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/timeseries.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/timeseries/transform.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/timeseries/transform.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/toggle/toggle.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/toggle/toggle.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/dashboard/widgets/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/dashboard/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/authentication/auth0.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/authentication/auth0.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/authentication/utils.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/clients/api.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/clients/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
         else:
             raise APIUrlNotFound()
 
     @staticmethod
     def __initialize_session(max_retries: int = 3) -> requests.Session:
         """Creates a HTTP/HTTPS session and returns."""
         retries = urllib3.Retry(
-            total=max_retries, backoff_factor=0.1, status_forcelist=[500, 502, 503, 504]
+            total=max_retries,
+            backoff_factor=0.1,
+            status_forcelist=[500, 502, 503, 504, 400, 401],
         )
         adapter = HTTPAdapter(max_retries=retries)
         session = requests.Session()
         session.mount("https://", adapter)
         session.mount("http://", adapter)
         return session
```

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/clients/exceptions.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/schema.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/schema.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/engineai/sdk/internal/graphql_dataclasses/types.py` & `engineai_sdk-0.87.2/engineai/sdk/internal/graphql_dataclasses/types.py`

 * *Files identical despite different names*

### Comparing `engineai_sdk-0.86.1/pyproject.toml` & `engineai_sdk-0.87.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "engineai.sdk"
-version = "0.86.1"
+version = "0.87.2"
 description = "EngineAI's Platform SDK"
 authors = ["Pedro Rodrigues <pedro@dystematic.com>"]
 maintainers = [
   "Pedro Cunha <cunha@engineai.com>",
   "Pedro Feiteira <feiteira@engineai.com>",
   "Li Zixiang <li.zixiang@engineai.com>",
   "Joao Matos <matos@engineai.com>",
```

### Comparing `engineai_sdk-0.86.1/PKG-INFO` & `engineai_sdk-0.87.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engineai.sdk
-Version: 0.86.1
+Version: 0.87.2
 Summary: EngineAI's Platform SDK
 License: MIT
 Author: Pedro Rodrigues
 Author-email: pedro@dystematic.com
 Maintainer: Pedro Cunha
 Maintainer-email: cunha@engineai.com
 Requires-Python: >=3.8,<3.12
```

