# Comparing `tmp/OZI-1.1.3.tar.gz` & `tmp/OZI-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.1.3.tar", last modified: Wed Apr 24 03:48:38 2024, max compression
+gzip compressed data, was "OZI-1.1.4.tar", last modified: Wed Apr 24 04:23:45 2024, max compression
```

## Comparing `OZI-1.1.3.tar` & `OZI-1.1.4.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:48:38.393778 OZI-1.1.3/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-24 03:42:47.000000 OZI-1.1.3/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-24 03:42:47.000000 OZI-1.1.3/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   282754 2024-04-24 03:42:47.000000 OZI-1.1.3/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-24 03:42:47.000000 OZI-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-24 03:48:38.393778 OZI-1.1.3/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-24 03:42:47.000000 OZI-1.1.3/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-24 03:42:47.000000 OZI-1.1.3/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-24 03:42:47.000000 OZI-1.1.3/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/dist/sigstore/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     3368 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/filter.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6265 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6193 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/.gitignore.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/CHANGELOG.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      487 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/LICENSE.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/PKG-INFO.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      763 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/README.rst.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/bandit.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/bandit.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/black.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/black.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/coverage.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/doc8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/doc8.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/flake8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      577 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/flake8.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/checkpoint.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/generate_provenance.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      747 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/publish.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/github_workflows/release.yml.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/gitlab_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/gitlab_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      494 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/isort.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/isort.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/cc-by-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/wtfpl.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/DFSG_approved/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/
--rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/
--rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apache_Software_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apache_Software_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/
--rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Artistic_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Artistic_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      590 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_License/mit.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      610 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/PostgreSQL_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/PostgreSQL_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1784 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/zlib_libpng_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Public_Domain/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Public_Domain/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Public_Domain/licenseref-public-domain.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Public_Domain/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/Public_Domain/unlicense.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/agpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/gfdl-1.3.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/gpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/gpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/lgpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/lgpl-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/lgpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1106 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/license/zlib.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      563 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/meson.options.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      313 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/mypy.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/mypy.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1296 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/new_child.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     2648 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.array.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.feature.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      689 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.integer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/__init__.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/__init__.pyi.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/new_module.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.name/py.typed.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/project.ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      396 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pydocstyle.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pylint.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pyproject.toml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pyright.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      390 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pyright.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      525 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pytest.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/pytest.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/requirements.in.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/restructuredtext-lint.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/root.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1271 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/ruff.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1269 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/semantic_release.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      486 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/setuptools_scm.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/tests/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/tests/new_test.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/templates/tox.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-24 03:42:47.000000 OZI-1.1.3/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10639 2024-04-24 03:42:47.000000 OZI-1.1.3/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-24 03:42:47.000000 OZI-1.1.3/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-24 03:42:47.000000 OZI-1.1.3/subprojects/blastpipe.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-24 03:42:47.000000 OZI-1.1.3/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 03:42:47.000000 OZI-1.1.3/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-24 03:42:47.000000 OZI-1.1.3/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11040 2024-04-24 03:42:47.000000 OZI-1.1.3/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    13823 2024-04-24 03:42:47.000000 OZI-1.1.3/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-24 03:42:47.000000 OZI-1.1.3/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:23:45.262110 OZI-1.1.4/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     5873 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3544 2024-04-24 04:18:05.000000 OZI-1.1.4/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-04-24 04:18:05.000000 OZI-1.1.4/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   282988 2024-04-24 04:18:05.000000 OZI-1.1.4/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-04-24 04:18:05.000000 OZI-1.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-24 04:23:45.262110 OZI-1.1.4/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-04-24 04:18:05.000000 OZI-1.1.4/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16576 2024-04-24 04:18:05.000000 OZI-1.1.4/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-04-24 04:18:05.000000 OZI-1.1.4/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      400 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/dist/sigstore/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     3368 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/filter.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2367 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6265 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3612 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7877 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      842 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4731 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6436 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6193 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2044 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1687 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6070 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4445 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6347 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      487 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      257 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      763 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      772 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      365 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      530 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      577 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1793 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      687 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      747 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      991 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1518 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      480 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      494 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      428 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      490 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      982 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      506 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      566 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      509 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      505 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      590 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      538 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      513 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      544 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      540 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      514 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      594 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      500 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      610 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      507 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1784 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      570 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1106 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1898 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      563 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1028 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      313 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      391 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1296 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      498 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2648 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      766 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      689 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3684 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      587 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      900 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      274 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      129 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      396 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      423 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      600 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      390 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      524 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      295 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1369 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1271 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1269 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      486 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      504 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      866 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1572 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/templates/tox.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-04-24 04:18:05.000000 OZI-1.1.4/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10639 2024-04-24 04:18:05.000000 OZI-1.1.4/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-04-24 04:18:05.000000 OZI-1.1.4/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (127)      342 2024-04-24 04:18:05.000000 OZI-1.1.4/subprojects/blastpipe.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-04-24 04:18:05.000000 OZI-1.1.4/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:18:05.000000 OZI-1.1.4/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-04-24 04:18:05.000000 OZI-1.1.4/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11040 2024-04-24 04:18:05.000000 OZI-1.1.4/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    13823 2024-04-24 04:18:05.000000 OZI-1.1.4/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-04-24 04:18:05.000000 OZI-1.1.4/tests/test_tap.py
```

### Comparing `OZI-1.1.3/.github/CODEOWNERS` & `OZI-1.1.4/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/CODE_OF_CONDUCT.md` & `OZI-1.1.4/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/CONTRIBUTING.md` & `OZI-1.1.4/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/SECURITY.md` & `OZI-1.1.4/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/workflows/codeql.yml` & `OZI-1.1.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/workflows/dependency-review.yml` & `OZI-1.1.4/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/workflows/dev-workflow.yml` & `OZI-1.1.4/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/workflows/dist-workflow.yml` & `OZI-1.1.4/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.github/workflows/scorecard.yml` & `OZI-1.1.4/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/.gitignore` & `OZI-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/CHANGELOG.md` & `OZI-1.1.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 # CHANGELOG
+## 1.1.4 (2024-04-24)
+
+### :bug:
+
+* :bug::hammer: Fix pytest-args for coverage.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`1193781`](https://github.com/OZI-Project/OZI/commit/119378168e8e56096e05751b170fcd29a23e676b))
+
 ## 1.1.3 (2024-04-24)
 
 ### :hammer:
 
 * :hammer: retry release
 
 Merge pull request #411 from OZI-Project/release/1.1 ([`5eef90b`](https://github.com/OZI-Project/OZI/commit/5eef90b471611999873de5fca990e687823c1246))
```

### Comparing `OZI-1.1.3/LICENSE.txt` & `OZI-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/PKG-INFO` & `OZI-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.1.3
+Version: 1.1.4
 Summary: Packager for Python projects using Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.1.3.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.1.4.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Rose Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.1.3/README.rst` & `OZI-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/meson.build` & `OZI-1.1.4/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/meson.options` & `OZI-1.1.4/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/__main__.py` & `OZI-1.1.4/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/actions.py` & `OZI-1.1.4/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/comment.py` & `OZI-1.1.4/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/filter.py` & `OZI-1.1.4/ozi/filter.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/__main__.py` & `OZI-1.1.4/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/build_definition.py` & `OZI-1.1.4/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/meson.build` & `OZI-1.1.4/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/missing.py` & `OZI-1.1.4/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/parser.py` & `OZI-1.1.4/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/fix/rewrite_command.py` & `OZI-1.1.4/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/lint/meson.build` & `OZI-1.1.4/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/lint/pyright/meson.build` & `OZI-1.1.4/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/meson.build` & `OZI-1.1.4/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/meson.py` & `OZI-1.1.4/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/new/__main__.py` & `OZI-1.1.4/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/new/meson.build` & `OZI-1.1.4/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/new/parser.py` & `OZI-1.1.4/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/new/validate.py` & `OZI-1.1.4/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/pkg_extra.py` & `OZI-1.1.4/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/render.py` & `OZI-1.1.4/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/core_metadata_template.py` & `OZI-1.1.4/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/meson.build` & `OZI-1.1.4/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.1.4/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.1.4/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/render_requirements.py` & `OZI-1.1.4/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.1.4/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/scm_version_snip.py` & `OZI-1.1.4/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/to_distribution_template.py` & `OZI-1.1.4/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/scripts/version_metadata_template.py` & `OZI-1.1.4/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spdx.py` & `OZI-1.1.4/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/_license.py` & `OZI-1.1.4/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/_spec.py` & `OZI-1.1.4/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/base.py` & `OZI-1.1.4/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/ci.py` & `OZI-1.1.4/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/meson.build` & `OZI-1.1.4/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/pkg.py` & `OZI-1.1.4/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/project.py` & `OZI-1.1.4/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/python.py` & `OZI-1.1.4/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/spec/src.py` & `OZI-1.1.4/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/tap.py` & `OZI-1.1.4/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/README.rst.j2` & `OZI-1.1.4/ozi/templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/coverage.pyproject.toml` & `OZI-1.1.4/ozi/templates/coverage.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/flake8.meson.options` & `OZI-1.1.4/ozi/templates/flake8.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/flake8.pyproject.toml` & `OZI-1.1.4/ozi/templates/flake8.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/checkpoint.yml.j2` & `OZI-1.1.4/ozi/templates/github_workflows/checkpoint.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/generate_provenance.yml.j2` & `OZI-1.1.4/ozi/templates/github_workflows/generate_provenance.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/meson.build` & `OZI-1.1.4/ozi/templates/github_workflows/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/ozi.yml.j2` & `OZI-1.1.4/ozi/templates/github_workflows/ozi.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/publish.yml.j2` & `OZI-1.1.4/ozi/templates/github_workflows/publish.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/github_workflows/release.yml.j2` & `OZI-1.1.4/ozi/templates/github_workflows/release.yml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/DFSG_approved/cc-by-4.0.txt` & `OZI-1.1.4/ozi/templates/license/DFSG_approved/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt` & `OZI-1.1.4/ozi/templates/license/DFSG_approved/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/DFSG_approved/meson.build` & `OZI-1.1.4/ozi/templates/license/DFSG_approved/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt` & `OZI-1.1.4/ozi/templates/license/Free_To_Use_But_Restricted/ncsa.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Apple_Public_Source_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/0bsd.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/BSD_License/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/BSD_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build` & `OZI-1.1.4/ozi/templates/license/OSI_Approved/zlib_libpng_License/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/Public_Domain/meson.build` & `OZI-1.1.4/ozi/templates/license/Public_Domain/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/Public_Domain/unlicense.txt` & `OZI-1.1.4/ozi/templates/license/Public_Domain/unlicense.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/agpl-3.0.txt` & `OZI-1.1.4/ozi/templates/license/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/apache-2.0.txt` & `OZI-1.1.4/ozi/templates/license/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/artistic-2.0.txt` & `OZI-1.1.4/ozi/templates/license/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/bsd-3-clause.txt` & `OZI-1.1.4/ozi/templates/license/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/cc0-1.0.txt` & `OZI-1.1.4/ozi/templates/license/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/epl-1.0.txt` & `OZI-1.1.4/ozi/templates/license/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/gfdl-1.3.txt` & `OZI-1.1.4/ozi/templates/license/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/gpl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/gpl-3.0.txt` & `OZI-1.1.4/ozi/templates/license/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/isc.txt` & `OZI-1.1.4/ozi/templates/license/isc.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/lgpl-2.0.txt` & `OZI-1.1.4/ozi/templates/license/lgpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/lgpl-2.1.txt` & `OZI-1.1.4/ozi/templates/license/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/lgpl-3.0.txt` & `OZI-1.1.4/ozi/templates/license/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/meson.build` & `OZI-1.1.4/ozi/templates/license/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/mit.txt` & `OZI-1.1.4/ozi/templates/license/mit.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/license/zlib.txt` & `OZI-1.1.4/ozi/templates/license/zlib.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/meson.build` & `OZI-1.1.4/ozi/templates/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/meson.build.j2` & `OZI-1.1.4/ozi/templates/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/meson.options.j2` & `OZI-1.1.4/ozi/templates/meson.options.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/new_child.j2` & `OZI-1.1.4/ozi/templates/new_child.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.PKG-INFO` & `OZI-1.1.4/ozi/templates/project.PKG-INFO`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.array.meson.options` & `OZI-1.1.4/ozi/templates/project.array.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.feature.meson.options` & `OZI-1.1.4/ozi/templates/project.feature.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.integer.meson.options` & `OZI-1.1.4/ozi/templates/project.integer.meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.meson.build` & `OZI-1.1.4/ozi/templates/project.meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.name/meson.build` & `OZI-1.1.4/ozi/templates/project.name/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/project.name/meson.build.j2` & `OZI-1.1.4/ozi/templates/project.name/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/pyproject.toml.j2` & `OZI-1.1.4/ozi/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/pytest.meson.options` & `OZI-1.1.4/ozi/templates/pytest.meson.options`

 * *Files 4% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     description: 'application',
     type: 'array',
     value: [
         '@build_root@/test',
         '--basetemp=temp',
         '--exitfirst',
         '--cov-config=pyproject.toml',
-        '@opt_cov_eq_project_name@',
+        '--cov={{ project.name }}',
         '-n',
         'auto',
         '-d',
     ]
 )
