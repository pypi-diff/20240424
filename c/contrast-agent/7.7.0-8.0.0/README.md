# Comparing `tmp/contrast-agent-7.7.0.tar.gz` & `tmp/contrast_agent-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrast-agent-7.7.0.tar", last modified: Tue Apr  9 18:16:43 2024, max compression
+gzip compressed data, was "contrast_agent-8.0.0.tar", last modified: Wed Apr 24 20:53:53 2024, max compression
```

## Comparing `contrast-agent-7.7.0.tar` & `contrast_agent-8.0.0.tar`

### file list

```diff
@@ -1,781 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/ext/hookspy.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.649119 contrast-agent-7.7.0/hookspy/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/hookspy/src/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/hookspy/src/hookspy/spy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.661119 contrast-agent-7.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.665119 contrast-agent-7.7.0/src/contrast/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.669119 contrast-agent-7.7.0/src/contrast/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.669119 contrast-agent-7.7.0/src/contrast/agent/agent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/input_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_lib/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.673119 contrast-agent-7.7.0/src/contrast/agent/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/adjusted_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/apply_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/assess_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/contrast_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.677119 contrast-agent-7.7.0/src/contrast/agent/assess/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/deadzone_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/preshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.689119 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/string_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.693120 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.697120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/base_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.705120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/dataflow_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.705120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.713120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_response_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/xss.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/static_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.717120 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/string_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/assess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/disable_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/heartbeat_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.721120 contrast-agent-7.7.0/src/contrast/agent/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/app_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14335 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/environ_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.721120 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/patch_location_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/policy_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/trigger_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/policy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/input_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.725120 contrast-agent-7.7.0/src/contrast/agent/protect/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/cmdi_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/http_method_tampering.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/malformed_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/path_traversal_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/protection_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/sqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/ssrf_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xss_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/reaction_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/request_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/server_settings_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/sys_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/thread_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/agent/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.729120 contrast-agent-7.7.0/src/contrast/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/aiohttp/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/api/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/architecture_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/route_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/trace_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/type_checked_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/api/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/assess/unsafe_code_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/applies/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/applies/sqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.733120 contrast-agent-7.7.0/src/contrast/assess_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/build_funchook.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.737120 contrast-agent-7.7.0/src/contrast/assess_extensions/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/cast.c
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/format.c
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/intern.c
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/propagate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/repeat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/repr.c
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/scope.c
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/subscript.c
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/common/trace.c
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/cs_str.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.git
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/
--rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.653119 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.741120 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
--rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
--rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
--rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-09 18:16:21.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/funchook.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/install-sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.749121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/__strerror.h
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook.c
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.c
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.c
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/suffix.list
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/test_main.c
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_test.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-09 18:16:20.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.657119 contrast-agent-7.7.0/src/contrast/assess_extensions/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.657119 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.753121 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py3/str_concat.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py310/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py311/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.757121 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py312/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py35/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py36/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py37/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.761121 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py38/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/assess_extensions/py39/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/bottle/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/bottle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/bottle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.765121 contrast-agent-7.7.0/src/contrast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/configuration/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/django/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/django_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/django_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/falcon_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/falcon_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.769121 contrast-agent-7.7.0/src/contrast/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/loader/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.773121 contrast-agent-7.7.0/src/contrast/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cgi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/concurrent_futures_thread_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cs_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/cs_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.773121 contrast-agent-7.7.0/src/contrast/patches/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/mysql_connector_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/psycopg2_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/pymysql_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/sqlalchemy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/databases/sqlite3_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/encodings_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/exec_and_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/patches/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/bottle_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/django_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/drf_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/falcon_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/pyramid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/frameworks/starlette_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/genshi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/import_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/lxml_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/patches/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/middleware/mod_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/pathlib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/re_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/str_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/threading_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/urllib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/patches/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/deadzones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.777121 contrast-agent-7.7.0/src/contrast/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/propagators/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.781121 contrast-agent-7.7.0/src/contrast/policy/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/cgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/quart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/sources/webob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/policy/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/cmd_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/httponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/nosql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/prompt_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/reflected_xss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/secure_flag_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/session_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/session_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/ssrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/trust_boundary_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/unsafe_code_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/untrusted_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/unvalidated_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/xpath_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/policy/triggers/xxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/pyramid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/quart/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/quart/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.785121 contrast-agent-7.7.0/src/contrast/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/activity_masker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/reporting_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/request_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.789121 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/effective_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/library_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/observed_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_startup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.789121 contrast-agent-7.7.0/src/contrast/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/fix_interpreter_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/propagator_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/scripts/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/duck_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/assess/tracking_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/base64_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/context_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/deprecated_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/digest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.793121 contrast-agent-7.7.0/src/contrast/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/ignored_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/utils/library_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/library_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/patched_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/library_reader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/loggers/structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/module_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/pattern_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/stack_trace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/stdlib_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 18:16:43.000000 contrast-agent-7.7.0/src/contrast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast/wsgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast/wsgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31844 2024-04-09 18:16:43.000000 contrast-agent-7.7.0/src/contrast_agent.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast_rewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.797121 contrast-agent-7.7.0/src/contrast_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.801121 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.805121 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.661119 contrast-agent-7.7.0/src/contrast_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.809121 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.813121 contrast-agent-7.7.0/src/contrast_vendor/structlog/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_greenlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/twisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/structlog/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/vendor-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.817122 contrast-agent-7.7.0/src/contrast_vendor/webob/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/acceptparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/byterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/cachecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/multidict.py
--rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/webob/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/zipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:43.821122 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-09 18:16:18.000000 contrast-agent-7.7.0/src/contrast_vendor/zipp/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/ext/hookspy.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.176628 contrast_agent-8.0.0/hookspy/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/hookspy/src/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/hookspy/src/hookspy/spy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:53:53.332630 contrast_agent-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.188629 contrast_agent-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.192628 contrast_agent-8.0.0/src/contrast/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.200629 contrast_agent-8.0.0/src/contrast/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.200629 contrast_agent-8.0.0/src/contrast/agent/agent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/input_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_lib/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.204629 contrast_agent-8.0.0/src/contrast/agent/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/adjusted_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/apply_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/assess_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15343 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/contrast_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.204629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/deadzone_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/preshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.208629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/string_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.212629 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.212629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/base_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.216629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/dataflow_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.216629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_response_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/static_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/trigger_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/string_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/assess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/disable_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/heartbeat_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/app_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/environ_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.220629 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.224629 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.224629 contrast_agent-8.0.0/src/contrast/agent/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/patch_location_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/policy_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/trigger_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/policy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/input_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.228629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/cmdi_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/http_method_tampering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/malformed_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/path_traversal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/sqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/ssrf_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xss_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/reaction_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/request_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/server_settings_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/sys_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/thread_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/agent/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/aiohttp/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/architecture_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/route_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/trace_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/type_checked_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/api/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.232629 contrast_agent-8.0.0/src/contrast/applies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/assess/unsafe_code_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/applies/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/applies/sqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.236629 contrast_agent-8.0.0/src/contrast/assess_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/build_funchook.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/cast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/intern.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/propagate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/repeat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/repr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/subscript.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/common/trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/cs_str.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 20:53:42.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.240629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.244629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.248629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.248629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/funchook.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/install-sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.252629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/__strerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.252629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/suffix.list
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/test_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_test.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 20:53:43.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.180628 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.256629 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py3/str_concat.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py310/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py311/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.260629 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py312/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py35/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py36/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py37/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.264629 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py38/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.268629 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/assess_extensions/py39/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.268629 contrast_agent-8.0.0/src/contrast/bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/bottle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/bottle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/configuration/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/django_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/django_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/falcon_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/falcon_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.272629 contrast_agent-8.0.0/src/contrast/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/loader/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.276629 contrast_agent-8.0.0/src/contrast/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cgi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/concurrent_futures_thread_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cs_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/cs_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/mysql_connector_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/psycopg2_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/pymysql_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/sqlalchemy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/databases/sqlite3_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/encodings_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/exec_and_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/bottle_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/django_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/drf_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/falcon_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/pyramid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/frameworks/starlette_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/genshi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/import_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/lxml_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/patches/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/middleware/mod_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/pathlib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/re_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/str_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/threading_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/urllib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/patches/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.280629 contrast_agent-8.0.0/src/contrast/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/deadzones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.284629 contrast_agent-8.0.0/src/contrast/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/propagators/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.284629 contrast_agent-8.0.0/src/contrast/policy/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/quart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/sources/webob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/policy/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/cmd_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/httponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/nosql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/prompt_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/reflected_xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/secure_flag_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/session_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/session_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/ssrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/trust_boundary_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/unsafe_code_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/untrusted_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/unvalidated_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/xpath_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/policy/triggers/xxe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/pyramid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/quart/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.288629 contrast_agent-8.0.0/src/contrast/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/activity_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/reporting_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/request_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.292629 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/agent_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/effective_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/library_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/observed_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/server_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.292629 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/protect_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/reporting/teamserver_responses/server_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.296629 contrast_agent-8.0.0/src/contrast/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/fix_interpreter_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/propagator_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/scripts/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/duck_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/assess/tracking_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/base64_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/context_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/deprecated_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/digest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.300629 contrast_agent-8.0.0/src/contrast/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/ignored_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/utils/library_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/library_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/patched_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/library_reader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/loggers/structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/pattern_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/stack_trace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/stdlib_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 20:53:52.000000 contrast_agent-8.0.0/src/contrast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast/wsgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-04-24 20:53:53.000000 contrast_agent-8.0.0/src/contrast_agent.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.304629 contrast_agent-8.0.0/src/contrast_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.308629 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.188629 contrast_agent-8.0.0/src/contrast_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.316630 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.324630 contrast_agent-8.0.0/src/contrast_vendor/structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_greenlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/threadlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/structlog/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/vendor-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/webob/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/acceptparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/byterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/cachecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/webob/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/zipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:53.328630 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-24 20:53:41.000000 contrast_agent-8.0.0/src/contrast_vendor/zipp/glob.py
```

### Comparing `contrast-agent-7.7.0/LICENSE.txt` & `contrast_agent-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/MANIFEST.in` & `contrast_agent-8.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/PKG-INFO` & `contrast_agent-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrast-agent
-Version: 7.7.0
+Version: 8.0.0
 Summary: Contrast Security's agent for Python web frameworks
 Author-email: "Contrast Security, Inc." <python@contrastsecurity.com>
 License: Copyright: 2024 Contrast Security, Inc
         Contact: support@contrastsecurity.com
         License: Commercial
         
         NOTICE: This Software and the patented inventions embodied within may only be used as
```

### Comparing `contrast-agent-7.7.0/hookspy/README.md` & `contrast_agent-8.0.0/hookspy/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/hookspy/ext/hookspy.c` & `contrast_agent-8.0.0/hookspy/ext/hookspy.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/hookspy/setup.py` & `contrast_agent-8.0.0/hookspy/setup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/hookspy/src/hookspy/autogen.py` & `contrast_agent-8.0.0/hookspy/src/hookspy/autogen.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/hookspy/src/hookspy/body.py` & `contrast_agent-8.0.0/hookspy/src/hookspy/body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .signatures import (
     fastcall_name,
     fastcall_kwargs_name,
     calls_by_name,
-    propagate_args_by_name,
     signatures_by_name,
 )
 
 
 hook_template = """{} {{{}
 }}
 """
