# Comparing `tmp/deebot-client-6.0.2.tar.gz` & `tmp/deebot_client-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-6.0.2.tar", last modified: Mon Feb 26 18:21:31 2024, max compression
+gzip compressed data, was "deebot_client-7.0.0.tar", last modified: Tue Apr 23 08:38:58 2024, max compression
```

## Comparing `deebot-client-6.0.2.tar` & `deebot_client-7.0.0.tar`

### file list

```diff
@@ -1,219 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.541421 deebot-client-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.509420 deebot-client-6.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.509420 deebot-client-6.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.509420 deebot-client-6.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-26 18:21:22.000000 deebot-client-6.0.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-26 18:21:22.000000 deebot-client-6.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-26 18:21:31.537421 deebot-client-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-02-26 18:21:22.000000 deebot-client-6.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.513420 deebot-client-6.0.2/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.513420 deebot-client-6.0.2/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.521421 deebot-client-6.0.2/deebot_client/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/clear_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/relocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/json/work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.521421 deebot-client-6.0.2/deebot_client/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/xml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/commands/xml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/event_bus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.521421 deebot-client-6.0.2/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/efficiency_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/events/work_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.521421 deebot-client-6.0.2/deebot_client/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.525421 deebot-client-6.0.2/deebot_client/hardware/deebot/
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/2o4lnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/55aiho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/5xu9h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/626v6g.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/85nbtp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/9ku8nu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/clojes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/lx3j7m.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/p1jij8.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/p95mgv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/rss8xk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/umwv6z.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/vi829v.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/x5d34r.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/yna5xi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/hardware/deebot/zjavof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23545 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.525421 deebot-client-6.0.2/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.525421 deebot-client-6.0.2/deebot_client/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/messages/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/messages/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/messages/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12117 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.525421 deebot-client-6.0.2/deebot_client/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/util/continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-26 18:21:22.000000 deebot-client-6.0.2/deebot_client/util/countries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-02-26 18:21:31.000000 deebot-client-6.0.2/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-02-26 18:21:31.000000 deebot-client-6.0.2/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 18:21:31.000000 deebot-client-6.0.2/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 18:21:31.000000 deebot-client-6.0.2/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-26 18:21:31.000000 deebot-client-6.0.2/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-26 18:21:22.000000 deebot-client-6.0.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-02-26 18:21:22.000000 deebot-client-6.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-26 18:21:22.000000 deebot-client-6.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-26 18:21:22.000000 deebot-client-6.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-26 18:21:22.000000 deebot-client-6.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 18:21:22.000000 deebot-client-6.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.529421 deebot-client-6.0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-02-26 18:21:22.000000 deebot-client-6.0.2/scripts/check_getLogger.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-02-26 18:21:22.000000 deebot-client-6.0.2/scripts/run-in-env.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 18:21:31.541421 deebot-client-6.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.529421 deebot-client-6.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.529421 deebot-client-6.0.2/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.533421 deebot-client-6.0.2/tests/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/json/test_work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/commands/xml/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/fixtures/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/fixtures/mqtt_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/hardware/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/helpers/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/json/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/mqtt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/test_mqtt_client_reconnect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:31.537421 deebot-client-6.0.2/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/util/test_continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/util/test_countries.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-26 18:21:22.000000 deebot-client-6.0.2/tests/util/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.460453 deebot_client-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.428454 deebot_client-7.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.428454 deebot_client-7.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.428454 deebot_client-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 08:38:53.000000 deebot_client-7.0.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-23 08:38:53.000000 deebot_client-7.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-23 08:38:58.460453 deebot_client-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-23 08:38:53.000000 deebot_client-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.428454 deebot_client-7.0.0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.432453 deebot_client-7.0.0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.436453 deebot_client-7.0.0/deebot_client/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/clear_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/json/work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.440454 deebot_client-7.0.0/deebot_client/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/commands/xml/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/event_bus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.440454 deebot_client-7.0.0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/efficiency_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/events/work_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.440454 deebot_client-7.0.0/deebot_client/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.444454 deebot_client-7.0.0/deebot_client/hardware/deebot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/2o4lnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/55aiho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/5xu9h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/626v6g.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/85nbtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/9ku8nu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/clojes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/itk04l.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/lf3bn4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/lx3j7m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/p1jij8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/p95mgv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/paeygf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/rss8xk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/umwv6z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/vi829v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/x5d34r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/yna5xi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/hardware/deebot/zjavof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23546 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.444454 deebot_client-7.0.0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.444454 deebot_client-7.0.0/deebot_client/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/messages/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/messages/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/messages/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.444454 deebot_client-7.0.0/deebot_client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/util/continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 08:38:53.000000 deebot_client-7.0.0/deebot_client/util/countries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-23 08:38:58.000000 deebot_client-7.0.0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-23 08:38:58.000000 deebot_client-7.0.0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:38:58.000000 deebot_client-7.0.0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 08:38:58.000000 deebot_client-7.0.0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 08:38:58.000000 deebot_client-7.0.0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-23 08:38:53.000000 deebot_client-7.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-23 08:38:53.000000 deebot_client-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 08:38:53.000000 deebot_client-7.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 08:38:53.000000 deebot_client-7.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 08:38:53.000000 deebot_client-7.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-23 08:38:53.000000 deebot_client-7.0.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.444454 deebot_client-7.0.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-23 08:38:53.000000 deebot_client-7.0.0/scripts/check_getLogger.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-04-23 08:38:53.000000 deebot_client-7.0.0/scripts/run-in-env.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:38:58.460453 deebot_client-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.448454 deebot_client-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.448454 deebot_client-7.0.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.452453 deebot_client-7.0.0/tests/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/json/test_work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/xml/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/xml/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/xml/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/commands/xml/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/fixtures/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/fixtures/mqtt_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/hardware/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/helpers/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/json/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/mqtt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/test_mqtt_client_reconnect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:58.456453 deebot_client-7.0.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/util/test_continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/util/test_countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 08:38:53.000000 deebot_client-7.0.0/tests/util/test_init.py
```

### Comparing `deebot-client-6.0.2/.devcontainer.json` & `deebot_client-7.0.0/.devcontainer.json`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         "editor.formatOnSave": true,
         "editor.formatOnType": true,
         "editor.tabSize": 4,
         "files.eol": "\n",
         "files.trimTrailingWhitespace": true,
         "python.analysis.autoImportCompletions": true,
         "python.analysis.autoSearchPaths": false,
-        "python.analysis.extraPaths": ["/home/vscode/.local/lib/python3.11/"],
+        "python.analysis.extraPaths": ["/home/vscode/.local/lib/python3.12/"],
         "python.analysis.typeCheckingMode": "basic",
         "python.defaultInterpreterPath": "/usr/local/bin/python",
         "python.formatting.autopep8Path": "/usr/local/py-utils/bin/autopep8",
         "python.formatting.blackPath": "/usr/local/py-utils/bin/black",
         "python.formatting.provider": "black",
         "python.formatting.yapfPath": "/usr/local/py-utils/bin/yapf",
         "python.languageServer": "Pylance",
```

