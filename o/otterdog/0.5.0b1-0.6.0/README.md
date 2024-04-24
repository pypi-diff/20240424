# Comparing `tmp/otterdog-0.5.0b1.tar.gz` & `tmp/otterdog-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otterdog-0.5.0b1.tar", max compression
+gzip compressed data, was "otterdog-0.6.0.tar", max compression
```

## Comparing `otterdog-0.5.0b1.tar` & `otterdog-0.6.0.tar`

### file list

```diff
@@ -1,255 +1,168 @@
--rw-r--r--   0        0        0    13171 2024-03-05 21:37:46.070242 otterdog-0.5.0b1/CHANGELOG.md
--rw-r--r--   0        0        0    14197 2024-03-05 21:37:46.070242 otterdog-0.5.0b1/LICENSE
--rw-r--r--   0        0        0     5911 2024-03-05 21:37:46.070242 otterdog-0.5.0b1/README.md
--rw-r--r--   0        0        0      441 2024-03-05 21:37:46.070242 otterdog-0.5.0b1/otterdog/__init__.py
--rw-r--r--   0        0        0     2340 2024-03-05 21:37:46.070242 otterdog-0.5.0b1/otterdog/app.py
--rw-r--r--   0        0        0    15144 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/cli.py
--rw-r--r--   0        0        0    10126 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/config.py
--rw-r--r--   0        0        0     2312 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/credentials/__init__.py
--rw-r--r--   0        0        0     4414 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/credentials/bitwarden_provider.py
--rw-r--r--   0        0        0     1198 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/credentials/inmemory_provider.py
--rw-r--r--   0        0        0     4124 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/credentials/pass_provider.py
--rw-r--r--   0        0        0    11633 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/jsonnet.py
--rw-r--r--   0        0        0    19085 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/__init__.py
--rw-r--r--   0        0        0    18106 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/branch_protection_rule.py
--rw-r--r--   0        0        0     9603 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/environment.py
--rw-r--r--   0        0        0    22528 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/github_organization.py
--rw-r--r--   0        0        0     5512 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/organization_secret.py
--rw-r--r--   0        0        0    10118 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/organization_settings.py
--rw-r--r--   0        0        0     5415 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/organization_variable.py
--rw-r--r--   0        0        0     2168 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/organization_webhook.py
--rw-r--r--   0        0        0     5497 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/organization_workflow_settings.py
--rw-r--r--   0        0        0     2557 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repo_ruleset.py
--rw-r--r--   0        0        0     2482 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repo_secret.py
--rw-r--r--   0        0        0     2510 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repo_variable.py
--rw-r--r--   0        0        0     2556 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repo_webhook.py
--rw-r--r--   0        0        0     8783 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repo_workflow_settings.py
--rw-r--r--   0        0        0    36505 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/repository.py
--rw-r--r--   0        0        0    22285 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/ruleset.py
--rw-r--r--   0        0        0     6872 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/secret.py
--rw-r--r--   0        0        0     2245 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/variable.py
--rw-r--r--   0        0        0     8997 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/webhook.py
--rw-r--r--   0        0        0     6919 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/models/workflow_settings.py
--rw-r--r--   0        0        0     6793 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/__init__.py
--rw-r--r--   0        0        0     5314 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/apply.py
--rw-r--r--   0        0        0     3881 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/canonical_diff.py
--rw-r--r--   0        0        0     4037 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/delete_file.py
--rw-r--r--   0        0        0     9624 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/diff_operation.py
--rw-r--r--   0        0        0     2308 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/dispatch_workflow.py
--rw-r--r--   0        0        0     3874 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/fetch_config.py
--rw-r--r--   0        0        0     4477 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/import_configuration.py
--rw-r--r--   0        0        0     2856 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/list_apps.py
--rw-r--r--   0        0        0     3753 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/list_members.py
--rw-r--r--   0        0        0     2038 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/local_plan.py
--rw-r--r--   0        0        0     4286 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/plan.py
--rw-r--r--   0        0        0     3418 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/push_config.py
--rw-r--r--   0        0        0    11627 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/show.py
--rw-r--r--   0        0        0     7470 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/show_default.py
--rw-r--r--   0        0        0     2523 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/show_live.py
--rw-r--r--   0        0        0     3471 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/sync_template.py
--rw-r--r--   0        0        0     4310 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/validate.py
--rw-r--r--   0        0        0     1526 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/operations/web_login.py
--rw-r--r--   0        0        0      441 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/__init__.py
--rw-r--r--   0        0        0    16010 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/__init__.py
--rw-r--r--   0        0        0     1057 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/auth/__init__.py
--rw-r--r--   0        0        0     2541 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/auth/app.py
--rw-r--r--   0        0        0     1156 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/auth/token.py
--rw-r--r--   0        0        0      626 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/cache/__init__.py
--rw-r--r--   0        0        0     1024 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/cache/file.py
--rw-r--r--   0        0        0     1077 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/cache/redis.py
--rw-r--r--   0        0        0     1121 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/exception.py
--rw-r--r--   0        0        0    11399 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/graphql.py
--rw-r--r--   0        0        0     3930 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/__init__.py
--rw-r--r--   0        0        0     2551 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/app_client.py
--rw-r--r--   0        0        0     1446 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/commit_client.py
--rw-r--r--   0        0        0     4624 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/content_client.py
--rw-r--r--   0        0        0     1271 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/issue_client.py
--rw-r--r--   0        0        0    24893 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/org_client.py
--rw-r--r--   0        0        0     1905 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/pull_request_client.py
--rw-r--r--   0        0        0    45094 2024-03-05 21:37:46.074242 otterdog-0.5.0b1/otterdog/providers/github/rest/repo_client.py
--rw-r--r--   0        0        0     5404 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/providers/github/rest/requester.py
--rw-r--r--   0        0        0     1794 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/providers/github/rest/team_client.py
--rw-r--r--   0        0        0     1116 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/providers/github/rest/user_client.py
--rw-r--r--   0        0        0     1410 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/providers/github/stats/__init__.py
--rw-r--r--   0        0        0    16253 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/providers/github/web.py
--rw-r--r--   0        0        0        0 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/py.typed
--rw-r--r--   0        0        0      441 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/__init__.py
--rw-r--r--   0        0        0     2271 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/github-web-settings.jsonnet
--rw-r--r--   0        0        0     2984 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-branch-protection-rules.gql
--rw-r--r--   0        0        0      610 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-bypass-force-push-allowances.gql
--rw-r--r--   0        0        0      612 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-bypass-pull-request-allowances.gql
--rw-r--r--   0        0        0      417 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-issue-comments.gql
--rw-r--r--   0        0        0      599 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-push-allowances.gql
--rw-r--r--   0        0        0      610 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-review-dismissal-allowances.gql
--rw-r--r--   0        0        0      291 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/graphql/get-team-membership.gql
--rw-r--r--   0        0        0     1984 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/branch-protection-rule.json
--rw-r--r--   0        0        0      440 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/environment.json
--rw-r--r--   0        0        0      363 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/org-secret.json
--rw-r--r--   0        0        0      365 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/org-variable.json
--rw-r--r--   0        0        0      697 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/org-workflow-settings.json
--rw-r--r--   0        0        0      599 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/organization.json
--rw-r--r--   0        0        0      213 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/repo-secret.json
--rw-r--r--   0        0        0      215 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/repo-variable.json
--rw-r--r--   0        0        0      576 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/repo-workflow-settings.json
--rw-r--r--   0        0        0     1690 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/repository-ruleset.json
--rw-r--r--   0        0        0     2975 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/repository.json
--rw-r--r--   0        0        0     3846 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/settings.json
--rw-r--r--   0        0        0      651 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/resources/schemas/webhook.json
--rw-r--r--   0        0        0    15994 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/utils.py
--rw-r--r--   0        0        0     2503 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/__init__.py
--rw-r--r--   0        0        0      539 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/api/__init__.py
--rw-r--r--   0        0        0     1994 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/api/routes.py
--rw-r--r--   0        0        0     2314 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/config.py
--rw-r--r--   0        0        0     1793 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/db/__init__.py
--rw-r--r--   0        0        0     3219 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/db/models.py
--rw-r--r--   0        0        0    14417 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/db/service.py
--rw-r--r--   0        0        0     2155 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/filters.py
--rw-r--r--   0        0        0      536 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/home/__init__.py
--rw-r--r--   0        0        0     7028 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/home/routes.py
--rw-r--r--   0        0        0        0 2024-03-05 21:37:46.078242 otterdog-0.5.0b1/otterdog/webapp/static/assets/.gitkeep
--rw-r--r--   0        0        0   782934 2024-03-05 21:37:46.082242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/adminlte.css
--rw-r--r--   0        0        0  1460324 2024-03-05 21:37:46.086242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/adminlte.css.map
--rw-r--r--   0        0        0   675171 2024-03-05 21:37:46.086242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/adminlte.min.css
--rw-r--r--   0        0        0   143463 2024-03-05 21:37:46.086242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.components.css
--rw-r--r--   0        0        0   287877 2024-03-05 21:37:46.090242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.components.css.map
--rw-r--r--   0        0        0   128794 2024-03-05 21:37:46.090242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.components.min.css
--rw-r--r--   0        0        0   130238 2024-03-05 21:37:46.090242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.components.min.css.map
--rw-r--r--   0        0        0   395356 2024-03-05 21:37:46.094242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.core.css
--rw-r--r--   0        0        0   794720 2024-03-05 21:37:46.094242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.core.css.map
--rw-r--r--   0        0        0   336170 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.core.min.css
--rw-r--r--   0        0        0   472858 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.core.min.css.map
--rw-r--r--   0        0        0    21524 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.extra-components.css
--rw-r--r--   0        0        0   148702 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.extra-components.css.map
--rw-r--r--   0        0        0    18032 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.extra-components.min.css
--rw-r--r--   0        0        0    85392 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.extra-components.min.css.map
--rw-r--r--   0        0        0     7592 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.pages.css
--rw-r--r--   0        0        0   127397 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.pages.css.map
--rw-r--r--   0        0        0     6335 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.pages.min.css
--rw-r--r--   0        0        0    65937 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.pages.min.css.map
--rw-r--r--   0        0        0   199998 2024-03-05 21:37:46.098242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.plugins.css
--rw-r--r--   0        0        0   310110 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.plugins.css.map
--rw-r--r--   0        0        0   180321 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.plugins.min.css
--rw-r--r--   0        0        0   135370 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/css/alt/adminlte.plugins.min.css.map
--rw-r--r--   0        0        0     1150 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/favicon.ico
--rw-r--r--   0        0        0     1600 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/gulpfile.js
--rw-r--r--   0        0        0     2637 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/img/AdminLTELogo.png
--rw-r--r--   0        0        0      866 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/js/.eslintrc.json
--rw-r--r--   0        0        0    68433 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/js/adminlte.js
--rw-r--r--   0        0        0    30024 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/js/adminlte.min.js
--rw-r--r--   0        0        0     1285 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/package.json
--rw-r--r--   0        0        0      958 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_adminlte.raw.scss
--rw-r--r--   0        0        0      614 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_alerts.scss
--rw-r--r--   0        0        0    36771 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_bootstrap-variables.scss
--rw-r--r--   0        0        0     1408 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_brand.scss
--rw-r--r--   0        0        0     2014 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_buttons.scss
--rw-r--r--   0        0        0      916 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_callout.scss
--rw-r--r--   0        0        0     7451 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_cards.scss
--rw-r--r--   0        0        0      286 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_carousel.scss
--rw-r--r--   0        0        0     1655 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_colors.scss
--rw-r--r--   0        0        0     2967 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_control-sidebar.scss
--rw-r--r--   0        0        0     3584 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_direct-chat.scss
--rw-r--r--   0        0        0     4709 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_dropdown.scss
--rw-r--r--   0        0        0      212 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_elevation.scss
--rw-r--r--   0        0        0     5507 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_forms.scss
--rw-r--r--   0        0        0     2445 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_info-box.scss
--rw-r--r--   0        0        0    12437 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_layout.scss
--rw-r--r--   0        0        0     2577 2024-03-05 21:37:46.102242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_main-header.scss
--rw-r--r--   0        0        0    19848 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_main-sidebar.scss
--rw-r--r--   0        0        0     7255 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_miscellaneous.scss
--rw-r--r--   0        0        0      274 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_mixins.scss
--rw-r--r--   0        0        0      566 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_modals.scss
--rw-r--r--   0        0        0     1989 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_navs.scss
--rw-r--r--   0        0        0      904 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_print.scss
--rw-r--r--   0        0        0      768 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_products.scss
--rw-r--r--   0        0        0      871 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_progress-bars.scss
--rw-r--r--   0        0        0     2877 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_sidebar-mini.scss
--rw-r--r--   0        0        0     2211 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_small-box.scss
--rw-r--r--   0        0        0     1446 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_social-widgets.scss
--rw-r--r--   0        0        0     1519 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_table.scss
--rw-r--r--   0        0        0      506 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_text.scss
--rw-r--r--   0        0        0     2370 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_timeline.scss
--rw-r--r--   0        0        0      745 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_toasts.scss
--rw-r--r--   0        0        0      620 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_users-list.scss
--rw-r--r--   0        0        0     9399 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/_variables.scss
--rw-r--r--   0        0        0      658 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/adminlte.scss
--rw-r--r--   0        0        0     2364 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_accent.scss
--rw-r--r--   0        0        0     1543 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_backgrounds.scss
--rw-r--r--   0        0        0     1495 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_cards.scss
--rw-r--r--   0        0        0     1890 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_custom-forms.scss
--rw-r--r--   0        0        0      314 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_direct-chat.scss
--rw-r--r--   0        0        0      698 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_miscellaneous.scss
--rw-r--r--   0        0        0      654 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_navbar.scss
--rw-r--r--   0        0        0     3441 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_sidebar.scss
--rw-r--r--   0        0        0      407 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/mixins/_toasts.scss
--rw-r--r--   0        0        0      671 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_404_500_errors.scss
--rw-r--r--   0        0        0      769 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_e-commerce.scss
--rw-r--r--   0        0        0      165 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_invoice.scss
--rw-r--r--   0        0        0     1163 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_lockscreen.scss
--rw-r--r--   0        0        0     1608 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_login_and_register.scss
--rw-r--r--   0        0        0     1307 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_mailbox.scss
--rw-r--r--   0        0        0      485 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_profile.scss
--rw-r--r--   0        0        0      319 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/pages/_projects.scss
--rw-r--r--   0        0        0      245 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_components.scss
--rw-r--r--   0        0        0      214 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_core.scss
--rw-r--r--   0        0        0      206 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_extra-components.scss
--rw-r--r--   0        0        0      142 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_miscellaneous.scss
--rw-r--r--   0        0        0      271 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_pages.scss
--rw-r--r--   0        0        0      419 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/_plugins.scss
--rw-r--r--   0        0        0      518 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/adminlte.components.scss
--rw-r--r--   0        0        0      534 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/adminlte.core.scss
--rw-r--r--   0        0        0      530 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/adminlte.extra-components.scss
--rw-r--r--   0        0        0      541 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/adminlte.pages.scss
--rw-r--r--   0        0        0      512 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/parts/adminlte.plugins.scss
--rw-r--r--   0        0        0      489 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_bootstrap-slider.scss
--rw-r--r--   0        0        0     4457 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_bootstrap-switch.scss
--rw-r--r--   0        0        0     1816 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_fullcalendar.scss
--rw-r--r--   0        0        0     1566 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_icheck-bootstrap.scss
--rw-r--r--   0        0        0      447 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_jqvmap.scss
--rw-r--r--   0        0        0     1338 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_mapael.scss
--rw-r--r--   0        0        0      572 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_miscellaneous.scss
--rw-r--r--   0        0        0     1677 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_mixins.scss
--rw-r--r--   0        0        0     3980 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_pace.scss
--rw-r--r--   0        0        0     5653 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_select2.scss
--rw-r--r--   0        0        0      647 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_sweetalert2.scss
--rw-r--r--   0        0        0     1197 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/static/assets/scss/plugins/_toastr.scss
--rw-r--r--   0        0        0     8056 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/__init__.py
--rw-r--r--   0        0        0     5735 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/apply_changes.py
--rw-r--r--   0        0        0     6941 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/check_sync.py
--rw-r--r--   0        0        0     2849 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/complete_pull_request.py
--rw-r--r--   0        0        0     2124 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/fetch_all_pull_requests.py
--rw-r--r--   0        0        0     2643 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/fetch_config.py
--rw-r--r--   0        0        0     1920 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/help_comment.py
--rw-r--r--   0        0        0     3298 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/retrieve_team_membership.py
--rw-r--r--   0        0        0     1779 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/update_pull_request.py
--rw-r--r--   0        0        0     8716 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/tasks/validate_pull_request.py
--rw-r--r--   0        0        0     3544 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/accounts/login.html
--rw-r--r--   0        0        0     3944 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/accounts/register.html
--rw-r--r--   0        0        0      526 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/applied_changes_comment.txt
--rw-r--r--   0        0        0       83 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/done_comment.txt
--rw-r--r--   0        0        0      519 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/help_comment.txt
--rw-r--r--   0        0        0      148 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/in_sync_comment.txt
--rw-r--r--   0        0        0      392 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/out_of_sync_comment.txt
--rw-r--r--   0        0        0      549 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/team_membership_comment.txt
--rw-r--r--   0        0        0      449 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/validation_comment.txt
--rw-r--r--   0        0        0      137 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/comment/wrong_team_done_comment.txt
--rw-r--r--   0        0        0     7562 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/index.html
--rw-r--r--   0        0        0    23534 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/organization.html
--rw-r--r--   0        0        0     4494 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/organizations.html
--rw-r--r--   0        0        0     2203 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/page-403.html
--rw-r--r--   0        0        0     1952 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/page-404.html
--rw-r--r--   0        0        0     1950 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/page-500.html
--rw-r--r--   0        0        0     8227 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/pullrequests.html
--rw-r--r--   0        0        0    20012 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/repository.html
--rw-r--r--   0        0        0     5704 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/home/tasks.html
--rw-r--r--   0        0        0      377 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/includes/footer.html
--rw-r--r--   0        0        0      453 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/includes/navigation.html
--rw-r--r--   0        0        0      405 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/includes/scripts.html
--rw-r--r--   0        0        0     4345 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/includes/sidebar.html
--rw-r--r--   0        0        0      708 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/layouts/base-fullscreen.html
--rw-r--r--   0        0        0     1028 2024-03-05 21:37:46.106242 otterdog-0.5.0b1/otterdog/webapp/templates/layouts/base.html
--rw-r--r--   0        0        0     7199 2024-03-05 21:37:46.110242 otterdog-0.5.0b1/otterdog/webapp/utils.py
--rw-r--r--   0        0        0     9034 2024-03-05 21:37:46.110242 otterdog-0.5.0b1/otterdog/webapp/webhook/__init__.py
--rw-r--r--   0        0        0     4050 2024-03-05 21:37:46.110242 otterdog-0.5.0b1/otterdog/webapp/webhook/github_models.py
--rw-r--r--   0        0        0     5935 2024-03-05 21:37:46.110242 otterdog-0.5.0b1/otterdog/webapp/webhook/github_webhook.py
--rw-r--r--   0        0        0     3272 2024-03-05 21:37:46.110242 otterdog-0.5.0b1/pyproject.toml
--rw-r--r--   0        0        0     7816 1970-01-01 00:00:00.000000 otterdog-0.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0    14593 2024-04-24 20:36:49.799538 otterdog-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    14197 2024-04-24 20:36:49.799538 otterdog-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5911 2024-04-24 20:36:49.799538 otterdog-0.6.0/README.md
+-rw-r--r--   0        0        0      520 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/__init__.py
+-rw-r--r--   0        0        0     2285 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/app.py
+-rw-r--r--   0        0        0    15035 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/cli.py
+-rw-r--r--   0        0        0    10126 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/config.py
+-rw-r--r--   0        0        0     2312 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/credentials/__init__.py
+-rw-r--r--   0        0        0     4414 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/credentials/bitwarden_provider.py
+-rw-r--r--   0        0        0     1198 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/credentials/inmemory_provider.py
+-rw-r--r--   0        0        0     4124 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/credentials/pass_provider.py
+-rw-r--r--   0        0        0    11633 2024-04-24 20:36:49.803538 otterdog-0.6.0/otterdog/jsonnet.py
+-rw-r--r--   0        0        0    19761 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/__init__.py
+-rw-r--r--   0        0        0    18106 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/branch_protection_rule.py
+-rw-r--r--   0        0        0     9603 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/environment.py
+-rw-r--r--   0        0        0    22528 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/github_organization.py
+-rw-r--r--   0        0        0     5512 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/organization_secret.py
+-rw-r--r--   0        0        0    10380 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/organization_settings.py
+-rw-r--r--   0        0        0     5415 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/organization_variable.py
+-rw-r--r--   0        0        0     2168 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/organization_webhook.py
+-rw-r--r--   0        0        0     5497 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/organization_workflow_settings.py
+-rw-r--r--   0        0        0     2557 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repo_ruleset.py
+-rw-r--r--   0        0        0     2482 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repo_secret.py
+-rw-r--r--   0        0        0     2510 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repo_variable.py
+-rw-r--r--   0        0        0     2556 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repo_webhook.py
+-rw-r--r--   0        0        0     8783 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repo_workflow_settings.py
+-rw-r--r--   0        0        0    36779 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/repository.py
+-rw-r--r--   0        0        0    22285 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/ruleset.py
+-rw-r--r--   0        0        0     6872 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/secret.py
+-rw-r--r--   0        0        0     2245 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/variable.py
+-rw-r--r--   0        0        0     8997 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/webhook.py
+-rw-r--r--   0        0        0     6919 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/models/workflow_settings.py
+-rw-r--r--   0        0        0     6793 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/__init__.py
+-rw-r--r--   0        0        0     5314 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/apply.py
+-rw-r--r--   0        0        0     3881 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/canonical_diff.py
+-rw-r--r--   0        0        0     4037 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/delete_file.py
+-rw-r--r--   0        0        0     9624 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/diff_operation.py
+-rw-r--r--   0        0        0     2308 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/dispatch_workflow.py
+-rw-r--r--   0        0        0     3874 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/fetch_config.py
+-rw-r--r--   0        0        0     4477 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/import_configuration.py
+-rw-r--r--   0        0        0     2856 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/list_apps.py
+-rw-r--r--   0        0        0     3753 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/list_members.py
+-rw-r--r--   0        0        0     2038 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/local_plan.py
+-rw-r--r--   0        0        0     4286 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/plan.py
+-rw-r--r--   0        0        0     3418 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/push_config.py
+-rw-r--r--   0        0        0    11627 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/show.py
+-rw-r--r--   0        0        0     7470 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/show_default.py
+-rw-r--r--   0        0        0     2523 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/show_live.py
+-rw-r--r--   0        0        0     3471 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/sync_template.py
+-rw-r--r--   0        0        0     4310 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/validate.py
+-rw-r--r--   0        0        0     1526 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/operations/web_login.py
+-rw-r--r--   0        0        0      441 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/providers/__init__.py
+-rw-r--r--   0        0        0    15930 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/providers/github/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/providers/github/auth/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/providers/github/auth/app.py
+-rw-r--r--   0        0        0     1156 2024-04-24 20:36:49.807538 otterdog-0.6.0/otterdog/providers/github/auth/token.py
+-rw-r--r--   0        0        0      626 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/cache/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/cache/file.py
+-rw-r--r--   0        0        0     1077 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/cache/redis.py
+-rw-r--r--   0        0        0     1121 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/exception.py
+-rw-r--r--   0        0        0    11399 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/graphql.py
+-rw-r--r--   0        0        0     3930 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/__init__.py
+-rw-r--r--   0        0        0     2551 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/app_client.py
+-rw-r--r--   0        0        0     2037 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/commit_client.py
+-rw-r--r--   0        0        0     4624 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/content_client.py
+-rw-r--r--   0        0        0     1271 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/issue_client.py
+-rw-r--r--   0        0        0    24893 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/org_client.py
+-rw-r--r--   0        0        0     4544 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/pull_request_client.py
+-rw-r--r--   0        0        0    47071 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/repo_client.py
+-rw-r--r--   0        0        0     5404 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/requester.py
+-rw-r--r--   0        0        0     1794 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/team_client.py
+-rw-r--r--   0        0        0     1116 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/rest/user_client.py
+-rw-r--r--   0        0        0     1410 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/stats/__init__.py
+-rw-r--r--   0        0        0    16253 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/providers/github/web.py
+-rw-r--r--   0        0        0        0 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/py.typed
+-rw-r--r--   0        0        0      441 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/__init__.py
+-rw-r--r--   0        0        0     2271 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/github-web-settings.jsonnet
+-rw-r--r--   0        0        0     2957 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-branch-protection-rules.gql
+-rw-r--r--   0        0        0      610 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-bypass-force-push-allowances.gql
+-rw-r--r--   0        0        0      612 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-bypass-pull-request-allowances.gql
+-rw-r--r--   0        0        0      417 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-issue-comments.gql
+-rw-r--r--   0        0        0      599 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-push-allowances.gql
+-rw-r--r--   0        0        0      610 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-review-dismissal-allowances.gql
+-rw-r--r--   0        0        0      291 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/graphql/get-team-membership.gql
+-rw-r--r--   0        0        0     1984 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/branch-protection-rule.json
+-rw-r--r--   0        0        0      440 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/environment.json
+-rw-r--r--   0        0        0      363 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/org-secret.json
+-rw-r--r--   0        0        0      365 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/org-variable.json
+-rw-r--r--   0        0        0      697 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/org-workflow-settings.json
+-rw-r--r--   0        0        0      599 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/organization.json
+-rw-r--r--   0        0        0      213 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/repo-secret.json
+-rw-r--r--   0        0        0      215 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/repo-variable.json
+-rw-r--r--   0        0        0      576 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/repo-workflow-settings.json
+-rw-r--r--   0        0        0     1690 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/repository-ruleset.json
+-rw-r--r--   0        0        0     3045 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/repository.json
+-rw-r--r--   0        0        0     3846 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/settings.json
+-rw-r--r--   0        0        0      651 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/resources/schemas/webhook.json
+-rw-r--r--   0        0        0    15994 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/utils.py
+-rw-r--r--   0        0        0     3580 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/api/__init__.py
+-rw-r--r--   0        0        0     1871 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/api/graphql.py
+-rw-r--r--   0        0        0     2551 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/api/routes.py
+-rw-r--r--   0        0        0     2608 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/api/schema.graphql
+-rw-r--r--   0        0        0     2148 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/auth/__init__.py
+-rw-r--r--   0        0        0     3385 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/auth/routes.py
+-rw-r--r--   0        0        0     2557 2024-04-24 20:36:49.811538 otterdog-0.6.0/otterdog/webapp/config.py
+-rw-r--r--   0        0        0     1835 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/db/__init__.py
+-rw-r--r--   0        0        0     4001 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/db/models.py
+-rw-r--r--   0        0        0    18147 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/db/service.py
+-rw-r--r--   0        0        0     2155 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/filters.py
+-rw-r--r--   0        0        0     1054 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/home/__init__.py
+-rw-r--r--   0        0        0    10316 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/home/routes.py
+-rw-r--r--   0        0        0     1150 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/assets/favicon.ico
+-rw-r--r--   0        0        0       26 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/assets/robots.txt
+-rw-r--r--   0        0        0    99600 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/package-lock.json
+-rw-r--r--   0        0        0      628 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/package.json
+-rw-r--r--   0        0        0       62 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/src/css/app.css
+-rw-r--r--   0        0        0      107 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/src/css/editor.css
+-rw-r--r--   0        0        0       20 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/src/js/app.js
+-rw-r--r--   0        0        0     1002 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/src/js/editor.js
+-rw-r--r--   0        0        0     3442 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/static/vite.config.js
+-rw-r--r--   0        0        0     9994 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/__init__.py
+-rw-r--r--   0        0        0     8552 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/apply_changes.py
+-rw-r--r--   0        0        0     1944 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/auto_merge_comment.py
+-rw-r--r--   0        0        0     9512 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/check_sync.py
+-rw-r--r--   0        0        0     3800 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/complete_pull_request.py
+-rw-r--r--   0        0        0     2084 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/fetch_all_pull_requests.py
+-rw-r--r--   0        0        0     4053 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/fetch_config.py
+-rw-r--r--   0        0        0     1881 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/help_comment.py
+-rw-r--r--   0        0        0     4222 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/merge_pull_request.py
+-rw-r--r--   0        0        0     3852 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/retrieve_team_membership.py
+-rw-r--r--   0        0        0     3350 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/update_pull_request.py
+-rw-r--r--   0        0        0    10627 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/tasks/validate_pull_request.py
+-rw-r--r--   0        0        0     1205 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/auth/login.html
+-rw-r--r--   0        0        0      648 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/applied_changes_comment.txt
+-rw-r--r--   0        0        0      436 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/auto_merge_comment.txt
+-rw-r--r--   0        0        0       83 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/done_comment.txt
+-rw-r--r--   0        0        0     1322 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/help_comment.txt
+-rw-r--r--   0        0        0      148 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/in_sync_comment.txt
+-rw-r--r--   0        0        0      442 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/out_of_sync_comment.txt
+-rw-r--r--   0        0        0      553 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/team_membership_comment.txt
+-rw-r--r--   0        0        0      438 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/validation_comment.txt
+-rw-r--r--   0        0        0      148 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/wrong_team_apply_comment.txt
+-rw-r--r--   0        0        0      152 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/wrong_team_done_comment.txt
+-rw-r--r--   0        0        0      152 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/comment/wrong_user_merge_comment.txt
+-rw-r--r--   0        0        0     8670 2024-04-24 20:36:49.815538 otterdog-0.6.0/otterdog/webapp/templates/home/index.html
+-rw-r--r--   0        0        0    23929 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/organization.html
+-rw-r--r--   0        0        0     3595 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/organizations.html
+-rw-r--r--   0        0        0     1306 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/page-401.html
+-rw-r--r--   0        0        0     1218 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/page-404.html
+-rw-r--r--   0        0        0     1216 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/page-500.html
+-rw-r--r--   0        0        0     4342 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/projects.html
+-rw-r--r--   0        0        0     7371 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/pullrequests.html
+-rw-r--r--   0        0        0     6196 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/query.html
+-rw-r--r--   0        0        0    20506 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/repository.html
+-rw-r--r--   0        0        0     4929 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/home/tasks.html
+-rw-r--r--   0        0        0      377 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/includes/footer.html
+-rw-r--r--   0        0        0     1606 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/includes/navigation.html
+-rw-r--r--   0        0        0     4975 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/includes/sidebar.html
+-rw-r--r--   0        0        0     1429 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/layouts/base-fullscreen.html
+-rw-r--r--   0        0        0     1698 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/templates/layouts/base.html
+-rw-r--r--   0        0        0     8275 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/utils.py
+-rw-r--r--   0        0        0     8872 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/webhook/__init__.py
+-rw-r--r--   0        0        0     6130 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/webhook/comment_handlers.py
+-rw-r--r--   0        0        0     4494 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/webhook/github_models.py
+-rw-r--r--   0        0        0     5935 2024-04-24 20:36:49.819537 otterdog-0.6.0/otterdog/webapp/webhook/github_webhook.py
+-rw-r--r--   0        0        0     3505 2024-04-24 20:36:49.819537 otterdog-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7814 1970-01-01 00:00:00.000000 otterdog-0.6.0/PKG-INFO
```

### Comparing `otterdog-0.5.0b1/CHANGELOG.md` & `otterdog-0.6.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 # Change Log
 
