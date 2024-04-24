# Comparing `tmp/craft_application-2.5.tar.gz` & `tmp/craft_application-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft_application-2.5.tar", last modified: Tue Apr 16 16:53:30 2024, max compression
+gzip compressed data, was "craft_application-2.6.tar", last modified: Wed Apr 24 18:24:07 2024, max compression
```

## Comparing `craft_application-2.5.tar` & `craft_application-2.6.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.747967 craft_application-2.5/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft_application-2.5/.editorconfig
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.719966 craft_application-2.5/.github/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft_application-2.5/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.719966 craft_application-2.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.5/.github/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.5/.github/release-drafter.yml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft_application-2.5/.github/renovate.json5
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/.github/workflows/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.5/.github/workflows/cla-check.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft_application-2.5/.github/workflows/docs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft_application-2.5/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft_application-2.5/.github/workflows/tests.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft_application-2.5/.gitignore
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft_application-2.5/.pre-commit-config.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft_application-2.5/.readthedocs.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft_application-2.5/.yamllint.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft_application-2.5/HACKING.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft_application-2.5/LICENSE
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-16 16:53:30.747967 craft_application-2.5/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft_application-2.5/README.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft_application-2.5/craft_application/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application/_version.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    29493 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/application.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft_application-2.5/craft_application/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/commands/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/commands/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/commands/other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft_application-2.5/craft_application/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3843 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/grammar.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/launchpad/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/launchpad/launchpad.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/launchpad/models/build.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/distro.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3496 2024-04-03 17:32:43.000000 craft_application-2.5/craft_application/launchpad/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft_application-2.5/craft_application/launchpad/models/recipe.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/launchpad/util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/misc/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/misc/instance_bashrc
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/models/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/models/constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3462 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/models/grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/models/metadata.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-04-16 16:52:04.000000 craft_application-2.5/craft_application/models/project.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/py.typed
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/remote/errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11974 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/remote/git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/remote/utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/remote/worktree.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    16185 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/services/lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft_application-2.5/craft_application/services/package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/services/provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    14846 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/services/remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/service_factory.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/craft_application/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/util/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/util/callbacks.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/util/error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft_application-2.5/craft_application/util/logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/util/paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft_application-2.5/craft_application/util/platforms.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2065 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/util/repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/util/snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/util/string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft_application-2.5/craft_application/util/yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/craft_application.egg-info/
--rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6026 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/top_level.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/docs/_static/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/_static/css/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-09-29 14:32:21.000000 craft_application-2.5/docs/_static/css/custom.css
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2023-09-29 14:32:21.000000 craft_application-2.5/docs/conf.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/explanation/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft_application-2.5/docs/explanation/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/howto/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft_application-2.5/docs/howto/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft_application-2.5/docs/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/reference/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft_application-2.5/docs/reference/index.rst
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/tutorials/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft_application-2.5/docs/tutorials/index.rst
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10638 2024-04-16 16:52:34.000000 craft_application-2.5/pyproject.toml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-16 16:53:30.747967 craft_application-2.5/setup.cfg
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     9326 2024-04-03 17:32:43.000000 craft_application-2.5/tests/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/integration/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3149 2024-04-03 17:32:43.000000 craft_application-2.5/tests/integration/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/integration/data/build-secrets/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/build-secrets/secret-source-folder/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft_application-2.5/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2023-10-19 21:00:44.000000 craft_application-2.5/tests/integration/data/build-secrets/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/invalid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/invalid_projects/build-error/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2023-10-25 15:47:00.000000 craft_application-2.5/tests/integration/data/invalid_projects/build-error/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/valid_projects/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/adoption/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/adoption/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/adoption/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/basic/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/basic/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/basic/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/environment/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/environment/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/environment/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/stderr
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      500 2024-04-16 16:52:34.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/testcraft.yaml
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/integration/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft_application-2.5/tests/integration/launchpad/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1700 2024-04-16 16:52:34.000000 craft_application-2.5/tests/integration/launchpad/test_anonymous_access.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft_application-2.5/tests/integration/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft_application-2.5/tests/integration/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1886 2024-04-03 17:32:43.000000 craft_application-2.5/tests/integration/services/test_remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft_application-2.5/tests/integration/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft_application-2.5/tests/integration/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft_application-2.5/tests/integration/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/test_version.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/unit/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/commands/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/commands/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft_application-2.5/tests/unit/commands/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/commands/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/commands/test_other.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/launchpad/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/launchpad/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/conftest.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/launchpad/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/launchpad/models/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/models/test_base.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/models/test_code.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft_application-2.5/tests/unit/launchpad/test_launchpad.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft_application-2.5/tests/unit/launchpad/test_util.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/models/project_models/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/basic_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/full_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/invalid_project.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/models/test_constraints.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-04-16 16:52:04.000000 craft_application-2.5/tests/unit/models/test_project.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/remote/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft_application-2.5/tests/unit/remote/test_git.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/remote/test_utils.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/test_worktree.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/services/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/services/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3946 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/services/conftest.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    21558 2024-04-02 11:30:59.000000 craft_application-2.5/tests/unit/services/test_lifecycle.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/services/test_package.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft_application-2.5/tests/unit/services/test_provider.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    11829 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/services/test_remotebuild.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3629 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/services/test_repositories.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/services/test_request.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-02-26 17:15:25.000000 craft_application-2.5/tests/unit/services/test_service_factory.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    53044 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/test_application.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/test_errors.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-04-16 16:52:04.000000 craft_application-2.5/tests/unit/test_grammar.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/test_nothing.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft_application-2.5/tests/unit/test_secrets.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/__init__.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/invalid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/_README
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft_application-2.5/tests/unit/util/test_error_formatting.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft_application-2.5/tests/unit/util/test_logging.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/util/test_paths.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft_application-2.5/tests/unit/util/test_snap_config.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/util/test_string.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft_application-2.5/tests/unit/util/test_yaml.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/valid_yaml/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/valid_yaml/empty.yaml
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-04-16 16:52:04.000000 craft_application-2.5/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.691014 craft_application-2.6/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft_application-2.6/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.663013 craft_application-2.6/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft_application-2.6/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.663013 craft_application-2.6/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft_application-2.6/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft_application-2.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft_application-2.6/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6/.github/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.6/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft_application-2.6/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.663013 craft_application-2.6/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.6/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft_application-2.6/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft_application-2.6/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft_application-2.6/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft_application-2.6/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft_application-2.6/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft_application-2.6/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft_application-2.6/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft_application-2.6/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft_application-2.6/LICENSE
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-24 18:24:07.691014 craft_application-2.6/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft_application-2.6/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.667013 craft_application-2.6/craft_application/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft_application-2.6/craft_application/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    29609 2024-04-24 18:21:50.000000 craft_application-2.6/craft_application/application.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.667013 craft_application-2.6/craft_application/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft_application-2.6/craft_application/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/commands/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/commands/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft_application-2.6/craft_application/commands/other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft_application-2.6/craft_application/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3843 2024-04-16 16:52:34.000000 craft_application-2.6/craft_application/grammar.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.667013 craft_application-2.6/craft_application/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/launchpad/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft_application-2.6/craft_application/launchpad/launchpad.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.667013 craft_application-2.6/craft_application/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft_application-2.6/craft_application/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft_application-2.6/craft_application/launchpad/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft_application-2.6/craft_application/launchpad/models/build.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft_application-2.6/craft_application/launchpad/models/code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft_application-2.6/craft_application/launchpad/models/distro.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3496 2024-04-03 17:32:43.000000 craft_application-2.6/craft_application/launchpad/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft_application-2.6/craft_application/launchpad/models/recipe.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft_application-2.6/craft_application/launchpad/util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.671013 craft_application-2.6/craft_application/misc/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/misc/instance_bashrc
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.671013 craft_application-2.6/craft_application/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-04-24 11:25:13.000000 craft_application-2.6/craft_application/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/models/constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3462 2024-04-22 14:18:58.000000 craft_application-2.6/craft_application/models/grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft_application-2.6/craft_application/models/metadata.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-04-24 11:25:13.000000 craft_application-2.6/craft_application/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/craft_application/py.typed
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.671013 craft_application-2.6/craft_application/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft_application-2.6/craft_application/remote/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11974 2024-04-16 16:52:34.000000 craft_application-2.6/craft_application/remote/git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/remote/utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/remote/worktree.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft_application-2.6/craft_application/secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.671013 craft_application-2.6/craft_application/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/services/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16549 2024-04-24 18:21:50.000000 craft_application-2.6/craft_application/services/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft_application-2.6/craft_application/services/package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-24 11:25:13.000000 craft_application-2.6/craft_application/services/provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14846 2024-04-16 16:52:34.000000 craft_application-2.6/craft_application/services/remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/services/request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/services/service_factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/craft_application/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/util/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft_application-2.6/craft_application/util/callbacks.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft_application-2.6/craft_application/util/error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft_application-2.6/craft_application/util/logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft_application-2.6/craft_application/util/paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft_application-2.6/craft_application/util/platforms.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2507 2024-04-24 18:21:50.000000 craft_application-2.6/craft_application/util/repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft_application-2.6/craft_application/util/snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft_application-2.6/craft_application/util/string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft_application-2.6/craft_application/util/yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.687013 craft_application-2.6/craft_application.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6026 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-24 18:24:07.000000 craft_application-2.6/craft_application.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.659013 craft_application-2.6/docs/_static/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-09-29 14:32:21.000000 craft_application-2.6/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2023-09-29 14:32:21.000000 craft_application-2.6/docs/conf.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/explanation/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft_application-2.6/docs/explanation/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/howto/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft_application-2.6/docs/howto/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft_application-2.6/docs/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/reference/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft_application-2.6/docs/reference/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/docs/tutorials/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft_application-2.6/docs/tutorials/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10638 2024-04-24 11:25:13.000000 craft_application-2.6/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-24 18:24:07.691014 craft_application-2.6/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9416 2024-04-24 18:21:50.000000 craft_application-2.6/tests/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3149 2024-04-03 17:32:43.000000 craft_application-2.6/tests/integration/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.659013 craft_application-2.6/tests/integration/data/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/integration/data/build-secrets/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/integration/data/build-secrets/secret-source-folder/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft_application-2.6/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2023-10-19 21:00:44.000000 craft_application-2.6/tests/integration/data/build-secrets/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.659013 craft_application-2.6/tests/integration/data/invalid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/integration/data/invalid_projects/build-error/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2023-10-25 15:47:00.000000 craft_application-2.6/tests/integration/data/invalid_projects/build-error/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.659013 craft_application-2.6/tests/integration/data/valid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.675013 craft_application-2.6/tests/integration/data/valid_projects/adoption/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/adoption/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/adoption/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/data/valid_projects/basic/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/basic/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/basic/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/data/valid_projects/environment/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/environment/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-02-26 17:15:25.000000 craft_application-2.6/tests/integration/data/valid_projects/environment/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/data/valid_projects/grammar/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.659013 craft_application-2.6/tests/integration/data/valid_projects/grammar/src/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.6/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft_application-2.6/tests/integration/data/valid_projects/grammar/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      500 2024-04-16 16:52:34.000000 craft_application-2.6/tests/integration/data/valid_projects/grammar/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6/tests/integration/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft_application-2.6/tests/integration/launchpad/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1709 2024-04-23 18:27:06.000000 craft_application-2.6/tests/integration/launchpad/test_anonymous_access.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.679013 craft_application-2.6/tests/integration/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/integration/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft_application-2.6/tests/integration/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft_application-2.6/tests/integration/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1886 2024-04-03 17:32:43.000000 craft_application-2.6/tests/integration/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft_application-2.6/tests/integration/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft_application-2.6/tests/integration/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft_application-2.6/tests/integration/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft_application-2.6/tests/integration/test_version.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft_application-2.6/tests/unit/commands/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft_application-2.6/tests/unit/commands/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/commands/test_other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft_application-2.6/tests/unit/launchpad/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft_application-2.6/tests/unit/launchpad/models/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft_application-2.6/tests/unit/launchpad/models/test_code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft_application-2.6/tests/unit/launchpad/test_launchpad.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft_application-2.6/tests/unit/launchpad/test_util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/models/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/models/project_models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/models/project_models/basic_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/models/project_models/full_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/models/project_models/invalid_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/models/test_constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-04-24 11:25:13.000000 craft_application-2.6/tests/unit/models/test_project.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.683014 craft_application-2.6/tests/unit/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/remote/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/remote/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft_application-2.6/tests/unit/remote/test_git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft_application-2.6/tests/unit/remote/test_utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/remote/test_worktree.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.687013 craft_application-2.6/tests/unit/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3946 2024-04-16 16:52:34.000000 craft_application-2.6/tests/unit/services/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    21815 2024-04-24 18:21:50.000000 craft_application-2.6/tests/unit/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft_application-2.6/tests/unit/services/test_package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft_application-2.6/tests/unit/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11829 2024-04-16 16:52:34.000000 craft_application-2.6/tests/unit/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3867 2024-04-24 18:21:50.000000 craft_application-2.6/tests/unit/services/test_repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-04-24 11:25:13.000000 craft_application-2.6/tests/unit/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    54323 2024-04-24 18:21:50.000000 craft_application-2.6/tests/unit/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-04-22 14:18:58.000000 craft_application-2.6/tests/unit/test_grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/test_nothing.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft_application-2.6/tests/unit/test_secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.687013 craft_application-2.6/tests/unit/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.687013 craft_application-2.6/tests/unit/util/invalid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/invalid_yaml/_README
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft_application-2.6/tests/unit/util/test_error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft_application-2.6/tests/unit/util/test_logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft_application-2.6/tests/unit/util/test_paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft_application-2.6/tests/unit/util/test_snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft_application-2.6/tests/unit/util/test_string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft_application-2.6/tests/unit/util/test_yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-24 18:24:07.687013 craft_application-2.6/tests/unit/util/valid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.6/tests/unit/util/valid_yaml/empty.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-04-16 16:52:04.000000 craft_application-2.6/tox.ini
```

### Comparing `craft_application-2.5/.editorconfig` & `craft_application-2.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/.jira_sync_config.yaml` & `craft_application-2.6/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/ISSUE_TEMPLATE/bug.yaml` & `craft_application-2.6/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/ISSUE_TEMPLATE/task.yaml` & `craft_application-2.6/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/renovate.json5` & `craft_application-2.6/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/workflows/docs.yaml` & `craft_application-2.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.github/workflows/tests.yaml` & `craft_application-2.6/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.gitignore` & `craft_application-2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/.pre-commit-config.yaml` & `craft_application-2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/HACKING.rst` & `craft_application-2.6/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/LICENSE` & `craft_application-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/PKG-INFO` & `craft_application-2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.5.0
+Version: 2.6.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft_application-2.5/README.rst` & `craft_application-2.6/README.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/__init__.py` & `craft_application-2.6/craft_application/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/application.py` & `craft_application-2.6/craft_application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,14 +579,20 @@
         # Perform variable expansion.
         self._expand_environment(yaml_data)
 
         # Handle build secrets.
         if self.app.features.build_secrets:
             self._render_secrets(yaml_data)
 