### Comparing `deebot-client-6.0.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `deebot_client-7.0.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/.github/release-drafter.yml` & `deebot_client-7.0.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/.github/workflows/ci.yml` & `deebot_client-7.0.0/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   code-quality:
     runs-on: "ubuntu-latest"
     name: Check code quality
     steps:
       - uses: "actions/checkout@v4"
       - name: Set up Python ${{ env.DEFAULT_PYTHON }}
         id: python
-        uses: actions/setup-python@v5.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: ${{ env.DEFAULT_PYTHON }}
           cache: "pip"
           cache-dependency-path: "requirements*"
       - name: Install dependencies
         run: |
           pip install -r requirements.txt
@@ -36,28 +36,28 @@
         run: scripts/check_getLogger.sh
 
   tests:
     runs-on: "ubuntu-latest"
     name: Run tests
     strategy:
       matrix:
-        python-version: ["3.11", "3.12"]
+        python-version: ["3.12"]
     steps:
       - uses: "actions/checkout@v4"
       - name: Set up Python ${{ matrix.python-version }}
         id: python
-        uses: actions/setup-python@v5.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: "requirements*"
       - name: Install dependencies
         run: |
           pip install -r requirements.txt
           pip install -r requirements-test.txt
       - name: Run pytest
         run: pytest --cov=./ --cov-report=xml
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           fail_ci_if_error: true
```

### Comparing `deebot-client-6.0.2/.github/workflows/codeql-analysis.yml` & `deebot_client-7.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/.github/workflows/python-publish.yml` & `deebot_client-7.0.0/.github/workflows/python-publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     permissions:
       id-token: write
     steps:
       - name: 📥 Checkout the repository
         uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v5.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: "3.12"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -q build
```

### Comparing `deebot-client-6.0.2/.pre-commit-config.yaml` & `deebot_client-7.0.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -7,41 +7,41 @@
     - verifyNoGetLogger
 
 default_language_version:
   python: python3.12
 
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.3.7
     hooks:
       - id: ruff
         args:
           - --fix
           # - --unsafe-fixes
       - id: ruff-format
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args:
-          - --py311-plus
+          - --py312-plus
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         args:
           - --ignore-words-list=deebot
           - --skip="./.*,*.csv,*.json"
           - --quiet-level=2
           - --exclude-file=deebot_client/util/continents.py
         exclude_types:
           - csv
           - json
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: detect-private-key
       - id: no-commit-to-branch
         args: [--branch, main, --branch, dev]
       - id: requirements-txt-fixer
@@ -51,15 +51,15 @@
       - id: prettier
         additional_dependencies:
           - prettier@3.2.4
           - prettier-plugin-sort-json@3.1.0
         exclude_types:
           - python
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.35.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
   - repo: local
     hooks:
       # Run mypy through our wrapper script in order to get the possible
       # pyenv and/or virtualenv activated; it may not have been e.g. if
       # committing from a GUI tool that was not launched from an activated
```

### Comparing `deebot-client-6.0.2/.yamllint` & `deebot_client-7.0.0/.yamllint`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/LICENSE.txt` & `deebot_client-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/PKG-INFO` & `deebot_client-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 6.0.2
+Version: 7.0.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp~=3.9
 Requires-Dist: aiomqtt<3.0,>=2.0.0
 Requires-Dist: cachetools<6.0,>=5.0.0
 Requires-Dist: defusedxml
 Requires-Dist: numpy<2.0,>=1.23.2
@@ -48,31 +48,30 @@
 import aiohttp
 import asyncio
 import logging
 import time
 
 from deebot_client.api_client import ApiClient
 from deebot_client.authentication import Authenticator, create_rest_config
-from deebot_client.commands import *
-from deebot_client.commands.clean import CleanAction
+from deebot_client.commands.json.clean import CleanAction
 from deebot_client.events import BatteryEvent
 from deebot_client.mqtt_client import MqttClient, create_mqtt_config
 from deebot_client.util import md5
 from deebot_client.device import Device
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
-country = "de"
+country = "DE"
 
 
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
-    rest_config = create_rest_config(session, device_id=device_id, country=country)
+    rest_config = create_rest_config(session, device_id=device_id, alpha_2_country=country)
 
     authenticator = Authenticator(rest_config, account_id, password_hash)
     api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
     bot = Device(devices_[0], authenticator)
```

### Comparing `deebot-client-6.0.2/README.md` & `deebot_client-7.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,30 @@
 import aiohttp
 import asyncio
 import logging
 import time
 
 from deebot_client.api_client import ApiClient
 from deebot_client.authentication import Authenticator, create_rest_config
-from deebot_client.commands import *
-from deebot_client.commands.clean import CleanAction
+from deebot_client.commands.json.clean import CleanAction
 from deebot_client.events import BatteryEvent
 from deebot_client.mqtt_client import MqttClient, create_mqtt_config
 from deebot_client.util import md5
 from deebot_client.device import Device
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
-country = "de"
+country = "DE"
 
 
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
-    rest_config = create_rest_config(session, device_id=device_id, country=country)
+    rest_config = create_rest_config(session, device_id=device_id, alpha_2_country=country)
 
     authenticator = Authenticator(rest_config, account_id, password_hash)
     api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
     bot = Device(devices_[0], authenticator)
```

### Comparing `deebot-client-6.0.2/deebot_client/api_client.py` & `deebot_client-7.0.0/deebot_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Api client module."""
+
 from __future__ import annotations
 
 import asyncio
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.hardware.deebot import get_static_device_info
```

### Comparing `deebot-client-6.0.2/deebot_client/authentication.py` & `deebot_client-7.0.0/deebot_client/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Authentication module."""
+
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from http import HTTPStatus
 import time
 from typing import TYPE_CHECKING, Any