```

### Comparing `OZI-1.1.3/ozi/templates/pytest.pyproject.toml` & `OZI-1.1.4/ozi/templates/pytest.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/root.pyproject.toml` & `OZI-1.1.4/ozi/templates/root.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/ruff.pyproject.toml` & `OZI-1.1.4/ozi/templates/ruff.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/semantic_release.pyproject.toml` & `OZI-1.1.4/ozi/templates/semantic_release.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/tests/meson.build.j2` & `OZI-1.1.4/ozi/templates/tests/meson.build.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/templates/tox.pyproject.toml` & `OZI-1.1.4/ozi/templates/tox.pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/trove.py` & `OZI-1.1.4/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/__init__.py` & `OZI-1.1.4/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/__main__.py` & `OZI-1.1.4/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/deliverability.py` & `OZI-1.1.4/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.1.4/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/meson.build` & `OZI-1.1.4/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.1.4/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/syntax.py` & `OZI-1.1.4/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/email_validator/validate_email.py` & `OZI-1.1.4/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/ozi/vendor/meson.build` & `OZI-1.1.4/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/pyproject.toml` & `OZI-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/templates/CHANGELOG.md.j2` & `OZI-1.1.4/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/tests/meson.build` & `OZI-1.1.4/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/tests/test_ozi_fix.py` & `OZI-1.1.4/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/tests/test_ozi_new.py` & `OZI-1.1.4/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.1.3/tests/test_tap.py` & `OZI-1.1.4/tests/test_tap.py`

 * *Files identical despite different names*

