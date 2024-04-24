# Comparing `tmp/extract_drugs-1.2.0.tar.gz` & `tmp/extract_drugs-1.3.0.tar.gz`

## Comparing `extract_drugs-1.2.0.tar` & `extract_drugs-1.3.0.tar`

### file list

```diff
@@ -1,773 +1,10 @@
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 extract_drugs-1.2.0/Cargo.toml
--rw-r--r--   0      501       20      287 2023-05-30 02:55:34.000000 extract_drugs-1.2.0/.gitignore
--rw-r--r--   0      501       20     9033 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/Activate.ps1
--rw-r--r--   0      501       20     2029 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/activate
--rw-r--r--   0      501       20      955 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/activate.csh
--rw-r--r--   0      501       20     2235 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/activate.fish
--rwxr-xr-x   0      501       20  1485408 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/bin/extract-drugs
--rwxr-xr-x   0      501       20      280 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/pip
--rwxr-xr-x   0      501       20      280 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/pip3
--rwxr-xr-x   0      501       20      280 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/bin/pip3.11
--rwxr-xr-x   0      501       80    52640 2024-01-12 17:08:25.000000 extract_drugs-1.2.0/.venv/bin/python
--rwxr-xr-x   0      501       80    52640 2024-01-12 17:08:25.000000 extract_drugs-1.2.0/.venv/bin/python3
--rwxr-xr-x   0      501       80    52640 2024-01-12 17:08:25.000000 extract_drugs-1.2.0/.venv/bin/python3.11
--rw-r--r--   0      501       20     6128 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0      501       20       44 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/_distutils_hack/override.py
--rw-r--r--   0      501       20      151 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/distutils-precedence.pth
--rw-r--r--   0      501       20        4 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/INSTALLER
--rw-r--r--   0      501       20     6251 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/METADATA
--rw-r--r--   0      501       20      717 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/RECORD
--rw-r--r--   0      501       20        0 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/REQUESTED
--rw-r--r--   0      501       20      101 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/WHEEL
--rw-r--r--   0      501       20      148 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/direct_url.json
--rw-r--r--   0      501       20     1053 2024-01-12 17:10:29.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/license_files/LICENSE.md
--rw-r--r--   0      501       20      357 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/__init__.py
--rw-r--r--   0      501       20     1198 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/__main__.py
--rw-r--r--   0      501       20     1444 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/__pip-runner__.py
--rw-r--r--   0      501       20      573 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-r--r--   0      501       20    10243 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-r--r--   0      501       20    10734 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cache.py
--rw-r--r--   0      501       20      132 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0      501       20     6676 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0      501       20     7842 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0      501       20    29497 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0      501       20      774 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0      501       20     2472 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0      501       20     4338 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0      501       20    10817 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0      501       20     1968 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0      501       20    18172 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0      501       20     5118 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0      501       20      116 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0      501       20     3882 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0      501       20     7582 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0      501       20     1685 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0      501       20     4129 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0      501       20     9815 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0      501       20     6591 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0      501       20     5289 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0      501       20     2951 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0      501       20     1703 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0      501       20     1132 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0      501       20     4793 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0      501       20     3188 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0      501       20    32389 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0      501       20    12343 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0      501       20     5697 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0      501       20     6419 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0      501       20     3886 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0      501       20     7396 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0      501       20    13529 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/configuration.py
--rw-r--r--   0      501       20      858 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0      501       20     1221 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0      501       20      729 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0      501       20     6494 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0      501       20     1164 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0      501       20    24244 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0      501       20       30 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0      501       20    16504 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0      501       20    37873 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0      501       20     6557 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0      501       20    15365 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0      501       20     6100 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0      501       20     7680 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0      501       20     2556 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0      501       20      340 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/main.py
--rw-r--r--   0      501       20     4280 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0      501       20     2595 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0      501       20    25277 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0      501       20      107 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0      501       20     1882 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0      501       20     8181 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0      501       20     7457 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0      501       20     9773 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0      501       20       63 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0      501       20      990 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0      501       20     6626 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0      501       20     2520 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0      501       20     1030 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-r--r--   0      501       20     2617 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0      501       20    18602 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-r--r--   0      501       20      738 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0      501       20     4644 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0      501       20     1907 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0      501       20     3858 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0      501       20     3600 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0      501       20       50 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0      501       20    16507 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0      501       20     2145 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0      501       20     6096 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-r--r--   0      501       20     7638 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0      501       20    18443 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-r--r--   0      501       20     4073 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0      501       20     1791 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0      501       20     4133 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0      501       20     1422 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0      501       20     1474 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0      501       20     2198 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0      501       20     1075 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0      501       20     1417 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0      501       20     3064 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0      501       20     5122 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0      501       20     9784 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0      501       20       51 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0      501       20     1354 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0      501       20     4105 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0      501       20    27407 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0      501       20    25091 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0      501       20     6987 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0      501       20     2807 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0      501       20    16611 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0      501       20    17646 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0      501       20    35763 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0      501       20     2858 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0      501       20    24045 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0      501       20      583 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0      501       20    24129 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0      501       20     5220 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0      501       20    18963 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0      501       20    27878 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0      501       20     5705 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0      501       20     9914 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0      501       20     2526 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0      501       20     5455 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0      501       20    11533 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0      501       20     8167 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0      501       20     1015 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0      501       20     1665 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0      501       20     1884 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0      501       20     5377 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0      501       20      242 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0      501       20     5764 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0      501       20     3206 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0      501       20     1115 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0      501       20     2118 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0      501       20     1169 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0      501       20     3064 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0      501       20     5122 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0      501       20      716 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0      501       20     3110 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0      501       20     4831 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0      501       20      795 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0      501       20    11632 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0      501       20    22253 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0      501       20     1193 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0      501       20     2108 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0      501       20     5662 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0      501       20     9200 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0      501       20     7702 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0      501       20     8821 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0      501       20     1759 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0      501       20     3456 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0      501       20     4549 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0      501       20      596 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0      501       20     3519 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0      501       20    18116 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0      501       20     5238 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0      501       20    11729 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0      501       20    22811 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0      501       20    13079 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0      501       20     4966 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0      501       20      465 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0      501       20     1379 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0      501       20     5033 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0      501       20     1535 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0      501       20      242 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0      501       20     5271 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0      501       20     1033 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0      501       20      778 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0      501       20    16416 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0      501       20     3946 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0      501       20     4154 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0      501       20     7105 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0      501       20      774 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0      501       20       94 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0      501       20      255 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0      501       20   275233 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0      501       20     4279 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0      501       20     4797 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0      501       20    31274 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0      501       20     1763 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0      501       20    10032 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0      501       20     3915 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0      501       20     5420 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0      501       20     3242 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0      501       20     3732 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0      501       20      542 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0      501       20     1860 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0      501       20     1683 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0      501       20     4006 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0      501       20    12176 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0      501       20     3934 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0      501       20    13566 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0      501       20     1753 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0      501       20    36913 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0      501       20     1753 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0      501       20    20735 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0      501       20     1759 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0      501       20    14537 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0      501       20    25796 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0      501       20    42498 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0      501       20     1752 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0      501       20    27055 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0      501       20   104562 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0      501       20    98484 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0      501       20    98196 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0      501       20   101363 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0      501       20   128035 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0      501       20   102774 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0      501       20    95372 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0      501       20     5380 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0      501       20     6077 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0      501       20     3715 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0      501       20     2131 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0      501       20    30391 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0      501       20    13560 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0      501       20      402 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0      501       20     6400 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0      501       20     4137 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0      501       20     4007 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0      501       20    14848 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0      501       20     8505 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0      501       20     2812 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0      501       20      244 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0      501       20      266 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0      501       20     2522 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0      501       20    11128 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0      501       20     3325 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0      501       20       75 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0      501       20     2839 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0      501       20    10678 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0      501       20     6741 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0      501       20     1866 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0      501       20     1079 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0      501       20     3709 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0      501       20     6181 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0      501       20     7134 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0      501       20      581 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0      501       20    41259 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0      501       20    51697 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0      501       20    20834 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0      501       20    51991 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0      501       20    14811 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0      501       20     5058 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0      501       20    39801 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0      501       20    10820 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0      501       20    18102 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0      501       20    97792 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0      501       20   182784 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0      501       20   108032 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0      501       20    66262 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0      501       20    23513 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0      501       20    91648 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0      501       20   168448 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0      501       20   101888 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0      501       20    43898 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0      501       20      981 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0      501       20       64 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0      501       20    49330 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0      501       20      849 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0      501       20     3374 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0      501       20      321 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0      501       20    12950 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0      501       20    44375 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0      501       20     1881 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0      501       20       21 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0      501       20   206539 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0      501       20     1132 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0      501       20     1081 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0      501       20     6080 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0      501       20    34557 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0      501       20      661 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0      501       20      497 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20    11488 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0      501       20     4378 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0      501       20     1431 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     8487 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     4676 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    30110 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20    15699 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0      501       20     4200 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    14665 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0      501       20   108287 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0      501       20      562 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0      501       20    12936 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0      501       20     1176 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0      501       20     4068 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0      501       20     4910 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0      501       20     2655 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0      501       20     6911 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0      501       20      160 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0      501       20     6596 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0      501       20     2999 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0      501       20      353 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0      501       20    23685 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0      501       20     1697 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0      501       20     1938 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0      501       20    40386 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0      501       20     2917 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0      501       20     4810 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0      501       20     4104 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0      501       20     3314 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0      501       20     5086 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0      501       20    35441 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0      501       20    21938 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0      501       20     5871 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0      501       20    19351 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0      501       20     5073 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0      501       20     2212 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0      501       20     5014 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0      501       20     7335 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0      501       20     4674 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0      501       20    11753 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0      501       20    32005 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0      501       20    11174 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0      501       20    70232 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0      501       20    53376 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0      501       20      986 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0      501       20     2591 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0      501       20     3072 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0      501       20     3092 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0      501       20     4630 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0      501       20     6257 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0      501       20     3419 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0      501       20     6184 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0      501       20    63187 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0      501       20     9110 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0      501       20     9171 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0      501       20     6426 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0      501       20    12936 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0      501       20   213344 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0      501       20    23685 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0      501       20     9023 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0      501       20    39129 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0      501       20    25341 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0      501       20    13402 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0      501       20    10787 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0      501       20     6805 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0      501       20      491 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0      501       20      138 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0      501       20    11920 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0      501       20      546 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0      501       20    10927 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0      501       20     5178 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0      501       20      435 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0      501       20     1397 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0      501       20    21443 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0      501       20     6377 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0      501       20    10187 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0      501       20      575 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0      501       20     1286 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0      501       20    18560 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0      501       20     3823 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0      501       20     3879 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0      501       20      733 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0      501       20    35288 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0      501       20      695 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0      501       20    30180 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0      501       20     4235 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0      501       20     2912 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0      501       20    33240 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0      501       20      537 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0      501       20      156 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0      501       20     5872 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0      501       20     1583 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0      501       20    17592 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0      501       20     4794 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0      501       20     6090 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0      501       20     8478 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0      501       20    10096 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0      501       20   140235 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0      501       20     1064 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0      501       20     2114 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0      501       20      265 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0      501       20     9695 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0      501       20     3225 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0      501       20     1236 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0      501       20     1643 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0      501       20     7063 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0      501       20      423 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0      501       20     5472 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0      501       20    19919 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0      501       20      351 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0      501       20      417 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0      501       20    22820 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0      501       20     1926 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0      501       20     2783 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0      501       20     1840 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0      501       20      890 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0      501       20    10368 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0      501       20     6819 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0      501       20     3264 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0      501       20     9842 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0      501       20     4503 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0      501       20    18015 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0      501       20     1054 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0      501       20     7131 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0      501       20    97992 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0      501       20     1288 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0      501       20     5497 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0      501       20     6630 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0      501       20     7954 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0      501       20      972 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0      501       20     2501 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0      501       20      642 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0      501       20     1616 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0      501       20     2508 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0      501       20     9585 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0      501       20     5053 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0      501       20     3252 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0      501       20    14007 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0      501       20    14172 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0      501       20     3667 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0      501       20    11903 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0      501       20     8198 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0      501       20     5305 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0      501       20     4970 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0      501       20      828 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0      501       20     3396 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0      501       20    10574 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0      501       20    37414 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0      501       20    59836 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0      501       20     8165 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0      501       20    11303 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0      501       20     1391 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0      501       20      166 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0      501       20     4436 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0      501       20     4773 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0      501       20     2843 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0      501       20     1591 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0      501       20    24224 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0      501       20     4374 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0      501       20     4425 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0      501       20    26332 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0      501       20     1258 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0      501       20    34995 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0      501       20    39684 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0      501       20     3370 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0      501       20    45686 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0      501       20     3627 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0      501       20      102 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0      501       20    26070 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0      501       20     9169 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0      501       20    34549 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/six.py
--rw-r--r--   0      501       20    18364 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0      501       20     3314 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0      501       20     1944 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0      501       20     1496 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0      501       20     1376 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0      501       20     1908 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0      501       20     1383 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0      501       20     7550 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0      501       20     2790 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0      501       20     2145 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0      501       20     8011 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0      501       20      396 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0      501       20    22633 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0      501       20     2943 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0      501       20      254 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0      501       20    80114 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0      501       20     3333 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0      501       20    10811 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0      501       20       64 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0      501       20    20070 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0      501       20    39095 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0      501       20      957 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0      501       20    17632 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0      501       20    13922 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0      501       20    11036 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0      501       20     4528 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0      501       20    17081 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0      501       20    34448 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0      501       20     7097 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0      501       20     8217 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0      501       20     8579 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0      501       20     2440 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0      501       20     1417 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0      501       20    34665 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0      501       20    19786 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0      501       20     5985 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0      501       20    30641 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0      501       20     1155 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0      501       20     4901 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0      501       20     1605 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0      501       20      498 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0      501       20     3997 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0      501       20     3510 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0      501       20    22003 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0      501       20    17177 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0      501       20     5758 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0      501       20     6895 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0      501       20    10003 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0      501       20    14298 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0      501       20     5403 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0      501       20      476 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0      501       20    10579 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0      501       20     8979 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0      501       20     1305 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0      501       20     6563 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0      501       20     4307 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0      501       20      286 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/py.typed
--rw-r--r--   0      501       20        4 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/INSTALLER
--rw-r--r--   0      501       20     1093 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--   0      501       20     4072 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/METADATA
--rw-r--r--   0      501       20    77163 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/RECORD
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/REQUESTED
--rw-r--r--   0      501       20       92 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/WHEEL
--rw-r--r--   0      501       20      125 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-r--r--   0      501       20        4 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--   0      501       20   109315 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/__init__.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0      501       20      506 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0      501       20     4504 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0      501       20     5457 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0      501       20     2925 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0      501       20      884 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0      501       20     3481 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0      501       20     5140 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0      501       20     3581 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0      501       20     2576 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0      501       20     7460 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0      501       20    13515 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0      501       20    15526 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0      501       20      148 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0      501       20   133344 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0      501       20    22975 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0      501       20      501 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20     3266 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-r--r--   0      501       20     8813 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0      501       20     2524 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0      501       20     9399 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-r--r--   0      501       20     1431 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     5148 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-r--r--   0      501       20     8161 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     3264 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    39046 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20    18065 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0      501       20     4355 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    16295 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0      501       20    12806 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-r--r--   0      501       20     1164 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-r--r--   0      501       20     4068 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-r--r--   0      501       20     4910 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-r--r--   0      501       20     2655 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-r--r--   0      501       20     6911 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-r--r--   0      501       20      160 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-r--r--   0      501       20     6596 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-r--r--   0      501       20    80078 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-r--r--   0      501       20     8425 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0      501       20     2442 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0      501       20     9170 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/__init__.py
--rw-r--r--   0      501       20      218 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0      501       20      359 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0      501       20     5300 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0      501       20      411 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0      501       20       43 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
--rw-r--r--   0      501       20      239 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0      501       20    19616 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0      501       20     8572 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0      501       20    14721 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0      501       20    48643 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0      501       20    17861 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0      501       20      430 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0      501       20     1614 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0      501       20     5408 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0      501       20     4665 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0      501       20    22013 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0      501       20     5584 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0      501       20     7684 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0      501       20    31503 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0      501       20    16537 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0      501       20     5604 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0      501       20     4872 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0      501       20     2594 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0      501       20    13077 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0      501       20    30153 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0      501       20     2762 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0      501       20     2788 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0      501       20     1180 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0      501       20     8409 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0      501       20     1932 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0      501       20      672 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0      501       20    11817 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0      501       20    19232 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0      501       20     7491 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0      501       20     4911 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0      501       20     9397 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0      501       20    11924 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0      501       20      139 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0      501       20     3414 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0      501       20     8072 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0      501       20    50174 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0      501       20     3589 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0      501       20    10270 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0      501       20    17899 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0      501       20     8212 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0      501       20    13715 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0      501       20     1201 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0      501       20    30188 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0      501       20    23577 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0      501       20      217 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0      501       20      639 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0      501       20     3495 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0      501       20    18928 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0      501       20    12085 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0      501       20    15601 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0      501       20    18099 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0      501       20    12951 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0      501       20     5205 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0      501       20     2282 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-r--r--   0      501       20     2392 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_imp.py
--rw-r--r--   0      501       20     1311 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-r--r--   0      501       20      675 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-r--r--   0      501       20     3722 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_normalization.py
--rw-r--r--   0      501       20     1056 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_path.py
--rw-r--r--   0      501       20      882 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_reqs.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0      501       20    26498 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0      501       20     2454 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0      501       20      743 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0      501       20     1859 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0      501       20     2895 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0      501       20     2068 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0      501       20     1165 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0      501       20     1098 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-r--r--   0      501       20     2166 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0      501       20      506 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0      501       20     4504 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0      501       20     5457 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0      501       20     2925 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0      501       20      884 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0      501       20     3481 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0      501       20     5140 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0      501       20     3581 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0      501       20     2576 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0      501       20        0 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0      501       20     7460 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0      501       20    13512 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0      501       20    15517 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0      501       20       82 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0      501       20   117959 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0      501       20    16256 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0      501       20    15130 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0      501       20      501 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0      501       20     3266 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-r--r--   0      501       20     8813 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0      501       20     2524 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0      501       20     9399 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-r--r--   0      501       20     1431 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0      501       20     5148 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-r--r--   0      501       20     8161 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0      501       20     3264 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0      501       20    39046 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0      501       20    18065 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0      501       20     4355 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0      501       20    16295 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0      501       20      396 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0      501       20    22633 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0      501       20     2943 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0      501       20      254 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0      501       20    87149 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0      501       20     8425 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0      501       20     7346 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-r--r--   0      501       20    19612 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/build_meta.py
--rw-r--r--   0      501       20    65536 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/cli-32.exe
--rw-r--r--   0      501       20    74752 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/cli-64.exe
--rw-r--r--   0      501       20   137216 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0      501       20    65536 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/cli.exe
--rw-r--r--   0      501       20      396 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-r--r--   0      501       20     2381 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-r--r--   0      501       20    16596 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0      501       20     1182 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0      501       20     6589 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/build.py
--rw-r--r--   0      501       20     4423 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0      501       20    15821 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0      501       20    14115 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-r--r--   0      501       20     6963 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-r--r--   0      501       20     4074 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0      501       20    85662 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0      501       20    31903 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0      501       20    28176 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0      501       20     5163 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/install.py
--rw-r--r--   0      501       20     2123 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0      501       20     3875 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0      501       20     2714 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0      501       20      628 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0      501       20     4946 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0      501       20      468 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/register.py
--rw-r--r--   0      501       20     2128 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-r--r--   0      501       20      658 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0      501       20     7071 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-r--r--   0      501       20     5086 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-r--r--   0      501       20     8102 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/test.py
--rw-r--r--   0      501       20      462 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-r--r--   0      501       20     7470 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0      501       20     1121 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-r--r--   0      501       20    13816 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0      501       20     1038 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0      501       20    11266 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0      501       20     1153 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0      501       20     1612 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0      501       20   274907 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0      501       20     9161 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0      501       20    16319 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-r--r--   0      501       20    19598 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0      501       20    25431 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0      501       20      949 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-r--r--   0      501       20     5499 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/depends.py
--rw-r--r--   0      501       20    21087 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/discovery.py
--rw-r--r--   0      501       20    45710 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/dist.py
--rw-r--r--   0      501       20     2464 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/errors.py
--rw-r--r--   0      501       20     5591 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/extension.py
--rw-r--r--   0      501       20     2527 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0      501       20     4873 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/glob.py
--rw-r--r--   0      501       20    65536 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/gui-32.exe
--rw-r--r--   0      501       20    75264 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/gui-64.exe
--rw-r--r--   0      501       20   137728 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0      501       20    65536 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/gui.exe
--rw-r--r--   0      501       20     5063 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/installer.py
--rw-r--r--   0      501       20      812 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/launch.py
--rw-r--r--   0      501       20     1232 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/logging.py
--rw-r--r--   0      501       20     4697 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/monkey.py
--rw-r--r--   0      501       20    47115 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/msvc.py
--rw-r--r--   0      501       20     3093 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-r--r--   0      501       20    39682 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/package_index.py
--rw-r--r--   0      501       20      245 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/py34compat.py
--rw-r--r--   0      501       20    14348 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-r--r--   0      501       20      218 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0      501       20      138 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/script.tmpl
--rw-r--r--   0      501       20      941 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0      501       20      134 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/version.py
--rw-r--r--   0      501       20     8608 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/wheel.py
--rw-r--r--   0      501       20      718 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools/windows_support.py
--rw-r--r--   0      501       20        4 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/INSTALLER
--rw-r--r--   0      501       20     1050 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/LICENSE
--rw-r--r--   0      501       20     6213 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/METADATA
--rw-r--r--   0      501       20    36539 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/RECORD
--rw-r--r--   0      501       20        0 2023-08-25 19:53:35.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/REQUESTED
--rw-r--r--   0      501       20       92 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/WHEEL
--rw-r--r--   0      501       20     2740 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/entry_points.txt
--rw-r--r--   0      501       20       41 2023-08-25 19:53:34.000000 extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/setuptools-67.6.1.dist-info/top_level.txt
--rw-r--r--   0      501       20      331 2023-08-25 19:53:33.000000 extract_drugs-1.2.0/.venv/pyvenv.cfg
--rw-r--r--   0      501       20     4106 2022-06-27 14:19:06.000000 extract_drugs-1.2.0/CONTRIBUTING.md
--rw-r--r--   0      501       20    18801 2024-01-12 17:16:44.000000 extract_drugs-1.2.0/Cargo.lock
--rw-r--r--   0      501       20     1053 2023-05-30 03:02:23.000000 extract_drugs-1.2.0/LICENSE.md
--rw-r--r--   0      501       20     5224 2023-05-30 02:55:34.000000 extract_drugs-1.2.0/README.md
--rw-r--r--   0      501       20    17555 2023-09-12 18:55:35.000000 extract_drugs-1.2.0/src/lib.rs
--rw-r--r--   0      501       20     4329 2023-05-30 02:55:34.000000 extract_drugs-1.2.0/src/main.rs
--rw-r--r--   0      501       20     1025 2024-01-12 17:16:30.000000 extract_drugs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 extract_drugs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 extract_drugs-1.3.0/Cargo.toml
+-rw-r--r--   0      501       20      287 2023-05-30 02:55:34.000000 extract_drugs-1.3.0/.gitignore
+-rw-r--r--   0      501       20     4106 2022-06-27 14:19:06.000000 extract_drugs-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0      501       20    18801 2024-04-24 14:53:47.000000 extract_drugs-1.3.0/Cargo.lock
+-rw-r--r--   0      501       20     1053 2023-05-30 03:02:23.000000 extract_drugs-1.3.0/LICENSE.md
+-rw-r--r--   0      501       20     5472 2024-04-24 14:51:35.000000 extract_drugs-1.3.0/README.md
+-rw-r--r--   0      501       20    17790 2024-04-24 14:59:39.000000 extract_drugs-1.3.0/src/lib.rs
+-rw-r--r--   0      501       20     4329 2023-05-30 02:55:34.000000 extract_drugs-1.3.0/src/main.rs
+-rw-r--r--   0      501       20     1082 2024-04-24 15:03:13.000000 extract_drugs-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6499 1970-01-01 00:00:00.000000 extract_drugs-1.3.0/PKG-INFO
```