```

### Comparing `deebot-client-6.0.2/deebot_client/capabilities.py` & `deebot_client-7.0.0/deebot_client/capabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Device capabilities module."""
+
 from __future__ import annotations
 
 from abc import ABC
 from dataclasses import dataclass, field, fields, is_dataclass
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
@@ -179,23 +180,23 @@
 
 @dataclass(frozen=True, kw_only=True)
 class CapabilitySettings:
     """Capabilities for settings."""
 
     advanced_mode: CapabilitySetEnable[AdvancedModeEvent]
     carpet_auto_fan_boost: CapabilitySetEnable[CarpetAutoFanBoostEvent] | None = None
-    efficiency_mode: (
-        CapabilitySetTypes[EfficiencyModeEvent, EfficiencyMode] | None
-    ) = None
+    efficiency_mode: CapabilitySetTypes[EfficiencyModeEvent, EfficiencyMode] | None = (
+        None
+    )
     border_switch: CapabilitySetEnable[BorderSwitchEvent] | None = None
     child_lock: CapabilitySetEnable[ChildLockEvent] | None = None
     moveup_warning: CapabilitySetEnable[MoveUpWarningEvent] | None = None
-    cross_map_border_warning: CapabilitySetEnable[
-        CrossMapBorderWarningEvent
-    ] | None = None
+    cross_map_border_warning: CapabilitySetEnable[CrossMapBorderWarningEvent] | None = (
+        None
+    )
     safe_protect: CapabilitySetEnable[SafeProtectEvent] | None = None
     ota: CapabilitySetEnable[OtaEvent] | CapabilityEvent[OtaEvent] | None = None
     sweep_mode: CapabilitySetEnable[SweepModeEvent] | None = None
     true_detect: CapabilitySetEnable[TrueDetectEvent] | None = None
     voice_assistant: CapabilitySetEnable[VoiceAssistantStateEvent] | None = None
     volume: CapabilitySet[VolumeEvent, int]
```

### Comparing `deebot-client-6.0.2/deebot_client/command.py` & `deebot_client-7.0.0/deebot_client/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base command."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 import asyncio
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, final
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/__init__.py` & `deebot_client-7.0.0/deebot_client/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Commands module."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from deebot_client.const import DataType
 
 from .json import (
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/__init__.py` & `deebot_client-7.0.0/deebot_client/commands/json/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Json commands module."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from deebot_client.command import Command, CommandMqttP2P
 
 from .advanced_mode import GetAdvancedMode, SetAdvancedMode
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/carpet.py` & `deebot_client-7.0.0/deebot_client/commands/json/carpet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Carpet pressure command module."""
+
 from __future__ import annotations
 
 from deebot_client.events import CarpetAutoFanBoostEvent
 
 from .common import GetEnableCommand, SetEnableCommand
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/charge.py` & `deebot_client-7.0.0/deebot_client/commands/json/charge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Charge commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import StateEvent
 from deebot_client.logging_filter import get_logger
 from deebot_client.message import HandlingResult
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/charge_state.py` & `deebot_client-7.0.0/deebot_client/commands/json/charge_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Charge state commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import StateEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
 from deebot_client.models import State
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/clean.py` & `deebot_client-7.0.0/deebot_client/commands/json/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Clean commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import StateEvent
 from deebot_client.logging_filter import get_logger
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/clean_count.py` & `deebot_client-7.0.0/deebot_client/commands/json/clean_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Clean count command module."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import CleanCountEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/clean_logs.py` & `deebot_client-7.0.0/deebot_client/commands/json/clean_logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """clean log commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import CommandResult
 from deebot_client.const import PATH_API_LG_LOG, REQUEST_HEADERS
 from deebot_client.events import CleanJobStatus, CleanLogEntry, CleanLogEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/common.py` & `deebot_client-7.0.0/deebot_client/commands/json/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base commands."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from datetime import datetime
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/continuous_cleaning.py` & `deebot_client-7.0.0/deebot_client/commands/json/continuous_cleaning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Continuous cleaning (break point) command module."""
+
 from __future__ import annotations
 
 from deebot_client.events import ContinuousCleaningEvent
 
 from .common import GetEnableCommand, SetEnableCommand
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/cross_map_border_warning.py` & `deebot_client-7.0.0/deebot_client/commands/json/cross_map_border_warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cross map border warning commands."""
+
 from __future__ import annotations
 
 from deebot_client.events import CrossMapBorderWarningEvent
 
 from .common import GetEnableCommand, SetEnableCommand
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/custom.py` & `deebot_client-7.0.0/deebot_client/commands/json/custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom command module."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import CommandResult
 from deebot_client.commands.json.common import JsonCommand
 from deebot_client.events import CustomCommandEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/efficiency.py` & `deebot_client-7.0.0/deebot_client/commands/json/efficiency.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Efficiency mode command module."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import EfficiencyMode, EfficiencyModeEvent
 from deebot_client.message import HandlingResult
+from deebot_client.util import get_enum
 
 from .common import JsonGetCommand, JsonSetCommand
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
 
 
@@ -36,9 +38,9 @@
 
     name = "setEfficiency"
     get_command = GetEfficiencyMode
     _mqtt_params = MappingProxyType({"efficiency": InitParam(EfficiencyMode)})
 
     def __init__(self, efficiency: EfficiencyMode | str) -> None:
         if isinstance(efficiency, str):
-            efficiency = EfficiencyMode.get(efficiency)
+            efficiency = get_enum(EfficiencyMode, efficiency)
         super().__init__({"efficiency": efficiency.value})
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/error.py` & `deebot_client-7.0.0/deebot_client/commands/json/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Error commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.const import ERROR_CODES
 from deebot_client.events import ErrorEvent, StateEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/fan_speed.py` & `deebot_client-7.0.0/deebot_client/commands/json/fan_speed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """(fan) speed commands."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import FanSpeedEvent, FanSpeedLevel
 from deebot_client.message import HandlingResult
+from deebot_client.util import get_enum
 
 from .common import JsonGetCommand, JsonSetCommand
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
 
 
@@ -36,9 +38,9 @@
 
     name = "setSpeed"
     get_command = GetFanSpeed
     _mqtt_params = MappingProxyType({"speed": InitParam(FanSpeedLevel)})
 
     def __init__(self, speed: FanSpeedLevel | str) -> None:
         if isinstance(speed, str):
-            speed = FanSpeedLevel.get(speed)
+            speed = get_enum(FanSpeedLevel, speed)
         super().__init__({"speed": speed.value})
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/life_span.py` & `deebot_client-7.0.0/deebot_client/commands/json/life_span.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Life span commands."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import CommandMqttP2P, InitParam
 from deebot_client.events import LifeSpan, LifeSpanEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/map.py` & `deebot_client-7.0.0/deebot_client/commands/json/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Maps commands."""
+
 from __future__ import annotations
 
 import json
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import Command, CommandResult
@@ -131,17 +132,16 @@
     _ARGS_SUBSETS = "subsets"
 
     name = "getMapSet"
 
     def __init__(
         self,
         mid: str,
-        type: (  # pylint: disable=redefined-builtin
-            MapSetType | str
-        ) = MapSetType.ROOMS,
+        # pylint: disable=redefined-builtin
+        type: (MapSetType | str) = MapSetType.ROOMS,
     ) -> None:
         if isinstance(type, MapSetType):
             type = type.value
 
         super().__init__({"mid": mid, "type": type})
 
     @classmethod