+        # apply application-specific transformations before expanding grammar
+        # because an application may add advanced grammar to the yaml
+        yaml_data = self._extra_yaml_transform(
+            yaml_data, build_on=build_on, build_for=build_for
+        )
+
         # Expand grammar.
         if "parts" in yaml_data:
             if not build_for:
                 # At the moment there is no perfect solution for what do to do
                 # resolve the grammar if there's no explicitly-provided target
                 # arch. However, we must resolve it with *something* otherwise
                 # we might have an invalid parts definition full of grammar
@@ -601,18 +607,15 @@
             craft_cli.emit.debug(f"Processing grammar (on {build_on} for {build_for})")
             yaml_data["parts"] = grammar.process_parts(
                 parts_yaml_data=yaml_data["parts"],
                 arch=build_on,
                 target_arch=build_for,
             )
 
-        # Perform extra, application-specific transformations.
-        return self._extra_yaml_transform(
-            yaml_data, build_on=build_on, build_for=build_for
-        )
+        return yaml_data
 
     def _expand_environment(self, yaml_data: dict[str, Any]) -> None:
         """Perform expansion of project environment variables."""
         environment_vars = self._get_project_vars(yaml_data)
         project_dirs = craft_parts.ProjectDirs(
             work_dir=self._work_dir, partitions=self._partitions
         )
