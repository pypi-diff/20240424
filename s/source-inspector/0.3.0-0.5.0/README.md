# Comparing `tmp/source-inspector-0.3.0.tar.gz` & `tmp/source_inspector-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "source-inspector-0.3.0.tar", last modified: Tue Mar 19 14:17:35 2024, max compression
+gzip compressed data, was "source_inspector-0.5.0.tar", last modified: Wed Apr 24 21:16:23 2024, max compression
```

## Comparing `source-inspector-0.3.0.tar` & `source_inspector-0.5.0.tar`

### file list

```diff
@@ -1,100 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.165171 source-inspector-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-19 14:17:30.000000 source-inspector-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.149171 source-inspector-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 14:17:30.000000 source-inspector-0.3.0/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-19 14:17:30.000000 source-inspector-0.3.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-19 14:17:30.000000 source-inspector-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-19 14:17:30.000000 source-inspector-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-19 14:17:30.000000 source-inspector-0.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 14:17:30.000000 source-inspector-0.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-19 14:17:30.000000 source-inspector-0.3.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-19 14:17:30.000000 source-inspector-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-19 14:17:30.000000 source-inspector-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-19 14:17:35.165171 source-inspector-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-19 14:17:30.000000 source-inspector-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 14:17:30.000000 source-inspector-0.3.0/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-19 14:17:30.000000 source-inspector-0.3.0/azure-pipelines.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-03-19 14:17:30.000000 source-inspector-0.3.0/configure
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/docs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.153171 source-inspector-0.3.0/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-19 14:17:30.000000 source-inspector-0.3.0/docs/source/skeleton-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.149171 source-inspector-0.3.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.157171 source-inspector-0.3.0/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.161171 source-inspector-0.3.0/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-19 14:17:30.000000 source-inspector-0.3.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-19 14:17:30.000000 source-inspector-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:30.000000 source-inspector-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:30.000000 source-inspector-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-19 14:17:35.169171 source-inspector-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.149171 source-inspector-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.161171 source-inspector-0.3.0/src/source_inspector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:30.000000 source-inspector-0.3.0/src/source_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-19 14:17:30.000000 source-inspector-0.3.0/src/source_inspector/strings_xgettext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-19 14:17:30.000000 source-inspector-0.3.0/src/source_inspector/symbols_ctags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.165171 source-inspector-0.3.0/src/source_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-19 14:17:35.000000 source-inspector-0.3.0/src/source_inspector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.161171 source-inspector-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.149171 source-inspector-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.161171 source-inspector-0.3.0/tests/data/strings_xgettext/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/fdisk.c
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/fdisk.c-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/fdisk.c.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    78526 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/lineedit.c
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/lineedit.c-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/lineedit.c.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/test3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/strings_xgettext/test3.cpp-expected.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:17:35.165171 source-inspector-0.3.0/tests/data/symbols_ctags/
--rw-r--r--   0 runner    (1001) docker     (127)   285697 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/symbols_ctags/if_ath.c
--rw-r--r--   0 runner    (1001) docker     (127)    57093 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/symbols_ctags/if_ath.c-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/symbols_ctags/test3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/data/symbols_ctags/test3.cpp-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/test_symbols_ctags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-19 14:17:30.000000 source-inspector-0.3.0/tests/test_symbols_xgettext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.807390 source_inspector-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 21:16:19.000000 source_inspector-0.5.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.787389 source_inspector-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 21:16:19.000000 source_inspector-0.5.0/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-24 21:16:19.000000 source_inspector-0.5.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 21:16:19.000000 source_inspector-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 21:16:19.000000 source_inspector-0.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 21:16:19.000000 source_inspector-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 21:16:19.000000 source_inspector-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-24 21:16:19.000000 source_inspector-0.5.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-24 21:16:19.000000 source_inspector-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 21:16:19.000000 source_inspector-0.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-24 21:16:23.807390 source_inspector-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 21:16:19.000000 source_inspector-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 21:16:19.000000 source_inspector-0.5.0/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 21:16:19.000000 source_inspector-0.5.0/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-04-24 21:16:19.000000 source_inspector-0.5.0/configure
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/docs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      131 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-24 21:16:19.000000 source_inspector-0.5.0/docs/source/skeleton-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.791390 source_inspector-0.5.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.795390 source_inspector-0.5.0/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.799390 source_inspector-0.5.0/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 21:16:19.000000 source_inspector-0.5.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 21:16:19.000000 source_inspector-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:19.000000 source_inspector-0.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:19.000000 source_inspector-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 21:16:23.807390 source_inspector-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.791390 source_inspector-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.799390 source_inspector-0.5.0/src/source_inspector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:19.000000 source_inspector-0.5.0/src/source_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-24 21:16:19.000000 source_inspector-0.5.0/src/source_inspector/strings_xgettext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-24 21:16:19.000000 source_inspector-0.5.0/src/source_inspector/symbols_ctags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-24 21:16:19.000000 source_inspector-0.5.0/src/source_inspector/symbols_pygments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-24 21:16:19.000000 source_inspector-0.5.0/src/source_inspector/symbols_tree_sitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.807390 source_inspector-0.5.0/src/source_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 21:16:23.000000 source_inspector-0.5.0/src/source_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.799390 source_inspector-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.791390 source_inspector-0.5.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.803390 source_inspector-0.5.0/tests/data/strings_xgettext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/fdisk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/fdisk.c-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/fdisk.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    78526 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/lineedit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/lineedit.c-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/lineedit.c.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/test3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/strings_xgettext/test3.cpp-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.803390 source_inspector-0.5.0/tests/data/symbols_ctags/
+-rw-r--r--   0 runner    (1001) docker     (127)   285697 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_ctags/if_ath.c
+-rw-r--r--   0 runner    (1001) docker     (127)    57093 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_ctags/if_ath.c-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_ctags/test3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_ctags/test3.cpp-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.803390 source_inspector-0.5.0/tests/data/symbols_pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)   285697 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/if_ath.c
+-rw-r--r--   0 runner    (1001) docker     (127)   523878 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/if_ath.c-expected-tokens.json
+-rw-r--r--   0 runner    (1001) docker     (127)    59737 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/if_ath.c-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/test3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30268 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/test3.cpp-expected-tokens.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_pygments/test3.cpp-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:16:23.807390 source_inspector-0.5.0/tests/data/symbols_tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)   285697 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_tree_sitter/if_ath.c
+-rw-r--r--   0 runner    (1001) docker     (127)   217773 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_tree_sitter/if_ath.c-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_tree_sitter/test3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/data/symbols_tree_sitter/test3.cpp-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/test_symbols_ctags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/test_symbols_pygments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/test_symbols_tree_shitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-24 21:16:19.000000 source_inspector-0.5.0/tests/test_symbols_xgettext.py
```

### Comparing `source-inspector-0.3.0/.github/workflows/docs-ci.yml` & `source_inspector-0.5.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/.github/workflows/pypi-release.yml` & `source_inspector-0.5.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/.gitignore` & `source_inspector-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/.readthedocs.yml` & `source_inspector-0.5.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/CHANGELOG.rst` & `source_inspector-0.5.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+v0.5.0
+------
+
+- Add support to collect strings, comments and symbols from source using Pygments 
+- Add support to collect strings and symbols from source using tree-sitter
+
 
 v0.3.0
 ------
 
 Improve xgettext handlings.
  - Handle empty, whitespace and special characters. https://github.com/nexB/source-inspector/issues/11
  - Properly handle the multiple starting lines for a string. https://github.com/nexB/source-inspector/issues/13
