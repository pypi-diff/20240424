# Comparing `tmp/nrp-devtools-0.1.8.tar.gz` & `tmp/nrp-devtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrp-devtools-0.1.8.tar", last modified: Thu Jan 18 08:19:26 2024, max compression
+gzip compressed data, was "nrp-devtools-0.1.9.tar", last modified: Thu Jan 18 21:22:35 2024, max compression
```

## Comparing `nrp-devtools-0.1.8.tar` & `nrp-devtools-0.1.9.tar`

### file list

```diff
@@ -1,163 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.321182 nrp-devtools-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-01-18 08:19:26.321182 nrp-devtools-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 08:19:26.321182 nrp-devtools-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.293182 nrp-devtools-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.301182 nrp-devtools-0.1.8/src/nrp_devtools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.301182 nrp-devtools-0.1.8/src/nrp_devtools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/develop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.305182 nrp-devtools-0.1.8/src/nrp_devtools/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/check_old.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.305182 nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/invenio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.305182 nrp-devtools-0.1.8/src/nrp_devtools/commands/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/model/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/model/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/pdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/less.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/link_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/commands/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/config/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/repository_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/config/wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/component.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/Dockerfile.production
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.309182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.293182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/en/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/en/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/translations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/webpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/invenio.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2222 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/nrp
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/site.overrides
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/site.variables
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.config
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/base/page.html
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/js/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/js/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/components/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/components/custom-components.less
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.313182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/TitlePage.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositForm.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositValidationSchema.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/EmptyResultsElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/MultipleSearchBarElement.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsGridItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.297182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Deposit.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Detail.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Search.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/templates/{{cookiecutter.template_name}}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/src/nrp_devtools/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.321182 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 08:19:26.000000 nrp-devtools-0.1.8/src/nrp_devtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 08:19:26.317182 nrp-devtools-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-18 08:19:20.000000 nrp-devtools-0.1.8/tests/test_repository_from_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.302800 nrp-devtools-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-18 21:22:35.302800 nrp-devtools-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 21:22:35.302800 nrp-devtools-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.274800 nrp-devtools-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.286800 nrp-devtools-0.1.9/src/nrp_devtools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/develop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.286800 nrp-devtools-0.1.9/src/nrp_devtools/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/check_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/invenio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/commands/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/model/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/model/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/pdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/less.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/link_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/commands/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/i18n_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/repository_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/config/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/component.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.290800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/Dockerfile.production
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.278800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/translations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/invenio.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2222 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/nrp
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.shared_package}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.278800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/site.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/globals/site.variables
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.278800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/templates/base/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.278800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.294800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/js/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.278800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/semantic-ui/less/components/custom-components.less
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/components/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/TitlePage.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositForm.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositValidationSchema.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/EmptyResultsElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/MultipleSearchBarElement.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsGridItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.282800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Deposit.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Detail.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/templates/semantic-ui/{{cookiecutter.name}}/Search.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/templates/{{cookiecutter.template_name}}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/src/nrp_devtools/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 21:22:35.000000 nrp-devtools-0.1.9/src/nrp_devtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 21:22:35.298800 nrp-devtools-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-18 21:22:24.000000 nrp-devtools-0.1.9/tests/test_repository_from_scratch.py
```

### Comparing `nrp-devtools-0.1.8/PKG-INFO` & `nrp-devtools-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-devtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: NRP repository development tools
 Author-email: Miroslav Simek <miroslav.simek@cesnet.cz>
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: pip
 Requires-Dist: wheel
 Requires-Dist: click
@@ -26,14 +26,15 @@
 Requires-Dist: oarepo-tools
 Requires-Dist: minio
 Requires-Dist: redis
 Requires-Dist: psycopg[binary]
 Requires-Dist: pika
 Requires-Dist: opensearch-py
 Requires-Dist: pytest
+Requires-Dist: oarepo-tools
 
 # NRP repository development tools
 
 This tool is used to setup and run an Invenio based NRP instance. 
 
 ## Prerequisites