```

### Comparing `craft_application-2.5/craft_application/commands/__init__.py` & `craft_application-2.6/craft_application/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/commands/base.py` & `craft_application-2.6/craft_application/commands/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/commands/lifecycle.py` & `craft_application-2.6/craft_application/commands/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/commands/other.py` & `craft_application-2.6/craft_application/commands/other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/errors.py` & `craft_application-2.6/craft_application/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/grammar.py` & `craft_application-2.6/craft_application/grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/__init__.py` & `craft_application-2.6/craft_application/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/errors.py` & `craft_application-2.6/craft_application/launchpad/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/launchpad.py` & `craft_application-2.6/craft_application/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/__init__.py` & `craft_application-2.6/craft_application/launchpad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/base.py` & `craft_application-2.6/craft_application/launchpad/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/build.py` & `craft_application-2.6/craft_application/launchpad/models/build.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/code.py` & `craft_application-2.6/craft_application/launchpad/models/code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/distro.py` & `craft_application-2.6/craft_application/launchpad/models/distro.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/project.py` & `craft_application-2.6/craft_application/launchpad/models/project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/models/recipe.py` & `craft_application-2.6/craft_application/launchpad/models/recipe.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/launchpad/util.py` & `craft_application-2.6/craft_application/launchpad/util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/misc/instance_bashrc` & `craft_application-2.6/craft_application/misc/instance_bashrc`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/__init__.py` & `craft_application-2.6/craft_application/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/base.py` & `craft_application-2.6/craft_application/models/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/constraints.py` & `craft_application-2.6/craft_application/models/constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/grammar.py` & `craft_application-2.6/craft_application/models/grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/metadata.py` & `craft_application-2.6/craft_application/models/metadata.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/models/project.py` & `craft_application-2.6/craft_application/models/project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/remote/__init__.py` & `craft_application-2.6/craft_application/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/remote/errors.py` & `craft_application-2.6/craft_application/remote/errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/remote/git.py` & `craft_application-2.6/craft_application/remote/git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/remote/utils.py` & `craft_application-2.6/craft_application/remote/utils.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/remote/worktree.py` & `craft_application-2.6/craft_application/remote/worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/secrets.py` & `craft_application-2.6/craft_application/secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/__init__.py` & `craft_application-2.6/craft_application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/base.py` & `craft_application-2.6/craft_application/services/base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/lifecycle.py` & `craft_application-2.6/craft_application/services/lifecycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,17 @@
         # Now that we are actually going to run we can validate what we're building.
         _validate_build_plan(self._build_plan)
 
         try:
             if self._project.package_repositories:
                 emit.trace("Installing package repositories")
                 repositories.install_package_repositories(
-                    self._project.package_repositories, self._lcm
+                    self._project.package_repositories,
+                    self._lcm,
+                    local_keys_path=self._get_local_keys_path(),
                 )
                 with contextlib.suppress(CallbackRegistrationError):
                     callbacks.register_configure_overlay(
                         repositories.install_overlay_repositories
                     )
             if target_step:
                 emit.trace(f"Planning {step_name} for {part_names or 'all parts'}")
@@ -392,14 +394,22 @@
                 emit.debug(
                     f"Using parallel build count of {parallel_build_count} "
                     "from CPU count"
                 )
 
         return parallel_build_count
 
+    def _get_local_keys_path(self) -> Path | None:
+        """Return a directory with public keys for package-repositories.
+
+        This default implementation does not support local keys; it should be
+        overridden by subclasses that do.
+        """
+        return None
+
 
 def _validate_build_plan(build_plan: list[models.BuildInfo]) -> None:
     """Check that the build plan has exactly 1 compatible build info."""
     if not build_plan:
         raise errors.EmptyBuildPlanError
 
     if len(build_plan) > 1:
```

