# Comparing `tmp/tdf_tool-2.4.8.tar.gz` & `tmp/tdf_tool-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdf_tool-2.4.8.tar", max compression
+gzip compressed data, was "tdf_tool-2.4.9.tar", max compression
```

## Comparing `tdf_tool-2.4.8.tar` & `tdf_tool-2.4.9.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.8/LICENSE
--rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.8/README.md
--rw-r--r--   0        0        0     1608 2024-04-20 02:38:19.860796 tdf_tool-2.4.8/pyproject.toml
--rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.8/tdf_tool/app.py
--rw-r--r--   0        0        0     1106 2024-04-18 09:33:56.862188 tdf_tool-2.4.8/tdf_tool/pipeline.py
--rw-r--r--   0        0        0     8469 2024-04-18 09:33:56.862568 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
--rw-r--r--   0        0        0     4497 2024-04-19 02:17:38.880307 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
--rw-r--r--   0        0        0     7799 2024-04-20 02:32:50.400921 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
--rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
--rw-r--r--   0        0        0     1676 2024-04-19 02:17:38.888443 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
--rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     1619 2024-04-19 02:17:38.894201 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     2292 2024-04-19 02:17:38.497917 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
--rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
--rw-r--r--   0        0        0     2243 2024-04-19 02:17:38.892162 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0    16038 2024-04-19 09:06:09.150577 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
--rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0     1989 2024-04-19 02:17:38.771913 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
--rw-r--r--   0        0        0      621 2024-04-18 09:33:56.866062 tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
--rw-r--r--   0        0        0     5130 2024-04-18 09:33:56.866355 tdf_tool-2.4.8/tdf_tool/pipelines/annotation.py
--rw-r--r--   0        0        0     7878 2024-04-20 02:32:38.597752 tdf_tool-2.4.8/tdf_tool/pipelines/api_interaction.py
--rw-r--r--   0        0        0     1244 2024-04-18 09:33:56.867085 tdf_tool-2.4.8/tdf_tool/pipelines/fix_header.py
--rw-r--r--   0        0        0     1211 2024-04-18 09:33:56.867471 tdf_tool-2.4.8/tdf_tool/pipelines/git.py
--rw-r--r--   0        0        0     1889 2024-04-18 09:33:56.867849 tdf_tool-2.4.8/tdf_tool/pipelines/module.py
--rw-r--r--   0        0        0     1630 2024-04-18 09:33:56.868234 tdf_tool-2.4.8/tdf_tool/pipelines/package.py
--rw-r--r--   0        0        0    21886 2024-04-19 08:19:40.561443 tdf_tool-2.4.8/tdf_tool/pipelines/router.py
--rw-r--r--   0        0        0     1656 2024-04-18 09:33:56.869173 tdf_tool-2.4.8/tdf_tool/pipelines/translate.py
--rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.8/tdf_tool/pipelines/upgrade.py
--rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2024-04-18 09:33:56.869593 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5149 2024-04-18 09:33:56.870029 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0     1113 2024-04-19 09:46:49.061939 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0      890 2024-04-19 09:59:10.596913 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/generator.cpython-39.pyc
--rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1464 2024-04-18 09:33:56.871044 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     2040 2024-04-19 09:43:51.505624 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc
--rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
--rw-r--r--   0        0        0     6181 2024-04-18 09:33:56.871935 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
--rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
--rw-r--r--   0        0        0     5620 2024-04-19 02:17:38.568605 tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
--rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
--rw-r--r--   0        0        0     7694 2024-04-18 09:33:56.873380 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
--rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
--rw-r--r--   0        0        0     4018 2024-04-18 09:33:56.873929 tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
--rw-r--r--   0        0        0     1835 2024-04-18 09:33:56.874377 tdf_tool-2.4.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.8/tdf_tool/tools/cli/bean/deps_item.py
--rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.8/tdf_tool/tools/cli/module_deps_rewrite.py
--rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.8/tdf_tool/tools/cli/project_cli.py
--rw-r--r--   0        0        0     1919 2024-04-18 09:33:56.874872 tdf_tool-2.4.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.8/tdf_tool/tools/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.8/tdf_tool/tools/cmd.py
--rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     3385 2024-04-18 09:33:56.875378 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1491 2024-04-19 02:17:38.769502 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     2103 2024-04-19 02:17:38.774000 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
--rw-r--r--   0        0        0     4496 2024-04-18 09:33:56.876915 tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
--rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.8/tdf_tool/tools/config/config.py
--rw-r--r--   0        0        0     1310 2024-04-18 09:33:56.877413 tdf_tool-2.4.8/tdf_tool/tools/config/initial_json_config.py
--rw-r--r--   0        0        0     1267 2024-04-18 09:33:56.877960 tdf_tool-2.4.8/tdf_tool/tools/config/module_json_config.py
--rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.8/tdf_tool/tools/config/packages_config.py
--rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.8/tdf_tool/tools/dependencies_analysis.py
--rw-r--r--   0        0        0      776 2024-04-19 09:46:46.688382 tdf_tool-2.4.8/tdf_tool/tools/env.py
--rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
--rw-r--r--   0        0        0     3616 2024-04-18 09:33:56.878578 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
--rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2004 2024-04-18 09:33:56.879118 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
--rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
--rw-r--r--   0        0        0     2464 2024-04-18 09:33:56.879669 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
--rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
--rw-r--r--   0        0        0     3681 2024-04-18 09:33:56.880258 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
--rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
--rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_entry.py
--rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint.py
--rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py
--rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py
--rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.8/tdf_tool/tools/flutter_script.py
--rw-r--r--   0        0        0      444 2024-04-19 09:59:03.824969 tdf_tool-2.4.8/tdf_tool/tools/generator.py
--rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2024-04-18 09:33:56.880901 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
--rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
--rw-r--r--   0        0        0     3786 2024-04-18 09:33:56.881487 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
--rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
--rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.8/tdf_tool/tools/gitlab/gitlab_utils.py
--rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.8/tdf_tool/tools/gitlab/python_gitlab_api.py
--rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1412 2024-04-18 09:33:56.882138 tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.8/tdf_tool/tools/module/module_tools.py
--rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5267 2024-04-18 09:33:56.882719 tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.8/tdf_tool/tools/package/seal_off_package_utils.py
--rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.8/tdf_tool/tools/platform_tools.py
--rw-r--r--   0        0        0     1226 2024-04-19 09:43:13.615410 tdf_tool-2.4.8/tdf_tool/tools/print.py
--rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.8/tdf_tool/tools/regular_tool.py
--rw-r--r--   0        0        0     5718 2024-04-18 09:33:56.883146 tdf_tool-2.4.8/tdf_tool/tools/shell_dir.py
--rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
--rw-r--r--   0        0        0     2161 2024-04-18 09:33:56.883746 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1678 2024-04-18 09:33:56.884279 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.8/tdf_tool/tools/translate/file_util.py
--rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     8285 2024-04-18 09:33:56.884733 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0    13427 2024-04-18 09:33:56.885241 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
--rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
--rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4595 2024-04-18 09:33:56.885795 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
--rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
--rw-r--r--   0        0        0     4216 2024-04-18 09:33:56.886328 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
--rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2347 2024-04-18 09:33:56.886740 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate.py
--rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate_lint.py
--rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
--rw-r--r--   0        0        0     2852 2024-04-18 09:33:56.887291 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
--rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
--rw-r--r--   0        0        0     9306 2024-04-18 09:33:56.887836 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4398 2024-04-18 09:33:56.888413 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
--rw-r--r--   0        0        0     1028 2024-04-18 09:33:56.889038 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0     5366 2024-04-18 09:33:56.889482 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
--rw-r--r--   0        0        0     2689 2024-04-18 09:33:56.889936 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
--rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
--rw-r--r--   0        0        0     6226 2024-04-18 09:33:56.890414 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
--rw-r--r--   0        0        0     2687 2024-04-18 09:33:56.890983 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
--rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_module.py
--rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
--rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
--rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
--rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py
--rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/podspec.py
--rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/string_util.py
--rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
--rw-r--r--   0        0        0     5032 2024-04-18 09:33:56.891445 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.8/tdf_tool/tools/translate/tools/translate_tool.py
--rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.8/tdf_tool/tools/translate/translate_lint.py
--rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
--rw-r--r--   0        0        0      880 2024-04-18 09:33:56.891894 tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
--rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.8/tdf_tool/tools/vscode/vscode.py
--rw-r--r--   0        0        0    10568 1970-01-01 00:00:00.000000 tdf_tool-2.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 07:59:17.944743 tdf_tool-2.4.9/LICENSE
+-rw-r--r--   0        0        0     9217 2024-04-16 07:59:17.944961 tdf_tool-2.4.9/README.md
+-rw-r--r--   0        0        0     1608 2024-04-20 03:05:23.292161 tdf_tool-2.4.9/pyproject.toml
+-rw-r--r--   0        0        0      321 2024-04-16 07:59:17.947227 tdf_tool-2.4.9/tdf_tool/app.py
+-rw-r--r--   0        0        0     1106 2024-04-18 09:33:56.862188 tdf_tool-2.4.9/tdf_tool/pipeline.py
+-rw-r--r--   0        0        0     8469 2024-04-18 09:33:56.862568 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc
+-rw-r--r--   0        0        0     4524 2024-04-20 03:04:01.674118 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc
+-rw-r--r--   0        0        0     7799 2024-04-20 02:32:50.400921 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc
+-rw-r--r--   0        0        0      424 2024-04-16 07:59:17.947648 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2567 2024-04-16 07:59:17.947827 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
+-rw-r--r--   0        0        0     1676 2024-04-19 02:17:38.888443 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
+-rw-r--r--   0        0        0     2668 2024-04-16 07:59:17.948134 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     1619 2024-04-19 02:17:38.894201 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2024-04-16 07:59:17.948441 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     3015 2024-04-16 07:59:17.948597 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     2292 2024-04-19 02:17:38.497917 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
+-rw-r--r--   0        0        0     2981 2024-04-16 07:59:17.948929 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0     2243 2024-04-19 02:17:38.892162 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0    36213 2024-04-16 07:59:17.949402 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0    16038 2024-04-19 09:06:09.150577 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
+-rw-r--r--   0        0        0     3262 2024-04-16 07:59:17.950144 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0     1989 2024-04-19 02:17:38.771913 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2024-04-16 07:59:17.950609 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
+-rw-r--r--   0        0        0      621 2024-04-18 09:33:56.866062 tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
+-rw-r--r--   0        0        0     5191 2024-04-20 03:03:57.569102 tdf_tool-2.4.9/tdf_tool/pipelines/annotation.py
+-rw-r--r--   0        0        0     7878 2024-04-20 02:32:38.597752 tdf_tool-2.4.9/tdf_tool/pipelines/api_interaction.py
+-rw-r--r--   0        0        0     1244 2024-04-18 09:33:56.867085 tdf_tool-2.4.9/tdf_tool/pipelines/fix_header.py
+-rw-r--r--   0        0        0     1211 2024-04-18 09:33:56.867471 tdf_tool-2.4.9/tdf_tool/pipelines/git.py
+-rw-r--r--   0        0        0     1889 2024-04-18 09:33:56.867849 tdf_tool-2.4.9/tdf_tool/pipelines/module.py
+-rw-r--r--   0        0        0     1630 2024-04-18 09:33:56.868234 tdf_tool-2.4.9/tdf_tool/pipelines/package.py
+-rw-r--r--   0        0        0    21886 2024-04-19 08:19:40.561443 tdf_tool-2.4.9/tdf_tool/pipelines/router.py
+-rw-r--r--   0        0        0     1656 2024-04-18 09:33:56.869173 tdf_tool-2.4.9/tdf_tool/pipelines/translate.py
+-rw-r--r--   0        0        0      179 2024-04-16 07:59:17.952763 tdf_tool-2.4.9/tdf_tool/pipelines/upgrade.py
+-rw-r--r--   0        0        0     1653 2024-04-16 07:59:17.953204 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
+-rw-r--r--   0        0        0     1064 2024-04-18 09:33:56.869593 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0    10270 2024-04-16 07:59:17.953777 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5149 2024-04-18 09:33:56.870029 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2024-04-16 07:59:17.954419 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0     1113 2024-04-19 09:46:49.061939 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0      890 2024-04-19 09:59:10.596913 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/generator.cpython-39.pyc
+-rw-r--r--   0        0        0     2480 2024-04-16 07:59:17.954948 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1464 2024-04-18 09:33:56.871044 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2024-04-16 07:59:17.955456 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     2040 2024-04-19 09:43:51.505624 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/print.cpython-39.pyc
+-rw-r--r--   0        0        0     9661 2024-04-16 07:59:17.955984 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     6181 2024-04-18 09:33:56.871935 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
+-rw-r--r--   0        0        0    10739 2024-04-16 07:59:17.956576 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
+-rw-r--r--   0        0        0     5649 2024-04-20 02:59:57.756466 tdf_tool-2.4.9/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
+-rw-r--r--   0        0        0    11432 2024-04-16 07:59:17.957426 tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
+-rw-r--r--   0        0        0     7694 2024-04-18 09:33:56.873380 tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
+-rw-r--r--   0        0        0     7216 2024-04-16 07:59:17.958050 tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
+-rw-r--r--   0        0        0     4018 2024-04-18 09:33:56.873929 tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     1835 2024-04-18 09:33:56.874377 tdf_tool-2.4.9/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2024-04-16 07:59:17.959126 tdf_tool-2.4.9/tdf_tool/tools/cli/bean/deps_item.py
+-rw-r--r--   0        0        0    12287 2024-04-16 07:59:17.959442 tdf_tool-2.4.9/tdf_tool/tools/cli/module_deps_rewrite.py
+-rw-r--r--   0        0        0     5041 2024-04-16 07:59:17.959734 tdf_tool-2.4.9/tdf_tool/tools/cli/project_cli.py
+-rw-r--r--   0        0        0     1919 2024-04-18 09:33:56.874872 tdf_tool-2.4.9/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1833 2024-04-16 07:59:17.960396 tdf_tool-2.4.9/tdf_tool/tools/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      559 2024-04-16 07:59:17.960648 tdf_tool-2.4.9/tdf_tool/tools/cmd.py
+-rw-r--r--   0        0        0     7002 2024-04-16 07:59:17.961174 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     3385 2024-04-18 09:33:56.875378 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2024-04-16 07:59:17.961718 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1491 2024-04-19 02:17:38.769502 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2024-04-16 07:59:17.962260 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2024-04-16 07:59:17.962513 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     2103 2024-04-19 02:17:38.774000 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     9155 2024-04-16 07:59:17.963058 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
+-rw-r--r--   0        0        0     4496 2024-04-18 09:33:56.876915 tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3983 2024-04-16 07:59:17.963572 tdf_tool-2.4.9/tdf_tool/tools/config/config.py
+-rw-r--r--   0        0        0     1310 2024-04-18 09:33:56.877413 tdf_tool-2.4.9/tdf_tool/tools/config/initial_json_config.py
+-rw-r--r--   0        0        0     1267 2024-04-18 09:33:56.877960 tdf_tool-2.4.9/tdf_tool/tools/config/module_json_config.py
+-rw-r--r--   0        0        0     5593 2024-04-16 07:59:17.964325 tdf_tool-2.4.9/tdf_tool/tools/config/packages_config.py
+-rw-r--r--   0        0        0     7704 2024-04-16 07:59:17.964588 tdf_tool-2.4.9/tdf_tool/tools/dependencies_analysis.py
+-rw-r--r--   0        0        0      776 2024-04-19 09:46:46.688382 tdf_tool-2.4.9/tdf_tool/tools/env.py
+-rw-r--r--   0        0        0     6312 2024-04-16 07:59:17.965341 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
+-rw-r--r--   0        0        0     3616 2024-04-18 09:33:56.878578 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
+-rw-r--r--   0        0        0     3174 2024-04-16 07:59:17.965839 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2004 2024-04-18 09:33:56.879118 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
+-rw-r--r--   0        0        0     4314 2024-04-16 07:59:17.966355 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     2464 2024-04-18 09:33:56.879669 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     6437 2024-04-16 07:59:17.966902 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     3681 2024-04-18 09:33:56.880258 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     2422 2024-04-16 07:59:17.967708 tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     3345 2024-04-16 07:59:17.967959 tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_entry.py
+-rw-r--r--   0        0        0     1586 2024-04-16 07:59:17.968270 tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_lint.py
+-rw-r--r--   0        0        0     2137 2024-04-16 07:59:17.968589 tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_lint_tool.py
+-rw-r--r--   0        0        0     4095 2024-04-16 07:59:17.968850 tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_replace_tool.py
+-rw-r--r--   0        0        0     1159 2024-04-16 07:59:17.969195 tdf_tool-2.4.9/tdf_tool/tools/flutter_script.py
+-rw-r--r--   0        0        0      444 2024-04-19 09:59:03.824969 tdf_tool-2.4.9/tdf_tool/tools/generator.py
+-rw-r--r--   0        0        0     7243 2024-04-16 07:59:17.969845 tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2024-04-18 09:33:56.880901 tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     7055 2024-04-16 07:59:17.970442 tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
+-rw-r--r--   0        0        0     3786 2024-04-18 09:33:56.881487 tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2024-04-16 07:59:17.971051 tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
+-rw-r--r--   0        0        0     5019 2024-04-16 07:59:17.971732 tdf_tool-2.4.9/tdf_tool/tools/gitlab/gitlab_utils.py
+-rw-r--r--   0        0        0     3814 2024-04-16 07:59:17.972085 tdf_tool-2.4.9/tdf_tool/tools/gitlab/python_gitlab_api.py
+-rw-r--r--   0        0        0     2482 2024-04-16 07:59:17.972678 tdf_tool-2.4.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1412 2024-04-18 09:33:56.882138 tdf_tool-2.4.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1063 2024-04-16 07:59:17.973603 tdf_tool-2.4.9/tdf_tool/tools/module/module_tools.py
+-rw-r--r--   0        0        0    11056 2024-04-16 07:59:17.974266 tdf_tool-2.4.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5267 2024-04-18 09:33:56.882719 tdf_tool-2.4.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9752 2024-04-16 07:59:17.974933 tdf_tool-2.4.9/tdf_tool/tools/package/seal_off_package_utils.py
+-rw-r--r--   0        0        0      911 2024-04-16 07:59:17.975191 tdf_tool-2.4.9/tdf_tool/tools/platform_tools.py
+-rw-r--r--   0        0        0     1226 2024-04-19 09:43:13.615410 tdf_tool-2.4.9/tdf_tool/tools/print.py
+-rw-r--r--   0        0        0     7598 2024-04-16 07:59:17.975770 tdf_tool-2.4.9/tdf_tool/tools/regular_tool.py
+-rw-r--r--   0        0        0     5718 2024-04-20 03:05:05.114112 tdf_tool-2.4.9/tdf_tool/tools/shell_dir.py
+-rw-r--r--   0        0        0     3840 2024-04-16 07:59:17.976600 tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2161 2024-04-18 09:33:56.883746 tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     2695 2024-04-16 07:59:17.977108 tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1678 2024-04-18 09:33:56.884279 tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    11711 2024-04-16 07:59:17.977716 tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1999 2024-04-16 07:59:17.977961 tdf_tool-2.4.9/tdf_tool/tools/translate/file_util.py
+-rw-r--r--   0        0        0    15484 2024-04-16 07:59:17.978545 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     8285 2024-04-18 09:33:56.884733 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    26818 2024-04-16 07:59:17.979344 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13427 2024-04-18 09:33:56.885241 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    10691 2024-04-16 07:59:17.980114 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
+-rw-r--r--   0        0        0    18954 2024-04-16 07:59:17.980464 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
+-rw-r--r--   0        0        0     8395 2024-04-16 07:59:17.981075 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4595 2024-04-18 09:33:56.885795 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     5228 2024-04-16 07:59:17.981648 tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
+-rw-r--r--   0        0        0      859 2024-04-16 07:59:17.982222 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     7351 2024-04-16 07:59:17.982702 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7599 2024-04-16 07:59:17.983077 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
+-rw-r--r--   0        0        0     4216 2024-04-18 09:33:56.886328 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
+-rw-r--r--   0        0        0     3952 2024-04-16 07:59:17.983786 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2347 2024-04-18 09:33:56.886740 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0      870 2024-04-16 07:59:17.984330 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0     4766 2024-04-16 07:59:17.984706 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     6219 2024-04-16 07:59:17.985086 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2024-04-16 07:59:17.985435 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     4438 2024-04-16 07:59:17.985774 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/ios_translate.py
+-rw-r--r--   0        0        0     2000 2024-04-16 07:59:17.986154 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/ios_translate_lint.py
+-rw-r--r--   0        0        0     5061 2024-04-16 07:59:17.986697 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     2852 2024-04-18 09:33:56.887291 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    17576 2024-04-16 07:59:17.987402 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
+-rw-r--r--   0        0        0     9306 2024-04-18 09:33:56.887836 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2024-04-16 07:59:17.988120 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4398 2024-04-18 09:33:56.888413 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2024-04-16 07:59:17.988695 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2024-04-18 09:33:56.889038 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0    10070 2024-04-16 07:59:17.989363 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     5366 2024-04-18 09:33:56.889482 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2773 2024-04-16 07:59:17.989983 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
+-rw-r--r--   0        0        0     2689 2024-04-18 09:33:56.889936 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
+-rw-r--r--   0        0        0    11353 2024-04-16 07:59:17.990542 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
+-rw-r--r--   0        0        0     6226 2024-04-18 09:33:56.890414 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2024-04-16 07:59:17.991277 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2687 2024-04-18 09:33:56.890983 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2024-04-16 07:59:17.991799 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
+-rw-r--r--   0        0        0    14326 2024-04-16 07:59:17.992093 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_module.py
+-rw-r--r--   0        0        0     5223 2024-04-16 07:59:17.992380 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
+-rw-r--r--   0        0        0     1189 2024-04-16 07:59:17.992605 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
+-rw-r--r--   0        0        0     8191 2024-04-16 07:59:17.992866 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
+-rw-r--r--   0        0        0     2337 2024-04-16 07:59:17.993215 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/location_string_temp.py
+-rw-r--r--   0        0        0     8684 2024-04-16 07:59:17.993505 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/podspec.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:59:17.993759 tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/string_util.py
+-rw-r--r--   0        0        0     8625 2024-04-16 07:59:17.994344 tdf_tool-2.4.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     5032 2024-04-18 09:33:56.891445 tdf_tool-2.4.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2024-04-16 07:59:17.994952 tdf_tool-2.4.9/tdf_tool/tools/translate/tools/translate_tool.py
+-rw-r--r--   0        0        0     1408 2024-04-16 07:59:17.995250 tdf_tool-2.4.9/tdf_tool/tools/translate/translate_lint.py
+-rw-r--r--   0        0        0     1268 2024-04-16 07:59:17.996782 tdf_tool-2.4.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
+-rw-r--r--   0        0        0      880 2024-04-18 09:33:56.891894 tdf_tool-2.4.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2024-04-16 07:59:17.997353 tdf_tool-2.4.9/tdf_tool/tools/vscode/vscode.py
+-rw-r--r--   0        0        0    10568 1970-01-01 00:00:00.000000 tdf_tool-2.4.9/PKG-INFO
```

### Comparing `tdf_tool-2.4.8/LICENSE` & `tdf_tool-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/README.md` & `tdf_tool-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/pyproject.toml` & `tdf_tool-2.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 项目信息
 [tool.poetry]
 name = "tdf_tool"