```

### Comparing `nrp-devtools-0.1.8/README.md` & `nrp-devtools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/pyproject.toml` & `nrp-devtools-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nrp-devtools"
-version = "0.1.8"
+version = "0.1.9"
 description = "NRP repository development tools"
 readme = "README.md"
 authors = [
   {name = "Miroslav Simek", email = "miroslav.simek@cesnet.cz" }
 ]
 dependencies = [
   "setuptools",
@@ -45,14 +45,17 @@
   "redis",
   "psycopg[binary]",
   "pika",
   "opensearch-py",
 
   # testing
   "pytest",
+
+  # i18n
+  "oarepo-tools"
 ]
 
 [project.scripts]
 nrp-devtools = "nrp_devtools.main:nrp_command"
 
 
 [build-system]
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/base.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/base.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/build.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 @nrp_command.command(name="build")
 @command_sequence()
 def build_command(*, config: OARepoConfig, **kwargs):
     """Builds the repository"""
     return build_command_internal(config=config, **kwargs)
 
+
 def build_command_internal(*, config: OARepoConfig, **kwargs):
     return (
         no_args(
             partial(click.secho, "Building repository for production", fg="yellow")
         ),
         make_step(clean_previous_installation),
         make_step(create_empty_venv),
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/check.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 from ..commands.check_old import check_imagemagick_callable
 from ..commands.db import check_db, fix_db
 from ..commands.docker import (
     check_containers,
     check_docker_callable,
     check_docker_compose_version,
+    check_docker_env,
     check_node_version,
     check_npm_version,
-    fix_containers, fix_docker_env, check_docker_env,
+    fix_containers,
+    fix_docker_env,
 )
 from ..commands.invenio import check_invenio_cfg, install_invenio_cfg
 from ..commands.opensearch import check_search, fix_custom_fields, fix_search
 from ..commands.pdm import (
     build_requirements,
     check_invenio_callable,
     check_requirements,
@@ -26,15 +28,14 @@
 from ..commands.s3 import (
     check_s3_bucket_exists,
     check_s3_location_in_database,
     fix_s3_bucket_exists,
     fix_s3_location_in_database,
 )
 from ..commands.ui import check_ui, fix_ui
-from ..commands.ui.assets import register_less_components
 from ..commands.utils import make_step, no_args, run_fixup
 from ..config import OARepoConfig
 from .base import command_sequence, nrp_command
 
 
 @nrp_command.command(name="check")
 @click.option("--fix", is_flag=True, default=False)
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/develop.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/develop.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/initialize.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/model.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import click
 
 from ..commands.model.compile import (
     add_requirements_and_entrypoints,
     compile_model_to_tempdir,
     copy_compiled_model,
     generate_alembic,
-    install_model_compiler,
+    install_model_compiler, add_model_to_i18n,
 )
 from ..commands.model.create import create_model
 from ..commands.pdm import install_python_repository
 from ..commands.utils import make_step
 from ..config import OARepoConfig, ask_for_configuration
 from ..config.model_config import ModelConfig
 from .base import command_sequence, nrp_command
@@ -58,8 +58,9 @@
     return (
         make_step(install_model_compiler, model=model),
         make_step(compile_model_to_tempdir, model=model, tempdir=tempdir),
         make_step(copy_compiled_model, model=model, tempdir=tempdir),
         make_step(add_requirements_and_entrypoints, model=model, tempdir=tempdir),
         make_step(install_python_repository),
         make_step(generate_alembic, model=model),
+        make_step(add_model_to_i18n, model=model),
     )
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/run.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from ..commands.develop import Runner
 from ..commands.develop.controller import run_develop_controller
 from ..commands.utils import make_step
 from ..config import OARepoConfig
 from .base import command_sequence, nrp_command
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/cli/ui.py` & `nrp-devtools-0.1.9/src/nrp_devtools/cli/ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 from pathlib import Path
 
 import click
-import cookiecutter
 
 from ..commands.ui.create import (
     create_model_ui,
     create_page_ui,
     register_model_ui,
     register_page_ui,
 )
-from ..commands.utils import make_step, run_cookiecutter, capitalize_name
+from ..commands.utils import capitalize_name, make_step
 from ..config import OARepoConfig
 from ..config.ui_config import UIConfig
 from .base import command_sequence, nrp_command
 
 
 @nrp_command.group(name="ui")
 def ui_group():
@@ -158,53 +157,68 @@
     help="""Create a new less component.  
 The component-type is the type of the component, such as element, view, module, or collection.
 The component-name is the name of the component, such as navbar or footer.
     """,
 )
 @click.argument("component-type")
 @click.argument("component-name")
-@click.option("--jinjax/--no-jinjax", default=True, help="Generate jinjax template as well")
+@click.option(
+    "--jinjax/--no-jinjax", default=True, help="Generate jinjax template as well"
+)
 @command_sequence()
-def create_less_component(config: OARepoConfig, component_type, component_name, jinjax, **kwargs):
+def create_less_component(
+    config: OARepoConfig, component_type, component_name, jinjax, **kwargs
+):
     ui_name = "components"
     # if the config.ui_dir/ui_name does not exist, run cookiecutter to create it
     ui_dir = config.ui_dir / ui_name
 
     def create_less_component(*args, **kwargs):
-
         # files and directories
         less_dir = ui_dir / "semantic-ui" / "less"
         definitions_dir = less_dir / ui_name / "definitions"
         default_theme_dir = less_dir / ui_name / "default"
         registration_less_file = less_dir / ui_name / "custom-components.less"
 
         component_type_plural = component_type + "s"
 
-        component_file = definitions_dir / component_type_plural / f"{component_name}.less"
-        component_variables_file = default_theme_dir / component_type_plural / f"{component_name}.variables"
-        component_overrides_file = default_theme_dir / component_type_plural / f"{component_name}.overrides"
+        component_file = (
+            definitions_dir / component_type_plural / f"{component_name}.less"
+        )
+        component_variables_file = (
+            default_theme_dir / component_type_plural / f"{component_name}.variables"
+        )
+        component_overrides_file = (
+            default_theme_dir / component_type_plural / f"{component_name}.overrides"
+        )
 
         # create variable and override files
         component_variables_file.parent.mkdir(parents=True, exist_ok=True)
         if not component_variables_file.exists():
-            component_variables_file.write_text(f"""
+            component_variables_file.write_text(
+                f"""
 /* https://github.com/Semantic-Org/example-github/blob/master/semantic/src/themes/default/globals/site.variables */
 /* @{component_name}Background: @inputBackground; */
-            """)
-        click.secho(f"Place variables that parametrize the component inside {component_variables_file}",
-                    fg="green")
+            """
+            )
+        click.secho(
+            f"Place variables that parametrize the component inside {component_variables_file}",
+            fg="green",
+        )
 
         component_overrides_file.parent.mkdir(parents=True, exist_ok=True)
         if not component_overrides_file.exists():
             component_overrides_file.touch()
 
         # create the component
-        less_data = (Path(__file__).parent.parent / "templates" / "component.less").read_text()
-        less_data = less_data.replace('{{component_type}}', component_type)
-        less_data = less_data.replace('{{component_name}}', component_name)
+        less_data = (
+            Path(__file__).parent.parent / "templates" / "component.less"
+        ).read_text()
+        less_data = less_data.replace("{{component_type}}", component_type)
+        less_data = less_data.replace("{{component_name}}", component_name)
 
         component_file.parent.mkdir(parents=True, exist_ok=True)
         if not component_file.exists():
             component_file.write_text(less_data)
         click.secho(f"Put the default css to {component_file}", fg="green")
 
         # add the component to the registration file
@@ -212,27 +226,31 @@
         registration_less_data += f'\n& {{\n @import "@less/{ui_name}/definitions/{component_type_plural}/{component_name}"; \n}}'
         registration_less_file.write_text(registration_less_data)
 
     def create_jinjax_component(*args, **kwargs):
         if not jinjax:
             return
         component_name_capitalized = capitalize_name(component_name)
-        jinjax_component_file = ui_dir / "templates" / ui_name / f"{component_name_capitalized}.jinja"
+        jinjax_component_file = (
+            ui_dir / "templates" / ui_name / f"{component_name_capitalized}.jinja"
+        )
 
         jinjax_component_file.parent.mkdir(parents=True, exist_ok=True)
         if not jinjax_component_file.exists():
-            jinjax_component_file.write_text(f"""{{# def #}}
+            jinjax_component_file.write_text(
+                f"""{{# def #}}
     <div class="ui {component_name}">
       Overwrite this file with your own jinja template.
     </div>
-            """)
-        click.secho(f"Place the HTML code of the component to {jinjax_component_file} "
-                    f"and reference it from elsewhere as <components.{component_name_capitalized} /> or <{component_name_capitalized} />. "
-                    f"Do not forget to put css classes 'ui {component_name}' to the root element of the template.",
-                    fg="green")
+            """
+            )
+        click.secho(
+            f"Place the HTML code of the component to {jinjax_component_file} "
+            f"and reference it from elsewhere as <components.{component_name_capitalized} /> or <{component_name_capitalized} />. "
+            f"Do not forget to put css classes 'ui {component_name}' to the root element of the template.",
+            fg="green",
+        )
 
     return (
         create_less_component,
         create_jinjax_component,
     )
-
-
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/db.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/db.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/controller.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 from pytimedinput import timedInput
 
-from .runner import Runner
 from nrp_devtools.config import OARepoConfig
 
+from .runner import Runner
+
 
 def show_menu(server: bool, ui: bool, development_mode: bool):
     click.secho("")
     click.secho("")
     if development_mode:
         click.secho("Development server is running", fg="green")
     else:
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/develop/runner.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/develop/runner.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/docker.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 def check_docker_env(config: OARepoConfig, **kwargs):
     if not (config.repository_dir / "docker" / ".env").exists():
         check_failed(
             "Docker environment file is missing. Please run this command with --fix to fix the problem."
         )
 
+
 def fix_docker_env(config: OARepoConfig, **kwargs):
     (config.repository_dir / "docker" / ".env").symlink_to(
         config.repository_dir / "variables"
     )
 
 
 def check_docker_callable(config: OARepoConfig):
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/initialize.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/initialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,7 +28,14 @@
     # link the variables
     (config.repository_dir / "docker" / ".env").symlink_to(
         config.repository_dir / "variables"
     )
 
     # mark the nrp command executable
     (config.repository_dir / "nrp").chmod(0o755)
+
+    # set up the i18n
+    config.i18n.babel_source_paths = [
+        config.repository.shared_package,
+        config.repository.ui_package,
+    ]
+    config.i18n.i18next_source_paths = [config.repository.ui_package]
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/invenio.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/invenio.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/model/compile.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/model/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,7 +385,12 @@
         file_text = f.read()
         file_text = file_text.replace(
             f"revision = '{current_revision_id}'", f"revision = '{new_id}'"
         )
     with open(target_file.replace(current_revision_id, new_id), "w") as f:
         f.write(file_text)
     os.remove(target_file)
+
+
+def add_model_to_i18n(config: OARepoConfig, *, model, **kwargs):
+    i18n_config = config.i18n
+    i18n_config.babel_source_paths.append(model.model_package)
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/model/create.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/model/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,21 +68,21 @@
                     "en": {"text": {}},
                 },
             }
         )
 
     if model.base_model == BaseModel.data:
         extend = {
-            "extend": '"nr-data#DataModel"',
+            "extend": "nr-data#DataModel",
         }
         plugins.add("oarepo-model-builder-nr")
         runtime_dependencies["nr-metadata"] = "2.0.0"
     elif model.base_model == BaseModel.documents:
         extend = {
-            "extend": '"nr-documents#DocumentModel"',
+            "extend": "nr-documents#DocumentModel",
         }
         plugins.add("oarepo-model-builder-nr")
         runtime_dependencies["nr-metadata"] = "2.0.0"
     elif model.base_model == BaseModel.empty:
         extend = {}
     else:
         raise ValueError(f"Unknown base model: {model.base_model}")
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/opensearch.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/opensearch.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/pdm.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/pdm.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,26 +89,36 @@
         )
 
 
 def install_python_repository(config, **kwargs):
     run_pdm(config, "install", "--dev", "--no-lock")
 
     # fixup for uritemplate / uritemplate.py