### Comparing `craft_application-2.5/craft_application/services/package.py` & `craft_application-2.6/craft_application/services/package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/provider.py` & `craft_application-2.6/craft_application/services/provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/remotebuild.py` & `craft_application-2.6/craft_application/services/remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/request.py` & `craft_application-2.6/craft_application/services/request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/services/service_factory.py` & `craft_application-2.6/craft_application/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/__init__.py` & `craft_application-2.6/craft_application/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/callbacks.py` & `craft_application-2.6/craft_application/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/error_formatting.py` & `craft_application-2.6/craft_application/util/error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/logging.py` & `craft_application-2.6/craft_application/util/logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/paths.py` & `craft_application-2.6/craft_application/util/paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/platforms.py` & `craft_application-2.6/craft_application/util/platforms.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/repositories.py` & `craft_application-2.6/craft_application/util/repositories.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,23 +26,33 @@
     ProjectInfo,
 )
 
 
 def install_package_repositories(
     package_repositories: list[dict[str, Any]] | None,
     lifecycle_manager: LifecycleManager,
+    local_keys_path: Path | None = None,
 ) -> None:
-    """Install package repositories in the environment."""
+    """Install package repositories in the environment.
+
+    :param package_repositories: The definition of the repositories.
+    :param lifecycle_manager: The lifecycle manager whose packages will be
+      refreshed if repositories are installed.
+    :param local_keys_path: The optional local directory containing public
+      keys (for repositories that don't use the keyserver).
+    """
     from craft_archives import repo  # type: ignore[import-untyped]
 
     if not package_repositories:
         emit.debug("No package repositories specified, none to install.")
         return
 
