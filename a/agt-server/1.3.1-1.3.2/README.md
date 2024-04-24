# Comparing `tmp/agt_server-1.3.1.tar.gz` & `tmp/agt_server-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agt_server-1.3.1.tar", last modified: Tue Apr 23 03:31:45 2024, max compression
+gzip compressed data, was "agt_server-1.3.2.tar", last modified: Wed Apr 24 01:57:30 2024, max compression
```

## Comparing `agt_server-1.3.1.tar` & `agt_server-1.3.2.tar`

### file list

```diff
@@ -1,445 +1,445 @@
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.397487 agt_server-1.3.1/
--rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.3.1/.gitignore
--rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.3.1/LICENSE
--rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.3.1/MANIFEST.in
--rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-04-23 03:31:45.397261 agt_server-1.3.1/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.3.1/README.md
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.308274 agt_server-1.3.1/data/
--rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.3.1/data/profile.svg
--rw-r--r--   0 johnwu     (501) staff       (20)       63 2024-04-21 07:32:05.000000 agt_server-1.3.1/requirements.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-04-23 03:31:45.397527 agt_server-1.3.1/setup.cfg
--rw-r--r--   0 johnwu     (501) staff       (20)     1176 2024-04-23 03:31:39.000000 agt_server-1.3.1/setup.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.308927 agt_server-1.3.1/src/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.3.1/src/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.309019 agt_server-1.3.1/src/agt_server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.3.1/src/agt_server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.309705 agt_server-1.3.1/src/agt_server/agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.312429 agt_server-1.3.1/src/agt_server/agents/base_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2136 2024-04-03 13:09:15.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/bos_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/bosii_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/chicken_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/cm_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)    12345 2024-04-03 16:02:56.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/game_report.py
--rw-r--r--   0 johnwu     (501) staff       (20)    10046 2024-03-31 16:34:04.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/lemonade_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)    19752 2024-04-10 02:17:05.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/lsvm_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.3.1/src/agt_server/agents/base_agents/rps_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.312899 agt_server-1.3.1/src/agt_server/agents/test_agents/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.298340 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.313159 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.313543 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.313821 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.314180 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.314727 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.315155 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.315396 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.315558 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.315709 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.315864 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.316021 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.316167 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.316401 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.299731 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.316553 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_compromise/
--rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.316902 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_stubborn/
--rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.317148 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/anti_punitive/
--rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.318828 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/chipping_fish/
--rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.319053 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.319400 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.319744 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/fishing_chip/
--rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.320038 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/mystery/
--rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.320388 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.320655 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.320916 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.321176 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.321402 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.321662 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.321965 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.322513 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.322663 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.322817 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.322979 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.323154 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.323270 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_continue/
--rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.323444 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_swerve/
--rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.323895 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/basic_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.324064 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.324360 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.325842 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.327313 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.327655 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/mystery_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.328893 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
--rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.329104 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.329273 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.329576 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.329738 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.329892 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.330057 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.330333 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.330511 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.330754 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.331029 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.331261 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.331637 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.331977 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.332260 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.332508 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.332839 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/etch_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.333099 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/eyes_out/
--rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.333300 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/good_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.333559 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/hi_bot/
--rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.333875 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/increment_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.334135 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/jimbus/
--rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.334341 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/
--rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.334593 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/q_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.334812 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.335035 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/spinner/
--rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.335251 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.335518 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.335840 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.336469 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.336627 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.336789 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.337140 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/stick_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.337311 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/sticky/
--rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.337464 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/team_player/
--rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.337619 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/zenly/
--rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.303943 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.337892 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-04-01 18:00:21.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.338117 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.338338 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
--rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.338616 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.338793 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.339060 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.339458 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.339806 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:39:15.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.340326 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:54.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:01.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1258 2024-04-02 19:33:38.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.340891 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:59.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:42.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1259 2024-04-02 19:34:13.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.341472 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:05.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:45:45.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1277 2024-04-02 19:34:47.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.341936 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:10.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      187 2024-04-02 21:41:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1275 2024-04-02 18:08:23.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.342371 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:16.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      202 2024-04-02 21:46:00.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1292 2024-04-02 19:36:57.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.342904 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:22.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:46:05.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1293 2024-04-02 19:37:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.343152 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.343257 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/exponential/
--rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.343507 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ficticious_play/
--rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.343756 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/random_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.344009 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/rock_lover/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.344315 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_move/
--rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.344603 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_type/
--rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.345174 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_delay/
--rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.345435 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_disconnect/
--rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.345939 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_flood/
--rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.346290 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_math_err/
--rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.346619 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ta_agent/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
--rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/agents/test_agents/stress_test.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.305556 agt_server-1.3.1/src/agt_server/configs/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.348267 agt_server-1.3.1/src/agt_server/configs/handin_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      294 2024-04-02 18:15:54.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/lsvm_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.3.1/src/agt_server/configs/handin_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.353559 agt_server-1.3.1/src/agt_server/configs/server_configs/
--rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/bos_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/bosii_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/chicken_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/lemonade_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      623 2024-03-31 16:36:02.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/lsvm_config.json
--rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.3.1/src/agt_server/configs/server_configs/rps_config.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.353755 agt_server-1.3.1/src/agt_server/handin/
--rw-r--r--   0 johnwu     (501) staff       (20)     3656 2024-04-03 02:38:28.000000 agt_server-1.3.1/src/agt_server/handin/handin.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.353869 agt_server-1.3.1/src/agt_server/handin/results/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.3.1/src/agt_server/handin/results/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.353962 agt_server-1.3.1/src/agt_server/handin/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.3.1/src/agt_server/handin/results/bos/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.354055 agt_server-1.3.1/src/agt_server/handin/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.3.1/src/agt_server/handin/results/bosii/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.354145 agt_server-1.3.1/src/agt_server/handin/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.3.1/src/agt_server/handin/results/chicken/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.379736 agt_server-1.3.1/src/agt_server/handin/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/LemonadeArena.txt
--rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/LemonadeTest.txt
--rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.3.1/src/agt_server/handin/results/lemonade/shortcut.json
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.381787 agt_server-1.3.1/src/agt_server/handin/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.3.1/src/agt_server/handin/results/rps/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.383894 agt_server-1.3.1/src/agt_server/local_games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/local_games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)     2334 2024-04-17 23:51:57.000000 agt_server-1.3.1/src/agt_server/local_games/base.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.3.1/src/agt_server/local_games/bos_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.3.1/src/agt_server/local_games/bosii_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.3.1/src/agt_server/local_games/chicken_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    17831 2024-04-02 02:32:20.000000 agt_server-1.3.1/src/agt_server/local_games/lemonade_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)    25787 2024-04-23 03:28:51.000000 agt_server-1.3.1/src/agt_server/local_games/lsvm_arena.py
--rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.3.1/src/agt_server/local_games/rps_arena.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.384249 agt_server-1.3.1/src/agt_server/server/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/server/__init__.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.392252 agt_server-1.3.1/src/agt_server/server/games/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.1/src/agt_server/server/games/__init__.py
--rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.3.1/src/agt_server/server/games/bos_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.3.1/src/agt_server/server/games/bosii_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.3.1/src/agt_server/server/games/chicken_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.3.1/src/agt_server/server/games/complete_2x2_matrix_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.3.1/src/agt_server/server/games/game.py
--rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.3.1/src/agt_server/server/games/lemonade_game.py
--rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.3.1/src/agt_server/server/games/rps_game.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.392547 agt_server-1.3.1/src/agt_server/server/results/
--rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.3.1/src/agt_server/server/results/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.392771 agt_server-1.3.1/src/agt_server/server/results/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.3.1/src/agt_server/server/results/bos/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.392862 agt_server-1.3.1/src/agt_server/server/results/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.3.1/src/agt_server/server/results/bosii/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.392957 agt_server-1.3.1/src/agt_server/server/results/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.3.1/src/agt_server/server/results/chicken/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.393052 agt_server-1.3.1/src/agt_server/server/results/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.3.1/src/agt_server/server/results/lemonade/.gitkeep
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.393146 agt_server-1.3.1/src/agt_server/server/results/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.3.1/src/agt_server/server/results/rps/.gitkeep
--rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.3.1/src/agt_server/server/server.py
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.309593 agt_server-1.3.1/src/agt_server.egg-info/
--rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-04-23 03:31:45.000000 agt_server-1.3.1/src/agt_server.egg-info/PKG-INFO
--rw-r--r--   0 johnwu     (501) staff       (20)    18184 2024-04-23 03:31:45.000000 agt_server-1.3.1/src/agt_server.egg-info/SOURCES.txt
--rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-04-23 03:31:45.000000 agt_server-1.3.1/src/agt_server.egg-info/dependency_links.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       62 2024-04-23 03:31:45.000000 agt_server-1.3.1/src/agt_server.egg-info/requires.txt
--rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-04-23 03:31:45.000000 agt_server-1.3.1/src/agt_server.egg-info/top_level.txt
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.306938 agt_server-1.3.1/test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.307243 agt_server-1.3.1/test/server_test/
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.393660 agt_server-1.3.1/test/server_test/bos/
--rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.3.1/test/server_test/bos/bos_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.3.1/test/server_test/bos/bos_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.394363 agt_server-1.3.1/test/server_test/bosii/
--rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.3.1/test/server_test/bosii/bosii_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.3.1/test/server_test/bosii/bosii_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.395051 agt_server-1.3.1/test/server_test/chicken/
--rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.3.1/test/server_test/chicken/chicken_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.3.1/test/server_test/chicken/chicken_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.396085 agt_server-1.3.1/test/server_test/lemonade/
--rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.3.1/test/server_test/lemonade/lemonade_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.3.1/test/server_test/lemonade/lemonade_ql.sh
--rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.3.1/test/server_test/lemonade/lemonade_test.sh
-drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-23 03:31:45.396680 agt_server-1.3.1/test/server_test/rps/
--rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.3.1/test/server_test/rps/rps_local_test.sh
--rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.3.1/test/server_test/rps/rps_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.890108 agt_server-1.3.2/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3537 2024-01-25 22:07:40.000000 agt_server-1.3.2/.gitignore
+-rw-r--r--   0 johnwu     (501) staff       (20)     1063 2024-01-17 14:08:17.000000 agt_server-1.3.2/LICENSE
+-rw-r--r--   0 johnwu     (501) staff       (20)       66 2024-01-25 21:21:35.000000 agt_server-1.3.2/MANIFEST.in
+-rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-04-24 01:57:30.889878 agt_server-1.3.2/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)     5853 2024-02-06 19:53:48.000000 agt_server-1.3.2/README.md
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.798179 agt_server-1.3.2/data/
+-rw-r--r--   0 johnwu     (501) staff       (20)    80155 2024-01-23 17:19:42.000000 agt_server-1.3.2/data/profile.svg
+-rw-r--r--   0 johnwu     (501) staff       (20)       63 2024-04-21 07:32:05.000000 agt_server-1.3.2/requirements.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       38 2024-04-24 01:57:30.890164 agt_server-1.3.2/setup.cfg
+-rw-r--r--   0 johnwu     (501) staff       (20)     1176 2024-04-24 01:57:20.000000 agt_server-1.3.2/setup.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.798862 agt_server-1.3.2/src/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:10.000000 agt_server-1.3.2/src/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.798955 agt_server-1.3.2/src/agt_server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 21:01:24.000000 agt_server-1.3.2/src/agt_server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.799672 agt_server-1.3.2/src/agt_server/agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.802497 agt_server-1.3.2/src/agt_server/agents/base_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2328 2024-04-24 01:52:33.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1917 2024-02-26 02:01:22.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/bos_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     8115 2024-02-26 02:01:35.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/bosii_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1875 2024-02-26 02:01:43.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/chicken_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     6043 2024-02-10 11:47:44.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/cm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    12345 2024-04-03 16:02:56.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/game_report.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10046 2024-03-31 16:34:04.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/lemonade_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    19752 2024-04-10 02:17:05.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/lsvm_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1969 2024-02-26 02:02:18.000000 agt_server-1.3.2/src/agt_server/agents/base_agents/rps_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.802948 agt_server-1.3.2/src/agt_server/agents/test_agents/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.786844 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.803159 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1636 2024-01-25 21:04:23.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.803549 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1600 2024-01-25 21:04:29.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.803762 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1755 2024-01-25 21:04:34.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.804064 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1996 2024-01-25 21:04:39.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.804352 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2211 2024-01-25 21:04:43.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.804534 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1618 2024-01-25 21:04:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.804730 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1985 2024-01-25 21:04:54.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.804924 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1541 2024-01-25 21:05:00.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.805059 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:05:04.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.805267 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1586 2024-01-25 21:05:08.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.805501 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:05:13.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.805644 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1575 2024-01-25 21:05:17.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.805924 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1591 2024-01-25 21:05:22.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.788358 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.806055 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_compromise/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1679 2024-01-25 21:05:44.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.806348 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_stubborn/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1658 2024-01-25 21:05:47.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.806562 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/anti_punitive/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1813 2024-01-25 21:05:53.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.806841 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/chipping_fish/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3915 2024-01-25 21:05:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.806972 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4518 2024-01-25 21:06:03.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.807254 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     4667 2024-01-25 21:06:09.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.807555 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/fishing_chip/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2054 2024-01-25 21:06:13.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.807854 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/mystery/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3403 2024-01-25 21:06:17.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.808162 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2263 2024-01-30 22:46:02.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.808446 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2993 2024-01-25 21:06:27.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.808694 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1676 2024-01-25 21:06:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.808946 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2041 2024-01-25 21:06:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.809157 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2474 2024-01-25 21:06:40.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.809444 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1604 2024-01-25 21:06:44.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.809696 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1628 2024-01-25 21:06:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.809924 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1649 2024-01-25 21:06:53.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.810569 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1632 2024-01-25 21:06:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.810718 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1693 2024-01-25 21:07:01.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.810867 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1654 2024-01-25 21:07:07.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811011 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811111 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_continue/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1623 2024-01-25 21:09:10.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811244 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_swerve/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1605 2024-01-25 21:09:14.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811637 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/basic_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:09:07.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/basic_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1708 2024-01-25 21:09:18.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811768 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3331 2024-01-25 21:09:23.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.811897 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3252 2024-01-25 21:09:28.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.813088 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-05 15:59:43.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2890 2024-01-25 21:09:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:52.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      160 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-05 15:59:58.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.815356 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:24:35.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3075 2024-01-25 21:09:42.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:45:02.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      192 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:24:35.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.815780 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/mystery_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-08 22:17:17.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/mystery_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1993 2024-01-25 21:09:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.817635 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)       93 2023-06-08 06:30:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/i_fixed_policy.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3219 2024-01-25 21:09:54.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     3809 2024-01-25 21:44:25.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      640 2024-02-15 16:21:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy
+-rw-r--r--   0 johnwu     (501) staff       (20)      309 2023-06-08 06:30:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/uniform_policy.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.817875 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1629 2024-01-25 21:09:59.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.818065 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1564 2024-01-25 21:10:03.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.818364 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1587 2024-01-25 21:10:07.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.818536 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1612 2024-01-25 21:10:11.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.818788 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1648 2024-01-25 21:10:15.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.819039 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1521 2024-01-25 21:10:19.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.819301 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1613 2024-01-25 21:10:25.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.819468 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:41:39.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.819705 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:09.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-02-15 18:47:18.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.820086 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-15 18:47:54.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.820321 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-15 18:48:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.820666 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:15.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-15 18:48:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.820989 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-15 18:49:07.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.821359 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1975 2024-02-15 18:49:21.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.821587 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7288 2024-02-15 18:49:40.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.821914 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/etch_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3073 2024-02-15 18:50:03.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.822162 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/eyes_out/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2418 2024-02-15 18:50:12.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.822368 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/good_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2088 2024-02-15 18:50:23.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.822610 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/hi_bot/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2798 2024-02-15 18:50:37.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.822945 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/increment_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:30:22.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/increment_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1614 2024-02-15 18:50:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.823398 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/jimbus/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2284 2024-02-15 18:51:08.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.823625 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2588 2024-02-15 18:51:19.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.823988 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/q_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3798 2024-02-15 18:51:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.824207 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-02-15 18:51:42.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.824419 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/spinner/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2056 2024-02-15 18:51:51.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.824641 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1485 2024-02-15 18:52:13.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.824889 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1515 2024-02-15 18:52:23.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.825164 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:52:30.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.825816 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-15 18:52:44.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.825975 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1533 2024-02-15 18:52:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.826255 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1531 2024-02-15 18:53:11.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.826620 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/stick_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 22:20:02.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/stick_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-15 18:53:22.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.826843 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/sticky/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2441 2024-02-15 18:53:32.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.827001 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/team_player/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3659 2024-02-15 18:53:44.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.827175 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/zenly/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3045 2024-02-15 18:53:56.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.792635 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.827438 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:10:52.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1583 2024-04-01 18:00:21.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.827720 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2051 2024-02-18 02:11:06.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.827951 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2793 2024-02-18 02:11:20.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.828369 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-18 02:11:25.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1603 2024-02-18 02:11:25.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.828608 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1910 2024-02-22 06:12:46.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.828857 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1522 2024-02-22 06:07:27.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.829169 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1571 2024-02-22 06:12:45.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.829437 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:39:15.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.830087 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:54.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:01.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1258 2024-04-02 19:33:38.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.830694 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:42:59.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      191 2024-04-02 21:45:42.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1259 2024-04-02 19:34:13.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.831270 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:05.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:45:45.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1277 2024-04-02 19:34:47.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.831821 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:10.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      187 2024-04-02 21:41:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1275 2024-04-02 18:08:23.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.832533 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:16.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      202 2024-04-02 21:46:00.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1292 2024-04-02 19:36:57.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.833389 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-04-02 19:43:22.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      188 2024-04-02 21:46:05.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/agent_submission.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1293 2024-04-02 19:37:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.833718 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.833819 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/exponential/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2954 2024-01-26 06:19:46.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/exponential/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.834092 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ficticious_play/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3052 2024-01-26 05:13:48.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.834356 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/random_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1549 2024-01-25 21:15:25.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.834609 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/rock_lover/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:32.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.834925 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_move/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1506 2024-01-25 21:15:38.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.835262 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_type/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1525 2024-01-25 21:15:43.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.837187 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_delay/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1543 2024-01-25 21:16:13.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.837591 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_disconnect/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1554 2024-01-25 21:16:18.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.837807 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_flood/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1444 2024-01-25 22:02:30.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.838050 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_math_err/
+-rw-r--r--   0 johnwu     (501) staff       (20)     1527 2024-01-25 21:16:28.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.838474 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ta_agent/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 22:14:36.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ta_agent/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     1454 2024-01-25 21:16:33.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      662 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/agents/test_agents/stress_test.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.794293 agt_server-1.3.2/src/agt_server/configs/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.840080 agt_server-1.3.2/src/agt_server/configs/handin_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:28:03.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      223 2024-02-22 04:27:55.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      231 2024-02-22 04:27:45.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      263 2024-03-02 19:44:48.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      294 2024-04-02 18:15:54.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-22 04:27:36.000000 agt_server-1.3.2/src/agt_server/configs/handin_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842045 agt_server-1.3.2/src/agt_server/configs/server_configs/
+-rw-r--r--   0 johnwu     (501) staff       (20)      603 2024-02-01 23:47:38.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/bos_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      797 2024-02-06 00:46:41.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/bosii_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      608 2024-02-15 16:14:51.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/chicken_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      621 2024-01-30 21:38:03.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/lemonade_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      623 2024-03-31 16:36:02.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/lsvm_config.json
+-rw-r--r--   0 johnwu     (501) staff       (20)      604 2024-01-30 21:37:55.000000 agt_server-1.3.2/src/agt_server/configs/server_configs/rps_config.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842228 agt_server-1.3.2/src/agt_server/handin/
+-rw-r--r--   0 johnwu     (501) staff       (20)     3656 2024-04-03 02:38:28.000000 agt_server-1.3.2/src/agt_server/handin/handin.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842482 agt_server-1.3.2/src/agt_server/handin/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:56.000000 agt_server-1.3.2/src/agt_server/handin/results/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842586 agt_server-1.3.2/src/agt_server/handin/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:30:49.000000 agt_server-1.3.2/src/agt_server/handin/results/bos/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842696 agt_server-1.3.2/src/agt_server/handin/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:04.000000 agt_server-1.3.2/src/agt_server/handin/results/bosii/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.842795 agt_server-1.3.2/src/agt_server/handin/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:25.000000 agt_server-1.3.2/src/agt_server/handin/results/chicken/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.872825 agt_server-1.3.2/src/agt_server/handin/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)     2786 2024-02-22 23:10:32.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3094 2024-02-23 00:23:34.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3249 2024-02-26 03:46:11.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:12:09.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:13:49.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:14:53.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:21:10.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:23:39.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:25:31.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:26:34.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:27:17.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1737 2024-02-26 04:27:28.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1673 2024-02-26 04:27:55.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:28:23.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:31:07.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2642 2024-02-26 04:32:45.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2297 2024-02-26 04:33:29.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2631 2024-02-26 04:34:38.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2866 2024-02-26 04:55:11.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2759 2024-02-26 06:39:27.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-26 06:49:59.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2674 2024-02-26 06:59:09.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9873 2024-02-26 23:17:30.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      526 2024-02-26 23:18:48.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2722 2024-02-26 23:36:33.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2784 2024-02-26 23:37:56.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2494 2024-02-26 23:38:30.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      219 2024-02-26 23:45:11.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:24.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:28.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-28_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:45:31.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-45-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:46:21.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3054 2024-02-26 23:47:10.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      183 2024-02-26 23:47:41.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-47-41_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      215 2024-02-26 23:50:39.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-50-38_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-26 23:58:51.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-58-51_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3014 2024-02-27 00:09:44.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:09:46.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2416 2024-02-27 00:13:56.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     2610 2024-02-27 00:14:32.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:19:21.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-19-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)      179 2024-02-27 00:21:53.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-21-53_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4940 2024-02-27 20:26:21.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3215 2024-02-27 20:27:18.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7406 2024-02-27 20:32:27.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3367 2024-02-27 20:33:47.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     7165 2024-02-27 20:36:53.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6897 2024-02-27 20:40:29.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5795 2024-02-27 20:40:37.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6689 2024-02-27 20:49:05.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    69971 2024-02-28 04:53:17.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    42190 2024-02-28 08:28:23.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38084 2024-02-28 10:04:34.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    38027 2024-02-28 11:31:24.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5240 2024-02-28 11:34:41.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     1921 2024-02-28 11:35:40.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8899 2024-02-28 11:42:21.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    39034 2024-02-28 14:22:14.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    74776 2024-02-28 19:14:37.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5920 2024-02-28 21:11:22.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5102 2024-02-28 21:13:24.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     4669 2024-02-28 21:16:32.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5107 2024-02-28 21:19:34.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    16781 2024-02-28 21:40:00.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15945 2024-02-28 21:51:18.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    17789 2024-02-28 22:18:47.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    15831 2024-02-28 22:55:20.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3939 2024-03-01 00:34:13.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    14259 2024-03-01 00:45:25.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3812 2024-03-01 00:46:34.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3998 2024-03-01 00:48:27.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     6081 2024-03-01 01:51:10.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     9474 2024-03-01 01:52:08.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     8767 2024-03-01 01:52:36.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     5900 2024-03-01 01:54:12.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    12641 2024-03-01 02:00:54.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    33503 2024-03-01 03:09:35.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    31050 2024-03-01 05:10:15.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18142 2024-03-01 05:31:08.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    18785 2024-03-01 06:24:52.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)    19642 2024-03-01 07:22:31.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3325 2024-03-01 07:22:31.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/LemonadeArena.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)     3900 2024-02-26 04:14:53.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/LemonadeTest.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)   785905 2024-03-01 23:54:21.000000 agt_server-1.3.2/src/agt_server/handin/results/lemonade/shortcut.json
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.875057 agt_server-1.3.2/src/agt_server/handin/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-02-15 16:31:14.000000 agt_server-1.3.2/src/agt_server/handin/results/rps/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.881890 agt_server-1.3.2/src/agt_server/local_games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/local_games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     2334 2024-04-17 23:51:57.000000 agt_server-1.3.2/src/agt_server/local_games/base.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9604 2024-02-15 18:16:30.000000 agt_server-1.3.2/src/agt_server/local_games/bos_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    10213 2024-02-15 18:16:15.000000 agt_server-1.3.2/src/agt_server/local_games/bosii_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9731 2024-02-15 18:17:49.000000 agt_server-1.3.2/src/agt_server/local_games/chicken_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    17831 2024-04-02 02:32:20.000000 agt_server-1.3.2/src/agt_server/local_games/lemonade_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    26125 2024-04-24 01:55:31.000000 agt_server-1.3.2/src/agt_server/local_games/lsvm_arena.py
+-rw-r--r--   0 johnwu     (501) staff       (20)     9703 2024-02-15 18:17:04.000000 agt_server-1.3.2/src/agt_server/local_games/rps_arena.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.882251 agt_server-1.3.2/src/agt_server/server/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/server/__init__.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.884580 agt_server-1.3.2/src/agt_server/server/games/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2023-05-31 04:43:31.000000 agt_server-1.3.2/src/agt_server/server/games/__init__.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      596 2024-01-31 02:48:39.000000 agt_server-1.3.2/src/agt_server/server/games/bos_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    18510 2024-01-30 21:30:44.000000 agt_server-1.3.2/src/agt_server/server/games/bosii_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      606 2024-01-25 21:17:28.000000 agt_server-1.3.2/src/agt_server/server/games/chicken_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    16908 2024-01-30 21:34:09.000000 agt_server-1.3.2/src/agt_server/server/games/complete_2x2_matrix_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      710 2024-01-23 13:08:08.000000 agt_server-1.3.2/src/agt_server/server/games/game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)    19180 2024-01-30 21:32:26.000000 agt_server-1.3.2/src/agt_server/server/games/lemonade_game.py
+-rw-r--r--   0 johnwu     (501) staff       (20)      671 2024-01-25 21:17:39.000000 agt_server-1.3.2/src/agt_server/server/games/rps_game.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.884869 agt_server-1.3.2/src/agt_server/server/results/
+-rw-r--r--   0 johnwu     (501) staff       (20)       18 2024-01-25 18:51:20.000000 agt_server-1.3.2/src/agt_server/server/results/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.885205 agt_server-1.3.2/src/agt_server/server/results/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:35.000000 agt_server-1.3.2/src/agt_server/server/results/bos/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.885307 agt_server-1.3.2/src/agt_server/server/results/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:39.000000 agt_server-1.3.2/src/agt_server/server/results/bosii/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.885402 agt_server-1.3.2/src/agt_server/server/results/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:43.000000 agt_server-1.3.2/src/agt_server/server/results/chicken/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.885501 agt_server-1.3.2/src/agt_server/server/results/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:49.000000 agt_server-1.3.2/src/agt_server/server/results/lemonade/.gitkeep
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.885602 agt_server-1.3.2/src/agt_server/server/results/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)        0 2024-01-25 18:52:54.000000 agt_server-1.3.2/src/agt_server/server/results/rps/.gitkeep
+-rw-r--r--   0 johnwu     (501) staff       (20)    23118 2024-02-15 16:20:24.000000 agt_server-1.3.2/src/agt_server/server/server.py
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.799558 agt_server-1.3.2/src/agt_server.egg-info/
+-rw-r--r--   0 johnwu     (501) staff       (20)     6650 2024-04-24 01:57:30.000000 agt_server-1.3.2/src/agt_server.egg-info/PKG-INFO
+-rw-r--r--   0 johnwu     (501) staff       (20)    18184 2024-04-24 01:57:30.000000 agt_server-1.3.2/src/agt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)        1 2024-04-24 01:57:30.000000 agt_server-1.3.2/src/agt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       62 2024-04-24 01:57:30.000000 agt_server-1.3.2/src/agt_server.egg-info/requires.txt
+-rw-r--r--   0 johnwu     (501) staff       (20)       11 2024-04-24 01:57:30.000000 agt_server-1.3.2/src/agt_server.egg-info/top_level.txt
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.795640 agt_server-1.3.2/test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.795970 agt_server-1.3.2/test/server_test/
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.886107 agt_server-1.3.2/test/server_test/bos/
+-rw-r--r--   0 johnwu     (501) staff       (20)     7014 2024-01-25 21:24:06.000000 agt_server-1.3.2/test/server_test/bos/bos_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8015 2024-01-25 21:22:03.000000 agt_server-1.3.2/test/server_test/bos/bos_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.886756 agt_server-1.3.2/test/server_test/bosii/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10139 2024-01-25 21:26:19.000000 agt_server-1.3.2/test/server_test/bosii/bosii_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11361 2024-01-25 21:28:31.000000 agt_server-1.3.2/test/server_test/bosii/bosii_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.887551 agt_server-1.3.2/test/server_test/chicken/
+-rw-r--r--   0 johnwu     (501) staff       (20)    10276 2024-01-25 21:35:28.000000 agt_server-1.3.2/test/server_test/chicken/chicken_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    11631 2024-01-25 21:50:35.000000 agt_server-1.3.2/test/server_test/chicken/chicken_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.888643 agt_server-1.3.2/test/server_test/lemonade/
+-rw-r--r--   0 johnwu     (501) staff       (20)    13981 2024-01-25 21:53:38.000000 agt_server-1.3.2/test/server_test/lemonade/lemonade_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     8108 2024-01-25 21:56:56.000000 agt_server-1.3.2/test/server_test/lemonade/lemonade_ql.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)    16031 2024-01-25 21:58:30.000000 agt_server-1.3.2/test/server_test/lemonade/lemonade_test.sh
+drwxr-xr-x   0 johnwu     (501) staff       (20)        0 2024-04-24 01:57:30.889289 agt_server-1.3.2/test/server_test/rps/
+-rw-r--r--   0 johnwu     (501) staff       (20)     5940 2024-01-25 22:00:19.000000 agt_server-1.3.2/test/server_test/rps/rps_local_test.sh
+-rw-r--r--   0 johnwu     (501) staff       (20)     6884 2024-01-25 22:00:40.000000 agt_server-1.3.2/test/server_test/rps/rps_test.sh
```

### Comparing `agt_server-1.3.1/.gitignore` & `agt_server-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/LICENSE` & `agt_server-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/PKG-INFO` & `agt_server-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt_server
-Version: 1.3.1
+Version: 1.3.2
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.3.1/README.md` & `agt_server-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/data/profile.svg` & `agt_server-1.3.2/data/profile.svg`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/setup.py` & `agt_server-1.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='agt_server', 
-    version='1.3.1',
+    version='1.3.2',
     author='John Wu', 
     author_email='john_w_wu@brown.edu', 
     description='The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.',  # Provide a short description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/brown-agt/agt-server-remastered',  
     project_urls={
```

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/agent.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 
     def setup(self):
         raise NotImplementedError
 
     def restart(self):
         self.game_report = GameReport()
         self.setup()
