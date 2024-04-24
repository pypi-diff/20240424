# Comparing `tmp/pyodide_mkdocs_theme-0.3.1.tar.gz` & `tmp/pyodide_mkdocs_theme-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide_mkdocs_theme-0.3.1.tar", max compression
+gzip compressed data, was "pyodide_mkdocs_theme-0.3.2.tar", max compression
```

## Comparing `pyodide_mkdocs_theme-0.3.1.tar` & `pyodide_mkdocs_theme-0.3.2.tar`

### file list

```diff
@@ -1,74 +1,75 @@
--rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.1/LICENSE
--rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.1/README.md
--rw-r--r--   0        0        0     1347 2024-04-18 21:28:53.878591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__init__.py
--rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__main__.py
--rw-r--r--   0        0        0       22 2024-04-18 21:28:53.914592 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__version__.py
--rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py
--rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
--rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
--rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
--rw-r--r--   0        0        0     4991 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
--rw-r--r--   0        0        0    21241 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
--rw-r--r--   0        0        0    14750 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
--rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
--rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
--rw-r--r--   0        0        0    11548 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
--rw-r--r--   0        0        0    13167 2024-04-18 21:28:32.174075 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/messages.py
--rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
--rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py
--rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
--rw-r--r--   0        0        0    11594 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
--rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
--rw-r--r--   0        0        0    13039 2024-04-18 09:36:07.501012 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
--rw-r--r--   0        0        0     1711 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
--rw-r--r--   0        0        0     3236 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
--rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
--rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
--rw-r--r--   0        0        0     1064 2024-04-18 21:28:53.870591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
--rw-r--r--   0        0        0     6881 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
--rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang.py
--rw-r--r--   0        0        0     3983 2024-04-18 21:28:53.878591 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py
--rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
--rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/__init__.py
--rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
--rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
--rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
--rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
--rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
--rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
--rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/main.html
--rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
--rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/copyright.html
--rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/footer.html
--rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/social.html
--rw-r--r--   0        0        0     9780 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
--rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
--rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
--rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
--rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
--rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
--rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
--rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
--rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
--rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
--rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
--rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
--rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
--rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
--rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
--rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
--rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
--rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
--rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
--rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
--rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
--rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
--rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
--rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
--rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
--rw-r--r--   0        0        0     1775 2024-04-18 21:28:50.330507 pyodide_mkdocs_theme-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35118 2024-04-04 09:39:00.129784 pyodide_mkdocs_theme-0.3.2/LICENSE
+-rwxr-xr-x   0        0        0     1337 2024-04-08 19:01:06.251164 pyodide_mkdocs_theme-0.3.2/README.md
+-rw-r--r--   0        0        0     1347 2024-04-24 20:07:39.566584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-24 20:07:39.602585 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__version__.py
+-rw-r--r--   0        0        0      807 2024-04-12 21:48:00.494695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-24 20:07:39.554583 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/deprecation.py
+-rw-r--r--   0        0        0      856 2024-04-04 09:56:58.098963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py
+-rw-r--r--   0        0        0     1190 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py
+-rw-r--r--   0        0        0     4974 2024-04-11 09:41:00.019938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py
+-rw-r--r--   0        0        0     4991 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py
+-rw-r--r--   0        0        0    21241 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py
+-rw-r--r--   0        0        0    14750 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py
+-rw-r--r--   0        0        0      689 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-04 09:56:58.102963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py
+-rw-r--r--   0        0        0     4093 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py
+-rw-r--r--   0        0        0    11548 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py
+-rw-r--r--   0        0        0    13167 2024-04-18 21:29:06.622893 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/messages.py
+-rw-r--r--   0        0        0     6945 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py
+-rw-r--r--   0        0        0     4237 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py
+-rw-r--r--   0        0        0     4462 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py
+-rw-r--r--   0        0        0    11593 2024-04-19 07:02:56.611776 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py
+-rw-r--r--   0        0        0    11690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py
+-rw-r--r--   0        0        0    13035 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py
+-rw-r--r--   0        0        0     1711 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py
+-rw-r--r--   0        0        0     2877 2024-04-19 06:57:28.632698 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py
+-rw-r--r--   0        0        0     9974 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py
+-rw-r--r--   0        0        0     2658 2024-04-11 09:41:00.023938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py
+-rw-r--r--   0        0        0     1064 2024-04-24 20:07:39.558584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py
+-rw-r--r--   0        0        0     6881 2024-04-19 06:57:41.645164 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py
+-rw-r--r--   0        0        0      690 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang.py
+-rw-r--r--   0        0        0     3983 2024-04-24 20:07:39.566584 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang_src.py
+-rw-r--r--   0        0        0     5490 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py
+-rw-r--r--   0        0        0      690 2024-04-04 09:56:58.106963 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js
+-rw-r--r--   0        0        0     7349 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js
+-rw-r--r--   0        0        0     1675 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js
+-rw-r--r--   0        0        0     1490 2024-04-09 19:35:36.230493 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js
+-rw-r--r--   0        0        0     4320 2024-04-12 21:48:00.498695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js
+-rw-r--r--   0        0        0     1078 2024-04-10 12:36:30.998040 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css
+-rw-r--r--   0        0        0     6426 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/main.html
+-rw-r--r--   0        0        0     1924 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml
+-rw-r--r--   0        0        0      802 2024-04-03 22:13:32.135114 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/copyright.html
+-rw-r--r--   0        0        0     2084 2024-04-03 21:47:24.620870 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/footer.html
+-rw-r--r--   0        0        0      578 2024-04-03 22:14:08.956199 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/social.html
+-rw-r--r--   0        0        0     9780 2024-04-24 20:05:58.907628 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js
+-rw-r--r--   0        0        0     5935 2024-04-04 09:56:58.174965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js
+-rw-r--r--   0        0        0     3459 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css
+-rw-r--r--   0        0        0     1645 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png
+-rw-r--r--   0        0        0     1328 2024-03-05 12:41:09.845669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png
+-rw-r--r--   0        0        0     1761 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png
+-rw-r--r--   0        0        0     1283 2024-03-05 12:41:09.849669 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png
+-rw-r--r--   0        0        0      952 2024-03-05 12:41:09.857670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png
+-rw-r--r--   0        0        0     1296 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png
+-rw-r--r--   0        0        0     1702 2024-04-04 09:56:58.190965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js
+-rw-r--r--   0        0        0      823 2024-03-04 14:13:04.212401 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md
+-rw-r--r--   0        0        0     6600 2024-04-12 21:48:00.502695 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js
+-rw-r--r--   0        0        0    16559 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js
+-rw-r--r--   0        0        0     9657 2024-04-04 09:56:58.138964 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js
+-rw-r--r--   0        0        0      252 2024-03-05 12:41:09.861670 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/README.md
+-rw-r--r--   0        0        0     1947 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css
+-rw-r--r--   0        0        0     9150 2024-04-07 12:16:07.568974 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js
+-rw-r--r--   0        0        0     3629 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css
+-rw-r--r--   0        0        0     1651 2024-04-14 07:06:03.108780 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css
+-rw-r--r--   0        0        0     5373 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js
+-rw-r--r--   0        0        0     4218 2024-04-11 09:41:00.027938 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js
+-rw-r--r--   0        0        0     1478 2024-04-04 09:56:58.198965 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js
+-rw-r--r--   0        0        0     2857 2024-03-25 22:17:16.937424 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg
+-rw-r--r--   0        0        0     3774 2024-04-14 12:10:19.820826 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css
+-rw-r--r--   0        0        0    12716 2024-04-14 21:38:49.051576 pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js
+-rw-r--r--   0        0        0     1775 2024-04-24 20:07:36.178484 pyodide_mkdocs_theme-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 pyodide_mkdocs_theme-0.3.2/PKG-INFO
```

### Comparing `pyodide_mkdocs_theme-0.3.1/LICENSE` & `pyodide_mkdocs_theme-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/README.md` & `pyodide_mkdocs_theme-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/__main__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/exceptions.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/html_builder/_html_builder.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/IDEs/ide_files_data.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/autres.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/isolated_components.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/macros/qcm.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/messages.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/messages.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pages_and_ides_configs.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/parsing.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/parsing.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/paths_utils.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 from mkdocs.config.base import Config
 from mkdocs.config import config_options as C