@@ -222,17 +222,16 @@
 
     def __init__(
         self,
         *,
         mid: str | int,
         mssid: str | int,
         msid: str | int | None = None,
-        type: (  # pylint: disable=redefined-builtin
-            MapSetType | str
-        ) = MapSetType.ROOMS,
+        # pylint: disable=redefined-builtin
+        type: (MapSetType | str) = MapSetType.ROOMS,
     ) -> None:
         if isinstance(type, MapSetType):
             type = type.value
 
         if msid is None and type == MapSetType.ROOMS.value:
             error_msid_type = f"msid is required when type='{MapSetType.ROOMS.value}'"
             raise ValueError(error_msid_type)
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/network.py` & `deebot_client-7.0.0/deebot_client/commands/json/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Network commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import NetworkInfoEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/ota.py` & `deebot_client-7.0.0/deebot_client/commands/json/ota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Ota command module."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import OtaEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/pos.py` & `deebot_client-7.0.0/deebot_client/commands/json/pos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Position command module."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import Position, PositionsEvent, PositionType
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/stats.py` & `deebot_client-7.0.0/deebot_client/commands/json/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Stats commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import StatsEvent, TotalStatsEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/voice_assistant_state.py` & `deebot_client-7.0.0/deebot_client/commands/json/voice_assistant_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Voice assistant state command module."""
+
 from __future__ import annotations
 
 from deebot_client.events import VoiceAssistantStateEvent
 
 from .common import GetEnableCommand, SetEnableCommand
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/volume.py` & `deebot_client-7.0.0/deebot_client/commands/json/volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Volume command module."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import VolumeEvent
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/water_info.py` & `deebot_client-7.0.0/deebot_client/commands/json/water_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Water info commands."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import WaterAmount, WaterInfoEvent
 from deebot_client.message import HandlingResult
+from deebot_client.util import get_enum
 
 from .common import JsonGetCommand, JsonSetCommand
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
 
 
@@ -47,9 +49,9 @@
             "amount": InitParam(WaterAmount),
             "enable": None,  # Remove it as we don't can set it (App includes it)
         }
     )
 
     def __init__(self, amount: WaterAmount | str) -> None:
         if isinstance(amount, str):
-            amount = WaterAmount.get(amount)
+            amount = get_enum(WaterAmount, amount)
         super().__init__({"amount": amount.value})
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/json/work_mode.py` & `deebot_client-7.0.0/deebot_client/commands/json/work_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Work mode commands."""
+
 from __future__ import annotations
 
 from types import MappingProxyType
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.command import InitParam
 from deebot_client.events import WorkMode, WorkModeEvent
 from deebot_client.message import HandlingResult
+from deebot_client.util import get_enum
 
 from .common import JsonGetCommand, JsonSetCommand
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
 
 
@@ -36,9 +38,9 @@
 
     name = "setWorkMode"
     get_command = GetWorkMode
     _mqtt_params = MappingProxyType({"mode": InitParam(WorkMode)})
 
     def __init__(self, mode: WorkMode | str) -> None:
         if isinstance(mode, str):
-            mode = WorkMode.get(mode)
+            mode = get_enum(WorkMode, mode)
         super().__init__({"mode": mode.value})
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/xml/__init__.py` & `deebot_client-7.0.0/deebot_client/commands/xml/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Xml commands module."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from deebot_client.command import Command, CommandMqttP2P
 
+from .charge_state import GetChargeState
 from .error import GetError
+from .fan_speed import GetFanSpeed
+from .pos import GetPos
 
 if TYPE_CHECKING:
     from .common import XmlCommand
 
 __all__ = [
+    "GetChargeState",
     "GetError",
+    "GetFanSpeed",
+    "GetPos",
 ]
 
 # fmt: off
 # ordered by file asc
 _COMMANDS: list[type[XmlCommand]] = [
     GetError,
 ]
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/xml/common.py` & `deebot_client-7.0.0/deebot_client/commands/xml/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common xml based commands."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, cast
 from xml.etree.ElementTree import Element, SubElement
 
 from defusedxml import ElementTree  # type: ignore[import-untyped]
```

### Comparing `deebot-client-6.0.2/deebot_client/commands/xml/error.py` & `deebot_client-7.0.0/deebot_client/commands/xml/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Error commands."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from deebot_client.const import ERROR_CODES
 from deebot_client.events import ErrorEvent, StateEvent
 from deebot_client.message import HandlingResult
```

### Comparing `deebot-client-6.0.2/deebot_client/const.py` & `deebot_client-7.0.0/deebot_client/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants module."""
+
 from __future__ import annotations
 
 from enum import Enum, StrEnum
 from typing import Self
 
 REALM = "ecouser.net"
 PATH_API_APPSVR_APP = "appsvr/app.do"
```

### Comparing `deebot-client-6.0.2/deebot_client/device.py` & `deebot_client-7.0.0/deebot_client/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Device module."""
+
 from __future__ import annotations
 
 import asyncio
 from contextlib import suppress
 from datetime import datetime
 import json
 from typing import TYPE_CHECKING, Any, Final, Generic