```

### Comparing `contrast-agent-7.7.0/hookspy/src/hookspy/signatures.py` & `contrast_agent-8.0.0/hookspy/src/hookspy/signatures.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/hookspy/src/hookspy/spy.py` & `contrast_agent-8.0.0/hookspy/src/hookspy/spy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/pyproject.toml` & `contrast_agent-8.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -53,14 +53,43 @@
     | build/*
   )/ |
   framework_test/django-2\.2\.1/app/view_definitions\.py |
   framework_test/django-3\.0\.6/app/view_definitions\.py
 )
 '''
 
+[tool.ruff]
+line-length = 88
+target-version = "py38"
+extend-exclude = [
+  "src/contrast_vendor/",
+  "tests/agent/data/rewriter/golden/",
+  "tests/agent/data/rewriter/source/",
+  "tests/extern/",
+]
+
+[tool.ruff.lint]
+extend-select = [
+    "E",
+    "W",
+    "PLE",
+    "PLC",
+    # we may want to add these eventually
+    # "B",
+    # "PLW",
+    # "RUF",
+    # "PERF",
+    # "UP",
+    # "RET",
+]
+# we may want to remove this eventually
+ignore = [
+  "E501",  # Line too long
+]
+
 [tool.pytest.ini_options]
 testpaths = "tests integration-tests/test-create-config-script"
 filterwarnings = [
   "error::DeprecationWarning",
   # for DeprecatedWarning which doesn't work for some reason if not like this
   "error:.*Call to deprecated.*",
   "error::PendingDeprecationWarning",
```

### Comparing `contrast-agent-7.7.0/setup.py` & `contrast_agent-8.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import platform
 import tempfile
 import time
 from glob import glob
 from io import open
 from os import environ, path, system
 from shutil import rmtree
-from setuptools import Extension, find_packages, setup
+from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.install_lib import install_lib
-import warnings
 
 root_dir = path.abspath(path.dirname(__file__))
 
 
 AGENT_LIB_REQUIREMENT = "~=0.5.4"
 
 
@@ -47,15 +46,15 @@
 debug = environ.get("ASSESS_DEBUG")
 debug_args = ["-g", "-O1"] if debug else []
 macros = [("ASSESS_DEBUG", 1)] if debug else []
 macros.append(("EXTENSION_BUILD_TIME", '"{}"'.format(time.ctime())))
 
 strict_build_args = ["-Werror"] if environ.get("CONTRAST_STRICT_BUILD") else []
 
-NO_FUNCHOOK = environ.get("CONTRAST_NO_FUNCHOOK") or is_arm()
+NO_FUNCHOOK = environ.get("CONTRAST_NO_FUNCHOOK", "1") != "0" or is_arm()
 if NO_FUNCHOOK:
     macros.append(("NO_FUNCHOOK", 1))
     c_sources = [
         path.join(common_dir, name)
         for name in [
             "patches.c",
             "scope.c",
```

### Comparing `contrast-agent-7.7.0/src/contrast/__init__.py` & `contrast_agent-8.0.0/src/contrast/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import os
 from contrast.agent.assess.string_tracker import StringTracker
 from contrast.utils.context_tracker import ContextTracker
 from contrast.version import __version__
-from contrast.assess_extensions import cs_str
-from contrast.agent.assess.utils import get_properties
+from contrast.assess_extensions import cs_str  # noqa: F401
+from contrast.agent.assess.utils import get_properties  # noqa: F401
 
 # process globals
 CS__CONTEXT_TRACKER = ContextTracker()
 STRING_TRACKER = StringTracker()
 TELEMETRY = None
 
 # PERF: These values are constant for the lifetime of the agent,
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/agent_lib/__init__.py` & `contrast_agent-8.0.0/src/contrast/agent/agent_lib/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,33 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 
 # we need this to ensure `agent_lib.modules.*` is available when importing `agent_lib`
-import contrast.agent.agent_lib.modules
+import contrast.agent.agent_lib.modules  # noqa: F401
+
 from contrast.agent.agent_lib.main import call, initialize, update_log_options
 from contrast.agent.agent_lib.input_tracing import (
     evaluate_header_input,
     evaluate_input_by_type,
     initialize_input_tracing,
     check_sql_injection_query,
     check_cmd_injection_query,
     check_method_tampering,
     map_result_and_free_eval_result,
     map_result_and_free_check_query_sink_result,
     DBType,
 )
+
+__all__ = [
+    "call",
+    "initialize",
+    "update_log_options",
+    "evaluate_header_input",
+    "evaluate_input_by_type",
+    "initialize_input_tracing",
+    "check_sql_injection_query",
+    "check_cmd_injection_query",
+    "check_method_tampering",
+    "map_result_and_free_eval_result",
+    "map_result_and_free_check_query_sink_result",
+    "DBType",
+]
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/agent_lib/input_tracing.py` & `contrast_agent-8.0.0/src/contrast/agent/agent_lib/input_tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,45 +93,68 @@
         )
         for input_type_str, input_type_int in agent_lib.modules.CONSTANTS.InputType.items()
     }
 
 
 class InputAnalysisResult:
     rule_id = TypeCheckedProperty(str)
+    _c_rule_id = TypeCheckedProperty(int)
     input_type = TypeCheckedProperty(InputType, constructor_arg=InputType.UNKNOWN)
+    _c_input_type = TypeCheckedProperty(int)
     score = TypeCheckedProperty(float)
     key = TypeCheckedProperty(str)
     value = TypeCheckedProperty(str)
     path = TypeCheckedProperty(str)
     ids = TypeCheckedProperty(list)
     attack_count = TypeCheckedProperty(int)
     prefer_worth_watching = TypeCheckedProperty(bool)
 
     def __init__(self, input_value, value, ceval_results, prefer_worth_watching):
         if (
             isinstance(ceval_results, agent_lib.modules.CONSTANTS.CEvalResult)
             and input_value is not None
             and isinstance(value, str)
         ):
-            self.rule_id = rule_id_lookup()[ceval_results.rule_id]
-            self.input_type = input_type_lookup()[ceval_results.input_type]
+            self._c_rule_id = ceval_results.rule_id
+            self.rule_id = rule_id_lookup()[self._c_rule_id]
+            self._c_input_type = ceval_results.input_type
+            self.input_type = input_type_lookup()[self._c_input_type]
 
             self.score = ceval_results.score
 
             if isinstance(input_value, str):
                 self.key = input_value
             elif isinstance(input_value, bytes):
                 self.key = input_value.decode()
             else:
                 # c_char_p
                 self.key = input_value.value.decode()
 
             self.value = value
             self.prefer_worth_watching = prefer_worth_watching
 
+    def fully_evaluate(self):
+        """
+        Evaluates the input using the same rule and input type, but without
+        optimizations such as worth watching preferences. This is slower, but
+        more accurate.
+        """
+        return (
+            agent_lib.evaluate_header_input(
+                self.key, self.value, self._c_rule_id, prefer_worth_watching=False
+            )
+            if self.input_type == InputType.HEADER
+            else agent_lib.evaluate_input_by_type(
+                self._c_input_type,
+                self.value,
+                self._c_rule_id,
+                prefer_worth_watching=False,
+            )
+        )
+
 
 class InjectionResult:
     def __init__(self, user_input, input_index, input_len, ccheck_query_sink_result):
         self.start_index = None
         self.end_index = None
         self.boundary_overrun_index = None
         self.input_boundary_index = None
@@ -273,26 +296,30 @@
 
 def check_method_tampering(input_value, prefer_worth_watching):
     evaluations = []
 
     if not agent_lib.modules.is_initialized():
         return evaluations
 
+    # These codes should match https://agent-lib.prod.dotnet.contsec.com/src/contrast_c/method_tampering.rs.html#11-28
+    IS_TAMPERING = 1
+    IS_NOT_TAMPERING = 0
+
     def is_valid_return(code):
-        return 1 >= code >= 0
+        return code in (IS_TAMPERING, IS_NOT_TAMPERING)
 
     name = ctypes.c_char_p(bytes(input_value, "utf8"))
 
     ret = agent_lib.call(
         agent_lib.modules.LIB_CONTRAST.is_method_tampering,
         is_valid_return,
         name,
     )
 
-    if ret != 1:
+    if ret != IS_TAMPERING:
         return []
 
     c_eval_res = agent_lib.modules.CONSTANTS.CEvalResult()
     c_eval_res.rule_id = agent_lib.modules.CONSTANTS.RuleType.get("method-tampering")
     c_eval_res.input_type = agent_lib.modules.CONSTANTS.InputType.get("Method")
     c_eval_res.score = 100
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/agent_lib/main.py` & `contrast_agent-8.0.0/src/contrast/agent/agent_lib/main.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/agent_state.py` & `contrast_agent-8.0.0/src/contrast/agent/agent_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-
 import sys
 import platform
 import atexit
 import threading
 import warnings
 
 from contextlib import contextmanager
@@ -27,24 +26,24 @@
     setup_basic_agent_logger,
     setup_agent_logger,
     setup_security_logger,
 )
 from contrast.utils import timer
 from contrast.utils.library_reader.library_reader import LibraryReader
 from contrast.utils.namespace import Namespace
-from contrast.utils.decorators import fail_loudly
+from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast_rewriter import (
     process_rewriter_logs,
     set_rewriter_logger,
 )
 from contrast.agent.runner import is_runner_in_use
 
 # NOTE: policy is currently loaded/generated on import. It is applied explicitly in
 # policy/applicator.py
-from contrast import policy  # pylint: disable=unused-import
+from contrast import policy  # noqa: F401
 
 logger = setup_basic_agent_logger()
 LOGS_SEPARATOR = "-" * 120
 
 SHARED_WARNING_MESSAGE = """
 For specific circumstances where explicit middleware configuration is still
 required, set `agent.python.enable_automatic_middleware` to `false` in the
@@ -160,56 +159,46 @@
         settings.is_agent_config_enabled()
         and not protect_enabled
         and not assess_enabled
     ):
         logger.warning("Neither Protect nor Assess is enabled. Neither is running.")
 
 
-def _successful_startup_msgs():
-    if not _send_startup_msg_with_retries(teamserver_messages.ServerStartup()):
-        return False
-    if not _send_startup_msg_with_retries(teamserver_messages.ApplicationStartup()):
-        return False
-    return True
-
+@fail_quietly(return_value=False)
+def _successful_startup_msgs() -> bool:
+    """
+    Send the AgentStartup message immediately.
+    This function intentionally runs in the main thread and is blocking.
 
-def _send_startup_msg_with_retries(msg):
+    Return False if the message, after retries, fails to connect to TeamServer.
+    Note that we only need to retry if we get an ambiguous response (5xx).
+    """
     attempt = 1
     while True:
-        if _send_startup_msg(msg):
-            return True
+        msg = teamserver_messages.AgentStartup()
+        response = module.reporting_client.send_message(msg)
+        if response is not None:
+            msg.process_response(response, module.reporting_client)
+            if response.status_code < 500:
+                return True
+            elif response.status_code == 500:
+                raise RuntimeError("Unexpected 500 response code from AgentStartup")
 
         attempt += 1
         if attempt > MAX_ATTEMPTS:
             break
 
-        logger.debug("%s: will retry - sleeping for 1 second", msg.class_name)
+        logger.debug("AgentStartup did not connect -  will retry sleeping for 1 second")
         timer.sleep(1)
 
-    # TODO: PYT-2612 use the commented-out logic here instead
-    # logger.error(
-    #     "%s: Unexpected error from Contrast UI. Will not initialize Contrast Agent."
-    # )
-    # return False
-    return True
-
-
-def _send_startup_msg(msg):
-    """
-    Send a single startup message (ServerStartup or ApplicationStartup) immediately.
-    This function runs in the main thread, and is blocking.
-
-    Return False if the message needs to be retried, True otherwise.
-    Note that we only need to retry if we get an ambiguous response (5xx).
-    """
-    response = module.reporting_client.send_message(msg)
-    if response is None:
-        return False
-    msg.process_response(response, module.reporting_client)
-    return response.status_code < 500
+    logger.error(
+        "Unexpected error from Contrast UI. Will not initialize Contrast Agent.",
+        message=msg.class_name,
+    )
+    return False
 
 
 def initialize_libraries():
     """
     If enabled, read libraries from the application
     :return: True
     """
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/asgi.py` & `contrast_agent-8.0.0/src/contrast/agent/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/adjusted_span.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/adjusted_span.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/apply_trigger.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/apply_trigger.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/contrast_event.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/contrast_event.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/analysis.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/analysis.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/deadzone_node.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/deadzone_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/patches.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/preshift.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/preshift.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_node.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagation_policy.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagation_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -172,62 +172,14 @@
 
     # If the stream is already considered tracked, it will not be treated as a
     # source.
     elif self_obj.cs__source and method_name in STREAM_SOURCES:
         apply_stream_source(method_name, target, self_obj, ret, args, kwargs)
 
 
-def cast_special_case(method_name, args, target):
-    """
-    We don't want to record an event when `target is source`.
-
-    This will never happen for bytearrays, because they are always at least copied.
-    For bytearrays, we check if the source and target are ==, and if so we copy
-    tags over without recording a new event.
-
-    It would be better if there were some way to check for this slightly later,
-    based on the policy node's information.
-
-    Currently, every other string function is an instance method, so we short-
-    circuit out of propagation if `self_obj is ret`. For casting, self_obj is None
-    because casting (which is really __new__ for unicode/bytes) is a module method
-    """
-    if method_name == "CAST":
-        source = args and args[0]
-        if target is source:
-            return True
-        if (
-            isinstance(source, bytearray)
-            and isinstance(target, bytearray)
-            and target == source
-        ):
-            track_copy_without_new_event(target, source)
-            return True
-    return False
-
-
-def translate_special_case(method_name, self_obj, ret):
-    """
-    py27 unicode objects and py3x str objects returned by str.translate()
-    are always new objects, so in order to keep our behavior consistent we
-    do not create a new event in the case where new == original
-
-    If this method returns True, we should copy all tags from
-    self_obj to target without creating a new event.
-    """
-    return (
-        method_name == "translate"
-        and ret == self_obj
-        and (
-            (PY2 and isinstance(self_obj, unicode))
-            or (PY3 and isinstance(self_obj, str))
-        )
-    )
-
-
 def apply_propagator(propagator_node, preshift, target, ret):
     if not propagator_node or not target:
         return
 
     if isinstance(target, dict):
         for key, value in target.items():
             apply_propagator(propagator_node, preshift, key, ret)
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/__init__.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from . import stream_propagator
-from .base_propagator import BasePropagator, SUPPORTED_TYPES
+from .base_propagator import BasePropagator, SUPPORTED_TYPES  # noqa: F401
 from .append_propagator import AppendPropagator
 from .center_propagator import CenterPropagator
 from .codecs_splat_propagator import CodecsSplatPropagator
 from .format_propagator import FormatPropagator
 from .join_propagator import JoinPropagator
 from .json_propagator import JsonPropagator
 from .keep_propagator import KeepPropagator
@@ -20,15 +20,14 @@
 from .reductive_propagator import ReductivePropagator
 from .regex_propagator import RegexFindallPropagator, RegexSplitPropagator
 from .db_write_propagator import DBWritePropagator
 from .encode_html_splat_propagator import EncodeHtmlSplatPropagator
 from .repr_propagator import ReprPropagator
 from .tagger import Tagger
 
-
 APPEND_ACTION = "APPEND"
 CENTER_ACTION = "CENTER"
 CODECS_SPLAT_ACTION = "CODECS_SPLAT"
 FORMAT_ACTION = "FORMAT"
 JOIN_ACTION = "JOIN"
 JSON_ACTION = "JSON"
 KEEP_ACTION = "KEEP"
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/append_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/append_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/base_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/base_propagator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 from contrast.utils.decorators import cached_property, fail_quietly
 from contrast.agent.assess.utils import (
     is_tracked,
     get_properties,
     track_string,
 )
 
-SUPPORTED_TYPES = (
-    str,
-    bytes,
-    bytearray,
-)
+SUPPORTED_TYPES = tracking_util.SUPPORTED_TYPES
 
 
 class BasePropagator:
     def __init__(self, node, preshift, target):
         """
         :param node: instance of PropagationNode
         """
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/format_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/format_propagator.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,48 +23,42 @@
         super().__init__(node, preshift, target)
         if node.method_name == "cformat":
             self.tokens = tokenize_cformat(preshift.obj)
         else:
             self.tokens = tokenize_format(preshift.obj)
         self._tracked_args = None
 
-    def any_args_tracked(self):
-        for string in self.sources:  # pylint: disable=not-an-iterable
-            if tracking_util.recursive_is_tracked(string):
-                return True
-
-        return False
-
     @cached_property
     def sources(self):
         sources = []
         # Any string that corresponds to a format token is a source
         for token in self.tokens:
             if isinstance(token, FormatToken):
                 sources.append(token.get_arg(self.preshift.args, self.preshift.kwargs))
         return sources + [self.preshift.obj]
 
-    @property
-    def tracked_args(self):
-        if self._tracked_args is None:
-            self._tracked_args = self.any_args_tracked()
-        return self._tracked_args
+    @cached_property
+    def tracked_sources(self):
+        return any(tracking_util.recursive_is_tracked(src) for src in self.sources)
 
     def get_parent_ids(self, *args):
         return get_last_event_ids_from_sources(self.sources)
 
     @property
     def inputs_require_propagation(self):
         if tracking_util.recursive_is_tracked(self.preshift.obj):
             return True
 
-        return self.tracked_args
+        return self.tracked_sources
 
     def track_target(self):
-        if tracking_util.recursive_is_tracked(self.preshift.obj) or self.tracked_args:
+        if (
+            tracking_util.recursive_is_tracked(self.preshift.obj)
+            or self.tracked_sources
+        ):
             track_string(self.target)
 
     def _propagate(self):
         args, kwargs = self.preshift.args, self.preshift.kwargs
 
         # Offset in the target string
         target_offset = 0
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/join_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/json_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/json_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/split_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/split_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_node.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/source_policy.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/source_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/string_propagation.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/string_propagation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from contrast_vendor import structlog as logging
 
 import contrast
 from contrast.agent.assess.policy.preshift import Preshift
 from contrast.agent.assess.policy.propagation_policy import track_copy_without_new_event
 
 # We call these from the C extension - they're import aliases
-from contrast.agent.assess.policy.propagation_policy import (  # pylint: disable=unused-import
+from contrast.agent.assess.policy.propagation_policy import (  # noqa: F401
     create_stream_source_event,
     propagate_stream,
 )
 from contrast.agent.assess.policy.propagators import BasePropagator, PROPAGATOR_ACTIONS
 from contrast.agent.policy import registry
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/policy/trigger_policy.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/policy/trigger_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/preflight.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/properties.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/properties.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/base_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_config_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/config/session_age_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/config/session_age_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/dataflow_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/non_dataflow_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/non_dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/enable.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/enable.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/analyze.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/analyze.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/base_response_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/base_response_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/response/xss.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/response/xss.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/static_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/static_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/trigger_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/sampling.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/string_tracker.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/string_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/tag.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/tag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/truncate.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/truncate.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/assess/utils.py` & `contrast_agent-8.0.0/src/contrast/agent/assess/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/disable_reaction.py` & `contrast_agent-8.0.0/src/contrast/agent/disable_reaction.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/events.py` & `contrast_agent-8.0.0/src/contrast/agent/events.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/exceptions.py` & `contrast_agent-8.0.0/src/contrast/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/exclusions.py` & `contrast_agent-8.0.0/src/contrast/agent/exclusions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
 
 
 from enum import Enum, auto
+from typing import List
 
 from contrast.utils.decorators import fail_loudly
 from contrast.api import TypeCheckedProperty
 
 
 from contrast_vendor import structlog as logging
 
@@ -96,15 +97,15 @@
         # Aliases for the same source type
         input_exclusions["HEADER"] = input_exclusions["HEADER_KEY"]
         input_exclusions["MULTIPART_FORM_DATA"] = input_exclusions["BODY"]
         input_exclusions["MULTIPART_CONTENT_DATA"] = input_exclusions["BODY"]
 
         return input_exclusions
 
-    def __init__(self, exclusions):
+    def __init__(self, exclusions: List[TsExclusion]):
         self.input_exclusions = self.init_input_exclusions_container()
         self.url_exclusions = []
 
         has_named_exclusion = False
 
         for exc in exclusions:
             if exc.type == ExclusionType.INPUT_EXCLUSION_TYPE:
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/framework.py` & `contrast_agent-8.0.0/src/contrast/agent/framework.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/heartbeat_thread.py` & `contrast_agent-8.0.0/src/contrast/agent/heartbeat_thread.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/metrics.py` & `contrast_agent-8.0.0/src/contrast/agent/metrics.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/app_finder.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/app_finder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/base_middleware.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/base_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,15 @@
           in the request context.
 
         We then call to each rule to determine if they have any special prefilter actions, whether due to not being
         implemented in agent-lib or b/c they need special analysis.
         """
         logger.debug("PROTECT: Running Agent prefilter.")
 
-        input_analysis.get_input_analysis(prefer_worth_watching=True)
+        input_analysis.analyze_inputs()
 
         for rule in self.settings.protect_rules.values():
             if rule.is_prefilter():
                 rule.prefilter()
 
     @fail_loudly("Unable to do postfilter")
     def postfilter(self, context):
@@ -346,19 +346,14 @@
 
         analyze_response_rules(context)
 
     @fail_quietly("Failed to run postfilter protect.")
     def postfilter_protect(self, context):
         logger.debug("PROTECT: Running Agent postfilter.")
 
-        input_analysis.get_input_analysis(prefer_worth_watching=False)
-
-        # TODO: PYT-3255 this second call to get_input_analysis discards previous data
-        # about attack_count
-
         for rule in self.settings.protect_rules.values():
             if rule.is_postfilter():
                 rule.postfilter()
 
     @fail_loudly("Unable to do check_for_blocked")
     def check_for_blocked(self, context: RequestContext):
         """
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/environ_tracker.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/environ_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/common.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,22 @@
 - route should be the path to the view function (aka controller for Java people)
 - one method type per route
 
 Example:
       GET /blog/foo/bar - app.blogs.find(request, ) 0
 """
 
+from typing import Iterable
+from contrast.api import Route
 import re
 
+from contrast_vendor import structlog as logging
+
+logger = logging.getLogger("contrast")
+
 
 DEFAULT_ROUTE_METHODS = ("GET", "POST")
 
 
 # A format template for constructing "path-component" regexps, ie between "/"-s in a URI
 # This is used to build regexps for uri normalization
 # We use a look-ahead to ensure correctness for back-to-back path components
@@ -99,7 +105,15 @@
         method_arg_names = str(
             func.__code__.co_varnames[0 : func.__code__.co_argcount]
         ).replace("'", "")
     elif isinstance(func, str):
         method_arg_names = func
 
     return method_arg_names
+
+
+def log_discovered_routes(framework: str, routes: Iterable[Route]) -> None:
+    logger.debug(
+        "Discovered routes",
+        framework=framework,
+        routes=[f"{route.verb} {route.url}" for route in routes],
+    )
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/django_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/django_routes.py`

 * *Files 13% similar despite different names*

```diff
@@ -228,25 +228,7 @@
         and settings.APPEND_SLASH
     ):
         result = get_view_func(f"{path}/")
     if result is None:
         return None
 
     return result.func
-
-
-class DjangoRoutesMixin:
-    @fail_quietly("Unable to get route coverage", return_value={})
-    def get_route_coverage(self):
-        """
-        Route Coverage is the Assess feature that looks for routes generally defined
-        in Django apps in a file like urls.py
-        """
-        return create_django_routes()
-
-    @fail_quietly("Unable to get Django view func")
-    def get_view_func(self, request):
-        return get_view_func(self.request_path)
-
-    @fail_quietly("Unable to build route", return_value="")
-    def build_route(self, view_func, url):
-        return build_django_route(view_func)
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,19 +95,14 @@
 
 def build_falcon_route(view_func, endpoint_cls):
     route_args = build_args_from_function(view_func)
     route = f"{endpoint_cls.__class__.__name__}.{view_func.__name__}{route_args}"
     return route
 
 
-@fail_quietly("Unable to get route coverage", return_value={})
-def get_route_coverage(falcon_app):
-    return create_falcon_routes(falcon_app)
-
-
 @fail_quietly("Unable to get Falcon view func")
 def get_view_func(request_path, falcon_app, request_method):
     if not request_path:
         return None
 
     route_info = falcon_app._router.find(request_path)
     if not route_info:
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,19 +69,14 @@
 
 def build_pyramid_route(pyramid_route_name, view_func):
     method_arg_names = build_args_from_function(view_func)
 
     return pyramid_route_name + method_arg_names
 
 
-@fail_quietly("Unable to get route coverage", return_value={})
-def get_route_coverage(registry):
-    return create_pyramid_routes(registry)
-
-
 @fail_quietly("Unable to find new routes")
 def get_view_func(request_path, routes_list, registry):
     if not request_path:
         logger.debug("No path info for pyramid request")
         return None
 
     # Ideally we would like to call get_route but
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py` & `contrast_agent-8.0.0/src/contrast/wsgi/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,180 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-from contrast.api import Route
-from contrast.agent import agent_state
-from contrast.agent.middlewares.route_coverage.common import build_key
+import functools
+from contrast_vendor.webob import Request
+
+import contrast
+from contrast.agent import agent_state, scope, request_state
+from contrast.agent.policy.trigger_node import TriggerNode
+from contrast.agent.middlewares.base_middleware import (
+    BaseMiddleware,
+    log_request_start_and_end,
+)
+from contrast.agent.middlewares.environ_tracker import track_environ_sources
+from contrast.utils.decorators import cached_property, fail_quietly
+from contrast.utils.safe_import import safe_import_list
+from contrast.utils.assess.duck_utils import safe_getattr_list
 
 from contrast_vendor import structlog as logging
+from contrast.utils import Profiler
 
 logger = logging.getLogger("contrast")
+DEFAULT_WSGI_NAME = "wsgi_app"
+
+
+@functools.lru_cache(maxsize=1)
+def _get_flask_types():
+    return tuple(safe_import_list("flask.Flask"))
 
 
-class RoutesMixin:
+class WSGIMiddleware(BaseMiddleware):
     """
-    Class for route coverage work.
-    Route coverage is assess only.
+    Contrast middleware; PEP-333(3) WSGI-compliant
     """
 
-    def handle_routes(self, context, request):
-        """
-        Method that should run for all middlewares immediately after the application
-        executes.
-        """
-        if context and request:
-            self.get_routes_on_first_request()
-            self.check_for_new_routes(context, request)
-            self.append_route_to_findings(context)
+    @scope.with_contrast_scope
+    def __init__(
+        self, wsgi_app, app_name=None, original_app=None, orig_pyramid_registry=None
+    ):
+        # We need to keep the `original_app` `orig_pyramid_registry` kwarg for now to prevent a breaking API
+        # change
+        del original_app
+        del orig_pyramid_registry
+
+        # TODO: PYT-2852 Revisit application name detection
+        self.app_name = (
+            app_name
+            if app_name is not None
+            else safe_getattr_list(
+                wsgi_app,
+                [
+                    "__name__",
+                    "name",
+                ],
+                DEFAULT_WSGI_NAME,
+            )
+        )
 
-    def get_routes_on_first_request(self):
-        """
-        Attempt to do route discovery on the first request
-        """
+        super().__init__()
 
-        # if we already have routes here, we must have populated them from a framework-
-        # specific patch. Eventually, `get_routes_on_first_request` will be completely
-        # removed, once all frameworks perform route discovery using patches.
-        if not agent_state.is_first_request():
-            logger.debug("skipping route discovery - not the first request")
-            return
-        if agent_state.get_routes():
-            logger.debug("skipping route discovery - already populated")
-            return
+        if not agent_state.in_automatic_middleware() and isinstance(
+            wsgi_app, _get_flask_types()
+        ):
+            # we need this to prevent a breaking API change when wrapping Flask apps
+            wsgi_app = wsgi_app.wsgi_app
 
-        logger.debug("First request so looking for app routes.")
+        self.wsgi_app = wsgi_app
 
-        discovered_routes = self.get_route_coverage()
+    def __call__(self, environ, start_response):
+        if request_state.get_request_id() is not None:
+            # This can happen if a single app is wrapped by multiple instances of the
+            # middleware (usually caused by automatic instrumentation)
+            logger.debug("Detected preexisting request_id - passing through")
+            return self.wsgi_app(environ, start_response)
 
-        if not discovered_routes or not isinstance(discovered_routes, dict):
-            logger.debug("Could not find any routes")
-            return
+        self.request_path = environ.get("PATH_INFO", "")
 
-        routes = agent_state.get_routes()
-        routes.update(discovered_routes)
+        # the request_id context manager must come first!
+        with request_state.request_id_context(), Profiler(
+            self.request_path
+        ), log_request_start_and_end(
+            environ.get("REQUEST_METHOD", ""), self.request_path
+        ):
+            context = self.should_analyze_request(environ)
+            if context:
+                with contrast.CS__CONTEXT_TRACKER.lifespan(context):
+                    return self.call_with_agent(context, environ, start_response)
 
-        routes_to_log = [f"{route.verb}: {route.url}" for route in routes.values()]
-        logger.debug("Found the following routes: %s", routes_to_log)
+            return self.call_without_agent(environ, start_response)
 
-    def check_for_new_routes(self, context, request):
-        """
-        Check to see if the current request is a new route. If so, add this to the list
-        of all discovered routes.
-        """
-        logger.debug("Checking for new route.")
+    @scope.with_contrast_scope
+    def call_with_agent(self, context, environ, start_response):
+        track_environ_sources("wsgi", context, environ)
 
-        if context.view_func is None:
-            context.view_func = self.get_view_func(request)
-            if context.view_func is None:
-                logger.debug(
-                    "unable to determine view function for the current request"
-                )
-                return
-        else:
-            logger.debug("already have the view function for this request")
+        try:
+            self.prefilter()
 
-        request_method = request.method
-        route_id = build_key(str(id(context.view_func)), request_method)
+            webob_request = Request(environ)
+            with scope.pop_contrast_scope():
+                response = webob_request.get_response(self.wsgi_app)
 
-        self.update_route_information(context, route_id, request_method)
+            context.extract_response_to_context(response)
 
-    def update_route_information(self, context, route_id, request_method):
-        """
-        Given a context and route_id, check if the route_id is in middleware (self)
-        routes. Store the route as current and observed route for later use.
+            self.postfilter(context)
+            self.check_for_blocked(context)
+            self.swap_environ_path(environ)  # should not be moved to finally
 
-        :param context: RequestContext instance
-        :param route_id: string id for a route
-        :param request_method: string such as 'GET'
-        :return: no return, side effects only
-        """
-        routes = agent_state.get_routes()
-        if route_id not in routes:
-            url = context.request.get_normalized_uri()
+            return response(environ, start_response)
 
-            if context.view_func_str is None:
-                context.view_func_str = self.build_route(context.view_func, url)
+        finally:
+            self.handle_ensure(context, context.request)
+            if self.settings.is_assess_enabled():
+                contrast.STRING_TRACKER.ageoff()
 
-            routes[route_id] = Route(
-                verb=request_method, url=url, route=context.view_func_str
-            )
+    def swap_environ_path(self, environ):
+        """
+        See PYT-1742.
 
-        route = routes[route_id]
-        logger.debug("Route visited: %s : %s", route.verb, route.url)
+        Special behavior required for bottle+django to account for an unfortunate
+        encoding behavior.
 
-        context.current_route = route
+        In bottle, it occurs here:
+        bottle.py:
+        def _handle(self, environ):
+            ...
+            environ['PATH_INFO'] = path.encode('latin1').decode('utf8')
+            ...
 
-        # Currently we do not report an observed route if the route signature is empty.
-        # As a team we've decided there isn't a meaningful default signature value
-        # we can provide to customers. If a route doesn't show up in Contrast UI,
-        # it may be due to its missing signature. In this scenario, we will have to work
-        # with the customer directly to understand why the signature was not created.
-        if not route.signature:
-            logger.debug(
-                "No route signature found for %s : %s (id=%s). Not updating observed"
-                " route",
-                route.verb,
-                route.url,
-                route_id,
-            )
-            return
+        This casing occurs after the application code is called, and will result in a
+        `UnicodeEncodeError` when the agent attempts to access request.path.
+        As a workaround, we store the original PATH_INFO - before bottle changed it
+        during calling app code - and use it for agent purposes.
+        """
+        environ["PATH_INFO"] = self.request_path
 
-        context.observed_route.signature = route.signature
+    def call_without_agent(self, environ, start_response):
+        """
+        Normal without middleware call
+        """
+        super().call_without_agent()
+        with scope.contrast_scope():
+            return self.wsgi_app(environ, start_response)
 
-        context.observed_route.url = route.url
-        context.observed_route.verb = route.verb
+    @cached_property
+    def trigger_node(self):
+        """
+        WSGI-specific trigger node used by reflected xss postfilter rule
 
-    def append_route_to_findings(self, context):
+        The rule itself is implemented in the base middleware but we need to
+        provide a WSGI-specific trigger node for reporting purposes.
         """
-        Route discovery and current route is not identified until the handle ensure
-        part of the request lifecycle, after assess has analyzed and potentially created
-        a finding, so that is why we have to append the now-available current route to
-        the existing finding.
-        """
-        if not context.current_route:
-            logger.debug("No current route to append to findings")
-            return
-
-        if not context.findings:
-            logger.debug("No findings to append route to")
-            return
-
-        for finding in context.findings:
-            if not finding.routes:
-                logger.debug(
-                    "Appending route %s:%s to %s",
-                    context.current_route.verb,
-                    context.current_route.url,
-                    finding.rule_id,
-                )
-                finding.routes.append(context.current_route)
+        method_name = self.app_name
+
+        module, class_name, args, instance_method = self._process_trigger_handler(
+            self.wsgi_app
+        )
+
+        return (
+            TriggerNode(module, class_name, instance_method, method_name, "RETURN"),
+            args,
+        )
 
-            finding.set_version()
+    @fail_quietly("Unable to get WSGI view func")
+    def get_view_func(self, _):
+        """
+        While most frameworks define view functions, WSGI doesn't so we will rely
+        on the path information for reporting.
+        If there is no path information, return None
 
-    def get_view_func(self, request):
-        return
+        :param request: RequestContext instance
+        :return: string of path information for this request or None
+        """
+        return self.request_path or None
 
+    @fail_quietly("Unable to build route", return_value="")
     def build_route(self, view_func, url):
-        return ""
+        return url.replace("/", "")
+
+    @cached_property
+    def name(self):
+        return "wsgi"
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py` & `contrast_agent-8.0.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/patch_controller.py` & `contrast_agent-8.0.0/src/contrast/agent/patch_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-from contrast_vendor import structlog as logging
-
-logger = logging.getLogger("contrast")
-
 from contrast.agent.assess.policy import string_propagation
 from contrast.agent.policy import registry
 from contrast.agent.policy.applicator import register_import_hooks
 from contrast.agent.policy.rewriter import apply_rewrite_policy
 from contrast.agent.settings import Settings
 from contrast.assess_extensions import cs_str
 from contrast.patches import (
@@ -16,14 +12,17 @@
     register_common_patches,
     register_library_patches,
 )
 from contrast.utils.namespace import Namespace
 from contrast.utils.patch_utils import repatch_imported_modules
 from contrast_rewriter import register as register_rewriter
 
+from contrast_vendor import structlog as logging
+
+logger = logging.getLogger("contrast")
 
 HAS_FUNCHOOK = cs_str.has_funchook()
 ALWAYS_PURE_PYTHON_METHODS = ["format", "__repr__", "__getitem__"]
 
 
 class module(Namespace):
     hook = None
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/applicator.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/applicator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/constants.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/constants.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/patch_location_policy.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/patch_location_policy.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/patch_manager.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/patch_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,15 @@
         reverse_patches_by_owner(foo.FooClass)
 
     :param owner: module or class that owns the attribute being reverse patched
     """
     if owner is None:
         return
 
-    if id(owner) not in module.patches_by_owner:
-        return
-
-    for name in list(module.patches_by_owner[id(owner)]):
+    for name in list(module.patches_by_owner.get(id(owner), [])):
         _reverse_patch(owner, name)
 
 
 def reverse_module_patches_by_name(module_name: str):
     """
     Reverse patches owned by module with given name
 
@@ -149,15 +146,21 @@
     an attribute via repatching.
     """
     for owner_name in module.patches_by_name.copy():
         try:
             owner = import_module(owner_name)
         except ImportError:
             module_name, _, attr_name = owner_name.rpartition(".")
-            owner = getattr(import_module(module_name), attr_name)
+            try:
+                owner = getattr(import_module(module_name), attr_name)
+            except AttributeError:
+                # If the patched object is dynamic, it won't be exposed
+                # from the module. Currently, we don't have a way to reverse
+                # these patches.
+                continue
 
         reverse_patches_by_owner(owner)
 
 
 def register_patch(owner, name, orig_attr):
     """
     Register patch in the patch map to prevent us from patching twice
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/policy_node.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/policy_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/registry.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/registry.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/rewriter.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/rewriter.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/trigger_node.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/trigger_node.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/policy/utils.py` & `contrast_agent-8.0.0/src/contrast/agent/policy/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/input_analysis.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/input_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             and rule_tuple[1].enabled
             and rule_tuple[1].RULE_NAME in agent_lib.modules.CONSTANTS.RuleType
         ):
             rules |= agent_lib.modules.CONSTANTS.RuleType[rule_tuple[1].RULE_NAME]
     return rules
 
 
-def get_input_analysis(*, prefer_worth_watching=True):
+def analyze_inputs():
     """
-    Get input analysis from agent-lib. Results are stored on
+    Perform input analysis through agent-lib. Results are stored on
     context.user_input_analysis, which is reset every time this function is called.
 
     Some rules have a special "worth watching" analysis mode. In prefilter, we use this
     more liberal mode to ensure we don't miss attacks that should be blocked at trigger
     time. However, if we make it to the end of the request (without raising a
     SecurityException), we redo input analysis with worth watching mode disabled, which
     leads to more accurate PROBED results (fewer PROBED FPs).
@@ -51,163 +51,152 @@
 
     context.user_input_analysis = []
     exclusions = Settings().exclusions
 
     rules = _get_enabled_rules()
 
     # Input analysis for all the input_tracing.InputType enum values
-    _evaluate_headers(context, rules, prefer_worth_watching, exclusions)
-    _evaluate_cookies(context, rules, prefer_worth_watching, exclusions)
-    _evaluate_body(context, rules, prefer_worth_watching, exclusions)
-    _call_check_method_tampering(context, prefer_worth_watching)
-    _evaluate_query_string_params(context, rules, prefer_worth_watching, exclusions)
+    _evaluate_headers(context, rules, exclusions)
+    _evaluate_cookies(context, rules, exclusions)
+    _evaluate_body(context, rules, exclusions)
+    _call_check_method_tampering(context)
+    _evaluate_query_string_params(context, rules, exclusions)
     _call_agent_lib_evaluate_input(
         agent_lib.modules.CONSTANTS.InputType.get("UriPath"),
         context.request.path,
         rules,
-        prefer_worth_watching,
         context,
     )
-    _evaluate_path_params(context, rules, prefer_worth_watching, exclusions)
-    _evaluate_multipart_request(context, rules, prefer_worth_watching)
+    _evaluate_path_params(context, rules, exclusions)
+    _evaluate_multipart_request(context, rules)
 
 
-def _evaluate_headers(context, rules, prefer_worth_watching, exclusions):
+def _evaluate_headers(context, rules, exclusions):
     for header_name, header_value in context.request.headers.items():
         if "cookie" in header_name.lower() or check_param_input_exclusions(
             exclusions, "HEADER", header_name
         ):
             continue
 
         input_analysis = agent_lib.evaluate_header_input(
-            header_name, header_value, rules, prefer_worth_watching
+            header_name,
+            header_value,
+            rules,
+            prefer_worth_watching=True,
         )
 
         if input_analysis:
             context.user_input_analysis.extend(input_analysis)
             # Report and block attack if necessary
             _report_and_block_by_rule_list(
                 input_analysis,
                 ["bot-blocker", "reflected-xss", "unsafe-file-upload"],
                 context,
             )
 
 
-def _evaluate_cookies(context, rules, prefer_worth_watching, exclusions):
+def _evaluate_cookies(context, rules, exclusions):
     for cookie_name, cookie_value in context.request.cookies.items():
         if check_param_input_exclusions(exclusions, "COOKIE", cookie_name):
             continue
 
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("CookieName"),
             cookie_name,
             rules,
-            prefer_worth_watching,
             context,
         )
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("CookieValue"),
             cookie_value,
             rules,
-            prefer_worth_watching,
             context,
         )
 
 
 @fail_quietly("Failed to evaluate body")
-def _evaluate_body(context, rules, prefer_worth_watching, exclusions):
+def _evaluate_body(context, rules, exclusions):
     if check_url_input_exclusion(exclusions, "BODY", context.request.url):
         return
 
     body_type = context.request._get_document_type()
     if body_type == DocumentType.JSON:
-        _evaluate_body_json(context, rules, prefer_worth_watching, context.request.json)
+        _evaluate_body_json(context, rules, context.request.json)
     elif body_type == DocumentType.XML:
         data = xml.etree.ElementTree.fromstring(context.request.body)
         text_list = [element.text for element in data]
 
         for text in text_list:
             if not str(text).startswith("\n"):
                 _call_agent_lib_evaluate_input(
                     agent_lib.modules.CONSTANTS.InputType.get("XmlValue"),
                     str(text),
                     rules,
-                    prefer_worth_watching,
                     context,
                 )
     else:
-        _evaluate_key_value_parameters(
-            context, rules, prefer_worth_watching, querystring=False
-        )
+        _evaluate_key_value_parameters(context, rules, querystring=False)
 
 
-def _evaluate_body_json(context, rules, prefer_worth_watching, body):
+def _evaluate_body_json(context, rules, body):
     # TODO: PYT-2826
     # Using recursion for now to get all the json values and keys and pass them
     # through agent_lib until agent_lib implements parsing of the body for python
     if isinstance(body, dict):
         for key, value in body.items():
             _call_agent_lib_evaluate_input(
                 agent_lib.modules.CONSTANTS.InputType.get("JsonKey"),
                 key,
                 rules,
-                prefer_worth_watching,
                 context,
             )
             # This check is to skip a level in the recursion, just a minor optimization
             if isinstance(value, (dict, list)):
-                _evaluate_body_json(context, rules, prefer_worth_watching, value)
+                _evaluate_body_json(context, rules, value)
             else:
                 _call_agent_lib_evaluate_input(
                     agent_lib.modules.CONSTANTS.InputType.get("JsonValue"),
                     value,
                     rules,
-                    prefer_worth_watching,
                     context,
                 )
     elif isinstance(body, list):
         for item in body:
             if isinstance(item, (dict, list)):
-                _evaluate_body_json(context, rules, prefer_worth_watching, item)
+                _evaluate_body_json(context, rules, item)
             else:
                 _call_agent_lib_evaluate_input(
                     agent_lib.modules.CONSTANTS.InputType.get("JsonValue"),
                     item,
                     rules,
-                    prefer_worth_watching,
                     context,
                 )
     else:
         # In theory we shouldn't enter this block but I would like to have it
         # just in case we get a value instead of dict
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("JsonValue"),
             body,
             rules,
-            prefer_worth_watching,
             context,
         )
 
 
-def _evaluate_query_string_params(context, rules, prefer_worth_watching, exclusions):
+def _evaluate_query_string_params(context, rules, exclusions):
     """
     Get agent-lib input analysis for all query parameters. This information is stored on
     request context.
     """
     if check_url_input_exclusion(exclusions, "QUERYSTRING", context.request.url):
         return
 
-    _evaluate_key_value_parameters(
-        context, rules, prefer_worth_watching, querystring=True
-    )
+    _evaluate_key_value_parameters(context, rules, querystring=True)
 
 
-def _evaluate_key_value_parameters(
-    context, rules, prefer_worth_watching, *, querystring: bool
-) -> None:
+def _evaluate_key_value_parameters(context, rules, *, querystring: bool) -> None:
     """
     Used for both form parameters (from the request body) and query string parameters
     """
     if querystring:
         param_dict = context.request.GET
     else:
         param_dict = context.request.POST
@@ -216,88 +205,83 @@
         if not isinstance(param_value, str):
             continue
 
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("ParameterKey"),
             param_key,
             rules,
-            prefer_worth_watching,
             context,
             is_querystring=querystring,
         )
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("ParameterValue"),
             param_value,
             rules,
-            prefer_worth_watching,
             context,
             is_querystring=querystring,
         )
 
 
-def _evaluate_path_params(context, rules, prefer_worth_watching, exclusions):
+def _evaluate_path_params(context, rules, exclusions):
     """
     Get agent-lib input analysis for all path parameters. This information is
     stored on request context.
     """
     for param in context.request.get_url_parameters():
         if check_param_input_exclusions(exclusions, "PARAMETER", param):
             continue
 
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("UrlParameter"),
             param,
             rules,
-            prefer_worth_watching,
             context,
         )
 
 
-def _evaluate_multipart_request(context, rules, prefer_worth_watching):
+def _evaluate_multipart_request(context, rules):
     """
     This is refering to Content-Type: multipart/form-data and checking the file_name for every
     multipart request if there is none it checks the name
     """
     for key, value in context.request.get_multipart_headers().items():
         if value is None and key is None:
             continue
 
         multipart_name = value if value is not None else key
         _call_agent_lib_evaluate_input(
             agent_lib.modules.CONSTANTS.InputType.get("MultipartName"),
             multipart_name,
             rules,
-            prefer_worth_watching,
             context,
         )
 
 
-def _call_check_method_tampering(context, prefer_worth_watching):
+def _call_check_method_tampering(context):
     input_analysis_value = agent_lib.check_method_tampering(
-        context.request.method, prefer_worth_watching
+        context.request.method, prefer_worth_watching=True
     )
 
     if input_analysis_value:
         context.user_input_analysis.extend(input_analysis_value)
         _report_and_block_by_rule_list(
             input_analysis_value, ["reflected-xss", "unsafe-file-upload"], context
         )
 
 
 def _call_agent_lib_evaluate_input(
     input_type,
     input_value,
     rule_set,
-    prefer_worth_watching,
     context,
     *,
     is_querystring=False,
 ):
     input_analysis_value = agent_lib.evaluate_input_by_type(
-        input_type, input_value, rule_set, prefer_worth_watching
+        input_type, input_value, rule_set, prefer_worth_watching=True
     )
 
     if input_analysis_value:
         # This check is specific for querystring because agent-lib doesn't have a way to distinguish
         # url parameter and querystring and TS is expecting it as QUERYSTRING in attack samples
         if is_querystring:
             for input_analysis in input_analysis_value:
@@ -317,18 +301,22 @@
     :param rule_names: list of names of rules that need to be checked and reported and blocked
     :return: doesn't return anything as it just needs to report and block if needed
     """
     settings = Settings()
     for input_row in input_analysis:
         for rule_name in rule_names:
             rule = settings.protect_rules.get(rule_name)
+
             # Bot blocker rule is valid only when the input_row.name/header name is "user-agent"
-            bot_blocker_header_check = lambda a, rule_name_val: (
-                a.lower() == "user-agent" if rule_name_val == "bot-blocker" else True
-            )
+            def bot_blocker_header_check(a, rule_name_val):
+                return (
+                    a.lower() == "user-agent"
+                    if rule_name_val == "bot-blocker"
+                    else True
+                )
 
             if rule_name == input_row.rule_id:
                 attack = rule.build_attack_with_match(input_row.value, input_row, None)
                 context.attacks.append(attack)
 
             if (
                 bot_blocker_header_check(input_row.key, rule_name)
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/policy/__init__.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/base_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/base_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,28 @@
 
 import contrast
 from contrast.agent import scope
 from contrast.agent.settings import Settings
 from contrast.api.attack import Attack, ProtectResponse
 from contrast.api.user_input import UserInput, InputType
 from contrast.api.sample import Sample
-from contrast.agent.protect.rule import ProtectionRule
+from contrast.agent.protect.rule.mode import Mode
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils.decorators import cached_property
 from contrast.utils.stack_trace_utils import build_and_clean_stack
 from contrast_vendor import structlog as logging
 from contrast.utils.loggers.logger import security_log_msg
 from contrast.utils.string_utils import ensure_string
 
 logger = logging.getLogger("contrast")
 
 
-BLOCKING_RULES = frozenset([ProtectionRule.BLOCK, ProtectionRule.BLOCK_AT_PERIMETER])
-PREFILTER_RULES = frozenset([ProtectionRule.BLOCK_AT_PERIMETER])
-POSTFILTER_RULES = frozenset(
-    [ProtectionRule.BLOCK, ProtectionRule.MONITOR, ProtectionRule.PERMIT]
-)
+BLOCKING_RULES = frozenset([Mode.BLOCK, Mode.BLOCK_AT_PERIMETER])
+PREFILTER_RULES = frozenset([Mode.BLOCK_AT_PERIMETER])
+POSTFILTER_RULES = frozenset([Mode.BLOCK, Mode.MONITOR, Mode.PERMIT])
 
 PREFILTER = "prefilter"
 INFILTER = "infilter"
 POSTFILTER = "postfilter"
 
 
 class BaseRule:
@@ -94,15 +92,15 @@
         if disabled_rules and self.name in disabled_rules:
             return False
 
         req_ctx = contrast.CS__CONTEXT_TRACKER.current()
         if req_ctx is not None and req_ctx.excluded_protect_rules:
             return self.name not in req_ctx.excluded_protect_rules
 
-        return self.mode != ProtectionRule.OFF
+        return self.mode != Mode.OFF
 
     def should_block(self, attack):
         return attack and attack.response == ProtectResponse.BLOCKED
 
     def excluded(self, exclusions):
         """
         Check if rule is being excluded from evaluation
@@ -134,15 +132,15 @@
             raise contrast.SecurityException(rule_name=self.name)
 
     def _infilter(self, match_string, **kwargs):
         """
         Scans the input analysis for the rule and looks for matched attack signatures. The call to this method may be
         rule specific and include additional context in a args list.
         """
-        if self.mode in [ProtectionRule.OFF, ProtectionRule.PERMIT]:
+        if self.mode in [Mode.OFF, Mode.PERMIT]:
             return
 
         logger.debug("PROTECT: Infilter for %s", self.name)
 
         attack = self.find_attack(match_string, analysis_stage=INFILTER, **kwargs)
         if attack is None or len(attack.samples) == 0:
             return
@@ -201,15 +199,15 @@
         """
         Scans the input analysis for the rule and looks for matched attack signatures
 
         Appends attacker to the context if a positive evaluation is found
         """
         logger.debug("PROTECT: Postfilter for %s", self.name)
 
-        if self.mode in [ProtectionRule.OFF, ProtectionRule.PERMIT]:
+        if self.mode in [Mode.OFF, Mode.PERMIT]:
             return
 
         attack = self.find_attack(analysis_stage=POSTFILTER)
         if attack is None or len(attack.samples) == 0:
             return
 
         self._append_to_context(attack)
@@ -226,15 +224,14 @@
 
         evaluations_for_rule = self.evaluations_for_rule()
 
         attack = None
         for evaluation in evaluations_for_rule:
             if analysis_stage == POSTFILTER and evaluation.attack_count > 0:
                 continue
-
             if candidate_string:
                 if candidate_string.find(evaluation.value) == -1:
                     continue
 
                 attack = self.build_attack_with_match(
                     candidate_string, evaluation, attack, **kwargs
                 )
@@ -254,15 +251,17 @@
             evaluation.attack_count += 1
 
         attack.set_response(self.response_from_mode(self.mode))
         self.log_rule_matched(evaluation, attack.response, candidate_string)
         return attack
 
     def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
-        if self.mode == ProtectionRule.BLOCK_AT_PERIMETER:
+        if evaluation and evaluation.score < 10:
+            return None
+        if self.mode == Mode.BLOCK_AT_PERIMETER:
             attack = self.build_or_append_attack(evaluation, attack, **kwargs)
 
             attack.set_response(self.response_from_mode(self.mode))
             self.log_rule_matched(evaluation, attack.response)
         elif evaluation is None or evaluation.attack_count == 0:
             attack = self.build_or_append_attack(evaluation, attack, **kwargs)
             attack.set_response(ProtectResponse.PROBED)
@@ -364,26 +363,27 @@
             # do not remove; this case is not yet well-understood
             logger.debug("WARNING: failed to get request context in _append_to_context")
             return
 
         context.attacks.append(attack)
 
     _RESPONSE_MAP = {
-        ProtectionRule.MONITOR: ProtectResponse.MONITORED,
-        ProtectionRule.BLOCK: ProtectResponse.BLOCKED,
-        ProtectionRule.BLOCK_AT_PERIMETER: ProtectResponse.BLOCKED_AT_PERIMETER,
-        ProtectionRule.OFF: ProtectResponse.NO_ACTION,
-        ProtectionRule.PERMIT: ProtectResponse.NO_ACTION,
+        Mode.MONITOR: ProtectResponse.MONITORED,
+        Mode.BLOCK: ProtectResponse.BLOCKED,
+        Mode.BLOCK_AT_PERIMETER: ProtectResponse.BLOCKED_AT_PERIMETER,
+        Mode.OFF: ProtectResponse.NO_ACTION,
+        Mode.PERMIT: ProtectResponse.NO_ACTION,
     }
 
     def response_from_mode(self, mode):
         return self._RESPONSE_MAP.get(mode)
 
-    def evaluations_for_rule(self):
-        context = contrast.CS__CONTEXT_TRACKER.current()
+    def evaluations_for_rule(self, context=None):
+        if context is None:
+            context = contrast.CS__CONTEXT_TRACKER.current()
         if context is None:
             # do not remove; this case is not yet well-understood
             logger.debug(
                 "WARNING: failed to get request context in evaluations_for_rule"
             )
             return []
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/cmdi_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/cmdi_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
 
 from contrast.agent.agent_lib.input_tracing import check_cmd_injection_query
+from contrast.agent.protect.rule.mode import Mode
 from .base_rule import BaseRule
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
@@ -50,14 +51,31 @@
 
         if attack is not None:
             attack.set_response(self.response_from_mode(self.mode))
             self.log_rule_matched(evaluation, attack.response, candidate_string)
 
         return attack
 
+    def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
+        if self.mode == Mode.BLOCK_AT_PERIMETER:
+            return super().build_attack_without_match(evaluation, attack, **kwargs)
+        if evaluation.score < 10:
+            return None
+
+        return next(
+            (
+                super(CmdInjection, self).build_attack_without_match(
+                    full_eval, attack, **kwargs
+                )
+                for full_eval in evaluation.fully_evaluate()
+                if full_eval.score >= 90
+            ),
+            None,
+        )
+
     def build_sample(self, evaluation, command, **kwargs):
         sample = self.build_base_sample(evaluation)
         if command is not None:
             sample.details["command"] = command
 
         if "startIndex" in kwargs:
             sample.details["startIndex"] = int(kwargs["startIndex"])
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/deserialization_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/deserialization_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/http_method_tampering.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/http_method_tampering.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/nosqli_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/nosqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/path_traversal_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/path_traversal_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/rules_builder.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/rules_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,14 @@
             BotBlocker.RULE_NAME: BotBlocker(),
             CmdInjection.RULE_NAME: CmdInjection(),
             Deserialization.RULE_NAME: Deserialization(),
             # Turned off until TS can handle rule information
             MalformedHeader.RULE_NAME: MalformedHeader(),
             MethodTampering.RULE_NAME: MethodTampering(),
             NoSqlInjection.RULE_NAME: NoSqlInjection(),
-            # Padding Oracle rule is currently disabled - CONTRAST-35352
-            # PaddingOracle.RULE_NAME: PaddingOracle(),
             PathTraversal.RULE_NAME: PathTraversal(),
             SqlInjection.RULE_NAME: SqlInjection(),
             Ssrf.RULE_NAME: Ssrf(),
             Xss.RULE_NAME: Xss(),
             Xxe.RULE_NAME: Xxe(),
         }
     )
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/sqli_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/sqli_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
 from contrast.agent.protect.rule.base_rule import BaseRule
 from contrast.agent import agent_lib
+from contrast.agent.protect.rule.mode import Mode
 
 
 class SqlInjection(BaseRule):
     """
     SQL Injection Protection rule
     """
 
@@ -40,14 +41,31 @@
 
         if attack is not None:
             attack.set_response(self.response_from_mode(self.mode))
             self.log_rule_matched(evaluation, attack.response, candidate_string)
 
         return attack
 
+    def build_attack_without_match(self, evaluation=None, attack=None, **kwargs):
+        if self.mode == Mode.BLOCK_AT_PERIMETER:
+            return super().build_attack_without_match(evaluation, attack, **kwargs)
+        if evaluation.score < 10:
+            return None
+
+        return next(
+            (
+                super(SqlInjection, self).build_attack_without_match(
+                    full_eval, attack, **kwargs
+                )
+                for full_eval in evaluation.fully_evaluate()
+                if full_eval.score >= 90
+            ),
+            None,
+        )
+
     def build_sample(self, evaluation, query, **kwargs):
         sample = self.build_base_sample(evaluation)
         if query is not None:
             sample.details["query"] = query
 
         if "start_idx" in kwargs:
             sample.details["start"] = int(kwargs["start_idx"])
@@ -71,13 +89,7 @@
         Some sql libraries use special objects (see from sqlalchemy import text)
         so we cannot just check if user_input is falsy.
         """
         if user_input is None:
             return True
 
         return False
-
-    def convert_input(self, user_input):
-        if not isinstance(user_input, (str, bytes)):
-            user_input = str(user_input)
-
-        return user_input
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/ssrf_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/ssrf_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xss_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xss_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from contrast.agent.protect.rule.base_rule import BaseRule
-from contrast.agent.protect.rule import ProtectionRule
+from contrast.agent.protect.rule.mode import Mode
 
 
 class Xss(BaseRule):
     """
     Cross Site Scripting Protection rule
     Currently only a prefilter / block at perimeter rule
     """
 
     RULE_NAME = "reflected-xss"
 
+    def is_prefilter(self):
+        return self.enabled
+
     @property
     def mode(self):
         """
         Always block at perimeter
         """
         mode = self.settings.config.get_value(self.config_rule_path_mode)
 
-        return (
-            ProtectionRule.BLOCK_AT_PERIMETER if mode == ProtectionRule.BLOCK else mode
-        )
+        return Mode.BLOCK_AT_PERIMETER if mode == Mode.BLOCK else mode
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/protect/rule/xxe_rule.py` & `contrast_agent-8.0.0/src/contrast/agent/protect/rule/xxe_rule.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/reaction_processor.py` & `contrast_agent-8.0.0/src/contrast/agent/reaction_processor.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/request.py` & `contrast_agent-8.0.0/src/contrast/agent/request.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/request_context.py` & `contrast_agent-8.0.0/src/contrast/agent/request_context.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/request_state.py` & `contrast_agent-8.0.0/src/contrast/agent/request_state.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/runner.py` & `contrast_agent-8.0.0/src/contrast/agent/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 
     if config.enable_automatic_middleware:
         register_middleware_patches()
 
     if config.assess_enabled:
         # NOTE: policy is currently loaded/generated on import. It is applied explicitly
         # in policy/applicator.py later
-        from contrast import policy  # pylint: disable=unused-import
+        from contrast import policy  # noqa: F401
 
         enable_assess_patches()
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/scope.py` & `contrast_agent-8.0.0/src/contrast/agent/scope.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/server_settings_poll.py` & `contrast_agent-8.0.0/src/contrast/agent/server_settings_poll.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/settings.py` & `contrast_agent-8.0.0/src/contrast/agent/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 # pylint: disable=too-many-lines
 from collections import defaultdict
 import os
 import pathlib
 from datetime import datetime, timezone
 import json
+from typing import List, Optional
 from urllib.parse import urlparse
 
 from contrast import AGENT_CURR_WORKING_DIR
 
 from contrast.utils.decorators import fail_quietly
-from contrast.agent.exclusions import Exclusions, TsExclusion, ExclusionType
+from contrast.agent.exclusions import Exclusions, TsExclusion
 from contrast.agent.framework import Framework, Server
 from contrast.agent.reaction_processor import ReactionProcessor
-from contrast.agent.protect.rule import ProtectionRule
 from contrast.configuration.config_option import (
     CONTRAST_UI_SRC,
     USER_CONFIGURATION_FILE_SRC,
     DEFAULT_VALUE_SRC,
 )
 from contrast.configuration.agent_config import AgentConfig
 from contrast.utils.decorators import cached_property
@@ -31,152 +31,14 @@
 logger = logging.getLogger("contrast")
 
 ASSESS_STACKTRACES = "assess.stacktraces"
 ASSESS_DISABLED_RULE_CONFIG_KEY = "assess.rules.disabled_rules"
 EXPORTED_CONFIG_FILE_NAME = "contrast_connection.json"
 
 
-class ServerFeatures:
-    def __init__(self, features):
-        self.features = features or {}
-
-    @cached_property
-    def log_file(self):
-        return self.features.get("features", {}).get("logFile", "")
-
-    @cached_property
-    def log_level(self):
-        return self.features.get("features", {}).get("logLevel", "")
-
-    @cached_property
-    def assess_enabled(self):
-        return (
-            self.features.get("features", {})
-            .get("assessment", {})
-            .get("enabled", False)
-        )
-
-    @cached_property
-    def protect_enabled(self):
-        return self.features.get("features", {}).get("defend", {}).get("enabled", False)
-
-
-class ApplicationSettings:
-    def __init__(self, settings_json=None):
-        self._raw_settings = settings_json or {}
-
-    @cached_property
-    def disabled_assess_rules(self):
-        return (
-            self._raw_settings.get("settings", {})
-            .get("assessment", {})
-            .get("disabledRules", [])
-        )
-
-    @cached_property
-    def protection_rules(self):
-        return [
-            ProtectRule(r)
-            for r in self._raw_settings.get("settings", {})
-            .get("defend", {})
-            .get("protectionRules", [])
-        ]
-
-    @cached_property
-    def session_id(self):
-        return (
-            self._raw_settings.get("settings", {})
-            .get("assessment", {})
-            .get("session_id", None)
-        )
-
-    @cached_property
-    def sensitive_data_masking_policy(self):
-        return self._raw_settings.get("settings", {}).get(
-            "sensitive_data_masking_policy"
-        )
-
-    @cached_property
-    def exclusions(self):
-        """
-        Build and return a plain list of TsExclusions based on raw application settings.
-        TsExclusions represent the exclusions more or less exactly as they were given to
-        us by teamserver.
-
-        The list returned by this property will be converted into our own Exclusions
-        class later, which is more useful when processing exclusion rules.
-        """
-        ts_exclusions = self._raw_settings.get("settings", {}).get("exceptions")
-        if ts_exclusions is None:
-            return None
-
-        exclusions = []
-
-        for exclusion in ts_exclusions.get("urlExceptions", []):
-            exclusions.append(
-                TsExclusion(
-                    ExclusionType.URL_EXCLUSION_TYPE,
-                    exclusion.get("name", ""),
-                    exclusion.get("modes", []),
-                    exclusion.get("matchStrategy", ""),
-                    exclusion.get("protectionRules", []),
-                    exclusion.get("assessmentRules", []),
-                    exclusion.get("urls", []),
-                )
-            )
-
-        for exclusion in ts_exclusions.get("inputExceptions", []):
-            exclusions.append(
-                TsExclusion(
-                    ExclusionType.INPUT_EXCLUSION_TYPE,
-                    exclusion.get("name", ""),
-                    exclusion.get("modes", []),
-                    exclusion.get("matchStrategy", ""),
-                    exclusion.get("protectionRules", []),
-                    exclusion.get("assessmentRules", []),
-                    exclusion.get("urls", []),
-                    exclusion.get("inputType", ""),
-                    exclusion.get("inputName", ""),
-                )
-            )
-
-        return exclusions
-
-    # note: there are more fields on ApplicationSettings that we currently don't use
-
-
-class ProtectRule:
-    def __init__(self, protect_rule_json):
-        self._raw_rule = protect_rule_json or {}
-
-    @cached_property
-    def id(self):
-        return self._raw_rule.get("id", "")
-
-    @cached_property
-    def mode(self):
-        raw_mode = self._raw_rule.get("mode", "OFF")
-        raw_block_at_entry = self._raw_rule.get("blockAtEntry", False)
-
-        # Common configuration uses lower case infinitives whereas TeamServer UI uses
-        # capital present participles. This mapping has to handle both.
-        return {
-            "MONITOR": ProtectionRule.MONITOR,
-            "MONITORING": ProtectionRule.MONITOR,
-            "BLOCK": ProtectionRule.BLOCK,
-            "BLOCKING": (
-                ProtectionRule.BLOCK_AT_PERIMETER
-                if raw_block_at_entry
-                else ProtectionRule.BLOCK
-            ),
-            "BLOCK_AT_PERIMETER": ProtectionRule.BLOCK_AT_PERIMETER,
-            "OFF": ProtectionRule.OFF,
-        }[raw_mode.upper()]
-
-
 class Settings(Singleton):
     def init(self, app_name=None, framework_name=None):
         """
         Agent settings for the entire lifetime of the agent.
 
         Singletons should override init, not __init__.
         """
@@ -192,16 +54,14 @@
         self.sys_module_count = 0
 
         # Server
         self.server_name = None
         self.server_path = None
         self.server_type = None
 
-        self.exclusion_matchers = []
-
         # Rules
         self.protect_rules = dict()
 
         # circular import
         from contrast.agent.assess.rules.response.autocomplete_missing_rule import (
             AutocompleteMissingRule,
         )
@@ -362,16 +222,16 @@
 
         pid must be unique for each worker process of an app.
         :return: int current process id
         """
         return os.getpid()
 
     def get_app_name(self, app_name):
-        if self.config.get_value("application.name"):
-            return self.config.get_value("application.name")
+        if config_name := self.config.get_value("application.name"):
+            return config_name
 
         return app_name if app_name else "root"
 
     def establish_heartbeat(self):
         """
         Initialize Heartbeat between Agent and TS if it has not been already initialized.
         """
@@ -392,25 +252,23 @@
 
             self.server_settings_poll = ServerSettingsPoll()
             self.server_settings_poll.start()
 
     def set_protect_assess_config_source(self, server_features):
         if self.config is None or server_features is None:
             return
-
-        assess_option = self.config.get("assess.enable")
-        if assess_option:
-            assess_option.ui_value = server_features.assess_enabled
-
-        protect_option = self.config.get("protect.enable")
-        if protect_option:
-            protect_option.ui_value = server_features.protect_enabled
+        self.config.set_ui_value("assess.enable", server_features.assess_enabled)
+        self.config.set_ui_value("protect.enable", server_features.protect_enabled)
 
     def apply_ts_feature_settings(self, response_body):
-        server_features = ServerFeatures(response_body)
+        from contrast.reporting.teamserver_responses.ng_server_settings import (
+            NGServerSettings,
+        )
+
+        server_features = NGServerSettings(response_body)
         self.log_server_features(server_features)
         self.update_sampling(server_features)
         self.update_logger_from_features(server_features)
         self.set_protect_assess_config_source(server_features)
         self.set_protect_rules()
         self.last_server_update_time_ms = now_ms()
 
@@ -433,72 +291,120 @@
         """
         logger.debug(
             "Received updated server features logFile=%s logLevel=%s Protect=%s Assess=%s Sampling=%s",
             server_features.log_file,
             server_features.log_level,
             server_features.protect_enabled,
             server_features.assess_enabled,
-            server_features.features.get("features", {})
-            .get("assessment", {})
-            .get("sampling", None),
+            server_features.sampling,
         )
 
-    @property
-    def code_exclusion_matchers(self):
-        return [x for x in self.exclusion_matchers if x.is_code]
-
-    def load_exclusions_from_server(self, exclusions):
+    def load_exclusions_from_server(self, exclusions: List[TsExclusion]):
         if exclusions:
             self.exclusions = Exclusions(exclusions)
 
     def evaluate_exclusions(self, context, path):
         if self.exclusions:
             if self.exclusions.evaluate_url_exclusions(context, path):
                 # Stop analyzing this endpoint since the URL exclusion applies
                 return True
 
             if self.exclusions.input_exclusions:
                 self.exclusions.set_input_exclusions_by_url(context, path)
 
         return False
 
-    def apply_ts_app_settings(self, response_json):
-        app_settings = ApplicationSettings(response_json)
+    def apply_application_settings(self, application_settings_json: dict):
+        from contrast.reporting.teamserver_responses.application_settings import (
+            ApplicationSettings,
+        )
+
+        logger.debug("Application settings", settings_json=application_settings_json)
+        app_settings = ApplicationSettings(application_settings_json)
         self.sensitive_data_masking_policy = app_settings.sensitive_data_masking_policy
         if app_settings.exclusions:
             self.load_exclusions_from_server(app_settings.exclusions)
+        self.config.set_ui_value(
+            ASSESS_DISABLED_RULE_CONFIG_KEY, app_settings.disabled_assess_rules
+        )
+        # This is the only place session_id is set by TS.
+        # If session id is set in the config, that value will be echoed back by TS
+        if app_settings.session_id:
+            self.config.set_ui_value("application.session_id", app_settings.session_id)
 
-        disabled_rule_option = self.config.get(ASSESS_DISABLED_RULE_CONFIG_KEY)
-        disabled_rule_option.ui_value = app_settings.disabled_assess_rules
+        # In order to update all the rules based on latest TS settings, we need to make sure that any rule not
+        # mentioned by TS, or more likely our tests, have their UI value reset.
+        self.set_protect_rules()
+        known_rules = set(self.protect_rules)
+        logger.debug("Checking for rules: %s", known_rules)
+        if app_settings.protect_rules:
+            for definition in app_settings.protect_rules:
+                logger.debug("Definition: %s  --- %s", definition.id, definition.mode)
+                self.config.set_ui_value(
+                    f"protect.rules.{definition.id}.mode", definition.mode
+                )
+                if definition.id in known_rules:
+                    known_rules.remove(definition.id)
+        logger.debug("Remaining rules: %s", known_rules)
+        for rule_name in known_rules:
+            self.config.set_ui_value(f"protect.rules.{rule_name}.mode", None)
+        self.last_app_update_time_ms = now_ms()
+
+    def apply_identification(self, identification_json: Optional[dict]):
+        if not identification_json:
+            return
+        self.application_uuid = identification_json.get("application_uuid", None)
+        self.organization_uuid = identification_json.get("organization_uuid", None)
+        self.server_uuid = identification_json.get("server_uuid", None)
+        self.session_id = identification_json.get("session_id", None)
+
+    def apply_server_settings(self, server_settings_json: dict):
+        from contrast.reporting.teamserver_responses.server_settings import (
+            ServerSettings,
+        )
+
+        server_features = ServerSettings(server_settings_json)
+        self.log_server_features(server_features)
+        self.update_sampling(server_features)
+        self.update_logger_from_features(server_features)
+        self.set_protect_assess_config_source(server_features)
+        self.set_protect_rules()
+        self.last_server_update_time_ms = now_ms()
+
+    def apply_ng_app_settings(self, response_json):
+        from contrast.reporting.teamserver_responses.ng_application_settings import (
+            NGApplicationSettings,
+        )
+
+        app_settings = NGApplicationSettings(response_json)
+        self.sensitive_data_masking_policy = app_settings.sensitive_data_masking_policy
+        if app_settings.exclusions:
+            self.load_exclusions_from_server(app_settings.exclusions)
+
+        self.config.set_ui_value(
+            ASSESS_DISABLED_RULE_CONFIG_KEY, app_settings.disabled_assess_rules
+        )
 
         # This is the only place session_id is set by TS.
         # If session id is set in the config, that value will be echoed back by TS
         if app_settings.session_id:
-            id_option = self.config.get("application.session_id")
-            id_option.ui_value = app_settings.session_id
+            self.config.set_ui_value("application.session_id", app_settings.session_id)
 
         # In order to update all the rules based on latest TS settings, we need to make sure that any rule not
         # mentioned by TS, or more likely our tests, have their UI value reset.
-        known_rules = []
-        for rule in self.protect_rules:
-            known_rules.append(rule)
+        known_rules = set(self.protect_rules)
         if app_settings.protection_rules:
             for definition in app_settings.protection_rules:
-                rule_key = f"protect.rules.{definition.id}.mode"
-                rule_option = self.config.get(rule_key)
-                # Sometimes there are rules we don't know about that TeamServer sends us :(
-                if rule_option:
-                    rule_option.ui_value = definition.mode
+                self.config.set_ui_value(
+                    f"protect.rules.{definition.id}.mode", definition.mode
+                )
                 if definition.id in known_rules:
                     known_rules.remove(definition.id)
         for rule_name in known_rules:
-            rule_key = f"protect.rules.{rule_name}.mode"
-            rule_option = self.config.get(rule_key)
-            if rule_option:
-                rule_option.ui_value = None
+            self.config.set_ui_value(f"protect.rules.{rule_name}.mode", None)
 
     def update_logger_from_features(self, server_features):
         if server_features is None:
             return
 
         logger_reset = reset_agent_logger(
             server_features.log_file,
@@ -533,18 +439,14 @@
 
     def is_protect_enabled(self):
         if self.config is None:
             return False
         return self.config.get_value("protect.enable")
 
     def set_protect_rules(self):
-        if not self.is_protect_enabled():
-            self.protect_rules = dict()
-            return
-
         from contrast.agent.protect.rule.rules_builder import build_protect_rules
 
         self.protect_rules = build_protect_rules()
 
     def get_server_name(self):
         """
         Hostname of the server
@@ -631,39 +533,27 @@
 
         return {}
 
     def update_sampling(self, server_features=None):
         if server_features is None:
             return
 
-        server_sampling = (
-            server_features.features.get("features", {})
-            .get("assessment", {})
-            .get("sampling")
-        )
+        server_sampling = server_features.sampling
         if server_sampling is None:
             return
 
-        sampling_enable = self.config.get("assess.sampling.enable")
-        if sampling_enable:
-            sampling_enable.ui_value = server_sampling.get("enabled", None)
-        sampling_baseline = self.config.get("assess.sampling.baseline")
-        if sampling_baseline:
-            sampling_baseline.ui_value = server_sampling.get("baseline", None)
-        sampling_request_frequency = self.config.get(
-            "assess.sampling.request_frequency"
-        )
-        if sampling_request_frequency:
-            sampling_request_frequency.ui_value = server_sampling.get("frequency", None)
-        sampling_window_ms = self.config.get("assess.sampling.window_ms")
-        if sampling_window_ms:
-            sampling_window_ms.ui_value = server_sampling.get("window", None)
+        self.config.set_ui_value("assess.sampling.enable", server_sampling.enable)
+        self.config.set_ui_value("assess.sampling.baseline", server_sampling.baseline)
+        self.config.set_ui_value(
+            "assess.sampling.request_frequency", server_sampling.request_frequency
+        )
+        self.config.set_ui_value("assess.sampling.window_ms", server_sampling.window_ms)
         logger.debug(
-            "Updated sampling setting with TeamServer sampling settings: %s",
-            server_sampling,
+            "Updated sampling setting with TeamServer sampling settings",
+            sampling_settings=server_sampling,
         )
 
     @cached_property
     def contrast_ui_status(self):
         config_name = "enable"
         error_msg = "Unable to connect to Contrast; configuration details from the Contrast UI will not be included."
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/sys_monitoring.py` & `contrast_agent-8.0.0/src/contrast/agent/sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/telemetry.py` & `contrast_agent-8.0.0/src/contrast/agent/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,17 @@
             try:
                 response = self._post(messages, path)
                 if retry_wait := self._retry_after(response):
                     # readd message so it can be sent again after retry_wait.
                     self._msgs[path] = messages
                     return retry_wait
             except Exception as ex:
-                logger.debug("Could not send batch of telemetry messages.", ex)
+                logger.debug(
+                    "Could not send batch of telemetry messages.", exception=str(ex)
+                )
 
         return self.WAIT
 
     def _store_message(self, msg):
         if self._msg_count >= self.MAX_MESSAGES:
             logger.debug(
                 "WARNING: message store limit reached, dropping message", msg=msg
```

### Comparing `contrast-agent-7.7.0/src/contrast/agent/thread_watcher.py` & `contrast_agent-8.0.0/src/contrast/agent/thread_watcher.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/agent/validator.py` & `contrast_agent-8.0.0/src/contrast/agent/validator.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/aiohttp/middleware.py` & `contrast_agent-8.0.0/src/contrast/aiohttp/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 
 import contrast
 
 from aiohttp.web import StreamResponse
 from aiohttp.web_urldispatcher import DynamicResource
 
 from contrast.aiohttp import sources
-from contrast.agent import scope, request_state
+from contrast.agent import scope, request_state, agent_state
 from contrast.agent.middlewares.route_coverage.aiohttp_routes import (
     create_aiohttp_routes,
 )
-from contrast.agent.middlewares.route_coverage.common import build_route
+from contrast.agent.middlewares.route_coverage.common import (
+    build_route,
+    log_discovered_routes,
+)
 from contrast.agent.policy.trigger_node import TriggerNode
 from contrast_vendor import structlog as logging
 from contrast.utils.decorators import cached_property
 from contrast.agent.middlewares.base_middleware import (
     BaseMiddleware,
     log_request_start_and_end,
 )
@@ -81,33 +84,54 @@
 
                 self.postfilter(context)
                 self.check_for_blocked(context)
 
                 return response
 
             finally:
+                if self.settings.is_assess_enabled():
+                    self.do_aiohttp_first_request_analysis()
+                    self.do_aiohttp_route_observation(context, request)
                 self.handle_ensure(context, request)
                 if self.settings.is_assess_enabled():
                     contrast.STRING_TRACKER.ageoff()
 
     async def call_without_agent_async(self, request, handler) -> StreamResponse:
         super().call_without_agent()
         with scope.contrast_scope():
             return await handler(request)
 
-    @fail_quietly("Unable to get route coverage", return_value={})
-    def get_route_coverage(self):
-        return create_aiohttp_routes(self.app)
-
-    @fail_quietly("Unable to build route", return_value="")
-    def build_route(self, view_func, url):
-        return build_route(url, view_func)
+    @fail_quietly()
+    def do_aiohttp_first_request_analysis(self) -> None:
+        if not agent_state.is_first_request():
+            return
+        discovered_routes = create_aiohttp_routes(self.app)
+        agent_state.update_routes(discovered_routes)
+        log_discovered_routes("aiohttp", discovered_routes.values())
+
+    @fail_quietly()
+    def do_aiohttp_route_observation(self, context, request) -> None:
+        view_func = self.get_aiohttp_view_func(request)
+        if view_func is None:
+            logger.debug("unable to get view function for aiohttp route observation")
+            return
+
+        context.view_func = view_func
+        context.view_func_str = build_route(
+            context.request.get_normalized_uri(), context.view_func
+        )
+        logger.debug("Observed aiohttp route: %s", context.view_func_str)
 
     @fail_quietly("Unable to get view func")
-    def get_view_func(self, request):
+    def get_aiohttp_view_func(self, request):
+        """
+        This intentionally does not override get_view_func. We're generally making route
+        coverage more framework-specific; this minimizes shared machinery between
+        aiohttp middleware and its base classes.
+        """
         if not self.request_path:
             return None
 
         view_func = None
 
         # This approach has at worst O(_resources) performance
         # but it's a first attempt at implementing a sync
```

### Comparing `contrast-agent-7.7.0/src/contrast/aiohttp/sources.py` & `contrast_agent-8.0.0/src/contrast/aiohttp/sources.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/architecture_component.py` & `contrast_agent-8.0.0/src/contrast/api/architecture_component.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/attack.py` & `contrast_agent-8.0.0/src/contrast/api/attack.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/finding.py` & `contrast_agent-8.0.0/src/contrast/api/finding.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/library.py` & `contrast_agent-8.0.0/src/contrast/api/library.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/route_coverage.py` & `contrast_agent-8.0.0/src/contrast/api/route_coverage.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/trace_event.py` & `contrast_agent-8.0.0/src/contrast/api/trace_event.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/type_checked_property.py` & `contrast_agent-8.0.0/src/contrast/api/type_checked_property.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/api/user_input.py` & `contrast_agent-8.0.0/src/contrast/api/user_input.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/applies/__init__.py` & `contrast_agent-8.0.0/src/contrast/applies/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/applies/assess/unsafe_code_execution.py` & `contrast_agent-8.0.0/src/contrast/applies/assess/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/applies/sqli.py` & `contrast_agent-8.0.0/src/contrast/applies/sqli.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/asgi/middleware.py` & `contrast_agent-8.0.0/src/contrast/asgi/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,14 +148,7 @@
             TriggerNode(module, class_name, instance_method, method_name, "RETURN"),
             args,
         )
 
     @cached_property
     def name(self):
         return "asgi"
-
-    def get_route_coverage(self):
-        """
-        ASGI has no concept of "routes", so we can't perform route discovery without a
-        framework
-        """
-        return {}
```

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/__init__.py` & `contrast_agent-8.0.0/src/contrast/assess_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/cast.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/cast.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/format.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/format.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/logging.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/logging.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/patches.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/patches.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/propagate.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/propagate.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/repeat.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/repeat.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/repr.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/repr.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/scope.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/scope.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/streams.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/streams.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/subscript.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/subscript.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/common/trace.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/common/trace.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/cs_str.pyi` & `contrast_agent-8.0.0/src/contrast/assess_extensions/cs_str.pyi`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/.travis.yml` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/.travis.yml`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/LICENSE` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/Makefile.in` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/README.md` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/appveyor.yml` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/appveyor.yml`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.guess` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.guess`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/config.sub` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/config.sub`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/configure.ac` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/configure.ac`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/COPYING` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/COPYING`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/README.md` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/README.md`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/setup.py` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/setup.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/config.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/config.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/include/funchook.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/include/funchook.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/install-sh` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/install-sh`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/Makefile.in` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/__strerror.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/__strerror.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_io.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_io.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/src/printf_base.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/src/printf_base.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/Makefile.in` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/suffix.list` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/suffix.list`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/test_main.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/test_main.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/test/x86_test.S` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/test/x86_test.S`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.sln` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.sln`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters` & `contrast_agent-8.0.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/logging.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/logging.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/patches.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/patches.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/scope.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/scope.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/include/contrast/assess/utils.h` & `contrast_agent-8.0.0/src/contrast/assess_extensions/include/contrast/assess/utils.h`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py3/patches.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py3/patches.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py3/str_concat.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py3/str_concat.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py310/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py310/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py311/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py311/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py312/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py312/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py35/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py35/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py36/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py36/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py37/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py37/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py38/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py38/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytearray.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytes.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/bytesio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/iobase.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/stringio.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/assess_extensions/py39/unicode.c` & `contrast_agent-8.0.0/src/contrast/assess_extensions/py39/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/agent.py` & `contrast_agent-8.0.0/src/contrast/configuration/agent.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/agent_config.py` & `contrast_agent-8.0.0/src/contrast/configuration/agent_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import re
+from typing import Optional
 
 from contrast.utils.configuration_utils import (
     DEFAULT_PATHS,
     load_yaml_config,
 )
 from contrast.utils.decorators import cached_property
 from contrast_vendor import structlog as logging
+from . import ConfigOption
 
 from .agent import Agent
 from .api import Api
 from .application import Application
 from .assess import Assess
 from .inventory import Inventory
 from .protect import Protect
@@ -56,22 +58,22 @@
 class AgentConfig:
     def __init__(self):
         self.config_status = None
         self._config = {}
         self.build_configs()
         self.check_for_api_config()
 
-    def get(self, key):
+    def get(self, key: str) -> Optional[ConfigOption]:
         return self._config.get(key, None)
 
-    def get_value(self, key):
+    def get_value(self, key: str):
         option = self.get(key)
         return option.value() if option else None
 
-    def get_loggable_value(self, key):
+    def get_loggable_value(self, key: str) -> Optional[str]:
         option = self.get(key)
         return option.loggable_value() if option else None
 
     def keys(self):
         return self._config.keys()
 
     def get_loggable_config(self):
@@ -156,15 +158,17 @@
 
     @session_id.setter
     def session_id(self, session_id):
         session_id_option = self.get("application.session_id")
         session_id_option.ui_value = session_id
 
         logger.debug(
-            "Set session_id to %s", session_id_option.value(), direct_to_teamserver=1
+            "Set session_id",
+            session_id=session_id_option.value(),
+            direct_to_teamserver=1,
         )
 
     def get_session_metadata(self):
         return self.get_value("application.session_metadata")
 
     @property
     def app_code(self):
@@ -251,7 +255,16 @@
                 return TESTING_TEAMSERVER_TYPE
 
         for name in PRIVATE_SASS_DOMAIN:
             if name in url:
                 return PRIVATE_SASS_TEAMSERVER_TYPE
 
         return DEFAULT_TEAMSERVER_TYPE
+
+    def set_ui_value(self, key: str, value: object):
+        """
+        We have to be safe here with unknown configuration options as TeamServer can send us settings for which we do
+        not have configurations. This most often happens when we're given configurations for rules that do not pertain
+        to this agent.
+        """
+        if config_option := self.get(key):
+            config_option.ui_value = value
```

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/api.py` & `contrast_agent-8.0.0/src/contrast/configuration/api.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/application.py` & `contrast_agent-8.0.0/src/contrast/configuration/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             ConfigOption(
                 # TODO: PYT-2852 Revisit application name detection
                 canonical_name="application.name",
                 default_value=os.path.basename(AGENT_CURR_WORKING_DIR),
                 type_cast=str,
             ),
             ConfigOption(
-                canonical_name="application.path", default_value="", type_cast=str
+                canonical_name="application.path", default_value="/", type_cast=str
             ),
             ConfigOption(
                 canonical_name="application.tags", default_value="", type_cast=str
             ),
             ConfigOption(
                 canonical_name="application.version", default_value="", type_cast=str
             ),
```

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/assess.py` & `contrast_agent-8.0.0/src/contrast/configuration/assess.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/config_builder.py` & `contrast_agent-8.0.0/src/contrast/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/config_option.py` & `contrast_agent-8.0.0/src/contrast/configuration/config_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 
+from contrast.utils.string_utils import removeprefix
+
 ENVIRONMENT_VARIABLE_SRC = "ENVIRONMENT_VARIABLE"
 USER_CONFIGURATION_FILE_SRC = "USER_CONFIGURATION_FILE"
 DEFAULT_VALUE_SRC = "DEFAULT_VALUE"
 CONTRAST_UI_SRC = "CONTRAST_UI"
 
 
 class ConfigOption:
@@ -27,15 +29,15 @@
             return self.env_value
         if self.file_values:
             return self.file_values[0]
         if self.ui_value is not None:
             return self.ui_value
         return self.default_value
 
-    def source(self):
+    def source(self) -> str:
         if self.env_value is not None:
             return ENVIRONMENT_VARIABLE_SRC
         if self.file_values:
             return USER_CONFIGURATION_FILE_SRC
         if self.ui_value is not None:
             return CONTRAST_UI_SRC
         return DEFAULT_VALUE_SRC
@@ -43,33 +45,33 @@
     def file_name(self):
         return (
             self.file_sources[0]
             if self.file_sources and self.source() == USER_CONFIGURATION_FILE_SRC
             else None
         )
 
-    def provided_name(self):
+    def provided_name(self) -> str:
         if self.name is not None:
             return self.name
         return self.canonical_name
 
-    def loggable_value(self):
+    def loggable_value(self) -> str:
         return self.to_string(self.value())
 
-    def to_string(self, raw_value):
+    def to_string(self, raw_value) -> str:
         # If the value is empty, just return empty String.
         if raw_value in (None, ""):
             return ""
         # If the option is sensitive, like an API credential, we do not log or report it.
         if self.redacted:
             return "**REDACTED**"
         str_value = str(raw_value)
         # If the option is an enum, we need to clean it up.
-        if str_value and str_value.startswith("ProtectionRule."):
-            return str_value.lstrip("ProtectionRule.").lower()
+        if str_value and str_value.startswith("Mode."):
+            return removeprefix(str_value, "Mode.").upper()
         return str_value
 
     def clear(self):
         """
         This is used as a convenience method during testing to ensure a clean slate.
         """
         self.override_value = None
```

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/inventory.py` & `contrast_agent-8.0.0/src/contrast/configuration/inventory.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/protect.py` & `contrast_agent-8.0.0/src/contrast/configuration/protect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 
 from .config_builder import ConfigBuilder
 from .config_option import ConfigOption
-from contrast.agent.protect.rule import ProtectionRule
+from contrast.agent.protect.rule.mode import Mode
 from contrast.utils.configuration_utils import (
     parse_disabled_rules,
     str_to_bool,
     str_to_protect_mode_enum,
 )
 
 
@@ -42,61 +42,61 @@
             ConfigOption(
                 canonical_name="protect.rules.bot-blocker.enable",
                 default_value=False,
                 type_cast=str_to_bool,
             ),
             ConfigOption(
                 canonical_name="protect.rules.cmd-injection.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.disabled_rules",
                 default_value=[],
                 type_cast=parse_disabled_rules,
             ),
             ConfigOption(
                 canonical_name="protect.rules.method-tampering.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.nosql-injection.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.path-traversal.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.reflected-xss.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.sql-injection.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.ssrf.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.unsafe-file-upload.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.untrusted-deserialization.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
             ConfigOption(
                 canonical_name="protect.rules.xxe.mode",
-                default_value=ProtectionRule.OFF,
+                default_value=Mode.OFF,
                 type_cast=str_to_protect_mode_enum,
             ),
         ]
```

### Comparing `contrast-agent-7.7.0/src/contrast/configuration/server.py` & `contrast_agent-8.0.0/src/contrast/configuration/server.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/loader/sitecustomize.py` & `contrast_agent-8.0.0/src/contrast/loader/sitecustomize.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 import contrast_rewriter
 
 # NOTE: This must be applied prior to importing the agent itself. Do not import any
 # other modules before registering the rewriter.
 contrast_rewriter.register()
 
 
-from contrast.agent.runner import start_runner
+from contrast.agent.runner import start_runner  # noqa: E402
 
 start_runner()
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/__init__.py` & `contrast_agent-8.0.0/src/contrast/patches/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
-from contrast_vendor import structlog as logging
-
-logger = logging.getLogger("contrast")
-
-
 from . import (
     cs_io,
     encodings_patch,
     re_patch,
     threading_patch,
     exec_and_eval,
     genshi_patch,
@@ -39,14 +34,18 @@
     starlette_patches,
     flask_and_quart_patches,
 )
 
 from .middleware import django, mod_wsgi, aiohttp
 from .middleware.common import CommonMiddlewarePatch, AppInterfaceType
 
+from contrast_vendor import structlog as logging
+
+logger = logging.getLogger("contrast")
+
 COMMON_PATCH_MODULES = (
     pathlib_patch,
     sqlalchemy_patch,
     # our sqlite3_patch also contains the import hook for pysqlite2.dbapi2
     sqlite3_patch,
     mysql_connector_patch,
     pymysql_patch,
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/cgi_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/cgi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/concurrent_futures_thread_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/concurrent_futures_thread_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/cs_io.py` & `contrast_agent-8.0.0/src/contrast/patches/cs_io.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/cs_str.py` & `contrast_agent-8.0.0/src/contrast/patches/cs_str.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/databases/dbapi2.py` & `contrast_agent-8.0.0/src/contrast/patches/databases/dbapi2.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/databases/mysql_connector_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/databases/mysql_connector_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/databases/psycopg2_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/databases/psycopg2_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/databases/sqlalchemy_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/databases/sqlalchemy_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/databases/sqlite3_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/databases/sqlite3_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/encodings_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/encodings_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/exec_and_eval.py` & `contrast_agent-8.0.0/src/contrast/patches/exec_and_eval.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/bottle_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/bottle_patches.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 from contrast_vendor.wrapt import register_post_import_hook
 
 import contrast
 from contrast.agent import scope
 from contrast.agent.policy.applicator import apply_module_patches
-from contrast.agent.middlewares.route_coverage.common import build_route
+from contrast.agent.middlewares.route_coverage.common import (
+    build_route,
+    log_discovered_routes,
+)
 from contrast.agent.middlewares.route_coverage.bottle_routes import create_bottle_routes
 from contrast.agent.policy import patch_manager
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 
 from contrast_vendor import structlog as logging
 
@@ -70,18 +73,15 @@
         from contrast.agent import agent_state
 
         if not agent_state.is_first_request():
             return
 
         discovered_routes = create_bottle_routes(bottle_instance)
         agent_state.update_routes(discovered_routes)
-        logger.debug(
-            "Discovered the following Bottle routes: %s",
-            [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-        )
+        log_discovered_routes("bottle", discovered_routes.values())
 
 
 def build_match_patch(orig_func, patch_policy):
     """
     Patch for bottle.Router.match()
 
     This sets up request context with all necessary info for current route observation
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/django_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/django_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/drf_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/drf_patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/falcon_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/falcon_patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 import contrast
 from contrast_vendor.wrapt import register_post_import_hook
 from contrast.agent import scope
 from contrast.agent.assess.policy.source_policy import apply_stream_source
 from contrast.agent.policy import patch_manager
+from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
 
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 from contrast_vendor import structlog as logging
 
 
 FALCON_MULTIPART_MIDDLEWARE_MODULE = "falcon_multipart.middleware"
@@ -105,18 +106,15 @@
     if not agent_state.is_first_request():
         return
 
     discovered_routes = create_falcon_routes(falcon_instance)
     agent_state.update_routes(discovered_routes)
 
     do_config_scanning(logger, falcon_instance)
-    logger.debug(
-        "Discovered the following Falcon routes: %s",
-        [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-    )
+    log_discovered_routes("falcon", discovered_routes.values())
 
 
 @fail_quietly("unable to perform Falcon route observation")
 @scope.with_contrast_scope
 def do_falcon_routes_observation(falcon_app_instance, request_args):
     from contrast.agent.middlewares.route_coverage.falcon_routes import (
         get_view_func,
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/flask_and_quart_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/flask_and_quart_patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 import functools
 from contrast_vendor.wrapt import register_post_import_hook
 
 import contrast
 from contrast.agent import scope
-from contrast.agent.middlewares.route_coverage.common import build_route
+from contrast.agent.middlewares.route_coverage.common import (
+    build_route,
+    log_discovered_routes,
+)
 from contrast.agent.middlewares.route_coverage.flask_routes import create_routes
 from contrast.agent.policy import patch_manager
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.safe_import import safe_import_list
 
 from contrast.agent.assess.rules.config import (
@@ -136,18 +139,15 @@
 
 @fail_quietly("unable to perform route discovery")
 def do_route_discovery(app_instance):
     from contrast.agent import agent_state
 
     discovered_routes = create_routes(app_instance)
     agent_state.update_routes(discovered_routes)
-    logger.debug(
-        "Discovered the following routes: %s",
-        [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-    )
+    log_discovered_routes("flask/quart", discovered_routes.values())
 
 
 def patch_flask(flask_module):
     build_and_apply_patch(
         flask_module.Flask,
         "full_dispatch_request",
         build_flask_full_dispatch_request_patch,
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/pyramid_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/pyramid_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from contrast.agent.policy import patch_manager
 from contrast.agent.policy.applicator import apply_assess_patch
 from contrast.agent.policy import registry
 from contrast.patches import urllib_patch
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.agent import scope
+from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
 
 from contrast_vendor import structlog as logging
 
 
 logger = logging.getLogger("contrast")
 
 PYRAMID_SESSION_MODULE = "pyramid.session"
@@ -123,19 +124,15 @@
     from contrast.agent import agent_state
 
     if not agent_state.is_first_request():
         return
 
     discovered_routes = create_pyramid_routes(pyramid_router_instance.registry)
     agent_state.update_routes(discovered_routes)
-
-    logger.debug(
-        "Discovered the following Pyramid routes: %s",
-        [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-    )
+    log_discovered_routes("pyramid", discovered_routes.values())
 
 
 @fail_quietly("unable to perform Pyramid route observation")
 @scope.with_contrast_scope
 def do_pyramid_routes_observation(pyramid_router_instance, request_path_arg):
     from contrast.agent.middlewares.route_coverage.pyramid_routes import (
         get_view_func,
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/frameworks/starlette_patches.py` & `contrast_agent-8.0.0/src/contrast/patches/frameworks/starlette_patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import contrast
 from contrast.agent import scope
 from contrast.agent.assess.policy.analysis import analyze
 from contrast.agent.policy import registry
 from contrast.agent.middlewares.route_coverage.starlette_routes import (
     create_starlette_routes,
 )
+from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
 from contrast.agent.policy import patch_manager
 from contrast.agent.middlewares.route_coverage.common import build_route
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 
 from contrast_vendor import structlog as logging
 
@@ -72,18 +73,15 @@
 
     if not agent_state.is_first_request():
         return
 
     discovered_routes = create_starlette_routes(starlette_router_instance)
 
     agent_state.update_routes(discovered_routes)
-    logger.debug(
-        "Discovered the following starlette routes: %s",
-        [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-    )
+    log_discovered_routes("starlette", discovered_routes.values())
 
 
 @fail_quietly("unable to perform starlette route observation")
 @scope.with_contrast_scope
 def do_starlette_route_observation(starlette_router_instance, *args, **kwargs):
     from starlette.staticfiles import StaticFiles
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/genshi_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/genshi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/import_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/import_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/lxml_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/lxml_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/middleware/aiohttp.py` & `contrast_agent-8.0.0/src/contrast/patches/middleware/aiohttp.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/middleware/common.py` & `contrast_agent-8.0.0/src/contrast/patches/middleware/common.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/middleware/django.py` & `contrast_agent-8.0.0/src/contrast/patches/middleware/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 
 import contrast
 from contrast.agent import scope
 from contrast.agent.policy import patch_manager
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
+from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
 
 from contrast_vendor.wrapt import register_post_import_hook
 from contrast_vendor import structlog as logging
 
 DJANGO_WSGI_NAME = "django.core.wsgi"
 DJANGO_ASGI_NAME = "django.core.asgi"
 
@@ -53,18 +54,15 @@
     logger.debug("performing route discovery for django application")
     discovered_routes = create_django_routes()
     if discovered_routes is None:
         logger.warning("no routes discovered for django application")
         return
 
     agent_state.update_routes(discovered_routes)
-    logger.debug(
-        "Discovered the following routes: %s",
-        [f"{route.verb} {route.url}" for route in discovered_routes.values()],
-    )
+    log_discovered_routes("django", discovered_routes.values())
 
 
 @fail_quietly("failed to run django first request analysis")
 @scope.with_contrast_scope
 def django_first_request(sender, **kwargs):
     # Lazy import for django
     from django.core import signals
```

### Comparing `contrast-agent-7.7.0/src/contrast/patches/middleware/mod_wsgi.py` & `contrast_agent-8.0.0/src/contrast/patches/middleware/mod_wsgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/pathlib_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/pathlib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/re_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/re_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/str_new.py` & `contrast_agent-8.0.0/src/contrast/patches/str_new.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/sys_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/sys_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/threading_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/threading_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/urllib_patch.py` & `contrast_agent-8.0.0/src/contrast/patches/urllib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/patches/utils.py` & `contrast_agent-8.0.0/src/contrast/patches/utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/deadzones.py` & `contrast_agent-8.0.0/src/contrast/policy/deadzones.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/codecs.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/codecs.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/encodings.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/encodings.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/frameworks.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/frameworks.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/paths.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/paths.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/re.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/re.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/serialize.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/serialize.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/propagators/string.py` & `contrast_agent-8.0.0/src/contrast/policy/propagators/string.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/asgi.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/cgi.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/cgi.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/django.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/django.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/falcon.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/falcon.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/flask.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/flask.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/quart.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/quart.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/sources/webob.py` & `contrast_agent-8.0.0/src/contrast/policy/sources/webob.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/__init__.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 
+# ruff: noqa: F403
+
 # Dataflow rules
 from .cmd_injection import *
 from .nosql_injection import *
 from .path_traversal import *
 from .sql_injection import *
 from .redos import *
 from .reflected_xss import *
```

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/cmd_injection.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/cmd_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/crypto.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/crypto.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/httponly.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/httponly.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/nosql_injection.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/nosql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/path_traversal.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/path_traversal.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/prompt_injection.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/prompt_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/redos.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/redos.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/reflected_xss.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/reflected_xss.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/secure_flag_missing.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/secure_flag_missing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/session_rewriting.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/session_rewriting.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/session_timeout.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/session_timeout.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/sql_injection.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/sql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/ssrf.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/ssrf.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/trust_boundary_violation.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/trust_boundary_violation.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/unsafe_code_execution.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/untrusted_deserialization.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/untrusted_deserialization.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/unvalidated_redirect.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/unvalidated_redirect.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/xpath_injection.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/xpath_injection.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/policy/triggers/xxe.py` & `contrast_agent-8.0.0/src/contrast/policy/triggers/xxe.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/activity_masker.py` & `contrast_agent-8.0.0/src/contrast/reporting/activity_masker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/reporting_client.py` & `contrast_agent-8.0.0/src/contrast/reporting/reporting_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 from contrast.agent import scope
 from contrast.agent.disable_reaction import DisableReaction
 from contrast.agent.settings import Settings
 from contrast.reporting import RequestAudit
 from contrast.reporting.teamserver_messages.base_ts_message import (
     PYTHON,
-    _b64url_stripped,
+    b64url_stripped,
 )
 from contrast_vendor import structlog as logging
 
 from .teamserver_messages import BaseTsMessage
 
 logger = logging.getLogger("contrast")
 
 REPORTING_CLIENT_THREAD_NAME = "ContrastReportingClient"
 
 MAX_ATTEMPTS = 2
 ERROR_STATUS_CODE = -1
 
 
 # TODO: PYT-2865 RepartingClient is still essentially a singleton, but it's implemented
-# using a function instead of a class. This still needs to be reworked.
+#   using a function instead of a class. This still needs to be reworked.
 class _ReportingClient(threading.Thread):
     # This must not be instantiated directly. Use get_reporting_client().
     def __init__(self):
         super().__init__(name=REPORTING_CLIENT_THREAD_NAME, daemon=True)
 
         self._stopper = object()  # sentinel sent over message_q to stop the thread
         self.message_q = queue.Queue(maxsize=128)
@@ -41,33 +41,33 @@
         self.session = Session()
         # disable persisting cookies, per Architecture team recommendation.
         self.session.cookies.set_policy(DefaultCookiePolicy(allowed_domains=[]))
         self.session.verify, self.session.cert = self.init_certs(self.settings)
         self.session.proxies = (
             self.settings.build_proxy_url() if self.settings.is_proxy_enabled else {}
         )
-        server_name_b64 = _b64url_stripped(self.settings.get_server_name())
-        server_path_b64 = _b64url_stripped(self.settings.get_server_path())
-        server_type_b64 = _b64url_stripped(self.settings.get_server_type())
+        server_name_b64 = b64url_stripped(self.settings.get_server_name())
+        server_path_b64 = b64url_stripped(self.settings.get_server_path())
+        server_type_b64 = b64url_stripped(self.settings.get_server_type())
         auth_header = f"{self.settings.api_user_name}:{self.settings.api_service_key}"
         self.session.headers.update(
             {
                 # the Authorization header must not have its padding stripped
                 "Authorization": base64.urlsafe_b64encode(
                     auth_header.encode()
                 ).decode(),
                 "API-Key": self.settings.api_key,
                 "Server-Name": server_name_b64,
                 "Server-Path": server_path_b64,
                 "Server-Type": server_type_b64,
                 "X-Contrast-Agent": f"{PYTHON} {contrast.__version__}",
                 "X-Contrast-Header-Encoding": "base64",
                 "Application-Language": PYTHON,
-                "Application-Name": _b64url_stripped(self.settings.app_name),
-                "Application-Path": _b64url_stripped(self.settings.app_path),
+                "Application-Name": b64url_stripped(self.settings.app_name),
+                "Application-Path": b64url_stripped(self.settings.app_path),
             }
         )
 
         self.request_audit = (
             RequestAudit(self.settings.config)
             if self.settings.config.is_request_audit_enabled
             else None
@@ -144,27 +144,27 @@
         except Exception as e:
             logger.exception(
                 "Failed to send %s message to Contrast: %s", msg.class_name, e
             )
 
         return None
 
-    def _send_message(self, msg):
+    def _send_message(self, msg: BaseTsMessage):
         """
         _send_message sends msg to Teamserver and returns the response.
 
         It is the caller's responsibility to handle any network exceptions.
 
         See send_message for the public interface, which handles exceptions.
         """
         status_code = ERROR_STATUS_CODE
         msg_name = msg.class_name
-        logger.debug("Sending %s message to Teamserver", msg_name)
 
         url = msg.base_url + msg.path
+        logger.debug("Sending %s message to Teamserver: %s", msg_name, url)
         response = msg.request_method(
             self.session,
             url,
             json=msg.body,
             headers=msg.headers,
             allow_redirects=False,
             # environment variables can interfere with session fields, so
@@ -175,15 +175,15 @@
             cert=self.session.cert,
         )
 
         try:
             status_code = response.status_code
             msg_success_status = response.json().get("success")
             messages = response.json().get("messages")
-            if not msg_success_status:
+            if not (msg_success_status or status_code == 200):
                 logger.error(
                     "Failure on Contrast UI processing request reason - (%s): %s",
                     messages,
                     status_code,
                 )
         except Exception as e:
             if status_code == ERROR_STATUS_CODE:
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/request_audit.py` & `contrast_agent-8.0.0/src/contrast/reporting/request_audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         else:
             self.messages_path = path.join(parent_path, "messages")
 
         for sub_dir in self.SUB_DIRS:
             sub_path = path.join(self.messages_path, sub_dir)
             pathlib.Path(sub_path).mkdir(parents=True, exist_ok=True)
 
-        logger.debug(f"Created request_audit dirs in %s", self.messages_path)
+        logger.debug("Created request_audit dirs in %s", self.messages_path)
 
     def audit(self, msg, response):
         if self.config.get_value("api.request_audit.requests"):
             self.write_data(msg, "requests", msg.name)
 
         if self.config.get_value("api.request_audit.responses"):
             self.write_data(response, "responses", msg.name)
@@ -62,10 +62,9 @@
 
         file_name = f"{time}-{msg_name}-teamserver.json"
         file_path = path.join(self.messages_path, msg_type, file_name)
 
         data = get_message_body(msg)
 
         # In the future, we'd like to somehow include status code + headers
-
         with pathlib.Path(file_path).open("w", encoding="UTF-8") as target:
             json.dump(data, target, indent=1)
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/__init__.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,29 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
+from .agent_startup import AgentStartup
 from .application_activity import ApplicationActivity
 from .application_inventory import ApplicationInventory
-from .application_startup import ApplicationStartup
 from .application_update import ApplicationUpdate
 from .effective_config import EffectiveConfig
 from .heartbeat import Heartbeat
 from .library_usage import LibraryUsage
 from .observed_route import ObservedRoute
 from .preflight import Preflight
 from .server_activity import ServerActivity
-from .server_startup import ServerStartup
 from .base_ts_message import BaseTsMessage, BaseTsAppMessage, BaseTsServerMessage
+
+__all__ = [
+    "AgentStartup",
+    "ApplicationActivity",
+    "ApplicationInventory",
+    "ApplicationUpdate",
+    "EffectiveConfig",
+    "Heartbeat",
+    "LibraryUsage",
+    "ObservedRoute",
+    "Preflight",
+    "ServerActivity",
+    "BaseTsMessage",
+    "BaseTsAppMessage",
+    "BaseTsServerMessage",
+]
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/_traces.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/_traces.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return "traces"
 
     @property
     def path(self) -> str:
         return "traces"
 
     @property
-    def request_method(self) -> str:
+    def request_method(self):
         return requests.Session.put
 
     @fail_loudly("Failed to process Traces response")
     def process_response(self, response, reporting_client):
         self.process_response_code(response, reporting_client)
 
     def _build_body(self, finding, reportable_request):
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_activity.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_activity.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,12 +68,12 @@
     @fail_loudly("Failed to process Activity response")
     def process_response(self, response, reporting_client):
         if not self.process_response_code(response, reporting_client):
             return
 
         body = response.json()
 
-        self.settings.apply_ts_app_settings(body)
+        self.settings.apply_ng_app_settings(body)
         self.settings.process_ts_reactions(body)
         self.settings.log_effective_config()
         if reporting_client is not None and self.settings.is_agent_config_enabled():
             reporting_client.add_message(EffectiveConfig())
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_inventory.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_inventory.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/application_update.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/application_update.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/base_ts_message.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/base_ts_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 logger = logging.getLogger("contrast")
 
 
 PYTHON = "Python"
 SLEEP_TIME_SECS = timedelta(minutes=15).seconds
 
 
-def _b64url_stripped(header_str):
+def b64url_stripped(header_str):
     """
     For some headers, TS expects a value that
     - is base64 encoded using URL-safe characters
     - has any padding (= or ==) stripped
 
     This follows RFC-4648 - base64 with URL and filename safe alphabet
     """
@@ -32,17 +32,17 @@
 
 class BaseTsMessage:
     def __init__(self):
         self._sent_count = 0
         self.settings = Settings()
 
         self.base_url = f"{self.settings.api_url}/api/ng/"
-        self.server_name_b64 = _b64url_stripped(self.settings.get_server_name())
-        self.server_path_b64 = _b64url_stripped(self.settings.get_server_path())
-        self.server_type_b64 = _b64url_stripped(self.settings.get_server_type())
+        self.server_name_b64 = b64url_stripped(self.settings.get_server_name())
+        self.server_path_b64 = b64url_stripped(self.settings.get_server_path())
+        self.server_type_b64 = b64url_stripped(self.settings.get_server_type())
 
         self.headers = {}
 
         if self.settings.config and self.settings.config.session_id != "":
             self.headers.update({"Session-ID": self.settings.config.session_id})
 
         self.body = ""
@@ -62,15 +62,15 @@
     def path(self) -> str:
         """
         URL path for teamserver; used for formatting as "/api/ng/{path}"
         """
         raise NotImplementedError(NOTIMPLEMENTED_MSG)
 
     @property
-    def request_method(self) -> str:
+    def request_method(self):
         raise NotImplementedError(NOTIMPLEMENTED_MSG)
 
     @property
     def expected_response_codes(self):
         return [204]
 
     @property
@@ -102,15 +102,15 @@
         an agent should parse this response and check for a `success` value of `false`
         before disabling."
 
         https://github.com/Contrast-Security-Inc/contrast-agent-api-spec/blob/master/agent-endpoints.yml
         """
         try:
             body = response.json()
-            return body.get("success") == False
+            return body.get("success") is False
         except Exception:
             pass
 
         return False
 
     def process_response_code(
         self, response, reporting_client
@@ -134,24 +134,28 @@
             return False
 
         if response.status_code == 404:
             if self.should_shutdown(response):
                 DisableReaction.run(self.settings)
             return False
 
-        if response.status_code in (409, 410, 412, 502):
+        if response.status_code in (403, 409, 410, 412, 422, 502):
+            # 403: Access forbidden because credentials failed to authenticate.
             # 409: app is archived, 502 app is locked in TS
             # 410: app is not registered. We could send App startup for not we won't
-            # 412: API key no longer valid. While spec may say to resend msg in 15 mins,
-            #  in reality the app server and agent should simply be restarted.
+            # 412: API key no longer valid. While spec may say to resend msg in 15 mins, in reality the app server and
+            #   agent should simply be restarted.
+            # 422: app could not be created because a condition, like session id or metadata failed
             DisableReaction.run(self.settings)
             return False
 
         if response.status_code in (401, 408):
-            # 401: Access forbidden because credentials failed to authenticate.
+            # 401:
+            #   NG: Access forbidden because credentials failed to authenticate.
+            #   V1: Access forbidden because credentials were not provided.
             # 408: TS Could not create settings in time.
             if self.disable_agent_on_401_and_408:
                 DisableReaction.run(self.settings)
             else:
                 logger.debug("Sleeping for 15 minutes")
 
                 sleep(SLEEP_TIME_SECS)
@@ -177,15 +181,15 @@
             )
             return False
 
         return True
 
 
 class BaseTsServerMessage(BaseTsMessage):
-    @fail_loudly(f"Failed to process server settings response")
+    @fail_loudly("Failed to process server settings response")
     def process_response(self, response, reporting_client):
         settings = Settings()
         if not self.process_response_code(response, reporting_client):
             return
 
         body = response.json()
 
@@ -194,16 +198,16 @@
 
 
 class BaseTsAppMessage(BaseTsMessage):
     def __init__(self):
         super().__init__()
 
         # App language should only be encoded for url paths, not for headers.
-        self.app_language_b64 = _b64url_stripped(PYTHON)
-        self.app_name_b64 = _b64url_stripped(self.settings.app_name)
+        self.app_language_b64 = b64url_stripped(PYTHON)
+        self.app_name_b64 = b64url_stripped(self.settings.app_name)
 
     @property
     def since_last_update(self):
         """
         Time in ms since app settings have been updated.
         If never updated, then it's been 0ms since then.
         """
```

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/effective_config.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/effective_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/heartbeat.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/library_usage.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/library_usage.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/observed_route.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/observed_route.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/preflight.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/reporting/teamserver_messages/server_activity.py` & `contrast_agent-8.0.0/src/contrast/reporting/teamserver_messages/server_activity.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/scripts/fix_interpreter_permissions.py` & `contrast_agent-8.0.0/src/contrast/scripts/fix_interpreter_permissions.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/scripts/propagator_check.py` & `contrast_agent-8.0.0/src/contrast/scripts/propagator_check.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/scripts/runner.py` & `contrast_agent-8.0.0/src/contrast/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/scripts/validate_config.py` & `contrast_agent-8.0.0/src/contrast/scripts/validate_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/duck_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/duck_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/base.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/base.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_cformat.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_cformat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/formatting/tokenize_format.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/formatting/tokenize_format.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/stream_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/stream_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/tag_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/tag_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/assess/tracking_util.py` & `contrast_agent-8.0.0/src/contrast/utils/assess/tracking_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,38 +2,51 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import io
 
 from contrast.agent.assess.utils import is_tracked
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.assess.duck_utils import safe_getattr, safe_iterator
 
+from contrast.utils.safe_import import safe_import
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
+SUPPORTED_TYPES = (
+    str,
+    bytes,
+    bytearray,
+)
+
+DJANGO_PROMISE_TYPE = safe_import("django.utils.functional.Promise")
+
 
 @fail_quietly("Failed check if obj is tracked", return_value=False)
-def recursive_is_tracked(obj):
+def recursive_is_tracked(obj):  # pylint: disable=too-many-return-statements
     """
     This is a fairly hot code path in some applications; be mindful of performance
     """
     if obj is None:
         return False
 
+    if isinstance(obj, SUPPORTED_TYPES):
+        return is_tracked(obj)
+
     if isinstance(obj, dict):
-        for key, value in obj.items():
-            if recursive_is_tracked(key) or recursive_is_tracked(value):
-                return True
-    elif isinstance(obj, io.IOBase):
+        return any(
+            recursive_is_tracked(key) or recursive_is_tracked(value)
+            for key, value in obj.items()
+        )
+    if isinstance(obj, io.IOBase):
         return safe_getattr(obj, "cs__tracked", False) or safe_getattr(
             obj, "cs__source", False
         )
     # These are the only safe objects where we can guarantee that we won't
     # destructively modify the object such that the application may see
     # different results.
-    elif isinstance(obj, (list, tuple)):
-        for item in safe_iterator(obj):
-            if recursive_is_tracked(item):
-                return True
-        return False
+    if isinstance(obj, (list, tuple)):
+        return any(recursive_is_tracked(item) for item in safe_iterator(obj))
+
+    if DJANGO_PROMISE_TYPE and isinstance(obj, DJANGO_PROMISE_TYPE):
+        return is_tracked(str(obj))
 
     return is_tracked(obj)
```

### Comparing `contrast-agent-7.7.0/src/contrast/utils/base64_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/configuration_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/configuration_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import socket
 from typing import List, Tuple
 
 from contrast import AGENT_CURR_WORKING_DIR
 from contrast.utils.string_utils import truncate
 from contrast_vendor.ruamel import yaml
 
-from contrast.agent.protect.rule import ProtectionRule
+from contrast.agent.protect.rule.mode import Mode
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
 CONFIG_LOCATIONS = [
@@ -45,15 +45,15 @@
 
 # Valid options are defined in the spec:
 # https://github.com/Contrast-Security-Inc/assess-specifications/blob/master/vulnerability/capture-stacktrace.md
 STACKTRACE_OPTIONS = ["ALL", "SOME", "NONE"]
 
 
 @lru_cache(maxsize=1)
-def get_hostname():
+def get_hostname() -> str:
     """
     Returns the hostname from the socket or "localhost"
     """
     hostname = "localhost"
 
     try:
         hostname = socket.gethostname() or hostname
@@ -106,15 +106,15 @@
         # For the user specified CONTRAST_CONFIG_PATH, warnings are logged
         # in load_yaml_config.
         logger.debug("Configuration file not found: %s", file_path)
 
     return None
 
 
-def flatten_config(config):
+def flatten_config(config) -> dict:
     """
     Convert a nested dict such as
         {'enable': True,
         'application':
             {'name': 'dani-flask'},
         'foo':
         'agent':
@@ -136,15 +136,15 @@
         elif x is not None:
             flattened_config[name[:-1]] = x
 
     flatten(config)
     return flattened_config
 
 
-def str_to_bool(val):
+def str_to_bool(val) -> bool:
     """
     Converts a str to a bool
 
     true -> True, false -> False
     """
     if isinstance(val, bool):
         return val
@@ -157,34 +157,34 @@
     if val in ("y", "yes", "t", "true", "on", "1"):
         return True
     if val in ("n", "no", "f", "false", "off", "0"):
         return False
     raise ValueError(f"invalid truth value {val!r}")
 
 
-def parse_disabled_rules(disabled_rules):
+def parse_disabled_rules(disabled_rules) -> List[str]:
     if not disabled_rules:
         return []
 
     return [rule.lower() for rule in disabled_rules.split(",")]
 
 
-def parse_stacktraces_options(option):
+def parse_stacktraces_options(option) -> str:
     option = option.upper()
     if option in STACKTRACE_OPTIONS:
         return option
 
     return "ALL"
 
 
-def parse_event_detail_option(option):
+def parse_event_detail_option(option) -> str:
     return "full" if option.lower() == "full" else "minimal"
 
 
-def str_to_protect_mode_enum(mode):
+def str_to_protect_mode_enum(mode) -> Mode:
     """
     Converts str config value to protect mode enum that the agent understands
     """
     if not mode:
-        return ProtectionRule.OFF
+        return Mode.OFF
 
-    return getattr(ProtectionRule, mode.upper(), ProtectionRule.MONITOR)
+    return getattr(Mode, mode.upper(), Mode.MONITOR)
```

### Comparing `contrast-agent-7.7.0/src/contrast/utils/context_tracker.py` & `contrast_agent-8.0.0/src/contrast/utils/context_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/decorators.py` & `contrast_agent-8.0.0/src/contrast/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/deprecated_middleware.py` & `contrast_agent-8.0.0/src/contrast/utils/deprecated_middleware.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/environ.py` & `contrast_agent-8.0.0/src/contrast/utils/environ.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py` & `contrast_agent-8.0.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/ignored_modules.py` & `contrast_agent-8.0.0/src/contrast/utils/ignored_modules.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/library_reader/library_reader.py` & `contrast_agent-8.0.0/src/contrast/utils/library_reader/library_reader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/library_reader/patched_state.py` & `contrast_agent-8.0.0/src/contrast/utils/library_reader/patched_state.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/library_reader/utils.py` & `contrast_agent-8.0.0/src/contrast/utils/library_reader/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import os
 import hashlib
 
 from contrast_vendor.importlib_metadata import packages_distributions
 from contrast_vendor.importlib_metadata import files as importlib_get_files
 
+from contrast_vendor import structlog as logging
+
+logger = logging.getLogger("contrast")
+
 CONTRAST_AGENT_DIST = "contrast-agent"
 
 # Both of these metadata files contain a file list of what is installed under the top level dirs
 RECORD = "RECORD"
 SOURCES = "SOURCES.txt"
 
 NAMESPACE_PACKAGE = "namespace_packages.txt"
@@ -17,18 +21,14 @@
 
 PY_SUFFIX = ".py"
 SO_SUFFIX = ".so"
 
 SITE_PACKAGES_DIR = f"{os.sep}site-packages{os.sep}"
 DIST_PACKAGES_DIR = f"{os.sep}dist-packages{os.sep}"
 
-from contrast_vendor import structlog as logging
-
-logger = logging.getLogger("contrast")
-
 INSTALLED_DISTRIBUTIONS = None
 INSTALLED_DISTRIBUTION_TOP_LEVEL_IMPORTS = None
 
 
 def _load_installed_dist_top_level_imports(cache):
     """
     Returns a dictionary containing a mapping of the package name to each of its top level importable packages by name.
```

### Comparing `contrast-agent-7.7.0/src/contrast/utils/loggers/logger.py` & `contrast_agent-8.0.0/src/contrast/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/loggers/structlog.py` & `contrast_agent-8.0.0/src/contrast/utils/loggers/structlog.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/module_parser.py` & `contrast_agent-8.0.0/src/contrast/utils/module_parser.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/namespace.py` & `contrast_agent-8.0.0/src/contrast/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/object_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/patch_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/patch_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/pattern_builder.py` & `contrast_agent-8.0.0/src/contrast/utils/pattern_builder.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/profiler.py` & `contrast_agent-8.0.0/src/contrast/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/safe_import.py` & `contrast_agent-8.0.0/src/contrast/utils/safe_import.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/singleton.py` & `contrast_agent-8.0.0/src/contrast/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/stack_trace_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/stack_trace_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/stdlib_modules.py` & `contrast_agent-8.0.0/src/contrast/utils/stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast/utils/string_utils.py` & `contrast_agent-8.0.0/src/contrast/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_agent.egg-info/SOURCES.txt` & `contrast_agent-8.0.0/src/contrast_agent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -175,17 +175,17 @@
 src/contrast/agent/protect/rule/__init__.py
 src/contrast/agent/protect/rule/base_rule.py
 src/contrast/agent/protect/rule/bot_blocker_rule.py
 src/contrast/agent/protect/rule/cmdi_rule.py
 src/contrast/agent/protect/rule/deserialization_rule.py
 src/contrast/agent/protect/rule/http_method_tampering.py
 src/contrast/agent/protect/rule/malformed_header.py
+src/contrast/agent/protect/rule/mode.py
 src/contrast/agent/protect/rule/nosqli_rule.py
 src/contrast/agent/protect/rule/path_traversal_rule.py
-src/contrast/agent/protect/rule/protection_rule.py
 src/contrast/agent/protect/rule/rules_builder.py
 src/contrast/agent/protect/rule/sqli_rule.py
 src/contrast/agent/protect/rule/ssrf_rule.py
 src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
 src/contrast/agent/protect/rule/xss_rule.py
 src/contrast/agent/protect/rule/xxe_rule.py
 src/contrast/agent/protect/rule/deserialization/__init__.py
@@ -482,26 +482,32 @@
 src/contrast/quart/middleware.py
 src/contrast/reporting/__init__.py
 src/contrast/reporting/activity_masker.py
 src/contrast/reporting/reporting_client.py
 src/contrast/reporting/request_audit.py
 src/contrast/reporting/teamserver_messages/__init__.py
 src/contrast/reporting/teamserver_messages/_traces.py
+src/contrast/reporting/teamserver_messages/agent_startup.py
 src/contrast/reporting/teamserver_messages/application_activity.py
 src/contrast/reporting/teamserver_messages/application_inventory.py
-src/contrast/reporting/teamserver_messages/application_startup.py
 src/contrast/reporting/teamserver_messages/application_update.py
 src/contrast/reporting/teamserver_messages/base_ts_message.py
 src/contrast/reporting/teamserver_messages/effective_config.py
 src/contrast/reporting/teamserver_messages/heartbeat.py
 src/contrast/reporting/teamserver_messages/library_usage.py
 src/contrast/reporting/teamserver_messages/observed_route.py
 src/contrast/reporting/teamserver_messages/preflight.py
 src/contrast/reporting/teamserver_messages/server_activity.py
-src/contrast/reporting/teamserver_messages/server_startup.py
+src/contrast/reporting/teamserver_responses/__init__.py
+src/contrast/reporting/teamserver_responses/application_settings.py
+src/contrast/reporting/teamserver_responses/ng_application_settings.py
+src/contrast/reporting/teamserver_responses/ng_server_settings.py
+src/contrast/reporting/teamserver_responses/protect_rule.py
+src/contrast/reporting/teamserver_responses/sampling.py
+src/contrast/reporting/teamserver_responses/server_settings.py
 src/contrast/scripts/__init__.py
 src/contrast/scripts/fix_interpreter_permissions.py
 src/contrast/scripts/propagator_check.py
 src/contrast/scripts/runner.py
 src/contrast/scripts/validate_config.py
 src/contrast/utils/__init__.py
 src/contrast/utils/base64_utils.py
```

### Comparing `contrast-agent-7.7.0/src/contrast_rewriter/__init__.py` & `contrast_agent-8.0.0/src/contrast_rewriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import ast
 import copy
 import operator
 import os
 
 # Seems like it is necessary to import this prior to rewriting to avoid some weird partial import state
-import tokenize  # pylint: disable=unused-import
+import tokenize  # noqa: F401
 
 from contrast_vendor.wrapt.importer import _ImportHookChainedLoader
 
 # NOTE: It is extremely important to limit the number of imports used by this
 # module. It should be restricted to only those imports that are absolutely
 # necessary for the operation of the rewriter, and ideally should include only
 # built-in or standard library modules that are already imported by the
```

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_adapters.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_collections.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_compat.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_functools.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_itertools.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_meta.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/_text.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/importlib_metadata/compat/py39.py` & `contrast_agent-8.0.0/src/contrast_vendor/importlib_metadata/compat/py39.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py27.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py310.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py311.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py312.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py36.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py37.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py38.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/isort/stdlibs/py39.py` & `contrast_agent-8.0.0/src/contrast_vendor/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ported_cpython_code/import_functionality.py` & `contrast_agent-8.0.0/src/contrast_vendor/ported_cpython_code/import_functionality.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/comments.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/compat.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/composer.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/constructor.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/cyaml.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/dumper.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/emitter.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/error.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/events.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/loader.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/main.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/nodes.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/parser.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/reader.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/representer.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/resolver.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarbool.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarint.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scalarstring.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/scanner.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/serializer.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tag.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/timestamp.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/tokens.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/ruamel/yaml/util.py` & `contrast_agent-8.0.0/src/contrast_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-APACHE` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/LICENSE-MIT` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_base.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_base.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_config.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_config.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_frames.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_frames.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_generic.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_greenlets.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_log_levels.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_native.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_native.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_output.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_output.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/_utils.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/contextvars.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/contextvars.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/dev.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/dev.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/processors.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/stdlib.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/stdlib.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/testing.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/testing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/threadlocal.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/tracebacks.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/tracebacks.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/twisted.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/twisted.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/types.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/types.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/structlog/typing.py` & `contrast_agent-8.0.0/src/contrast_vendor/structlog/typing.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/acceptparse.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/byterange.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/cachecontrol.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/client.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/client.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/compat.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/compat.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/cookies.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/datetime_utils.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/dec.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/dec.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/descriptors.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/etag.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/etag.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/exc.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/exc.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/headers.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/headers.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/license.txt` & `contrast_agent-8.0.0/src/contrast_vendor/webob/license.txt`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/multidict.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/request.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/request.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/response.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/response.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/static.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/static.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/webob/util.py` & `contrast_agent-8.0.0/src/contrast_vendor/webob/util.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/arguments.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/decorators.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/importer.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/patches.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/weakrefs.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/wrapt/wrappers.py` & `contrast_agent-8.0.0/src/contrast_vendor/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/zipp/LICENSE` & `contrast_agent-8.0.0/src/contrast_vendor/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/zipp/__init__.py` & `contrast_agent-8.0.0/src/contrast_vendor/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast-agent-7.7.0/src/contrast_vendor/zipp/glob.py` & `contrast_agent-8.0.0/src/contrast_vendor/zipp/glob.py`

 * *Files identical despite different names*