-    run_cmdline(config.venv_dir / "bin" / "pip", "install", "-U",
-                "--force-reinstall", "--upgrade-strategy", "eager", "uritemplate")
+    run_cmdline(
+        config.venv_dir / "bin" / "pip",
+        "install",
+        "-U",
+        "--force-reinstall",
+        "--upgrade-strategy",
+        "eager",
+        "uritemplate",
+    )
+
 
 def create_pdm_file(config: OARepoConfig, output_directory: str):
     original_pdm_file = tomli.loads(
         (config.repository_dir / "pyproject.toml").read_text()
     )
     dependencies = original_pdm_file["project"]["dependencies"]
     oarepo_dependency = [
         x
         for x in dependencies
-        if re.match(r"^\s*oarepo\s*(\[[^\]]+\])?\s*==.*", x)  # take only oarepo package, discard others
+        if re.match(
+            r"^\s*oarepo\s*(\[[^\]]+\])?\s*==.*", x
+        )  # take only oarepo package, discard others
     ][0]
 
     original_pdm_file["project"]["dependencies"] = [oarepo_dependency]
 
     output_path = config.repository_dir / output_directory
     output_path.mkdir(parents=True, exist_ok=True)
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/pyproject.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/pyproject.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/s3.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/s3.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/__init__.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/assets.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/assets.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import shutil
 from pathlib import Path
 