```

### Comparing `source-inspector-0.3.0/CODE_OF_CONDUCT.rst` & `source_inspector-0.5.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/Makefile` & `source_inspector-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/NOTICE` & `source_inspector-0.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/PKG-INFO` & `source_inspector-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: source-inspector
-Version: 0.3.0
+Version: 0.5.0
 Summary: source-inspector
 Home-page: https://github.com/nexB/source-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,24 @@
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
 License-File: CODE_OF_CONDUCT.rst
 Requires-Dist: scancode-toolkit
 Requires-Dist: plugincode
 Requires-Dist: commoncode
 Requires-Dist: typecode
+Requires-Dist: tree-sitter
+Requires-Dist: tree-sitter-bash
+Requires-Dist: tree-sitter-c
+Requires-Dist: tree-sitter-cpp
+Requires-Dist: tree-sitter-go
+Requires-Dist: tree-sitter-java
+Requires-Dist: tree-sitter-javascript
+Requires-Dist: tree-sitter-python
+Requires-Dist: tree-sitter-rust
+Requires-Dist: pygments
 Provides-Extra: testing
 Requires-Dist: pytest!=7.0.0,>=6; extra == "testing"
 Requires-Dist: pytest-xdist>=2; extra == "testing"
 Requires-Dist: aboutcode-toolkit>=7.0.2; extra == "testing"
 Requires-Dist: pycodestyle>=2.8.0; extra == "testing"
 Requires-Dist: twine; extra == "testing"
 Requires-Dist: black; extra == "testing"