+    
+    def teardown(self): 
+        # TODO: While the active competition is running we can't have this raising an Error but have it raise an error afterwards to be more robust 
+        pass
 
     def get_device_id(self):
         return uuid.UUID(int=uuid.getnode()).hex[-12:]
 
     def connect(self, ip='localhost', port=1234):
         self.client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client.connect((ip, port))
```

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/bos_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/bos_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/bosii_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/bosii_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/chicken_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/chicken_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/cm_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/cm_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/game_report.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/game_report.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/lemonade_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/lemonade_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/lsvm_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/lsvm_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/base_agents/rps_agent.py` & `agt_server-1.3.2/src/agt_server/agents/base_agents/rps_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bos/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_compromise/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/always_stubborn/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/anti_punitive/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/chipping_fish/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/fishing_chip/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/mystery/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/punitive_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/reluctant_mood_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/bosii/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_continue/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/always_swerve/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/basic_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lastmove_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/lookback_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/mystery_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/q_learning.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/ql_chicken/qtable_static.npy`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/chicken/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/dumb_chicken/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/end_to_end_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/etch_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/eyes_out/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/good_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/hi_bot/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/increment_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/jimbus/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/kamen_rider/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/q_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/spinner/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/stick_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/sticky/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/team_player/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade/zenly/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/always_stay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/best_respond_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/circular_hotel/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/decrement_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/del_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lemonade_small/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder/jump_bidder.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/jump_bidder 2/jump_bidder.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/min_bidder 2/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/lsvm/truthful_bidder 2/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/exponential/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/exponential/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ficticious_play/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/random_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/rock_lover/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_move/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_bad_type/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_delay/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_disconnect/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_flood/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/st_math_err/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py` & `agt_server-1.3.2/src/agt_server/agents/test_agents/rps/ta_agent/my_agent.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/agents/test_agents/stress_test.txt` & `agt_server-1.3.2/src/agt_server/agents/test_agents/stress_test.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/bos_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/bos_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/bosii_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/bosii_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/chicken_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/chicken_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/lemonade_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/lemonade_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/lsvm_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/lsvm_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/configs/server_configs/rps_config.json` & `agt_server-1.3.2/src/agt_server/configs/server_configs/rps_config.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/handin.py` & `agt_server-1.3.2/src/agt_server/handin/handin.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-22_18-10-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-22_19-23-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_22-46-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-11-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-13-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-14-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-20-41_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-23-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-25-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-26-48_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-27-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-30-39_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-32-17_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-33-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-34-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-25_23-54-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-39-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-49-58_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_01-59-01_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-17-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-18-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-36-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-37-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-38-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_18-46-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-09-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-13-54_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-26_19-14-30_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-26-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-27-14_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-29-42_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-33-08_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-35-25_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-37-31_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-40-33_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_15-48-49_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-27_16-18-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_00-03-46_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_03-34-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_05-05-22_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-33-35_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-35-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-36-11_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_06-50-43_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_09-22-32_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-09-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-12-05_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-15-09_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-18-26_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-26-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-41-36_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_16-53-47_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-28_17-26-15_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-33-57_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-35-13_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-46-29_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_19-48-21_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-03_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-51-52_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-24_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-52-55_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_20-54-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_21-02-04_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-02-29_22-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_00-10-45_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_01-02-27_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/2024-03-01_01-48-16_log.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/LemonadeArena.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/LemonadeArena.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/LemonadeTest.txt` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/LemonadeTest.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/handin/results/lemonade/shortcut.json` & `agt_server-1.3.2/src/agt_server/handin/results/lemonade/shortcut.json`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/base.py` & `agt_server-1.3.2/src/agt_server/local_games/base.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/bos_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/bos_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/bosii_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/bosii_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/chicken_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/chicken_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/lemonade_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/lemonade_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/local_games/lsvm_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/lsvm_arena.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,23 +138,21 @@
                     rating_diffs[name] = abs(self.game_reports[name]['elo'].event_history[-1].mu - target_rating)
                 else: 
                     rating_diffs[name] = 1600 - target_rating
         
         closest_matches = sorted(rating_diffs, key=rating_diffs.get)[:5]
         return set(closest_matches)
     