-    refresh_required = repo.install(package_repositories, key_assets=Path("/dev/null"))
+    key_assets = local_keys_path if local_keys_path else Path("/dev/null")
+
+    refresh_required = repo.install(package_repositories, key_assets=key_assets)
     if refresh_required:
         emit.progress("Refreshing repositories")
         lifecycle_manager.refresh_packages_list()
 
     emit.progress("Package repositories installed")
```

### Comparing `craft_application-2.5/craft_application/util/snap_config.py` & `craft_application-2.6/craft_application/util/snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/string.py` & `craft_application-2.6/craft_application/util/string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application/util/yaml.py` & `craft_application-2.6/craft_application/util/yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application.egg-info/PKG-INFO` & `craft_application-2.6/craft_application.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.5.0
+Version: 2.6.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft_application-2.5/craft_application.egg-info/SOURCES.txt` & `craft_application-2.6/craft_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/craft_application.egg-info/requires.txt` & `craft_application-2.6/craft_application.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/docs/conf.py` & `craft_application-2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/docs/index.rst` & `craft_application-2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/pyproject.toml` & `craft_application-2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/conftest.py` & `craft_application-2.6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,25 +253,26 @@
 def fake_lifecycle_service_class(tmp_path, fake_build_plan):
     class FakeLifecycleService(services.LifecycleService):
         def __init__(
             self,
             app: application.AppMetadata,
             project: models.Project,
             services: services.ServiceFactory,
-            **lifecycle_kwargs: Any,
+            **kwargs: Any,
         ):