-## [0.5.0] - unreleased
+## [0.6.0] - 24/04/2024
+
+### Added
+
+- Added support for oauth authentication using GitHub. ([#202](https://github.com/eclipse-csi/otterdog/issues/202))
+- Added support for auto-merging of PRs under certain conditions. ([#110](https://github.com/eclipse-csi/otterdog/issues/110))
+- Added handling for settings that require access to the Web UI. ([#208](https://github.com/eclipse-csi/otterdog/issues/208))
+- Added support for repository setting `private_vulnerability_reporting_enabled`. ([#205](https://github.com/eclipse-csi/otterdog/issues/205))
+- Added a graphql based query interface to the dashboard. ([#204](https://github.com/eclipse-csi/otterdog/issues/204))
+
+### Changed
+
+- Reduced the number of automatic checks that are performed every time a PR gets updated. ([#217](https://github.com/eclipse-csi/otterdog/issues/217))
+- Support auto-merge also for project leads and admins. ([#216](https://github.com/eclipse-csi/otterdog/issues/216))
+- Do not enable auto-merge for PRs that also touch files other than the configuration. ([#220](https://github.com/eclipse-csi/otterdog/issues/220))
+- Use scoped commands for interaction via pull requests. ([#211](https://github.com/eclipse-csi/otterdog/issues/211))
+
+### Fixed
+
+- Use pagination when retrieving all branches of a repository.
+
+
+## [0.5.0] - 05/03/2024
+
+Note: this version includes lots of additions and changes related to the GitHub App mode which are not
+covered in the changelog.
 
 ### Added
 
 - Added automatic handling of configuration changes by acting as a GitHub App.
 - Support adding wildcards to `Webhook` urls to hide sensitive parts. ([#84](https://github.com/eclipse-csi/otterdog/issues/84))
 
 ### Changed
```

### Comparing `otterdog-0.5.0b1/LICENSE` & `otterdog-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/README.md` & `otterdog-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/cli.py` & `otterdog-0.6.0/otterdog/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 #  This program and the accompanying materials are made available
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
 import asyncio
-import importlib.metadata
 import sys
 import traceback
 from typing import Any
 
 import click
 from click.shell_completion import CompletionItem
 
+from . import __version__
 from .config import OtterdogConfig
 from .operations import Operation
 from .operations.apply import ApplyOperation
 from .operations.canonical_diff import CanonicalDiffOperation
 from .operations.delete_file import DeleteFileOperation
 from .operations.dispatch_workflow import DispatchWorkflowOperation
 from .operations.fetch_config import FetchOperation
@@ -33,18 +33,14 @@
 from .operations.show_live import ShowLiveOperation
 from .operations.sync_template import SyncTemplateOperation
 from .operations.validate import ValidateOperation
 from .operations.web_login import WebLoginOperation
 from .utils import IndentingPrinter, init, is_debug_enabled, print_error
 
 _CONFIG_FILE = "otterdog.json"
-
-_DISTRIBUTION_METADATA = importlib.metadata.metadata("otterdog")
-_VERSION = _DISTRIBUTION_METADATA["Version"]
-
 _CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"], max_content_width=120)
 
 _CONFIG: OtterdogConfig | None = None
 
 
 def complete_organizations(ctx, param, incomplete):
     config_file = ctx.params.get("config")
@@ -118,15 +114,15 @@
             print_error(str(e))
             sys.exit(2)
 
         return super().invoke(ctx)
 
 
 @click.group(context_settings=_CONTEXT_SETTINGS)
-@click.version_option(version=_VERSION, prog_name="otterdog.sh")
+@click.version_option(version=__version__, prog_name="otterdog.sh")
 def cli():
     """
     Managing GitHub organizations at scale.
     """
 
 
 @cli.command(cls=StdCommand)
```

### Comparing `otterdog-0.5.0b1/otterdog/config.py` & `otterdog-0.6.0/otterdog/config.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/credentials/__init__.py` & `otterdog-0.6.0/otterdog/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/credentials/bitwarden_provider.py` & `otterdog-0.6.0/otterdog/credentials/bitwarden_provider.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/credentials/inmemory_provider.py` & `otterdog-0.6.0/otterdog/credentials/inmemory_provider.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/credentials/pass_provider.py` & `otterdog-0.6.0/otterdog/credentials/pass_provider.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/jsonnet.py` & `otterdog-0.6.0/otterdog/jsonnet.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/__init__.py` & `otterdog-0.6.0/otterdog/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,28 @@
         forced_update: bool,
         fn: LivePatchApplyFn,
     ) -> LivePatch:
         return LivePatch(
             LivePatchType.CHANGE, expected_object, current_object, changes, parent_object, forced_update, fn
         )
 
+    def requires_web_ui(self) -> bool:
+        match self.patch_type:
+            case LivePatchType.ADD:
+                assert self.expected_object is not None
+                return self.expected_object.requires_web_ui()
+
+            case LivePatchType.REMOVE:
+                return False
+
+            case LivePatchType.CHANGE:
+                assert self.expected_object is not None
+                assert self.changes is not None
+                return self.expected_object.changes_require_web_ui(self.changes)
+
     def requires_secrets(self) -> bool:
         match self.patch_type:
             case LivePatchType.ADD:
                 assert self.expected_object is not None
                 return self.expected_object.contains_secrets()
 
             case LivePatchType.REMOVE:
@@ -433,14 +447,20 @@
             if self.is_nested_model_key(key):
                 result[key] = cast(ModelObject, value).to_model_dict(for_diff, include_nested_models)
             else:
                 result[key] = value
 
         return result
 
+    def requires_web_ui(self) -> bool:
+        return False
+
+    def changes_require_web_ui(self, changes: dict[str, Change]) -> bool:
+        return False
+
     def contains_secrets(self) -> bool:
         return False
 
     def resolve_secrets(self, secret_resolver: Callable[[str], str]) -> None:
         pass
 
     def copy_secrets(self, other_object: ModelObject) -> None:
```

### Comparing `otterdog-0.5.0b1/otterdog/models/branch_protection_rule.py` & `otterdog-0.6.0/otterdog/models/branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/environment.py` & `otterdog-0.6.0/otterdog/models/environment.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/github_organization.py` & `otterdog-0.6.0/otterdog/models/github_organization.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/organization_secret.py` & `otterdog-0.6.0/otterdog/models/organization_secret.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/organization_settings.py` & `otterdog-0.6.0/otterdog/models/organization_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,19 @@
             field.name: S(field.name) for field in cls.provider_fields() if not is_unset(data.get(field.name, UNSET))
         }
         return mapping
 
     def get_jsonnet_template_function(self, jsonnet_config: JsonnetConfig, extend: bool) -> str | None:
         return None
 
+    def changes_require_web_ui(self, changes: dict[str, Change]) -> bool:
+        from otterdog.providers.github import is_org_settings_key_retrieved_via_web_ui
+
+        return any(map(lambda key: is_org_settings_key_retrieved_via_web_ui(key), changes.keys()))
+
     def to_jsonnet(
         self,
         printer: IndentingPrinter,
         jsonnet_config: JsonnetConfig,
         context: PatchContext,
         extend: bool,
         default_object: ModelObject,
```

### Comparing `otterdog-0.5.0b1/otterdog/models/organization_variable.py` & `otterdog-0.6.0/otterdog/models/organization_variable.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/organization_webhook.py` & `otterdog-0.6.0/otterdog/models/organization_webhook.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/organization_workflow_settings.py` & `otterdog-0.6.0/otterdog/models/organization_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repo_ruleset.py` & `otterdog-0.6.0/otterdog/models/repo_ruleset.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repo_secret.py` & `otterdog-0.6.0/otterdog/models/repo_secret.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repo_variable.py` & `otterdog-0.6.0/otterdog/models/repo_variable.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repo_webhook.py` & `otterdog-0.6.0/otterdog/models/repo_webhook.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repo_workflow_settings.py` & `otterdog-0.6.0/otterdog/models/repo_workflow_settings.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/repository.py` & `otterdog-0.6.0/otterdog/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     archived: bool
     allow_forking: bool
     web_commit_signoff_required: bool
     secret_scanning: str
     secret_scanning_push_protection: str
     dependabot_alerts_enabled: bool
     dependabot_security_updates_enabled: bool
+    private_vulnerability_reporting_enabled: bool
 
     gh_pages_build_type: str
     gh_pages_source_branch: str | None
     gh_pages_source_path: str | None
 
     forked_repository: str | None = dataclasses.field(metadata={"model_only": True})
     fork_default_branch_only: bool = dataclasses.field(metadata={"model_only": True})
@@ -111,14 +112,18 @@
 
     _security_properties: ClassVar[list[str]] = [
         "secret_scanning",
         "secret_scanning_push_protection",
         "dependabot_security_updates_enabled",
     ]
 
+    _additional_security_properties: ClassVar[list[str]] = [
+        "private_vulnerability_reporting_enabled",
+    ]
+
     _unavailable_fields_in_archived_repos: ClassVar[set[str]] = {
         "description",
         "homepage",
         "allow_auto_merge",
         "allow_merge_commit",
         "allow_rebase_merge",
         "allow_squash_merge",
@@ -126,14 +131,15 @@
         "delete_branch_on_merge",
         "merge_commit_message",
         "merge_commit_title",
         "squash_merge_commit_message",
         "squash_merge_commit_title",
         "dependabot_alerts_enabled",
         "dependabot_security_updates_enabled",
+        "private_vulnerability_reporting_enabled",
         "secret_scanning",
         "secret_scanning_push_protection",
         "has_issues",
         "has_wiki",
         "has_projects",
     }
 
@@ -401,15 +407,15 @@
     @staticmethod
     def _valid_topic(topic, search=re.compile(r"[^a-z0-9\-]").search):
         return not bool(search(topic))
 
     def include_field_for_diff_computation(self, field: dataclasses.Field) -> bool:
         # private repos don't support security analysis.
         if self.private is True:
-            if field.name in self._security_properties:
+            if field.name in self._security_properties or field.name in self._additional_security_properties:
                 return False
 
         if self.archived is True:
             if field.name in self._unavailable_fields_in_archived_repos:
                 return False
 
         if self.gh_pages_build_type in ["disabled", "workflow"]:
```

### Comparing `otterdog-0.5.0b1/otterdog/models/ruleset.py` & `otterdog-0.6.0/otterdog/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/secret.py` & `otterdog-0.6.0/otterdog/models/secret.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/variable.py` & `otterdog-0.6.0/otterdog/models/variable.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/webhook.py` & `otterdog-0.6.0/otterdog/models/webhook.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/models/workflow_settings.py` & `otterdog-0.6.0/otterdog/models/workflow_settings.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/__init__.py` & `otterdog-0.6.0/otterdog/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/apply.py` & `otterdog-0.6.0/otterdog/operations/apply.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/canonical_diff.py` & `otterdog-0.6.0/otterdog/operations/canonical_diff.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/delete_file.py` & `otterdog-0.6.0/otterdog/operations/delete_file.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/diff_operation.py` & `otterdog-0.6.0/otterdog/operations/diff_operation.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/dispatch_workflow.py` & `otterdog-0.6.0/otterdog/operations/dispatch_workflow.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/fetch_config.py` & `otterdog-0.6.0/otterdog/operations/fetch_config.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/import_configuration.py` & `otterdog-0.6.0/otterdog/operations/import_configuration.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/list_apps.py` & `otterdog-0.6.0/otterdog/operations/list_apps.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/list_members.py` & `otterdog-0.6.0/otterdog/operations/list_members.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/local_plan.py` & `otterdog-0.6.0/otterdog/operations/local_plan.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/plan.py` & `otterdog-0.6.0/otterdog/operations/plan.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/push_config.py` & `otterdog-0.6.0/otterdog/operations/push_config.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/show.py` & `otterdog-0.6.0/otterdog/operations/show.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/show_default.py` & `otterdog-0.6.0/otterdog/operations/show_default.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/show_live.py` & `otterdog-0.6.0/otterdog/operations/show_live.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/sync_template.py` & `otterdog-0.6.0/otterdog/operations/sync_template.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/validate.py` & `otterdog-0.6.0/otterdog/operations/validate.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/operations/web_login.py` & `otterdog-0.6.0/otterdog/operations/web_login.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/__init__.py` & `otterdog-0.6.0/otterdog/providers/github/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,30 @@
 
 from .graphql import GraphQLClient
 from .rest import RestApi
 from .web import WebClient
 
 _ORG_SETTINGS_SCHEMA = json.loads(files(resources).joinpath("schemas/settings.json").read_text())
 
+# collect supported rest api keys
+_SETTINGS_RESTAPI_KEYS = {k for k, v in _ORG_SETTINGS_SCHEMA["properties"].items() if v.get("provider") == "restapi"}
+# collect supported web interface keys
+_SETTINGS_WEB_KEYS = {k for k, v in _ORG_SETTINGS_SCHEMA["properties"].items() if v.get("provider") == "web"}
+# TODO: make this cleaner
+_SETTINGS_WEB_KEYS.add("discussion_source_repository_id")
+
+
+def is_org_settings_key_retrieved_via_web_ui(key: str) -> bool:
+    return key in _SETTINGS_WEB_KEYS
+
 
 class GitHubProvider:
     def __init__(self, credentials: Credentials | None):
         self._credentials = credentials
 
-        self._settings_schema = _ORG_SETTINGS_SCHEMA
-        # collect supported rest api keys
-        self._settings_restapi_keys = {
-            k for k, v in self._settings_schema["properties"].items() if v.get("provider") == "restapi"
-        }
-
-        # collect supported web interface keys
-        self._settings_web_keys = {
-            k for k, v in self._settings_schema["properties"].items() if v.get("provider") == "web"
-        }
-        # TODO: make this cleaner
-        self._settings_web_keys.add("discussion_source_repository_id")
-
         if credentials is not None:
             self._init_clients()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exception_type, exception_value, exception_traceback):
@@ -69,21 +67,21 @@
         content: str,
         message: str | None = None,
     ) -> bool:
         return await self.rest_api.content.update_content(org_id, repo_name, path, content, message)
 
     async def get_org_settings(self, org_id: str, included_keys: set[str], no_web_ui: bool) -> dict[str, Any]:
         # first, get supported settings via the rest api.
-        required_rest_keys = {x for x in included_keys if x in self._settings_restapi_keys}
+        required_rest_keys = {x for x in included_keys if x in _SETTINGS_RESTAPI_KEYS}
         merged_settings = await self.rest_api.org.get_settings(org_id, required_rest_keys)
 
         # second, get settings only accessible via the web interface and merge
         # them with the other settings, unless --no-web-ui is specified.
         if not no_web_ui:
-            required_web_keys = {x for x in included_keys if x in self._settings_web_keys}
+            required_web_keys = {x for x in included_keys if x in _SETTINGS_WEB_KEYS}
             if len(required_web_keys) > 0:
                 web_settings = await self.web_client.get_org_settings(org_id, required_web_keys)
                 merged_settings.update(web_settings)
 
             utils.print_trace(f"merged org settings = {merged_settings}")
 
         return merged_settings
@@ -91,17 +89,17 @@
     async def update_org_settings(self, org_id: str, settings: dict[str, Any]) -> None:
         rest_fields = {}
         web_fields = {}
 
         # split up settings to be updated whether they need be updated
         # via rest api or web interface.
         for k, v in sorted(settings.items()):
-            if k in self._settings_restapi_keys:
+            if k in _SETTINGS_RESTAPI_KEYS:
                 rest_fields[k] = v
-            elif k in self._settings_web_keys:
+            elif k in _SETTINGS_WEB_KEYS:
                 web_fields[k] = v
             else:
                 utils.print_warn(f"encountered unknown field '{k}' during update, ignoring")
 
         # update any settings via the rest api
         if len(rest_fields) > 0:
             await self.rest_api.org.update_settings(org_id, rest_fields)
```

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/auth/__init__.py` & `otterdog-0.6.0/otterdog/providers/github/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/auth/app.py` & `otterdog-0.6.0/otterdog/providers/github/auth/app.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/auth/token.py` & `otterdog-0.6.0/otterdog/providers/github/auth/token.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/cache/__init__.py` & `otterdog-0.6.0/otterdog/providers/github/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/cache/file.py` & `otterdog-0.6.0/otterdog/providers/github/cache/file.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/cache/redis.py` & `otterdog-0.6.0/otterdog/providers/github/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/exception.py` & `otterdog-0.6.0/otterdog/providers/github/exception.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/graphql.py` & `otterdog-0.6.0/otterdog/providers/github/graphql.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/__init__.py` & `otterdog-0.6.0/otterdog/providers/github/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/app_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/app_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/commit_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/commit_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,35 @@
 #  This program and the accompanying materials are made available
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
 import json
+from typing import Any
 
+from otterdog.providers.github.exception import GitHubException
 from otterdog.utils import print_debug
 
 from . import RestApi, RestClient
 
 
 class CommitClient(RestClient):
     def __init__(self, rest_api: RestApi):
         super().__init__(rest_api)
 
+    async def get_commit_statuses(self, org_id: str, repo_name: str, ref: str) -> list[dict[str, Any]]:
+        print_debug(f"getting commit statuses for ref '{ref}' from repo '{org_id}/{repo_name}'")
+
+        try:
+            return await self.requester.request_paged_json("GET", f"/repos/{org_id}/{repo_name}/commits/{ref}/statuses")
+        except GitHubException as ex:
+            tb = ex.__traceback__
+            raise RuntimeError(f"failed retrieving commit statuses:\n{ex}").with_traceback(tb)
+
     async def create_commit_status(
         self,
         org_id: str,
         repo_name: str,
         sha: str,
         state: str,
         context: str,
```

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/content_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/content_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/issue_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/issue_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/org_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/org_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/repo_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/repo_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,17 +33,26 @@
         super().__init__(rest_api)
 
     async def get_repo_data(self, org_id: str, repo_name: str) -> dict[str, Any]:
         print_debug(f"retrieving org repo data for '{org_id}/{repo_name}'")
 
         try:
             repo_data = await self.requester.request_json("GET", f"/repos/{org_id}/{repo_name}")
+
+            archived = repo_data.get("archived", False)
+            if not archived:
+                await self._fill_vulnerability_alerts(org_id, repo_name, repo_data)
+
+                private = repo_data.get("private", False)
+                if not private:
+                    await self._fill_private_vulnerability_reporting(org_id, repo_name, repo_data)
+
             await self._fill_github_pages_config(org_id, repo_name, repo_data)
-            await self._fill_vulnerability_report(org_id, repo_name, repo_data)
             await self._fill_topics(org_id, repo_name, repo_data)
+
             return repo_data
         except GitHubException as ex:
             tb = ex.__traceback__
             raise RuntimeError(f"failed retrieving data for repo '{repo_name}':\n{ex}").with_traceback(tb)
 
     async def get_repo_by_id(self, repo_id: int) -> dict[str, Any]:
         print_debug(f"retrieving repo by id for '{repo_id}'")
@@ -56,17 +65,22 @@
 
     async def update_repo(self, org_id: str, repo_name: str, data: dict[str, Any]) -> None:
         print_debug(f"updating repo settings for repo '{org_id}/{repo_name}'")
 
         changes = len(data)
 
         if "dependabot_alerts_enabled" in data:
-            vulnerability_reports = bool(data.pop("dependabot_alerts_enabled"))
+            vulnerability_alerts = bool(data.pop("dependabot_alerts_enabled"))
+        else:
+            vulnerability_alerts = None
+
+        if "private_vulnerability_reporting_enabled" in data:
+            private_vulnerability_reporting = bool(data.pop("private_vulnerability_reporting_enabled"))
         else:
-            vulnerability_reports = None
+            private_vulnerability_reporting = None
 
         if "topics" in data:
             topics = list(data.pop("topics"))
         else:
             topics = None
 
         if "gh_pages" in data:
@@ -80,16 +94,20 @@
             default_branch = None
 
         if changes > 0:
             try:
                 if len(data) > 0:
                     await self.requester.request_json("PATCH", f"/repos/{org_id}/{repo_name}", data)
 
-                if vulnerability_reports is not None:
-                    await self._update_vulnerability_report(org_id, repo_name, vulnerability_reports)
+                if vulnerability_alerts is not None:
+                    await self._update_vulnerability_alerts(org_id, repo_name, vulnerability_alerts)
+                if private_vulnerability_reporting is not None:
+                    await self._update_private_vulnerability_reporting(
+                        org_id, repo_name, private_vulnerability_reporting
+                    )
                 if topics is not None:
                     await self._update_topics(org_id, repo_name, topics)
                 if gh_pages is not None:
                     await self._update_github_pages_config(org_id, repo_name, gh_pages)
                 if default_branch is not None:
                     await self._update_default_branch(org_id, repo_name, default_branch)
 
@@ -474,37 +492,66 @@
                 print_debug(f"renamed default branch for '{org_id}/{repo_name}'")
         except GitHubException as ex:
             tb = ex.__traceback__
             raise RuntimeError(
                 f"failed to update default branch for repo '{org_id}/{repo_name}':\n{ex}"
             ).with_traceback(tb)
 
-    async def _fill_vulnerability_report(self, org_id: str, repo_name: str, repo_data: dict[str, Any]) -> None:
-        print_debug(f"retrieving repo vulnerability report status for '{org_id}/{repo_name}'")
+    async def _fill_vulnerability_alerts(self, org_id: str, repo_name: str, repo_data: dict[str, Any]) -> None:
+        print_debug(f"retrieving repo vulnerability alerts for '{org_id}/{repo_name}'")
 
         status, _ = await self.requester.request_raw("GET", f"/repos/{org_id}/{repo_name}/vulnerability-alerts")
         if status == 204:
             repo_data["dependabot_alerts_enabled"] = True
         else:
             repo_data["dependabot_alerts_enabled"] = False
 
-    async def _update_vulnerability_report(self, org_id: str, repo_name: str, vulnerability_reports: bool) -> None:
-        print_debug(f"updating repo vulnerability report status for '{org_id}/{repo_name}'")
+    async def _update_vulnerability_alerts(self, org_id: str, repo_name: str, vulnerability_reports: bool) -> None:
+        print_debug(f"updating repo vulnerability alerts for '{org_id}/{repo_name}'")
 
         if vulnerability_reports is True:
             method = "PUT"
         else:
             method = "DELETE"
 
         status, body = await self.requester.request_raw(method, f"/repos/{org_id}/{repo_name}/vulnerability-alerts")
 
         if status != 204:
-            raise RuntimeError(f"failed to update vulnerability_reports for repo '{repo_name}': {body}")
+            raise RuntimeError(f"failed to update vulnerability alerts for repo '{repo_name}': {body}")
+
+        print_debug(f"updated vulnerability alerts for repo '{repo_name}'")
+
+    async def _fill_private_vulnerability_reporting(
+        self, org_id: str, repo_name: str, repo_data: dict[str, Any]
+    ) -> None:
+        print_debug(f"retrieving repo private vulnerability reporting status for '{org_id}/{repo_name}'")
+
+        response = await self.requester.request_json(
+            "GET", f"/repos/{org_id}/{repo_name}/private-vulnerability-reporting"
+        )
+        repo_data["private_vulnerability_reporting_enabled"] = response["enabled"]
+
+    async def _update_private_vulnerability_reporting(
+        self, org_id: str, repo_name: str, private_vulnerability_reporting_enabled: bool
+    ) -> None:
+        print_debug(f"updating repo private vulnerability reporting for '{org_id}/{repo_name}'")
+
+        if private_vulnerability_reporting_enabled is True:
+            method = "PUT"
+        else:
+            method = "DELETE"
+
+        status, body = await self.requester.request_raw(
+            method, f"/repos/{org_id}/{repo_name}/private-vulnerability-reporting"
+        )
+
+        if status != 204:
+            raise RuntimeError(f"failed to update private vulnerability reporting for repo '{repo_name}': {body}")
 
-        print_debug(f"updated vulnerability_reports for repo '{repo_name}'")
+        print_debug(f"updated private vulnerability reporting for repo '{repo_name}'")
 
     async def _fill_topics(self, org_id: str, repo_name: str, repo_data: dict[str, Any]) -> None:
         print_debug(f"retrieving repo topics for '{org_id}/{repo_name}'")
 
         try:
             response = await self.requester.request_json("GET", f"/repos/{org_id}/{repo_name}/topics")
             repo_data["topics"] = response.get("names", [])
@@ -518,15 +565,15 @@
         await self.requester.request_json("PUT", f"/repos/{org_id}/{repo_name}/topics", data=data)
         print_debug(f"updated topics for repo '{repo_name}'")
 
     async def get_branches(self, org_id: str, repo_name) -> list[dict[str, Any]]:
         print_debug(f"retrieving branches for repo '{org_id}/{repo_name}'")
 
         try:
-            return await self.requester.request_json("GET", f"/repos/{org_id}/{repo_name}/branches")
+            return await self.requester.request_paged_json("GET", f"/repos/{org_id}/{repo_name}/branches")
         except GitHubException as ex:
             tb = ex.__traceback__
             raise RuntimeError(f"failed getting branches for repo '{org_id}/{repo_name}':\n{ex}").with_traceback(tb)
 
     async def get_environments(self, org_id: str, repo_name: str) -> list[dict[str, Any]]:
         print_debug(f"retrieving environments for repo '{org_id}/{repo_name}'")
```

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/requester.py` & `otterdog-0.6.0/otterdog/providers/github/rest/requester.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/team_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/team_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/rest/user_client.py` & `otterdog-0.6.0/otterdog/providers/github/rest/user_client.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/stats/__init__.py` & `otterdog-0.6.0/otterdog/providers/github/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/providers/github/web.py` & `otterdog-0.6.0/otterdog/providers/github/web.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/github-web-settings.jsonnet` & `otterdog-0.6.0/otterdog/resources/github-web-settings.jsonnet`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/graphql/get-branch-protection-rules.gql` & `otterdog-0.6.0/otterdog/resources/graphql/get-branch-protection-rules.gql`

 * *Files 1% similar despite different names*

```diff
@@ -125,11 +125,8 @@
       }
       pageInfo {
         hasNextPage
         endCursor
       }
     }
   }
-  rateLimit {
-    cost
-  }
 }
```

### Comparing `otterdog-0.5.0b1/otterdog/resources/graphql/get-bypass-force-push-allowances.gql` & `otterdog-0.6.0/otterdog/resources/graphql/get-bypass-force-push-allowances.gql`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/graphql/get-bypass-pull-request-allowances.gql` & `otterdog-0.6.0/otterdog/resources/graphql/get-bypass-pull-request-allowances.gql`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/graphql/get-push-allowances.gql` & `otterdog-0.6.0/otterdog/resources/graphql/get-push-allowances.gql`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/graphql/get-review-dismissal-allowances.gql` & `otterdog-0.6.0/otterdog/resources/graphql/get-review-dismissal-allowances.gql`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/branch-protection-rule.json` & `otterdog-0.6.0/otterdog/resources/schemas/branch-protection-rule.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/org-workflow-settings.json` & `otterdog-0.6.0/otterdog/resources/schemas/org-workflow-settings.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/organization.json` & `otterdog-0.6.0/otterdog/resources/schemas/organization.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/repo-workflow-settings.json` & `otterdog-0.6.0/otterdog/resources/schemas/repo-workflow-settings.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/repository-ruleset.json` & `otterdog-0.6.0/otterdog/resources/schemas/repository-ruleset.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/repository.json` & `otterdog-0.6.0/otterdog/resources/schemas/repository.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981481481481481%*

 * *Differences: {"'properties'": "{'private_vulnerability_reporting_enabled': OrderedDict([('type', 'boolean')])}"}*

```diff
@@ -118,14 +118,17 @@
                 "type": "string"
             },
             "type": "array"
         },
         "private": {
             "type": "boolean"
         },
+        "private_vulnerability_reporting_enabled": {
+            "type": "boolean"
+        },
         "rulesets": {
             "items": {
                 "$ref": "repository-ruleset.json"
             },
             "type": "array"
         },
         "secret_scanning": {
```

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/settings.json` & `otterdog-0.6.0/otterdog/resources/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/resources/schemas/webhook.json` & `otterdog-0.6.0/otterdog/resources/schemas/webhook.json`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/utils.py` & `otterdog-0.6.0/otterdog/utils.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/webapp/config.py` & `otterdog-0.6.0/otterdog/webapp/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 class AppConfig:
     QUART_APP = "otterdog.webapp"
 
     # Assets Management
     ASSETS_ROOT = config("ASSETS_ROOT", default="/static/assets")
 
+    CACHE_CONTROL = config("CACHE_CONTROL", default=False)
+
     APP_ROOT = config("APP_ROOT")
     DB_ROOT = os.path.join(APP_ROOT, "db")
 
     MONGO_URI = config("MONGO_URI", default="mongodb://mongodb:27017/otterdog")
     REDIS_URI = config("REDIS_URI", default="redis://redis:6379")
 
     OTTERDOG_CONFIG_OWNER = config("OTTERDOG_CONFIG_OWNER", default=None)
@@ -31,20 +33,24 @@
     OTTERDOG_CONFIG_TOKEN = config("OTTERDOG_CONFIG_TOKEN", default=None)
 
     # Set up the App SECRET_KEY
     SECRET_KEY = config("SECRET_KEY", default=None)
     if not SECRET_KEY:
         SECRET_KEY = "".join(random.choice(string.ascii_lowercase) for i in range(32))
 
-    GITHUB_ADMIN_TEAM = config("GITHUB_ADMIN_TEAM", default="otterdog-admins")
+    GITHUB_ADMIN_TEAMS = config("GITHUB_ADMIN_TEAMS", default="otterdog-admins")
     GITHUB_WEBHOOK_ENDPOINT = config("GITHUB_WEBHOOK_ENDPOINT", default="/github-webhook/receive")
     GITHUB_WEBHOOK_SECRET = config("GITHUB_WEBHOOK_SECRET", default=None)
     GITHUB_WEBHOOK_VALIDATION_CONTEXT = config("GITHUB_WEBHOOK_VALIDATION_CONTEXT", default="otterdog-validate")
     GITHUB_WEBHOOK_SYNC_CONTEXT = config("GITHUB_WEBHOOK_SYNC_CONTEXT", default="otterdog-sync")
 
+    # GitHub OAuth config
+    GITHUB_CLIENT_ID = config("GITHUB_OAUTH_CLIENT_ID")
+    GITHUB_CLIENT_SECRET = config("GITHUB_OAUTH_CLIENT_SECRET")
+
     # GitHub App config
     GITHUB_APP_ID = config("GITHUB_APP_ID")
     GITHUB_APP_PRIVATE_KEY = config("GITHUB_APP_PRIVATE_KEY")
 
 
 class ProductionConfig(AppConfig):
     DEBUG = False
@@ -54,10 +60,12 @@
     REMEMBER_COOKIE_HTTPONLY = True
     REMEMBER_COOKIE_DURATION = 3600
 
 
 class DebugConfig(AppConfig):
     DEBUG = True
 
+    TEMPLATES_AUTO_RELOAD = True
+
 
 # Load all possible configurations
 config_dict = {"Production": ProductionConfig, "Debug": DebugConfig}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/db/__init__.py` & `otterdog-0.6.0/otterdog/webapp/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,20 @@
 async def init_mongo_database(mongo: Mongo) -> None:
     from .models import (
         ConfigurationModel,
         InstallationModel,
         PullRequestModel,
         StatisticsModel,
         TaskModel,
+        UserModel,
     )
 
     await mongo.odm.configure_database(
         [
             InstallationModel,
             TaskModel,
             ConfigurationModel,
             PullRequestModel,
             StatisticsModel,
+            UserModel,
         ]  # type: ignore
     )
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/db/models.py` & `otterdog-0.6.0/otterdog/webapp/db/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Optional
 
-from odmantic import Field, Index, Model
+from odmantic import EmbeddedModel, Field, Model
 
 from otterdog.webapp.utils import current_utc_time
 
 
 class InstallationStatus(str, Enum):
     INSTALLED = "installed"
     NOT_INSTALLED = "not_installed"
@@ -33,25 +33,26 @@
     installation_status: InstallationStatus
     config_repo: Optional[str] = None
     base_template: Optional[str] = None
 
 
 class TaskStatus(str, Enum):
     CREATED = "created"
+    SCHEDULED = "scheduled"
     FINISHED = "finished"
     FAILED = "failed"
 
     def __str__(self) -> str:
         return self.name
 
 
 class TaskModel(Model):
-    type: str
-    org_id: str
-    repo_name: str
+    type: str = Field(index=True)
+    org_id: str = Field(index=True)
+    repo_name: str = Field(index=True)
     pull_request: int = 0
     status: TaskStatus = TaskStatus.CREATED
     log: Optional[str] = None
     cache_stats: str = ""
     rate_limit_remaining: str = ""
     created_at: datetime = Field(index=True, default_factory=current_utc_time)
     updated_at: datetime = Field(default_factory=current_utc_time)
@@ -79,41 +80,59 @@
     PARTIALLY_APPLIED = "partially_applied"
     COMPLETED = "completed"
 
     def __str__(self) -> str:
         return self.name
 
 
-class PullRequestModel(Model):
+class PullRequestId(EmbeddedModel):
     org_id: str
     repo_name: str
     pull_request: int
+
+
+class PullRequestModel(Model):
+    id: PullRequestId = Field(primary_field=True)
     draft: bool
     status: PullRequestStatus = Field(index=True)
     apply_status: ApplyStatus = Field(index=True, default=ApplyStatus.NOT_APPLIED)
 
     valid: Optional[bool] = None
     in_sync: Optional[bool] = None
-    requires_manual_apply: bool = False
+    requires_manual_apply: Optional[bool] = None
+    supports_auto_merge: Optional[bool] = None
+    author_can_auto_merge: Optional[bool] = None
+    has_required_approvals: Optional[bool] = None
 
     created_at: datetime = Field(index=True)
     updated_at: datetime = Field(index=True)
 
     closed_at: Optional[datetime] = None
     merged_at: Optional[datetime] = Field(index=True, default=None)
 
-    model_config = {  # type: ignore
-        "indexes": lambda: [
-            Index(
-                PullRequestModel.org_id,
-                PullRequestModel.repo_name,
-                PullRequestModel.pull_request,
-                unique=True,
-            ),
-        ],
-    }
+    def can_be_automerged(self) -> bool:
+        return (
+            self.valid is True
+            and self.in_sync is True
+            and self.supports_auto_merge is True
+            and (self.author_can_auto_merge is True or self.has_required_approvals is True)
+        )
 
 
 class StatisticsModel(Model):
     project_name: str = Field(primary_field=True)
     github_id: str = Field(index=True)
-    num_repos: int
+    two_factor_enforced: int
+    total_repos: int
+    archived_repos: int
+    repos_with_secret_scanning: int
+    repos_with_secret_scanning_push_protection: int
+    repos_with_branch_protection: int
+    repos_with_private_vulnerability_reporting: int
+
+
+class UserModel(Model):
+    node_id: str = Field(primary_field=True)
+    username: str
+    email: Optional[str] = None
+    full_name: Optional[str] = None
+    projects: list[str] = Field(default_factory=list)
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/db/service.py` & `otterdog-0.6.0/otterdog/webapp/db/service.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
 from __future__ import annotations
 
+import dataclasses
 from logging import getLogger
 
 from odmantic import query
 from odmantic.query import QueryExpression
 from quart import current_app
 
 from otterdog.config import OtterdogConfig
@@ -20,33 +21,43 @@
 from otterdog.webapp.webhook.github_models import PullRequest
 
 from .models import (
     ApplyStatus,
     ConfigurationModel,
     InstallationModel,
     InstallationStatus,
+    PullRequestId,
     PullRequestModel,
     PullRequestStatus,
     StatisticsModel,
     TaskModel,
     TaskStatus,
+    UserModel,
 )
 
 logger = getLogger(__name__)
 
 
 async def update_installation_status(installation_id: int, action: str) -> None:
     logger.info(f"updating installation status for installation with id '{installation_id}': {action}")
 
     match action:
         case "created":
             await update_app_installations()
 
         case "deleted":
-            await update_app_installations()
+            installation = await mongo.odm.find_one(
+                InstallationModel, InstallationModel.installation_id == installation_id
+            )
+
+            if installation is not None:
+                installation.installation_id = 0
+                installation.installation_status = InstallationStatus.NOT_INSTALLED
+                await mongo.odm.save(installation)
+                await cleanup_data()
 
         case "suspend":
             installation = await mongo.odm.find_one(
                 InstallationModel, InstallationModel.installation_id == installation_id
             )
 
             if installation is not None:
@@ -104,21 +115,25 @@
                 existing_installations.remove(github_id)
 
         # remove all remaining installations which are not present in the otterdog config
         for github_id in existing_installations:
             await session.remove(InstallationModel, InstallationModel.github_id == github_id)
 
     # remove all PullRequest and Statistics data for invalid installations
+    await cleanup_data()
+
+    await update_app_installations()
+
+
+async def cleanup_data() -> None:
     valid_orgs = list(map(lambda x: x.github_id, await get_installations()))
     await cleanup_pull_requests(valid_orgs)
     await cleanup_statistics(valid_orgs)
     await cleanup_configurations(valid_orgs)
 
-    await update_app_installations()
-
 
 async def update_app_installations() -> None:
     logger.info("updating app installations")
 
     rest_api = get_rest_api_for_app()
     all_installations = await rest_api.app.get_app_installations()
 
@@ -248,57 +263,80 @@
     await mongo.odm.remove(ConfigurationModel, query.not_in(ConfigurationModel.github_id, valid_orgs))
 
 
 async def create_task(task: TaskModel) -> None:
     await mongo.odm.save(task)
 
 
+async def schedule_task(task: TaskModel) -> None:
+    task.status = TaskStatus.SCHEDULED
+    await mongo.odm.save(task)
+
+
 async def finish_task(task: TaskModel) -> None:
     task.status = TaskStatus.FINISHED
     task.updated_at = current_utc_time()
     await mongo.odm.save(task)
 
 
 async def fail_task(task: TaskModel, exception: Exception) -> None:
     task.status = TaskStatus.FAILED
     task.updated_at = current_utc_time()
     task.log = str(exception)
     await mongo.odm.save(task)
 
 
+async def get_latest_sync_or_apply_task_for_organization(org_id: str, repo_name: str) -> TaskModel | None:
+    tasks = await mongo.odm.find(
+        TaskModel,
+        query.or_(TaskModel.type == "CheckConfigurationInSyncTask", TaskModel.type == "ApplyChangesTask"),
+        TaskModel.status != TaskStatus.CREATED,
+        TaskModel.org_id == org_id,
+        TaskModel.repo_name == repo_name,
+        sort=query.desc(TaskModel.created_at),
+        limit=1,
+    )
+
+    if len(tasks) == 1:
+        return tasks[0]
+    else:
+        return None
+
+
 async def save_config(config: ConfigurationModel) -> None:
     await mongo.odm.save(config)
 
 
 async def find_pull_request(owner: str, repo: str, pull_request: int) -> PullRequestModel | None:
     return await mongo.odm.find_one(
         PullRequestModel,
-        PullRequestModel.org_id == owner,
-        PullRequestModel.repo_name == repo,
-        PullRequestModel.pull_request == pull_request,
+        PullRequestModel.id.org_id == owner,
+        PullRequestModel.id.repo_name == repo,
+        PullRequestModel.id.pull_request == pull_request,
     )
 
 
 async def update_or_create_pull_request(
     owner: str,
     repo: str,
     pull_request: PullRequest,
     valid: bool | None = None,
     in_sync: bool | None = None,
     requires_manual_apply: bool | None = None,
+    supports_auto_merge: bool | None = None,
+    author_can_auto_merge: bool | None = None,
+    has_required_approvals: bool | None = None,
     apply_status: ApplyStatus | None = None,
-) -> None:
+) -> PullRequestModel:
     pull_request_status = PullRequestStatus[pull_request.get_pr_status()]
 
     pr_model = await find_pull_request(owner, repo, pull_request.number)
     if pr_model is None:
         pr_model = PullRequestModel(  # type: ignore
-            org_id=owner,
-            repo_name=repo,
-            pull_request=pull_request.number,
+            id=PullRequestId(org_id=owner, repo_name=repo, pull_request=pull_request.number),
             draft=pull_request.draft,
             status=pull_request_status,
             created_at=pull_request.created_at,
             updated_at=pull_request.updated_at,
             closed_at=pull_request.closed_at,
             merged_at=pull_request.merged_at,
         )
@@ -318,15 +356,25 @@
 
     if in_sync is not None:
         pr_model.in_sync = in_sync
 
     if requires_manual_apply is not None:
         pr_model.requires_manual_apply = requires_manual_apply
 
+    if supports_auto_merge is not None:
+        pr_model.supports_auto_merge = supports_auto_merge
+
+    if author_can_auto_merge is not None:
+        pr_model.author_can_auto_merge = author_can_auto_merge
+
+    if has_required_approvals is not None:
+        pr_model.has_required_approvals = has_required_approvals
+
     await update_pull_request(pr_model)
+    return pr_model
 
 
 async def update_pull_request(pull_request: PullRequestModel) -> None:
     await mongo.odm.save(pull_request)
 
 
 async def get_open_or_incomplete_pull_requests() -> list[PullRequestModel]:
@@ -366,38 +414,47 @@
         PullRequestModel.apply_status == ApplyStatus.COMPLETED,
     )
 
 
 async def get_merged_pull_requests_paged(params: dict[str, str]) -> tuple[list[PullRequestModel], int]:
     page_index = 1
     page_size = 20
-    sort_field = "merged_at"
+    sort_field_name = "merged_at"
     sort_order = "desc"
 
     queries: list[QueryExpression] = [_merged_pull_requests_query()]
 
     for k, v in params.items():
         match k:
             case "pageIndex":
                 page_index = int(v)
             case "pageSize":
                 page_size = int(v)
             case "sortField":
-                sort_field = v
+                sort_field_name = v
             case "sortOrder":
                 sort_order = v
             case _:
                 if v:
                     queries.append(query.match(PullRequestModel.__dict__[k], v))
 
-    sort = (
-        query.desc(PullRequestModel.__dict__[sort_field])
-        if sort_order == "desc"
-        else query.asc(PullRequestModel.__dict__[sort_field])
-    )
+    if sort_field_name.startswith("id."):
+        match sort_field_name:
+            case "id.org_id":
+                sort_field = PullRequestModel.id.org_id
+            case "id.repo_name":
+                sort_field = PullRequestModel.id.repo_name
+            case "id.pull_request":
+                sort_field = PullRequestModel.id.pull_request  # type: ignore
+            case _:
+                raise RuntimeError(f"unexpected sort field '{sort_field_name}'")
+    else:
+        sort_field = PullRequestModel.__dict__[sort_field_name]
+
+    sort = query.desc(sort_field) if sort_order == "desc" else query.asc(sort_field)
 
     skip = (page_index - 1) * page_size
     return (
         await mongo.odm.find(
             PullRequestModel,
             *queries,
             skip=skip,
@@ -405,36 +462,75 @@
             sort=sort,
         ),
         await mongo.odm.count(PullRequestModel, *queries),
     )
 
 
 async def cleanup_pull_requests(valid_orgs: list[str]) -> None:
-    await mongo.odm.remove(PullRequestModel, query.not_in(PullRequestModel.org_id, valid_orgs))
+    await mongo.odm.remove(PullRequestModel, query.not_in(PullRequestModel.id.org_id, valid_orgs))
 
 
 async def save_statistics(model: StatisticsModel) -> None:
     await mongo.odm.save(model)
 
 
-async def get_statistics() -> tuple[int, int]:
+@dataclasses.dataclass(frozen=True)
+class Statistics:
+    total_projects: int = 0
+    projects_with_two_factor_auth_enforced: int = 0
+    total_repos: int = 0
+    archived_repos: int = 0
+    repos_with_branch_protection: int = 0
+    repos_with_secret_scanning: int = 0
+    repos_with_secret_scanning_and_protection: int = 0
+    repos_with_private_vulnerability_reporting: int = 0
+
+    @property
+    def active_repos(self) -> int:
+        return self.total_repos - self.archived_repos
+
+
+async def get_statistics() -> Statistics:
     pipeline = [
         {
             "$group": {
                 "_id": None,
-                "num_projects": {"$sum": 1},
-                "num_repos": {"$sum": "$num_repos"},
+                "total_projects": {"$sum": 1},
+                "two_factor_enforced": {"$sum": "$two_factor_enforced"},
+                "total_repos": {"$sum": "$total_repos"},
+                "archived_repos": {"$sum": "$archived_repos"},
+                "repos_with_branch_protection": {"$sum": "$repos_with_branch_protection"},
+                "repos_with_secret_scanning": {"$sum": "$repos_with_secret_scanning"},
+                "repos_with_secret_scanning_push_protection": {"$sum": "$repos_with_secret_scanning_push_protection"},
+                "repos_with_private_vulnerability_reporting": {"$sum": "$repos_with_private_vulnerability_reporting"},
             },
         }
     ]
 
     collection = mongo.odm.get_collection(StatisticsModel)
     stats_list = await collection.aggregate(pipeline).to_list(1)
     if stats_list is None or len(stats_list) == 0:
-        return 0, 0
+        return Statistics()
     else:
         stats = stats_list[0]
-        return stats["num_projects"], stats["num_repos"]
+        return Statistics(
+            stats["total_projects"],
+            stats["two_factor_enforced"],
+            stats["total_repos"],
+            stats["archived_repos"],
+            stats["repos_with_branch_protection"],
+            stats["repos_with_secret_scanning"],
+            stats["repos_with_secret_scanning_push_protection"],
+            stats["repos_with_private_vulnerability_reporting"],
+        )
 
 
 async def cleanup_statistics(valid_orgs: list[str]) -> None:
     await mongo.odm.remove(StatisticsModel, query.not_in(StatisticsModel.github_id, valid_orgs))
+
+
+async def get_user(node_id: str) -> UserModel | None:
+    return await mongo.odm.find_one(UserModel, UserModel.node_id == node_id)
+
+
+async def save_user(user: UserModel) -> None:
+    await mongo.odm.save(user)
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/filters.py` & `otterdog-0.6.0/otterdog/webapp/filters.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/webapp/home/routes.py` & `otterdog-0.6.0/otterdog/webapp/home/routes.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,30 @@
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
 import json
 from typing import Any
 
-from quart import redirect, render_template, request, url_for
+from quart import (
+    current_app,
+    redirect,
+    render_template,
+    request,
+    send_from_directory,
+    url_for,
+)
+from quart_auth import current_user, login_required
 from werkzeug.routing import BuildError
 
 from otterdog.models.github_organization import GitHubOrganization
 from otterdog.utils import associate_by_key
 from otterdog.webapp.db.service import (
     get_active_installations,
+    get_configuration_by_github_id,
     get_configuration_by_project_name,
     get_configurations,
     get_installations,
     get_merged_pull_requests_count,
     get_open_or_incomplete_pull_requests,
     get_open_or_incomplete_pull_requests_count,
     get_statistics,
@@ -29,79 +38,161 @@
 )
 from otterdog.webapp.utils import refresh_otterdog_config
 
 from . import blueprint
 
 
 @blueprint.route("/")
-def route_default():
+async def route_default():
     return redirect(url_for(".index"))
 
 
+@blueprint.route("/robots.txt")
+@blueprint.route("/favicon.ico")
+async def static_from_root():
+    return await send_from_directory(current_app.static_folder, request.path[1:])
+
+
 @blueprint.route("/index")
 async def index():
     installations = await get_installations()
     configurations = await get_configurations()
     configurations_by_key = associate_by_key(configurations, lambda x: x.github_id)
-    statistics = await get_statistics()
+    stats = await get_statistics()
+
+    two_factor_data = [
+        stats.total_projects - stats.projects_with_two_factor_auth_enforced,
+        stats.projects_with_two_factor_auth_enforced,
+    ]
+
+    secret_scanning_data = [
+        stats.active_repos - stats.repos_with_secret_scanning - stats.repos_with_secret_scanning_and_protection,
+        stats.repos_with_secret_scanning,
+        stats.repos_with_secret_scanning_and_protection,
+    ]
+
+    branch_protection_data = [
+        stats.active_repos - stats.repos_with_branch_protection,
+        stats.repos_with_branch_protection,
+    ]
+
+    private_vulnerability_reporting_data = [
+        stats.active_repos - stats.repos_with_private_vulnerability_reporting,
+        stats.repos_with_private_vulnerability_reporting,
+    ]
+
     return await render_home_template(
         "index.html",
         open_pull_request_count=await get_open_or_incomplete_pull_requests_count(),
         merged_pull_request_count=await get_merged_pull_requests_count(),
         installations=installations,
         configurations=configurations_by_key,
-        total_repository_count=statistics[1],
+        total_repository_count=stats.total_repos,
+        active_repository_count=stats.active_repos,
+        archived_repository_count=stats.archived_repos,
+        two_factor_data=json.dumps(two_factor_data),
+        secret_scanning_data=json.dumps(secret_scanning_data),
+        branch_protection_data=json.dumps(branch_protection_data),
+        private_vulnerability_reporting_data=json.dumps(private_vulnerability_reporting_data),
     )
 
 
+@blueprint.route("/myprojects")
+@login_required
+async def myprojects():
+    projects = set(await current_user.projects)
+
+    installations = list(filter(lambda x: x.project_name in projects, await get_installations()))
+    configurations = await get_configurations()
+    configurations_by_key = associate_by_key(configurations, lambda x: x.github_id)
+    return await render_home_template(
+        "projects.html",
+        title="My Projects",
+        installations=installations,
+        configurations=configurations_by_key,
+    )
+
+
+@blueprint.route("/allprojects")
+async def allprojects():
+    installations = await get_installations()
+    configurations = await get_configurations()
+    configurations_by_key = associate_by_key(configurations, lambda x: x.github_id)
+    return await render_home_template(
+        "projects.html",
+        title="All Projects",
+        installations=installations,
+        configurations=configurations_by_key,
+    )
+
+
+@blueprint.route("/query")
+async def query():
+    from otterdog.webapp.api.graphql import type_defs
+
+    return await render_home_template(
+        "query.html",
+        graphql_schema=type_defs,
+    )
+
+
+@blueprint.route("/organizations/<org_name>")
+async def organization(org_name: str):
+    config = await get_configuration_by_github_id(org_name)
+    if config is None:
+        return await render_template("home/page-404.html"), 404
+    else:
+        return redirect(url_for(".project", project_name=config.project_name))
+
+
 @blueprint.route("/projects/<project_name>")
 async def project(project_name: str):
     config = await get_configuration_by_project_name(project_name)
 
     if config is None:
         return await render_template("home/page-404.html"), 404
 
     from otterdog.models.github_organization import GitHubOrganization
 
     github_organization = GitHubOrganization.from_model_data(config.config)
 
     return await render_home_template(
         "organization.html",
-        project_name=project_name,
+        project_name=config.project_name,
         github_id=config.github_id,
         config=github_organization,
         secret_scanning_data=json.dumps(_get_secret_scanning_data(github_organization)),
         branch_protection_data=json.dumps(_get_branch_protection_data(github_organization)),
     )
 
 
-def _get_secret_scanning_data(organization: GitHubOrganization) -> list[int]:
+def _get_secret_scanning_data(org: GitHubOrganization) -> list[int]:
     alert_mode = 0
     protection_mode = 0
     not_configured = 0
 
-    for repo in organization.repositories:
+    for repo in org.repositories:
         if repo.archived is True:
             continue
 
         if repo.secret_scanning_push_protection == "enabled":
             protection_mode += 1
         elif repo.secret_scanning == "enabled":
             alert_mode += 1
         else:
             not_configured += 1
 
     return [not_configured, alert_mode, protection_mode]
 
 
-def _get_branch_protection_data(organization: GitHubOrganization) -> list[int]:
+def _get_branch_protection_data(org: GitHubOrganization) -> list[int]:
     protected = 0
     not_protected = 0
 
-    for repo in organization.repositories:
+    for repo in org.repositories:
         if repo.archived is True:
             continue
 
         if len(repo.rulesets) > 0 or len(repo.branch_protection_rules) > 0:
             protected += 1
         else:
             not_protected += 1
@@ -184,16 +275,24 @@
             endpoint = template.rstrip(".html")
         else:
             endpoint = template
 
         return redirect(url_for(f".{endpoint}"))
     except BuildError:
         return await render_template("home/page-404.html"), 404
-    except:  # noqa: E722
-        return await render_template("home/page-500.html"), 500
+
+
+@blueprint.errorhandler(401)
+async def error_unauthorized(error):
+    return await render_template("home/page-401.html"), 401
+
+
+@blueprint.errorhandler(Exception)
+async def error_exception(error):
+    return await render_template("home/page-500.html"), 500
 
 
 # Helper - Extract current page name from request
 def get_segments(request):
     try:
         segments = request.path.split("/")
 
@@ -213,21 +312,25 @@
     navigation = {}
 
     for installation in installations:
         if installation.project_name is None:
             continue
 
         levels = installation.project_name.split(".")
+
+        # if the project_name is a tlp, e.g. ee4j, add a second level with the same name
+        # to support multiple projects under the same tlp, e.g. ee4j and ee4j.jakartaee-platform,
+        # which will be transformed to ee4j.ee4j.
         if len(levels) == 1:
-            navigation[levels[0]] = installation
-        else:
-            curr = navigation.get(levels[0], {})
-            remainder = "".join(levels[1:])
-            curr.update({remainder: installation})
-            navigation[levels[0]] = curr
+            levels.append(levels[0])
+
+        curr = navigation.get(levels[0], {})
+        remainder = "".join(levels[1:])
+        curr.update({remainder: installation})
+        navigation[levels[0]] = curr
 
     return navigation
 
 
 async def render_home_template(template_name: str, **context: Any) -> str:
     return await render_template(
         f"home/{template_name}",
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/static/assets/favicon.ico` & `otterdog-0.6.0/otterdog/webapp/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/__init__.py` & `otterdog-0.6.0/otterdog/webapp/tasks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 #  Copyright (c) 2023-2024 Eclipse Foundation and others.
 #  This program and the accompanying materials are made available
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
+from __future__ import annotations
+
 import contextlib
 from abc import ABC, abstractmethod
-from collections.abc import AsyncIterator
+from collections.abc import AsyncIterator, Iterable
 from functools import cached_property
 from logging import Logger, getLogger
-from typing import Generic, Protocol, TypeVar
+from typing import Any, Generic, Protocol, TypeVar
 
 import aiofiles
+from quart import current_app
 
 from otterdog.config import OrganizationConfig
 from otterdog.providers.github import GitHubProvider, GraphQLClient
 from otterdog.providers.github.rest import RestApi
 from otterdog.providers.github.stats import RequestStatistics
 from otterdog.webapp.db.models import InstallationModel, TaskModel
 from otterdog.webapp.db.service import (
     create_task,
     fail_task,
     finish_task,
     get_installation,
+    schedule_task,
 )
 from otterdog.webapp.utils import (
     get_graphql_api_for_installation,
     get_rest_api_for_installation,
     get_temporary_base_directory,
 )
 
@@ -49,40 +53,41 @@
     async def execute(self) -> T | None:
         self.logger.debug(f"executing task '{self!r}'")
 
         task_model = self.create_task_model()
         if task_model is not None:
             await create_task(task_model)
 
-        try:
-            await self._pre_execute()
-
-            result = await self._execute()
-            await self._post_execute(result)
-
-            if task_model is not None:
-                self._update_task_model(task_model)
-
-            if task_model is not None:
-                await finish_task(task_model)
+        task_result: Any = None
 
-            return result
+        try:
+            if await self._pre_execute() is True:
+                if task_model is not None:
+                    await schedule_task(task_model)
+
+                result = await self._execute()
+                await self._post_execute(result)
+                task_result = result
         except Exception as ex:
             self.logger.exception(f"failed to execute task '{self!r}'", exc_info=ex)
             await self._post_execute(ex)
-
+            task_result = ex
+        finally:
             if task_model is not None:
-                await fail_task(task_model, ex)
+                self._update_task_model(task_model)
+                if isinstance(task_result, Exception):
+                    await fail_task(task_model, task_result)
+                else:
+                    await finish_task(task_model)
 
-            return None
-        finally:
             await self._cleanup()
+            return task_result
 
-    async def _pre_execute(self) -> None:
-        pass
+    async def _pre_execute(self) -> bool:
+        return True
 
     async def _post_execute(self, result_or_exception: T | Exception) -> None:
         pass
 
     def _update_task_model(self, task: TaskModel) -> None:
         pass
 
@@ -210,14 +215,44 @@
             comment_id = comment["id"]
             body = comment["body"]
             is_minimized = comment["isMinimized"]
 
             if bool(is_minimized) is False and matching_header in body:
                 await graphql_api.minimize_comment(comment_id, "OUTDATED")
 
+    async def comment_with_header_exists(
+        self,
+        org_id: str,
+        repo_name: str,
+        pull_request_number: int,
+        matching_header: str,
+    ):
+        graphql_api = await self.graphql_api
+        comments = await graphql_api.get_issue_comments(org_id, repo_name, pull_request_number)
+        for comment in comments:
+            body = comment["body"]
+            is_minimized = comment["isMinimized"]
+
+            if bool(is_minimized) is False and matching_header in body:
+                return True
+
+        return False
+
+    def schedule_automerge_task(self, org_id: str, repo_name: str, pull_request_number: int) -> None:
+        from .auto_merge_comment import AutoMergeCommentTask
+
+        current_app.add_background_task(
+            AutoMergeCommentTask(
+                self.installation_id,
+                org_id,
+                repo_name,
+                pull_request_number,
+            )
+        )
+
     async def _cleanup(self) -> None:
         if self.__rest_api is not None:
             await self.__rest_api.close()
 
         if self.__graphql_api is not None:
             await self.__graphql_api.close()
 
@@ -231,7 +266,31 @@
         org_model.project_name,
         org_model.github_id,
         org_model.config_repo,
         org_model.base_template,
         {"provider": "inmemory", "api_token": token},
         work_dir,
     )
+
+
+def contains_valid_team_for_approval(teams: Iterable[str]) -> bool:
+    # FIXME: teams that can approve must be made configurable, this is just EF specific for now
+    return any(
+        map(
+            lambda x: x.endswith("project-leads"),
+            teams,
+        )
+    )
+
+
+def contains_eligible_team_for_auto_merge(teams: Iterable[str]) -> bool:
+    from otterdog.webapp.utils import get_admin_teams
+
+    admin_teams = get_admin_teams()
+
+    # FIXME: teams that can approve must be made configurable, this is just EF specific for now
+    return any(
+        map(
+            lambda x: x.endswith("project-leads") or x in admin_teams,
+            teams,
+        )
+    )
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/complete_pull_request.py` & `otterdog-0.6.0/otterdog/webapp/tasks/help_comment.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,65 +6,53 @@
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
 from dataclasses import dataclass
 
 from quart import render_template
 
-from otterdog.webapp.db.models import ApplyStatus, PullRequestStatus, TaskModel
-from otterdog.webapp.db.service import find_pull_request, update_pull_request
+from otterdog.webapp.db.models import TaskModel
 from otterdog.webapp.tasks import InstallationBasedTask, Task
-from otterdog.webapp.utils import get_admin_team
 
 
 @dataclass(repr=False)
-class CompletePullRequestTask(InstallationBasedTask, Task[None]):
+class HelpCommentTask(InstallationBasedTask, Task[None]):
     installation_id: int
     org_id: str
     repo_name: str
     pull_request_number: int
-    author: str
 
     def create_task_model(self):
         return TaskModel(
             type=type(self).__name__,
             org_id=self.org_id,
             repo_name=self.repo_name,
             pull_request=self.pull_request_number,
         )
 
-    async def _pre_execute(self) -> None:
+    async def _execute(self) -> None:
         self.logger.info(
-            "completing pull request #%d on behalf of user '%s' for repo '%s/%s'",
+            "adding help text to pull request #%d of repo '%s/%s'",
             self.pull_request_number,
-            self.author,
             self.org_id,
             self.repo_name,
         )
 
-    async def _execute(self) -> None:
-        pr_model = await find_pull_request(self.org_id, self.repo_name, self.pull_request_number)
-        if pr_model is None:
-            self.logger.warning(f"failed to find data for pull request #%d in repo '{self.org_id}/{self.repo_name}'")
-            return
-
-        if pr_model.status != PullRequestStatus.MERGED:
-            return
-
-        if pr_model.apply_status != ApplyStatus.PARTIALLY_APPLIED and pr_model.apply_status != ApplyStatus.FAILED:
-            return
-
         rest_api = await self.rest_api
-        admin_team = get_admin_team()
-        if not await rest_api.team.is_user_member_of_team(self.org_id, admin_team, self.author):
-            comment = await render_template("comment/wrong_team_done_comment.txt", admin_team=admin_team)
-            await rest_api.issue.create_comment(self.org_id, self.repo_name, str(self.pull_request_number), comment)
-            return
+        comment = await render_template("comment/help_comment.txt")
 
-        pr_model.apply_status = ApplyStatus.COMPLETED
-        await update_pull_request(pr_model)
+        await self.minimize_outdated_comments(
+            self.org_id,
+            self.repo_name,
+            self.pull_request_number,
+            "<!-- Otterdog Comment: help -->",
+        )
 
-        comment = await render_template("comment/done_comment.txt")
-        await rest_api.issue.create_comment(self.org_id, self.repo_name, str(self.pull_request_number), comment)
+        await rest_api.issue.create_comment(
+            self.org_id,
+            self.repo_name,
+            str(self.pull_request_number),
+            comment,
+        )
 
     def __repr__(self) -> str:
-        return f"CompletePullRequestTask(repo={self.org_id}/{self.repo_name}, pull_request=#{self.pull_request_number})"
+        return f"HelpCommentTask(repo='{self.org_id}/{self.repo_name}', pull_request=#{self.pull_request_number})"
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/fetch_all_pull_requests.py` & `otterdog-0.6.0/otterdog/webapp/tasks/fetch_all_pull_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,22 +23,21 @@
     def create_task_model(self):
         return TaskModel(
             type=type(self).__name__,
             org_id=self.org_id,
             repo_name=self.repo_name,
         )
 
-    async def _pre_execute(self) -> None:
+    async def _execute(self) -> None:
         self.logger.info(
             "fetching all pull requests from repo '%s/%s'",
             self.org_id,
             self.repo_name,
         )
 
-    async def _execute(self) -> None:
         rest_api = await self.rest_api
 
         all_pull_requests = await rest_api.pull_request.get_pull_requests(
             self.org_id, self.repo_name, state="all", base_ref="main"
         )
 
         for pr in all_pull_requests:
@@ -52,8 +51,8 @@
                 self.org_id,
                 self.repo_name,
                 pr_from_github,
                 apply_status=apply_status,
             )
 
     def __repr__(self) -> str:
-        return f"FetchAllPullRequestsTask(repo={self.org_id}/{self.repo_name})"
+        return f"FetchAllPullRequestsTask(repo='{self.org_id}/{self.repo_name}')"
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/fetch_config.py` & `otterdog-0.6.0/otterdog/webapp/api/routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,71 +2,78 @@
 #  Copyright (c) 2024 Eclipse Foundation and others.
 #  This program and the accompanying materials are made available
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
-from dataclasses import dataclass
+from ariadne import graphql
+from ariadne.explorer import ExplorerGraphiQL
+from quart import jsonify, request
 
-from otterdog.models.github_organization import GitHubOrganization
-from otterdog.utils import jsonnet_evaluate_file
-from otterdog.webapp.db.models import ConfigurationModel, StatisticsModel, TaskModel
-from otterdog.webapp.db.service import save_config, save_statistics
-from otterdog.webapp.tasks import InstallationBasedTask, Task
-from otterdog.webapp.utils import fetch_config_from_github
-
-
-@dataclass(repr=False)
-class FetchConfigTask(InstallationBasedTask, Task[None]):
-    installation_id: int
-    org_id: str
-    repo_name: str
-
-    def create_task_model(self):
-        return TaskModel(
-            type=type(self).__name__,
-            org_id=self.org_id,
-            repo_name=self.repo_name,
-        )
-
-    async def _pre_execute(self) -> None:
-        self.logger.info(
-            "fetching latest config from repo '%s/%s'",
-            self.org_id,
-            self.repo_name,
-        )
-
-    async def _execute(self) -> None:
-        async with self.get_organization_config() as org_config:
-            rest_api = await self.rest_api
-
-            config_file = org_config.jsonnet_config.org_config_file
-            sha = await fetch_config_from_github(
-                rest_api,
-                self.org_id,
-                self.org_id,
-                org_config.config_repo,
-                config_file,
-            )
-
-            # save configuration
-            config_data = jsonnet_evaluate_file(config_file)
-            config = ConfigurationModel(  # type: ignore
-                github_id=self.org_id,
-                project_name=org_config.name,
-                config=config_data,
-                sha=sha,
-            )
-            await save_config(config)
-
-            # save statistics
-            github_organization = GitHubOrganization.from_model_data(config_data)
-            statistics = StatisticsModel(  # type: ignore
-                project_name=org_config.name,
-                github_id=self.org_id,
-                num_repos=len(github_organization.repositories),
-            )
-            await save_statistics(statistics)
+from otterdog.webapp.db.service import (
+    get_configuration_by_github_id,
+    get_configuration_by_project_name,
+    get_installations,
+    get_merged_pull_requests_paged,
+    get_tasks_paged,
+)
 
-    def __repr__(self) -> str:
-        return f"FetchConfigTask(repo={self.org_id}/{self.repo_name})"
+from . import blueprint
+
+explorer_html = ExplorerGraphiQL(title="Otterdog GraphQL").html(None)
+
+
+@blueprint.route("/organizations")
+async def organizations():
+    installations = await get_installations()
+    result = list(map(lambda x: x.model_dump(include={"github_id", "project_name"}), installations))
+    return jsonify(result)
+
+
+@blueprint.route("/organizations/<github_id>")
+async def organization(github_id: str):
+    config = await get_configuration_by_github_id(github_id)
+    if config is None:
+        return {}, 404
+    else:
+        return jsonify(config.config)
+
+
+@blueprint.route("/projects/<project_name>")
+async def project(project_name: str):
+    config = await get_configuration_by_project_name(project_name)
+    if config is None:
+        return {}, 404
+    else:
+        return jsonify(config.config)
+
+
+@blueprint.route("/tasks")
+async def tasks():
+    paged_tasks, count = await get_tasks_paged(request.args.to_dict())
+    result = {"data": list(map(lambda x: x.model_dump(exclude={"id"}), paged_tasks)), "itemsCount": count}
+    return jsonify(result)
+
+
+@blueprint.route("/pullrequests/merged")
+async def merged_pullrequests():
+    paged_pull_requests, count = await get_merged_pull_requests_paged(request.args.to_dict())
+    result = {"data": list(map(lambda x: x.model_dump(), paged_pull_requests)), "itemsCount": count}
+    return jsonify(result)
+
+
+@blueprint.route("/graphql", methods=["GET"])
+async def graphql_playground():
+    return explorer_html, 200
+
+
+@blueprint.route("/graphql", methods=["POST"])
+async def graphql_server():
+    from .graphql import schema
+
+    data = await request.get_json()
+
+    success, result = await graphql(schema, data, context_value=request, debug=False)
+
+    status_code = 200 if success else 400
+    return jsonify(result), status_code
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/help_comment.py` & `otterdog-0.6.0/otterdog/webapp/tasks/auto_merge_comment.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,49 +11,47 @@
 from quart import render_template
 
 from otterdog.webapp.db.models import TaskModel
 from otterdog.webapp.tasks import InstallationBasedTask, Task
 
 
 @dataclass(repr=False)
-class HelpCommentTask(InstallationBasedTask, Task[None]):
+class AutoMergeCommentTask(InstallationBasedTask, Task[None]):
     installation_id: int
     org_id: str
     repo_name: str
     pull_request_number: int
 
     def create_task_model(self):
         return TaskModel(
             type=type(self).__name__,
             org_id=self.org_id,
             repo_name=self.repo_name,
             pull_request=self.pull_request_number,
         )
 
-    async def _pre_execute(self) -> None:
+    async def _execute(self) -> None:
         self.logger.info(
-            "adding help text to pull request #%d of repo '%s/%s'",
+            "adding auto merge comment to pull request #%d of repo '%s/%s'",
             self.pull_request_number,
             self.org_id,
             self.repo_name,
         )
 
-    async def _execute(self) -> None:
-        rest_api = await self.rest_api
-        comment = await render_template("comment/help_comment.txt")
-
-        await self.minimize_outdated_comments(
+        if not self.comment_with_header_exists(
             self.org_id,
             self.repo_name,
             self.pull_request_number,
-            "<!-- Otterdog Comment: help -->",
-        )
-
-        await rest_api.issue.create_comment(
-            self.org_id,
-            self.repo_name,
-            str(self.pull_request_number),
-            comment,
-        )
+            "<!-- Otterdog Comment: automerge -->",
+        ):
+            comment = await render_template("comment/auto_merge_comment.txt")
+
+            rest_api = await self.rest_api
+            await rest_api.issue.create_comment(
+                self.org_id,
+                self.repo_name,
+                str(self.pull_request_number),
+                comment,
+            )
 
     def __repr__(self) -> str:
-        return f"HelpCommentTask(repo={self.org_id}/{self.repo_name}, pull_request={self.pull_request_number})"
+        return f"AutoMergeCommentTask(repo='{self.org_id}/{self.repo_name}', pull_request=#{self.pull_request_number})"
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/retrieve_team_membership.py` & `otterdog-0.6.0/otterdog/webapp/tasks/retrieve_team_membership.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 #  *******************************************************************************
 
 from dataclasses import dataclass
 
 from quart import render_template
 
 from otterdog.webapp.db.models import TaskModel
-from otterdog.webapp.tasks import InstallationBasedTask, Task
+from otterdog.webapp.db.service import update_or_create_pull_request
+from otterdog.webapp.tasks import (
+    InstallationBasedTask,
+    Task,
+    contains_eligible_team_for_auto_merge,
+)
 from otterdog.webapp.webhook.github_models import PullRequest
 
 
 @dataclass(repr=False)
 class RetrieveTeamMembershipTask(InstallationBasedTask, Task[None]):
     installation_id: int
     org_id: str
@@ -34,42 +39,56 @@
         return TaskModel(
             type=type(self).__name__,
             org_id=self.org_id,
             repo_name=self.repo_name,
             pull_request=self.pull_request_number,
         )
 
-    async def _pre_execute(self) -> None:
+    async def _pre_execute(self) -> bool:
         if isinstance(self.pull_request_or_number, int):
             rest_api = await self.rest_api
             response = await rest_api.pull_request.get_pull_request(
                 self.org_id, self.repo_name, str(self.pull_request_number)
             )
             self._pull_request = PullRequest.model_validate(response)
         else:
             self._pull_request = self.pull_request_or_number
 
+        return True
+
+    async def _execute(self) -> None:
         self.logger.info(
             "retrieving team membership of author '%s' for pull request #%d of repo '%s/%s'",
             self._pull_request.user.login,
             self.pull_request_number,
             self.org_id,
             self.repo_name,
         )
 
-    async def _execute(self) -> None:
         rest_api = await self.rest_api
 
         user = self._pull_request.user.login
         association = self._pull_request.author_association
 
         graphql_api = await self.graphql_api
         team_data = await graphql_api.get_team_membership(self.org_id, user)
         team_membership = [team["name"] for team in team_data]
 
+        if self._pull_request.author_association == "MEMBER":
+            author_can_auto_merge = contains_eligible_team_for_auto_merge(team_membership)
+        else:
+            author_can_auto_merge = False
+
+        await update_or_create_pull_request(
+            self.org_id,
+            self.repo_name,
+            self._pull_request,
+            author_can_auto_merge=author_can_auto_merge,
+        )
+
         teams = [(team, f"https://github.com/orgs/{self.org_id}/teams/{team}") for team in team_membership]
         comment = await render_template(
             "comment/team_membership_comment.txt",
             user=user,
             association=association,
             teams=teams,
         )
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/tasks/validate_pull_request.py` & `otterdog-0.6.0/otterdog/webapp/tasks/validate_pull_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,35 +10,39 @@
 
 import filecmp
 from dataclasses import dataclass
 from io import StringIO
 
 from quart import current_app, render_template
 
-from otterdog.models import LivePatch
+from otterdog.models import LivePatch, LivePatchType
 from otterdog.operations.diff_operation import DiffStatus
 from otterdog.operations.local_plan import LocalPlanOperation
+from otterdog.providers.github import RestApi
 from otterdog.utils import IndentingPrinter, LogLevel
 from otterdog.webapp.db.models import TaskModel
 from otterdog.webapp.db.service import update_or_create_pull_request
 from otterdog.webapp.tasks import InstallationBasedTask, Task
 from otterdog.webapp.utils import (
     escape_for_github,
     fetch_config_from_github,
-    get_admin_team,
+    get_full_admin_team_slugs,
     get_otterdog_config,
 )
 from otterdog.webapp.webhook.github_models import PullRequest
 
 
 @dataclass
 class ValidationResult:
     plan_output: str = ""
-    validation_success: bool = True
-    requires_secrets: bool = False
+    validation_success: bool = False
+    touches_non_configuration: bool = False
+    requires_secrets: bool | None = None
+    requires_web_ui: bool | None = None
+    includes_deletions: bool | None = None
 
 
 @dataclass(repr=False)
 class ValidatePullRequestTask(InstallationBasedTask, Task[ValidationResult]):
     """Validates a PR and adds the result as a comment."""
 
     installation_id: int
@@ -63,41 +67,43 @@
         return TaskModel(
             type=type(self).__name__,
             org_id=self.org_id,
             repo_name=self.repo_name,
             pull_request=self.pull_request_number,
         )
 
-    async def _pre_execute(self) -> None:
+    async def _pre_execute(self) -> bool:
         if isinstance(self.pull_request_or_number, int):
             rest_api = await self.rest_api
             response = await rest_api.pull_request.get_pull_request(
                 self.org_id, self.repo_name, str(self.pull_request_or_number)
             )
             self._pull_request = PullRequest.model_validate(response)
         else:
             self._pull_request = self.pull_request_or_number
 
-        self.logger.info(
-            "validating pull request #%d of repo '%s/%s' with log level '%s'",
-            self.pull_request_number,
-            self.org_id,
-            self.repo_name,
-            self.log_level,
-        )
-
         await self._create_pending_status()
 
+        return True
+
     async def _post_execute(self, result_or_exception: ValidationResult | Exception) -> None:
         if isinstance(result_or_exception, Exception):
             await self._create_failure_status()
         else:
             await self._update_final_status(result_or_exception)
 
     async def _execute(self) -> ValidationResult:
+        self.logger.info(
+            "validating pull request #%d of repo '%s/%s' with log level '%s'",
+            self.pull_request_number,
+            self.org_id,
+            self.repo_name,
+            self.log_level,
+        )
+
         async with self.get_organization_config() as org_config:
             rest_api = await self.rest_api
 
             org_config_file = org_config.jsonnet_config.org_config_file
 
             # get BASE config
             base_file = org_config_file + "-BASE"
@@ -122,25 +128,36 @@
                 self._pull_request.head.repo.name,
                 head_file,
                 self._pull_request.head.ref,
             )
 
             validation_result = ValidationResult()
 
+            for file in await self._get_pull_request_files(rest_api):
+                self.logger.debug(f"touched file: {file}")
+                if file != f"otterdog/{self.org_id}.jsonnet":
+                    validation_result.touches_non_configuration = True
+                    break
+
             if filecmp.cmp(base_file, head_file):
                 self.logger.debug("head and base config are identical, no need to validate")
                 validation_result.plan_output = "No changes."
                 validation_result.validation_success = True
             else:
                 output = StringIO()
                 printer = IndentingPrinter(output, log_level=self.log_level)
                 operation = LocalPlanOperation("-BASE", False, False, "")
 
                 def callback(org_id: str, diff_status: DiffStatus, patches: list[LivePatch]):
                     validation_result.requires_secrets = any(list(map(lambda x: x.requires_secrets(), patches)))
+                    validation_result.requires_web_ui = any(list(map(lambda x: x.requires_web_ui(), patches)))
+
+                    validation_result.includes_deletions = any(
+                        list(map(lambda x: x.patch_type == LivePatchType.REMOVE, patches))
+                    )
 
                 otterdog_config = await get_otterdog_config()
 
                 operation.set_callback(callback)
                 operation.init(otterdog_config, printer)
 
                 try:
@@ -154,33 +171,41 @@
                     validation_result.validation_success = False
 
                 self.logger.info("local plan:" + validation_result.plan_output)
 
             warnings = []
             if validation_result.requires_secrets:
                 warnings.append("some of requested changes require secrets, need to apply these changes manually")
+            if validation_result.requires_web_ui:
+                warnings.append(
+                    "some of requested changes require accessing the Web UI, need to apply these changes manually"
+                )
 
             comment = await render_template(
                 "comment/validation_comment.txt",
                 sha=self._pull_request.head.sha,
                 result=escape_for_github(validation_result.plan_output),
                 warnings=warnings,
-                admin_team=f"{self.org_id}/{get_admin_team()}",
+                admin_teams=get_full_admin_team_slugs(self.org_id),
             )
 
             await self.minimize_outdated_comments(
                 self.org_id,
                 self.repo_name,
                 self.pull_request_number,
                 "<!-- Otterdog Comment: validate -->",
             )
 
             # add a comment about the validation result to the PR
+            rest_api = await self.rest_api
             await rest_api.issue.create_comment(
-                self.org_id, org_config.config_repo, str(self.pull_request_number), comment
+                self.org_id,
+                self.repo_name,
+                str(self.pull_request_number),
+                comment,
             )
 
             return validation_result
 
     async def _create_pending_status(self):
         rest_api = await self.rest_api
         await rest_api.commit.create_commit_status(
@@ -217,21 +242,38 @@
             self.repo_name,
             self._pull_request.head.sha,
             status,
             _get_webhook_validation_context(),
             desc,
         )
 
-        await update_or_create_pull_request(
+        pull_request_model = await update_or_create_pull_request(
             self.org_id,
             self.repo_name,
             self._pull_request,
             valid=validation_result.validation_success,
-            requires_manual_apply=validation_result.requires_secrets,
+            requires_manual_apply=validation_result.requires_secrets or validation_result.requires_web_ui,
+            supports_auto_merge=not (
+                validation_result.requires_secrets
+                or validation_result.requires_web_ui
+                or validation_result.includes_deletions
+                or validation_result.touches_non_configuration
+            ),
+        )
+
+        if pull_request_model.can_be_automerged():
+            self.schedule_automerge_task(self.org_id, self.repo_name, self.pull_request_number)
+
+    async def _get_pull_request_files(self, rest_api: RestApi) -> list[str]:
+        pull_request_data = await rest_api.pull_request.get_files(
+            self.org_id,
+            self.repo_name,
+            str(self.pull_request_number),
         )
+        return list(map(lambda x: x["filename"], pull_request_data))
 
     def __repr__(self) -> str:
         return (
             f"ValidatePullRequestTask(repo='{self.org_id}/{self.repo_name}', "
             f"pull_request=#{self.pull_request_number})"
         )
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/accounts/register.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/projects.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,110 @@
-{% extends "layouts/base-fullscreen.html" %}
+{% extends "layouts/base.html" %}
 
-{% block title %} Register {% endblock %}
+{% block title %} Dashboard {% endblock %}
 
 <!-- Element injected in the BODY element -->
-{% block body_class %} register-page {% endblock body_class %}
+{% block body_class %} sidebar-mini {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
-
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
-  <!-- icheck bootstrap -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/icheck-bootstrap@3.0.1/icheck-bootstrap.min.css">
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
-
+  {{ super() }}
 {% endblock stylesheets %}
 
 {% block content %}
 
-  <div class="register-box">
+  <div class="content-wrapper">
 
-    <div class="login-logo">
-        <a target="_blank" rel="noopener noreferrer"
-           href="https://appseed.us/product/adminlte/flask/"><b>Admin</b>LTE Flask</a>
+    <!-- Content Header (Page header) -->
+    <div class="content-header">
+      <div class="container-fluid">
+        <div class="row mb-2">
+          <div class="col-sm-6">
+            <h1 class="m-0 text-dark">{{ title }}</h1>
+          </div><!-- /.col -->
+          <div class="col-sm-6">
+            <ol class="breadcrumb float-sm-right">
+              <li class="breadcrumb-item"><a href="/index">Home</a></li>
+              <li class="breadcrumb-item active">{{ title }}</li>
+            </ol>
+          </div><!-- /.col -->
+        </div><!-- /.row -->
+      </div><!-- /.container-fluid -->
     </div>
+    <!-- /.content-header -->
 
-    <div class="card">
-      <div class="card-body register-card-body">
-        <p class="login-box-msg">
-            {% if msg %}
-                <span class="text-danger">{{ msg | safe }}</span>
-            {% else %}
-            <span>
-                Add your credentials
-            </span>
-            {% endif %}
-        </p>
-
-        <form role="form" method="post" action="">
-
-          {{ form.hidden_tag() }}
-
-          <div class="input-group mb-3">
-            {{ form.username(placeholder="Username", class="form-control") }}
-            <div class="input-group-append">
-              <div class="input-group-text">
-                <span class="fas fa-user"></span>
-              </div>
-            </div>
-          </div>
-          <div class="input-group mb-3">
-            {{ form.email(placeholder="Email", class="form-control") }}
-            <div class="input-group-append">
-              <div class="input-group-text">
-                <span class="fas fa-envelope"></span>
-              </div>
-            </div>
-          </div>
-          <div class="input-group mb-3">
-            {{ form.password(placeholder="Password", class="form-control", type="password") }}
-            <div class="input-group-append">
-              <div class="input-group-text">
-                <span class="fas fa-lock"></span>
+    <!-- Main content -->
+    <section class="content">
+      <div class="container-fluid">
+        <div class="row">
+          {% for installation in installations %}
+          {% set github_id = installation.github_id %}
+          {% set project_name = installation.project_name %}
+          {% set installation_status = installation.installation_status %}
+          <div class="col-md-3">
+            <div class="card">
+              {% if installation_status|status == 'success' %}
+              <a class="text-reset" href="/projects/{{ project_name }}">
+                <div class="card-header bg-{{ installation_status|status }}">
+                  <h3 class="card-title">{{ project_name }}</h3>
+                  <div class="float-right">
+                    <i class="fas fa-arrow-circle-right"></i>
+                  </div>
+                </div>
+              </a>
+              {% else %}
+              <a class="text-reset" href="#">
+                <div class="card-header bg-{{ installation_status|status }}">
+                  <h3 class="card-title">{{ project_name }}</h3>
+                </div>
+              </a>
+              {% endif %}
+              <div class="card-body">
+                <a href="https://github.com/{{ github_id }}"><i class="fab fa-github"></i> &nbsp; {{ github_id }}</a>
               </div>
-            </div>
-          </div>
-
-          <div class="row">
-            <div class="col-8">
-              <div class="icheck-primary">
-                <input type="checkbox" id="agreeTerms" name="terms" value="agree">
-                <label for="agreeTerms">
-                I agree to the <a href="#">terms</a>
-                </label>
+              <div class="card-footer p-0">
+                {% if installation_status|status == 'success' %}
+                <ul class="nav flex-column">
+                  {% if configurations[github_id] %}
+                  {% set config = configurations[github_id].config %}
+                  <li class="nav-item">
+                    <a href="/projects/{{ project_name }}#settings" class="nav-link">
+                      {% set two_factor_enabled = config.settings.two_factor_requirement %}
+                      2FA enforced <span class="float-right badge bg-{{ 'success' if two_factor_enabled == true else 'danger' }}">{{ two_factor_enabled }}</span>
+                    </a>
+                  </li>
+                  <li class="nav-item">
+                    <a href="/projects/{{ project_name }}#workflow-settings" class="nav-link tab-link">
+                      {% set default_workflow_permissions = config.settings.workflows.default_workflow_permissions %}
+                      Default workflow permissions <span class="float-right badge bg-{{ 'success' if default_workflow_permissions == 'read' else 'danger' }}">{{ default_workflow_permissions }}</span>
+                    </a>
+                  </li>
+                  <li class="nav-item">
+                    <a href="/projects/{{ project_name }}#repositories" class="nav-link">
+                      Repositories <span class="float-right badge bg-primary">{{ config.repositories|length }}</span>
+                    </a>
+                  </li>
+                  {% endif %}
+                </ul>
+                {% endif %}
               </div>
+              <!-- /.card-body -->
             </div>
-            <!-- /.col -->
-            <div class="col-4">
-              <button type="submit" name="register" class="btn btn-primary btn-block">Register</button>
-            </div>
-            <!-- /.col -->
+            <!-- /.card -->
           </div>
-        </form>
-
-        <br />
-        <div class="text-center">
-            Have an account? <a href="{{ url_for('authentication_blueprint.login') }}" class="text-center">Login</a>
-            <br />
-            <br />
-            &copy; ColorLib
-            <a target="_blank" rel="noopener noreferrer"
-               href="https://appseed.us/product/adminlte/flask/"><b>Admin</b>LTE</a>
-            - coded by <a target="_blank" rel="noopener noreferrer" href="https://appseed.us">AppSeed</a>.
+          {% endfor %}
+          <!-- /.col -->
         </div>
+        <!-- /.row -->
+
+      </div><!-- /.container-fluid -->
+    </section>
+    <!-- /.content -->
 
-      </div>
-      <!-- /.form-box -->
-    </div><!-- /.card -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
-
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
-
+  {{ super() }}
 {% endblock javascripts %}
```

#### html2text {}

```diff
@@ -1,19 +1,29 @@
-{% extends "layouts/base-fullscreen.html" %} {% block title %} Register {%
-endblock %} {% block body_class %} register-page {% endblock body_class %} {%
-block stylesheets %}
-{% endblock stylesheets %} {% block content %}
-_AA_dd_mm_ii_nn_L_T_E_ _F_l_a_s_k
-{% if msg %} {{ msg | safe }} {% else %} Add your credentials {% endif %}
-{{ form.hidden_tag() }}
-{{ form.username(placeholder="Username", class="form-control") }}
-{{ form.email(placeholder="Email", class="form-control") }}
-{{ form.password(placeholder="Password", class="form-control", type="password")
-}}
-??I agree to the _t_e_r_m_s
-Register
-
-Have an account? _L_o_g_i_n
-
-© ColorLib _AA_dd_mm_ii_nn_L_T_E - coded by _A_p_p_S_e_e_d.
-{% endblock content %} {% block javascripts %}
-{% endblock javascripts %}
+{% extends "layouts/base.html" %} {% block title %} Dashboard {% endblock %} {%
+block body_class %} sidebar-mini {% endblock body_class %} {% block stylesheets
+%} {{ super() }} {% endblock stylesheets %} {% block content %}
+************ {{{{ ttiittllee }}}} ************
+   1. _H_o_m_e
+   2. {{ title }}
+{% for installation in installations %} {% set github_id =
+installation.github_id %} {% set project_name = installation.project_name %} {%
+set installation_status = installation.installation_status %}
+{% if installation_status|status == 'success' %}
+_**_**_**_**_ _{{_{{_ _pp_rr_oo_jj_ee_cc_tt____nn_aa_mm_ee_ _}}_}}_ _**_**_**_**
+{% else %}
+_**_**_**_**_ _{{_{{_ _pp_rr_oo_jj_ee_cc_tt____nn_aa_mm_ee_ _}}_}}_ _**_**_**_**
+{% endif %}
+_ _ _{_{_ _g_i_t_h_u_b___i_d_ _}_}
+{% if installation_status|status == 'success' %}
+    * {% if configurations[github_id] %} {% set config = configurations
+      [github_id].config %}
+    * _{_%_ _s_e_t_ _t_w_o___f_a_c_t_o_r___e_n_a_b_l_e_d_ _=_ _c_o_n_f_i_g_._s_e_t_t_i_n_g_s_._t_w_o___f_a_c_t_o_r___r_e_q_u_i_r_e_m_e_n_t_ _%_}_ _2_F_A
+      _e_n_f_o_r_c_e_d_ _{_{_ _t_w_o___f_a_c_t_o_r___e_n_a_b_l_e_d_ _}_}
+    * _{_%_ _s_e_t_ _d_e_f_a_u_l_t___w_o_r_k_f_l_o_w___p_e_r_m_i_s_s_i_o_n_s_ _=
+      _c_o_n_f_i_g_._s_e_t_t_i_n_g_s_._w_o_r_k_f_l_o_w_s_._d_e_f_a_u_l_t___w_o_r_k_f_l_o_w___p_e_r_m_i_s_s_i_o_n_s_ _%_}_ _D_e_f_a_u_l_t
+      _w_o_r_k_f_l_o_w_ _p_e_r_m_i_s_s_i_o_n_s_ _{_{_ _d_e_f_a_u_l_t___w_o_r_k_f_l_o_w___p_e_r_m_i_s_s_i_o_n_s_ _}_}
+    * _R_e_p_o_s_i_t_o_r_i_e_s_ _{_{_ _c_o_n_f_i_g_._r_e_p_o_s_i_t_o_r_i_e_s_|_l_e_n_g_t_h_ _}_}
+    * {% endif %}
+{% endif %}
+{% endfor %}
+{% endblock content %} {% block javascripts %} {{ super() }} {% endblock
+javascripts %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/comment/team_membership_comment.txt` & `otterdog-0.6.0/otterdog/webapp/templates/comment/team_membership_comment.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 <!-- Otterdog Comment: team-info -->
-This is your friendly self-service bot. The author ([{{ user }}](https://github.com/{{ user }})) of this PR is associated with this organization in the role of `{{ association }}`.
+This is your friendly self-service bot.
 
+The author ([{{ user }}](https://github.com/{{ user }})) of this PR is associated with this organization in the role of `{{ association }}`.
 {% if (teams is defined) and teams %}
 Additionally, [{{ user }}](https://github.com/{{ user }}) is a member of the following teams:
 
 {% for team in teams %}
 - [{{ team.0 }}]({{ team.1 }})
 {% endfor %}
 {% else %}
-The author ([{{ user }}](https://github.com/{{ user }})) of this PR is not a member of this organization.
+The author ([{{ user }}](https://github.com/{{ user }})) of this PR is **NOT** a member of this organization.
 {% endif %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/organization.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/organization.html`

 * *Files 17% similar despite different names*

```diff
@@ -3,28 +3,21 @@
 {% block title %} Profile {% endblock %}
 
 <!-- Element injected in the BODY element -->
 {% block body_class %} sidebar-mini {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
+  {{ super() }}
+  <!-- Editor -->
+  <link rel="stylesheet" href="{{ asset('css/editor.css') }}">
 
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
-  <!-- Codemirror -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/lib/codemirror.min.css">
-
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
   <style>
     .CodeMirror { font-size: 12px; }
   </style>
-
 {% endblock stylesheets %}
 
 {% block content %}
 
   <!-- Content Wrapper. Contains page content -->
   <div class="content-wrapper">
     <!-- Content Header (Page header) -->
@@ -296,14 +289,15 @@
                           <tr>
                             <th>Repository</th>
                             <th class="text-center">Branch Protections</th>
                             <th class="text-center">Secrets</th>
                             <th class="text-center">Variables</th>
                             <th class="text-center">Webhooks</th>
                             <th class="text-center">Secret Scanning</th>
+                            <th class="text-center">Private Vulnerability Reporting</th>
                           </tr>
                         </thead>
                         <tbody>
                           {% for repo in config.repositories|sort(attribute='name') %}
                           <tr>
                             <td>
                               {% if repo.archived == true %}
@@ -357,14 +351,25 @@
                               <i class="text-success fa-solid fa-circle-check"></i>
                               {% elif repo.secret_scanning == "enabled" %}
                               <i class="text-warning fa-solid fa-circle-check"></i>
                               {% else %}
                               <i class="text-danger fa-solid fa-circle-xmark"></i>
                               {% endif %}
                             </td>
+                            <td class="text-center">
+                              {% if repo.archived == true %}
+                              <i class="text-muted fa-solid fa-circle"></i>
+                              {% elif repo.private_vulnerability_reporting_enabled == true %}
+                              <i class="text-success fa-solid fa-circle-check"></i>
+                              {% elif repo.private_vulnerability_reporting_enabled == false %}
+                              <i class="text-warning fa-solid fa-circle-xmark"></i>
+                              {% else %}
+                              <i class="text-muted fa-solid fa-circle"></i>
+                              {% endif %}
+                            </td>
                           </tr>
                           {% endfor %}
                         </tbody>
                       </table>
                     </div>
                   </div>
                 </div>
@@ -381,36 +386,52 @@
     <!-- /.content -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
-
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
+  {{ super() }}
   <!-- Chart.js -->
-  <script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.2/dist/chart.umd.min.js"></script>
-  <!-- Codemirror -->
-  <script src="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/lib/codemirror.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/mode/javascript/javascript.min.js"></script>
-  <!-- AdminLTE App -->
-  <script src="/static/assets/js/adminlte.min.js"></script>
+  <script src="/assets/vendor/chartjs/chart.umd.js"></script>
+
+  <script type="module">
+    import {createJavascriptEditor} from '{{ asset('js/editor.js') }}';
 
-  <script>
     $(document).ready(function() {
-      var hash = window.location.hash;
-      if (hash) {
-        $('[data-toggle="pill"][href="' + hash + '"]').trigger('click');
-      }
+      enableTabFromHash();
 
       drawSecretScanningChart();
       drawBranchProtectionChart();
+
+      window.onhashchange = function() {
+        enableTabFromHash();
+      };
+    });
+
+    function enableTabFromHash() {
+      var hash = window.location.hash;
+      if (!hash) {
+        hash = "#overview";
+      }
+      $('[data-toggle="pill"][href="' + hash + '"]').trigger('click', false);
+    }
+
+    $(".nav-tabs").find("li a").each(function(key, val) {
+      $(val).on("click", function(e, updateHistory) {
+        if (updateHistory == false) {
+          return;
+        }
+
+        if(history.pushState) {
+          history.pushState(null, null, $(this).attr('href'));
+        } else {
+          window.location.hash = $(this).attr('href');
+        }
+      });
     });
 
     $('.tab-link').on('click', function(event) {
       // Prevent url change
       event.preventDefault();
 
       // `this` is the clicked <a> tag
@@ -429,19 +450,15 @@
         }
       }
     });
 
     function enableEditor(selector) {
       var editor = $(selector).next('.CodeMirror').get(0);
       if (editor == null) {
-        editor = CodeMirror.fromTextArea($(selector).get(0), {
-          mode: "javascript",
-          lineWrapping: true,
-          readOnly: true
-        });
+        editor = createJavascriptEditor($(selector).get(0));
         editor.setSize(null, 750);
       }
     };
 
     function drawSecretScanningChart() {
       const secret_scanning_ctx = document.getElementById('secret-scanning-chart');
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "layouts/base.html" %} {% block title %} Profile {% endblock %} {%
 block body_class %} sidebar-mini {% endblock body_class %} {% block stylesheets
-%}
+%} {{ super() }}
 {% endblock stylesheets %} {% block content %}
 ************ {{{{ pprroojjeecctt__nnaammee }}}} ************
    1. _H_o_m_e
    2. {{ project_name }}
     * _O_v_e_r_v_i_e_w
     * _S_e_t_t_i_n_g_s
     * _W_o_r_k_f_l_o_w_ _S_e_t_t_i_n_g_s
@@ -43,16 +43,16 @@
 UURRLL         AAccttiivvee         EEvveennttss               UUsseess SSSSLL             RReessoollvveedd SSeeccrreett
             {% if              * {% for event                        {% if webhook.secret %}
 {           webhook.active       in             {% if                {% if not
 {           == true %} {%        webhook.events webhook.insecure_ssl webhook|has_dummy_secret
 webhook.url else %} {%           %}             == "0" %} {% else %} %} {% else %} {% endif
 }}          endif %}           * {{ event }}    {% endif %}          %} {% else %} {% endif
                                * {% endfor %}                        %}
-RReeppoossiittoorryy    BBrraanncchh PPrrootteeccttiioonnss                  SSeeccrreettss                        VVaarriiaabblleess             WWeebbhhooookkss                        SSeeccrreett SSccaannnniinngg
-{% if         {% if repo.archived == true %} {%   {% if repo.secrets|length > 0                        {% if repo.webhooks|length > 0  {% if repo.archived == true %} {%
-repo.archived elif                                %} {% if not                   {% if                 %} {% if not                    elif
-== true %} {% repo.branch_protection_rules|length repo.secrets|has_dummy_secrets repo.variables|length repo.webhooks|has_dummy_secrets repo.secret_scanning_push_protection
-endif %} _{    > 0 or repo.rulesets|length > 0 %}  %} {% else %} {% endif %} {%   > 0 %} {% else %} {%  %} {% else %} {% endif %} {%    == "enabled" %} {% elif
-_{_ _r_e_p_o_._n_a_m_e   {% else %} {% endif %}              else %} {% endif %}            endif %}              else %} {% endif %}             repo.secret_scanning == "enabled" %}
+RReeppoossiittoorryy    BBrraanncchh PPrrootteeccttiioonnss                  SSeeccrreettss                        VVaarriiaabblleess             WWeebbhhooookkss                        SSeeccrreett SSccaannnniinngg                      PPrriivvaattee VVuullnneerraabbiilliittyy RReeppoorrttiinngg
+{% if         {% if repo.archived == true %} {%   {% if repo.secrets|length > 0                        {% if repo.webhooks|length > 0  {% if repo.archived == true %} {%    {% if repo.archived == true %} {% elif
+repo.archived elif                                %} {% if not                   {% if                 %} {% if not                    elif                                 repo.private_vulnerability_reporting_enabled
+== true %} {% repo.branch_protection_rules|length repo.secrets|has_dummy_secrets repo.variables|length repo.webhooks|has_dummy_secrets repo.secret_scanning_push_protection == true %} {% elif
+endif %} _{    > 0 or repo.rulesets|length > 0 %}  %} {% else %} {% endif %} {%   > 0 %} {% else %} {%  %} {% else %} {% endif %} {%    == "enabled" %} {% elif              repo.private_vulnerability_reporting_enabled
+_{_ _r_e_p_o_._n_a_m_e   {% else %} {% endif %}              else %} {% endif %}            endif %}              else %} {% endif %}             repo.secret_scanning == "enabled" %} == false %} {% else %} {% endif %}
 _}_}                                                                                                                                     {% else %} {% endif %}
-{% endblock content %} {% block javascripts %}
+{% endblock content %} {% block javascripts %} {{ super() }}
 {% endblock javascripts %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/organizations.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/organizations.html`

 * *Files 23% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 {% block title %} GitHub Organizations {% endblock %}
 
 <!-- Element injected in the BODY element -->
 {% block body_class %} {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
-
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
+  {{ super() }}
   <!-- DataTables -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/datatables.net-bs4@1.13.10/css/dataTables.bootstrap4.min.css">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/datatables.net-responsive-bs4@2.2.9/css/responsive.bootstrap4.min.css">
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
-
+  <link rel="stylesheet" href="/assets/vendor/datatables/dataTables.bootstrap4.min.css">
+  <link rel="stylesheet" href="/assets/vendor/datatables/responsive.bootstrap4.min.css">
 {% endblock stylesheets %}
 
 {% block content %}
 
   <!-- Content Wrapper. Contains page content -->
   <div class="content-wrapper">
     <!-- Content Header (Page header) -->
@@ -86,26 +79,20 @@
     <!-- /.content -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
-
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
-  <!-- DataTables -->
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net@1.13.10/js/jquery.dataTables.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-bs4@1.13.10/js/dataTables.bootstrap4.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-responsive@2.2.9/js/dataTables.responsive.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-responsive-bs4@2.2.9/js/responsive.bootstrap4.min.js"></script>
-  <!-- AdminLTE App -->
-  <script src="/static/assets/js/adminlte.min.js"></script>
+  {{ super() }}
+ <!-- DataTables -->
+  <script src="/assets/vendor/datatables/jquery.dataTables.min.js"></script>
+  <script src="/assets/vendor/datatables/dataTables.bootstrap4.min.js"></script>
+  <script src="/assets/vendor/datatables/dataTables.responsive.min.js"></script>
+  <script src="/assets/vendor/datatables/responsive.bootstrap4.min.js"></script>
 
   <!-- page script -->
   <script>
     $(function () {
       $('#organizations').DataTable({
         "autoWidth": false,
         "responsive": true,
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/page-403.html` & `otterdog-0.6.0/otterdog/webapp/templates/layouts/base.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,55 @@
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Error 403 {% endblock %}
-
-<!-- Element injected in the BODY element -->
-{% block body_class %} login-page {% endblock body_class %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}
+<!DOCTYPE html>
+<html lang="en">
+<head>
+  <meta charset="utf-8">
+  <meta name="viewport" content="width=device-width, initial-scale=1">
+  <link rel="icon" href="/favicon.ico" type="image/x-icon">
+  <link rel="canonical" href="https://otterdog.eclipse.org/"/>
+
+  <title>
+    Otterdog Dashboard - {% block title %}{% endblock %} | Eclipse Foundation
+  </title>
 
+  {% block stylesheets %}
   <!-- Google Font: Source Sans Pro -->
   <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
   <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
-  <!-- icheck bootstrap -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/icheck-bootstrap@3.0.1/icheck-bootstrap.min.css">
+  <link rel="stylesheet" href="/assets/vendor/fontawesome-free/css/all.min.css">
+  <!-- Bootstrap 4 -->
+  <link rel="stylesheet" href="/assets/vendor/bootstrap/bootstrap.min.css">
   <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
-
-{% endblock stylesheets %}
-
-{% block content %}
+  <link rel="stylesheet" href="{{ asset('css/app.css') }}">
+  {% endblock stylesheets %}
 
-  <div class="login-box">
+</head>
+<body class="hold-transition {% block body_class %}{% endblock body_class %}">
+<div class="wrapper">
 
-    <div class="login-logo">
-        <a target="_blank" rel="noopener noreferrer"
-           href="https://github.com/eclipse-csi/otterdog">Otterdog Dashboard</a>
-    </div>
+    {% include 'includes/navigation.html' %}
 
-    <!-- /.login-logo -->
-    <div class="card">
+    {% include 'includes/sidebar.html' %}
 
-      <div class="card-body login-card-body">
+    {% block content %}{% endblock content %}
 
-        <h5 class="login-box-msg">
-          Error 403 - Access Denied
-        </h5>
-        <p class="login-box-msg">
-          Authentication is required to access this resource
-          - please <a href="{{ url_for('authentication_blueprint.login') }}" class="text-center">Login</a>
-        </p>
+    {% include 'includes/footer.html' %}
 
-        <br />
-        <div class="text-center">
-            Not a member? <a href="{{ url_for('authentication_blueprint.register') }}" class="text-center">Register</a>
-            <br />
-            <br />
-            &copy; <a target="_blank" rel="noopener noreferrer" href="https://eclipse.org">Eclipse Foundation and others</a>.
-        </div>
+    <!-- Control Sidebar -->
+    <aside class="control-sidebar control-sidebar-dark">
+        <!-- Control sidebar content goes here -->
+    </aside>
+    <!-- /.control-sidebar -->
 
-      </div>
-      <!-- /.login-card-body -->
-    </div>
+</div>
+<!-- ./wrapper -->
 
-  </div>
-
-{% endblock content %}
-
-<!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
-
   <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
+  <script src="/assets/vendor/jquery/jquery.min.js"></script>
   <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
-
+  <script src="/assets/vendor/bootstrap/bootstrap.bundle.min.js"></script>
+  <!-- AdminLTE App -->
+  <script type="module" src="{{ asset('js/app.js') }}"></script>
 {% endblock javascripts %}
+
+</body>
+</html>
```

#### html2text {}

```diff
@@ -1,13 +1,6 @@
-{% extends "layouts/base-fullscreen.html" %} {% block title %} Error 403 {%
-endblock %} {% block body_class %} login-page {% endblock body_class %} {%
-block stylesheets %}
-{% endblock stylesheets %} {% block content %}
-_O_t_t_e_r_d_o_g_ _D_a_s_h_b_o_a_r_d
-**** EErrrroorr 440033 -- AAcccceessss DDeenniieedd ****
-Authentication is required to access this resource - please _L_o_g_i_n
-
-Not a member? _R_e_g_i_s_t_e_r
-
-© _E_c_l_i_p_s_e_ _F_o_u_n_d_a_t_i_o_n_ _a_n_d_ _o_t_h_e_r_s.
-{% endblock content %} {% block javascripts %}
+{% block stylesheets %}
+{% endblock stylesheets %}
+{% include 'includes/navigation.html' %} {% include 'includes/sidebar.html' %}
+{% block content %}{% endblock content %} {% include 'includes/footer.html' %}
+{% block javascripts %}
 {% endblock javascripts %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/pullrequests.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/pullrequests.html`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,21 @@
 {% block title %} Pull Requests {% endblock %}
 
 <!-- Element injected in the BODY element -->
 {% block body_class %} {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
-
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
+  {{ super() }}
   <!-- DataTables -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/datatables.net-bs4@1.13.10/css/dataTables.bootstrap4.min.css">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/datatables.net-responsive-bs4@2.2.9/css/responsive.bootstrap4.min.css">
+  <link rel="stylesheet" href="/assets/vendor/datatables/dataTables.bootstrap4.min.css">
+  <link rel="stylesheet" href="/assets/vendor/datatables/responsive.bootstrap4.min.css">
   <!-- jsGrid -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid.min.css">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid-theme.min.css">
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
-
+  <link rel="stylesheet" href="/assets/vendor/jsgrid/jsgrid.min.css">
+  <link rel="stylesheet" href="/assets/vendor/jsgrid/jsgrid-theme.min.css">
 {% endblock stylesheets %}
 
 {% block content %}
 
   <!-- Content Wrapper. Contains page content -->
   <div class="content-wrapper">
     <!-- Content Header (Page header) -->
@@ -60,30 +53,35 @@
                   <tr>
                     <th>Organization</th>
                     <th>Repo</th>
                     <th>PR</th>
                     <th>Created</th>
                     <th>PR Status</th>
                     <th>Draft</th>
-                    <th>Config in-sync</th>
-                    <th>Manual required</th>
+                    <th>In-sync</th>
+                    <th>Requires manual</th>
+                    <th>Support automerge</th>
+                    <th>Approved</th>
                     <th>Apply Status</th>
                   </tr>
                   </thead>
                   <tbody>
                     {% for pr in open_pull_requests %}
+                    {% set id = pr.id %}
                     <tr class="{{ 'table-secondary' if pr.draft == True else ''}}">
-                      <td><a href="https://github.com/{{ pr.org_id }}">{{ pr.org_id }}</a></td>
-                      <td><a href="https://github.com/{{ pr.org_id }}/{{ pr.repo_name }}">{{ pr.repo_name }}</a></td>
-                      <td><a href="https://github.com/{{ pr.org_id }}/{{ pr.repo_name }}/pull/{{ pr.pull_request }}">#{{ pr.pull_request }}</a></td>
+                      <td><a href="https://github.com/{{ id.org_id }}">{{ id.org_id }}</a></td>
+                      <td><a href="https://github.com/{{ id.org_id }}/{{ id.repo_name }}">{{ id.repo_name }}</a></td>
+                      <td><a href="https://github.com/{{ id.org_id }}/{{ id.repo_name }}/pull/{{ id.pull_request }}">#{{ id.pull_request }}</a></td>
                       <td>{{ pr.created_at }}</td>
                       <td>{{ pr.status }}</td>
                       <td class="{{ 'text-primary' if pr.draft == True else '' }}">{{ pr.draft }}</td>
                       <td>{{ pr.in_sync }}</td>
                       <td>{{ pr.requires_manual_apply }}</td>
+                      <td>{{ pr.supports_auto_merge }}</td>
+                      <td>{{ pr.has_required_approval }}</td>
                       <td>{{ pr.apply_status }}</td>
                     </tr>
                     {% endfor %}
                   </tbody>
                 </table>
               </div>
               <!-- /.card-body -->
@@ -117,44 +115,32 @@
     <!-- /.content -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
+  {{ super() }}
 
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
   <!-- DataTables -->
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net@1.13.10/js/jquery.dataTables.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-bs4@1.13.10/js/dataTables.bootstrap4.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-responsive@2.2.9/js/dataTables.responsive.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/datatables.net-responsive-bs4@2.2.9/js/responsive.bootstrap4.min.js"></script>
+  <script src="/assets/vendor/datatables/jquery.dataTables.min.js"></script>
+  <script src="/assets/vendor/datatables/dataTables.bootstrap4.min.js"></script>
+  <script src="/assets/vendor/datatables/dataTables.responsive.min.js"></script>
+  <script src="/assets/vendor/datatables/responsive.bootstrap4.min.js"></script>
   <!-- jsGrid -->
-  <script src="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid.min.js"></script>
-  <!-- AdminLTE App -->
-  <script src="/static/assets/js/adminlte.min.js"></script>
+  <script src="/assets/vendor/jsgrid/jsgrid.min.js"></script>
 
   <!-- page script -->
   <script>
     $(function () {
-      $('#open-pull-requests').DataTable({
-        "order": [[3, 'desc']],
-        "autoWidth": false,
-        "responsive": true,
-      });
-
       $('#merged-pull-requests').DataTable({
         "order": [[3, 'desc']],
         "autoWidth": false,
         "responsive": true,
       });
-
     });
 
     $(function () {
       $("#mergedPullRequestsGrid").jsGrid({
           height: "auto",
           width: "100%",
 
@@ -179,28 +165,28 @@
                   });
 
                   return d.promise();
               }
           },
 
           fields: [
-              { name: "org_id", title: "GitHub Organization", type: "text", width: 70,
+              { name: "id.org_id", title: "GitHub Organization", type: "text", width: 70,
                 itemTemplate: function(value, item) {
                   return "<a href='https://github.com/" + value + "'>" + value + "</a>";
                 }
               },
-              { name: "repo_name", title: "Repo name", type: "text", width: 50,
+              { name: "id.repo_name", title: "Repo name", type: "text", width: 50,
                 itemTemplate: function(value, item) {
-                  return "<a href='https://github.com/" + item.org_id + "/" + value + "'>" + value + "</a>";
+                  return "<a href='https://github.com/" + item.id.org_id + "/" + value + "'>" + value + "</a>";
                 }
               },
-              { name: "pull_request", title: "Pull Request", type: "number", align: "center", width: 50,
+              { name: "id.pull_request", title: "Pull Request", type: "number", align: "center", width: 50,
                 itemTemplate: function(value, item) {
                   if (value > 0) {
-                    return "<a href='https://github.com/" + item.org_id + "/" + item.repo_name + "/pull/" + value + "'>#" + value + "</a>";
+                    return "<a href='https://github.com/" + item.id.org_id + "/" + item.id.repo_name + "/pull/" + value + "'>#" + value + "</a>";
                   } else {
                     return "N/A";
                   }
                 }
               },
               { name: "merged_at", title: "Merge Time", type: "text", width: 70 },
               { name: "status", title: "Status", type: "text", align: "center", width: 40,
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/repository.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/repository.html`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 {% block title %} Profile {% endblock %}
 
 <!-- Element injected in the BODY element -->
 {% block body_class %} sidebar-mini {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
+  {{ super() }}
+  <!-- Editor -->
+  <link rel="stylesheet" href="{{ asset('css/editor.css') }}">
 
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
-  <!-- Codemirror -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/lib/codemirror.min.css">
-
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
   <style>
     .CodeMirror { font-size: 12px; }
   </style>
 
 {% endblock stylesheets %}
 
 {% block content %}
@@ -91,14 +85,22 @@
                     <ul class="nav flex-column">
                       <li class="nav-item">
                         <a href="https://github.com/{{ github_id }}/{{ repo_name }}" class="nav-link">
                           Repository
                           <span class="float-right">{{ repo_name }}</span>
                         </a>
                       </li>
+                      {% if repo_config.private_vulnerability_reporting_enabled != null %}
+                      <li class="nav-item">
+                        <a href="#settings" class="nav-link tab-link">
+                          {% set private_vulnerability_reporting_enabled = repo_config.private_vulnerability_reporting_enabled %}
+                          Private Vulnerability Reporting <span class="float-right badge bg-{{ 'success' if private_vulnerability_reporting_enabled == true else 'danger' }}">{{ private_vulnerability_reporting_enabled }}</span>
+                        </a>
+                      </li>
+                      {% endif %}
                       <li class="nav-item">
                         <a href="#secrets" class="nav-link tab-link">
                           Secrets <span class="float-right badge bg-{{ repo_config.secrets|length_to_color}}">{{ repo_config.secrets|length }}</span>
                         </a>
                       </li>
                       <li class="nav-item">
                         <a href="#variables" class="nav-link tab-link">
@@ -325,26 +327,48 @@
     <!-- /.content -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
+  {{ super() }}
+  <script type="module">
+    import {createJavascriptEditor} from '{{ asset('js/editor.js') }}';
+
+    $(document).ready(function() {
+      enableTabFromHash();
+
+      window.onhashchange = function() {
+        enableTabFromHash();
+      };
+    });
 
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
-  <!-- Codemirror -->
-  <script src="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/lib/codemirror.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/codemirror@5.65.16/mode/javascript/javascript.min.js"></script>
-  <!-- AdminLTE App -->
-  <script src="/static/assets/js/adminlte.min.js"></script>
+    function enableTabFromHash() {
+      var hash = window.location.hash;
+      if (!hash) {
+        hash = "#overview";
+      }
+      $('[data-toggle="pill"][href="' + hash + '"]').trigger('click', false);
+    }
+
+    $(".nav-tabs").find("li a").each(function(key, val) {
+      $(val).on("click", function(e, updateHistory) {
+        if (updateHistory == false) {
+          return;
+        }
+
+        if(history.pushState) {
+          history.pushState(null, null, $(this).attr('href'));
+        } else {
+          window.location.hash = $(this).attr('href');
+        }
+      });
+    });
 
-  <script>
     $('.tab-link').on('click', function(event) {
       // Prevent url change
       event.preventDefault();
 
       // `this` is the clicked <a> tag
       $('[data-toggle="pill"][href="' + this.hash + '"]').trigger('click');
     });
@@ -388,20 +412,20 @@
            enableEditor(selector);
            break;
         }
       }
     });
 
     function enableEditor(selector) {
+      if ($(selector).length == 0) {
+        return;
+      }
+
       var editor = $(selector).next('.CodeMirror').get(0);
       if (editor == null) {
-        editor = CodeMirror.fromTextArea($(selector).get(0), {
-          mode: "javascript",
-          lineWrapping: true,
-          readOnly: true
-        });
+        editor = createJavascriptEditor($(selector).get(0));
         editor.setSize(null, 770);
       }
     };
   </script>
 
 {% endblock javascripts %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "layouts/base.html" %} {% block title %} Profile {% endblock %} {%
 block body_class %} sidebar-mini {% endblock body_class %} {% block stylesheets
-%}
+%} {{ super() }}
 {% endblock stylesheets %} {% block content %}
 ************ RReeppoossiittoorryy {{{{ rreeppoo__nnaammee }}}} ************
    1. _H_o_m_e
    2. _{_{_ _p_r_o_j_e_c_t___n_a_m_e_ _}_}
    3. {{ repo_name }}
     * _O_v_e_r_v_i_e_w
     * _S_e_t_t_i_n_g_s
@@ -12,14 +12,19 @@
     * _S_e_c_r_e_t_s
     * _V_a_r_i_a_b_l_e_s
     * _W_e_b_h_o_o_k_s
     * _E_n_v_i_r_o_n_m_e_n_t_s
     * _B_r_a_n_c_h_ _P_r_o_t_e_c_t_i_o_n_ _R_u_l_e_s
     * _R_u_l_e_s_e_t_s
     * _R_e_p_o_s_i_t_o_r_y_ _{_{_ _r_e_p_o___n_a_m_e_ _}_}
+    * {% if repo_config.private_vulnerability_reporting_enabled != null %}
+    * _{_%_ _s_e_t_ _p_r_i_v_a_t_e___v_u_l_n_e_r_a_b_i_l_i_t_y___r_e_p_o_r_t_i_n_g___e_n_a_b_l_e_d_ _=
+      _r_e_p_o___c_o_n_f_i_g_._p_r_i_v_a_t_e___v_u_l_n_e_r_a_b_i_l_i_t_y___r_e_p_o_r_t_i_n_g___e_n_a_b_l_e_d_ _%_}_ _P_r_i_v_a_t_e
+      _V_u_l_n_e_r_a_b_i_l_i_t_y_ _R_e_p_o_r_t_i_n_g_ _{_{_ _p_r_i_v_a_t_e___v_u_l_n_e_r_a_b_i_l_i_t_y___r_e_p_o_r_t_i_n_g___e_n_a_b_l_e_d_ _}_}
+    * {% endif %}
     * _S_e_c_r_e_t_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._s_e_c_r_e_t_s_|_l_e_n_g_t_h_ _}_}
     * _V_a_r_i_a_b_l_e_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._v_a_r_i_a_b_l_e_s_|_l_e_n_g_t_h_ _}_}
     * _W_e_b_h_o_o_k_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._w_e_b_h_o_o_k_s_|_l_e_n_g_t_h_ _}_}
     * _E_n_v_i_r_o_n_m_e_n_t_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._e_n_v_i_r_o_n_m_e_n_t_s_|_l_e_n_g_t_h_ _}_}
     * _B_r_a_n_c_h_ _P_r_o_t_e_c_t_i_o_n_ _R_u_l_e_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._b_r_a_n_c_h___p_r_o_t_e_c_t_i_o_n___r_u_l_e_s_|_l_e_n_g_t_h_ _}_}
     * _R_u_l_e_s_e_t_s_ _{_{_ _r_e_p_o___c_o_n_f_i_g_._r_u_l_e_s_e_t_s_|_l_e_n_g_t_h_ _}_}
 {{ repo_config|pretty_format_model }}
@@ -50,9 +55,9 @@
 {% endfor %}
 {% for ruleset in repo_config.rulesets %} {% set ruleset_id = 'ruleset-' ~
 loop.index %} _{_{_ _r_u_l_e_s_e_t_._n_a_m_e_ _}_} {% endfor %}
 {% for ruleset in repo_config.rulesets %} {% set ruleset_id = 'ruleset-' ~
 loop.index %}
 {{ ruleset|pretty_format_model }}
 {% endfor %}
-{% endblock content %} {% block javascripts %}
+{% endblock content %} {% block javascripts %} {{ super() }}
 {% endblock javascripts %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/home/tasks.html` & `otterdog-0.6.0/otterdog/webapp/templates/home/tasks.html`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 {% block title %} Executed Tasks {% endblock %}
 
 <!-- Element injected in the BODY element -->
 {% block body_class %} {% endblock body_class %}
 
 <!-- Specific Page CSS goes HERE  -->
 {% block stylesheets %}
-
-  <!-- Google Font: Source Sans Pro -->
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,400i,700&display=fallback">
-  <!-- Font Awesome -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.5.1/css/all.min.css">
+  {{ super() }}
   <!-- jsGrid -->
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid.min.css">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid-theme.min.css">
-  <!-- Theme style -->
-  <link rel="stylesheet" href="/static/assets/css/adminlte.min.css">
-
+  <link rel="stylesheet" href="/assets/vendor/jsgrid/jsgrid.min.css">
+  <link rel="stylesheet" href="/assets/vendor/jsgrid/jsgrid-theme.min.css">
 {% endblock stylesheets %}
 
 {% block content %}
 
   <!-- Content Wrapper. Contains page content -->
   <div class="content-wrapper">
     <!-- Content Header (Page header) -->
@@ -67,24 +60,18 @@
     <!-- /.content -->
   </div>
 
 {% endblock content %}
 
 <!-- Specific Page JS goes HERE  -->
 {% block javascripts %}
-
-  <!-- jQuery -->
-  <script src="https://cdn.jsdelivr.net/npm/jquery@3.5.1/dist/jquery.min.js"></script>
-  <!-- Bootstrap 4 -->
-  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/js/bootstrap.bundle.min.js"></script>
+  {{ super() }}
   <!-- jsGrid -->
-  <script src="https://cdn.jsdelivr.net/npm/jsgrid@1.5.3/dist/jsgrid.min.js"></script>
-  <script src="https://cdn.jsdelivr.net/npm/moment@2.30.1/moment.min.js"></script>
-  <!-- AdminLTE App -->
-  <script src="/static/assets/js/adminlte.min.js"></script>
+  <script src="/assets/vendor/moment/moment.min.js"></script>
+  <script src="/assets/vendor/jsgrid/jsgrid.min.js"></script>
 
   <!-- page script -->
   <script>
     var DateField = function (config) {
       jsGrid.Field.call(this, config);
     };
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/templates/includes/sidebar.html` & `otterdog-0.6.0/otterdog/webapp/templates/includes/sidebar.html`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,46 @@
               <p>
                 Dashboard
                 <i class="fas nav-icon"></i>
               </p>
             </a>
           </li>
 
+          {% if current_user.is_authenticated %}
+          <li class="nav-item">
+            <a href="/myprojects" class="nav-link {% if 'myprojects' in segments %} active {% endif %}">
+              <i class="nav-icon fas fa-house-user"></i>
+              <p>
+                My Projects
+                <i class="fas nav-icon"></i>
+              </p>
+            </a>
+          </li>
+          {% endif %}
+
+          <li class="nav-item">
+            <a href="/allprojects" class="nav-link {% if 'allprojects' in segments %} active {% endif %}">
+              <i class="nav-icon fas fa-globe"></i>
+              <p>
+                All Projects
+                <i class="fas nav-icon"></i>
+              </p>
+            </a>
+          </li>
+
+          <li class="nav-item">
+            <a href="/query" class="nav-link {% if 'query' in segments %} active {% endif %}">
+              <i class="nav-icon fa-brands fa-searchengin"></i>
+              <p>
+                Query
+                <i class="fas nav-icon"></i>
+              </p>
+            </a>
+          </li>
+
           <li class="nav-header">PROJECTS</li>
             {% for nav_level1, value_level1 in projects|dictsort %}
             {% if value_level1|is_dict %}
             <li class="nav-item has-treeview {% if segments[1] and segments[1].startswith(nav_level1) %} menu-open {% endif %}">
               <a href="#" class="nav-link {% if segments[1] and segments[1].startswith(nav_level1) %} active {% endif %}">
                 <i class="nav-icon fas fa-sitemap"></i>
                 <p class="font-weight-bold">
@@ -54,24 +86,14 @@
                       <i class="fas nav-icon"></i>
                     </p>
                   </a>
                 </li>
               {% endfor %}
               </ul>
             </li>
-            {% else %}
-            <li class="nav-item">
-              <a href="/projects/{{ value_level1.project_name }}" class="nav-link {% if value_level1.project_name in segments %} active {% endif %}">
-                <i class="nav-icon fab fa-square-github"></i>
-                <p>
-                  {{ value_level1.project_name }}
-                  <i class="fas nav-icon"></i>
-                </p>
-              </a>
-            </li>
             {% endif %}
             {% endfor %}
 
           <li class="nav-header">ADMINISTRATION</li>
 
           <li class="nav-item">
             <a href="/admin/organizations" class="nav-link {% if 'organizations' in segments %} active {% endif %}">
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
 _O_t_t_e_r_d_o_g
 [Unknown INPUT type]
     * _D_a_s_h_b_o_a_r_d
+    * {% if current_user.is_authenticated %}
+    * _M_y_ _P_r_o_j_e_c_t_s
+    * {% endif %}
+    * _A_l_l_ _P_r_o_j_e_c_t_s
+    * _Q_u_e_r_y
     * PROJECTS
     * {% for nav_level1, value_level1 in projects|dictsort %} {% if
       value_level1|is_dict %}
     * _{_{_ _n_a_v___l_e_v_e_l_1_ _}_}
           o {% for nav_level2, value_level2 in value_level1|dictsort %}
           o _{_{_ _v_a_l_u_e___l_e_v_e_l_2_._p_r_o_j_e_c_t___n_a_m_e_|_s_h_o_r_t___n_a_m_e_ _}_}
           o {% endfor %}
-    * {% else %}
-    * _{_{_ _v_a_l_u_e___l_e_v_e_l_1_._p_r_o_j_e_c_t___n_a_m_e_ _}_}
     * {% endif %} {% endfor %}
     * ADMINISTRATION
     * _G_i_t_H_u_b_ _O_r_g_s
     * _P_u_l_l_ _R_e_q_u_e_s_t_s
     * _T_a_s_k_s
 {% block javascripts %}
 {% endblock javascripts %}
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/utils.py` & `otterdog-0.6.0/otterdog/webapp/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -143,16 +143,21 @@
         async with aiofiles.tempfile.NamedTemporaryFile("wt") as file:
             name = cast(str, file.name)
             await file.write(content)
             await file.flush()
             return OtterdogConfig(name, False, app_root)
 
 
-def get_admin_team() -> str:
-    return current_app.config["GITHUB_ADMIN_TEAM"]
+def get_admin_teams() -> list[str]:
+    teams = str(current_app.config["GITHUB_ADMIN_TEAMS"])
+    return teams.split(",")
+
+
+def get_full_admin_team_slugs(org_id: str) -> list[str]:
+    return list(map(lambda team_slug: f"{org_id}/{team_slug}", get_admin_teams()))
 
 
 async def fetch_config_from_github(
     rest_api: RestApi,
     org_id: str,
     owner: str,
     repo: str,
@@ -208,7 +213,36 @@
 def current_utc_time() -> datetime:
     if sys.version_info < (3, 12):
         return datetime.utcnow()
     else:
         from datetime import UTC
 
         return datetime.now(UTC)
+
+
+def make_aware_utc(d: datetime) -> datetime:
+    if sys.version_info < (3, 12):
+        from datetime import timezone
+
+        utc = timezone(timedelta(0))
+        return d.astimezone(utc)
+    else:
+        from datetime import UTC
+
+        return d.astimezone(UTC)
+
+
+async def backoff_if_needed(last_event: datetime, required_timeout: timedelta) -> None:
+    last_event = make_aware_utc(last_event)
+    now = make_aware_utc(current_utc_time())
+
+    current_timeout = now - last_event
+
+    if current_timeout < required_timeout:
+        remaining_backoff = required_timeout - current_timeout
+        remaining_backoff_seconds = remaining_backoff.total_seconds() + 1
+        logger.debug(f"backing off {remaining_backoff_seconds}s")
+        await asyncio.sleep(remaining_backoff_seconds)
+
+
+def is_cache_control_enabled() -> bool:
+    return bool(current_app.config["CACHE_CONTROL"]) is True
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/webhook/__init__.py` & `otterdog-0.6.0/otterdog/webapp/webhook/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,46 +2,64 @@
 #  Copyright (c) 2023-2024 Eclipse Foundation and others.
 #  This program and the accompanying materials are made available
 #  under the terms of the Eclipse Public License 2.0
 #  which is available at http://www.eclipse.org/legal/epl-v20.html
 #  SPDX-License-Identifier: EPL-2.0
 #  *******************************************************************************
 
-import re
 from logging import getLogger
 
 from pydantic import ValidationError
 from quart import Response, current_app
 
-from otterdog.utils import LogLevel
 from otterdog.webapp.db.service import (
     get_installation,
     update_installation_status,
     update_installations_from_config,
 )
 from otterdog.webapp.tasks.apply_changes import ApplyChangesTask
 from otterdog.webapp.tasks.check_sync import CheckConfigurationInSyncTask
-from otterdog.webapp.tasks.complete_pull_request import CompletePullRequestTask
 from otterdog.webapp.tasks.fetch_config import FetchConfigTask
 from otterdog.webapp.tasks.help_comment import HelpCommentTask
 from otterdog.webapp.tasks.retrieve_team_membership import RetrieveTeamMembershipTask
 from otterdog.webapp.tasks.update_pull_request import UpdatePullRequestTask
 from otterdog.webapp.tasks.validate_pull_request import ValidatePullRequestTask
 from otterdog.webapp.utils import refresh_otterdog_config
 
+from .comment_handlers import (
+    ApplyCommentHandler,
+    CheckSyncCommentHandler,
+    CommentHandler,
+    DoneCommentHandler,
+    HelpCommentHandler,
+    MergeCommentHandler,
+    TeamInfoCommentHandler,
+    ValidateCommentHandler,
+)
 from .github_models import (
     InstallationEvent,
     IssueCommentEvent,
     PullRequestEvent,
+    PullRequestReviewEvent,
     PushEvent,
 )
 from .github_webhook import GitHubWebhook
 
 webhook = GitHubWebhook()
 
+comment_handlers: list[CommentHandler] = [
+    HelpCommentHandler(),
+    TeamInfoCommentHandler(),
+    CheckSyncCommentHandler(),
+    DoneCommentHandler(),
+    ApplyCommentHandler(),
+    MergeCommentHandler(),
+    ValidateCommentHandler(),
+]
+
 logger = getLogger(__name__)
 
 
 @webhook.hook("pull_request")
 async def on_pull_request_received(data):
     try:
         event = PullRequestEvent.model_validate(data)
@@ -51,34 +69,56 @@
 
     if event.installation is None or event.organization is None:
         return success()
 
     if not await targets_config_repo(event.repository.name, event.installation.id):
         return success()
 
-    current_app.add_background_task(
-        UpdatePullRequestTask(
-            event.installation.id,
-            event.organization.login,
-            event.repository.name,
-            event.pull_request,
+    if event.action in [
+        "opened",
+        "closed",
+        "ready_for_review",
+        "converted_to_draft",
+        "ready_for_review",
+        "reopened",
+        "synchronize",
+    ]:
+        current_app.add_background_task(
+            UpdatePullRequestTask(
+                event.installation.id,
+                event.organization.login,
+                event.repository.name,
+                event.pull_request,
+            )
         )
-    )
 
     if event.action in ["opened", "ready_for_review"] and event.pull_request.draft is False:
         current_app.add_background_task(
+            HelpCommentTask(
+                event.installation.id,
+                event.organization.login,
+                event.repository.name,
+                event.pull_request.number,
+            )
+        )
+
+        current_app.add_background_task(
             RetrieveTeamMembershipTask(
                 event.installation.id,
                 event.organization.login,
                 event.repository.name,
                 event.pull_request.number,
             )
         )
 
-    if event.action in ["opened", "synchronize", "ready_for_review", "reopened"] and event.pull_request.draft is False:
+    if (
+        event.action in ["opened", "synchronize", "ready_for_review", "reopened"]
+        and event.pull_request.state == "open"
+        and event.pull_request.draft is False
+    ):
         # schedule a validate task
         current_app.add_background_task(
             ValidatePullRequestTask(
                 event.installation.id,
                 event.organization.login,
                 event.repository.name,
                 event.pull_request,
@@ -99,22 +139,50 @@
         if event.pull_request.base.ref != event.repository.default_branch:
             return success()
 
         current_app.add_background_task(
             ApplyChangesTask(
                 event.installation.id,
                 event.organization.login,
-                event.repository,
+                event.repository.name,
                 event.pull_request,
             )
         )
 
     return success()
 
 
+@webhook.hook("pull_request_review")
+async def on_pull_request_review_received(data):
+    try:
+        event = PullRequestReviewEvent.model_validate(data)
+    except ValidationError:
+        logger.error("failed to load pull request review event data", exc_info=True)
+        return success()
+
+    if event.installation is None or event.organization is None:
+        return success()
+
+    if not await targets_config_repo(event.repository.name, event.installation.id):
+        return success()
+
+    if event.action in ["submitted", "edited", "dismissed"]:
+        current_app.add_background_task(
+            UpdatePullRequestTask(
+                event.installation.id,
+                event.organization.login,
+                event.repository.name,
+                event.pull_request,
+                event.review,
+            )
+        )
+
+    return success()
+
+
 @webhook.hook("issue_comment")
 async def on_issue_comment_received(data):
     try:
         event = IssueCommentEvent.model_validate(data)
     except ValidationError:
         logger.error("failed to load issue comment event data", exc_info=True)
         return success()
@@ -126,78 +194,19 @@
     if event.issue.pull_request is None:
         return success()
 
     if not await targets_config_repo(event.repository.name, event.installation.id):
         return success()
 
     if event.action in ["created", "edited"]:
-        org_id = event.organization.login
-        installation_id = event.installation.id
-
-        if re.match(r"\s*/help\s*", event.comment.body) is not None:
-            current_app.add_background_task(
-                HelpCommentTask(
-                    installation_id,
-                    org_id,
-                    event.repository.name,
-                    event.issue.number,
-                )
-            )
-            return success()
-        elif re.match(r"\s*/team-info\s*", event.comment.body) is not None:
-            current_app.add_background_task(
-                RetrieveTeamMembershipTask(
-                    installation_id,
-                    org_id,
-                    event.repository.name,
-                    event.issue.number,
-                )
-            )
-            return success()
-        elif re.match(r"\s*/check-sync\s*", event.comment.body) is not None:
-            current_app.add_background_task(
-                CheckConfigurationInSyncTask(
-                    installation_id,
-                    org_id,
-                    event.repository.name,
-                    event.issue.number,
-                )
-            )
-            return success()
-        elif re.match(r"\s*/done\s*", event.comment.body) is not None:
-            current_app.add_background_task(
-                CompletePullRequestTask(
-                    installation_id,
-                    org_id,
-                    event.repository.name,
-                    event.issue.number,
-                    event.sender.login,
-                )
-            )
-            return success()
-
-        m = re.match(r"\s*/validate(\s+info)?\s*", event.comment.body)
-        if m is None:
-            return success()
-
-        log_level_str = m.group(1)
-        log_level = LogLevel.WARN
-
-        if log_level_str is not None and log_level_str.strip() == "info":
-            log_level = LogLevel.INFO
-
-        current_app.add_background_task(
-            ValidatePullRequestTask(
-                installation_id,
-                org_id,
-                event.repository.name,
-                event.issue.number,
-                log_level,
-            )
-        )
+        for handler in comment_handlers:
+            match = handler.matches(event.comment.body)
+            if match is not None:
+                handler.process(match, event)
+                break
 
     return success()
 
 
 @webhook.hook("push")
 async def on_push_received(data):
     try:
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/webhook/github_models.py` & `otterdog-0.6.0/otterdog/webapp/webhook/github_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,27 @@
                 return "MERGED"
             else:
                 return "CLOSED"
         else:
             raise RuntimeError(f"unexpected state '{self.state}'")
 
 
+class Review(BaseModel):
+    """Represents a review on a pull request."""
+
+    author_association: str
+    body: str | None
+    commit_id: str
+    id: int
+    node_id: str
+    state: str
+    submitted_at: datetime | None
+    user: Actor | None
+
+
 class Comment(BaseModel):
     """Represents a comment in an issue."""
 
     id: int
     node_id: str
     user: Actor
     body: str
@@ -160,14 +173,23 @@
 
     action: str
     number: int
     pull_request: PullRequest
     repository: Repository
 
 
+class PullRequestReviewEvent(Event):
+    """A payload sent for pull request review specific events."""
+
+    action: str
+    pull_request: PullRequest
+    review: Review
+    repository: Repository
+
+
 class PushEvent(Event):
     """A payload sent for push events."""
 
     ref: str
     before: str
     after: str
```

### Comparing `otterdog-0.5.0b1/otterdog/webapp/webhook/github_webhook.py` & `otterdog-0.6.0/otterdog/webapp/webhook/github_webhook.py`

 * *Files identical despite different names*

### Comparing `otterdog-0.5.0b1/pyproject.toml` & `otterdog-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "otterdog"
-version       = "0.5.0b1"
+version       = "0.6.0"
 description   = "Tool to manage GitHub organizations and their repositories."
 authors       = ["Thomas Neidhart <thomas.neidhart@eclipse-foundation.org>"]
 readme        = "README.md"
 homepage      = "https://github.com/eclipse-csi/otterdog"
 repository    = "https://github.com/eclipse-csi/otterdog"
 documentation = "https://otterdog.readthedocs.io"
 keywords      = ["infrastructure-as-code", "supply-chain-security", "github", "gitops"]
@@ -56,31 +56,33 @@
 requests             = "^2.31"
 
 [tool.poetry.group.app.dependencies]
 quart                = "^0.19"
 quart-flask-patch    = "^0.3"
 python-decouple      = "^3.8"
 python-dotenv        = "^1.0"
-pydantic             = "^2.6"
-quart_minify         = "^0.4"
+pydantic             = "2.6.*"
+odmantic             = "^1.0.1"
 quart-auth           = "^0.9"
-quart-wtforms        = "^1.0"
-odmantic             = "^1.0"
 quart-redis          = "^2.0"
+github-flask         = "^3.2"
 aiohttp-client-cache = {version="^0.11.0", extras=["redis"]}
+ariadne              = "^0.22"
 
 
 [tool.poetry.group.dev.dependencies]
-black      = "^23.3"
+black      = ">=23.3,<25.0"
 flake8     = "^6.0"
 mypy       = "^1.8"
 pre-commit = "^3.3"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3"
+pytest         = "^7.3"
+pytest-asyncio = "^0.23"
+parameterized  = "^0.9"
 
 [tool.poetry.group.typing.dependencies]
 types-colorama   = "^0.4"
 types-requests   = "^2.31"
 types-jsonschema = "^4.17"
 types-chevron    = "^0.14"
 types-aiofiles   = "^23.2"
@@ -104,14 +106,19 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 testpaths  = ["tests"]
 pythonpath = [".", "otterdog"]
 
+log_cli = true
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+
 [tool.black]
 color          = true
 line-length    = 120
 target-version = ['py310']
 
 [tool.isort]
 profile = "black"
```

### Comparing `otterdog-0.5.0b1/PKG-INFO` & `otterdog-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otterdog
-Version: 0.5.0b1
+Version: 0.6.0
 Summary: Tool to manage GitHub organizations and their repositories.
 Home-page: https://github.com/eclipse-csi/otterdog
 Keywords: infrastructure-as-code,supply-chain-security,github,gitops
 Author: Thomas Neidhart
 Author-email: thomas.neidhart@eclipse-foundation.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

