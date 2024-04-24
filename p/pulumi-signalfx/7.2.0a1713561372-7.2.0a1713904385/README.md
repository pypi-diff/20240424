# Comparing `tmp/pulumi_signalfx-7.2.0a1713561372.tar.gz` & `tmp/pulumi_signalfx-7.2.0a1713904385.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-7.2.0a1713561372.tar", last modified: Fri Apr 19 21:19:23 2024, max compression
+gzip compressed data, was "pulumi_signalfx-7.2.0a1713904385.tar", last modified: Tue Apr 23 20:42:13 2024, max compression
```

## Comparing `pulumi_signalfx-7.2.0a1713561372.tar` & `pulumi_signalfx-7.2.0a1713904385.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.726909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   153334 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.726909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    82908 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (127)   138325 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.730909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-19 21:19:23.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-19 21:19:23.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:19:23.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:19:23.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:19:23.000000 pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 21:19:17.000000 pulumi_signalfx-7.2.0a1713561372/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:19:23.734909 pulumi_signalfx-7.2.0a1713561372/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.031039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   153334 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.031039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82908 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138325 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.035039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-23 20:42:13.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-23 20:42:13.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:42:13.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:42:13.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 20:42:13.000000 pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 20:42:05.000000 pulumi_signalfx-7.2.0a1713904385/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:42:13.039039 pulumi_signalfx-7.2.0a1713904385/setup.cfg
```

### Comparing `pulumi_signalfx-7.2.0a1713561372/PKG-INFO` & `pulumi_signalfx-7.2.0a1713904385/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1713561372
+Version: 7.2.0a1713904385
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1713561372/README.md` & `pulumi_signalfx-7.2.0a1713904385/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/__init__.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/__init__.pyi` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/data_link.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/detector.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/timeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/log/view.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/log/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/org_token.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/outputs.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,22 +65,20 @@
 def get_integration(name: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIntegrationResult:
     """
     Use this data source to get information on an existing PagerDuty integration.
 
     ## Example
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_signalfx as signalfx
 
     pd_integration = signalfx.pagerduty.get_integration(name="PD-Integration")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Arguments
 
     * `name` - Specify the exact name of the desired PagerDuty integration
 
     ## Attributes
 
@@ -103,22 +101,20 @@
 def get_integration_output(name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIntegrationResult]:
     """
     Use this data source to get information on an existing PagerDuty integration.
 
     ## Example
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_signalfx as signalfx
 
     pd_integration = signalfx.pagerduty.get_integration(name="PD-Integration")
     ```
-    <!--End PulumiCodeChooser -->
 
     ## Arguments
 
     * `name` - Specify the exact name of the desired PagerDuty integration
 
     ## Attributes
```

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/provider.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/slo.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/team.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1713561372
+Version: 7.2.0a1713904385
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1713561372/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-7.2.0a1713904385/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1713561372/pyproject.toml` & `pulumi_signalfx-7.2.0a1713904385/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_signalfx"
   description = "A Pulumi package for creating and managing SignalFx resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "signalfx"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.2.0a1713561372"
+  version = "7.2.0a1713904385"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-signalfx"
 
 [build-system]
```