+            kwargs.pop("build_plan", None)  # We'll use ours
             super().__init__(
                 app,
                 services,
                 project=project,
-                work_dir=tmp_path / "work",
-                cache_dir=tmp_path / "cache",
+                work_dir=kwargs.pop("work_dir", tmp_path / "work"),
+                cache_dir=kwargs.pop("cache_dir", tmp_path / "cache"),
                 platform=None,
                 build_plan=fake_build_plan,
-                **lifecycle_kwargs,
+                **kwargs,
             )
 
     return FakeLifecycleService
 
 
 @pytest.fixture()
 def fake_services(
```

### Comparing `craft_application-2.5/tests/integration/conftest.py` & `craft_application-2.6/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/launchpad/conftest.py` & `craft_application-2.6/tests/integration/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/launchpad/test_anonymous_access.py` & `craft_application-2.6/tests/integration/launchpad/test_anonymous_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 @pytest.mark.parametrize(
     ("name", "owner", "project"),
     [
         ("python-apt", "deity", "python-apt"),
         ("charmcraft", "charmcraft-team", "charmcraft"),
-        ("snapcraft", "sergiusens", "snapcraft"),
+        ("snapcraft", "canonical-starcraft", "snapcraft"),
     ],
 )
 def test_get_real_repository_by_name(anonymous_lp, name, owner, project):
     repo = anonymous_lp.get_repository(name=name, owner=owner, project=project)
 
     assert repo.name == name
     assert repo.owner_name == owner
```

### Comparing `craft_application-2.5/tests/integration/services/test_lifecycle.py` & `craft_application-2.6/tests/integration/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/services/test_provider.py` & `craft_application-2.6/tests/integration/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/services/test_remotebuild.py` & `craft_application-2.6/tests/integration/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/services/test_request.py` & `craft_application-2.6/tests/integration/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/services/test_service_factory.py` & `craft_application-2.6/tests/integration/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/test_application.py` & `craft_application-2.6/tests/integration/test_application.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/integration/test_version.py` & `craft_application-2.6/tests/integration/test_version.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/commands/test_base.py` & `craft_application-2.6/tests/unit/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/commands/test_lifecycle.py` & `craft_application-2.6/tests/unit/commands/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/commands/test_other.py` & `craft_application-2.6/tests/unit/commands/test_other.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/conftest.py` & `craft_application-2.6/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/launchpad/conftest.py` & `craft_application-2.6/tests/unit/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/launchpad/models/test_base.py` & `craft_application-2.6/tests/unit/launchpad/models/test_base.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/launchpad/models/test_code.py` & `craft_application-2.6/tests/unit/launchpad/models/test_code.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/launchpad/test_launchpad.py` & `craft_application-2.6/tests/unit/launchpad/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/launchpad/test_util.py` & `craft_application-2.6/tests/unit/launchpad/test_util.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/models/test_constraints.py` & `craft_application-2.6/tests/unit/models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/models/test_project.py` & `craft_application-2.6/tests/unit/models/test_project.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/remote/conftest.py` & `craft_application-2.6/tests/unit/remote/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/remote/test_errors.py` & `craft_application-2.6/tests/unit/remote/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/remote/test_git.py` & `craft_application-2.6/tests/unit/remote/test_git.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/remote/test_utils.py` & `craft_application-2.6/tests/unit/remote/test_utils.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/remote/test_worktree.py` & `craft_application-2.6/tests/unit/remote/test_worktree.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/conftest.py` & `craft_application-2.6/tests/unit/services/conftest.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/test_lifecycle.py` & `craft_application-2.6/tests/unit/services/test_lifecycle.py`

 * *Files 4% similar despite different names*

```diff
@@ -459,16 +459,26 @@
         fake_parts_lifecycle.post_prime(step_info)
 
 
 # endregion
 # region Feature package repositories tests
 
 
+@pytest.mark.parametrize(
+    "local_keys_path",
+    [None, Path("my/keys")],
+)
 def test_lifecycle_package_repositories(
-    app_metadata, fake_project, fake_services, tmp_path, mocker, fake_build_plan
+    app_metadata,
+    fake_project,
+    fake_services,
+    tmp_path,
+    mocker,
+    fake_build_plan,
+    local_keys_path,
 ):
     """Test that package repositories installation is called in the lifecycle."""
     fake_repositories = [{"type": "apt", "ppa": "ppa/ppa"}]
     fake_project.package_repositories = fake_repositories.copy()
     work_dir = tmp_path / "work"
 
     service = lifecycle.LifecycleService(
@@ -476,14 +486,16 @@
         fake_services,
         project=fake_project,
         work_dir=work_dir,
         cache_dir=tmp_path / "cache",
         platform=None,
         build_plan=fake_build_plan,
     )
+    mocker.patch.object(service, "_get_local_keys_path", return_value=local_keys_path)
+
     service._lcm = mock.MagicMock(spec=LifecycleManager)
     service._lcm.project_info = mock.MagicMock(spec=ProjectInfo)
     service._lcm.project_info.get_project_var = lambda _: "foo"
 
     # Installation of repositories in the build instance
     mock_install = mocker.patch(
         "craft_application.util.repositories.install_package_repositories"
@@ -491,15 +503,17 @@
     # Installation of repositories in overlays
     mock_callback = mocker.patch.object(
         craft_parts.callbacks, "register_configure_overlay"
     )
 
     service.run("prime")
 
-    mock_install.assert_called_once_with(fake_repositories, service._lcm)
+    mock_install.assert_called_once_with(
+        fake_repositories, service._lcm, local_keys_path=local_keys_path
+    )
     mock_callback.assert_called_once_with(repositories.install_overlay_repositories)
 
 
 # endregion
 
 # region parallel build count tests
```

### Comparing `craft_application-2.5/tests/unit/services/test_package.py` & `craft_application-2.6/tests/unit/services/test_package.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/test_provider.py` & `craft_application-2.6/tests/unit/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/test_remotebuild.py` & `craft_application-2.6/tests/unit/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/test_repositories.py` & `craft_application-2.6/tests/unit/services/test_repositories.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,28 +14,35 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Tests for PackageService."""
 from __future__ import annotations
 
 from pathlib import Path
 
+import pytest
 from craft_application.util import repositories
 
 
-def test_repo_install_package_repositories(emitter, mocker, lifecycle_service):
+@pytest.mark.parametrize(
+    ("local_keys_path", "expected_key_assets"),
+    [(None, Path("/dev/null")), (Path("my/keys"), Path("my/keys"))],
+)
+def test_repo_install_package_repositories(
+    emitter, mocker, lifecycle_service, local_keys_path, expected_key_assets
+):
     package_repositories = [{"type": "apt", "ppa": "ppa/ppa"}]
 
     repo_install = mocker.patch("craft_archives.repo.install", return_value=False)
 
     repositories.install_package_repositories(
-        package_repositories, lifecycle_service._lcm
+        package_repositories, lifecycle_service._lcm, local_keys_path=local_keys_path
     )
 
     repo_install.assert_called_once_with(
-        package_repositories, key_assets=Path("/dev/null")
+        package_repositories, key_assets=expected_key_assets
     )
 
     emitter.assert_progress("Package repositories installed")
 
 
 def test_repo_install_package_repositories_empty(emitter, mocker, lifecycle_service):
     package_repositories = None
```

### Comparing `craft_application-2.5/tests/unit/services/test_request.py` & `craft_application-2.6/tests/unit/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/services/test_service_factory.py` & `craft_application-2.6/tests/unit/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/test_application.py` & `craft_application-2.6/tests/unit/test_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # SATISFACTORY QUALITY, or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Unit tests for craft-application app classes."""
 import argparse
+import copy
 import dataclasses
 import importlib
 import importlib.metadata
 import logging
 import pathlib
 import re
 import subprocess
@@ -1463,14 +1464,52 @@
     """Test that if the build plan is empty, the grammar uses the host as target arch."""
     mocker.patch("craft_application.util.get_host_architecture", return_value="i386")
     project = grammar_app_mini.get_project()
     # "source" is empty because "i386" doesn't match any of the grammar statements.
     assert project.parts["mypart"]["source"] is None
 
 
+class FakeApplicationWithYamlTransform(FakeApplication):
+    """Application class that adds advanced grammar in `_extra_yaml_transform`."""
+
+    @override
+    def _extra_yaml_transform(
+        self,
+        yaml_data: dict[str, Any],
+        *,
+        build_on: str,  # noqa: ARG002 (Unused method argument)
+        build_for: str | None,  # noqa: ARG002 (Unused method argument)
+    ) -> dict[str, Any]:
+        # do not modify the dict passed in
+        new_yaml_data = copy.deepcopy(yaml_data)
+        new_yaml_data["parts"] = {
+            "mypart": {
+                "plugin": "nil",
+                "source": [
+                    {"to riscv64": "to-riscv64"},
+                    {"to s390x": "to-s390x"},
+                ],
+            }
+        }
+
+        return new_yaml_data
+
+
+def test_process_grammar_from_extra_transform(app_metadata, fake_services, tmp_path):
+    """Test that grammar is applied on data from `_extra_yaml_transform`."""
+    project_file = tmp_path / "testcraft.yaml"
+    project_file.write_text(BASIC_PROJECT_YAML)
+
+    app = FakeApplicationWithYamlTransform(app_metadata, fake_services)
+    app.project_dir = tmp_path
+
+    project = app.get_project(build_for="riscv64")
+    assert project.parts["mypart"]["source"] == "to-riscv64"
+
+
 class FakePartitionsApplication(FakeApplication):
     """A partition using FakeApplication."""
 
     @override
     def _setup_partitions(self, yaml_data) -> list[str]:
         _ = yaml_data
         return ["default", "mypartition"]
```

### Comparing `craft_application-2.5/tests/unit/test_errors.py` & `craft_application-2.6/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/test_grammar.py` & `craft_application-2.6/tests/unit/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/test_secrets.py` & `craft_application-2.6/tests/unit/test_secrets.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_error_formatting.py` & `craft_application-2.6/tests/unit/util/test_error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_logging.py` & `craft_application-2.6/tests/unit/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_paths.py` & `craft_application-2.6/tests/unit/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_snap_config.py` & `craft_application-2.6/tests/unit/util/test_snap_config.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_string.py` & `craft_application-2.6/tests/unit/util/test_string.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tests/unit/util/test_yaml.py` & `craft_application-2.6/tests/unit/util/test_yaml.py`

 * *Files identical despite different names*

### Comparing `craft_application-2.5/tox.ini` & `craft_application-2.6/tox.ini`

 * *Files identical despite different names*