```

### Comparing `source-inspector-0.3.0/README.rst` & `source_inspector-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/apache-2.0.LICENSE` & `source_inspector-0.5.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/azure-pipelines.yml` & `source_inspector-0.5.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/configure` & `source_inspector-0.5.0/configure`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/Makefile` & `source_inspector-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/make.bat` & `source_inspector-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/source/_static/theme_overrides.css` & `source_inspector-0.5.0/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/source/conf.py` & `source_inspector-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/source/contribute/contrib_doc.rst` & `source_inspector-0.5.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/docs/source/skeleton-usage.rst` & `source_inspector-0.5.0/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/azure-container-deb.yml` & `source_inspector-0.5.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/azure-container-rpm.yml` & `source_inspector-0.5.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/azure-posix.yml` & `source_inspector-0.5.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/azure-win.yml` & `source_inspector-0.5.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/macports-ci` & `source_inspector-0.5.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/macports-ci.ABOUT` & `source_inspector-0.5.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/ci/mit.LICENSE` & `source_inspector-0.5.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/README.rst` & `source_inspector-0.5.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/check_thirdparty.py` & `source_inspector-0.5.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/fetch_thirdparty.py` & `source_inspector-0.5.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/gen_pypi_simple.py` & `source_inspector-0.5.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `source_inspector-0.5.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/gen_requirements.py` & `source_inspector-0.5.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/gen_requirements_dev.py` & `source_inspector-0.5.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `source_inspector-0.5.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/test_utils_pypi_supported_tags.py` & `source_inspector-0.5.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `source_inspector-0.5.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_dejacode.py` & `source_inspector-0.5.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_pip_compatibility_tags.py` & `source_inspector-0.5.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_pypi_supported_tags.py` & `source_inspector-0.5.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `source_inspector-0.5.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_requirements.py` & `source_inspector-0.5.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_thirdparty.py` & `source_inspector-0.5.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/etc/scripts/utils_thirdparty.py.ABOUT` & `source_inspector-0.5.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/pyproject.toml` & `source_inspector-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/setup.cfg` & `source_inspector-0.5.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -32,22 +32,34 @@
 setup_requires = setuptools_scm[toml] >= 4
 python_requires = >=3.7
 install_requires = 
 	scancode-toolkit
 	plugincode
 	commoncode
 	typecode
+	tree-sitter
+	tree-sitter-bash
+	tree-sitter-c
+	tree-sitter-cpp
+	tree-sitter-go
+	tree-sitter-java
+	tree-sitter-javascript
+	tree-sitter-python
+	tree-sitter-rust
+	pygments
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 scancode_scan = 
 	source_symbol = source_inspector.symbols_ctags:CtagsSymbolScannerPlugin
 	source_string = source_inspector.strings_xgettext:XgettextStringScannerPlugin
+	treesitter_symbol_and_string = source_inspector.symbols_tree_sitter:TreeSitterSymbolAndStringScannerPlugin
+	pygments_symbol_and_string = source_inspector.symbols_pygments:PygmentsSymbolsAndStringScannerPlugin
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 7.0.0
 	pytest-xdist >= 2
 	aboutcode-toolkit >= 7.0.2
 	pycodestyle >= 2.8.0
```