-
 from mkdocs_macros.plugin import MacrosPlugin
-from .maestro_tools import typ_deprecated_with_custom_msg
+
+from ..deprecation import typ_deprecated_with_custom_msg
```

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_IDE.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_base_and_indent.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from pathlib import Path
 
 from mkdocs.plugins import BasePlugin
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 from mkdocs.exceptions import BuildError
 
-from pyodide_mkdocs_theme.pyodide_macros.messages import Lang, Msg, Tip
+from ..deprecation import deprecation_warning
+from ..messages import Lang, Msg, Tip
 
 from ...__version__ import __version__
 from ..tools_and_constants import PageUrl
 from ..pyodide_logger import logger
 from ..parsing import eat
 
 from .maestro_tools import ConfigExtractor
@@ -186,19 +187,18 @@
             logger.error("Breakpoint! (the CALL to this method should be removed)")
 
 
     def warn_unmaintained(self, that:str):
         """
         Generic warning message for people trying to used untested/unmaintained macros.
         """
-        logger.warning(
+        deprecation_warning(
             f"{ that.capitalize() } has not been maintained since the original pyodide-mkdocs "
-            "project and may not currently work.\n"
-            "Please open an issue on the pyodide-mkdocs-theme repository, providing a concrete "
-            "use case so that it can be updated.\n\n"
+            "project, may not currently work, and will be deprecated in the future.\n"
+            "Please open an issue on the pyodide-mkdocs-theme repository, if you need it.\n\n"
             f"\t{ self.pmt_url }"
         )
```

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_extras.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/maestro_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,23 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.
 If not, see <https://www.gnu.org/licenses/>.
 """
 
 
-import json
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
-from mkdocs.config import config_options as C
-
-from pyodide_mkdocs_theme.pyodide_macros.parsing import camel
+from ..parsing import camel
 
 if TYPE_CHECKING:
     from .pyodide_macros_plugin import PyodideMacrosPlugin
 
 
 
-def typ_deprecated_with_custom_msg(prop:str, typ:Any):
-    return C.Deprecated(
-        message=f"Macros using {prop} may not work anymore. "
-                "Please contact the theme author about that.",
-        option_type = C.Optional(C.Type(typ)),
-    )
-
-
-
 
 class ConfigExtractor:
     """
     Data descriptor extracting automatically the matching property name from the mkdocs config.
     An additional path (dot separated keys/properties) can be provided, that will be prepended
     to the property name.
     """
```

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/plugin/pyodide_macros_plugin.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/pyodide_logger.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/scripts_templates.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/pyodide_macros/tools_and_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 
 class AutoDescriptor:
     """ StrEnum-like property for py3.11-
         If the item string doesn't match the name anymore, one can set the wanted name
         through the constructor, without changing the property name (but F2 will most
-        likely also do the trick... Unless string content is actually used somewhere...)
+        likely also do the trick... Unless string version is actually used somewhere...)
     """
 
     def __init__(self, prop:str=None):      # allow to override the property name,
         self._prop = prop
 
     def __set_name__(self, _, prop:str):
         self._prop = self._prop or prop
```

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/custom_lang_src.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/custom_lang_src.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/scripts/mkdocs_yaml.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/__init__.py` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/0_config-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/functools-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/jsLogger-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/mathjax-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/securedPagesData-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_globalGuiButtons-libs.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/js-libs/z_header-btns-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/main.html` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/main.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/mkdocs_theme.yml` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/mkdocs_theme.yml`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/copyright.html` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/footer.html` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/footer.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/partials/social.html` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/partials/social.html`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/0_buttonsAndCounter-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ace-editor-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/ide-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-check-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-download-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-play-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-restart-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-save-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/images/icons8-upload-64.png`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/IDE-and-buttons/z_doLast-subscriptions-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/README.md`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/0_tasks-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/actions/genericCodeRunner-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/error-logs-generator-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/perPageScripts/start-pyodide.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/pyoditeur-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/css/terminal-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-helpers-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/pyodide-mkdocs/terminal/z_doLast_terminal-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/.qcm-circle.svg`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-libs.css`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js` & `pyodide_mkdocs_theme-0.3.2/pyodide_mkdocs_theme/templates/qcm/qcm-scripts.js`

 * *Files identical despite different names*

### Comparing `pyodide_mkdocs_theme-0.3.1/pyproject.toml` & `pyodide_mkdocs_theme-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyodide-mkdocs-theme"
-version = "0.3.1"
+version = "0.3.2"
 description = "Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations"
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
 readme = "README.md"
 keywords = [
     "mkdocs", "mkdocs-plugin", "pyodide", "IDE", "terminal"
 ]
 classifiers = [
```

### Comparing `pyodide_mkdocs_theme-0.3.1/PKG-INFO` & `pyodide_mkdocs_theme-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-mkdocs-theme
-Version: 0.3.1
+Version: 0.3.2
 Summary: Package embedding the necessary tools to host pyodide, ACE editors, jQuery terminals in mkdocs documentations
 Keywords: mkdocs,mkdocs-plugin,pyodide,IDE,terminal
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