### Comparing `extract_drugs-1.2.0/Cargo.toml` & `extract_drugs-1.3.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "drug-extraction-cli"
-version = "1.2.0"
+version = "1.3.0"
 edition = "2021"
 authors = ["Nick Anthony <nicholas.anthony@uky.edu>"]
 description = "A CLI for extracting drugs from text records"
 license = "MIT"
 repository = "https://github.com/UK-IPOP/drug-extraction"
 keywords = ["drug", "extraction", "nlp", "text"]
 categories = ["parsing", "command-line-interface"]
```

### Comparing `extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/METADATA` & `extract_drugs-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: extract-drugs
-Version: 1.1.1
+Version: 1.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Text Processing
 License-File: LICENSE.md
@@ -45,20 +45,23 @@
 
 ![demo-gif](../images/demo.gif)
 
 ## Description
 
 This application takes a CSV file and parses text records from another CSV file to detect and extract search term mentions using string similarity algorithms to account for common misspellings. It is named for the drug searching it does most commonly for us at IPOP but is flexible enough to accept any type search terms.
 
+> NOTE: In our text-preprocessing, we specifically *allow* hyphens ("-") to to their frequency in drug terminologies. If you want to see this functionality removed or put behind a feature flag, please file an Issue.
+
 If you are wondering about specific use cases, check out the [Examples](../examples/) folder!
 
 ## Requires
 
 - [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) package manager (rust toolchain)
 - [just](https://github.com/casey/just) (optional dev-dependency if you clone this repo)
+- Valid UTF-8 encoded CSV data
 
 ## Installation
 
 To install the drug-extraction-cli application, simply:
 
 ### Python Developers / Data Scientists
```

### Comparing `extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/extract_drugs-1.1.1.dist-info/license_files/LICENSE.md` & `extract_drugs-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.2.0/.venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `extract_drugs-1.3.0/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,495 +1,510 @@
-from __future__ import absolute_import
-
-import hmac
-import os
-import sys
-import warnings
-from binascii import hexlify, unhexlify
-from hashlib import md5, sha1, sha256
-
-from ..exceptions import (
-    InsecurePlatformWarning,
-    ProxySchemeUnsupported,
-    SNIMissingWarning,
-    SSLError,
-)
-from ..packages import six
-from .url import BRACELESS_IPV6_ADDRZ_RE, IPV4_RE
-
-SSLContext = None
-SSLTransport = None
-HAS_SNI = False
-IS_PYOPENSSL = False
-IS_SECURETRANSPORT = False
-ALPN_PROTOCOLS = ["http/1.1"]
-
-# Maps the length of a digest to a possible hash function producing this digest
-HASHFUNC_MAP = {32: md5, 40: sha1, 64: sha256}
-
-
-def _const_compare_digest_backport(a, b):
-    """
-    Compare two digests of equal length in constant time.
-
-    The digests must be of type str/bytes.
-    Returns True if the digests match, and False otherwise.
-    """
-    result = abs(len(a) - len(b))
-    for left, right in zip(bytearray(a), bytearray(b)):
-        result |= left ^ right
-    return result == 0
-
-
-_const_compare_digest = getattr(hmac, "compare_digest", _const_compare_digest_backport)
-
-try:  # Test for SSL features
-    import ssl
-    from ssl import CERT_REQUIRED, wrap_socket
-except ImportError:
-    pass
-
-try:
-    from ssl import HAS_SNI  # Has SNI?
-except ImportError:
-    pass
-
-try:
-    from .ssltransport import SSLTransport
-except ImportError:
-    pass
-
-
-try:  # Platform-specific: Python 3.6
-    from ssl import PROTOCOL_TLS
-
-    PROTOCOL_SSLv23 = PROTOCOL_TLS
-except ImportError:
-    try:
-        from ssl import PROTOCOL_SSLv23 as PROTOCOL_TLS
-
-        PROTOCOL_SSLv23 = PROTOCOL_TLS
-    except ImportError:
-        PROTOCOL_SSLv23 = PROTOCOL_TLS = 2
-
-try:
-    from ssl import PROTOCOL_TLS_CLIENT
-except ImportError:
-    PROTOCOL_TLS_CLIENT = PROTOCOL_TLS
-
-
-try:
-    from ssl import OP_NO_COMPRESSION, OP_NO_SSLv2, OP_NO_SSLv3
-except ImportError:
-    OP_NO_SSLv2, OP_NO_SSLv3 = 0x1000000, 0x2000000
-    OP_NO_COMPRESSION = 0x20000
-
-
-try:  # OP_NO_TICKET was added in Python 3.6
-    from ssl import OP_NO_TICKET
-except ImportError:
-    OP_NO_TICKET = 0x4000
-
-
-# A secure default.
-# Sources for more information on TLS ciphers:
-#
-# - https://wiki.mozilla.org/Security/Server_Side_TLS
-# - https://www.ssllabs.com/projects/best-practices/index.html
-# - https://hynek.me/articles/hardening-your-web-servers-ssl-ciphers/
-#
-# The general intent is:
-# - prefer cipher suites that offer perfect forward secrecy (DHE/ECDHE),
-# - prefer ECDHE over DHE for better performance,
-# - prefer any AES-GCM and ChaCha20 over any AES-CBC for better performance and
-#   security,
-# - prefer AES-GCM over ChaCha20 because hardware-accelerated AES is common,
-# - disable NULL authentication, MD5 MACs, DSS, and other
-#   insecure ciphers for security reasons.
-# - NOTE: TLS 1.3 cipher suites are managed through a different interface
-#   not exposed by CPython (yet!) and are enabled by default if they're available.
-DEFAULT_CIPHERS = ":".join(
-    [
-        "ECDHE+AESGCM",
-        "ECDHE+CHACHA20",
-        "DHE+AESGCM",
-        "DHE+CHACHA20",
-        "ECDH+AESGCM",
-        "DH+AESGCM",
-        "ECDH+AES",
-        "DH+AES",
-        "RSA+AESGCM",
-        "RSA+AES",
-        "!aNULL",
-        "!eNULL",
-        "!MD5",
-        "!DSS",
-    ]
-)
-
-try:
-    from ssl import SSLContext  # Modern SSL?
-except ImportError:
-
-    class SSLContext(object):  # Platform-specific: Python 2
-        def __init__(self, protocol_version):
-            self.protocol = protocol_version
-            # Use default values from a real SSLContext
-            self.check_hostname = False
-            self.verify_mode = ssl.CERT_NONE
-            self.ca_certs = None
-            self.options = 0
-            self.certfile = None
-            self.keyfile = None
-            self.ciphers = None
-
-        def load_cert_chain(self, certfile, keyfile):
-            self.certfile = certfile
-            self.keyfile = keyfile
-
-        def load_verify_locations(self, cafile=None, capath=None, cadata=None):
-            self.ca_certs = cafile
-
-            if capath is not None:
-                raise SSLError("CA directories not supported in older Pythons")
-
-            if cadata is not None:
-                raise SSLError("CA data not supported in older Pythons")
-
-        def set_ciphers(self, cipher_suite):
-            self.ciphers = cipher_suite
-
-        def wrap_socket(self, socket, server_hostname=None, server_side=False):
-            warnings.warn(
-                "A true SSLContext object is not available. This prevents "
-                "urllib3 from configuring SSL appropriately and may cause "
-                "certain SSL connections to fail. You can upgrade to a newer "
-                "version of Python to solve this. For more information, see "
-                "https://urllib3.readthedocs.io/en/1.26.x/advanced-usage.html"
-                "#ssl-warnings",
-                InsecurePlatformWarning,
-            )
-            kwargs = {
-                "keyfile": self.keyfile,
-                "certfile": self.certfile,
-                "ca_certs": self.ca_certs,
-                "cert_reqs": self.verify_mode,
-                "ssl_version": self.protocol,
-                "server_side": server_side,
-            }
-            return wrap_socket(socket, ciphers=self.ciphers, **kwargs)
-
+use color_eyre::{
+    eyre::{eyre, Context, ContextCompat},
+    Result,
+};
+use indicatif::{ProgressBar, ProgressIterator, ProgressStyle};
+
+use std::{collections::HashSet, fs::File, path::Path, time::Duration};
+
+use serde::{Deserialize, Serialize};
+
+use itertools::Itertools;
+
+/// Create a spinner with default style, takes a message
+fn initialize_spinner_style(msg: String) -> ProgressBar {
+    let pb = ProgressBar::new_spinner();
+    pb.enable_steady_tick(Duration::from_millis(100));
+    pb.with_style(
+        ProgressStyle::with_template("{spinner:.blue} {msg}")
+            .unwrap()
+            .tick_strings(&[
+                "▹▹▹▹▹",
+                "▸▹▹▹▹",
+                "▹▸▹▹▹",
+                "▹▹▸▹▹",
+                "▹▹▹▸▹",
+                "▹▹▹▹▸",
+                "▪▪▪▪▪",
+            ]),
+    )
+    .with_message(msg)
+}
 
-def assert_fingerprint(cert, fingerprint):
-    """
-    Checks if given fingerprint matches the supplied certificate.
-
-    :param cert:
-        Certificate as bytes object.
-    :param fingerprint:
-        Fingerprint as string of hexdigits, can be interspersed by colons.
-    """
-
-    fingerprint = fingerprint.replace(":", "").lower()
-    digest_length = len(fingerprint)
-    hashfunc = HASHFUNC_MAP.get(digest_length)
-    if not hashfunc:
-        raise SSLError("Fingerprint of invalid length: {0}".format(fingerprint))
-
-    # We need encode() here for py32; works on py2 and p33.
-    fingerprint_bytes = unhexlify(fingerprint.encode())
-
-    cert_digest = hashfunc(cert).digest()
-
-    if not _const_compare_digest(cert_digest, fingerprint_bytes):
-        raise SSLError(
-            'Fingerprints did not match. Expected "{0}", got "{1}".'.format(
-                fingerprint, hexlify(cert_digest)
-            )
-        )
-
-
-def resolve_cert_reqs(candidate):
-    """
-    Resolves the argument to a numeric constant, which can be passed to
-    the wrap_socket function/method from the ssl module.
-    Defaults to :data:`ssl.CERT_REQUIRED`.
-    If given a string it is assumed to be the name of the constant in the
-    :mod:`ssl` module or its abbreviation.
-    (So you can specify `REQUIRED` instead of `CERT_REQUIRED`.
-    If it's neither `None` nor a string we assume it is already the numeric
-    constant which can directly be passed to wrap_socket.
-    """
-    if candidate is None:
-        return CERT_REQUIRED
-
-    if isinstance(candidate, str):
-        res = getattr(ssl, candidate, None)
-        if res is None:
-            res = getattr(ssl, "CERT_" + candidate)
-        return res
-
-    return candidate
-
-
-def resolve_ssl_version(candidate):
-    """
-    like resolve_cert_reqs
-    """
-    if candidate is None:
-        return PROTOCOL_TLS
-
-    if isinstance(candidate, str):
-        res = getattr(ssl, candidate, None)
-        if res is None:
-            res = getattr(ssl, "PROTOCOL_" + candidate)
-        return res
-
-    return candidate
-
-
-def create_urllib3_context(
-    ssl_version=None, cert_reqs=None, options=None, ciphers=None
-):
-    """All arguments have the same meaning as ``ssl_wrap_socket``.
-
-    By default, this function does a lot of the same work that
-    ``ssl.create_default_context`` does on Python 3.4+. It:
-
-    - Disables SSLv2, SSLv3, and compression
-    - Sets a restricted set of server ciphers
-
-    If you wish to enable SSLv3, you can do::
-
-        from pip._vendor.urllib3.util import ssl_
-        context = ssl_.create_urllib3_context()
-        context.options &= ~ssl_.OP_NO_SSLv3
-
-    You can do the same to enable compression (substituting ``COMPRESSION``
-    for ``SSLv3`` in the last line above).
-
-    :param ssl_version:
-        The desired protocol version to use. This will default to
-        PROTOCOL_SSLv23 which will negotiate the highest protocol that both
-        the server and your installation of OpenSSL support.
-    :param cert_reqs:
-        Whether to require the certificate verification. This defaults to
-        ``ssl.CERT_REQUIRED``.
-    :param options:
-        Specific OpenSSL options. These default to ``ssl.OP_NO_SSLv2``,
-        ``ssl.OP_NO_SSLv3``, ``ssl.OP_NO_COMPRESSION``, and ``ssl.OP_NO_TICKET``.
-    :param ciphers:
-        Which cipher suites to allow the server to select.
-    :returns:
-        Constructed SSLContext object with specified options
-    :rtype: SSLContext
-    """
-    # PROTOCOL_TLS is deprecated in Python 3.10
-    if not ssl_version or ssl_version == PROTOCOL_TLS:
-        ssl_version = PROTOCOL_TLS_CLIENT
-
-    context = SSLContext(ssl_version)
-
-    context.set_ciphers(ciphers or DEFAULT_CIPHERS)
-
-    # Setting the default here, as we may have no ssl module on import
-    cert_reqs = ssl.CERT_REQUIRED if cert_reqs is None else cert_reqs
-
-    if options is None:
-        options = 0
-        # SSLv2 is easily broken and is considered harmful and dangerous
-        options |= OP_NO_SSLv2
-        # SSLv3 has several problems and is now dangerous
-        options |= OP_NO_SSLv3
-        # Disable compression to prevent CRIME attacks for OpenSSL 1.0+
-        # (issue #309)
-        options |= OP_NO_COMPRESSION
-        # TLSv1.2 only. Unless set explicitly, do not request tickets.
-        # This may save some bandwidth on wire, and although the ticket is encrypted,
-        # there is a risk associated with it being on wire,
-        # if the server is not rotating its ticketing keys properly.
-        options |= OP_NO_TICKET
-
-    context.options |= options
-
-    # Enable post-handshake authentication for TLS 1.3, see GH #1634. PHA is
-    # necessary for conditional client cert authentication with TLS 1.3.
-    # The attribute is None for OpenSSL <= 1.1.0 or does not exist in older
-    # versions of Python.  We only enable on Python 3.7.4+ or if certificate
-    # verification is enabled to work around Python issue #37428
-    # See: https://bugs.python.org/issue37428
-    if (cert_reqs == ssl.CERT_REQUIRED or sys.version_info >= (3, 7, 4)) and getattr(
-        context, "post_handshake_auth", None
-    ) is not None:
-        context.post_handshake_auth = True
-
-    def disable_check_hostname():
-        if (
-            getattr(context, "check_hostname", None) is not None
-        ):  # Platform-specific: Python 3.2
-            # We do our own verification, including fingerprints and alternative
-            # hostnames. So disable it here
-            context.check_hostname = False
-
-    # The order of the below lines setting verify_mode and check_hostname
-    # matter due to safe-guards SSLContext has to prevent an SSLContext with
-    # check_hostname=True, verify_mode=NONE/OPTIONAL. This is made even more
-    # complex because we don't know whether PROTOCOL_TLS_CLIENT will be used
-    # or not so we don't know the initial state of the freshly created SSLContext.
-    if cert_reqs == ssl.CERT_REQUIRED:
-        context.verify_mode = cert_reqs
-        disable_check_hostname()
-    else:
-        disable_check_hostname()
-        context.verify_mode = cert_reqs
-
-    # Enable logging of TLS session keys via defacto standard environment variable
-    # 'SSLKEYLOGFILE', if the feature is available (Python 3.8+). Skip empty values.
-    if hasattr(context, "keylog_filename"):
-        sslkeylogfile = os.environ.get("SSLKEYLOGFILE")
-        if sslkeylogfile:
-            context.keylog_filename = sslkeylogfile
-
-    return context
-
-
-def ssl_wrap_socket(
-    sock,
-    keyfile=None,
-    certfile=None,
-    cert_reqs=None,
-    ca_certs=None,
-    server_hostname=None,
-    ssl_version=None,
-    ciphers=None,
-    ssl_context=None,
-    ca_cert_dir=None,
-    key_password=None,
-    ca_cert_data=None,
-    tls_in_tls=False,
-):
-    """
-    All arguments except for server_hostname, ssl_context, and ca_cert_dir have
-    the same meaning as they do when using :func:`ssl.wrap_socket`.
-
-    :param server_hostname:
-        When SNI is supported, the expected hostname of the certificate
-    :param ssl_context:
-        A pre-made :class:`SSLContext` object. If none is provided, one will
-        be created using :func:`create_urllib3_context`.
-    :param ciphers:
-        A string of ciphers we wish the client to support.
-    :param ca_cert_dir:
-        A directory containing CA certificates in multiple separate files, as
-        supported by OpenSSL's -CApath flag or the capath argument to
-        SSLContext.load_verify_locations().
-    :param key_password:
-        Optional password if the keyfile is encrypted.
-    :param ca_cert_data:
-        Optional string containing CA certificates in PEM format suitable for
-        passing as the cadata parameter to SSLContext.load_verify_locations()
-    :param tls_in_tls:
-        Use SSLTransport to wrap the existing socket.
-    """
-    context = ssl_context
-    if context is None:
-        # Note: This branch of code and all the variables in it are no longer
-        # used by urllib3 itself. We should consider deprecating and removing
-        # this code.
-        context = create_urllib3_context(ssl_version, cert_reqs, ciphers=ciphers)
-
-    if ca_certs or ca_cert_dir or ca_cert_data:
-        try:
-            context.load_verify_locations(ca_certs, ca_cert_dir, ca_cert_data)
-        except (IOError, OSError) as e:
-            raise SSLError(e)
-
-    elif ssl_context is None and hasattr(context, "load_default_certs"):
-        # try to load OS default certs; works well on Windows (require Python3.4+)
-        context.load_default_certs()
-
-    # Attempt to detect if we get the goofy behavior of the
-    # keyfile being encrypted and OpenSSL asking for the
-    # passphrase via the terminal and instead error out.
-    if keyfile and key_password is None and _is_key_file_encrypted(keyfile):
-        raise SSLError("Client private key is encrypted, password is required")
-
-    if certfile:
-        if key_password is None:
-            context.load_cert_chain(certfile, keyfile)
-        else:
-            context.load_cert_chain(certfile, keyfile, key_password)
-
-    try:
-        if hasattr(context, "set_alpn_protocols"):
-            context.set_alpn_protocols(ALPN_PROTOCOLS)
-    except NotImplementedError:  # Defensive: in CI, we always have set_alpn_protocols
-        pass
-
-    # If we detect server_hostname is an IP address then the SNI
-    # extension should not be used according to RFC3546 Section 3.1
-    use_sni_hostname = server_hostname and not is_ipaddress(server_hostname)
-    # SecureTransport uses server_hostname in certificate verification.
-    send_sni = (use_sni_hostname and HAS_SNI) or (
-        IS_SECURETRANSPORT and server_hostname
+/// Initialize a progress bar with default style, takes a message and length
+fn initialize_progress_bar(msg: String, len: u64) -> ProgressBar {
+    let pb = ProgressBar::new(len);
+    pb.enable_steady_tick(Duration::from_millis(100));
+    pb.with_style(
+        ProgressStyle::default_bar()
+            .template("{spinner:.blue} {msg} [{elapsed_precise}] [{bar:40.cyan/blue}] {pos:>7}/{len:7} ({eta})").unwrap()
+            .progress_chars("##-"),
     )
-    # Do not warn the user if server_hostname is an invalid SNI hostname.
-    if not HAS_SNI and use_sni_hostname:
-        warnings.warn(
-            "An HTTPS request has been made, but the SNI (Server Name "
-            "Indication) extension to TLS is not available on this platform. "
-            "This may cause the server to present an incorrect TLS "
-            "certificate, which can cause validation failures. You can upgrade to "
-            "a newer version of Python to solve this. For more information, see "
-            "https://urllib3.readthedocs.io/en/1.26.x/advanced-usage.html"
-            "#ssl-warnings",
-            SNIMissingWarning,
-        )
-
-    if send_sni:
-        ssl_sock = _ssl_wrap_socket_impl(
-            sock, context, tls_in_tls, server_hostname=server_hostname
-        )
-    else:
-        ssl_sock = _ssl_wrap_socket_impl(sock, context, tls_in_tls)
-    return ssl_sock
-
-
-def is_ipaddress(hostname):
-    """Detects whether the hostname given is an IPv4 or IPv6 address.
-    Also detects IPv6 addresses with Zone IDs.
-
-    :param str hostname: Hostname to examine.
-    :return: True if the hostname is an IP address, False otherwise.
-    """
-    if not six.PY2 and isinstance(hostname, bytes):
-        # IDN A-label bytes are ASCII compatible.
-        hostname = hostname.decode("ascii")
-    return bool(IPV4_RE.match(hostname) or BRACELESS_IPV6_ADDRZ_RE.match(hostname))
-
-
-def _is_key_file_encrypted(key_file):
-    """Detects if a key file is encrypted or not."""
-    with open(key_file, "r") as f:
-        for line in f:
-            # Look for Proc-Type: 4,ENCRYPTED
-            if "ENCRYPTED" in line:
-                return True
-
-    return False
-
-
-def _ssl_wrap_socket_impl(sock, ssl_context, tls_in_tls, server_hostname=None):
-    if tls_in_tls:
-        if not SSLTransport:
-            # Import error, ssl is not available.
-            raise ProxySchemeUnsupported(
-                "TLS in TLS requires support for the 'ssl' module"
-            )
-
-        SSLTransport._validate_ssl_context_for_tls_in_tls(ssl_context)
-        return SSLTransport(sock, ssl_context, server_hostname)
-
-    if server_hostname:
-        return ssl_context.wrap_socket(sock, server_hostname=server_hostname)
-    else:
-        return ssl_context.wrap_socket(sock)
+    .with_message(msg)
+}
+
+/// Struct to hold search term and metadata
+#[derive(Deserialize, Debug, Clone, Default, PartialEq)]
+pub struct SearchTerm {
+    /// The search term
+    pub term: String,
+    /// Optional metadata to be included in output
+    pub metadata: Option<String>,
+}
+
+/// Struct to hold search output
+#[derive(Serialize, Debug, Clone, PartialEq)]
+pub struct SearchOutput<'a> {
+    /// The row id of the matched record, either from specified column or line number
+    row_id: &'a str,
+    /// The search term that was matched
+    search_term: &'a str,
+    /// The matched term from the record
+    matched_term: &'a str,
+    /// The number of edits required to match the search term
+    edits: usize,
+    /// The similarity score between the search term and the matched term
+    similarity_score: f64,
+    /// The field that was searched
+    search_field: &'a str,
+    /// The metadata associated with the search term
+    metadata: &'a Option<String>,
+}
+
+/// Function to read in search terms from a csv file
+/// Performs cleaning of terms, ignoring metadata column
+pub fn read_terms_from_file<P: AsRef<Path>>(p: P) -> Result<Vec<SearchTerm>> {
+    let mut rdr = csv::Reader::from_path(p).wrap_err("Unable to read search terms file")?;
+    let mut records: Vec<SearchTerm> = Vec::new();
+    for (i, row) in rdr
+        .deserialize()
+        .enumerate()
+        .progress_with(initialize_spinner_style(
+            "Loading Search Terms...".to_string(),
+        ))
+    {
+        let mut record: SearchTerm =
+            row.wrap_err(format!("Could not load search term from line: {}", i))?;
+        record.term = clean_text(&record.term);
+        records.push(record);
+    }
+    records.sort_by_key(|x| x.term.split_ascii_whitespace().count());
+    Ok(records)
+}
+
+/// Function to remove non-alphanumeric characters from a string
+/// keeps hyphens due to their usage in abbreviations/medical terms.
+/// Also uppercase for standardization.
+/// Example:
+/// ```
+/// use drug_extraction_cli::clean_text;
+///
+/// let s = "This is a test-string with 1234 and some punctuation!@#$%^&*()";
+/// let cleaned = clean_text(s);
+/// assert_ne!(cleaned, "THIS IS A TEST STRING WITH 1234 AND SOME PUNCTUATION");
+/// assert_eq!(cleaned, "THIS IS A TEST-STRING WITH 1234 AND SOME PUNCTUATION");
+/// ```
+pub fn clean_text(s: &str) -> String {
+    s.replace(|c: char| !c.is_ascii_alphanumeric() && c != '-', " ")
+        .trim()
+        .to_ascii_uppercase()
+}
+
+/// Struct to hold information about the dataset
+#[derive(Debug)]
+pub struct DataSet {
+    /// csv reader for the dataset
+    pub reader: csv::Reader<File>,
+    /// rows in the dataset from first scan
+    pub rows: usize,
+    /// indices of the columns to search in the dataset
+    pub clean_search_columns: Vec<ColumnInfo>,
+    /// index of the column to use as an id
+    pub clean_id_column: Option<ColumnInfo>,
+    /// csv writer for the output file
+    pub writer: csv::Writer<File>,
+}
+
+#[derive(Debug, Clone, Default, PartialEq)]
+pub struct ColumnInfo {
+    pub name: String,
+    pub index: usize,
+}
+
+/// Function to get the column index for a given column name
+/// Returns an error if the column name is not found
+/// Typically ran using the header from the csv reader and is called
+/// inside the [collect_column_info] function to do this for each target column.
+/// Example:
+/// ```
+/// use drug_extraction_cli::get_column_info;
+///
+/// let header = vec!["ID", "NAME", "DESCRIPTION"];
+/// let column = "NAME";
+/// let column_info = get_column_info(&header, &column);
+/// assert!(column_info.is_ok());
+/// let column_info = column_info.unwrap();
+/// assert_eq!(column_info.name, "NAME");
+/// assert_eq!(column_info.index, 1);
+/// ```
+pub fn get_column_info<S: AsRef<str> + PartialEq>(header: &[S], column: &S) -> Result<ColumnInfo> {
+    let pos = header.iter().position(|h| h == column);
+    match pos {
+        Some(i) => Ok(ColumnInfo {
+            name: column.as_ref().to_string(),
+            index: i,
+        }),
+        None => Err(eyre!("Unable to find column {}", column.as_ref())),
+    }
+}
+
+/// Function to collect column info for each column to search
+/// Typically ran using the header from the csv reader and is called
+/// inside the [initialize_dataset] function to do this for each target column.
+/// Example:
+/// ```
+/// use drug_extraction_cli::collect_column_info;
+///
+/// let header = vec!["ID", "NAME", "DESCRIPTION"];
+/// let columns = vec!["NAME", "DESCRIPTION"];
+/// let column_info = collect_column_info(&header, &columns);
+/// assert!(column_info.is_ok());
+/// let column_info = column_info.unwrap();
+/// assert_eq!(column_info.len(), 2);
+/// assert_eq!(column_info[0].name, "NAME");
+/// assert_eq!(column_info[0].index, 1);
+/// assert_eq!(column_info[1].name, "DESCRIPTION");
+/// assert_eq!(column_info[1].index, 2);
+/// ```
+pub fn collect_column_info<S: AsRef<str> + PartialEq>(
+    header: &[S],
+    column_names: &[S],
+) -> Result<Vec<ColumnInfo>> {
+    column_names
+        .iter()
+        .map(|column| get_column_info(header, column))
+        .collect()
+}
+
+/// Function to initialize the dataset
+pub fn initialize_dataset<P: AsRef<Path>>(
+    data_file: P,
+    search_columns: &[String],
+    id_column: Option<String>,
+) -> Result<DataSet> {
+    let mut rdr = csv::Reader::from_path(&data_file).wrap_err("Unable to initialize csv reader")?;
+    let header = rdr
+        .headers()
+        .wrap_err("Unable to parse csv headers")?
+        .iter()
+        .map(clean_text)
+        .collect_vec();
+    // clean search cols and id col
+    let clean_search_cols = search_columns.iter().map(|c| clean_text(c)).collect_vec();
+    let clean_id_col = id_column.map(|c| clean_text(&c));
+    let column_info = collect_column_info(&header, &clean_search_cols)
+        .wrap_err("Unable to collect column indices")?;
+    let ds = match clean_id_col {
+        Some(c) => DataSet {
+            reader: csv::Reader::from_path(&data_file)
+                .wrap_err("Unable to initialize csv reader")?,
+            rows: rdr.records().count(),
+            clean_search_columns: column_info,
+            clean_id_column: Some(get_column_info(&header, &c)?),
+            writer: csv::Writer::from_path("output.csv")?,
+        },
+        None => DataSet {
+            reader: csv::Reader::from_path(&data_file)
+                .wrap_err("Unable to initialize csv reader")?,
+            rows: rdr.records().count(),
+            clean_search_columns: column_info,
+            clean_id_column: None,
+            writer: csv::Writer::from_path("output.csv")?,
+        },
+    };
+    Ok(ds)
+}
+
+/// Primary search function
+pub fn search(mut dataset: DataSet, search_terms: Vec<SearchTerm>) -> Result<()> {
+    let mut total_records_with_matches = 0;
+    let mut total_records = 0;
+    let mut matched_terms: HashSet<&str> = HashSet::new();
+
+    let spinner =
+        initialize_progress_bar("Searching for matches...".to_string(), dataset.rows as u64);
+    for (i, row) in dataset
+        .reader
+        .records()
+        .enumerate()
+        .progress_with(spinner.clone())
+    {
+        let record = row.wrap_err(format!("Unable to read record from line {}", i))?;
+
+        let id = match &dataset.clean_id_column {
+            Some(c) => record
+                .get(c.index)
+                .wrap_err(format!(
+                    "Unable to read id column {} from line {}",
+                    c.name, i
+                ))?
+                .to_string(),
+            None => i.to_string(),
+        };
+
+        let mut found_match = false;
+        for column in &dataset.clean_search_columns {
+            let text = record.get(column.index).wrap_err(format!(
+                "Unable to read column {} from line {}",
+                column.name, i
+            ))?;
+            let cleaned_text = clean_text(text);
+            let grams = cleaned_text.split_ascii_whitespace().collect_vec();
+            for (term_len, term_list) in &search_terms
+                .iter()
+                .group_by(|st| st.term.split_ascii_whitespace().count())
+            {
+                let combos = if term_len == 1 {
+                    term_list.cartesian_product(
+                        grams
+                            .iter()
+                            .unique()
+                            .map(|word| word.to_string())
+                            .collect_vec(),
+                    )
+                } else {
+                    term_list.cartesian_product(
+                        grams
+                            .windows(term_len)
+                            .unique()
+                            .map(|words| words.join(" "))
+                            .collect_vec(),
+                    )
+                };
+                for (search_term, comparison_term) in combos {
+                    let edits = strsim::osa_distance(&search_term.term, &comparison_term);
+                    match edits {
+                        0 => {
+                            dataset
+                                .writer
+                                .serialize(SearchOutput {
+                                    row_id: &id,
+                                    search_term: &search_term.term,
+                                    matched_term: &comparison_term,
+                                    edits,
+                                    similarity_score: 1.0,
+                                    search_field: &column.name,
+                                    metadata: &search_term.metadata,
+                                })
+                                .wrap_err("Enable to serialize output")?;
+                            found_match = true;
+                            matched_terms.insert(&search_term.term);
+                        }
+                        1 => {
+                            let sim = strsim::jaro_winkler(&search_term.term, &comparison_term);
+                            if sim >= 0.95 {
+                                dataset
+                                    .writer
+                                    .serialize(SearchOutput {
+                                        row_id: &id,
+                                        search_term: &search_term.term,
+                                        matched_term: &comparison_term,
+                                        edits,
+                                        similarity_score: sim,
+                                        search_field: &column.name,
+                                        metadata: &search_term.metadata,
+                                    })
+                                    .wrap_err("Enable to serialize output")?;
+                                found_match = true;
+                                matched_terms.insert(&search_term.term);
+                            }
+                        }
+                        2 => {
+                            let sim = strsim::jaro_winkler(&search_term.term, &comparison_term);
+                            if sim >= 0.97 {
+                                dataset
+                                    .writer
+                                    .serialize(SearchOutput {
+                                        row_id: &id,
+                                        search_term: &search_term.term,
+                                        matched_term: &comparison_term,
+                                        edits,
+                                        similarity_score: sim,
+                                        search_field: &column.name,
+                                        metadata: &search_term.metadata,
+                                    })
+                                    .wrap_err("Enable to serialize output")?;
+                                found_match = true;
+                                matched_terms.insert(&search_term.term);
+                            }
+                        }
+                        _ => continue,
+                    }
+                }
+            }
+        }
+        if found_match {
+            total_records_with_matches += 1;
+        }
+        total_records += 1;
+    }
+    dataset.writer.flush().wrap_err("Unable to flush writer")?;
+    spinner.finish_with_message("Done!");
+
+    println!(
+        "Found matches in {:} of {:} records ({:.2}%)",
+        total_records_with_matches,
+        total_records,
+        (total_records_with_matches as f64 / total_records as f64) * 100.0
+    );
+    println!(
+        "Found {:} of {:} search terms ({:.2}%)",
+        matched_terms.len(),
+        search_terms.len(),
+        (matched_terms.len() as f64 / search_terms.len() as f64) * 100.0
+    );
+
+    Ok(())
+}
+
+pub fn run_searcher<P: AsRef<Path>>(
+    data_file: P,
+    search_terms_file: P,
+    search_columns: Vec<String>,
+    id_column: Option<String>,
+) -> Result<()> {
+    let search_terms = read_terms_from_file(search_terms_file)?;
+    let dataset = initialize_dataset(data_file, &search_columns, id_column)?;
+    search(dataset, search_terms)
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_clean_text_no_changes() {
+        let s = "This is a test string.";
+        assert_eq!(clean_text(s), "this is a test string".to_ascii_uppercase());
+    }
+
+    #[test]
+    fn test_clean_text_numeric() {
+        let s = "This is a test string with 1234 numbers.";
+        assert_eq!(
+            clean_text(s),
+            "this is a test string with 1234 numbers".to_ascii_uppercase()
+        );
+    }
+
+    #[test]
+    fn test_clean_text_symbols() {
+        let s = "!@#$%^&*()_+-";
+        assert_eq!(clean_text(s), "-");
+    }
+
+    #[test]
+    fn test_clean_empty() {
+        let s = "";
+        assert_eq!(clean_text(s), "");
+    }
+
+    #[test]
+    fn test_clean_end_whitespace() {
+        let s = "!! This is a test string.   ";
+        assert_eq!(clean_text(s), "this is a test string".to_ascii_uppercase());
+    }
+
+    #[test]
+    fn test_clean_end_whitespace2() {
+        let s = "!! This is a test to test- - hyphenated string.   ";
+        assert_eq!(
+            clean_text(s),
+            "this is a test to test- - hyphenated string".to_ascii_uppercase()
+        );
+    }
+
+    #[test]
+    fn test_whitespace_split() {
+        let s = "!! This is a test to test- - hyphenated string.   ";
+        assert_eq!(
+            clean_text(s),
+            "this is a test to test- - hyphenated string".to_ascii_uppercase()
+        );
+        let c = clean_text(s);
+        let v = c.split_ascii_whitespace().collect_vec();
+        assert_eq!(
+            v,
+            vec![
+                "THIS",
+                "IS",
+                "A",
+                "TEST",
+                "TO",
+                "TEST-",
+                "-",
+                "HYPHENATED",
+                "STRING"
+            ]
+        );
+    }
+
+    #[test]
+    fn test_get_column_info() {
+        let header = vec!["a", "b", "c"];
+        let col = "a";
+        assert_eq!(get_column_info(&header, &col).unwrap().index, 0);
+    }
+
+    #[test]
+    fn test_get_column_info_errors() {
+        let header = vec!["a", "b", "c"];
+        let col = "d";
+        assert!(get_column_info(&header, &col).is_err());
+    }
+
+    #[test]
+    fn test_collect_column_info() {
+        let header = vec!["a", "b", "c"];
+        let cols = vec!["a", "b"];
+        let info = collect_column_info(&header, &cols);
+        assert!(info.is_ok());
+        let info = info.unwrap();
+        assert_eq!(info.len(), 2);
+        assert_eq!(
+            info,
+            vec![
+                ColumnInfo {
+                    name: "a".to_string(),
+                    index: 0
+                },
+                ColumnInfo {
+                    name: "b".to_string(),
+                    index: 1
+                }
+            ]
+        );
+    }
+
+    #[test]
+    fn test_collect_column_info_sample() -> Result<()> {
+        let header = csv::Reader::from_path("../data/search_terms.csv")?
+            .headers()?
+            .into_iter()
+            .map(clean_text)
+            .collect_vec();
+        let cols = ["term", "metadata"]
+            .iter()
+            .map(|c| clean_text(c))
+            .collect_vec();
+        let info = collect_column_info(&header, &cols)?;
+        assert_eq!(info.len(), 2);
+        Ok(())
+    }
+
+    #[test]
+    fn test_enumerated_reader() {
+        let mut reader = csv::Reader::from_path("../data/search_terms.csv").unwrap();
+        let (i, _) = reader.records().enumerate().next().unwrap();
+        assert!(i == 0);
+    }
+}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `extract_drugs-1.2.0/CONTRIBUTING.md` & `extract_drugs-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.2.0/Cargo.lock` & `extract_drugs-1.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 dependencies = [
  "console",
  "shell-words",
 ]
 
 [[package]]
 name = "drug-extraction-cli"
-version = "1.2.0"
+version = "1.3.0"
 dependencies = [
  "clap",
  "color-eyre",
  "csv",
  "dialoguer",
  "indicatif",
  "itertools",
```

### Comparing `extract_drugs-1.2.0/README.md` & `extract_drugs-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,23 @@
 
 ![demo-gif](../images/demo.gif)
 
 ## Description
 
 This application takes a CSV file and parses text records from another CSV file to detect and extract search term mentions using string similarity algorithms to account for common misspellings. It is named for the drug searching it does most commonly for us at IPOP but is flexible enough to accept any type search terms.
 
+> NOTE: In our text-preprocessing, we specifically *allow* hyphens ("-") to to their frequency in drug terminologies. If you want to see this functionality removed or put behind a feature flag, please file an Issue.
+
 If you are wondering about specific use cases, check out the [Examples](../examples/) folder!
 
 ## Requires
 
 - [cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html) package manager (rust toolchain)
 - [just](https://github.com/casey/just) (optional dev-dependency if you clone this repo)
+- Valid UTF-8 encoded CSV data
 
 ## Installation
 
 To install the drug-extraction-cli application, simply:
 
 ### Python Developers / Data Scientists
```

### Comparing `extract_drugs-1.2.0/src/main.rs` & `extract_drugs-1.3.0/src/main.rs`

 * *Files identical despite different names*

### Comparing `extract_drugs-1.2.0/pyproject.toml` & `extract_drugs-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "extract-drugs"
-version = "1.2.0"
+version = "1.3.0"
+summary = "A CLI for extracting drugs from text records"
 description = "A CLI for extracting drugs from text records"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.7"
 authors = [
     {name = "Nick Anthony", email = "nanthony007@gmail.com"}
 ]
 maintainers = [
```