### Comparing `source-inspector-0.3.0/src/source_inspector/strings_xgettext.py` & `source_inspector-0.5.0/src/source_inspector/strings_xgettext.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         PluggableCommandLineOption(
             ("--source-string",),
             is_flag=True,
             default=False,
             help="Collect source strings using xgettext.",
             help_group=SCAN_GROUP,
             sort_order=100,
+            conflicting_options=["treesitter_symbol_and_string", "pygments_symbol_and_string"],
         ),
     ]
 
     def is_enabled(self, source_string, **kwargs):
         return source_string
 
     def get_scanner(self, **kwargs):
@@ -83,15 +84,15 @@
             "--output=-",
             location,
         ],
         to_files=False,
     )
 
     if rc != 0:
-        raise Exception(open(err).read())
+        raise Exception(err)
 
     yield from parse_po_text(po_text=result, drop_header=True, clean=clean)
 
 
 def parse_po_text(po_text, drop_header=False, clean=True):
     """
     Yield mappings of strings collected from the ``po_text`` string.
```

### Comparing `source-inspector-0.3.0/src/source_inspector/symbols_ctags.py` & `source_inspector-0.5.0/src/source_inspector/symbols_ctags.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         PluggableCommandLineOption(
             ("--source-symbol",),
             is_flag=True,
             default=False,
             help="Collect source symbols using Universal ctags.",
             help_group=SCAN_GROUP,
             sort_order=100,
+            conflicting_options=["treesitter_symbol_and_string", "pygments_symbol_and_string"],
         ),
     ]
 
     def is_enabled(self, source_symbol, **kwargs):
         return source_symbol
 
     def get_scanner(self, **kwargs):
@@ -74,15 +75,15 @@
     rc, result, err = command.execute(
         cmd_loc="ctags",
         args=["--output-format=json", "-f", "-", location],
         to_files=False,
     )
 
     if rc != 0:
-        raise Exception(open(err).read())
+        raise Exception(err)
 
     # set of ctags field names we support
     supported_fields = {
         "name",
         "pattern",
         "file",
         "kind",
```

### Comparing `source-inspector-0.3.0/src/source_inspector.egg-info/PKG-INFO` & `source_inspector-0.5.0/src/source_inspector.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: source-inspector
-Version: 0.3.0
+Version: 0.5.0
 Summary: source-inspector
 Home-page: https://github.com/nexB/source-inspector
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,24 @@
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
 License-File: CODE_OF_CONDUCT.rst
 Requires-Dist: scancode-toolkit
 Requires-Dist: plugincode
 Requires-Dist: commoncode
 Requires-Dist: typecode
+Requires-Dist: tree-sitter
+Requires-Dist: tree-sitter-bash
+Requires-Dist: tree-sitter-c
+Requires-Dist: tree-sitter-cpp
+Requires-Dist: tree-sitter-go
+Requires-Dist: tree-sitter-java
+Requires-Dist: tree-sitter-javascript
+Requires-Dist: tree-sitter-python
+Requires-Dist: tree-sitter-rust
+Requires-Dist: pygments
 Provides-Extra: testing
 Requires-Dist: pytest!=7.0.0,>=6; extra == "testing"
 Requires-Dist: pytest-xdist>=2; extra == "testing"
 Requires-Dist: aboutcode-toolkit>=7.0.2; extra == "testing"
 Requires-Dist: pycodestyle>=2.8.0; extra == "testing"
 Requires-Dist: twine; extra == "testing"
 Requires-Dist: black; extra == "testing"
```

### Comparing `source-inspector-0.3.0/src/source_inspector.egg-info/SOURCES.txt` & `source_inspector-0.5.0/src/source_inspector.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -53,29 +53,43 @@
 etc/scripts/utils_pypi_supported_tags.py.ABOUT
 etc/scripts/utils_requirements.py
 etc/scripts/utils_thirdparty.py
 etc/scripts/utils_thirdparty.py.ABOUT
 src/source_inspector/__init__.py
 src/source_inspector/strings_xgettext.py
 src/source_inspector/symbols_ctags.py
+src/source_inspector/symbols_pygments.py
+src/source_inspector/symbols_tree_sitter.py
 src/source_inspector.egg-info/PKG-INFO
 src/source_inspector.egg-info/SOURCES.txt
 src/source_inspector.egg-info/dependency_links.txt
 src/source_inspector.egg-info/entry_points.txt
 src/source_inspector.egg-info/not-zip-safe
 src/source_inspector.egg-info/requires.txt
 src/source_inspector.egg-info/top_level.txt
 tests/test_skeleton_codestyle.py
 tests/test_symbols_ctags.py
+tests/test_symbols_pygments.py
+tests/test_symbols_tree_shitter.py
 tests/test_symbols_xgettext.py
 tests/data/strings_xgettext/fdisk.c
 tests/data/strings_xgettext/fdisk.c-expected.json
 tests/data/strings_xgettext/fdisk.c.ABOUT
 tests/data/strings_xgettext/lineedit.c
 tests/data/strings_xgettext/lineedit.c-expected.json
 tests/data/strings_xgettext/lineedit.c.ABOUT
 tests/data/strings_xgettext/test3.cpp
 tests/data/strings_xgettext/test3.cpp-expected.json
 tests/data/symbols_ctags/if_ath.c
 tests/data/symbols_ctags/if_ath.c-expected.json
 tests/data/symbols_ctags/test3.cpp
-tests/data/symbols_ctags/test3.cpp-expected.json
+tests/data/symbols_ctags/test3.cpp-expected.json
+tests/data/symbols_pygments/if_ath.c
+tests/data/symbols_pygments/if_ath.c-expected-tokens.json
+tests/data/symbols_pygments/if_ath.c-expected.json
+tests/data/symbols_pygments/test3.cpp
+tests/data/symbols_pygments/test3.cpp-expected-tokens.json
+tests/data/symbols_pygments/test3.cpp-expected.json
+tests/data/symbols_tree_sitter/if_ath.c
+tests/data/symbols_tree_sitter/if_ath.c-expected.json
+tests/data/symbols_tree_sitter/test3.cpp
+tests/data/symbols_tree_sitter/test3.cpp-expected.json
```

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/fdisk.c` & `source_inspector-0.5.0/tests/data/strings_xgettext/fdisk.c`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/fdisk.c-expected.json` & `source_inspector-0.5.0/tests/data/strings_xgettext/fdisk.c-expected.json`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/lineedit.c` & `source_inspector-0.5.0/tests/data/strings_xgettext/lineedit.c`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/lineedit.c-expected.json` & `source_inspector-0.5.0/tests/data/strings_xgettext/lineedit.c-expected.json`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/test3.cpp` & `source_inspector-0.5.0/tests/data/strings_xgettext/test3.cpp`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/strings_xgettext/test3.cpp-expected.json` & `source_inspector-0.5.0/tests/data/strings_xgettext/test3.cpp-expected.json`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/symbols_ctags/if_ath.c` & `source_inspector-0.5.0/tests/data/symbols_ctags/if_ath.c`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/symbols_ctags/if_ath.c-expected.json` & `source_inspector-0.5.0/tests/data/symbols_ctags/if_ath.c-expected.json`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/symbols_ctags/test3.cpp` & `source_inspector-0.5.0/tests/data/symbols_ctags/test3.cpp`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/data/symbols_ctags/test3.cpp-expected.json` & `source_inspector-0.5.0/tests/data/symbols_ctags/test3.cpp-expected.json`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/test_skeleton_codestyle.py` & `source_inspector-0.5.0/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/test_symbols_ctags.py` & `source_inspector-0.5.0/tests/test_symbols_ctags.py`

 * *Files identical despite different names*

### Comparing `source-inspector-0.3.0/tests/test_symbols_xgettext.py` & `source_inspector-0.5.0/tests/test_symbols_xgettext.py`

 * *Files identical despite different names*