```

### Comparing `deebot-client-6.0.2/deebot_client/event_bus.py` & `deebot_client-7.0.0/deebot_client/event_bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Event emitter module."""
+
 from __future__ import annotations
 
 import asyncio
 from datetime import UTC, datetime, timedelta
 import threading
 from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar
```

### Comparing `deebot-client-6.0.2/deebot_client/events/__init__.py` & `deebot_client-7.0.0/deebot_client/events/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Events module."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
-from enum import Enum, unique
+from enum import Enum, IntEnum, unique
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events.base import Event
-from deebot_client.util import DisplayNameIntEnum
 
 from .efficiency_mode import EfficiencyMode, EfficiencyModeEvent
 from .fan_speed import FanSpeedEvent, FanSpeedLevel
 from .map import (
     CachedMapInfoEvent,
     MajorMapEvent,
     MapChangedEvent,
@@ -62,23 +62,24 @@
 @dataclass(frozen=True)
 class BatteryEvent(Event):
     """Battery event representation."""
 
     value: int
 
 
-class CleanJobStatus(DisplayNameIntEnum):
+@unique
+class CleanJobStatus(IntEnum):
     """Enum of the different clean job status."""
 
     NO_STATUS = -2
     CLEANING = -1
     # below the identified stop_reason values
     FINISHED = 1
-    MANUAL_STOPPED = 2, "manual stopped"
-    FINISHED_WITH_WARNINGS = 3, "finished with warnings"
+    MANUALLY_STOPPED = 2
+    FINISHED_WITH_WARNINGS = 3
 
 
 @dataclass(frozen=True)
 class CleanLogEntry:
     """Clean log entry representation."""
 
     timestamp: int
```

### Comparing `deebot-client-6.0.2/deebot_client/events/map.py` & `deebot_client-7.0.0/deebot_client/events/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Map event module."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from enum import Enum, unique
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import Event
```

### Comparing `deebot-client-6.0.2/deebot_client/events/water_info.py` & `deebot_client-7.0.0/deebot_client/events/water_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Water info event module."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-
-from deebot_client.util import DisplayNameIntEnum
+from enum import IntEnum, unique
 
 from .base import Event
 
 
-class WaterAmount(DisplayNameIntEnum):
+@unique
+class WaterAmount(IntEnum):
     """Enum class for all possible water amounts."""
 
     LOW = 1
     MEDIUM = 2
     HIGH = 3
     ULTRAHIGH = 4
```

### Comparing `deebot-client-6.0.2/deebot_client/exceptions.py` & `deebot_client-7.0.0/deebot_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot client exception module."""
+
 from __future__ import annotations
 
 
 class DeebotError(Exception):
     """Deebot error."""
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/2o4lnm.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/2o4lnm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """DEEBOT X1 Turbo Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/55aiho.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/55aiho.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """DEEBOT OZMO T8 AIVI Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/5xu9h3.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/5xu9h3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """DEEBOT GOAT G1 Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/626v6g.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/626v6g.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/85nbtp.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/85nbtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T20 Omni Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/9ku8nu.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/9ku8nu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T20 Omni Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/__init__.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hardware deebot module."""
+
 from __future__ import annotations
 
 import importlib
 import pkgutil
 from typing import TYPE_CHECKING
 
 from deebot_client.logging_filter import get_logger
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/clojes.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/clojes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/fallback.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/fallback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fallback Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/lx3j7m.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/lf3bn4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T20 Omni Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/p1jij8.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/lx3j7m.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T20 Omni Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/p95mgv.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/p95mgv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/rss8xk.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/rss8xk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/umwv6z.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/umwv6z.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/vi829v.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/vi829v.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot Ozmo 920/950 Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/x5d34r.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/x5d34r.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """DEEBOT OZMO T8 AIVI Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/yna5xi.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/yna5xi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot Ozmo 920/950 Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/hardware/deebot/zjavof.py` & `deebot_client-7.0.0/deebot_client/hardware/deebot/zjavof.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Deebot T10 PLUS Capabilities."""
+
 from __future__ import annotations
 
 from deebot_client.capabilities import (
     CapabilityClean,
     CapabilityCleanAction,
     CapabilityCustomCommand,
     CapabilityEvent,
```

### Comparing `deebot-client-6.0.2/deebot_client/logging_filter.py` & `deebot_client-7.0.0/deebot_client/logging_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logging filter module."""
+
 from __future__ import annotations
 
 import copy
 from logging import Filter, Logger, LogRecord, getLogger
 from typing import Any
```

### Comparing `deebot-client-6.0.2/deebot_client/map.py` & `deebot_client-7.0.0/deebot_client/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Map module."""
+
 from __future__ import annotations
 
 import ast
 import asyncio
 import base64
 import dataclasses
 from datetime import UTC, datetime
```

### Comparing `deebot-client-6.0.2/deebot_client/message.py` & `deebot_client-7.0.0/deebot_client/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base messages."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import IntEnum, auto
 import functools
 from typing import TYPE_CHECKING, Any, TypeVar, final
```

### Comparing `deebot-client-6.0.2/deebot_client/messages/__init__.py` & `deebot_client-7.0.0/deebot_client/messages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Messages module."""
+
 from __future__ import annotations
 
 import re
 
 from deebot_client.const import DataType
 from deebot_client.logging_filter import get_logger
 from deebot_client.message import Message
```

### Comparing `deebot-client-6.0.2/deebot_client/messages/json/__init__.py` & `deebot_client-7.0.0/deebot_client/messages/json/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Json messages."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from .battery import OnBattery
 from .map import OnMapSetV2
 from .stats import ReportStats
```

### Comparing `deebot-client-6.0.2/deebot_client/messages/json/battery.py` & `deebot_client-7.0.0/deebot_client/messages/json/battery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Battery messages."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import BatteryEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/messages/json/map.py` & `deebot_client-7.0.0/deebot_client/messages/json/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Map set v2 messages."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events.map import MapSetType
 from deebot_client.message import HandlingResult, HandlingState, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/messages/json/stats.py` & `deebot_client-7.0.0/deebot_client/messages/json/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Stats messages."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from deebot_client.events import CleanJobStatus, ReportStatsEvent
 from deebot_client.message import HandlingResult, MessageBodyDataDict
```

### Comparing `deebot-client-6.0.2/deebot_client/models.py` & `deebot_client-7.0.0/deebot_client/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Models module."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import IntEnum, StrEnum, unique
 from pathlib import Path
 from typing import TYPE_CHECKING, Generic, Required, TypedDict, TypeVar
```

### Comparing `deebot-client-6.0.2/deebot_client/mqtt_client.py` & `deebot_client-7.0.0/deebot_client/mqtt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT module."""
+
 from __future__ import annotations
 
 import asyncio
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
 import json
@@ -121,17 +122,17 @@
         config: MqttConfiguration,
         authenticator: Authenticator,
     ) -> None:
         self._config = config
         self._authenticator = authenticator
 
         self._subscriptions: MutableMapping[str, SubscriberInfo] = {}
-        self._subscription_changes: asyncio.Queue[
-            tuple[SubscriberInfo, bool]
-        ] = asyncio.Queue()
+        self._subscription_changes: asyncio.Queue[tuple[SubscriberInfo, bool]] = (
+            asyncio.Queue()
+        )
         self._mqtt_task: asyncio.Task[Any] | None = None
 
         self._received_p2p_commands: MutableMapping[str, CommandMqttP2P] = TTLCache(
             maxsize=60 * 60, ttl=60
         )
         self._last_message_received_at: datetime | None = None