-from .less import register_less_components
 from ..utils import run_cmdline
+from .less import register_less_components
 
 
 def load_watched_paths(paths_json, extra_paths):
     watched_paths = {}
     with open(paths_json) as f:
         for target, paths in json.load(f).items():
             if target.startswith("@"):
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/build.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/build.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/create.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import caseconverter
 
 from nrp_devtools.commands.pyproject import PyProject
-from nrp_devtools.commands.utils import run_cookiecutter, capitalize_name
+from nrp_devtools.commands.utils import capitalize_name, run_cookiecutter
 from nrp_devtools.config import OARepoConfig
 
 
 def create_page_ui(config: OARepoConfig, *, ui_name: str):
     ui_config = config.get_ui(ui_name)
 
     if (config.ui_dir / ui_config.name).exists():
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/less.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/less.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import re
-from pathlib import Path
 
 from nrp_devtools.commands.utils import run_cmdline
 from nrp_devtools.config import OARepoConfig
 
 
 def register_less_components(config: OARepoConfig, invenio_instance_path):
     data = run_cmdline(
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/ui/link_assets.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/ui/link_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import shutil
-import sys
 from pathlib import Path
 
 import click
 from tqdm import tqdm
 
 from nrp_devtools.config import OARepoConfig
 
@@ -42,15 +41,18 @@
         )
         linked[kind][source_file] = target_file
         if target_file in existing[kind]:
             existing[kind].remove(target_file)
 
     for kind, existing_data in existing.items():
         if existing_data:
-            click.secho(f"Error: following {kind} are not linked, will remove those from .venv assets", fg="red")
+            click.secho(
+                f"Error: following {kind} are not linked, will remove those from .venv assets",
+                fg="red",
+            )
             for target in existing_data:
                 if target.exists():
                     click.secho(f"  {target}", fg="red")
                     if target.is_dir():
                         shutil.rmtree(target)
                     else:
                         target.unlink()
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/commands/utils.py` & `nrp-devtools-0.1.9/src/nrp_devtools/commands/utils.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/config/config.py` & `nrp-devtools-0.1.9/src/nrp_devtools/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from typing import List, Optional, Set
 
 import dacite
 import yaml
 from yaml.representer import SafeRepresenter
 
+from .i18n_config import I18NConfig
 from .model_config import BaseModel, ModelConfig, ModelFeature
 from .repository_config import RepositoryConfig
 from .ui_config import UIConfig
 
 serialization_config = dacite.Config()
 serialization_config.type_hooks = {
     Path: lambda x: Path(x),
@@ -41,14 +42,15 @@
 
 @dataclasses.dataclass
 class OARepoConfig:
     repository_dir: Path
     repository: Optional[RepositoryConfig] = None
     models: List[ModelConfig] = dataclasses.field(default_factory=list)
     uis: List[UIConfig] = dataclasses.field(default_factory=list)
+    i18n: I18NConfig = dataclasses.field(default_factory=I18NConfig)
 
     python = "python3"
     python_version = ">=3.9,<3.11"
 
     @property
     def venv_dir(self):
         return self.repository_dir / ".venv"
@@ -127,14 +129,15 @@
             {"repository_dir": self.repository_dir, **config_data},
             serialization_config,
         )
 
         self.models = loaded.models
         self.uis = loaded.uis
         self.repository = loaded.repository
+        self.i18n = loaded.i18n
 
     def save(self):
         if self.config_file.exists():
             previous_config_data = self.config_file.read_text().strip()
         else:
             previous_config_data = None
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/config/enums.py` & `nrp-devtools-0.1.9/src/nrp_devtools/config/enums.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/config/model_config.py` & `nrp-devtools-0.1.9/src/nrp_devtools/config/model_config.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/config/repository_config.py` & `nrp-devtools-0.1.9/src/nrp_devtools/config/repository_config.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/config/wizard.py` & `nrp-devtools-0.1.9/src/nrp_devtools/config/wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 def prompt_set_choices(enum, prompt, default=None):
     """
     Prompt user to choose from enum values.
     """
     print(prompt)
 
