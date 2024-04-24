# Comparing `tmp/django-authorization-1.2.1.tar.gz` & `tmp/django_authorization-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-authorization-1.2.1.tar", last modified: Sat Oct 28 15:44:56 2023, max compression
+gzip compressed data, was "django_authorization-1.3.0.tar", last modified: Wed Apr 24 13:03:05 2024, max compression
```

## Comparing `django-authorization-1.2.1.tar` & `django_authorization-1.3.0.tar`

### file list

```diff
@@ -1,113 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-28 15:44:17.000000 django-authorization-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2023-10-28 15:44:56.348870 django-authorization-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2023-10-28 15:44:17.000000 django-authorization-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/dauthz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/dauthz/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/dauthz/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/backends/casbin_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/dauthz/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/decorators/_enforcer_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/decorators/_request_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/dauthz/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/dauthz/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/commands/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/commands/role.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/management/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/dauthz/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/middlewares/enforcer_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/middlewares/request_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/dauthz/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-28 15:44:17.000000 django-authorization-1.2.1/dauthz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/django_authorization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2023-10-28 15:44:56.000000 django-authorization-1.2.1/django_authorization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2023-10-28 15:44:56.000000 django-authorization-1.2.1/django_authorization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 15:44:56.000000 django-authorization-1.2.1/django_authorization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-28 15:44:56.000000 django-authorization-1.2.1/django_authorization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-28 15:44:56.000000 django-authorization-1.2.1/django_authorization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/npm/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.340870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1250 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.344870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
--rw-r--r--   0 runner    (1001) docker     (127)    45350 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74297 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)    19742 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24096 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3709 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31684 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    49966 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    49248 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17553 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
--rw-r--r--   0 runner    (1001) docker     (127)   110406 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
--rw-r--r--   0 runner    (1001) docker     (127)   150550 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1266 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   118407 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    66115 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   126719 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30260 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    54358 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15164 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    81834 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
--rw-r--r--   0 runner    (1001) docker     (127)   135712 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7691 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3063 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/tools/graphviz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5021 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_gyp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5482 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_sln.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10633 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_vcproj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/test/fixtures/test-charmap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2337 2023-10-28 15:44:32.000000 django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/update-gyp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/semantic-release-pypi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.336870 django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/py/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-10-28 15:44:34.000000 django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/py/set_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-10-28 15:44:34.000000 django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/py/verify_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-28 15:44:48.000000 django-authorization-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-28 15:44:17.000000 django-authorization-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 15:44:56.348870 django-authorization-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 15:44:56.348870 django-authorization-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-10-28 15:44:17.000000 django-authorization-1.2.1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-10-28 15:44:17.000000 django-authorization-1.2.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-10-28 15:44:17.000000 django-authorization-1.2.1/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-10-28 15:44:17.000000 django-authorization-1.2.1/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-10-28 15:44:17.000000 django-authorization-1.2.1/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.396223 django_authorization-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:02:34.000000 django_authorization-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-24 13:03:05.396223 django_authorization-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-24 13:02:34.000000 django_authorization-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/dauthz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/dauthz/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/dauthz/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/backends/casbin_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/dauthz/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/decorators/_enforcer_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/decorators/_request_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/dauthz/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/dauthz/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/commands/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/commands/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/management/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/dauthz/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/middlewares/enforcer_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/middlewares/request_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/dauthz/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 13:02:34.000000 django_authorization-1.3.0/dauthz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.396223 django_authorization-1.3.0/django_authorization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-24 13:03:05.000000 django_authorization-1.3.0/django_authorization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-24 13:03:05.000000 django_authorization-1.3.0/django_authorization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:03:05.000000 django_authorization-1.3.0/django_authorization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 13:03:05.000000 django_authorization-1.3.0/django_authorization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 13:03:05.000000 django_authorization-1.3.0/django_authorization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.372223 django_authorization-1.3.0/node_modules/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/npm/node_modules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.380222 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1250 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.388223 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45344 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74297 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24134 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22667 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3950 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.392223 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31562 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49950 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49196 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110262 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)   150892 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1266 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118347 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66020 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126254 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30260 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54090 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15131 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81728 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135641 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.396223 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33036 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39969 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18355 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16236 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7691 2024-04-24 13:02:44.000000 django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/semantic-release-pypi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.376222 django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.396223 django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 13:02:47.000000 django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/py/set_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 13:02:47.000000 django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/py/verify_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-24 13:03:02.000000 django_authorization-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 13:02:34.000000 django_authorization-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:03:05.396223 django_authorization-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:03:05.396223 django_authorization-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-24 13:02:34.000000 django_authorization-1.3.0/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 13:02:34.000000 django_authorization-1.3.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 13:02:34.000000 django_authorization-1.3.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-24 13:02:34.000000 django_authorization-1.3.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-24 13:02:34.000000 django_authorization-1.3.0/tests/test_middleware.py
```

### Comparing `django-authorization-1.2.1/LICENSE` & `django_authorization-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/PKG-INFO` & `django_authorization-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.2.1
+Version: 1.3.0
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Author-email: JonLee <leeqvip@gmail.com>
 License: Apache 2.0
 Project-URL: Home-page, https://github.com/pycasbin/django-authorization
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,42 +17,35 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: casbin>=1.17.0
 Requires-Dist: Django>=3.0.0
 
 # Django Authorization
 