-    # TODO: Run some tests to figure out file loading time locally
+    
     # TODO: Add support for a setup and teardown to reduce overhead of opening and closing files 
     # TODO: Write Autograder tests for gradescope
-    # TODO: Connect the Code with gradescope and then cron it. 
-    # TODO: pip install common packages like gym, tensorflow, pytorch, etc...
-    # TODO: Draft up an announcement for friendly competition being up for spectrum
     # TODO: Connect the code with google drive to uplink the files to a shared drive with the students. 
     # TODO: Add a pygame visualizer for the actual games themselves
     
+    
     def run(self):
         """
         Simulates an LSVM auction with all of the players in self.players. 
         For each player, they are matched with the 5 other players closest in ELO to that player, 
         Then for the number of cycles each player plays, each player will cycle through being the national bidder once in a match 
         In each match the other regional bidders will be assigned one of the regional goods uniform at random. 
         Note that the regional bidders can be assigned the same regional good. 
@@ -192,14 +190,25 @@
                                         self.game_reports[p.name]['disconnected'] = True
                                         continue
                             try:
                                 self.run_game(curr_players)
                             except:
                                 self.reset_game_reports()
                                 continue
+                            
+                            for p in curr_players: 
+                                if p is None or self.game_reports[p.name]['disconnected']: 
+                                    continue 
+                                else: 
+                                    try:
+                                        self.run_func_w_time(
+                                            p.teardown, self.timeout, p.name)
+                                    except:
+                                        self.game_reports[p.name]['disconnected'] = True
+                                        continue
                         else: 
                             for p in curr_players: 
                                 self.run_func_w_time(p.restart, self.timeout, p.name)
                             self.run_game(curr_players)
         results = self.summarize_results()
         return results
```

### Comparing `agt_server-1.3.1/src/agt_server/local_games/rps_arena.py` & `agt_server-1.3.2/src/agt_server/local_games/rps_arena.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/bos_game.py` & `agt_server-1.3.2/src/agt_server/server/games/bos_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/bosii_game.py` & `agt_server-1.3.2/src/agt_server/server/games/bosii_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/chicken_game.py` & `agt_server-1.3.2/src/agt_server/server/games/chicken_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/complete_2x2_matrix_game.py` & `agt_server-1.3.2/src/agt_server/server/games/complete_2x2_matrix_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/game.py` & `agt_server-1.3.2/src/agt_server/server/games/game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/lemonade_game.py` & `agt_server-1.3.2/src/agt_server/server/games/lemonade_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/games/rps_game.py` & `agt_server-1.3.2/src/agt_server/server/games/rps_game.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server/server/server.py` & `agt_server-1.3.2/src/agt_server/server/server.py`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/src/agt_server.egg-info/PKG-INFO` & `agt_server-1.3.2/src/agt_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agt-server
-Version: 1.3.1
+Version: 1.3.2
 Summary: The AGT Server is a python platform designed to run and implement game environments that autonomous agents can connect to and compete in.
 Home-page: https://github.com/brown-agt/agt-server-remastered
 Author: John Wu
 Author-email: john_w_wu@brown.edu
 Project-URL: Bug Tracker, https://github.com/brown-agt/agt-server-remastered/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agt_server-1.3.1/src/agt_server.egg-info/SOURCES.txt` & `agt_server-1.3.2/src/agt_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/bos/bos_local_test.sh` & `agt_server-1.3.2/test/server_test/bos/bos_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/bos/bos_test.sh` & `agt_server-1.3.2/test/server_test/bos/bos_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/bosii/bosii_local_test.sh` & `agt_server-1.3.2/test/server_test/bosii/bosii_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/bosii/bosii_test.sh` & `agt_server-1.3.2/test/server_test/bosii/bosii_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/chicken/chicken_local_test.sh` & `agt_server-1.3.2/test/server_test/chicken/chicken_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/chicken/chicken_test.sh` & `agt_server-1.3.2/test/server_test/chicken/chicken_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/lemonade/lemonade_local_test.sh` & `agt_server-1.3.2/test/server_test/lemonade/lemonade_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/lemonade/lemonade_ql.sh` & `agt_server-1.3.2/test/server_test/lemonade/lemonade_ql.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/lemonade/lemonade_test.sh` & `agt_server-1.3.2/test/server_test/lemonade/lemonade_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/rps/rps_local_test.sh` & `agt_server-1.3.2/test/server_test/rps/rps_local_test.sh`

 * *Files identical despite different names*

### Comparing `agt_server-1.3.1/test/server_test/rps/rps_test.sh` & `agt_server-1.3.2/test/server_test/rps/rps_test.sh`

 * *Files identical despite different names*