-    choices = {chr(ord('A') + idx): e for idx, e in enumerate(enum)}
+    choices = {chr(ord("A") + idx): e for idx, e in enumerate(enum)}
 
     value = set(default or {})
 
     while True:
         for idx, c in choices.items():
             if c in value:
                 tick = "[x]"
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/component.less` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/component.less`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/README.md` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/README.md`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/Dockerfile.production` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/Dockerfile.production`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/docker-compose.yml` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/i18next.js` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/i18n/semantic-ui/translations/i18next.js`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/invenio.cfg` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/invenio.cfg`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/nrp` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/nrp`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/pyproject.toml` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/variables` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/variables`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/README.md` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.model_package}}/README.md`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/README.md` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/README.md`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.config` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.config`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.less` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/semantic-ui/less/theme.less`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/webpack.py` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/branding/webpack.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/TitlePage.jinja` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/{{cookiecutter.ui_package}}/titlepage/templates/TitlePage.jinja`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/__init__.py` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/__init__.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositForm.jsx` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/forms/deposit/DepositForm.jsx`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/EmptyResultsElement.jsx` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/EmptyResultsElement.jsx`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/MultipleSearchBarElement.jsx` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/MultipleSearchBarElement.jsx`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsGridItem.jsx` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsGridItem.jsx`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsListItem.jsx` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/components/ResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/index.js` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/semantic-ui/js/{{cookiecutter.name}}/search/index.js`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/webpack.py` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_model/{{cookiecutter.name}}/webpack.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/__init__.py` & `nrp-devtools-0.1.9/src/nrp_devtools/templates/ui_page/{{cookiecutter.name}}/__init__.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools/x509.py` & `nrp-devtools-0.1.9/src/nrp_devtools/x509.py`

 * *Files identical despite different names*

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools.egg-info/PKG-INFO` & `nrp-devtools-0.1.9/src/nrp_devtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrp-devtools
-Version: 0.1.8
+Version: 0.1.9
 Summary: NRP repository development tools
 Author-email: Miroslav Simek <miroslav.simek@cesnet.cz>
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools
 Requires-Dist: pip
 Requires-Dist: wheel
 Requires-Dist: click
@@ -26,14 +26,15 @@
 Requires-Dist: oarepo-tools
 Requires-Dist: minio
 Requires-Dist: redis
 Requires-Dist: psycopg[binary]
 Requires-Dist: pika
 Requires-Dist: opensearch-py
 Requires-Dist: pytest
+Requires-Dist: oarepo-tools
 
 # NRP repository development tools
 
 This tool is used to setup and run an Invenio based NRP instance. 
 
 ## Prerequisites
```

### Comparing `nrp-devtools-0.1.8/src/nrp_devtools.egg-info/SOURCES.txt` & `nrp-devtools-0.1.9/src/nrp_devtools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/nrp_devtools/cli/base.py
 src/nrp_devtools/cli/build.py
 src/nrp_devtools/cli/check.py
 src/nrp_devtools/cli/develop.py
 src/nrp_devtools/cli/initialize.py
 src/nrp_devtools/cli/model.py
 src/nrp_devtools/cli/run.py
+src/nrp_devtools/cli/translations.py
 src/nrp_devtools/cli/ui.py
 src/nrp_devtools/cli/upgrade.py
 src/nrp_devtools/commands/__init__.py
 src/nrp_devtools/commands/check.py
 src/nrp_devtools/commands/check_old.py
 src/nrp_devtools/commands/db.py
 src/nrp_devtools/commands/docker.py
@@ -44,14 +45,15 @@
 src/nrp_devtools/commands/ui/build.py
 src/nrp_devtools/commands/ui/create.py
 src/nrp_devtools/commands/ui/less.py
 src/nrp_devtools/commands/ui/link_assets.py
 src/nrp_devtools/config/__init__.py
 src/nrp_devtools/config/config.py
 src/nrp_devtools/config/enums.py
+src/nrp_devtools/config/i18n_config.py
 src/nrp_devtools/config/model_config.py
 src/nrp_devtools/config/repository_config.py
 src/nrp_devtools/config/ui_config.py
 src/nrp_devtools/config/wizard.py
 src/nrp_devtools/templates/component.less
 src/nrp_devtools/templates/repository/cookiecutter.json
 src/nrp_devtools/templates/repository/{{cookiecutter.repository_name}}/README.md
```

### Comparing `nrp-devtools-0.1.8/tests/test_repository_from_scratch.py` & `nrp-devtools-0.1.9/tests/test_repository_from_scratch.py`

 * *Files identical despite different names*