-English | [中文](README_zh.md)
-
-
-
-Django-authorization is an authorization library for Django framework.
-
 [![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/django-authorization?branch=master)
 [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
-Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
+Django-authorization is an authorization library for Django framework.
 
-![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
+Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
+![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 - [Django Authorization](#django-authorization)
   * [Installation and Configure](#installation-and-configure)
   * [Usage](#usage)
     + [Some Important Concepts:](#some-important-concepts-)
     + [Middleware Usage](#middleware-usage)
     + [Decorator Usage](#decorator-usage)
     + [Command Line Usage](#command-line-usage)
   * [License](#license)
 
-
-
 ## Installation and Configure
 
 ```
 pip install django-authorization
 ```
 
 We recommend that you first configure the adapter for persistent storage of the policy, such as:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-authorization-1.2.1/README.md` & `django_authorization-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 # Django Authorization
 
-English | [中文](README_zh.md)
-
-
-
-Django-authorization is an authorization library for Django framework.
-
 [![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/django-authorization?branch=master)
 [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
-Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
+Django-authorization is an authorization library for Django framework.
 
-![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
+Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
+![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 - [Django Authorization](#django-authorization)
   * [Installation and Configure](#installation-and-configure)
   * [Usage](#usage)
     + [Some Important Concepts:](#some-important-concepts-)
     + [Middleware Usage](#middleware-usage)
     + [Decorator Usage](#decorator-usage)
     + [Command Line Usage](#command-line-usage)
   * [License](#license)
 
-
-
 ## Installation and Configure
 
 ```
 pip install django-authorization
 ```
 
 We recommend that you first configure the adapter for persistent storage of the policy, such as:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-authorization-1.2.1/dauthz/backends/casbin_backend.py` & `django_authorization-1.3.0/dauthz/backends/casbin_backend.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/core.py` & `django_authorization-1.3.0/dauthz/core.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/management/commands/group.py` & `django_authorization-1.3.0/dauthz/management/commands/group.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/management/commands/policy.py` & `django_authorization-1.3.0/dauthz/management/commands/policy.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/management/commands/role.py` & `django_authorization-1.3.0/dauthz/management/commands/role.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/middlewares/enforcer_middleware.py` & `django_authorization-1.3.0/dauthz/middlewares/enforcer_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/middlewares/request_middleware.py` & `django_authorization-1.3.0/dauthz/middlewares/request_middleware.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/dauthz/settings.py` & `django_authorization-1.3.0/dauthz/settings.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/django_authorization.egg-info/PKG-INFO` & `django_authorization-1.3.0/django_authorization.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authorization
-Version: 1.2.1
+Version: 1.3.0
 Summary: An authorization library that supports access control models like ACL, RBAC, ABAC in Django
 Author-email: JonLee <leeqvip@gmail.com>
 License: Apache 2.0
 Project-URL: Home-page, https://github.com/pycasbin/django-authorization
 Keywords: casbin,django,acl,rbac,abac,auth,authz,authorization,access control,permission
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,42 +17,35 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: casbin>=1.17.0
 Requires-Dist: Django>=3.0.0
 
 # Django Authorization
 
-English | [中文](README_zh.md)
-
-
-
-Django-authorization is an authorization library for Django framework.
-
 [![tests](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml/badge.svg)](https://github.com/pycasbin/django-authorization/actions/workflows/release.yml)
 [![Coverage Status](https://coveralls.io/repos/github/pycasbin/django-authorization/badge.svg?branch=master)](https://coveralls.io/github/pycasbin/django-authorization?branch=master)
 [![Version](https://img.shields.io/pypi/v/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Download](https://img.shields.io/pypi/dm/django-authorization.svg)](https://pypi.org/project/django-authorization/)
 [![Discord](https://img.shields.io/discord/1022748306096537660?logo=discord&label=discord&color=5865F2)](https://discord.gg/S5UjpzGZjN)
 
-Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin ](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
+Django-authorization is an authorization library for Django framework.
 
-![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
+Based on [Casbin](https://github.com/casbin/pycasbin) and [Django-casbin](https://github.com/pycasbin/django-casbin) (middleware, light weight of this plugin), an authorization library that that supports access control models like ACL, RBAC, ABAC.
 
+![image](https://user-images.githubusercontent.com/75596353/188881538-a6a99cb1-c88b-4738-bf4f-452be4fb7c2d.png)
 
 - [Django Authorization](#django-authorization)
   * [Installation and Configure](#installation-and-configure)
   * [Usage](#usage)
     + [Some Important Concepts:](#some-important-concepts-)
     + [Middleware Usage](#middleware-usage)
     + [Decorator Usage](#decorator-usage)
     + [Command Line Usage](#command-line-usage)
   * [License](#license)
 
-
-
 ## Installation and Configure
 
 ```
 pip install django-authorization
 ```
 
 We recommend that you first configure the adapter for persistent storage of the policy, such as:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-authorization-1.2.1/django_authorization.egg-info/SOURCES.txt` & `django_authorization-1.3.0/django_authorization.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 dauthz/middlewares/request_middleware.py
 dauthz/migrations/__init__.py
 django_authorization.egg-info/PKG-INFO
 django_authorization.egg-info/SOURCES.txt
 django_authorization.egg-info/dependency_links.txt
 django_authorization.egg-info/requires.txt
 django_authorization.egg-info/top_level.txt
-node_modules/npm/node_modules/node-gyp/update-gyp.py
 node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py
 node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py
@@ -68,19 +67,29 @@
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py
 node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py
-node_modules/npm/node_modules/node-gyp/gyp/tools/graphviz.py
-node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_gyp.py
-node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_sln.py
-node_modules/npm/node_modules/node-gyp/gyp/tools/pretty_vcproj.py
-node_modules/npm/node_modules/node-gyp/test/fixtures/test-charmap.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/__init__.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_elffile.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_manylinux.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_musllinux.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_parser.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_structures.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/_tokenizer.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/markers.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/metadata.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/py.typed
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/requirements.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/specifiers.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/tags.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/utils.py
+node_modules/npm/node_modules/node-gyp/gyp/pylib/packaging/version.py
 node_modules/semantic-release-pypi/dist/py/set_version.py
 node_modules/semantic-release-pypi/dist/py/verify_setup.py
 tests/test_backend.py
 tests/test_basic.py
 tests/test_command.py
 tests/test_decorator.py
 tests/test_middleware.py
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/gyp_main.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSNew.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,27 +281,25 @@
                 f.write(
                     "\tProjectSection(WebsiteProperties) = preProject\r\n"
                     '\t\tDebug.AspNetCompiler.Debug = "True"\r\n'
                     '\t\tRelease.AspNetCompiler.Debug = "False"\r\n'
                     "\tEndProjectSection\r\n"
                 )
 
-            if isinstance(e, MSVSFolder):
-                if e.items:
-                    f.write("\tProjectSection(SolutionItems) = preProject\r\n")
-                    for i in e.items:
-                        f.write(f"\t\t{i} = {i}\r\n")
-                    f.write("\tEndProjectSection\r\n")
-
-            if isinstance(e, MSVSProject):
-                if e.dependencies:
-                    f.write("\tProjectSection(ProjectDependencies) = postProject\r\n")
-                    for d in e.dependencies:
-                        f.write(f"\t\t{d.get_guid()} = {d.get_guid()}\r\n")
-                    f.write("\tEndProjectSection\r\n")
+            if isinstance(e, MSVSFolder) and e.items:
+                f.write("\tProjectSection(SolutionItems) = preProject\r\n")
+                for i in e.items:
+                    f.write(f"\t\t{i} = {i}\r\n")
+                f.write("\tEndProjectSection\r\n")
+
+            if isinstance(e, MSVSProject) and e.dependencies:
+                f.write("\tProjectSection(ProjectDependencies) = postProject\r\n")
+                for d in e.dependencies:
+                    f.write(f"\t\t{d.get_guid()} = {d.get_guid()}\r\n")
+                f.write("\tEndProjectSection\r\n")
 
             f.write("EndProject\r\n")
 
         # Global section
         f.write("Global\r\n")
 
         # Configurations (variants)
@@ -349,15 +347,15 @@
         # never seen this be any different)
         f.write("\tGlobalSection(SolutionProperties) = preSolution\r\n")
         f.write("\t\tHideSolutionNode = FALSE\r\n")
         f.write("\tEndGlobalSection\r\n")
 
         # Folder mappings
         # Omit this section if there are no folders
-        if any([e.entries for e in all_entries if isinstance(e, MSVSFolder)]):
+        if any(e.entries for e in all_entries if isinstance(e, MSVSFolder)):
             f.write("\tGlobalSection(NestedProjects) = preSolution\r\n")
             for e in all_entries:
                 if not isinstance(e, MSVSFolder):
                     continue  # Does not apply to projects, only folders
                 for subentry in e.entries:
                     f.write(f"\t\t{subentry.get_guid()} = {e.get_guid()}\r\n")
             f.write("\tEndGlobalSection\r\n")
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSProject.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         for platform in platforms:
             self.platform_section.append(["Platform", {"Name": platform}])
         self.tool_files_section = ["ToolFiles"]
         self.configurations_section = ["Configurations"]
         self.files_section = ["Files"]
 
         # Keep a dict keyed on filename to speed up access.
-        self.files_dict = dict()
+        self.files_dict = {}
 
     def AddToolFile(self, path):
         """Adds a tool file to the project.
 
     Args:
       path: Relative path from project to tool file.
     """
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             return ConvertVCMacrosToMSBuild(value)
 
 
 class _Boolean(_Type):
     """Boolean settings, can have the values 'false' or 'true'."""
 
     def _Validate(self, value):
-        if value != "true" and value != "false":
+        if value not in {"true", "false"}:
             raise ValueError("expected bool; got %r" % value)
 
     def ValidateMSVS(self, value):
         self._Validate(value)
 
     def ValidateMSBuild(self, value):
         self._Validate(value)
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSSettings_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSToolFile.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUserFile.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSUtil.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/MSVSVersion.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,17 @@
     for (key, val) in generator.generator_default_variables.items():
         default_variables.setdefault(key, val)
 
     output_dir = params["options"].generator_output or params["options"].toplevel_dir
     if default_variables["GENERATOR"] == "ninja":
         default_variables.setdefault(
             "PRODUCT_DIR_ABS",
-            os.path.join(output_dir, "out", default_variables["build_type"]),
+            os.path.join(
+                output_dir, "out", default_variables.get("build_type", "default")
+            ),
         )
     else:
         default_variables.setdefault(
             "PRODUCT_DIR_ABS",
             os.path.join(output_dir, default_variables["CONFIGURATION_NAME"]),
         )
 
@@ -618,15 +620,15 @@
     # are global across all generator runs.
     gen_flags = []
     if options.use_environment:
         gen_flags += ShlexEnv("GYP_GENERATOR_FLAGS")
     if options.generator_flags:
         gen_flags += options.generator_flags
     generator_flags = NameValueListToDict(gen_flags)
-    if DEBUG_GENERAL in gyp.debug.keys():
+    if DEBUG_GENERAL in gyp.debug:
         DebugOutput(DEBUG_GENERAL, "generator_flags: %s", generator_flags)
 
     # Generate all requested formats (use a set in case we got one format request
     # twice)
     for format in set(options.formats):
         params = {
             "options": options,
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,28 +140,24 @@
     # relative_to.
     # If |follow_symlink_path| is true (default) and |path| is a symlink, then
     # this method returns a path to the real file represented by |path|. If it is
     # false, this method returns a path to the symlink. If |path| is not a
     # symlink, this option has no effect.
 
     # Convert to normalized (and therefore absolute paths).
-    if follow_path_symlink:
-        path = os.path.realpath(path)
-    else:
-        path = os.path.abspath(path)
+    path = os.path.realpath(path) if follow_path_symlink else os.path.abspath(path)
     relative_to = os.path.realpath(relative_to)
 
     # On Windows, we can't create a relative path to a different drive, so just
     # use the absolute path.
-    if sys.platform == "win32":
-        if (
-            os.path.splitdrive(path)[0].lower()
-            != os.path.splitdrive(relative_to)[0].lower()
-        ):
-            return path
+    if sys.platform == "win32" and (
+        os.path.splitdrive(path)[0].lower()
+        != os.path.splitdrive(relative_to)[0].lower()
+    ):
+        return path
 
     # Split the paths into components.
     path_split = path.split(os.path.sep)
     relative_to_split = relative_to.split(os.path.sep)
 
     # Determine how much of the prefix the two paths share.
     prefix_len = len(os.path.commonprefix([path_split, relative_to_split]))
@@ -273,18 +269,15 @@
   to remain intact without escaping the $, to allow the argument to contain
   references to variables to be expanded by the shell.
   """
 
     if not isinstance(argument, str):
         argument = str(argument)
 
-    if _quote.search(argument):
-        quote = '"'
-    else:
-        quote = ""
+    quote = '"' if _quote.search(argument) else ""
 
     encoded = quote + re.sub(_escape, r"\\\1", argument) + quote
 
     return encoded
 
 
 def EncodePOSIXShellList(list):
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/common_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,19 @@
     encoding: The encoding to report on the first line of the XML file.
     pretty: True if we want pretty printing with indents and new lines.
   """
     xml_string = XmlToString(content, encoding, pretty)
     if win32 and os.linesep != "\r\n":
         xml_string = xml_string.replace("\n", "\r\n")
 
-    default_encoding = locale.getdefaultlocale()[1]
+    try:  # getdefaultlocale() was removed in Python 3.11
+        default_encoding = locale.getdefaultlocale()[1]
+    except AttributeError:
+        default_encoding = locale.getencoding()
+
     if default_encoding and default_encoding.upper() != encoding.upper():
         xml_string = xml_string.encode(encoding)
 
     # Get the old content
     try:
         with open(path) as file:
             existing = file.read()
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/easy_xml_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             "</PropertyGroup>"
             '<Import Project="$(VCTargetsPath)\\Microsoft.Cpp.props"/>'
             "<PropertyGroup "
             "Condition=\"'$(Configuration)|$(Platform)'=="
             '\'Debug|Win32\'" Label="Configuration">'
             "<ConfigurationType>Application</ConfigurationType>"
             "<CharacterSet>Unicode</CharacterSet>"
+            "<SpectreMitigation>SpectreLoadCF</SpectreMitigation>"
+            "<VCToolsVersion>14.36.32532</VCToolsVersion>"
             "</PropertyGroup>"
             "</Project>"
         )
 
         xml = easy_xml.XmlToString(
             [
                 "Project",
@@ -95,14 +97,16 @@
                     "PropertyGroup",
                     {
                         "Condition": "'$(Configuration)|$(Platform)'=='Debug|Win32'",
                         "Label": "Configuration",
                     },
                     ["ConfigurationType", "Application"],
                     ["CharacterSet", "Unicode"],
+                    ["SpectreMitigation", "SpectreLoadCF"],
+                    ["VCToolsVersion", "14.36.32532"],
                 ],
             ]
         )
         self.assertEqual(xml, target)
 
 
 if __name__ == "__main__":
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/flock_tool.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         target.visited = True
         target.requires_build = _DoesTargetTypeRequireBuild(target_dicts[target_name])
         target_type = target_dicts[target_name]["type"]
         target.is_executable = target_type == "executable"
         target.is_static_library = target_type == "static_library"
         target.is_or_has_linked_ancestor = (
-            target_type == "executable" or target_type == "shared_library"
+            target_type in {"executable", "shared_library"}
         )
 
         build_file = gyp.common.ParseQualifiedTarget(target_name)[0]
         if build_file not in build_file_in_files:
             build_file_in_files[build_file] = _WasBuildFileModified(
                 build_file, data, files, toplevel_dir
             )
@@ -429,34 +429,34 @@
   . mapping (dictionary) from unqualified name to Target for all the
     Targets in |to_find|.
   . any target names not found. If this is empty all targets were found."""
     result = {}
     if not to_find:
         return {}, []
     to_find = set(to_find)
-    for target_name in all_targets.keys():
+    for target_name in all_targets:
         extracted = gyp.common.ParseQualifiedTarget(target_name)
         if len(extracted) > 1 and extracted[1] in to_find:
             to_find.remove(extracted[1])
             result[extracted[1]] = all_targets[target_name]
             if not to_find:
                 return result, []
-    return result, [x for x in to_find]
+    return result, list(to_find)
 
 
 def _DoesTargetDependOnMatchingTargets(target):
     """Returns true if |target| or any of its dependencies is one of the
   targets containing the files supplied as input to analyzer. This updates
   |matches| of the Targets as it recurses.
   target: the Target to look for."""
     if target.match_status == MATCH_STATUS_DOESNT_MATCH:
         return False
     if (
-        target.match_status == MATCH_STATUS_MATCHES
-        or target.match_status == MATCH_STATUS_MATCHES_BY_DEPENDENCY
+        target.match_status in {MATCH_STATUS_MATCHES,
+                                MATCH_STATUS_MATCHES_BY_DEPENDENCY}
     ):
         return True
     for dep in target.deps:
         if _DoesTargetDependOnMatchingTargets(dep):
             target.match_status = MATCH_STATUS_MATCHES_BY_DEPENDENCY
             print("\t", target.name, "matches by dep", dep.name)
             return True
@@ -679,36 +679,34 @@
         test_target_names_no_all = set(self._test_target_names)
         test_target_names_no_all.discard("all")
         test_targets_no_all = _LookupTargets(
             test_target_names_no_all, self._unqualified_mapping
         )
         test_target_names_contains_all = "all" in self._test_target_names
         if test_target_names_contains_all:
-            test_targets = [
-                x for x in (set(test_targets_no_all) | set(self._root_targets))
-            ]
+            test_targets = list(set(test_targets_no_all) | set(self._root_targets))
         else:
-            test_targets = [x for x in test_targets_no_all]
+            test_targets = list(test_targets_no_all)
         print("supplied test_targets")
         for target_name in self._test_target_names:
             print("\t", target_name)
         print("found test_targets")
         for target in test_targets:
             print("\t", target.name)
         print("searching for matching test targets")
         matching_test_targets = _GetTargetsDependingOnMatchingTargets(test_targets)
         matching_test_targets_contains_all = test_target_names_contains_all and set(
             matching_test_targets
         ) & set(self._root_targets)
         if matching_test_targets_contains_all:
             # Remove any of the targets for all that were not explicitly supplied,
             # 'all' is subsequentely added to the matching names below.
-            matching_test_targets = [
-                x for x in (set(matching_test_targets) & set(test_targets_no_all))
-            ]
+            matching_test_targets = list(
+                set(matching_test_targets) & set(test_targets_no_all)
+            )
         print("matched test_targets")
         for target in matching_test_targets:
             print("\t", target.name)
         matching_target_names = [
             gyp.common.ParseQualifiedTarget(target.name)[1]
             for target in matching_test_targets
         ]
@@ -725,17 +723,15 @@
         for target in self._name_to_target.values():
             target.visited = False
 
         supplied_targets = _LookupTargets(
             self._supplied_target_names_no_all(), self._unqualified_mapping
         )
         if "all" in self._supplied_target_names():
-            supplied_targets = [
-                x for x in (set(supplied_targets) | set(self._root_targets))
-            ]
+            supplied_targets = list(set(supplied_targets) | set(self._root_targets))
         print("Supplied test_targets & compile_targets")
         for target in supplied_targets:
             print("\t", target.name)
         print("Finding compile targets")
         compile_targets = _GetCompileTargets(self._changed_targets, supplied_targets)
         return [
             gyp.common.ParseQualifiedTarget(target.name)[1]
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/android.py`

 * *Files 2% similar despite different names*

```diff
@@ -693,15 +693,15 @@
                 "ERROR: What output file should be generated?",
                 "type",
                 self.type,
                 "target",
                 target,
             )
 
-        if self.type != "static_library" and self.type != "shared_library":
+        if self.type not in {"static_library", "shared_library"}:
             target_prefix = spec.get("product_prefix", target_prefix)
             target = spec.get("product_name", target)
             product_ext = spec.get("product_extension")
             if product_ext:
                 target_ext = "." + product_ext
 
         target_stem = target_prefix + target
@@ -735,17 +735,17 @@
             if self.toolset == "host":
                 path = (
                     "$(call intermediates-dir-for,%s,%s,true,,"
                     "$(GYP_HOST_VAR_PREFIX))"
                     % (self.android_class, self.android_module)
                 )
             else:
-                path = "$(call intermediates-dir-for,{},{},,,$(GYP_VAR_PREFIX))".format(
-                    self.android_class,
-                    self.android_module,
+                path = (
+                    "$(call intermediates-dir-for,"
+                    f"{self.android_class},{self.android_module},,,$(GYP_VAR_PREFIX))"
                 )
 
         assert spec.get("product_dir") is None  # TODO: not supported?
         return os.path.join(path, self.ComputeOutputBasename(spec))
 
     def NormalizeIncludePaths(self, include_paths):
         """Normalize include_paths.
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
   If rel_path is an absolute path it is returned unchanged.
   Otherwise it is resolved against base_path and normalized.
   If the result is a relative path, it is forced to be relative to the
   CMakeLists.txt.
   """
     if os.path.isabs(rel_path):
         return rel_path
-    if any([rel_path.startswith(var) for var in FULL_PATH_VARS]):
+    if any(rel_path.startswith(var) for var in FULL_PATH_VARS):
         return rel_path
     # TODO: do we need to check base_path for absolute variables as well?
     return os.path.join(
         "${CMAKE_CURRENT_LIST_DIR}", os.path.normpath(os.path.join(base_path, rel_path))
     )
 
 
@@ -324,15 +324,15 @@
         output.write("\n)\n")
 
         extra_deps.append(action_target_name)
 
 
 def NormjoinRulePathForceCMakeSource(base_path, rel_path, rule_source):
     if rel_path.startswith(("${RULE_INPUT_PATH}", "${RULE_INPUT_DIRNAME}")):
-        if any([rule_source.startswith(var) for var in FULL_PATH_VARS]):
+        if any(rule_source.startswith(var) for var in FULL_PATH_VARS):
             return rel_path
     return NormjoinPathForceCMakeSource(base_path, rel_path)
 
 
 def WriteRules(target_name, rules, extra_sources, extra_deps, path_to_gyp, output):
     """Write CMake for the 'rules' in the target.
 
@@ -925,18 +925,15 @@
                 "target",
                 target_name,
             )
 
         product_prefix = spec.get("product_prefix", default_product_prefix)
         product_name = spec.get("product_name", default_product_name)
         product_ext = spec.get("product_extension")
-        if product_ext:
-            product_ext = "." + product_ext
-        else:
-            product_ext = default_product_ext
+        product_ext = "." + product_ext if product_ext else default_product_ext
 
         SetTargetProperty(output, cmake_target_name, "PREFIX", product_prefix)
         SetTargetProperty(
             output,
             cmake_target_name,
             cmake_target_type.property_modifier + "_OUTPUT_NAME",
             product_name,
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/compile_commands_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "SHARED_LIB_PREFIX": "lib",
     "STATIC_LIB_PREFIX": "lib",
     "STATIC_LIB_SUFFIX": ".a",
 }
 
 
 def IsMac(params):
-    return "mac" == gyp.common.GetFlavor(params)
+    return gyp.common.GetFlavor(params) == "mac"
 
 
 def CalculateVariables(default_variables, params):
     default_variables.setdefault("OS", gyp.common.GetFlavor(params))
 
 
 def AddCommandsForTarget(cwd, target, params, per_config_commands):
@@ -89,30 +89,33 @@
                     defines,
                     includes,
                     cflags,
                     "-c",
                     gyp.common.EncodePOSIXShellArgument(file),
                 )
             )
-            commands.append(dict(command=command, directory=output_dir, file=file))
+            commands.append({"command": command, "directory": output_dir, "file": file})
 
 
 def GenerateOutput(target_list, target_dicts, data, params):
     per_config_commands = {}
     for qualified_target, target in target_dicts.items():
         build_file, target_name, toolset = gyp.common.ParseQualifiedTarget(
             qualified_target
         )
         if IsMac(params):
             settings = data[build_file]
             gyp.xcode_emulation.MergeGlobalXcodeSettingsToSpec(settings, target)
         cwd = os.path.dirname(build_file)
         AddCommandsForTarget(cwd, target, params, per_config_commands)
 
-    output_dir = params["generator_flags"].get("output_dir", "out")
+    try:
+        output_dir = params["options"].generator_output
+    except (AttributeError, KeyError):
+        output_dir = params["generator_flags"].get("output_dir", "out")
     for configuration_name, commands in per_config_commands.items():
         filename = os.path.join(output_dir, configuration_name, "compile_commands.json")
         gyp.common.EnsureDirExists(filename)
         fp = open(filename, "w")
         json.dump(commands, fp=fp, indent=0, check_circular=False)
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/dump_dependency_json.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/eclipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,18 +244,15 @@
         cpp_output = cpp_proc.communicate()[0].decode("utf-8")
         cpp_lines = cpp_output.split("\n")
         for cpp_line in cpp_lines:
             if not cpp_line.strip():
                 continue
             cpp_line_parts = cpp_line.split(" ", 2)
             key = cpp_line_parts[1]
-            if len(cpp_line_parts) >= 3:
-                val = cpp_line_parts[2]
-            else:
-                val = "1"
+            val = cpp_line_parts[2] if len(cpp_line_parts) >= 3 else "1"
             all_defines[key] = val
 
     return all_defines
 
 
 def WriteIncludePaths(out, eclipse_langs, include_dirs):
     """Write the includes section of a CDT settings export file."""
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypd.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/gypsh.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,14 +45,13 @@
         "target_dicts": target_dicts,
         "data": data,
     }
 
     # Use a banner that looks like the stock Python one and like what
     # code.interact uses by default, but tack on something to indicate what
     # locals are available, and identify gypsh.
-    banner = "Python {} on {}\nlocals.keys() = {}\ngypsh".format(
-        sys.version,
-        sys.platform,
-        repr(sorted(locals.keys())),
+    banner = (
+        f"Python {sys.version} on {sys.platform}\nlocals.keys() = "
+        f"{repr(sorted(locals.keys()))}\ngypsh"
     )
 
     code.interact(banner, local=locals)
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/make.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,18 +677,15 @@
     ".s": "cc",
     ".S": "cc",
 }
 
 
 def Compilable(filename):
     """Return true if the file is compilable (should be in OBJS)."""
-    for res in (filename.endswith(e) for e in COMPILABLE_EXTENSIONS):
-        if res:
-            return True
-    return False
+    return any(res for res in (filename.endswith(e) for e in COMPILABLE_EXTENSIONS))
 
 
 def Linkable(filename):
     """Return true if the file is linkable (should be on the link line)."""
     return filename.endswith(".o")
 
 
@@ -774,15 +771,15 @@
         self.flavor = flavor
 
         self.suffix_rules_srcdir = {}
         self.suffix_rules_objdir1 = {}
         self.suffix_rules_objdir2 = {}
 
         # Generate suffix rules for all compilable extensions.
-        for ext in COMPILABLE_EXTENSIONS.keys():
+        for ext in COMPILABLE_EXTENSIONS:
             # Suffix rules for source folder.
             self.suffix_rules_srcdir.update(
                 {
                     ext: (
                         """\
 $(obj).$(TOOLSET)/$(TARGET)/%%.o: $(srcdir)/%%%s FORCE_DO_CMD
 \t@$(call do_cmd,%s,1)
@@ -1062,15 +1059,15 @@
 
             # Set LD_LIBRARY_PATH in case the action runs an executable from this
             # build which links to shared libs from this build.
             # actions run on the host, so they should in theory only use host
             # libraries, but until everything is made cross-compile safe, also use
             # target libraries.
             # TODO(piman): when everything is cross-compile safe, remove lib.target
-            if self.flavor == "zos" or self.flavor == "aix":
+            if self.flavor in {"zos", "aix"}:
                 self.WriteLn(
                     "cmd_%s = LIBPATH=$(builddir)/lib.host:"
                     "$(builddir)/lib.target:$$LIBPATH; "
                     "export LIBPATH; "
                     "%s%s" % (name, cd_action, command)
                 )
             else:
@@ -1988,18 +1985,15 @@
                 installable_deps.append(self.output)
             if (
                 self.flavor == "mac"
                 and "product_dir" not in spec
                 and self.toolset == "target"
             ):
                 # On mac, products are created in install_path immediately.
-                assert install_path == self.output, "{} != {}".format(
-                    install_path,
-                    self.output,
-                )
+                assert install_path == self.output, f"{install_path} != {self.output}"
 
             # Point the target alias to the final binary output.
             self.WriteMakeRule(
                 [self.target], [install_path], comment="Add target alias", phony=True
             )
             if install_path != self.output:
                 assert not self.is_mac_bundle  # See comment a few lines above.
@@ -2030,15 +2024,15 @@
                     part_of_all=part_of_all,
                 )
                 # Place libnode.version.so and libnode.x symlink in lib.target dir
                 installable_deps.append(self.GetSharedObjectFromSidedeck(install_path))
                 installable_deps.append(
                     self.GetUnversionedSidedeckFromSidedeck(install_path)
                 )
-            if self.output != self.alias and self.alias != self.target:
+            if self.alias not in (self.output, self.target):
                 self.WriteMakeRule(
                     [self.alias],
                     installable_deps,
                     comment="Short alias for building this %s." % file_desc,
                     phony=True,
                 )
             if self.flavor == "zos" and self.type == "shared_library":
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
   Returns:
     The path with all slashes made into backslashes.
   """
     if (
         fixpath_prefix
         and path
         and not os.path.isabs(path)
-        and not path[0] == "$"
+        and path[0] != "$"
         and not _IsWindowsAbsPath(path)
     ):
         path = os.path.join(fixpath_prefix, path)
     if separator == "\\":
         path = path.replace("/", "\\")
     path = _NormalizedSource(path)
     if separator == "/":
@@ -277,17 +277,17 @@
     # TODO(bradnelson): ugly hack, fix this more generally!!!
     if "Directories" in setting or "Dependencies" in setting:
         if type(value) == str:
             value = value.replace("/", "\\")
         else:
             value = [i.replace("/", "\\") for i in value]
     if not tools.get(tool_name):
-        tools[tool_name] = dict()
+        tools[tool_name] = {}
     tool = tools[tool_name]
-    if "CompileAsWinRT" == setting:
+    if setting == "CompileAsWinRT":
         return
     if tool.get(setting):
         if only_if_unset:
             return
         if type(tool[setting]) == list and type(value) == list:
             tool[setting] += value
         else:
@@ -408,18 +408,15 @@
         if has_input_path and direct_cmd.find("INPUTPATH") >= 0:
             cmd += "set INPUTPATH=$(InputPath) && "
         cmd += 'bash -c "%(cmd)s"'
         cmd = cmd % {"cygwin_dir": cygwin_dir, "cmd": direct_cmd}
         return input_dir_preamble + cmd
     else:
         # Convert cat --> type to mimic unix.
-        if cmd[0] == "cat":
-            command = ["type"]
-        else:
-            command = [cmd[0].replace("/", "\\")]
+        command = ["type"] if cmd[0] == "cat" else [cmd[0].replace("/", "\\")]
         # Add call before command to ensure that commands can be tied together one
         # after the other without aborting in Incredibuild, since IB makes a bat
         # file out of the raw command string, and some commands (like python) are
         # actually batch files themselves.
         command.insert(0, "call")
         # Fix the paths
         # TODO(quote): This is a really ugly heuristic, and will miss path fixing
@@ -434,14 +431,15 @@
         ]
         arguments = [i.replace("$(InputDir)", "%INPUTDIR%") for i in arguments]
         arguments = [MSVSSettings.FixVCMacroSlashes(i) for i in arguments]
         if quote_cmd:
             # Support a mode for using cmd directly.
             # Convert any paths to native form (first element is used directly).
             # TODO(quote):  regularize quoting path names throughout the module
+            command[1] = '"%s"' % command[1]
             arguments = ['"%s"' % i for i in arguments]
         # Collapse into a single command.
         return input_dir_preamble + " ".join(command + arguments)
 
 
 def _BuildCommandLineForRule(spec, rule, has_input_path, do_setup_env):
     # Currently this weird argument munging is used to duplicate the way a
@@ -683,15 +681,15 @@
         trigger_files = _FindRuleTriggerFiles(rule, sources)
         for tf in trigger_files:
             inputs, outputs = _RuleInputsAndOutputs(rule, tf)
             all_inputs.update(OrderedSet(inputs))
             all_outputs.update(OrderedSet(outputs))
             # Only use one target from each rule as the dependency for
             # 'all' so we don't try to build each rule multiple times.
-            first_outputs.append(list(outputs)[0])
+            first_outputs.append(next(iter(outputs)))
             # Get the unique output directories for this rule.
             output_dirs = [os.path.split(i)[0] for i in outputs]
             for od in output_dirs:
                 all_output_dirs.add(od)
     first_outputs_cyg = [_Cygwinify(i) for i in first_outputs]
     # Write out all: target, including mkdir for each output directory.
     mk_file.write("all: %s\n" % " ".join(first_outputs_cyg))
@@ -752,15 +750,15 @@
   to understand why we have to do this.
 
   Args:
       s: The string to be escaped.
 
   Returns:
       The escaped string.
-  """  # noqa: E731,E123,E501
+  """
     s = s.replace("%", "%%")
     return s
 
 
 quote_replacer_regex = re.compile(r'(\\*)"')
 
 
@@ -1185,15 +1183,15 @@
     disabled_warnings = _GetDisabledWarnings(config)
     prebuild = config.get("msvs_prebuild")
     postbuild = config.get("msvs_postbuild")
     def_file = _GetModuleDefinition(spec)
     precompiled_header = config.get("msvs_precompiled_header")
 
     # Prepare the list of tools as a dictionary.
-    tools = dict()
+    tools = {}
     # Add in user specified msvs_settings.
     msvs_settings = config.get("msvs_settings", {})
     MSVSSettings.ValidateMSVSSettings(msvs_settings)
 
     # Prevent default library inheritance from the environment.
     _ToolAppend(tools, "VCLinkerTool", "AdditionalDependencies", ["$(NOINHERIT)"])
 
@@ -1380,18 +1378,15 @@
     config: The dictionary that defines the special processing to be done
             for this configuration.
   Returns:
     The list of preprocessor definitions.
   """
     defines = []
     for d in config.get("defines", []):
-        if type(d) == list:
-            fd = "=".join([str(dpart) for dpart in d])
-        else:
-            fd = str(d)
+        fd = "=".join([str(dpart) for dpart in d]) if isinstance(d, list) else str(d)
         defines.append(fd)
     return defines
 
 
 def _GetDisabledWarnings(config):
     return [str(i) for i in config.get("msvs_disabled_warnings", [])]
 
@@ -1574,18 +1569,18 @@
         msvs_version=version,
     )
 
     # Prune filters with a single child to flatten ugly directory structures
     # such as ../../src/modules/module1 etc.
     if version.UsesVcxproj():
         while (
-            all([isinstance(s, MSVSProject.Filter) for s in sources])
+            all(isinstance(s, MSVSProject.Filter) for s in sources)
             and len({s.name for s in sources}) == 1
         ):
-            assert all([len(s.contents) == 1 for s in sources])
+            assert all(len(s.contents) == 1 for s in sources)
             sources = [s.contents[0] for s in sources]
     else:
         while len(sources) == 1 and isinstance(sources[0], MSVSProject.Filter):
             sources = sources[0].contents
 
     return sources, excluded_sources, excluded_idl
 
@@ -1594,18 +1589,15 @@
     # If any non-native rules use 'idl' as an extension exclude idl files.
     # Gather a list here to use later.
     using_idl = False
     for rule in spec.get("rules", []):
         if rule["extension"] == "idl" and int(rule.get("msvs_external_rule", 0)):
             using_idl = True
             break
-    if using_idl:
-        excluded_idl = [i for i in sources if i.endswith(".idl")]
-    else:
-        excluded_idl = []
+    excluded_idl = [i for i in sources if i.endswith(".idl")] if using_idl else []
     return excluded_idl
 
 
 def _GetPrecompileRelatedFiles(spec):
     # Gather a list of precompiled header related sources.
     precompiled_related = []
     for _, config in spec["configurations"].items():
@@ -1782,48 +1774,45 @@
             # outputs, so do the same for our generated command line.
             if src.endswith("/"):
                 src_bare = src[:-1]
                 base_dir = posixpath.split(src_bare)[0]
                 outer_dir = posixpath.split(src_bare)[1]
                 fixed_dst = _FixPath(dst)
                 full_dst = f'"{fixed_dst}\\{outer_dir}\\"'
-                cmd = 'mkdir {} 2>nul & cd "{}" && xcopy /e /f /y "{}" {}'.format(
-                    full_dst,
-                    _FixPath(base_dir),
-                    outer_dir,
-                    full_dst,
+                cmd = (
+                    f'mkdir {full_dst} 2>nul & cd "{_FixPath(base_dir)}" && '
+                    f'xcopy /e /f /y "{outer_dir}" {full_dst}'
                 )
                 copies.append(
                     (
                         [src],
                         ["dummy_copies", dst],
                         cmd,
                         f"Copying {src} to {fixed_dst}",
                     )
                 )
             else:
                 fix_dst = _FixPath(cpy["destination"])
-                cmd = 'mkdir "{}" 2>nul & set ERRORLEVEL=0 & copy /Y "{}" "{}"'.format(
-                    fix_dst,
-                    _FixPath(src),
-                    _FixPath(dst),
+                cmd = (
+                    f'mkdir "{fix_dst}" 2>nul & set ERRORLEVEL=0 & '
+                    f'copy /Y "{_FixPath(src)}" "{_FixPath(dst)}"'
                 )
                 copies.append(([src], [dst], cmd, f"Copying {src} to {fix_dst}"))
     return copies
 
 
 def _GetPathDict(root, path):
     # |path| will eventually be empty (in the recursive calls) if it was initially
     # relative; otherwise it will eventually end up as '\', 'D:\', etc.
     if not path or path.endswith(os.sep):
         return root
     parent, folder = os.path.split(path)
     parent_dict = _GetPathDict(root, parent)
     if folder not in parent_dict:
-        parent_dict[folder] = dict()
+        parent_dict[folder] = {}
     return parent_dict[folder]
 
 
 def _DictsToFolders(base_path, bucket, flat):
     # Convert to folders recursively.
     children = []
     for folder, contents in bucket.items():
@@ -1903,17 +1892,16 @@
 def _GetPlatformOverridesOfProject(spec):
     # Prepare a dict indicating which project configurations are used for which
     # solution configurations for this target.
     config_platform_overrides = {}
     for config_name, c in spec["configurations"].items():
         config_fullname = _ConfigFullName(config_name, c)
         platform = c.get("msvs_target_platform", _ConfigPlatform(c))
-        fixed_config_fullname = "{}|{}".format(
-            _ConfigBaseName(config_name, _ConfigPlatform(c)),
-            platform,
+        fixed_config_fullname = (
+            f"{_ConfigBaseName(config_name, _ConfigPlatform(c))}|{platform}"
         )
         if spec["toolset"] == "host" and generator_supports_multiple_toolsets:
             fixed_config_fullname = f"{config_name}|x64"
         config_platform_overrides[config_fullname] = fixed_config_fullname
     return config_platform_overrides
 
 
@@ -3009,26 +2997,34 @@
 
 def _GetMSBuildConfigurationDetails(spec, build_file):
     properties = {}
     for name, settings in spec["configurations"].items():
         msbuild_attributes = _GetMSBuildAttributes(spec, settings, build_file)
         condition = _GetConfigurationCondition(name, settings, spec)
         character_set = msbuild_attributes.get("CharacterSet")
+        vctools_version = msbuild_attributes.get("VCToolsVersion")
         config_type = msbuild_attributes.get("ConfigurationType")
         _AddConditionalProperty(properties, condition, "ConfigurationType", config_type)
+        spectre_mitigation = msbuild_attributes.get('SpectreMitigation')
+        if spectre_mitigation:
+            _AddConditionalProperty(properties, condition, "SpectreMitigation",
+                                    spectre_mitigation)
         if config_type == "Driver":
             _AddConditionalProperty(properties, condition, "DriverType", "WDM")
             _AddConditionalProperty(
                 properties, condition, "TargetVersion", _ConfigTargetVersion(settings)
             )
-        if character_set:
-            if "msvs_enable_winrt" not in spec:
-                _AddConditionalProperty(
-                    properties, condition, "CharacterSet", character_set
-                )
+        if character_set and "msvs_enable_winrt" not in spec:
+            _AddConditionalProperty(
+                properties, condition, "CharacterSet", character_set
+            )
+        if vctools_version and "msvs_enable_winrt" not in spec:
+            _AddConditionalProperty(
+                properties, condition, "VCToolsVersion", vctools_version
+            )
     return _GetMSBuildPropertyGroup(spec, "Configuration", properties)
 
 
 def _GetMSBuildLocalProperties(msbuild_toolset):
     # Currently the only local property we support is PlatformToolset
     properties = {}
     if msbuild_toolset:
@@ -3100,14 +3096,18 @@
             if not directory.endswith("\\"):
                 directory += "\\"
             msbuild_attributes[a] = directory
         elif a == "CharacterSet":
             msbuild_attributes[a] = _ConvertMSVSCharacterSet(msvs_attributes[a])
         elif a == "ConfigurationType":
             msbuild_attributes[a] = _ConvertMSVSConfigurationType(msvs_attributes[a])
+        elif a == "SpectreMitigation":
+            msbuild_attributes[a] = msvs_attributes[a]
+        elif a == "VCToolsVersion":
+            msbuild_attributes[a] = msvs_attributes[a]
         else:
             print("Warning: Do not know how to convert MSVS attribute " + a)
     return msbuild_attributes
 
 
 def _ConvertMSVSCharacterSet(char_set):
     if char_set.isdigit():
@@ -3322,23 +3322,22 @@
         group = [
             "ItemDefinitionGroup",
             {"Condition": _GetConfigurationCondition(name, configuration, spec)},
         ]
         for tool_name, tool_settings in sorted(msbuild_settings.items()):
             # Skip the tool named '' which is a holder of global settings handled
             # by _GetMSBuildConfigurationGlobalProperties.
-            if tool_name:
-                if tool_settings:
-                    tool = [tool_name]
-                    for name, value in sorted(tool_settings.items()):
-                        formatted_value = _GetValueFormattedForMSBuild(
-                            tool_name, name, value
-                        )
-                        tool.append([name, formatted_value])
-                    group.append(tool)
+            if tool_name and tool_settings:
+                tool = [tool_name]
+                for name, value in sorted(tool_settings.items()):
+                    formatted_value = _GetValueFormattedForMSBuild(
+                        tool_name, name, value
+                    )
+                    tool.append([name, formatted_value])
+                group.append(tool)
         groups.append(group)
     return groups
 
 
 def _FinalizeMSBuildSettings(spec, configuration):
     if "msbuild_settings" in configuration:
         converted = False
@@ -3458,18 +3457,15 @@
         # For most tools, entries in a list should be separated with ';' but some
         # settings use a space.  Check for those first.
         exceptions = {
             "ClCompile": ["AdditionalOptions"],
             "Link": ["AdditionalOptions"],
             "Lib": ["AdditionalOptions"],
         }
-        if tool_name in exceptions and name in exceptions[tool_name]:
-            char = " "
-        else:
-            char = ";"
+        char = " " if name in exceptions.get(tool_name, []) else ";"
         formatted_value = char.join(
             [MSVSSettings.ConvertVCMacrosToMSBuild(i) for i in value]
         )
     else:
         formatted_value = MSVSSettings.ConvertVCMacrosToMSBuild(value)
     return formatted_value
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/msvs_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja.py`

 * *Files 0% similar despite different names*

```diff
@@ -1811,18 +1811,15 @@
         DEFAULT_EXTENSION = {
             "loadable_module": default_variables["SHARED_LIB_SUFFIX"],
             "shared_library": default_variables["SHARED_LIB_SUFFIX"],
             "static_library": default_variables["STATIC_LIB_SUFFIX"],
             "executable": default_variables["EXECUTABLE_SUFFIX"],
         }
         extension = spec.get("product_extension")
-        if extension:
-            extension = "." + extension
-        else:
-            extension = DEFAULT_EXTENSION.get(type, "")
+        extension = "." + extension if extension else DEFAULT_EXTENSION.get(type, "")
 
         if "product_name" in spec:
             # If we were given an explicit name, use that.
             target = spec["product_name"]
         else:
             # Otherwise, derive a name from the target name.
             target = spec["target_name"]
@@ -2529,15 +2526,15 @@
         )
 
         master_ninja.rule(
             "solink",
             description="SOLINK $lib",
             restat=True,
             command=mtime_preserving_solink_base
-            % {"suffix": "@$link_file_list"},  # noqa: E501
+            % {"suffix": "@$link_file_list"},
             rspfile="$link_file_list",
             rspfile_content=(
                 "-Wl,--whole-archive $in $solibs -Wl," "--no-whole-archive $libs"
             ),
             pool="link_pool",
         )
         master_ninja.rule(
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/ninja_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,15 +435,15 @@
                         )
 
         # Update all references to other projects, to make sure that the lists of
         # remote products are complete.  Otherwise, Xcode will fill them in when
         # it opens the project file, which will result in unnecessary diffs.
         # TODO(mark): This is evil because it relies on internal knowledge of
         # PBXProject._other_pbxprojects.
-        for other_pbxproject in self.project._other_pbxprojects.keys():
+        for other_pbxproject in self.project._other_pbxprojects:
             self.project.AddOrGetProjectReference(other_pbxproject)
 
         self.project.SortRemoteProductReferences()
 
         # Give everything an ID.
         self.project_file.ComputeIDs()
 
@@ -1114,18 +1114,15 @@
                     # Add a rule that declares it can build each concrete output of a
                     # rule source.  Collect the names of the directories that are
                     # required.
                     concrete_output_dirs = []
                     for concrete_output_index, concrete_output in enumerate(
                         concrete_outputs
                     ):
-                        if concrete_output_index == 0:
-                            bol = ""
-                        else:
-                            bol = "    "
+                        bol = "" if concrete_output_index == 0 else "    "
                         makefile.write(f"{bol}{concrete_output} \\\n")
 
                         concrete_output_dir = posixpath.dirname(concrete_output)
                         if (
                             concrete_output_dir
                             and concrete_output_dir not in concrete_output_dirs
                         ):
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/generator/xcode_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import re
 import shlex
 import signal
 import subprocess
 import sys
 import threading
 import traceback
-from distutils.version import StrictVersion
 from gyp.common import GypError
 from gyp.common import OrderedSet
+from packaging.version import Version
 
 # A list of types that are treated as linkable.
 linkable_types = [
     "executable",
     "shared_library",
     "loadable_module",
     "mac_kernel_extension",
@@ -221,15 +221,15 @@
 
 
 def LoadOneBuildFile(build_file_path, data, aux_data, includes, is_target, check):
     if build_file_path in data:
         return data[build_file_path]
 
     if os.path.exists(build_file_path):
-        build_file_contents = open(build_file_path, encoding='utf-8').read()
+        build_file_contents = open(build_file_path, encoding="utf-8").read()
     else:
         raise GypError(f"{build_file_path} not found (cwd: {os.getcwd()})")
 
     build_file_data = None
     try:
         if check:
             build_file_data = CheckedEval(build_file_contents)
@@ -866,18 +866,15 @@
                 build_file_dir = None
 
         # Support <|(listfile.txt ...) which generates a file
         # containing items from a gyp list, generated at gyp time.
         # This works around actions/rules which have more inputs than will
         # fit on the command line.
         if file_list:
-            if type(contents) is list:
-                contents_list = contents
-            else:
-                contents_list = contents.split(" ")
+            contents_list = contents if type(contents) is list else contents.split(" ")
             replacement = contents_list[0]
             if os.path.isabs(replacement):
                 raise GypError('| cannot handle absolute paths, got "%s"' % replacement)
 
             if not generator_filelist_paths:
                 path = os.path.join(build_file_dir, replacement)
             else:
@@ -1134,26 +1131,24 @@
     i = 0
     result = None
     while i < len(condition):
         cond_expr = condition[i]
         true_dict = condition[i + 1]
         if type(true_dict) is not dict:
             raise GypError(
-                "{} {} must be followed by a dictionary, not {}".format(
-                    conditions_key, cond_expr, type(true_dict)
-                )
+                f"{conditions_key} {cond_expr} must be followed by a dictionary, not "
+                f"{type(true_dict)}"
             )
         if len(condition) > i + 2 and type(condition[i + 2]) is dict:
             false_dict = condition[i + 2]
             i = i + 3
             if i != len(condition):
                 raise GypError(
-                    "{} {} has {} unexpected trailing items".format(
-                        conditions_key, cond_expr, len(condition) - i
-                    )
+                    f"{conditions_key} {cond_expr} has {len(condition) - i} "
+                    "unexpected trailing items"
                 )
         else:
             false_dict = None
             i = i + 2
         if result is None:
             result = EvalSingleCondition(
                 cond_expr, true_dict, false_dict, phase, variables, build_file
@@ -1179,15 +1174,15 @@
 
     try:
         if cond_expr_expanded in cached_conditions_asts:
             ast_code = cached_conditions_asts[cond_expr_expanded]
         else:
             ast_code = compile(cond_expr_expanded, "<string>", "eval")
             cached_conditions_asts[cond_expr_expanded] = ast_code
-        env = {"__builtins__": {}, "v": StrictVersion}
+        env = {"__builtins__": {}, "v": Version}
         if eval(ast_code, env, variables):
             return true_dict
         return false_dict
     except SyntaxError as e:
         syntax_error = SyntaxError(
             "%s while evaluating condition '%s' in %s "
             "at character %d." % (str(e.args[0]), e.text, build_file, e.offset),
@@ -1575,22 +1570,20 @@
                 # wildcard.
                 dependency_target_dicts = data[dependency_build_file]["targets"]
                 for dependency_target_dict in dependency_target_dicts:
                     if int(dependency_target_dict.get("suppress_wildcard", False)):
                         continue
                     dependency_target_name = dependency_target_dict["target_name"]
                     if (
-                        dependency_target != "*"
-                        and dependency_target != dependency_target_name
+                        dependency_target not in {"*", dependency_target_name}
                     ):
                         continue
                     dependency_target_toolset = dependency_target_dict["toolset"]
                     if (
-                        dependency_toolset != "*"
-                        and dependency_toolset != dependency_target_toolset
+                        dependency_toolset not in {"*", dependency_target_toolset}
                     ):
                         continue
                     dependency = gyp.common.QualifiedTarget(
                         dependency_build_file,
                         dependency_target_name,
                         dependency_target_toolset,
                     )
@@ -1626,23 +1619,22 @@
     """Remove self dependencies from targets that have the prune_self_dependency
   variable set."""
     for target_name, target_dict in targets.items():
         for dependency_key in dependency_sections:
             dependencies = target_dict.get(dependency_key, [])
             if dependencies:
                 for t in dependencies:
-                    if t == target_name:
-                        if (
-                            targets[t]
-                            .get("variables", {})
-                            .get("prune_self_dependency", 0)
-                        ):
-                            target_dict[dependency_key] = Filter(
-                                dependencies, target_name
-                            )
+                    if t == target_name and (
+                        targets[t]
+                        .get("variables", {})
+                        .get("prune_self_dependency", 0)
+                    ):
+                        target_dict[dependency_key] = Filter(
+                            dependencies, target_name
+                        )
 
 
 def RemoveLinkDependenciesFromNoneTargets(targets):
     """Remove dependencies having the 'link_dependency' attribute from the 'none'
   targets."""
     for target_name, target_dict in targets.items():
         for dependency_key in dependency_sections:
@@ -2234,18 +2226,15 @@
     # Make membership testing of hashables in |to| (in particular, strings)
     # faster.
     hashable_to_set = {x for x in to if is_hashable(x)}
     for item in fro:
         singleton = False
         if type(item) in (str, int):
             # The cheap and easy case.
-            if is_paths:
-                to_item = MakePathRelative(to_file, fro_file, item)
-            else:
-                to_item = item
+            to_item = MakePathRelative(to_file, fro_file, item) if is_paths else item
 
             if not (type(item) is str and item.startswith("-")):
                 # Any string that doesn't begin with a "-" is a singleton - it can
                 # only appear once in a list, to be enforced by the list merge append
                 # or prepend.
                 singleton = True
         elif type(item) is dict:
@@ -2463,30 +2452,27 @@
             continue
         # Configurations inherit (most) settings from the enclosing target scope.
         # Get the inheritance relationship right by making a copy of the target
         # dict.
         new_configuration_dict = {}
         for (key, target_val) in target_dict.items():
             key_ext = key[-1:]
-            if key_ext in key_suffixes:
-                key_base = key[:-1]
-            else:
-                key_base = key
+            key_base = key[:-1] if key_ext in key_suffixes else key
             if key_base not in non_configuration_keys:
                 new_configuration_dict[key] = gyp.simple_copy.deepcopy(target_val)
 
         # Merge in configuration (with all its parents first).
         MergeConfigWithInheritance(
             new_configuration_dict, build_file, target_dict, configuration, []
         )
 
         merged_configurations[configuration] = new_configuration_dict
 
     # Put the new configurations back into the target dict as a configuration.
-    for configuration in merged_configurations.keys():
+    for configuration in merged_configurations:
         target_dict["configurations"][configuration] = merged_configurations[
             configuration
         ]
 
     # Now drop all the abstract ones.
     configs = target_dict["configurations"]
     target_dict["configurations"] = {
@@ -2495,27 +2481,24 @@
 
     # Now that all of the target's configurations have been built, go through
     # the target dict's keys and remove everything that's been moved into a
     # "configurations" section.
     delete_keys = []
     for key in target_dict:
         key_ext = key[-1:]
-        if key_ext in key_suffixes:
-            key_base = key[:-1]
-        else:
-            key_base = key
+        key_base = key[:-1] if key_ext in key_suffixes else key
         if key_base not in non_configuration_keys:
             delete_keys.append(key)
     for key in delete_keys:
         del target_dict[key]
 
     # Check the configurations to see if they contain invalid keys.
-    for configuration in target_dict["configurations"].keys():
+    for configuration in target_dict["configurations"]:
         configuration_dict = target_dict["configurations"][configuration]
-        for key in configuration_dict.keys():
+        for key in configuration_dict:
             if key in invalid_configuration_keys:
                 raise GypError(
                     "%s not allowed in the %s configuration, found in "
                     "target %s" % (key, configuration, target)
                 )
 
 
@@ -2550,15 +2533,15 @@
     # the _included and _excluded keys need to be added to the_dict, and that
     # can't be done while iterating through it.
 
     lists = []
     del_lists = []
     for key, value in the_dict.items():
         operation = key[-1]
-        if operation != "!" and operation != "/":
+        if operation not in {"!", "/"}:
             continue
 
         if type(value) is not list:
             raise ValueError(
                 name + " key " + key + " must be list, not " + value.__class__.__name__
             )
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/input_test.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/mac_tool.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/msvs_emulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,39 +89,39 @@
 
 
 def _AddPrefix(element, prefix):
     """Add |prefix| to |element| or each subelement if element is iterable."""
     if element is None:
         return element
     # Note, not Iterable because we don't want to handle strings like that.
-    if isinstance(element, list) or isinstance(element, tuple):
+    if isinstance(element, (list, tuple)):
         return [prefix + e for e in element]
     else:
         return prefix + element
 
 
 def _DoRemapping(element, map):
     """If |element| then remap it through |map|. If |element| is iterable then
     each item will be remapped. Any elements not found will be removed."""
     if map is not None and element is not None:
         if not callable(map):
             map = map.get  # Assume it's a dict, otherwise a callable to do the remap.
-        if isinstance(element, list) or isinstance(element, tuple):
+        if isinstance(element, (list, tuple)):
             element = filter(None, [map(elem) for elem in element])
         else:
             element = map(element)
     return element
 
 
 def _AppendOrReturn(append, element):
     """If |append| is None, simply return |element|. If |append| is not None,
     then add |element| to it, adding each item in |element| if it's a list or
     tuple."""
     if append is not None and element is not None:
-        if isinstance(element, list) or isinstance(element, tuple):
+        if isinstance(element, (list, tuple)):
             append.extend(element)
         else:
             append.append(element)
     else:
         return element
 
 
@@ -179,15 +179,15 @@
     if not all_system_includes:
         return None
     # Expand macros in all_system_includes.
     env = GetGlobalVSMacroEnv(GetVSVersion(generator_flags))
     expanded_system_includes = OrderedSet(
         [ExpandMacros(include, env) for include in all_system_includes]
     )
-    if any(["$" in include for include in expanded_system_includes]):
+    if any("$" in include for include in expanded_system_includes):
         # Some path relies on target-specific variables, bail.
         return None
 
     # Remove system includes shared by all targets from the targets.
     for config in configs:
         includes = config.get("msvs_system_include_dirs", [])
         if includes:  # Don't insert a msvs_system_include_dirs key if not needed.
@@ -251,18 +251,15 @@
             return ext
         return gyp.MSVSUtil.TARGET_TYPE_EXT.get(self.spec["type"], "")
 
     def GetVSMacroEnv(self, base_to_build=None, config=None):
         """Get a dict of variables mapping internal VS macro names to their gyp
         equivalents."""
         target_arch = self.GetArch(config)
-        if target_arch == "x86":
-            target_platform = "Win32"
-        else:
-            target_platform = target_arch
+        target_platform = "Win32" if target_arch == "x86" else target_arch
         target_name = self.spec.get("product_prefix", "") + self.spec.get(
             "product_name", self.spec["target_name"]
         )
         target_dir = base_to_build + "\\" if base_to_build else ""
         target_ext = "." + self.GetExtension()
         target_file_name = target_name + target_ext
 
@@ -734,18 +731,15 @@
         ld("ResourceOnlyDLL", map={"true": "/NOENTRY"})
         ld("EntryPointSymbol", prefix="/ENTRY:")
         ld("Profile", map={"true": "/PROFILE"})
         ld("LargeAddressAware", map={"1": ":NO", "2": ""}, prefix="/LARGEADDRESSAWARE")
         # TODO(scottmg): This should sort of be somewhere else (not really a flag).
         ld("AdditionalDependencies", prefix="")
 
-        if self.GetArch(config) == "x86":
-            safeseh_default = "true"
-        else:
-            safeseh_default = None
+        safeseh_default = "true" if self.GetArch(config) == "x86" else None
         ld(
             "ImageHasSafeExceptionHandlers",
             map={"false": ":NO", "true": ""},
             prefix="/SAFESEH",
             default=safeseh_default,
         )
 
@@ -832,25 +826,22 @@
                 "2": "requireAdministrator",
             }
 
             ui_access = self._Setting(
                 ("VCLinkerTool", "UACUIAccess"), config, default="false"
             )
 
-            inner = """
+            inner = f"""
 <trustInfo xmlns="urn:schemas-microsoft-com:asm.v3">
   <security>
     <requestedPrivileges>
-      <requestedExecutionLevel level='{}' uiAccess='{}' />
+      <requestedExecutionLevel level='{execution_level_map[execution_level]}' uiAccess='{ui_access}' />
     </requestedPrivileges>
   </security>
-</trustInfo>""".format(
-                execution_level_map[execution_level],
-                ui_access,
-            )
+</trustInfo>"""  # noqa: E501
         else:
             inner = ""
 
         generated_manifest_contents = generated_manifest_outer % inner
         generated_name = name + ".generated.manifest"
         # Need to join with the build_dir here as we're writing it during
         # generation time, but we return the un-joined version because the build
@@ -956,23 +947,20 @@
         quote_cmd = int(rule.get("msvs_quote_cmd", 1))
         assert quote_cmd != 0 or cygwin != 1, \
                "msvs_quote_cmd=0 only applicable for msvs_cygwin_shell=0"
         return MsvsSettings.RuleShellFlags(cygwin, quote_cmd)
 
     def _HasExplicitRuleForExtension(self, spec, extension):
         """Determine if there's an explicit rule for a particular extension."""
-        for rule in spec.get("rules", []):
-            if rule["extension"] == extension:
-                return True
-        return False
+        return any(rule["extension"] == extension for rule in spec.get("rules", []))
 
     def _HasExplicitIdlActions(self, spec):
         """Determine if an action should not run midl for .idl files."""
         return any(
-            [action.get("explicit_idl_action", 0) for action in spec.get("actions", [])]
+            action.get("explicit_idl_action", 0) for action in spec.get("actions", [])
         )
 
     def HasExplicitIdlRulesOrActions(self, spec):
         """Determine if there's an explicit rule or action for idl files. When
         there isn't we need to generate implicit rules to build MIDL .idl files."""
         return self._HasExplicitRuleForExtension(
             spec, "idl"
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/simple_copy.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/win_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,19 +215,18 @@
                 "-manifest %(out)s.manifest %(intermediate_manifest)s "
                 "-out:%(out)s.assert.manifest" % variables
             )
             assert_manifest = "%(out)s.assert.manifest" % variables
             our_manifest = "%(out)s.manifest" % variables
             # Load and normalize the manifests. mt.exe sometimes removes whitespace,
             # and sometimes doesn't unfortunately.
-            with open(our_manifest) as our_f:
-                with open(assert_manifest) as assert_f:
-                    translator = str.maketrans('', '', string.whitespace)
-                    our_data = our_f.read().translate(translator)
-                    assert_data = assert_f.read().translate(translator)
+            with open(our_manifest) as our_f, open(assert_manifest) as assert_f:
+                translator = str.maketrans("", "", string.whitespace)
+                our_data = our_f.read().translate(translator)
+                assert_data = assert_f.read().translate(translator)
             if our_data != assert_data:
                 os.unlink(out)
 
                 def dump(filename):
                     print(filename, file=sys.stderr)
                     print("-----", file=sys.stderr)
                     with open(filename) as f:
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_emulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,18 +681,15 @@
         cflags += self._Settings().get("WARNING_CFLAGS", [])
 
         if self._IsXCTest():
             platform_root = self._XcodePlatformPath(configname)
             if platform_root:
                 cflags.append("-F" + platform_root + "/Developer/Library/Frameworks/")
 
-        if sdk_root:
-            framework_root = sdk_root
-        else:
-            framework_root = ""
+        framework_root = sdk_root if sdk_root else ""
         config = self.spec["configurations"][self.configname]
         framework_dirs = config.get("mac_framework_dirs", [])
         for directory in framework_dirs:
             cflags.append("-F" + directory.replace("$(SDKROOT)", framework_root))
 
         self.configname = None
         return cflags
@@ -1244,18 +1241,15 @@
         return pre + postbuilds + post
 
     def _AdjustLibrary(self, library, config_name=None):
         if library.endswith(".framework"):
             l_flag = "-framework " + os.path.splitext(os.path.basename(library))[0]
         else:
             m = self.library_re.match(library)
-            if m:
-                l_flag = "-l" + m.group(1)
-            else:
-                l_flag = library
+            l_flag = "-l" + m.group(1) if m else library
 
         sdk_root = self._SdkPath(config_name)
         if not sdk_root:
             sdk_root = ""
         # Xcode 7 started shipping with ".tbd" (text based stubs) files instead of
         # ".dylib" without providing a real support for them. What it does, for
         # "/usr/lib" libraries, is do "-L/usr/lib -lname" which is dependent on the
@@ -1541,15 +1535,15 @@
     for key in [MAVERICKS_PKG_ID, STANDALONE_PKG_ID, FROM_XCODE_PKG_ID]:
         try:
             output = GetStdout(["/usr/sbin/pkgutil", "--pkg-info", key])
             return re.search(regex, output).groupdict()["version"]
         except GypError:
             continue
 
-    regex = re.compile(r'Command Line Tools for Xcode\s+(?P<version>\S+)')
+    regex = re.compile(r"Command Line Tools for Xcode\s+(?P<version>\S+)")
     try:
         output = GetStdout(["/usr/sbin/softwareupdate", "--history"])
         return re.search(regex, output).groupdict()["version"]
     except GypError:
         return None
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcode_ninja.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xcodeproj_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,15 +967,15 @@
 
     def __init__(self, properties=None, id=None, parent=None):
         # super
         XCObject.__init__(self, properties, id, parent)
         if "path" in self._properties and "name" not in self._properties:
             path = self._properties["path"]
             name = posixpath.basename(path)
-            if name != "" and path != name:
+            if name not in ("", path):
                 self.SetProperty("name", name)
 
         if "path" in self._properties and (
             "sourceTree" not in self._properties
             or self._properties["sourceTree"] == "<group>"
         ):
             # If the pathname begins with an Xcode variable like "$(SDKROOT)/", take
@@ -2351,17 +2351,16 @@
         # super
         XCRemoteObject.__init__(self, properties, id, parent)
 
         # Set up additional defaults not expressed in the schema.  If a "name"
         # property was supplied, set "productName" if it is not present.  Also set
         # the "PRODUCT_NAME" build setting in each configuration, but only if
         # the setting is not present in any build configuration.
-        if "name" in self._properties:
-            if "productName" not in self._properties:
-                self.SetProperty("productName", self._properties["name"])
+        if "name" in self._properties and "productName" not in self._properties:
+            self.SetProperty("productName", self._properties["name"])
 
         if "productName" in self._properties:
             if "buildConfigurationList" in self._properties:
                 configs = self._properties["buildConfigurationList"]
                 if configs.HasBuildSetting("PRODUCT_NAME") == 0:
                     configs.SetBuildSetting(
                         "PRODUCT_NAME", self._properties["productName"]
@@ -2543,21 +2542,20 @@
                     self.SetBuildSetting("MACH_O_TYPE", "mh_bundle")
                     self.SetBuildSetting("DYLIB_CURRENT_VERSION", "")
                     self.SetBuildSetting("DYLIB_COMPATIBILITY_VERSION", "")
                     if force_extension is None:
                         force_extension = suffix[1:]
 
                 if (
-                    self._properties["productType"]
-                    == "com.apple.product-type-bundle.unit.test"
-                    or self._properties["productType"]
-                    == "com.apple.product-type-bundle.ui-testing"
-                ):
-                    if force_extension is None:
-                        force_extension = suffix[1:]
+                    self._properties["productType"] in {
+                        "com.apple.product-type-bundle.unit.test",
+                        "com.apple.product-type-bundle.ui-testing"
+                    }
+                ) and force_extension is None:
+                    force_extension = suffix[1:]
 
                 if force_extension is not None:
                     # If it's a wrapper (bundle), set WRAPPER_EXTENSION.
                     # Extension override.
                     suffix = "." + force_extension
                     if filetype.startswith("wrapper."):
                         self.SetBuildSetting("WRAPPER_EXTENSION", force_extension)
@@ -2632,18 +2630,21 @@
         if headers_phase is None:
             headers_phase = PBXHeadersBuildPhase()
 
             # The headers phase should come before the resources, sources, and
             # frameworks phases, if any.
             insert_at = len(self._properties["buildPhases"])
             for index, phase in enumerate(self._properties["buildPhases"]):
-                if (
-                    isinstance(phase, PBXResourcesBuildPhase)
-                    or isinstance(phase, PBXSourcesBuildPhase)
-                    or isinstance(phase, PBXFrameworksBuildPhase)
+                if isinstance(
+                    phase,
+                    (
+                        PBXResourcesBuildPhase,
+                        PBXSourcesBuildPhase,
+                        PBXFrameworksBuildPhase,
+                    ),
                 ):
                     insert_at = index
                     break
 
             self._properties["buildPhases"].insert(insert_at, headers_phase)
             headers_phase.parent = self
 
@@ -2654,17 +2655,15 @@
         if resources_phase is None:
             resources_phase = PBXResourcesBuildPhase()
 
             # The resources phase should come before the sources and frameworks
             # phases, if any.
             insert_at = len(self._properties["buildPhases"])
             for index, phase in enumerate(self._properties["buildPhases"]):
-                if isinstance(phase, PBXSourcesBuildPhase) or isinstance(
-                    phase, PBXFrameworksBuildPhase
-                ):
+                if isinstance(phase, (PBXSourcesBuildPhase, PBXFrameworksBuildPhase)):
                     insert_at = index
                     break
 
             self._properties["buildPhases"].insert(insert_at, resources_phase)
             resources_phase.parent = self
 
         return resources_phase
@@ -2697,16 +2696,18 @@
             and "productType" in self._properties
             and self._properties["productType"] != static_library_type
             and "productType" in other._properties
             and (
                 other._properties["productType"] == static_library_type
                 or (
                     (
-                        other._properties["productType"] == shared_library_type
-                        or other._properties["productType"] == framework_type
+                        other._properties["productType"] in {
+                            shared_library_type,
+                            framework_type
+                        }
                     )
                     and (
                         (not other.HasBuildSetting("MACH_O_TYPE"))
                         or other.GetBuildSetting("MACH_O_TYPE") != "mh_bundle"
                     )
                 )
             )
```

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/pylib/gyp/xml_fix.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py` & `django_authorization-1.3.0/node_modules/npm/node_modules/node-gyp/gyp/test_gyp.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/py/set_version.py` & `django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/py/set_version.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/node_modules/semantic-release-pypi/dist/py/verify_setup.py` & `django_authorization-1.3.0/node_modules/semantic-release-pypi/dist/py/verify_setup.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/pyproject.toml` & `django_authorization-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-authorization"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
     {name = "JonLee", email = "leeqvip@gmail.com"},
 ]
 description = "An authorization library that supports access control models like ACL, RBAC, ABAC in Django"
 readme = "README.md"
 keywords = [
     "casbin",
```

### Comparing `django-authorization-1.2.1/tests/test_backend.py` & `django_authorization-1.3.0/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/tests/test_basic.py` & `django_authorization-1.3.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/tests/test_command.py` & `django_authorization-1.3.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/tests/test_decorator.py` & `django_authorization-1.3.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django-authorization-1.2.1/tests/test_middleware.py` & `django_authorization-1.3.0/tests/test_middleware.py`

 * *Files identical despite different names*