-version = "2.4.8"
+version = "2.4.9"
 description = "二维火 flutter 脚手架工具"
 authors = ["Jian Xu <3386218996@qq.com>", "FanJiao Gai <gaijiaofan@2dfire.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://git.2dfire.net/app/flutter/tools/package_tools"
 repository = "https://git.2dfire.net/app/flutter/tools/package_tools.git"
 keywords = ["tdf", "tdf-tool", "tdf_tool"]
```

### Comparing `tdf_tool-2.4.8/tdf_tool/pipeline.py` & `tdf_tool-2.4.9/tdf_tool/pipeline.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/anno.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/annotation.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:33:56 2024 UTC, .py size: 5130 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,282 +1,283 @@
-00000000: 610d 0d0a 0000 0000 04e9 2066 0a14 0000  a......... f....
+00000000: 610d 0d0a 0000 0000 9d30 2366 4714 0000  a........0#fG...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
+00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 6400 6408 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
-00000090: 0100 4700 6409 640a 8400 640a 8302 5a11  ..G.d.d...d...Z.
-000000a0: 6401 5300 290b e900 0000 004e 2901 da11  d.S.)......N)...
-000000b0: 496e 6974 6961 6c4a 736f 6e43 6f6e 6669  InitialJsonConfi
-000000c0: 6729 02da 0e4d 6f64 756c 6549 7465 6d54  g)...ModuleItemT
-000000d0: 7970 65da 104d 6f64 756c 654a 736f 6e43  ype..ModuleJsonC
-000000e0: 6f6e 6669 6729 02da 0b50 6163 6b61 6765  onfig)...Package
-000000f0: 4e6f 6465 da12 5061 636b 6167 6573 4a73  Node..PackagesJs
-00000100: 6f6e 436f 6e66 6967 2901 da05 5072 696e  onConfig)...Prin
-00000110: 7429 01da 0853 6865 6c6c 4469 7229 01da  t)...ShellDir)..
-00000120: 0652 6f75 7465 7229 01da 0d41 7069 416e  .Router)...ApiAn
-00000130: 6e6f 7461 7469 6f6e 6300 0000 0000 0000  notationc.......
-00000140: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000150: 0073 5600 0000 6500 5a01 6400 5a02 6401  .sV...e.Z.d.Z.d.
-00000160: 5a03 6402 6403 8400 5a04 6404 6405 8400  Z.d.d...Z.d.d...
-00000170: 5a05 6506 6406 9c01 6407 6408 8404 5a07  Z.e.d...d.d...Z.
-00000180: 6409 640a 8400 5a08 6506 6509 640b 9c02  d.d...Z.e.e.d...
-00000190: 640c 640d 8404 5a0a 640e 640f 8400 5a0b  d.d...Z.d.d...Z.
-000001a0: 6410 6411 8400 5a0c 6412 5300 2913 da0a  d.d...Z.d.S.)...
-000001b0: 416e 6e6f 7461 7469 6f6e 7545 0000 000a  AnnotationuE....
-000001c0: 2020 2020 e6a8 a1e5 9d97 e997 b4e6 94af      ............
-000001d0: e68c 81e7 9bb8 e585 b3e5 91bd e4bb a4ef  ................
-000001e0: bc9a 746c 2061 6e6e 6f74 6174 696f 6e20  ..tl annotation 
-000001f0: 2d68 20e6 9fa5 e79c 8be8 afa6 e683 850a  -h .............
-00000200: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00000210: 0001 0000 0003 0000 0043 0000 0073 3e00  .........C...s>.
-00000220: 0000 7400 a001 6401 a101 0100 6402 7c00  ..t...d.....d.|.
-00000230: 5f02 7403 8300 7c00 5f04 7405 8300 7c00  _.t...|._.t...|.
-00000240: 5f06 7c00 a007 a100 7c00 5f08 7409 740a  _.|.....|._.t.t.
-00000250: a00b a100 8301 6a0c 7c00 5f0d 6400 5300  ......j.|._.d.S.
-00000260: 2903 4e75 0c00 0000 e6a3 80e6 b58b e4b8  ).Nu............
-00000270: ad2e 2e2e 5a0c 6275 696c 645f 7275 6e6e  ....Z.build_runn
-00000280: 6572 290e 7207 0000 00da 0574 6974 6c65  er).r......title
-00000290: da1c 5f41 6e6e 6f74 6174 696f 6e5f 5f62  .._Annotation__b
-000002a0: 7569 6c64 5275 6e6e 6572 4e61 6d65 7209  uildRunnerNamer.
-000002b0: 0000 00da 1d5f 416e 6e6f 7461 7469 6f6e  ....._Annotation
-000002c0: 5f5f 726f 7574 6572 416e 6e6f 7461 7469  __routerAnnotati
-000002d0: 6f6e 720a 0000 00da 1a5f 416e 6e6f 7461  onr......_Annota
-000002e0: 7469 6f6e 5f5f 6170 6941 6e6e 6f74 6174  tion__apiAnnotat
-000002f0: 696f 6eda 235f 416e 6e6f 7461 7469 6f6e  ion.#_Annotation
-00000300: 5f5f 6170 695f 6275 7369 6e65 7373 4d6f  __api_businessMo
-00000310: 6475 6c65 4c69 7374 da1f 5f41 6e6e 6f74  duleList.._Annot
-00000320: 6174 696f 6e5f 5f62 7573 696e 6573 734d  ation__businessM
-00000330: 6f64 756c 654c 6973 7472 0600 0000 7208  oduleListr....r.
-00000340: 0000 00da 0b67 6574 5368 656c 6c44 6972  .....getShellDir
-00000350: da08 7061 636b 6167 6573 da19 5f41 6e6e  ..packages.._Ann
-00000360: 6f74 6174 696f 6e5f 5f70 6163 6b61 6765  otation__package
-00000370: 734c 6973 74a9 01da 0473 656c 66a9 0072  sList....self..r
-00000380: 1700 0000 f569 0000 002f 5573 6572 732f  .....i.../Users/
-00000390: 7875 6a69 616e 2f44 6f63 756d 656e 7473  xujian/Documents
-000003a0: 2f32 3032 342f e6a8 a1e5 9d97 e997 b4e4  /2024/..........
-000003b0: baa4 e4ba 92e9 a1b9 e79b ae74 6ce5 8d87  ...........tl...
-000003c0: e7ba a72f 7061 636b 6167 655f 746f 6f6c  .../package_tool
-000003d0: 732f 7464 665f 746f 6f6c 2f70 6970 656c  s/tdf_tool/pipel
-000003e0: 696e 6573 2f61 6e6e 6f74 6174 696f 6e2e  ines/annotation.
-000003f0: 7079 da08 5f5f 696e 6974 5f5f 1000 0000  py..__init__....
-00000400: 730c 0000 0000 010a 0106 0208 0108 010a  s...............
-00000410: 017a 1341 6e6e 6f74 6174 696f 6e2e 5f5f  .z.Annotation.__
-00000420: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-00000430: 0000 0006 0000 0008 0000 0043 0000 0073  ...........C...s
-00000440: 2c01 0000 7400 a001 a100 0100 7402 a003  ,...t.......t...
-00000450: 6401 a101 0100 7404 7c00 6a05 8301 4400  d.....t.|.j...D.
-00000460: 5d1a 5c02 7d01 7d02 7406 7c01 9b00 6402  ].\.}.}.t.|...d.
-00000470: 7c02 9b00 9d03 8301 0100 711c 7406 8300  |.........q.t...
-00000480: 0100 7407 6403 8301 7d03 7c03 6404 6b02  ..t.d...}.|.d.k.
-00000490: 7356 7c03 6405 6b02 7260 7408 6406 8301  sV|.d.k.r`t.d...
-000004a0: 0100 713e 7c03 6407 6b02 727a 7c00 a009  ..q>|.d.k.rz|...
-000004b0: a100 0100 7408 6406 8301 0100 713e 7c03  ....t.d.....q>|.
-000004c0: 7c00 6a05 7600 72ae 7c00 a00a 7c03 a101  |.j.v.r.|...|...
-000004d0: 0100 7402 a00b 7c03 6408 1700 a101 0100  ..t...|.d.......
-000004e0: 7c00 a009 a100 0100 7408 6406 8301 0100  |.......t.d.....
-000004f0: 713e 7a58 740c 7c03 8301 7d04 7c04 740d  q>zXt.|...}.|.t.
-00000500: 7c00 6a05 8301 6b00 72fa 7c00 6a05 7c04  |.j...k.r.|.j.|.
-00000510: 1900 7d05 7c00 a00a 7c05 a101 0100 7402  ..}.|...|.....t.
-00000520: a00b 7c05 6408 1700 a101 0100 7c00 a009  ..|.d.......|...
-00000530: a100 0100 7408 6406 8301 0100 6e0a 7402  ....t.d.....n.t.
-00000540: a00e 6409 a101 0100 5700 713e 0400 740f  ..d.....W.q>..t.
-00000550: 9001 7924 0100 0100 0100 7402 a00e 6409  ..y$......t...d.
-00000560: a101 0100 5900 713e 3000 713e 640a 5300  ....Y.q>0.q>d.S.
-00000570: 290b 759f 0000 000a 2020 2020 2020 2020  ).u.....        
-00000580: 746c 2061 6e6e 6f74 6174 696f 6e20 7374  tl annotation st
-00000590: 6172 74ef bc9a e4bc 9ae4 bba5 e4ba a4e4  art.............
-000005a0: ba92 e5bc 8fe8 bf9b e8a1 8ce6 938d e4bd  ................
-000005b0: 9cef bc8c e5af b9e6 8c87 e5ae 9ae7 9a84  ................
-000005c0: e6a8 a1e5 9d97 e689 a7e8 a18c e68f 8fe8  ................
-000005d0: bfb0 e696 87e4 bbb6 28e5 8c85 e68b ace8  ........(.......
-000005e0: b7af e794 b1ef bc8c 6170 69e4 baa4 e4ba  ........api.....
-000005f0: 9229 e794 9fe6 8890 e592 8ce8 87aa e58a  .)..............
-00000600: a8e6 b3a8 e586 8ce9 80bb e8be 910a 2020  ..............  
-00000610: 2020 2020 2020 752e 0000 00e6 a380 e6b5        u.........
-00000620: 8be5 88b0 e4bb a5e4 b88b e6a8 a1e5 9d97  ................
-00000630: e58f afe7 949f e688 90e6 8f8f e8bf b0e6  ................
-00000640: 9687 e4bb b6ef bc9a 0a7a 023a 2075 5f00  .........z.: u_.
-00000650: 0000 e8af b7e8 be93 e585 a5e9 9c80 e8a6  ................
-00000660: 81e7 949f e688 90e6 8f8f e8bf b0e6 9687  ................
-00000670: e4bb b6e7 9a84 e6a8 a1e5 9d97 e590 8de6  ................
-00000680: 8896 e585 b6e4 b88b e6a0 8728 696e 7075  ...........(inpu
-00000690: 7420 2120 e980 80e5 87ba efbc 8c61 6c6c  t ! .........all
-000006a0: 20e8 87aa e58a a8e6 b3a8 e586 8c29 efbc   ............)..
-000006b0: 9afa 0121 7503 0000 00ef bc81 7201 0000  ...!u.......r...
-000006c0: 00da 0361 6c6c 7518 0000 00e6 8f8f e8bf  ...allu.........
-000006d0: b0e6 9687 e4bb b6e7 949f e688 90e5 ae8c  ................
-000006e0: e688 9075 1e00 0000 e8be 93e5 85a5 e69c  ...u............
-000006f0: 89e8 afaf efbc 8ce8 afb7 e987 8de6 96b0  ................
-00000700: e8be 93e5 85a5 4e29 1072 0800 0000 da0c  ......N).r......
-00000710: 676f 496e 5368 656c 6c44 6972 7207 0000  goInShellDirr...
-00000720: 00da 0373 7472 da09 656e 756d 6572 6174  ...str..enumerat
-00000730: 6572 1100 0000 da05 7072 696e 74da 0569  er......print..i
-00000740: 6e70 7574 da04 6578 6974 da1c 5f41 6e6e  nput..exit.._Ann
-00000750: 6f74 6174 696f 6e5f 5f69 6e74 6567 7261  otation__integra
-00000760: 7465 5f73 6865 6c6c da19 5f41 6e6e 6f74  te_shell.._Annot
-00000770: 6174 696f 6e5f 5f67 656e 6572 6174 6543  ation__generateC
-00000780: 6f64 6572 0c00 0000 da03 696e 74da 036c  oder......int..l
-00000790: 656e da07 7761 726e 696e 67da 0a56 616c  en..warning..Val
-000007a0: 7565 4572 726f 7229 0672 1600 0000 da05  ueError).r......
-000007b0: 696e 6465 78da 0469 7465 6dda 0b6d 6f64  index..item..mod
-000007c0: 756c 655f 6e61 6d65 da01 695a 0c5f 6d6f  ule_name..iZ._mo
-000007d0: 6475 6c65 5f61 6e6d 6572 1700 0000 7217  dule_anmer....r.
-000007e0: 0000 0072 1800 0000 da05 7374 6172 7419  ...r......start.
-000007f0: 0000 0073 3600 0000 0004 0802 0a01 1201  ...s6...........
-00000800: 1401 0602 0801 1001 0a01 0801 0801 0a01  ................
-00000810: 0a01 0a01 0e01 0801 0a02 0201 0801 0e01  ................
-00000820: 0a01 0a01 0e01 0801 0a02 0e01 0e01 7a10  ..............z.
-00000830: 416e 6e6f 7461 7469 6f6e 2e73 7461 7274  Annotation.start
-00000840: 2901 da0c 7461 7267 6574 4d6f 6475 6c65  )...targetModule
-00000850: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000860: 0006 0000 0043 0000 0073 8600 0000 7400  .....C...s....t.
-00000870: a001 7c01 6401 1700 a101 0100 7c00 6a02  ..|.d.......|.j.
-00000880: 4400 5d6c 7d02 7c02 6a03 7c01 6b02 7214  D.]l}.|.j.|.k.r.
-00000890: 7c02 6a04 6402 6b02 7270 7405 a006 a100  |.j.d.k.rpt.....
-000008a0: 0100 7c00 a007 7c02 6a08 a101 725e 7405  ..|...|.j...r^t.
-000008b0: a006 a100 0100 7409 a00a 7c02 6a08 a101  ......t...|.j...
-000008c0: 0100 7c00 a00b a100 0100 7180 7400 a00c  ..|.......q.t...
-000008d0: 6403 a00d 7c01 a101 a101 0100 7114 7400  d...|.......q.t.
-000008e0: a00c 6404 a00d 7c01 a101 a101 0100 7114  ..d...|.......q.
-000008f0: 6400 5300 2905 4e75 2200 0000 20e6 a8a1  d.S.).Nu"... ...
-00000900: e59d 97e7 949f e688 90e6 b3a8 e8a7 a3e6  ................
-00000910: 8f8f e8bf b0e6 9687 e4bb b62e 2e2e 4675  ..............Fu
-00000920: 5400 0000 e8af b7e7 a1ae e4bf 9de6 a8a1  T...............
-00000930: e59d 977b 307d e5b7 b2e4 be9d e8b5 9662  ...{0}.........b
-00000940: 7569 6c64 5f72 756e 6e65 72ef bc8c e58f  uild_runner.....
-00000950: afe5 8f82 e880 83e5 85b6 e4bb 96e6 a8a1  ................
-00000960: e59d 97e8 bf9b e8a1 8ce4 be9d e8b5 96e9  ................
-00000970: 858d e7bd aee2 9d8c 754b 0000 00e6 a380  ........uK......
-00000980: e6b5 8be5 88b0 e6a8 a1e5 9d97 7b30 7de5  ............{0}.
-00000990: bd93 e589 8de6 98af e8bf 9ce7 a88b e4be  ................
-000009a0: 9de8 b596 efbc 8ce6 97a0 e6b3 95e7 949f  ................
-000009b0: e688 90e8 b7af e794 b1e6 8f8f e8bf b0e6  ................
-000009c0: 9687 e4bb b6e2 9d8c 290e 7207 0000 0072  ........).r....r
-000009d0: 0c00 0000 7214 0000 00da 0b70 6163 6b61  ....r......packa
-000009e0: 6765 4e61 6d65 5a08 6973 5265 6d6f 7465  geNameZ.isRemote
-000009f0: 7208 0000 0072 1c00 0000 da27 5f41 6e6e  r....r.....'_Ann
-00000a00: 6f74 6174 696f 6e5f 5f6a 7564 6765 4861  otation__judgeHa
-00000a10: 7342 7569 6c64 5275 6e6e 6572 5061 636b  sBuildRunnerPack
-00000a20: 6167 655a 0b70 6163 6b61 6765 5061 7468  ageZ.packagePath
-00000a30: da02 6f73 da05 6368 6469 72da 1a5f 416e  ..os..chdir.._An
-00000a40: 6e6f 7461 7469 6f6e 5f5f 6765 6e65 7261  notation__genera
-00000a50: 746f 7246 756e 6372 1d00 0000 da06 666f  torFuncr......fo
-00000a60: 726d 6174 2903 7216 0000 0072 2d00 0000  rmat).r....r-...
-00000a70: 7229 0000 0072 1700 0000 7217 0000 0072  r)...r....r....r
-00000a80: 1800 0000 5a0e 5f5f 6765 6e65 7261 7465  ....Z.__generate
-00000a90: 436f 6465 3e00 0000 7322 0000 0000 010e  Code>...s"......
-00000aa0: 010a 010a 010a 0108 010c 0108 010c 010a  ................
-00000ab0: 0204 0104 0102 ff02 ff06 0604 0108 ff7a  ...............z
-00000ac0: 1941 6e6e 6f74 6174 696f 6e2e 5f5f 6765  .Annotation.__ge
-00000ad0: 6e65 7261 7465 436f 6465 6301 0000 0000  nerateCodec.....
-00000ae0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000af0: 0000 0073 1800 0000 7400 a001 6401 a101  ...s....t...d...
-00000b00: 0100 7400 a001 6402 a101 0100 6400 5300  ..t...d.....d.S.
-00000b10: 2903 4e7a 2b66 6c75 7474 6572 2070 6163  ).Nz+flutter pac
-00000b20: 6b61 6765 7320 7075 6220 7275 6e20 6275  kages pub run bu
-00000b30: 696c 645f 7275 6e6e 6572 2063 6c65 616e  ild_runner clean
-00000b40: 7a48 666c 7574 7465 7220 7061 636b 6167  zHflutter packag
-00000b50: 6573 2070 7562 2072 756e 2062 7569 6c64  es pub run build
-00000b60: 5f72 756e 6e65 7220 6275 696c 6420 2d2d  _runner build --
-00000b70: 6465 6c65 7465 2d63 6f6e 666c 6963 7469  delete-conflicti
-00000b80: 6e67 2d6f 7574 7075 7473 2902 7230 0000  ng-outputs).r0..
-00000b90: 00da 0673 7973 7465 6d72 1500 0000 7217  ...systemr....r.
-00000ba0: 0000 0072 1700 0000 7218 0000 005a 0f5f  ...r....r....Z._
-00000bb0: 5f67 656e 6572 6174 6f72 4675 6e63 5300  _generatorFuncS.
-00000bc0: 0000 7308 0000 0000 010a 0104 0102 ff7a  ..s............z
-00000bd0: 1a41 6e6e 6f74 6174 696f 6e2e 5f5f 6765  .Annotation.__ge
-00000be0: 6e65 7261 746f 7246 756e 6329 02da 0e70  neratorFunc)...p
-00000bf0: 6163 6b61 6765 4c69 6250 6174 68da 0672  ackageLibPath..r
-00000c00: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-00000c10: 0000 0500 0000 0400 0000 4300 0000 733e  ..........C...s>
-00000c20: 0000 0074 00a0 017c 01a1 0101 0074 0274  ...t...|.....t.t
-00000c30: 00a0 03a1 0064 0164 028d 027d 0264 017d  .....d.d...}.d.}
-00000c40: 037c 026a 0444 005d 147d 047c 046a 057c  .|.j.D.].}.|.j.|
-00000c50: 006a 066b 0272 2464 037d 0371 247c 0353  .j.k.r$d.}.q$|.S
-00000c60: 0029 044e 4629 015a 0d66 696c 7465 725f  .).NF).Z.filter_
-00000c70: 6279 5f74 6466 5429 0772 3000 0000 7231  by_tdfT).r0...r1
-00000c80: 0000 0072 0600 0000 da06 6765 7463 7764  ...r......getcwd
-00000c90: 7213 0000 0072 2e00 0000 720d 0000 0029  r....r....r....)
-00000ca0: 0572 1600 0000 7235 0000 005a 1170 6163  .r....r5...Z.pac
-00000cb0: 6b61 6765 4a73 6f6e 436f 6e66 6967 5a0e  kageJsonConfigZ.
-00000cc0: 6861 7342 7569 6c64 5275 6e6e 6572 7229  hasBuildRunnerr)
-00000cd0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000ce0: 0000 5a1c 5f5f 6a75 6467 6548 6173 4275  ..Z.__judgeHasBu
-00000cf0: 696c 6452 756e 6e65 7250 6163 6b61 6765  ildRunnerPackage
-00000d00: 5a00 0000 7312 0000 0000 010a 0102 0108  Z...s...........
-00000d10: ff06 0304 010a 010c 0106 027a 2741 6e6e  ...........z'Ann
-00000d20: 6f74 6174 696f 6e2e 5f5f 6a75 6467 6548  otation.__judgeH
-00000d30: 6173 4275 696c 6452 756e 6e65 7250 6163  asBuildRunnerPac
-00000d40: 6b61 6765 6301 0000 0000 0000 0000 0000  kagec...........
-00000d50: 0001 0000 0003 0000 0043 0000 0073 2200  .........C...s".
-00000d60: 0000 7c00 6a00 a001 a100 0100 7c00 6a02  ..|.j.......|.j.
-00000d70: a001 a100 0100 7403 a004 6401 a101 0100  ......t...d.....
-00000d80: 6400 5300 2902 4e75 0c00 0000 e695 b4e5  d.S.).Nu........
-00000d90: 9088 e5ae 8ce6 8890 2905 720e 0000 005a  ........).r....Z
-00000da0: 0f69 6e74 6567 7261 7465 5f73 6865 6c6c  .integrate_shell
-00000db0: 720f 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
-00000dc0: 1500 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000dd0: 0000 005a 115f 5f69 6e74 6567 7261 7465  ...Z.__integrate
-00000de0: 5f73 6865 6c6c 6700 0000 7306 0000 0000  _shellg...s.....
-00000df0: 010a 010a 017a 1c41 6e6e 6f74 6174 696f  .....z.Annotatio
-00000e00: 6e2e 5f5f 696e 7465 6772 6174 655f 7368  n.__integrate_sh
-00000e10: 656c 6c63 0100 0000 0000 0000 0000 0000  ellc............
-00000e20: 0500 0000 0400 0000 4300 0000 7360 0000  ........C...s`..
-00000e30: 0074 0083 007d 0167 007d 0274 0183 006a  .t...}.g.}.t...j
-00000e40: 0244 005d 487d 037c 01a0 037c 03a1 017d  .D.]H}.|...|...}
-00000e50: 047c 046a 0474 056a 066b 0273 507c 046a  .|.j.t.j.k.sP|.j
-00000e60: 0474 056a 076b 0273 507c 046a 0474 056a  .t.j.k.sP|.j.t.j
-00000e70: 086b 0273 507c 046a 0474 056a 096b 0272  .k.sP|.j.t.j.k.r
-00000e80: 127c 02a0 0a7c 03a1 0101 0071 127c 0253  .|...|.....q.|.S
-00000e90: 0029 014e 290b 7204 0000 0072 0200 0000  .).N).r....r....
-00000ea0: da0e 6d6f 6475 6c65 4e61 6d65 4c69 7374  ..moduleNameList
-00000eb0: da08 6765 745f 6974 656d da04 7479 7065  ..get_item..type
-00000ec0: 7203 0000 00da 034c 6962 da03 4170 69da  r......Lib..Api.
-00000ed0: 064d 6f64 756c 65da 0650 6c75 6769 6eda  .Module..Plugin.
-00000ee0: 0661 7070 656e 6429 0572 1600 0000 5a1a  .append).r....Z.
-00000ef0: 5f41 6e6e 6f74 6174 696f 6e5f 5f6d 6f64  _Annotation__mod
-00000f00: 756c 655f 636f 6e66 6967 5a11 5f41 6e6e  ule_configZ._Ann
-00000f10: 6f74 6174 696f 6e5f 5f6c 6973 7472 2900  otation__listr).
-00000f20: 0000 5a0a 636f 6669 675f 6974 656d 7217  ..Z.cofig_itemr.
-00000f30: 0000 0072 1700 0000 7218 0000 005a 185f  ...r....r....Z._
-00000f40: 5f61 7069 5f62 7573 696e 6573 734d 6f64  _api_businessMod
-00000f50: 756c 654c 6973 746c 0000 0073 1c00 0000  uleListl...s....
-00000f60: 0001 0601 0401 0c01 0a02 0aff 0202 0afe  ................
-00000f70: 0203 0afd 0204 0afc 0206 0c01 7a23 416e  ............z#An
-00000f80: 6e6f 7461 7469 6f6e 2e5f 5f61 7069 5f62  notation.__api_b
-00000f90: 7573 696e 6573 734d 6f64 756c 654c 6973  usinessModuleLis
-00000fa0: 744e 290d da08 5f5f 6e61 6d65 5f5f da0a  tN)...__name__..
-00000fb0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000fc0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00000fd0: 5f72 1900 0000 722c 0000 0072 1d00 0000  _r....r,...r....
-00000fe0: 7223 0000 0072 3200 0000 da04 626f 6f6c  r#...r2.....bool
-00000ff0: 722f 0000 0072 2200 0000 7210 0000 0072  r/...r"...r....r
-00001000: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00001010: 0000 0072 0b00 0000 0b00 0000 7310 0000  ...r........s...
-00001020: 0008 0104 0408 0908 250e 1508 0710 0d08  ........%.......
-00001030: 0572 0b00 0000 2912 7230 0000 00da 2974  .r....).r0....)t
-00001040: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 636f  df_tool.tools.co
-00001050: 6e66 6967 2e69 6e69 7469 616c 5f6a 736f  nfig.initial_jso
-00001060: 6e5f 636f 6e66 6967 7202 0000 00da 2874  n_configr.....(t
-00001070: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 636f  df_tool.tools.co
-00001080: 6e66 6967 2e6d 6f64 756c 655f 6a73 6f6e  nfig.module_json
-00001090: 5f63 6f6e 6669 6772 0300 0000 7204 0000  _configr....r...
-000010a0: 005a 2574 6466 5f74 6f6f 6c2e 746f 6f6c  .Z%tdf_tool.tool
-000010b0: 732e 636f 6e66 6967 2e70 6163 6b61 6765  s.config.package
-000010c0: 735f 636f 6e66 6967 7205 0000 0072 0600  s_configr....r..
-000010d0: 0000 da14 7464 665f 746f 6f6c 2e74 6f6f  ....tdf_tool.too
-000010e0: 6c73 2e70 7269 6e74 7207 0000 00da 1874  ls.printr......t
-000010f0: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 7368  df_tool.tools.sh
-00001100: 656c 6c5f 6469 7272 0800 0000 5a19 7464  ell_dirr....Z.td
-00001110: 665f 746f 6f6c 2e70 6970 656c 696e 6573  f_tool.pipelines
-00001120: 2e72 6f75 7465 7272 0900 0000 5a22 7464  .routerr....Z"td
-00001130: 665f 746f 6f6c 2e70 6970 656c 696e 6573  f_tool.pipelines
-00001140: 2e61 7069 5f69 6e74 6572 6163 7469 6f6e  .api_interaction
-00001150: 720a 0000 0072 0b00 0000 7217 0000 0072  r....r....r....r
-00001160: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-00001170: 3c6d 6f64 756c 653e 0100 0000 7310 0000  <module>....s...
-00001180: 0008 010c 0110 0110 010c 010c 020c 010c  ................
-00001190: 02                                       .
+00000070: 6406 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
+00000080: 6407 6c0e 6d0f 5a0f 0100 6400 6408 6c10  d.l.m.Z...d.d.l.
+00000090: 6d11 5a11 0100 4700 6409 640a 8400 640a  m.Z...G.d.d...d.
+000000a0: 8302 5a12 6401 5300 290b e900 0000 004e  ..Z.d.S.)......N
+000000b0: 2901 da11 496e 6974 6961 6c4a 736f 6e43  )...InitialJsonC
+000000c0: 6f6e 6669 6729 02da 0e4d 6f64 756c 6549  onfig)...ModuleI
+000000d0: 7465 6d54 7970 65da 104d 6f64 756c 654a  temType..ModuleJ
+000000e0: 736f 6e43 6f6e 6669 6729 02da 0b50 6163  sonConfig)...Pac
+000000f0: 6b61 6765 4e6f 6465 da12 5061 636b 6167  kageNode..Packag
+00000100: 6573 4a73 6f6e 436f 6e66 6967 2901 da05  esJsonConfig)...
+00000110: 5072 696e 7429 02da 0853 6865 6c6c 4469  Print)...ShellDi
+00000120: 72da 0b50 726f 6a65 6374 5479 7065 2901  r..ProjectType).
+00000130: da06 526f 7574 6572 2901 da0d 4170 6941  ..Router)...ApiA
+00000140: 6e6e 6f74 6174 696f 6e63 0000 0000 0000  nnotationc......
+00000150: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000160: 0000 7356 0000 0065 005a 0164 005a 0264  ..sV...e.Z.d.Z.d
+00000170: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
+00000180: 005a 0565 0664 069c 0164 0764 0884 045a  .Z.e.d...d.d...Z
+00000190: 0764 0964 0a84 005a 0865 0665 0964 0b9c  .d.d...Z.e.e.d..
+000001a0: 0264 0c64 0d84 045a 0a64 0e64 0f84 005a  .d.d...Z.d.d...Z
+000001b0: 0b64 1064 1184 005a 0c64 1253 0029 13da  .d.d...Z.d.S.)..
+000001c0: 0a41 6e6e 6f74 6174 696f 6e75 4500 0000  .AnnotationuE...
+000001d0: 0a20 2020 20e6 a8a1 e59d 97e9 97b4 e694  .    ...........
+000001e0: afe6 8c81 e79b b8e5 85b3 e591 bde4 bba4  ................
+000001f0: efbc 9a74 6c20 616e 6e6f 7461 7469 6f6e  ...tl annotation
+00000200: 202d 6820 e69f a5e7 9c8b e8af a6e6 8385   -h ............
+00000210: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
+00000220: 0000 0100 0000 0300 0000 4300 0000 734c  ..........C...sL
+00000230: 0000 0074 00a0 0164 01a1 0101 0074 02a0  ...t...d.....t..
+00000240: 03a1 0074 046a 056b 0272 4864 027c 005f  ...t.j.k.rHd.|._
+00000250: 0674 0783 007c 005f 0874 0983 007c 005f  .t...|._.t...|._
+00000260: 0a7c 00a0 0ba1 007c 005f 0c74 0d74 02a0  .|.....|._.t.t..
+00000270: 0ea1 0083 016a 0f7c 005f 1064 0053 0029  .....j.|._.d.S.)
+00000280: 034e 750c 0000 00e6 a380 e6b5 8be4 b8ad  .Nu.............
+00000290: 2e2e 2e5a 0c62 7569 6c64 5f72 756e 6e65  ...Z.build_runne
+000002a0: 7229 1172 0700 0000 da05 7469 746c 6572  r).r......titler
+000002b0: 0800 0000 da0e 6765 7450 726f 6a65 6374  ......getProject
+000002c0: 5479 7065 7209 0000 00da 0746 4c55 5454  Typer......FLUTT
+000002d0: 4552 da1c 5f41 6e6e 6f74 6174 696f 6e5f  ER.._Annotation_
+000002e0: 5f62 7569 6c64 5275 6e6e 6572 4e61 6d65  _buildRunnerName
+000002f0: 720a 0000 00da 1d5f 416e 6e6f 7461 7469  r......_Annotati
+00000300: 6f6e 5f5f 726f 7574 6572 416e 6e6f 7461  on__routerAnnota
+00000310: 7469 6f6e 720b 0000 00da 1a5f 416e 6e6f  tionr......_Anno
+00000320: 7461 7469 6f6e 5f5f 6170 6941 6e6e 6f74  tation__apiAnnot
+00000330: 6174 696f 6eda 235f 416e 6e6f 7461 7469  ation.#_Annotati
+00000340: 6f6e 5f5f 6170 695f 6275 7369 6e65 7373  on__api_business
+00000350: 4d6f 6475 6c65 4c69 7374 da1f 5f41 6e6e  ModuleList.._Ann
+00000360: 6f74 6174 696f 6e5f 5f62 7573 696e 6573  otation__busines
+00000370: 734d 6f64 756c 654c 6973 7472 0600 0000  sModuleListr....
+00000380: da0b 6765 7453 6865 6c6c 4469 72da 0870  ..getShellDir..p
+00000390: 6163 6b61 6765 73da 195f 416e 6e6f 7461  ackages.._Annota
+000003a0: 7469 6f6e 5f5f 7061 636b 6167 6573 4c69  tion__packagesLi
+000003b0: 7374 a901 da04 7365 6c66 a900 721a 0000  st....self..r...
+000003c0: 00f5 6900 0000 2f55 7365 7273 2f78 756a  ..i.../Users/xuj
+000003d0: 6961 6e2f 446f 6375 6d65 6e74 732f 3230  ian/Documents/20
+000003e0: 3234 2fe6 a8a1 e59d 97e9 97b4 e4ba a4e4  24/.............
+000003f0: ba92 e9a1 b9e7 9bae 746c e58d 87e7 baa7  ........tl......
+00000400: 2f70 6163 6b61 6765 5f74 6f6f 6c73 2f74  /package_tools/t
+00000410: 6466 5f74 6f6f 6c2f 7069 7065 6c69 6e65  df_tool/pipeline
+00000420: 732f 616e 6e6f 7461 7469 6f6e 2e70 79da  s/annotation.py.
+00000430: 085f 5f69 6e69 745f 5f10 0000 0073 0e00  .__init__....s..
+00000440: 0000 0001 0a01 0e01 0601 0801 0801 0a01  ................
+00000450: 7a13 416e 6e6f 7461 7469 6f6e 2e5f 5f69  z.Annotation.__i
+00000460: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000470: 0000 0600 0000 0800 0000 4300 0000 732c  ..........C...s,
+00000480: 0100 0074 00a0 01a1 0001 0074 02a0 0364  ...t.......t...d
+00000490: 01a1 0101 0074 047c 006a 0583 0144 005d  .....t.|.j...D.]
+000004a0: 1a5c 027d 017d 0274 067c 019b 0064 027c  .\.}.}.t.|...d.|
+000004b0: 029b 009d 0383 0101 0071 1c74 0683 0001  .........q.t....
+000004c0: 0074 0764 0383 017d 037c 0364 046b 0273  .t.d...}.|.d.k.s
+000004d0: 567c 0364 056b 0272 6074 0864 0683 0101  V|.d.k.r`t.d....
+000004e0: 0071 3e7c 0364 076b 0272 7a7c 00a0 09a1  .q>|.d.k.rz|....
+000004f0: 0001 0074 0864 0683 0101 0071 3e7c 037c  ...t.d.....q>|.|
+00000500: 006a 0576 0072 ae7c 00a0 0a7c 03a1 0101  .j.v.r.|...|....
+00000510: 0074 02a0 0b7c 0364 0817 00a1 0101 007c  .t...|.d.......|
+00000520: 00a0 09a1 0001 0074 0864 0683 0101 0071  .......t.d.....q
+00000530: 3e7a 5874 0c7c 0383 017d 047c 0474 0d7c  >zXt.|...}.|.t.|
+00000540: 006a 0583 016b 0072 fa7c 006a 057c 0419  .j...k.r.|.j.|..
+00000550: 007d 057c 00a0 0a7c 05a1 0101 0074 02a0  .}.|...|.....t..
+00000560: 0b7c 0564 0817 00a1 0101 007c 00a0 09a1  .|.d.......|....
+00000570: 0001 0074 0864 0683 0101 006e 0a74 02a0  ...t.d.....n.t..
+00000580: 0e64 09a1 0101 0057 0071 3e04 0074 0f90  .d.....W.q>..t..
+00000590: 0179 2401 0001 0001 0074 02a0 0e64 09a1  .y$......t...d..
+000005a0: 0101 0059 0071 3e30 0071 3e64 0a53 0029  ...Y.q>0.q>d.S.)
+000005b0: 0b75 9f00 0000 0a20 2020 2020 2020 2074  .u.....        t
+000005c0: 6c20 616e 6e6f 7461 7469 6f6e 2073 7461  l annotation sta
+000005d0: 7274 efbc 9ae4 bc9a e4bb a5e4 baa4 e4ba  rt..............
+000005e0: 92e5 bc8f e8bf 9be8 a18c e693 8de4 bd9c  ................
+000005f0: efbc 8ce5 afb9 e68c 87e5 ae9a e79a 84e6  ................
+00000600: a8a1 e59d 97e6 89a7 e8a1 8ce6 8f8f e8bf  ................
+00000610: b0e6 9687 e4bb b628 e58c 85e6 8bac e8b7  .......(........
+00000620: afe7 94b1 efbc 8c61 7069 e4ba a4e4 ba92  .......api......
+00000630: 29e7 949f e688 90e5 928c e887 aae5 8aa8  )...............
+00000640: e6b3 a8e5 868c e980 bbe8 be91 0a20 2020  .............   
+00000650: 2020 2020 2075 2e00 0000 e6a3 80e6 b58b       u..........
+00000660: e588 b0e4 bba5 e4b8 8be6 a8a1 e59d 97e5  ................
+00000670: 8faf e794 9fe6 8890 e68f 8fe8 bfb0 e696  ................
+00000680: 87e4 bbb6 efbc 9a0a 7a02 3a20 755f 0000  ........z.: u_..
+00000690: 00e8 afb7 e8be 93e5 85a5 e99c 80e8 a681  ................
+000006a0: e794 9fe6 8890 e68f 8fe8 bfb0 e696 87e4  ................
+000006b0: bbb6 e79a 84e6 a8a1 e59d 97e5 908d e688  ................
+000006c0: 96e5 85b6 e4b8 8be6 a087 2869 6e70 7574  ..........(input
+000006d0: 2021 20e9 8080 e587 baef bc8c 616c 6c20   ! .........all 
+000006e0: e887 aae5 8aa8 e6b3 a8e5 868c 29ef bc9a  ............)...
+000006f0: fa01 2175 0300 0000 efbc 8172 0100 0000  ..!u.......r....
+00000700: da03 616c 6c75 1800 0000 e68f 8fe8 bfb0  ..allu..........
+00000710: e696 87e4 bbb6 e794 9fe6 8890 e5ae 8ce6  ................
+00000720: 8890 751e 0000 00e8 be93 e585 a5e6 9c89  ..u.............
+00000730: e8af afef bc8c e8af b7e9 878d e696 b0e8  ................
+00000740: be93 e585 a54e 2910 7208 0000 00da 0c67  .....N).r......g
+00000750: 6f49 6e53 6865 6c6c 4469 7272 0700 0000  oInShellDirr....
+00000760: da03 7374 72da 0965 6e75 6d65 7261 7465  ..str..enumerate
+00000770: 7214 0000 00da 0570 7269 6e74 da05 696e  r......print..in
+00000780: 7075 74da 0465 7869 74da 0969 6e74 6567  put..exit..integ
+00000790: 7261 7465 da19 5f41 6e6e 6f74 6174 696f  rate.._Annotatio
+000007a0: 6e5f 5f67 656e 6572 6174 6543 6f64 6572  n__generateCoder
+000007b0: 0d00 0000 da03 696e 74da 036c 656e da07  ......int..len..
+000007c0: 7761 726e 696e 67da 0a56 616c 7565 4572  warning..ValueEr
+000007d0: 726f 7229 0672 1900 0000 da05 696e 6465  ror).r......inde
+000007e0: 78da 0469 7465 6dda 0b6d 6f64 756c 655f  x..item..module_
+000007f0: 6e61 6d65 da01 695a 0c5f 6d6f 6475 6c65  name..iZ._module
+00000800: 5f61 6e6d 6572 1a00 0000 721a 0000 0072  _anmer....r....r
+00000810: 1b00 0000 da05 7374 6172 7419 0000 0073  ......start....s
+00000820: 3600 0000 0004 0802 0a01 1201 1401 0602  6...............
+00000830: 0801 1001 0a01 0801 0801 0a01 0a01 0a01  ................
+00000840: 0e01 0801 0a02 0201 0801 0e01 0a01 0a01  ................
+00000850: 0e01 0801 0a02 0e01 0e01 7a10 416e 6e6f  ..........z.Anno
+00000860: 7461 7469 6f6e 2e73 7461 7274 2901 da0c  tation.start)...
+00000870: 7461 7267 6574 4d6f 6475 6c65 6302 0000  targetModulec...
+00000880: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+00000890: 0043 0000 0073 8600 0000 7400 a001 7c01  .C...s....t...|.
+000008a0: 6401 1700 a101 0100 7c00 6a02 4400 5d6c  d.......|.j.D.]l
+000008b0: 7d02 7c02 6a03 7c01 6b02 7214 7c02 6a04  }.|.j.|.k.r.|.j.
+000008c0: 6402 6b02 7270 7405 a006 a100 0100 7c00  d.k.rpt.......|.
+000008d0: a007 7c02 6a08 a101 725e 7405 a006 a100  ..|.j...r^t.....
+000008e0: 0100 7409 a00a 7c02 6a08 a101 0100 7c00  ..t...|.j.....|.
+000008f0: a00b a100 0100 7180 7400 a00c 6403 a00d  ......q.t...d...
+00000900: 7c01 a101 a101 0100 7114 7400 a00c 6404  |.......q.t...d.
+00000910: a00d 7c01 a101 a101 0100 7114 6400 5300  ..|.......q.d.S.
+00000920: 2905 4e75 2200 0000 20e6 a8a1 e59d 97e7  ).Nu"... .......
+00000930: 949f e688 90e6 b3a8 e8a7 a3e6 8f8f e8bf  ................
+00000940: b0e6 9687 e4bb b62e 2e2e 4675 5400 0000  ..........FuT...
+00000950: e8af b7e7 a1ae e4bf 9de6 a8a1 e59d 977b  ...............{
+00000960: 307d e5b7 b2e4 be9d e8b5 9662 7569 6c64  0}.........build
+00000970: 5f72 756e 6e65 72ef bc8c e58f afe5 8f82  _runner.........
+00000980: e880 83e5 85b6 e4bb 96e6 a8a1 e59d 97e8  ................
+00000990: bf9b e8a1 8ce4 be9d e8b5 96e9 858d e7bd  ................
+000009a0: aee2 9d8c 754b 0000 00e6 a380 e6b5 8be5  ....uK..........
+000009b0: 88b0 e6a8 a1e5 9d97 7b30 7de5 bd93 e589  ........{0}.....
+000009c0: 8de6 98af e8bf 9ce7 a88b e4be 9de8 b596  ................
+000009d0: efbc 8ce6 97a0 e6b3 95e7 949f e688 90e8  ................
+000009e0: b7af e794 b1e6 8f8f e8bf b0e6 9687 e4bb  ................
+000009f0: b6e2 9d8c 290e 7207 0000 0072 0d00 0000  ....).r....r....
+00000a00: 7217 0000 00da 0b70 6163 6b61 6765 4e61  r......packageNa
+00000a10: 6d65 5a08 6973 5265 6d6f 7465 7208 0000  meZ.isRemoter...
+00000a20: 0072 1f00 0000 da27 5f41 6e6e 6f74 6174  .r.....'_Annotat
+00000a30: 696f 6e5f 5f6a 7564 6765 4861 7342 7569  ion__judgeHasBui
+00000a40: 6c64 5275 6e6e 6572 5061 636b 6167 655a  ldRunnerPackageZ
+00000a50: 0b70 6163 6b61 6765 5061 7468 da02 6f73  .packagePath..os
+00000a60: da05 6368 6469 72da 1a5f 416e 6e6f 7461  ..chdir.._Annota
+00000a70: 7469 6f6e 5f5f 6765 6e65 7261 746f 7246  tion__generatorF
+00000a80: 756e 6372 2000 0000 da06 666f 726d 6174  uncr .....format
+00000a90: 2903 7219 0000 0072 3000 0000 722c 0000  ).r....r0...r,..
+00000aa0: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00000ab0: 5a0e 5f5f 6765 6e65 7261 7465 436f 6465  Z.__generateCode
+00000ac0: 3e00 0000 7322 0000 0000 010e 010a 010a  >...s"..........
+00000ad0: 010a 0108 010c 0108 010c 010a 0204 0104  ................
+00000ae0: 0102 ff02 ff06 0604 0108 ff7a 1941 6e6e  ...........z.Ann
+00000af0: 6f74 6174 696f 6e2e 5f5f 6765 6e65 7261  otation.__genera
+00000b00: 7465 436f 6465 6301 0000 0000 0000 0000  teCodec.........
+00000b10: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000b20: 1800 0000 7400 a001 6401 a101 0100 7400  ....t...d.....t.
+00000b30: a001 6402 a101 0100 6400 5300 2903 4e7a  ..d.....d.S.).Nz
+00000b40: 2b66 6c75 7474 6572 2070 6163 6b61 6765  +flutter package
+00000b50: 7320 7075 6220 7275 6e20 6275 696c 645f  s pub run build_
+00000b60: 7275 6e6e 6572 2063 6c65 616e 7a48 666c  runner cleanzHfl
+00000b70: 7574 7465 7220 7061 636b 6167 6573 2070  utter packages p
+00000b80: 7562 2072 756e 2062 7569 6c64 5f72 756e  ub run build_run
+00000b90: 6e65 7220 6275 696c 6420 2d2d 6465 6c65  ner build --dele
+00000ba0: 7465 2d63 6f6e 666c 6963 7469 6e67 2d6f  te-conflicting-o
+00000bb0: 7574 7075 7473 2902 7233 0000 00da 0673  utputs).r3.....s
+00000bc0: 7973 7465 6d72 1800 0000 721a 0000 0072  ystemr....r....r
+00000bd0: 1a00 0000 721b 0000 005a 0f5f 5f67 656e  ....r....Z.__gen
+00000be0: 6572 6174 6f72 4675 6e63 5300 0000 7308  eratorFuncS...s.
+00000bf0: 0000 0000 010a 0104 0102 ff7a 1a41 6e6e  ...........z.Ann
+00000c00: 6f74 6174 696f 6e2e 5f5f 6765 6e65 7261  otation.__genera
+00000c10: 746f 7246 756e 6329 02da 0e70 6163 6b61  torFunc)...packa
+00000c20: 6765 4c69 6250 6174 68da 0672 6574 7572  geLibPath..retur
+00000c30: 6e63 0200 0000 0000 0000 0000 0000 0500  nc..............
+00000c40: 0000 0400 0000 4300 0000 733e 0000 0074  ......C...s>...t
+00000c50: 00a0 017c 01a1 0101 0074 0274 00a0 03a1  ...|.....t.t....
+00000c60: 0064 0164 028d 027d 0264 017d 037c 026a  .d.d...}.d.}.|.j
+00000c70: 0444 005d 147d 047c 046a 057c 006a 066b  .D.].}.|.j.|.j.k
+00000c80: 0272 2464 037d 0371 247c 0353 0029 044e  .r$d.}.q$|.S.).N
+00000c90: 4629 015a 0d66 696c 7465 725f 6279 5f74  F).Z.filter_by_t
+00000ca0: 6466 5429 0772 3300 0000 7234 0000 0072  dfT).r3...r4...r
+00000cb0: 0600 0000 da06 6765 7463 7764 7216 0000  ......getcwdr...
+00000cc0: 0072 3100 0000 7210 0000 0029 0572 1900  .r1...r....).r..
+00000cd0: 0000 7238 0000 005a 1170 6163 6b61 6765  ..r8...Z.package
+00000ce0: 4a73 6f6e 436f 6e66 6967 5a0e 6861 7342  JsonConfigZ.hasB
+00000cf0: 7569 6c64 5275 6e6e 6572 722c 0000 0072  uildRunnerr,...r
+00000d00: 1a00 0000 721a 0000 0072 1b00 0000 5a1c  ....r....r....Z.
+00000d10: 5f5f 6a75 6467 6548 6173 4275 696c 6452  __judgeHasBuildR
+00000d20: 756e 6e65 7250 6163 6b61 6765 5a00 0000  unnerPackageZ...
+00000d30: 7312 0000 0000 010a 0102 0108 ff06 0304  s...............
+00000d40: 010a 010c 0106 027a 2741 6e6e 6f74 6174  .......z'Annotat
+00000d50: 696f 6e2e 5f5f 6a75 6467 6548 6173 4275  ion.__judgeHasBu
+00000d60: 696c 6452 756e 6e65 7250 6163 6b61 6765  ildRunnerPackage
+00000d70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000d80: 0003 0000 0043 0000 0073 2200 0000 7c00  .....C...s"...|.
+00000d90: 6a00 a001 a100 0100 7c00 6a02 a001 a100  j.......|.j.....
+00000da0: 0100 7403 a004 6401 a101 0100 6400 5300  ..t...d.....d.S.
+00000db0: 2902 4e75 0c00 0000 e695 b4e5 9088 e5ae  ).Nu............
+00000dc0: 8ce6 8890 2905 7211 0000 005a 0f69 6e74  ....).r....Z.int
+00000dd0: 6567 7261 7465 5f73 6865 6c6c 7212 0000  egrate_shellr...
+00000de0: 0072 0700 0000 720d 0000 0072 1800 0000  .r....r....r....
+00000df0: 721a 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
+00000e00: 2500 0000 6700 0000 7306 0000 0000 010a  %...g...s.......
+00000e10: 010a 017a 1441 6e6e 6f74 6174 696f 6e2e  ...z.Annotation.
+00000e20: 696e 7465 6772 6174 6563 0100 0000 0000  integratec......
+00000e30: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00000e40: 0000 7360 0000 0074 0083 007d 0167 007d  ..s`...t...}.g.}
+00000e50: 0274 0183 006a 0244 005d 487d 037c 01a0  .t...j.D.]H}.|..
+00000e60: 037c 03a1 017d 047c 046a 0474 056a 066b  .|...}.|.j.t.j.k
+00000e70: 0273 507c 046a 0474 056a 076b 0273 507c  .sP|.j.t.j.k.sP|
+00000e80: 046a 0474 056a 086b 0273 507c 046a 0474  .j.t.j.k.sP|.j.t
+00000e90: 056a 096b 0272 127c 02a0 0a7c 03a1 0101  .j.k.r.|...|....
+00000ea0: 0071 127c 0253 0029 014e 290b 7204 0000  .q.|.S.).N).r...
+00000eb0: 0072 0200 0000 da0e 6d6f 6475 6c65 4e61  .r......moduleNa
+00000ec0: 6d65 4c69 7374 da08 6765 745f 6974 656d  meList..get_item
+00000ed0: da04 7479 7065 7203 0000 00da 034c 6962  ..typer......Lib
+00000ee0: da03 4170 69da 064d 6f64 756c 65da 0650  ..Api..Module..P
+00000ef0: 6c75 6769 6eda 0661 7070 656e 6429 0572  lugin..append).r
+00000f00: 1900 0000 5a1a 5f41 6e6e 6f74 6174 696f  ....Z._Annotatio
+00000f10: 6e5f 5f6d 6f64 756c 655f 636f 6e66 6967  n__module_config
+00000f20: 5a11 5f41 6e6e 6f74 6174 696f 6e5f 5f6c  Z._Annotation__l
+00000f30: 6973 7472 2c00 0000 5a0a 636f 6669 675f  istr,...Z.cofig_
+00000f40: 6974 656d 721a 0000 0072 1a00 0000 721b  itemr....r....r.
+00000f50: 0000 005a 185f 5f61 7069 5f62 7573 696e  ...Z.__api_busin
+00000f60: 6573 734d 6f64 756c 654c 6973 746c 0000  essModuleListl..
+00000f70: 0073 1c00 0000 0001 0601 0401 0c01 0a02  .s..............
+00000f80: 0aff 0202 0afe 0203 0afd 0204 0afc 0206  ................
+00000f90: 0c01 7a23 416e 6e6f 7461 7469 6f6e 2e5f  ..z#Annotation._
+00000fa0: 5f61 7069 5f62 7573 696e 6573 734d 6f64  _api_businessMod
+00000fb0: 756c 654c 6973 744e 290d da08 5f5f 6e61  uleListN)...__na
+00000fc0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000fd0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000fe0: 5f5f 646f 635f 5f72 1c00 0000 722f 0000  __doc__r....r/..
+00000ff0: 0072 2000 0000 7226 0000 0072 3500 0000  .r ...r&...r5...
+00001000: da04 626f 6f6c 7232 0000 0072 2500 0000  ..boolr2...r%...
+00001010: 7213 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00001020: 1a00 0000 721b 0000 0072 0c00 0000 0b00  ....r....r......
+00001030: 0000 7310 0000 0008 0104 0408 0908 250e  ..s...........%.
+00001040: 1508 0710 0d08 0572 0c00 0000 2913 7233  .......r....).r3
+00001050: 0000 00da 2974 6466 5f74 6f6f 6c2e 746f  ....)tdf_tool.to
+00001060: 6f6c 732e 636f 6e66 6967 2e69 6e69 7469  ols.config.initi
+00001070: 616c 5f6a 736f 6e5f 636f 6e66 6967 7202  al_json_configr.
+00001080: 0000 00da 2874 6466 5f74 6f6f 6c2e 746f  ....(tdf_tool.to
+00001090: 6f6c 732e 636f 6e66 6967 2e6d 6f64 756c  ols.config.modul
+000010a0: 655f 6a73 6f6e 5f63 6f6e 6669 6772 0300  e_json_configr..
+000010b0: 0000 7204 0000 005a 2574 6466 5f74 6f6f  ..r....Z%tdf_too
+000010c0: 6c2e 746f 6f6c 732e 636f 6e66 6967 2e70  l.tools.config.p
+000010d0: 6163 6b61 6765 735f 636f 6e66 6967 7205  ackages_configr.
+000010e0: 0000 0072 0600 0000 da14 7464 665f 746f  ...r......tdf_to
+000010f0: 6f6c 2e74 6f6f 6c73 2e70 7269 6e74 7207  ol.tools.printr.
+00001100: 0000 00da 1874 6466 5f74 6f6f 6c2e 746f  .....tdf_tool.to
+00001110: 6f6c 732e 7368 656c 6c5f 6469 7272 0800  ols.shell_dirr..
+00001120: 0000 7209 0000 005a 1974 6466 5f74 6f6f  ..r....Z.tdf_too
+00001130: 6c2e 7069 7065 6c69 6e65 732e 726f 7574  l.pipelines.rout
+00001140: 6572 720a 0000 005a 2274 6466 5f74 6f6f  err....Z"tdf_too
+00001150: 6c2e 7069 7065 6c69 6e65 732e 6170 695f  l.pipelines.api_
+00001160: 696e 7465 7261 6374 696f 6e72 0b00 0000  interactionr....
+00001170: 720c 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
+00001180: 1a00 0000 721b 0000 00da 083c 6d6f 6475  ....r......<modu
+00001190: 6c65 3e01 0000 0073 1000 0000 0801 0c01  le>....s........
+000011a0: 1001 1001 0c01 1002 0c01 0c02            ............
```

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/api_interaction.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/annotation.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 from tdf_tool.tools.config.initial_json_config import InitialJsonConfig
 from tdf_tool.tools.config.module_json_config import ModuleItemType, ModuleJsonConfig
 from tdf_tool.tools.config.packages_config import PackageNode, PackagesJsonConfig
 from tdf_tool.tools.print import Print
-from tdf_tool.tools.shell_dir import ShellDir
+from tdf_tool.tools.shell_dir import ShellDir, ProjectType
 
 from tdf_tool.pipelines.router import Router
 from tdf_tool.pipelines.api_interaction import ApiAnnotation
 
 class Annotation:
     """
     模块间支持相关命令：tl annotation -h 查看详情
     """
 
     def __init__(self):
         Print.title("检测中...")
-        self.__buildRunnerName: str = "build_runner" # build_runner库名
-
-        self.__routerAnnotation: Router = Router()
-        self.__apiAnnotation: ApiAnnotation = ApiAnnotation()
-        self.__businessModuleList = self.__api_businessModuleList()
-        self.__packagesList: list[PackageNode] = PackagesJsonConfig(ShellDir.getShellDir()).packages # 壳依赖的所有库
+        if ShellDir.getProjectType() == ProjectType.FLUTTER:
+            self.__buildRunnerName: str = "build_runner" # build_runner库名
+            self.__routerAnnotation: Router = Router()
+            self.__apiAnnotation: ApiAnnotation = ApiAnnotation()
+            self.__businessModuleList = self.__api_businessModuleList()
+            self.__packagesList: list[PackageNode] = PackagesJsonConfig(ShellDir.getShellDir()).packages # 壳依赖的所有库
 
     def start(self):
         """
         tl annotation start：会以交互式进行操作，对指定的模块执行描述文件(包括路由，api交互)生成和自动注册逻辑
         """
         ShellDir.goInShellDir()
         
@@ -33,29 +33,29 @@
             print(f"{index}: {item}")
         print()
         while True:
             module_name = input("请输入需要生成描述文件的模块名或其下标(input ! 退出，all 自动注册)：")
             if module_name == "!" or module_name == "！":
                 exit(0)
             elif module_name == "all":
-                self.__integrate_shell()
+                self.integrate()
                 exit(0)
             elif module_name in self.__businessModuleList:
                 self.__generateCode(module_name)
                 Print.title(module_name + "描述文件生成完成")
-                self.__integrate_shell()
+                self.integrate()
                 exit(0)
             else:
                 try:
                     i = int(module_name)
                     if (i < len(self.__businessModuleList)):
                         _module_anme = self.__businessModuleList[i]
                         self.__generateCode(_module_anme)
                         Print.title(_module_anme + "描述文件生成完成")
-                        self.__integrate_shell()
+                        self.integrate()
                         exit(0)
                     else:
                         Print.warning("输入有误，请重新输入")
                 except ValueError:
                     Print.warning("输入有误，请重新输入")                    
     
     # 生成指定模块的描述文件
@@ -96,15 +96,15 @@
         for item in packageJsonConfig.packages:
             if item.packageName == self.__buildRunnerName:
                 hasBuildRunner = True
                 
         return hasBuildRunner
                 
 
-    def __integrate_shell(self):
+    def integrate(self):
         self.__routerAnnotation.integrate_shell()
         self.__apiAnnotation.integrate_shell()
         Print.title("整合完成")
         
     def __api_businessModuleList(self):
         __module_config = ModuleJsonConfig()
         __list = []
```

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/api_interaction.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/api_interaction.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/fix_header.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/fix_header.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/git.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/git.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/module.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/package.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/package.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/router.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/router.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/pipelines/translate.py` & `tdf_tool-2.4.9/tdf_tool/pipelines/translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/generator.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/generator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr 18 09:33:56 2024 UTC, .py size: 5718 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 04e9 2066 5616 0000  a......... fV...
+00000000: 610d 0d0a 0000 0000 ab2f 2366 a016 0000  a......../#f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6501 8303  ..G.d.d...d.e...
@@ -105,248 +105,250 @@
 00000680: 7216 0000 00da 046e 616d 6572 1000 0000  r......namer....
 00000690: 7210 0000 0072 1100 0000 da0e 6765 7450  r....r......getP
 000006a0: 726f 6a65 6374 5479 7065 2a00 0000 7312  rojectType*...s.
 000006b0: 0000 0000 0108 0110 0106 0110 0106 020e  ................
 000006c0: 010a 010c 017a 1753 6865 6c6c 4469 722e  .....z.ShellDir.
 000006d0: 6765 7450 726f 6a65 6374 5479 7065 6300  getProjectTypec.
 000006e0: 0000 0000 0000 0000 0000 0003 0000 0008  ................
-000006f0: 0000 0043 0000 0073 de00 0000 7400 a001  ...C...s....t...
-00000700: a100 7402 5f03 7404 a005 a100 7214 6ec6  ..t._.t.....r.n.
-00000710: 7aa8 7402 a006 a100 7d00 7c00 7407 6a08  z.t.....}.|.t.j.
-00000720: 6b02 72a6 7409 6401 6402 6403 8d02 8f60  k.r.t.d.d.d....`
-00000730: 7d01 740a a00b 7c01 a101 7d02 740c 7c02  }.t...|...}.t.|.
-00000740: 740d 8302 727e 7c02 a00e 6404 a101 727e  t...r~|...d...r~
-00000750: 740c 7c02 6404 1900 740d 8302 727e 7c02  t.|.d...t...r~|.
-00000760: 6404 1900 a00e 6405 a101 6406 7501 727e  d.....d...d.u.r~
-00000770: 740f a010 6407 a101 0100 7c01 a011 a100  t...d.....|.....
-00000780: 0100 5700 6400 0400 0400 8303 0100 71ba  ..W.d.........q.
-00000790: 3100 739a 3000 0100 0100 0100 5900 0100  1.s.0.......Y...
-000007a0: 6e14 7c00 7407 6a12 6b02 72ba 740f a010  n.|.t.j.k.r.t...
-000007b0: 6407 a101 0100 5700 6e1c 0400 7413 79d8  d.....W.n...t.y.
-000007c0: 0100 0100 0100 740f a010 6407 a101 0100  ......t...d.....
-000007d0: 5900 6e02 3000 6400 5300 2908 4e7a 0c70  Y.n.0.d.S.).Nz.p
-000007e0: 7562 7370 6563 2e79 616d 6cfa 0575 7466  ubspec.yaml..utf
-000007f0: 2d38 a901 da08 656e 636f 6469 6e67 5a07  -8....encodingZ.
-00000800: 666c 7574 7465 72da 066d 6f64 756c 6554  flutter..moduleT
-00000810: 7538 0000 00e5 bd93 e589 8de4 b88d e698  u8..............
-00000820: afe5 a3b3 e5b7 a5e7 a88b e79b aee5 bd95  ................
-00000830: efbc 8ce7 a681 e6ad a2e6 89a7 e8a1 8c74  ...............t
-00000840: 6466 5f74 6f6f 6ce5 91bd e4bb a429 1472  df_tool......).r
-00000850: 1b00 0000 da06 6765 7463 7764 7212 0000  ......getcwdr...
-00000860: 0072 1400 0000 7204 0000 005a 0869 735f  .r....r....Z.is_
-00000870: 6465 6275 6772 2900 0000 7207 0000 0072  debugr)...r....r
-00000880: 0e00 0000 da04 6f70 656e 7206 0000 00da  ......openr.....
-00000890: 0f72 6f75 6e64 5f74 7269 705f 6c6f 6164  .round_trip_load
-000008a0: da0a 6973 696e 7374 616e 6365 da04 6469  ..isinstance..di
-000008b0: 6374 da0c 5f5f 636f 6e74 6169 6e73 5f5f  ct..__contains__
-000008c0: 7205 0000 00da 0565 7272 6f72 da05 636c  r......error..cl
-000008d0: 6f73 6572 0d00 0000 da07 494f 4572 726f  oser......IOErro
-000008e0: 7229 03da 0b70 726f 6a65 6374 5479 7065  r)...projectType
-000008f0: da01 66da 0364 6f63 7210 0000 0072 1000  ..f..docr....r..
-00000900: 0000 7211 0000 00da 0d64 6972 496e 7661  ..r......dirInva
-00000910: 6c69 6461 7465 3700 0000 7326 0000 0000  lidate7...s&....
-00000920: 010a 0108 0102 0202 0108 020a 010e 010a  ................
-00000930: 0114 020c ff02 0210 fe02 040a 0128 010a  .............(..
-00000940: 010e 010c 017a 1653 6865 6c6c 4469 722e  .....z.ShellDir.
-00000950: 6469 7249 6e76 616c 6964 6174 6563 0000  dirInvalidatec..
-00000960: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000970: 0000 4300 0000 7308 0000 0074 00a0 01a1  ..C...s....t....
-00000980: 0053 0072 1500 0000 a902 7212 0000 0072  .S.r......r....r
-00000990: 2500 0000 7210 0000 0072 1000 0000 7210  %...r....r....r.
-000009a0: 0000 0072 1100 0000 da0b 6765 7453 6865  ...r......getShe
-000009b0: 6c6c 4469 724e 0000 0073 0200 0000 0001  llDirN...s......
-000009c0: 7a14 5368 656c 6c44 6972 2e67 6574 5368  z.ShellDir.getSh
-000009d0: 656c 6c44 6972 6300 0000 0000 0000 0000  ellDirc.........
-000009e0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-000009f0: 3200 0000 7400 a001 a100 7d00 7402 6a03  2...t.....}.t.j.
-00000a00: a004 7c00 a101 7220 7402 a005 7c00 a101  ..|...r t...|...
-00000a10: 0100 6e0e 7406 a007 7c00 6401 1700 a101  ..n.t...|.d.....
-00000a20: 0100 6400 5300 a902 4ef5 0f00 0000 e8b7  ..d.S...N.......
-00000a30: afe5 be84 e4b8 8de5 ad98 e59c a8a9 0872  ...............r
-00000a40: 1200 0000 7225 0000 0072 1b00 0000 7216  ....r%...r....r.
-00000a50: 0000 0072 2600 0000 da05 6368 6469 7272  ...r&.....chdirr
-00000a60: 0500 0000 7234 0000 00a9 015a 0f5f 5368  ....r4.....Z._Sh
-00000a70: 656c 6c44 6972 5f5f 7061 7468 7210 0000  ellDir__pathr...
-00000a80: 0072 1000 0000 7211 0000 00da 0c67 6f49  .r....r......goI
-00000a90: 6e53 6865 6c6c 4469 7252 0000 0073 0800  nShellDirR...s..
-00000aa0: 0000 0001 0801 0c01 0c02 7a15 5368 656c  ..........z.Shel
-00000ab0: 6c44 6972 2e67 6f49 6e53 6865 6c6c 4469  lDir.goInShellDi
-00000ac0: 7263 0000 0000 0000 0000 0000 0000 0100  rc..............
-00000ad0: 0000 0400 0000 4300 0000 7336 0000 0074  ......C...s6...t
-00000ae0: 00a0 01a1 0064 0117 007d 0074 026a 03a0  .....d...}.t.j..
-00000af0: 047c 00a1 0172 2474 02a0 057c 00a1 0101  .|...r$t...|....
-00000b00: 006e 0e74 06a0 077c 0064 0217 00a1 0101  .n.t...|.d......
-00000b10: 0064 0053 0029 034e fa04 2f6c 6962 723e  .d.S.).N../libr>
-00000b20: 0000 0072 3f00 0000 2901 7216 0000 0072  ...r?...).r....r
-00000b30: 1000 0000 7210 0000 0072 1100 0000 da0f  ....r....r......
-00000b40: 676f 496e 5368 656c 6c4c 6962 4469 725a  goInShellLibDirZ
-00000b50: 0000 0073 0800 0000 0001 0c01 0c01 0c02  ...s............
-00000b60: 7a18 5368 656c 6c44 6972 2e67 6f49 6e53  z.ShellDir.goInS
-00000b70: 6865 6c6c 4c69 6244 6972 2902 722d 0000  hellLibDir).r-..
-00000b80: 0072 1700 0000 6301 0000 0000 0000 0000  .r....c.........
-00000b90: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000ba0: 1000 0000 7400 a001 a100 6401 1700 7c00  ....t.....d...|.
-00000bb0: 1700 5300 2902 4efa 112f 2e2e 2f2e 7464  ..S.).N../../.td
-00000bc0: 665f 666c 7574 7465 722f 723b 0000 00a9  f_flutter/r;....
-00000bd0: 0172 2d00 0000 7210 0000 0072 1000 0000  .r-...r....r....
-00000be0: 7211 0000 00da 0c67 6574 4d6f 6475 6c65  r......getModule
-00000bf0: 4469 7262 0000 0073 0200 0000 0001 7a15  Dirb...s......z.
-00000c00: 5368 656c 6c44 6972 2e67 6574 4d6f 6475  ShellDir.getModu
-00000c10: 6c65 4469 7272 4600 0000 6301 0000 0000  leDirrF...c.....
-00000c20: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000c30: 0000 0073 3400 0000 7400 a001 7c00 a101  ...s4...t...|...
-00000c40: 7d01 7402 6a03 a004 7c01 a101 7222 7402  }.t.j...|...r"t.
-00000c50: a005 7c01 a101 0100 6e0e 7406 a007 7c01  ..|.....n.t...|.
-00000c60: 6401 1700 a101 0100 6400 5300 723d 0000  d.......d.S.r=..
-00000c70: 0029 0872 1200 0000 7247 0000 0072 1b00  .).r....rG...r..
-00000c80: 0000 7216 0000 0072 2600 0000 7240 0000  ..r....r&...r@..
-00000c90: 0072 0500 0000 7234 0000 00a9 0272 2d00  .r....r4.....r-.
-00000ca0: 0000 5a0b 6d6f 6475 6c65 5f70 6174 6872  ..Z.module_pathr
-00000cb0: 1000 0000 7210 0000 0072 1100 0000 da0d  ....r....r......
-00000cc0: 676f 496e 4d6f 6475 6c65 4469 7266 0000  goInModuleDirf..
-00000cd0: 0073 0800 0000 0001 0a01 0c01 0c02 7a16  .s............z.
-00000ce0: 5368 656c 6c44 6972 2e67 6f49 6e4d 6f64  ShellDir.goInMod
-00000cf0: 756c 6544 6972 6301 0000 0000 0000 0000  uleDirc.........
-00000d00: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
-00000d10: 1400 0000 7400 a001 a100 6401 1700 7c00  ....t.....d...|.
-00000d20: 1700 6402 1700 5300 2903 4e72 4500 0000  ..d...S.).NrE...
-00000d30: 7243 0000 0072 3b00 0000 7246 0000 0072  rC...r;...rF...r
-00000d40: 1000 0000 7210 0000 0072 1100 0000 da0f  ....r....r......
-00000d50: 6765 744d 6f64 756c 654c 6962 4469 726e  getModuleLibDirn
-00000d60: 0000 0073 0200 0000 0001 7a18 5368 656c  ...s......z.Shel
-00000d70: 6c44 6972 2e67 6574 4d6f 6475 6c65 4c69  lDir.getModuleLi
-00000d80: 6244 6972 6301 0000 0000 0000 0000 0000  bDirc...........
-00000d90: 0002 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
-00000da0: 0000 7400 a001 7c00 a101 7d01 7402 6a03  ..t...|...}.t.j.
-00000db0: a004 7c01 a101 7222 7402 a005 7c01 a101  ..|...r"t...|...
-00000dc0: 0100 6e0e 7406 a007 7c01 6401 1700 a101  ..n.t...|.d.....
-00000dd0: 0100 6400 5300 723d 0000 0029 0872 1200  ..d.S.r=...).r..
-00000de0: 0000 724a 0000 0072 1b00 0000 7216 0000  ..rJ...r....r...
-00000df0: 0072 2600 0000 7240 0000 0072 0500 0000  .r&...r@...r....
-00000e00: 7234 0000 0072 4800 0000 7210 0000 0072  r4...rH...r....r
-00000e10: 1000 0000 7211 0000 00da 1067 6f49 6e4d  ....r......goInM
-00000e20: 6f64 756c 654c 6962 4469 7272 0000 0073  oduleLibDirr...s
-00000e30: 0800 0000 0001 0a01 0c01 0c02 7a19 5368  ............z.Sh
-00000e40: 656c 6c44 6972 2e67 6f49 6e4d 6f64 756c  ellDir.goInModul
-00000e50: 654c 6962 4469 7263 0100 0000 0000 0000  eLibDirc........
-00000e60: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000e70: 7314 0000 0074 00a0 01a1 0064 0117 007c  s....t.....d...|
-00000e80: 0017 0064 0217 0053 0029 034e 7245 0000  ...d...S.).NrE..
-00000e90: 007a 0d2f 6c69 622f 7464 665f 696e 746c  .z./lib/tdf_intl
-00000ea0: 723b 0000 0072 4600 0000 7210 0000 0072  r;...rF...r....r
-00000eb0: 1000 0000 7211 0000 00da 1267 6574 496e  ....r......getIn
-00000ec0: 4d6f 6475 6c65 496e 746c 4469 727a 0000  ModuleIntlDirz..
-00000ed0: 0073 0200 0000 0001 7a1b 5368 656c 6c44  .s......z.ShellD
-00000ee0: 6972 2e67 6574 496e 4d6f 6475 6c65 496e  ir.getInModuleIn
-00000ef0: 746c 4469 7263 0100 0000 0000 0000 0000  tlDirc..........
-00000f00: 0000 0200 0000 0400 0000 4300 0000 7334  ..........C...s4
-00000f10: 0000 0074 00a0 017c 00a1 017d 0174 026a  ...t...|...}.t.j
-00000f20: 03a0 047c 01a1 0172 2274 02a0 057c 01a1  ...|...r"t...|..
-00000f30: 0101 006e 0e74 06a0 077c 0164 0117 00a1  ...n.t...|.d....
-00000f40: 0101 0064 0053 0072 3d00 0000 2908 7212  ...d.S.r=...).r.
-00000f50: 0000 0072 4c00 0000 721b 0000 0072 1600  ...rL...r....r..
-00000f60: 0000 7226 0000 0072 4000 0000 7205 0000  ..r&...r@...r...
-00000f70: 0072 3400 0000 7248 0000 0072 1000 0000  .r4...rH...r....
-00000f80: 7210 0000 0072 1100 0000 da11 676f 496e  r....r......goIn
-00000f90: 4d6f 6475 6c65 496e 746c 4469 727e 0000  ModuleIntlDir~..
-00000fa0: 0073 0800 0000 0001 0a01 0c01 0c02 7a1a  .s............z.
-00000fb0: 5368 656c 6c44 6972 2e67 6f49 6e4d 6f64  ShellDir.goInMod
-00000fc0: 756c 6549 6e74 6c44 6972 6300 0000 0000  uleIntlDirc.....
-00000fd0: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
-00000fe0: 0000 0073 0c00 0000 7400 a001 a100 6401  ...s....t.....d.
-00000ff0: 1700 5300 2902 4e7a 102f 2e2e 2f2e 7464  ..S.).Nz./../.td
-00001000: 665f 666c 7574 7465 7229 0272 1200 0000  f_flutter).r....
-00001010: 723c 0000 0072 1000 0000 7210 0000 0072  r<...r....r....r
-00001020: 1000 0000 7211 0000 00da 1267 6574 496e  ....r......getIn
-00001030: 5464 6646 6c75 7474 6572 4469 7286 0000  TdfFlutterDir...
-00001040: 0073 0200 0000 0001 7a1b 5368 656c 6c44  .s......z.ShellD
-00001050: 6972 2e67 6574 496e 5464 6646 6c75 7474  ir.getInTdfFlutt
-00001060: 6572 4469 7263 0000 0000 0000 0000 0000  erDirc..........
-00001070: 0000 0100 0000 0300 0000 4300 0000 732c  ..........C...s,
-00001080: 0000 0074 00a0 01a1 007d 0074 026a 03a0  ...t.....}.t.j..
-00001090: 047c 00a1 0173 1e74 02a0 057c 00a1 0101  .|...s.t...|....
-000010a0: 0074 02a0 067c 00a1 0101 0064 0053 0072  .t...|.....d.S.r
-000010b0: 1500 0000 2907 7212 0000 0072 4e00 0000  ....).r....rN...
-000010c0: 721b 0000 0072 1600 0000 7226 0000 00da  r....r....r&....
-000010d0: 056d 6b64 6972 7240 0000 0072 4100 0000  .mkdirr@...rA...
-000010e0: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-000010f0: 1167 6f49 6e54 6466 466c 7574 7465 7244  .goInTdfFlutterD
-00001100: 6972 8a00 0000 7308 0000 0000 0108 010c  ir....s.........
-00001110: 010a 017a 1a53 6865 6c6c 4469 722e 676f  ...z.ShellDir.go
-00001120: 496e 5464 6646 6c75 7474 6572 4469 7263  InTdfFlutterDirc
-00001130: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00001140: 0300 0000 4300 0000 735e 0000 0074 00a0  ....C...s^...t..
-00001150: 01a1 0001 0074 026a 03a0 0464 01a1 0172  .....t.j...d...r
-00001160: 2074 02a0 0564 01a1 0101 006e 3a74 026a   t...d.....n:t.j
-00001170: 03a0 0464 01a1 0173 5a74 0664 0283 017d  ...d...sZt.d...}
-00001180: 007c 0064 036b 0272 4874 02a0 0764 01a1  .|.d.k.rHt...d..
-00001190: 0101 006e 1274 08a0 0964 04a1 0101 0074  ...n.t...d.....t
-000011a0: 0a64 0583 0101 0064 0053 0029 064e da09  .d.....d.S.).N..
-000011b0: 7464 665f 6361 6368 6575 4800 0000 e5bd  tdf_cacheuH.....
-000011c0: 93e5 898d e79b aee5 bd95 e6b2 a1e6 9c89  ................
-000011d0: e689 bee5 88b0 7464 665f 6361 6368 65e7  ......tdf_cache.
-000011e0: bc93 e5ad 98e6 9687 e4bb b6e5 a4b9 efbc  ................
-000011f0: 8ce6 98af e590 a6e5 889b e5bb baef bc9f  ................
-00001200: 2879 2f6e 293a da01 797a 164f 682c 6974  (y/n):..yz.Oh,it
-00001210: 2773 2064 6973 6170 706f 696e 7469 6e67  's disappointing
-00001220: 2e72 0800 0000 290b 7212 0000 0072 4200  .r....).r....rB.
-00001230: 0000 721b 0000 0072 1600 0000 7226 0000  ..r....r....r&..
-00001240: 0072 4000 0000 da05 696e 7075 7472 4f00  .r@.....inputrO.
-00001250: 0000 7205 0000 0072 3400 0000 da04 6578  ..r....r4.....ex
-00001260: 6974 2901 5a06 6372 6561 7465 7210 0000  it).Z.creater...
-00001270: 0072 1000 0000 7211 0000 00da 0d67 6f54  .r....r......goT
-00001280: 6466 4361 6368 6544 6972 9100 0000 7312  dfCacheDir....s.
-00001290: 0000 0000 0108 010c 010c 010c 0108 0108  ................
-000012a0: 010c 020a 017a 1653 6865 6c6c 4469 722e  .....z.ShellDir.
-000012b0: 676f 5464 6643 6163 6865 4469 7229 02da  goTdfCacheDir)..
-000012c0: 0979 616d 6c5f 7061 7468 7217 0000 0063  .yaml_pathr....c
-000012d0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-000012e0: 0800 0000 4300 0000 7376 0000 0074 007c  ....C...sv...t.|
-000012f0: 0064 0164 0264 038d 038f 547d 0174 01a0  .d.d.d....T}.t..
-00001300: 027c 01a0 03a1 00a1 017d 027c 0264 0075  .|.......}.|.d.u
-00001310: 0172 4a7c 02a0 0464 04a1 0172 4a7c 0264  .rJ|...d...rJ|.d
-00001320: 0419 007d 037c 0357 0002 0064 0004 0004  ...}.|.W...d....
-00001330: 0083 0301 0053 0074 05a0 0664 05a1 0101  .....S.t...d....
-00001340: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001350: 0073 6830 0001 0001 0001 0059 0001 0064  .sh0.......Y...d
-00001360: 0053 0029 064e da01 7272 2a00 0000 722b  .S.).N..rr*...r+
-00001370: 0000 0072 2800 0000 7555 0000 00e8 afbb  ...r(...uU......
-00001380: e58f 96e5 a3b3 e6a8 a1e5 9d97 e6a8 a1e5  ................
-00001390: 9d97 e590 8de5 a4b1 e8b4 a5ef bc8c e8af  ................
-000013a0: b7e7 a1ae e4bf 9de5 a3b3 e6a8 a1e5 9d97  ................
-000013b0: e79a 8470 7562 7370 6563 2e79 616d 6ce9  ...pubspec.yaml.
-000013c0: 858d e7bd aee4 ba86 6e61 6d65 e5b1 9ee6  ........name....
-000013d0: 80a7 2907 722f 0000 0072 0600 0000 7230  ..).r/...r....r0
-000013e0: 0000 00da 0472 6561 6472 3300 0000 7205  .....readr3...r.
-000013f0: 0000 0072 3400 0000 2904 7256 0000 005a  ...r4...).rV...Z
-00001400: 0272 46da 0364 6963 da0b 7368 656c 6c4d  .rF..dic..shellM
-00001410: 6f64 756c 6572 1000 0000 7210 0000 0072  oduler....r....r
-00001420: 1100 0000 da15 6765 744d 6f64 756c 654e  ......getModuleN
-00001430: 616d 6546 726f 6d59 616d 6c9e 0000 0073  ameFromYaml....s
-00001440: 0c00 0000 0001 1001 0e01 1201 0801 1202  ................
-00001450: 7a1e 5368 656c 6c44 6972 2e67 6574 4d6f  z.ShellDir.getMo
-00001460: 6475 6c65 4e61 6d65 4672 6f6d 5961 6d6c  duleNameFromYaml
-00001470: 4e29 1972 0a00 0000 720b 0000 0072 0c00  N).r....r....r..
-00001480: 0000 7214 0000 00da 0373 7472 da0f 5f5f  ..r......str..__
-00001490: 616e 6e6f 7461 7469 6f6e 735f 5f72 2500  annotations__r%.
-000014a0: 0000 7223 0000 0072 2400 0000 7207 0000  ..r#...r$...r...
-000014b0: 0072 2900 0000 723a 0000 0072 3c00 0000  .r)...r:...r<...
-000014c0: 7242 0000 0072 4400 0000 7247 0000 0072  rB...rD...rG...r
-000014d0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
-000014e0: 0000 0072 4d00 0000 724e 0000 0072 5000  ...rM...rN...rP.
-000014f0: 0000 7255 0000 0072 5b00 0000 7210 0000  ..rU...r[...r...
-00001500: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00001510: 7212 0000 000f 0000 0073 2600 0000 0a01  r........s&.....
-00001520: 0c02 0808 1008 1008 0e0d 0817 0e04 0808  ................
-00001530: 0808 1004 0e08 1004 0e08 0e04 0e08 0804  ................
-00001540: 0807 080d 7212 0000 0029 0dda 0465 6e75  ....r....)...enu
-00001550: 6d72 0200 0000 721b 0000 00da 1274 6466  mr....r......tdf
-00001560: 5f74 6f6f 6c2e 746f 6f6c 732e 636d 6472  _tool.tools.cmdr
-00001570: 0300 0000 5a12 7464 665f 746f 6f6c 2e74  ....Z.tdf_tool.t
-00001580: 6f6f 6c73 2e65 6e76 7204 0000 00da 1474  ools.envr......t
-00001590: 6466 5f74 6f6f 6c2e 746f 6f6c 732e 7072  df_tool.tools.pr
-000015a0: 696e 7472 0500 0000 da06 7275 616d 656c  intr......ruamel
-000015b0: 7206 0000 0072 0700 0000 7212 0000 0072  r....r....r....r
-000015c0: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
-000015d0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000015e0: 0073 0e00 0000 0c01 0801 0c01 0c01 0c01  .s..............
-000015f0: 0c03 1006                                ....
+000006f0: 0000 0043 0000 0073 f000 0000 7400 a001  ...C...s....t...
+00000700: a100 7402 5f03 7404 7402 6a03 8301 0100  ..t._.t.t.j.....
+00000710: 7405 a006 a100 721e 6ece 7ab0 7402 a007  t.....r.n.z.t...
+00000720: a100 7d00 7404 7c00 8301 0100 7c00 7408  ..}.t.|.....|.t.
+00000730: 6a09 6b02 72b8 740a 6401 6402 6403 8d02  j.k.r.t.d.d.d...
+00000740: 8f60 7d01 740b a00c 7c01 a101 7d02 740d  .`}.t...|...}.t.
+00000750: 7c02 740e 8302 7290 7c02 a00f 6404 a101  |.t...r.|...d...
+00000760: 7290 740d 7c02 6404 1900 740e 8302 7290  r.t.|.d...t...r.
+00000770: 7c02 6404 1900 a00f 6405 a101 6406 7501  |.d.....d...d.u.
+00000780: 7290 7410 a011 6407 a101 0100 7c01 a012  r.t...d.....|...
+00000790: a100 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+000007a0: 71cc 3100 73ac 3000 0100 0100 0100 5900  q.1.s.0.......Y.
+000007b0: 0100 6e14 7c00 7408 6a13 6b02 72cc 7410  ..n.|.t.j.k.r.t.
+000007c0: a011 6407 a101 0100 5700 6e1c 0400 7414  ..d.....W.n...t.
+000007d0: 79ea 0100 0100 0100 7410 a011 6407 a101  y.......t...d...
+000007e0: 0100 5900 6e02 3000 6400 5300 2908 4e7a  ..Y.n.0.d.S.).Nz
+000007f0: 0c70 7562 7370 6563 2e79 616d 6cfa 0575  .pubspec.yaml..u
+00000800: 7466 2d38 a901 da08 656e 636f 6469 6e67  tf-8....encoding
+00000810: 5a07 666c 7574 7465 72da 066d 6f64 756c  Z.flutter..modul
+00000820: 6554 7538 0000 00e5 bd93 e589 8de4 b88d  eTu8............
+00000830: e698 afe5 a3b3 e5b7 a5e7 a88b e79b aee5  ................
+00000840: bd95 efbc 8ce7 a681 e6ad a2e6 89a7 e8a1  ................
+00000850: 8c74 6466 5f74 6f6f 6ce5 91bd e4bb a429  .tdf_tool......)
+00000860: 1572 1b00 0000 da06 6765 7463 7764 7212  .r......getcwdr.
+00000870: 0000 0072 1400 0000 da05 7072 696e 7472  ...r......printr
+00000880: 0400 0000 5a08 6973 5f64 6562 7567 7229  ....Z.is_debugr)
+00000890: 0000 0072 0700 0000 720e 0000 00da 046f  ...r....r......o
+000008a0: 7065 6e72 0600 0000 da0f 726f 756e 645f  penr......round_
+000008b0: 7472 6970 5f6c 6f61 64da 0a69 7369 6e73  trip_load..isins
+000008c0: 7461 6e63 65da 0464 6963 74da 0c5f 5f63  tance..dict..__c
+000008d0: 6f6e 7461 696e 735f 5f72 0500 0000 da05  ontains__r......
+000008e0: 6572 726f 72da 0563 6c6f 7365 720d 0000  error..closer...
+000008f0: 00da 0749 4f45 7272 6f72 2903 da0b 7072  ...IOError)...pr
+00000900: 6f6a 6563 7454 7970 65da 0166 da03 646f  ojectType..f..do
+00000910: 6372 1000 0000 7210 0000 0072 1100 0000  cr....r....r....
+00000920: da0d 6469 7249 6e76 616c 6964 6174 6537  ..dirInvalidate7
+00000930: 0000 0073 2a00 0000 0001 0a01 0a01 0801  ...s*...........
+00000940: 0202 0201 0801 0802 0a01 0e01 0a01 1402  ................
+00000950: 0cff 0202 10fe 0204 0a01 2801 0a01 0e01  ..........(.....
+00000960: 0c01 7a16 5368 656c 6c44 6972 2e64 6972  ..z.ShellDir.dir
+00000970: 496e 7661 6c69 6461 7465 6300 0000 0000  Invalidatec.....
+00000980: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00000990: 0000 0073 0800 0000 7400 a001 a100 5300  ...s....t.....S.
+000009a0: 7215 0000 00a9 0272 1200 0000 7225 0000  r......r....r%..
+000009b0: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
+000009c0: 7211 0000 00da 0b67 6574 5368 656c 6c44  r......getShellD
+000009d0: 6972 5000 0000 7302 0000 0000 017a 1453  irP...s......z.S
+000009e0: 6865 6c6c 4469 722e 6765 7453 6865 6c6c  hellDir.getShell
+000009f0: 4469 7263 0000 0000 0000 0000 0000 0000  Dirc............
+00000a00: 0100 0000 0400 0000 4300 0000 7332 0000  ........C...s2..
+00000a10: 0074 00a0 01a1 007d 0074 026a 03a0 047c  .t.....}.t.j...|
+00000a20: 00a1 0172 2074 02a0 057c 00a1 0101 006e  ...r t...|.....n
+00000a30: 0e74 06a0 077c 0064 0117 00a1 0101 0064  .t...|.d.......d
+00000a40: 0053 00a9 024e f50f 0000 00e8 b7af e5be  .S...N..........
+00000a50: 84e4 b88d e5ad 98e5 9ca8 a908 7212 0000  ............r...
+00000a60: 0072 2500 0000 721b 0000 0072 1600 0000  .r%...r....r....
+00000a70: 7226 0000 00da 0563 6864 6972 7205 0000  r&.....chdirr...
+00000a80: 0072 3500 0000 a901 5a0f 5f53 6865 6c6c  .r5.....Z._Shell
+00000a90: 4469 725f 5f70 6174 6872 1000 0000 7210  Dir__pathr....r.
+00000aa0: 0000 0072 1100 0000 da0c 676f 496e 5368  ...r......goInSh
+00000ab0: 656c 6c44 6972 5400 0000 7308 0000 0000  ellDirT...s.....
+00000ac0: 0108 010c 010c 027a 1553 6865 6c6c 4469  .......z.ShellDi
+00000ad0: 722e 676f 496e 5368 656c 6c44 6972 6300  r.goInShellDirc.
+00000ae0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000af0: 0000 0043 0000 0073 3600 0000 7400 a001  ...C...s6...t...
+00000b00: a100 6401 1700 7d00 7402 6a03 a004 7c00  ..d...}.t.j...|.
+00000b10: a101 7224 7402 a005 7c00 a101 0100 6e0e  ..r$t...|.....n.
+00000b20: 7406 a007 7c00 6402 1700 a101 0100 6400  t...|.d.......d.
+00000b30: 5300 2903 4efa 042f 6c69 6272 3f00 0000  S.).N../libr?...
+00000b40: 7240 0000 0029 0172 1600 0000 7210 0000  r@...).r....r...
+00000b50: 0072 1000 0000 7211 0000 00da 0f67 6f49  .r....r......goI
+00000b60: 6e53 6865 6c6c 4c69 6244 6972 5c00 0000  nShellLibDir\...
+00000b70: 7308 0000 0000 010c 010c 010c 027a 1853  s............z.S
+00000b80: 6865 6c6c 4469 722e 676f 496e 5368 656c  hellDir.goInShel
+00000b90: 6c4c 6962 4469 7229 0272 2d00 0000 7217  lLibDir).r-...r.
+00000ba0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000bb0: 0100 0000 0200 0000 4300 0000 7310 0000  ........C...s...
+00000bc0: 0074 00a0 01a1 0064 0117 007c 0017 0053  .t.....d...|...S
+00000bd0: 0029 024e fa11 2f2e 2e2f 2e74 6466 5f66  .).N../../.tdf_f
+00000be0: 6c75 7474 6572 2f72 3c00 0000 a901 722d  lutter/r<.....r-
+00000bf0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+00000c00: 0000 da0c 6765 744d 6f64 756c 6544 6972  ....getModuleDir
+00000c10: 6400 0000 7302 0000 0000 017a 1553 6865  d...s......z.She
+00000c20: 6c6c 4469 722e 6765 744d 6f64 756c 6544  llDir.getModuleD
+00000c30: 6972 7247 0000 0063 0100 0000 0000 0000  irrG...c........
+00000c40: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00000c50: 7334 0000 0074 00a0 017c 00a1 017d 0174  s4...t...|...}.t
+00000c60: 026a 03a0 047c 01a1 0172 2274 02a0 057c  .j...|...r"t...|
+00000c70: 01a1 0101 006e 0e74 06a0 077c 0164 0117  .....n.t...|.d..
+00000c80: 00a1 0101 0064 0053 0072 3e00 0000 2908  .....d.S.r>...).
+00000c90: 7212 0000 0072 4800 0000 721b 0000 0072  r....rH...r....r
+00000ca0: 1600 0000 7226 0000 0072 4100 0000 7205  ....r&...rA...r.
+00000cb0: 0000 0072 3500 0000 a902 722d 0000 005a  ...r5.....r-...Z
+00000cc0: 0b6d 6f64 756c 655f 7061 7468 7210 0000  .module_pathr...
+00000cd0: 0072 1000 0000 7211 0000 00da 0d67 6f49  .r....r......goI
+00000ce0: 6e4d 6f64 756c 6544 6972 6800 0000 7308  nModuleDirh...s.
+00000cf0: 0000 0000 010a 010c 010c 027a 1653 6865  ...........z.She
+00000d00: 6c6c 4469 722e 676f 496e 4d6f 6475 6c65  llDir.goInModule
+00000d10: 4469 7263 0100 0000 0000 0000 0000 0000  Dirc............
+00000d20: 0100 0000 0200 0000 4300 0000 7314 0000  ........C...s...
+00000d30: 0074 00a0 01a1 0064 0117 007c 0017 0064  .t.....d...|...d
+00000d40: 0217 0053 0029 034e 7246 0000 0072 4400  ...S.).NrF...rD.
+00000d50: 0000 723c 0000 0072 4700 0000 7210 0000  ..r<...rG...r...
+00000d60: 0072 1000 0000 7211 0000 00da 0f67 6574  .r....r......get
+00000d70: 4d6f 6475 6c65 4c69 6244 6972 7000 0000  ModuleLibDirp...
+00000d80: 7302 0000 0000 017a 1853 6865 6c6c 4469  s......z.ShellDi
+00000d90: 722e 6765 744d 6f64 756c 654c 6962 4469  r.getModuleLibDi
+00000da0: 7263 0100 0000 0000 0000 0000 0000 0200  rc..............
+00000db0: 0000 0400 0000 4300 0000 7334 0000 0074  ......C...s4...t
+00000dc0: 00a0 017c 00a1 017d 0174 026a 03a0 047c  ...|...}.t.j...|
+00000dd0: 01a1 0172 2274 02a0 057c 01a1 0101 006e  ...r"t...|.....n
+00000de0: 0e74 06a0 077c 0164 0117 00a1 0101 0064  .t...|.d.......d
+00000df0: 0053 0072 3e00 0000 2908 7212 0000 0072  .S.r>...).r....r
+00000e00: 4b00 0000 721b 0000 0072 1600 0000 7226  K...r....r....r&
+00000e10: 0000 0072 4100 0000 7205 0000 0072 3500  ...rA...r....r5.
+00000e20: 0000 7249 0000 0072 1000 0000 7210 0000  ..rI...r....r...
+00000e30: 0072 1100 0000 da10 676f 496e 4d6f 6475  .r......goInModu
+00000e40: 6c65 4c69 6244 6972 7400 0000 7308 0000  leLibDirt...s...
+00000e50: 0000 010a 010c 010c 027a 1953 6865 6c6c  .........z.Shell
+00000e60: 4469 722e 676f 496e 4d6f 6475 6c65 4c69  Dir.goInModuleLi
+00000e70: 6244 6972 6301 0000 0000 0000 0000 0000  bDirc...........
+00000e80: 0001 0000 0002 0000 0043 0000 0073 1400  .........C...s..
+00000e90: 0000 7400 a001 a100 6401 1700 7c00 1700  ..t.....d...|...
+00000ea0: 6402 1700 5300 2903 4e72 4600 0000 7a0d  d...S.).NrF...z.
+00000eb0: 2f6c 6962 2f74 6466 5f69 6e74 6c72 3c00  /lib/tdf_intlr<.
+00000ec0: 0000 7247 0000 0072 1000 0000 7210 0000  ..rG...r....r...
+00000ed0: 0072 1100 0000 da12 6765 7449 6e4d 6f64  .r......getInMod
+00000ee0: 756c 6549 6e74 6c44 6972 7c00 0000 7302  uleIntlDir|...s.
+00000ef0: 0000 0000 017a 1b53 6865 6c6c 4469 722e  .....z.ShellDir.
+00000f00: 6765 7449 6e4d 6f64 756c 6549 6e74 6c44  getInModuleIntlD
+00000f10: 6972 6301 0000 0000 0000 0000 0000 0002  irc.............
+00000f20: 0000 0004 0000 0043 0000 0073 3400 0000  .......C...s4...
+00000f30: 7400 a001 7c00 a101 7d01 7402 6a03 a004  t...|...}.t.j...
+00000f40: 7c01 a101 7222 7402 a005 7c01 a101 0100  |...r"t...|.....
+00000f50: 6e0e 7406 a007 7c01 6401 1700 a101 0100  n.t...|.d.......
+00000f60: 6400 5300 723e 0000 0029 0872 1200 0000  d.S.r>...).r....
+00000f70: 724d 0000 0072 1b00 0000 7216 0000 0072  rM...r....r....r
+00000f80: 2600 0000 7241 0000 0072 0500 0000 7235  &...rA...r....r5
+00000f90: 0000 0072 4900 0000 7210 0000 0072 1000  ...rI...r....r..
+00000fa0: 0000 7211 0000 00da 1167 6f49 6e4d 6f64  ..r......goInMod
+00000fb0: 756c 6549 6e74 6c44 6972 8000 0000 7308  uleIntlDir....s.
+00000fc0: 0000 0000 010a 010c 010c 027a 1a53 6865  ...........z.She
+00000fd0: 6c6c 4469 722e 676f 496e 4d6f 6475 6c65  llDir.goInModule
+00000fe0: 496e 746c 4469 7263 0000 0000 0000 0000  IntlDirc........
+00000ff0: 0000 0000 0000 0000 0200 0000 4300 0000  ............C...
+00001000: 730c 0000 0074 00a0 01a1 0064 0117 0053  s....t.....d...S
+00001010: 0029 024e 7a10 2f2e 2e2f 2e74 6466 5f66  .).Nz./../.tdf_f
+00001020: 6c75 7474 6572 2902 7212 0000 0072 3d00  lutter).r....r=.
+00001030: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00001040: 0072 1100 0000 da12 6765 7449 6e54 6466  .r......getInTdf
+00001050: 466c 7574 7465 7244 6972 8800 0000 7302  FlutterDir....s.
+00001060: 0000 0000 017a 1b53 6865 6c6c 4469 722e  .....z.ShellDir.
+00001070: 6765 7449 6e54 6466 466c 7574 7465 7244  getInTdfFlutterD
+00001080: 6972 6300 0000 0000 0000 0000 0000 0001  irc.............
+00001090: 0000 0003 0000 0043 0000 0073 2c00 0000  .......C...s,...
+000010a0: 7400 a001 a100 7d00 7402 6a03 a004 7c00  t.....}.t.j...|.
+000010b0: a101 731e 7402 a005 7c00 a101 0100 7402  ..s.t...|.....t.
+000010c0: a006 7c00 a101 0100 6400 5300 7215 0000  ..|.....d.S.r...
+000010d0: 0029 0772 1200 0000 724f 0000 0072 1b00  .).r....rO...r..
+000010e0: 0000 7216 0000 0072 2600 0000 da05 6d6b  ..r....r&.....mk
+000010f0: 6469 7272 4100 0000 7242 0000 0072 1000  dirrA...rB...r..
+00001100: 0000 7210 0000 0072 1100 0000 da11 676f  ..r....r......go
+00001110: 496e 5464 6646 6c75 7474 6572 4469 728c  InTdfFlutterDir.
+00001120: 0000 0073 0800 0000 0001 0801 0c01 0a01  ...s............
+00001130: 7a1a 5368 656c 6c44 6972 2e67 6f49 6e54  z.ShellDir.goInT
+00001140: 6466 466c 7574 7465 7244 6972 6300 0000  dfFlutterDirc...
+00001150: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00001160: 0043 0000 0073 5e00 0000 7400 a001 a100  .C...s^...t.....
+00001170: 0100 7402 6a03 a004 6401 a101 7220 7402  ..t.j...d...r t.
+00001180: a005 6401 a101 0100 6e3a 7402 6a03 a004  ..d.....n:t.j...
+00001190: 6401 a101 735a 7406 6402 8301 7d00 7c00  d...sZt.d...}.|.
+000011a0: 6403 6b02 7248 7402 a007 6401 a101 0100  d.k.rHt...d.....
+000011b0: 6e12 7408 a009 6404 a101 0100 740a 6405  n.t...d.....t.d.
+000011c0: 8301 0100 6400 5300 2906 4eda 0974 6466  ....d.S.).N..tdf
+000011d0: 5f63 6163 6865 7548 0000 00e5 bd93 e589  _cacheuH........
+000011e0: 8de7 9bae e5bd 95e6 b2a1 e69c 89e6 89be  ................
+000011f0: e588 b074 6466 5f63 6163 6865 e7bc 93e5  ...tdf_cache....
+00001200: ad98 e696 87e4 bbb6 e5a4 b9ef bc8c e698  ................
+00001210: afe5 90a6 e588 9be5 bbba efbc 9f28 792f  .............(y/
+00001220: 6e29 3ada 0179 7a16 4f68 2c69 7427 7320  n):..yz.Oh,it's 
+00001230: 6469 7361 7070 6f69 6e74 696e 672e 7208  disappointing.r.
+00001240: 0000 0029 0b72 1200 0000 7243 0000 0072  ...).r....rC...r
+00001250: 1b00 0000 7216 0000 0072 2600 0000 7241  ....r....r&...rA
+00001260: 0000 00da 0569 6e70 7574 7250 0000 0072  .....inputrP...r
+00001270: 0500 0000 7235 0000 00da 0465 7869 7429  ....r5.....exit)
+00001280: 015a 0663 7265 6174 6572 1000 0000 7210  .Z.creater....r.
+00001290: 0000 0072 1100 0000 da0d 676f 5464 6643  ...r......goTdfC
+000012a0: 6163 6865 4469 7293 0000 0073 1200 0000  acheDir....s....
+000012b0: 0001 0801 0c01 0c01 0c01 0801 0801 0c02  ................
+000012c0: 0a01 7a16 5368 656c 6c44 6972 2e67 6f54  ..z.ShellDir.goT
+000012d0: 6466 4361 6368 6544 6972 2902 da09 7961  dfCacheDir)...ya
+000012e0: 6d6c 5f70 6174 6872 1700 0000 6301 0000  ml_pathr....c...
+000012f0: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00001300: 0043 0000 0073 7600 0000 7400 7c00 6401  .C...sv...t.|.d.
+00001310: 6402 6403 8d03 8f54 7d01 7401 a002 7c01  d.d....T}.t...|.
+00001320: a003 a100 a101 7d02 7c02 6400 7501 724a  ......}.|.d.u.rJ
+00001330: 7c02 a004 6404 a101 724a 7c02 6404 1900  |...d...rJ|.d...
+00001340: 7d03 7c03 5700 0200 6400 0400 0400 8303  }.|.W...d.......
+00001350: 0100 5300 7405 a006 6405 a101 0100 5700  ..S.t...d.....W.
+00001360: 6400 0400 0400 8303 0100 6e10 3100 7368  d.........n.1.sh
+00001370: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00001380: 2906 4eda 0172 722a 0000 0072 2b00 0000  ).N..rr*...r+...
+00001390: 7228 0000 0075 5500 0000 e8af bbe5 8f96  r(...uU.........
+000013a0: e5a3 b3e6 a8a1 e59d 97e6 a8a1 e59d 97e5  ................
+000013b0: 908d e5a4 b1e8 b4a5 efbc 8ce8 afb7 e7a1  ................
+000013c0: aee4 bf9d e5a3 b3e6 a8a1 e59d 97e7 9a84  ................
+000013d0: 7075 6273 7065 632e 7961 6d6c e985 8de7  pubspec.yaml....
+000013e0: bdae e4ba 866e 616d 65e5 b19e e680 a729  .....name......)
+000013f0: 0772 3000 0000 7206 0000 0072 3100 0000  .r0...r....r1...
+00001400: da04 7265 6164 7234 0000 0072 0500 0000  ..readr4...r....
+00001410: 7235 0000 0029 0472 5700 0000 5a02 7246  r5...).rW...Z.rF
+00001420: da03 6469 63da 0b73 6865 6c6c 4d6f 6475  ..dic..shellModu
+00001430: 6c65 7210 0000 0072 1000 0000 7211 0000  ler....r....r...
+00001440: 00da 1567 6574 4d6f 6475 6c65 4e61 6d65  ...getModuleName
+00001450: 4672 6f6d 5961 6d6c a000 0000 730c 0000  FromYaml....s...
+00001460: 0000 0110 010e 0112 0108 0112 027a 1e53  .............z.S
+00001470: 6865 6c6c 4469 722e 6765 744d 6f64 756c  hellDir.getModul
+00001480: 654e 616d 6546 726f 6d59 616d 6c4e 2919  eNameFromYamlN).
+00001490: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+000014a0: 1400 0000 da03 7374 72da 0f5f 5f61 6e6e  ......str..__ann
+000014b0: 6f74 6174 696f 6e73 5f5f 7225 0000 0072  otations__r%...r
+000014c0: 2300 0000 7224 0000 0072 0700 0000 7229  #...r$...r....r)
+000014d0: 0000 0072 3b00 0000 723d 0000 0072 4300  ...r;...r=...rC.
+000014e0: 0000 7245 0000 0072 4800 0000 724a 0000  ..rE...rH...rJ..
+000014f0: 0072 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
+00001500: 724e 0000 0072 4f00 0000 7251 0000 0072  rN...rO...rQ...r
+00001510: 5600 0000 725c 0000 0072 1000 0000 7210  V...r\...r....r.
+00001520: 0000 0072 1000 0000 7211 0000 0072 1200  ...r....r....r..
+00001530: 0000 0f00 0000 7326 0000 000a 010c 0208  ......s&........
+00001540: 0810 0810 080e 0d08 190e 0408 0808 0810  ................
+00001550: 040e 0810 040e 080e 040e 0808 0408 0708  ................
+00001560: 0d72 1200 0000 290d da04 656e 756d 7202  .r....)...enumr.
+00001570: 0000 0072 1b00 0000 da12 7464 665f 746f  ...r......tdf_to
+00001580: 6f6c 2e74 6f6f 6c73 2e63 6d64 7203 0000  ol.tools.cmdr...
+00001590: 005a 1274 6466 5f74 6f6f 6c2e 746f 6f6c  .Z.tdf_tool.tool
+000015a0: 732e 656e 7672 0400 0000 da14 7464 665f  s.envr......tdf_
+000015b0: 746f 6f6c 2e74 6f6f 6c73 2e70 7269 6e74  tool.tools.print
+000015c0: 7205 0000 00da 0672 7561 6d65 6c72 0600  r......ruamelr..
+000015d0: 0000 7207 0000 0072 1200 0000 7210 0000  ..r....r....r...
+000015e0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+000015f0: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+00001600: 0000 000c 0108 010c 010c 010c 010c 0310  ................
+00001610: 06                                       .
```

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/bean/deps_item.py` & `tdf_tool-2.4.9/tdf_tool/tools/cli/bean/deps_item.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/module_deps_rewrite.py` & `tdf_tool-2.4.9/tdf_tool/tools/cli/module_deps_rewrite.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/project_cli.py` & `tdf_tool-2.4.9/tdf_tool/tools/cli/project_cli.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cli/utils/yaml_utils.py` & `tdf_tool-2.4.9/tdf_tool/tools/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/cmd.py` & `tdf_tool-2.4.9/tdf_tool/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/config.py` & `tdf_tool-2.4.9/tdf_tool/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/initial_json_config.py` & `tdf_tool-2.4.9/tdf_tool/tools/config/initial_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/module_json_config.py` & `tdf_tool-2.4.9/tdf_tool/tools/config/module_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/config/packages_config.py` & `tdf_tool-2.4.9/tdf_tool/tools/config/packages_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/dependencies_analysis.py` & `tdf_tool-2.4.9/tdf_tool/tools/dependencies_analysis.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/env.py` & `tdf_tool-2.4.9/tdf_tool/tools/env.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_entry.py` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_entry.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint.py` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_lint_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py` & `tdf_tool-2.4.9/tdf_tool/tools/fix_header/fix_header_replace_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/flutter_script.py` & `tdf_tool-2.4.9/tdf_tool/tools/flutter_script.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/gitlab_utils.py` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/gitlab/python_gitlab_api.py` & `tdf_tool-2.4.9/tdf_tool/tools/gitlab/python_gitlab_api.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/module/module_tools.py` & `tdf_tool-2.4.9/tdf_tool/tools/module/module_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/package/seal_off_package_utils.py` & `tdf_tool-2.4.9/tdf_tool/tools/package/seal_off_package_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/platform_tools.py` & `tdf_tool-2.4.9/tdf_tool/tools/platform_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/print.py` & `tdf_tool-2.4.9/tdf_tool/tools/print.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/regular_tool.py` & `tdf_tool-2.4.9/tdf_tool/tools/regular_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/shell_dir.py` & `tdf_tool-2.4.9/tdf_tool/tools/shell_dir.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/file_util.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/file_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/flutter_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/flutter_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/ios_translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/ios_translate_lint.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/ios_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_module.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/location_string_temp.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/podspec.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/podspec.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/ios/tools/string_util.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/ios/tools/string_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/tools/translate_tool.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/tools/translate_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/translate/translate_lint.py` & `tdf_tool-2.4.9/tdf_tool/tools/translate/translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc` & `tdf_tool-2.4.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.4.8/PKG-INFO` & `tdf_tool-2.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdf_tool
-Version: 2.4.8
+Version: 2.4.9
 Summary: 二维火 flutter 脚手架工具
 Home-page: https://git.2dfire.net/app/flutter/tools/package_tools
 License: MIT
 Keywords: tdf,tdf-tool,tdf_tool
 Author: Jian Xu
 Author-email: 3386218996@qq.com
 Requires-Python: >=3.9.0,<4.0.0
```