```

### Comparing `deebot-client-6.0.2/deebot_client/util/continents.py` & `deebot_client-7.0.0/deebot_client/util/continents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Continents module."""
+
 from __future__ import annotations
 
 from deebot_client.const import COUNTRY_CHINA
 
 
 def get_continent(alpha_2_country: str | None) -> str:
     """Return the continent for the given country or ww."""
```

### Comparing `deebot-client-6.0.2/deebot_client.egg-info/PKG-INFO` & `deebot_client-7.0.0/deebot_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 6.0.2
+Version: 7.0.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp~=3.9
 Requires-Dist: aiomqtt<3.0,>=2.0.0
 Requires-Dist: cachetools<6.0,>=5.0.0
 Requires-Dist: defusedxml
 Requires-Dist: numpy<2.0,>=1.23.2
@@ -48,31 +48,30 @@
 import aiohttp
 import asyncio
 import logging
 import time
 
 from deebot_client.api_client import ApiClient
 from deebot_client.authentication import Authenticator, create_rest_config
-from deebot_client.commands import *
-from deebot_client.commands.clean import CleanAction
+from deebot_client.commands.json.clean import CleanAction
 from deebot_client.events import BatteryEvent
 from deebot_client.mqtt_client import MqttClient, create_mqtt_config
 from deebot_client.util import md5
 from deebot_client.device import Device
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
-country = "de"
+country = "DE"
 
 
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
-    rest_config = create_rest_config(session, device_id=device_id, country=country)
+    rest_config = create_rest_config(session, device_id=device_id, alpha_2_country=country)
 
     authenticator = Authenticator(rest_config, account_id, password_hash)
     api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
     bot = Device(devices_[0], authenticator)
```

### Comparing `deebot-client-6.0.2/deebot_client.egg-info/SOURCES.txt` & `deebot_client-7.0.0/deebot_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,19 @@
 deebot_client/commands/json/sweep_mode.py
 deebot_client/commands/json/true_detect.py
 deebot_client/commands/json/voice_assistant_state.py
 deebot_client/commands/json/volume.py
 deebot_client/commands/json/water_info.py
 deebot_client/commands/json/work_mode.py
 deebot_client/commands/xml/__init__.py
+deebot_client/commands/xml/charge_state.py
 deebot_client/commands/xml/common.py
 deebot_client/commands/xml/error.py
+deebot_client/commands/xml/fan_speed.py
+deebot_client/commands/xml/pos.py
 deebot_client/events/__init__.py
 deebot_client/events/base.py
 deebot_client/events/efficiency_mode.py
 deebot_client/events/fan_speed.py
 deebot_client/events/map.py
 deebot_client/events/network.py
 deebot_client/events/water_info.py
@@ -99,17 +102,20 @@
 deebot_client/hardware/deebot/5xu9h3.py
 deebot_client/hardware/deebot/626v6g.py
 deebot_client/hardware/deebot/85nbtp.py
 deebot_client/hardware/deebot/9ku8nu.py
 deebot_client/hardware/deebot/__init__.py
 deebot_client/hardware/deebot/clojes.py
 deebot_client/hardware/deebot/fallback.py
+deebot_client/hardware/deebot/itk04l.py
+deebot_client/hardware/deebot/lf3bn4.py
 deebot_client/hardware/deebot/lx3j7m.py
 deebot_client/hardware/deebot/p1jij8.py
 deebot_client/hardware/deebot/p95mgv.py
+deebot_client/hardware/deebot/paeygf.py
 deebot_client/hardware/deebot/rss8xk.py
 deebot_client/hardware/deebot/umwv6z.py
 deebot_client/hardware/deebot/vi829v.py
 deebot_client/hardware/deebot/x5d34r.py
 deebot_client/hardware/deebot/yna5xi.py
 deebot_client/hardware/deebot/zjavof.py
 deebot_client/messages/__init__.py
@@ -163,17 +169,19 @@
 tests/commands/json/test_sweep_mode.py
 tests/commands/json/test_true_detect.py
 tests/commands/json/test_voice_assistant_state.py
 tests/commands/json/test_volume.py
 tests/commands/json/test_water_info.py
 tests/commands/json/test_work_mode.py
 tests/commands/xml/__init__.py
+tests/commands/xml/test_charge_state.py
 tests/commands/xml/test_error.py
+tests/commands/xml/test_fan_speed.py
+tests/commands/xml/test_pos.py
 tests/events/__init__.py
-tests/events/test_water_info.py
 tests/fixtures/__init__.py
 tests/fixtures/base.py
 tests/fixtures/mqtt_server.py
 tests/hardware/__init__.py
 tests/hardware/test_init.py
 tests/helpers/__init__.py
 tests/helpers/tasks.py
```

### Comparing `deebot-client-6.0.2/mypy.ini` & `deebot_client-7.0.0/mypy.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [mypy]
-python_version = 3.11
+python_version = 3.12
 show_error_codes = true
 strict_equality = true
 warn_incomplete_stub = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
 check_untyped_defs = true
```

### Comparing `deebot-client-6.0.2/pyproject.toml` & `deebot_client-7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     {name = "Robert Resch", email = "robert@resch.dev"}
 ]
 keywords    = ["home", "automation", "homeassistant", "vacuum", "robot", "deebot", "ecovacs"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Home Automation",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-requires-python = ">=3.11.0"
+requires-python = ">=3.12.0"
 dynamic = ["dependencies", "version"]
 
 [project.urls]
 "Homepage"    = "https://deebot.readthedocs.io/"
 "Source Code" = "https://github.com/DeebotUniverse/client.py"
 "Bug Reports" = "https://github.com/DeebotUniverse/client.py/issues"
 
@@ -115,15 +115,15 @@
 max-complexity = 12
 
 [tool.ruff.lint.pylint]
 max-args = 7
 
 
 [tool.pylint.MAIN]
-py-version = "3.11"
+py-version = "3.12"
 ignore = [
     "tests",
 ]
 fail-on = [
     "I",
 ]
```

### Comparing `deebot-client-6.0.2/scripts/check_getLogger.sh` & `deebot_client-7.0.0/scripts/check_getLogger.sh`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/__init__.py` & `deebot_client-7.0.0/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/__init__.py` & `deebot_client-7.0.0/tests/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_advanced_mode.py` & `deebot_client-7.0.0/tests/commands/json/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_battery.py` & `deebot_client-7.0.0/tests/commands/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_border_switch.py` & `deebot_client-7.0.0/tests/commands/json/test_border_switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests regarding border switch commands."""
+
 from __future__ import annotations
 
 import pytest
 
 from deebot_client.commands.json import GetBorderSwitch, SetBorderSwitch
 from deebot_client.events import BorderSwitchEvent
 from tests.helpers import get_request_json, get_success_body
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_carpet.py` & `deebot_client-7.0.0/tests/commands/json/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_charge.py` & `deebot_client-7.0.0/tests/commands/json/test_charge.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,9 +42,9 @@
     await assert_command(
         Charge(), json, None, command_result=CommandResult(HandlingState.FAILED)
     )
 
     assert (
         "deebot_client.commands.json.common",
         logging.WARNING,
-        f"Command \"charge\" was not successfully. body={json['resp']['body']}",
+        f'Command "charge" was not successfully. body={json['resp']['body']}',
     ) in caplog.record_tuples
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_charge_state.py` & `deebot_client-7.0.0/tests/commands/json/test_charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_child_lock.py` & `deebot_client-7.0.0/tests/commands/json/test_child_lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests regarding child lock commands."""
+
 from __future__ import annotations
 
 import pytest
 
 from deebot_client.commands.json import GetChildLock, SetChildLock
 from deebot_client.events import ChildLockEvent
 from tests.helpers import get_request_json, get_success_body
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_clean.py` & `deebot_client-7.0.0/tests/commands/json/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_clean_count.py` & `deebot_client-7.0.0/tests/commands/json/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_clean_log.py` & `deebot_client-7.0.0/tests/commands/json/test_clean_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                 duration=366,
             ),
             CleanLogEntry(
                 timestamp=1655564399,
                 image_url="https://portal-eu.ecouser.net/api/lg/image/acb2e78e-8f25-454a-a0ac-***@***@iCmB",
                 type="spotArea",
                 area=0,
-                stop_reason=CleanJobStatus.MANUAL_STOPPED,
+                stop_reason=CleanJobStatus.MANUALLY_STOPPED,
                 duration=61,
             ),
             CleanLogEntry(
                 timestamp=1655564222,
                 image_url="https://portal-eu.ecouser.net/api/lg/image/acb2e78e-8f25-454a-a0ac-***@***@iCmB",
                 type="spotArea",
                 area=0,
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_clean_preference.py` & `deebot_client-7.0.0/tests/commands/json/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_common.py` & `deebot_client-7.0.0/tests/commands/json/test_common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_continuous_cleaning.py` & `deebot_client-7.0.0/tests/commands/json/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_cross_map_border_warning.py` & `deebot_client-7.0.0/tests/commands/json/test_cross_map_border_warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests regarding cross map border warning commands."""
+
 from __future__ import annotations
 
 import pytest
 
 from deebot_client.commands.json import (
     GetCrossMapBorderWarning,
     SetCrossMapBorderWarning,
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_custom.py` & `deebot_client-7.0.0/tests/commands/json/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_efficiency.py` & `deebot_client-7.0.0/tests/commands/json/test_efficiency.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 import pytest
 
 from deebot_client.commands.json import GetEfficiencyMode, SetEfficiencyMode
 from deebot_client.events import EfficiencyMode, EfficiencyModeEvent
 from tests.helpers import (
     get_request_json,
     get_success_body,
-    verify_DisplayNameEnum_unique,
 )
 
 from . import assert_command, assert_set_command
 
 
-def test_WorkMode_unique() -> None:
-    verify_DisplayNameEnum_unique(EfficiencyMode)
-
-
 @pytest.mark.parametrize(
     ("json", "expected"),
     [
         ({"efficiency": 0}, EfficiencyModeEvent(EfficiencyMode.STANDARD_MODE)),
         ({"efficiency": 1}, EfficiencyModeEvent(EfficiencyMode.ENERGY_EFFICIENT_MODE)),
     ],
 )
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_error.py` & `deebot_client-7.0.0/tests/commands/json/test_error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_fan_speed.py` & `deebot_client-7.0.0/tests/commands/json/test_fan_speed.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,19 @@
 
 from deebot_client.commands.json import GetFanSpeed, SetFanSpeed
 from deebot_client.events import FanSpeedEvent
 from deebot_client.events.fan_speed import FanSpeedLevel
 from tests.helpers import (
     get_request_json,
     get_success_body,
-    verify_DisplayNameEnum_unique,
 )
 
 from . import assert_command, assert_set_command
 
 
-def test_FanSpeedLevel_unique() -> None:
-    verify_DisplayNameEnum_unique(FanSpeedLevel)
-
-
 async def test_GetFanSpeed() -> None:
     json = get_request_json(get_success_body({"speed": 2}))
     await assert_command(GetFanSpeed(), json, FanSpeedEvent(FanSpeedLevel.MAX_PLUS))
 
 
 @pytest.mark.parametrize(("value"), [FanSpeedLevel.MAX, "max"])
 async def test_SetFanSpeed(value: FanSpeedLevel | str) -> None:
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_life_span.py` & `deebot_client-7.0.0/tests/commands/json/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_map.py` & `deebot_client-7.0.0/tests/commands/json/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_moveup_warning.py` & `deebot_client-7.0.0/tests/commands/json/test_moveup_warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests regarding moveup warning commands."""
+
 from __future__ import annotations
 
 import pytest
 
 from deebot_client.commands.json import GetMoveUpWarning, SetMoveUpWarning
 from deebot_client.events import MoveUpWarningEvent
 from tests.helpers import get_request_json, get_success_body
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_mulitmap_state.py` & `deebot_client-7.0.0/tests/commands/json/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_network.py` & `deebot_client-7.0.0/tests/commands/json/test_network.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_ota.py` & `deebot_client-7.0.0/tests/commands/json/test_ota.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_safe_protect.py` & `deebot_client-7.0.0/tests/commands/json/test_safe_protect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests regarding safe protect commands."""
+
 from __future__ import annotations
 
 import pytest
 
 from deebot_client.commands.json import GetSafeProtect, SetSafeProtect
 from deebot_client.events import SafeProtectEvent
 from tests.helpers import get_request_json, get_success_body
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_sweep_mode.py` & `deebot_client-7.0.0/tests/commands/json/test_sweep_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_true_detect.py` & `deebot_client-7.0.0/tests/commands/json/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_voice_assistant_state.py` & `deebot_client-7.0.0/tests/commands/json/test_voice_assistant_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_volume.py` & `deebot_client-7.0.0/tests/commands/json/test_volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/commands/json/test_water_info.py` & `deebot_client-7.0.0/tests/commands/json/test_water_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 import pytest
 
 from deebot_client.commands.json import GetWaterInfo, SetWaterInfo
 from deebot_client.events import WaterAmount, WaterInfoEvent
 from tests.helpers import (
     get_request_json,
     get_success_body,
-    verify_DisplayNameEnum_unique,
 )
 
 from . import assert_command, assert_set_command
 
 
-def test_WaterAmount_unique() -> None:
-    verify_DisplayNameEnum_unique(WaterAmount)
-
-
 @pytest.mark.parametrize(
     ("json", "expected"),
     [
         ({"amount": 2}, WaterInfoEvent(WaterAmount.MEDIUM)),
         (
             {"amount": 1, "enable": 1},
             WaterInfoEvent(WaterAmount.LOW, mop_attached=True),
```

### Comparing `deebot-client-6.0.2/tests/commands/json/test_work_mode.py` & `deebot_client-7.0.0/tests/commands/json/test_work_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 import pytest
 
 from deebot_client.commands.json import GetWorkMode, SetWorkMode
 from deebot_client.events import WorkMode, WorkModeEvent
 from tests.helpers import (
     get_request_json,
     get_success_body,
-    verify_DisplayNameEnum_unique,
 )
 
 from . import assert_command, assert_set_command
 
 
-def test_WorkMode_unique() -> None:
-    verify_DisplayNameEnum_unique(WorkMode)
-
-
 @pytest.mark.parametrize(
     ("json", "expected"),
     [
         ({"mode": 0}, WorkModeEvent(WorkMode.VACUUM_AND_MOP)),
         ({"mode": 1}, WorkModeEvent(WorkMode.VACUUM)),
         ({"mode": 2}, WorkModeEvent(WorkMode.MOP)),
         ({"mode": 3}, WorkModeEvent(WorkMode.MOP_AFTER_VACUUM)),
```

### Comparing `deebot-client-6.0.2/tests/commands/xml/test_error.py` & `deebot_client-7.0.0/tests/commands/xml/test_error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/conftest.py` & `deebot_client-7.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/fixtures/base.py` & `deebot_client-7.0.0/tests/fixtures/base.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/fixtures/mqtt_server.py` & `deebot_client-7.0.0/tests/fixtures/mqtt_server.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/hardware/test_init.py` & `deebot_client-7.0.0/tests/hardware/test_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hardware init tests."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import pytest
 
 from deebot_client.commands.json.advanced_mode import GetAdvancedMode
@@ -159,14 +160,37 @@
                 StatsEvent: [GetStats()],
                 TotalStatsEvent: [GetTotalStats()],
                 TrueDetectEvent: [GetTrueDetect()],
                 VolumeEvent: [GetVolume()],
             },
         ),
         (
+            "itk04l",
+            {
+                AdvancedModeEvent: [GetAdvancedMode()],
+                AvailabilityEvent: [GetBattery(is_available_check=True)],
+                BatteryEvent: [GetBattery()],
+                BorderSwitchEvent: [GetBorderSwitch()],
+                ChildLockEvent: [GetChildLock()],
+                CrossMapBorderWarningEvent: [GetCrossMapBorderWarning()],
+                CustomCommandEvent: [],
+                ErrorEvent: [GetError()],
+                LifeSpanEvent: [GetLifeSpan([LifeSpan.BLADE, LifeSpan.LENS_BRUSH])],
+                MoveUpWarningEvent: [GetMoveUpWarning()],
+                NetworkInfoEvent: [GetNetInfo()],
+                ReportStatsEvent: [],
+                SafeProtectEvent: [GetSafeProtect()],
+                StateEvent: [GetChargeState(), GetCleanInfoV2()],
+                StatsEvent: [GetStats()],
+                TotalStatsEvent: [GetTotalStats()],
+                TrueDetectEvent: [GetTrueDetect()],
+                VolumeEvent: [GetVolume()],
+            },
+        ),
+        (
             "yna5xi",
             {
                 AdvancedModeEvent: [GetAdvancedMode()],
                 AvailabilityEvent: [GetBattery(is_available_check=True)],
                 BatteryEvent: [GetBattery()],
                 CachedMapInfoEvent: [GetCachedMapInfo()],
                 CarpetAutoFanBoostEvent: [GetCarpetAutoFanBoost()],
@@ -234,15 +258,15 @@
                 TrueDetectEvent: [GetTrueDetect()],
                 VoiceAssistantStateEvent: [GetVoiceAssistantState()],
                 VolumeEvent: [GetVolume()],
                 WaterInfoEvent: [GetWaterInfo()],
             },
         ),
     ],
-    ids=[FALLBACK, "5xu9h3", "yna5xi", "p95mgv"],
+    ids=[FALLBACK, "5xu9h3", "itk04l", "yna5xi", "p95mgv"],
 )
 def test_capabilities_event_extraction(
     class_: str, expected: dict[type[Event], list[Command]]
 ) -> None:
     capabilities = get_static_device_info(class_).capabilities
     assert capabilities._events.keys() == expected.keys()
     for event, expected_commands in expected.items():
@@ -259,17 +283,20 @@
         "55aiho",
         "5xu9h3",
         "626v6g",
         "85nbtp",
         "9ku8nu",
         "clojes",
         "fallback",
+        "itk04l",
+        "lf3bn4",
         "lx3j7m",
         "p1jij8",
         "p95mgv",
+        "paeygf",
         "rss8xk",
         "umwv6z",
         "vi829v",
         "x5d34r",
         "yna5xi",
         "zjavof",
     ]
```

### Comparing `deebot-client-6.0.2/tests/helpers/__init__.py` & `deebot_client-7.0.0/tests/helpers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,41 +2,22 @@
 
 from typing import TYPE_CHECKING, Any
 from unittest.mock import Mock
 
 from deebot_client.capabilities import Capabilities
 from deebot_client.const import DataType
 from deebot_client.models import StaticDeviceInfo
-from deebot_client.util import DisplayNameIntEnum
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
 
     from deebot_client.command import Command
     from deebot_client.events.base import Event
 
 
-def verify_DisplayNameEnum_unique(enum: type[DisplayNameIntEnum]) -> None:
-    assert issubclass(enum, DisplayNameIntEnum)
-    names: set[str] = set()
-    values: set[int] = set()
-    for member in enum:
-        assert member.value not in values
-        values.add(member.value)
-
-        name = member.name.lower()
-        assert name not in names
-        names.add(name)
-
-        display_name = member.display_name.lower()
-        if display_name != name:
-            assert display_name not in names
-            names.add(display_name)
-
-
 def get_request_json(body: dict[str, Any]) -> dict[str, Any]:
     return {"id": "ALZf", "ret": "ok", "resp": get_message_json(body)}
 
 
 def get_success_body(data: dict[str, Any] | None | list[Any] = None) -> dict[str, Any]:
     body = {
         "code": 0,
```

### Comparing `deebot-client-6.0.2/tests/helpers/tasks.py` & `deebot_client-7.0.0/tests/helpers/tasks.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/messages/__init__.py` & `deebot_client-7.0.0/tests/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/messages/json/test_battery.py` & `deebot_client-7.0.0/tests/messages/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/messages/json/test_map.py` & `deebot_client-7.0.0/tests/messages/json/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/messages/json/test_stats.py` & `deebot_client-7.0.0/tests/messages/json/test_stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/messages/test_get_messages.py` & `deebot_client-7.0.0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/mqtt_util.py` & `deebot_client-7.0.0/tests/mqtt_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for testing MQTT."""
+
 from __future__ import annotations
 
 import asyncio
 import datetime
 import json
 from typing import TYPE_CHECKING
 from unittest.mock import MagicMock, Mock
```

### Comparing `deebot-client-6.0.2/tests/test_authentication.py` & `deebot_client-7.0.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_command.py` & `deebot_client-7.0.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_device.py` & `deebot_client-7.0.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_event_bus.py` & `deebot_client-7.0.0/tests/test_event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_map.py` & `deebot_client-7.0.0/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_mqtt_client.py` & `deebot_client-7.0.0/tests/test_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/test_mqtt_client_reconnect.py` & `deebot_client-7.0.0/tests/test_mqtt_client_reconnect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/util/test_continents.py` & `deebot_client-7.0.0/tests/util/test_continents.py`

 * *Files identical despite different names*

### Comparing `deebot-client-6.0.2/tests/util/test_init.py` & `deebot_client-7.0.0/tests/util/test_init.py`

 * *Files identical despite different names*

