# Comparing `tmp/onionprobe-1.1.2.tar.gz` & `tmp/onionprobe-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onionprobe-1.1.2.tar", last modified: Thu Sep 28 21:19:45 2023, max compression
+gzip compressed data, was "onionprobe-1.2.0.tar", last modified: Wed Apr 24 18:00:03 2024, max compression
```

## Comparing `onionprobe-1.1.2.tar` & `onionprobe-1.2.0.tar`

### file list

```diff
@@ -1,141 +1,149 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.659142 onionprobe-1.1.2/
--rw-r--r--   0 user      (1000) user      (1000)        5 2022-05-23 21:15:17.000000 onionprobe-1.1.2/.dockerignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.251136 onionprobe-1.1.2/.github/
--rw-r--r--   0 user      (1000) user      (1000)     1421 2023-03-13 15:44:25.000000 onionprobe-1.1.2/.github/gh-pages.yml
--rw-r--r--   0 user      (1000) user      (1000)       71 2023-03-13 16:08:31.000000 onionprobe-1.1.2/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      311 2023-03-31 12:57:14.000000 onionprobe-1.1.2/.gitlab-ci-pages.yml
--rw-r--r--   0 user      (1000) user      (1000)      407 2023-04-10 18:53:38.000000 onionprobe-1.1.2/.gitlab-ci-slides.yml
--rw-r--r--   0 user      (1000) user      (1000)     1453 2023-03-31 12:52:40.000000 onionprobe-1.1.2/.gitlab-ci.yml
--rw-r--r--   0 user      (1000) user      (1000)      248 2023-03-13 20:47:53.000000 onionprobe-1.1.2/.gitmodules
--rw-r--r--   0 user      (1000) user      (1000)     5489 2022-03-11 13:55:54.000000 onionprobe-1.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 user      (1000) user      (1000)    14791 2023-09-28 21:18:16.000000 onionprobe-1.1.2/ChangeLog.md
--rw-r--r--   0 user      (1000) user      (1000)    35147 2022-03-11 13:55:54.000000 onionprobe-1.1.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     2132 2023-04-04 13:06:41.000000 onionprobe-1.1.2/Makefile
--rw-r--r--   0 user      (1000) user      (1000)     1962 2023-09-28 21:19:45.655141 onionprobe-1.1.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      665 2023-04-03 19:30:39.000000 onionprobe-1.1.2/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.323136 onionprobe-1.1.2/configs/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.339136 onionprobe-1.1.2/configs/alertmanager/
--rw-r--r--   0 user      (1000) user      (1000)     2353 2022-05-24 00:13:45.000000 onionprobe-1.1.2/configs/alertmanager/alertmanager.yml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.359136 onionprobe-1.1.2/configs/apt/
--rw-r--r--   0 user      (1000) user      (1000)      955 2023-04-03 17:31:42.000000 onionprobe-1.1.2/configs/apt/tor.list
--rw-r--r--   0 user      (1000) user      (1000)     3385 2022-05-31 16:54:40.000000 onionprobe-1.1.2/configs/env.sample
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.375136 onionprobe-1.1.2/configs/grafana/
--rw-r--r--   0 user      (1000) user      (1000)    13001 2023-04-04 12:22:17.000000 onionprobe-1.1.2/configs/grafana/home.json
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.059135 onionprobe-1.1.2/configs/grafana/provisioning/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.395136 onionprobe-1.1.2/configs/grafana/provisioning/dashboards/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:22.000000 onionprobe-1.1.2/configs/grafana/provisioning/dashboards/.gitignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.423137 onionprobe-1.1.2/configs/grafana/provisioning/datasources/
--rw-r--r--   0 user      (1000) user      (1000)      719 2022-05-23 13:08:40.000000 onionprobe-1.1.2/configs/grafana/provisioning/datasources/prometheus.yml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.447137 onionprobe-1.1.2/configs/grafana/provisioning/notifiers/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:59.000000 onionprobe-1.1.2/configs/grafana/provisioning/notifiers/.gitignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.471137 onionprobe-1.1.2/configs/grafana/provisioning/plugins/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:49.000000 onionprobe-1.1.2/configs/grafana/provisioning/plugins/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      305 2022-05-11 17:39:06.000000 onionprobe-1.1.2/configs/onionprobe.yaml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.511137 onionprobe-1.1.2/configs/prometheus/
--rw-r--r--   0 user      (1000) user      (1000)     1855 2023-06-22 17:05:27.000000 onionprobe-1.1.2/configs/prometheus/prometheus-rules.yml
--rw-r--r--   0 user      (1000) user      (1000)     1439 2023-03-30 18:22:38.000000 onionprobe-1.1.2/configs/prometheus/prometheus.yml
--rw-r--r--   0 user      (1000) user      (1000)    32781 2023-03-30 19:44:46.000000 onionprobe-1.1.2/configs/real-world-onion-sites.yaml
--rw-r--r--   0 user      (1000) user      (1000)     7507 2023-03-30 19:44:54.000000 onionprobe-1.1.2/configs/securedrop.yaml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.527137 onionprobe-1.1.2/configs/systemd/
--rw-r--r--   0 user      (1000) user      (1000)     1431 2022-05-25 18:31:42.000000 onionprobe-1.1.2/configs/systemd/onionprobe-monitor.service
--rw-r--r--   0 user      (1000) user      (1000)     2086 2023-03-30 18:40:33.000000 onionprobe-1.1.2/configs/test.yaml
--rw-r--r--   0 user      (1000) user      (1000)    19376 2023-03-30 18:38:42.000000 onionprobe-1.1.2/configs/tor.yaml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.071135 onionprobe-1.1.2/containers/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.571137 onionprobe-1.1.2/containers/onionprobe/
--rw-r--r--   0 user      (1000) user      (1000)     1839 2023-04-03 17:31:45.000000 onionprobe-1.1.2/containers/onionprobe/Dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     2097 2022-06-23 10:54:02.000000 onionprobe-1.1.2/containers/onionprobe/Dockerfile.pip
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.611137 onionprobe-1.1.2/containers/tor/
--rw-r--r--   0 user      (1000) user      (1000)     1775 2023-04-03 17:31:38.000000 onionprobe-1.1.2/containers/tor/Dockerfile
--rw-r--r--   0 user      (1000) user      (1000)     1999 2022-05-23 23:46:59.000000 onionprobe-1.1.2/containers/tor/torrc
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.623138 onionprobe-1.1.2/contrib/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 13:08:40.000000 onionprobe-1.1.2/contrib/.gitignore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.795138 onionprobe-1.1.2/debian/
--rw-r--r--   0 user      (1000) user      (1000)     1180 2022-04-19 18:24:30.000000 onionprobe-1.1.2/debian/README.Debian
--rw-r--r--   0 user      (1000) user      (1000)     1629 2023-09-28 21:11:24.000000 onionprobe-1.1.2/debian/changelog
--rw-r--r--   0 user      (1000) user      (1000)      940 2023-04-03 18:18:40.000000 onionprobe-1.1.2/debian/control
--rw-r--r--   0 user      (1000) user      (1000)     1115 2022-04-13 16:18:45.000000 onionprobe-1.1.2/debian/copyright
--rw-r--r--   0 user      (1000) user      (1000)       52 2022-04-13 16:18:45.000000 onionprobe-1.1.2/debian/gbp.conf
--rw-r--r--   0 user      (1000) user      (1000)       22 2022-04-13 16:18:45.000000 onionprobe-1.1.2/debian/manpages
--rw-r--r--   0 user      (1000) user      (1000)      319 2022-04-19 18:24:30.000000 onionprobe-1.1.2/debian/onionprobe.default
--rw-r--r--   0 user      (1000) user      (1000)       10 2022-04-13 16:18:45.000000 onionprobe-1.1.2/debian/onionprobe.docs
--rw-r--r--   0 user      (1000) user      (1000)     1897 2022-04-19 18:24:30.000000 onionprobe-1.1.2/debian/onionprobe.init
--rw-r--r--   0 user      (1000) user      (1000)      161 2022-05-10 21:12:42.000000 onionprobe-1.1.2/debian/onionprobe.install
--rw-r--r--   0 user      (1000) user      (1000)     1150 2022-04-19 19:46:54.000000 onionprobe-1.1.2/debian/onionprobe.service
--rw-r--r--   0 user      (1000) user      (1000)      550 2022-05-11 16:14:16.000000 onionprobe-1.1.2/debian/postinst
--rw-r--r--   0 user      (1000) user      (1000)      517 2022-05-11 16:14:16.000000 onionprobe-1.1.2/debian/postrm
--rwxr-xr-x   0 user      (1000) user      (1000)      664 2023-03-31 13:26:19.000000 onionprobe-1.1.2/debian/rules
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.807138 onionprobe-1.1.2/debian/source/
--rw-r--r--   0 user      (1000) user      (1000)       13 2022-04-13 16:18:45.000000 onionprobe-1.1.2/debian/source/format
--rw-r--r--   0 user      (1000) user      (1000)     6015 2023-04-04 12:45:16.000000 onionprobe-1.1.2/docker-compose.yaml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.979139 onionprobe-1.1.2/docs/
--rw-r--r--   0 user      (1000) user      (1000)      275 2022-03-23 13:59:34.000000 onionprobe-1.1.2/docs/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      289 2023-04-10 19:09:06.000000 onionprobe-1.1.2/docs/.pages
--rw-r--r--   0 user      (1000) user      (1000)      688 2023-03-31 13:44:09.000000 onionprobe-1.1.2/docs/README.md
--rw-r--r--   0 user      (1000) user      (1000)      199 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/acknowledgements.md
--rw-r--r--   0 user      (1000) user      (1000)      903 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/alternatives.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.043139 onionprobe-1.1.2/docs/api/
--rw-r--r--   0 user      (1000) user      (1000)       52 2023-03-13 23:41:14.000000 onionprobe-1.1.2/docs/api/.pages
--rw-r--r--   0 user      (1000) user      (1000)      824 2023-03-14 10:59:30.000000 onionprobe-1.1.2/docs/api/README.md
--rw-r--r--   0 user      (1000) user      (1000)      467 2023-03-13 23:55:53.000000 onionprobe-1.1.2/docs/api/helpers.md
--rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-13 23:56:08.000000 onionprobe-1.1.2/docs/api/onionprobe.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.079139 onionprobe-1.1.2/docs/assets/
--rw-r--r--   0 user      (1000) user      (1000)   156452 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/assets/dashboard.png
--rw-r--r--   0 user      (1000) user      (1000)    47138 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/assets/logo.jpg
--rw-r--r--   0 user      (1000) user      (1000)     1496 2023-03-13 18:15:27.000000 onionprobe-1.1.2/docs/configurations.md
--rw-r--r--   0 user      (1000) user      (1000)      671 2023-03-13 18:27:36.000000 onionprobe-1.1.2/docs/installation.md
--rw-r--r--   0 user      (1000) user      (1000)      448 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/issues.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.119140 onionprobe-1.1.2/docs/man/
--rw-r--r--   0 user      (1000) user      (1000)    35563 2023-09-28 21:11:57.000000 onionprobe-1.1.2/docs/man/onionprobe.1.md
--rw-r--r--   0 user      (1000) user      (1000)     1299 2023-03-31 13:05:21.000000 onionprobe-1.1.2/docs/man/onionprobe.1.md.tmpl
--rw-r--r--   0 user      (1000) user      (1000)     1022 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/references.md
--rw-r--r--   0 user      (1000) user      (1000)      687 2023-03-13 15:44:25.000000 onionprobe-1.1.2/docs/requirements.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.139140 onionprobe-1.1.2/docs/slides/
--rw-r--r--   0 user      (1000) user      (1000)      708 2023-03-14 11:29:44.000000 onionprobe-1.1.2/docs/slides/Makefile
--rw-r--r--   0 user      (1000) user      (1000)     8302 2023-03-30 18:40:34.000000 onionprobe-1.1.2/docs/standalone.md
--rw-r--r--   0 user      (1000) user      (1000)      626 2023-03-13 15:59:26.000000 onionprobe-1.1.2/docs/structure.md
--rw-r--r--   0 user      (1000) user      (1000)     2083 2023-04-03 22:35:35.000000 onionprobe-1.1.2/docs/upgrading.md
--rw-r--r--   0 user      (1000) user      (1000)      774 2023-03-15 11:27:48.000000 onionprobe-1.1.2/docs/usage.md
--rw-r--r--   0 user      (1000) user      (1000)     9233 2022-05-23 21:37:50.000000 onionprobe-1.1.2/kvmxfile
--rw-r--r--   0 user      (1000) user      (1000)     1903 2023-06-22 12:14:28.000000 onionprobe-1.1.2/mkdocs.yml
--rwxr-xr-x   0 user      (1000) user      (1000)      900 2022-04-09 16:32:21.000000 onionprobe-1.1.2/onionprobe
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.187140 onionprobe-1.1.2/packages/
--rwxr-xr-x   0 user      (1000) user      (1000)     2703 2022-05-11 16:38:07.000000 onionprobe-1.1.2/packages/manpage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.443141 onionprobe-1.1.2/packages/onionprobe/
--rw-r--r--   0 user      (1000) user      (1000)       58 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     3491 2023-03-21 14:39:42.000000 onionprobe-1.1.2/packages/onionprobe/app.py
--rw-r--r--   0 user      (1000) user      (1000)    10281 2023-03-21 14:39:42.000000 onionprobe-1.1.2/packages/onionprobe/certificate.py
--rw-r--r--   0 user      (1000) user      (1000)    19480 2023-09-28 21:09:44.000000 onionprobe-1.1.2/packages/onionprobe/config.py
--rw-r--r--   0 user      (1000) user      (1000)     7186 2023-05-11 21:56:25.000000 onionprobe-1.1.2/packages/onionprobe/descriptor.py
--rw-r--r--   0 user      (1000) user      (1000)     8460 2023-03-21 14:39:42.000000 onionprobe-1.1.2/packages/onionprobe/http.py
--rw-r--r--   0 user      (1000) user      (1000)     4980 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/init.py
--rw-r--r--   0 user      (1000) user      (1000)     2383 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/logger.py
--rw-r--r--   0 user      (1000) user      (1000)     2870 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/main.py
--rw-r--r--   0 user      (1000) user      (1000)    20564 2023-04-03 17:00:23.000000 onionprobe-1.1.2/packages/onionprobe/metrics.py
--rw-r--r--   0 user      (1000) user      (1000)     5509 2023-03-21 14:39:42.000000 onionprobe-1.1.2/packages/onionprobe/prober.py
--rw-r--r--   0 user      (1000) user      (1000)     1313 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/teardown.py
--rw-r--r--   0 user      (1000) user      (1000)     2527 2023-03-21 12:02:25.000000 onionprobe-1.1.2/packages/onionprobe/time.py
--rw-r--r--   0 user      (1000) user      (1000)    10312 2023-04-03 17:20:38.000000 onionprobe-1.1.2/packages/onionprobe/tls.py
--rw-r--r--   0 user      (1000) user      (1000)     8772 2023-09-28 21:07:17.000000 onionprobe-1.1.2/packages/onionprobe/tor.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.539141 onionprobe-1.1.2/packages/onionprobe.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1962 2023-09-28 21:19:43.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2729 2023-09-28 21:19:44.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-09-28 21:19:43.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       63 2023-09-28 21:19:43.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      102 2023-09-28 21:19:43.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2023-09-28 21:19:43.000000 onionprobe-1.1.2/packages/onionprobe.egg-info/top_level.txt
--rwxr-xr-x   0 user      (1000) user      (1000)     4201 2022-06-23 13:11:34.000000 onionprobe-1.1.2/packages/real-world-onion-sites.py
--rwxr-xr-x   0 user      (1000) user      (1000)     4617 2022-06-23 13:12:47.000000 onionprobe-1.1.2/packages/securedrop.py
--rwxr-xr-x   0 user      (1000) user      (1000)     5793 2022-06-23 15:51:18.000000 onionprobe-1.1.2/packages/tpo.py
--rw-r--r--   0 user      (1000) user      (1000)       90 2023-03-30 21:34:32.000000 onionprobe-1.1.2/pyproject.toml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.623141 onionprobe-1.1.2/scripts/
--rwxr-xr-x   0 user      (1000) user      (1000)     3873 2022-05-24 19:19:27.000000 onionprobe-1.1.2/scripts/generate-auth-keys-for-all-onion-services
--rwxr-xr-x   0 user      (1000) user      (1000)     2170 2023-03-29 19:00:58.000000 onionprobe-1.1.2/scripts/get-tor-debian-key
--rwxr-xr-x   0 user      (1000) user      (1000)     1724 2023-09-14 15:37:23.000000 onionprobe-1.1.2/scripts/provision
--rwxr-xr-x   0 user      (1000) user      (1000)      882 2023-03-30 21:05:53.000000 onionprobe-1.1.2/scripts/provision-onionprobe
--rwxr-xr-x   0 user      (1000) user      (1000)      476 2023-03-30 21:18:45.000000 onionprobe-1.1.2/scripts/provision-packaging-debian
--rwxr-xr-x   0 user      (1000) user      (1000)      417 2023-03-30 21:39:43.000000 onionprobe-1.1.2/scripts/provision-packaging-python
--rwxr-xr-x   0 user      (1000) user      (1000)     2696 2023-04-03 22:09:31.000000 onionprobe-1.1.2/scripts/upgrade-postgresql-database
--rw-r--r--   0 user      (1000) user      (1000)     1549 2023-09-28 21:19:45.663142 onionprobe-1.1.2/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:44.111135 onionprobe-1.1.2/tests/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-09-28 21:19:45.639141 onionprobe-1.1.2/tests/tpo/
--rw-r--r--   0 user      (1000) user      (1000)     5820 2022-05-05 18:47:15.000000 onionprobe-1.1.2/tests/tpo/tpo.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.754724 onionprobe-1.2.0/
+-rw-r--r--   0 user      (1000) user      (1000)        5 2022-05-23 21:15:17.000000 onionprobe-1.2.0/.dockerignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.834771 onionprobe-1.2.0/.github/
+-rw-r--r--   0 user      (1000) user      (1000)     1421 2023-03-13 15:44:25.000000 onionprobe-1.2.0/.github/gh-pages.yml
+-rw-r--r--   0 user      (1000) user      (1000)       78 2024-04-23 17:36:34.000000 onionprobe-1.2.0/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      348 2023-11-10 17:12:20.000000 onionprobe-1.2.0/.gitlab-ci-pages.yml
+-rw-r--r--   0 user      (1000) user      (1000)      454 2023-11-10 17:12:20.000000 onionprobe-1.2.0/.gitlab-ci-slides.yml
+-rw-r--r--   0 user      (1000) user      (1000)     2084 2024-04-18 18:13:49.000000 onionprobe-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 user      (1000) user      (1000)      256 2023-11-10 17:12:20.000000 onionprobe-1.2.0/.gitmodules
+-rw-r--r--   0 user      (1000) user      (1000)     5489 2022-03-11 13:55:54.000000 onionprobe-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 user      (1000) user      (1000)    19144 2024-04-24 17:55:21.000000 onionprobe-1.2.0/ChangeLog.md
+-rw-r--r--   0 user      (1000) user      (1000)    35147 2022-03-11 13:55:54.000000 onionprobe-1.2.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2098 2024-04-23 19:03:07.000000 onionprobe-1.2.0/Makefile
+-rw-r--r--   0 user      (1000) user      (1000)     1981 2024-04-24 18:00:03.754724 onionprobe-1.2.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      684 2024-03-21 11:46:08.000000 onionprobe-1.2.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.882769 onionprobe-1.2.0/configs/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.890768 onionprobe-1.2.0/configs/alertmanager/
+-rw-r--r--   0 user      (1000) user      (1000)     2337 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/alertmanager/alertmanager.yml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.902768 onionprobe-1.2.0/configs/apt/
+-rw-r--r--   0 user      (1000) user      (1000)      955 2023-10-03 16:50:11.000000 onionprobe-1.2.0/configs/apt/tor.list
+-rw-r--r--   0 user      (1000) user      (1000)     3890 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/env.sample
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.914767 onionprobe-1.2.0/configs/grafana/
+-rw-r--r--   0 user      (1000) user      (1000)    94451 2024-04-17 21:01:47.000000 onionprobe-1.2.0/configs/grafana/home.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.698778 onionprobe-1.2.0/configs/grafana/provisioning/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.930766 onionprobe-1.2.0/configs/grafana/provisioning/dashboards/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:22.000000 onionprobe-1.2.0/configs/grafana/provisioning/dashboards/.gitignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.946765 onionprobe-1.2.0/configs/grafana/provisioning/datasources/
+-rw-r--r--   0 user      (1000) user      (1000)      719 2022-05-23 13:08:40.000000 onionprobe-1.2.0/configs/grafana/provisioning/datasources/prometheus.yml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.966764 onionprobe-1.2.0/configs/grafana/provisioning/notifiers/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:59.000000 onionprobe-1.2.0/configs/grafana/provisioning/notifiers/.gitignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.982764 onionprobe-1.2.0/configs/grafana/provisioning/plugins/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 23:23:49.000000 onionprobe-1.2.0/configs/grafana/provisioning/plugins/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      305 2022-05-11 17:39:06.000000 onionprobe-1.2.0/configs/onionprobe.yaml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.006762 onionprobe-1.2.0/configs/prometheus/
+-rw-r--r--   0 user      (1000) user      (1000)     1839 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/prometheus/prometheus-rules.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1423 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/prometheus/prometheus.yml
+-rw-r--r--   0 user      (1000) user      (1000)    32781 2024-04-10 08:31:05.000000 onionprobe-1.2.0/configs/real-world-onion-sites.yaml
+-rw-r--r--   0 user      (1000) user      (1000)     6776 2024-04-10 08:31:31.000000 onionprobe-1.2.0/configs/securedrop.yaml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.018762 onionprobe-1.2.0/configs/systemd/
+-rw-r--r--   0 user      (1000) user      (1000)     1415 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/systemd/onionprobe-monitor.service
+-rw-r--r--   0 user      (1000) user      (1000)     2086 2023-03-30 18:40:33.000000 onionprobe-1.2.0/configs/test.yaml
+-rw-r--r--   0 user      (1000) user      (1000)    19360 2024-04-18 17:45:45.000000 onionprobe-1.2.0/configs/tor.yaml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.706778 onionprobe-1.2.0/containers/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.042760 onionprobe-1.2.0/containers/onionprobe/
+-rw-r--r--   0 user      (1000) user      (1000)     1823 2024-04-24 13:33:29.000000 onionprobe-1.2.0/containers/onionprobe/Dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     2081 2024-04-18 17:45:45.000000 onionprobe-1.2.0/containers/onionprobe/Dockerfile.pip
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.066759 onionprobe-1.2.0/containers/tor/
+-rw-r--r--   0 user      (1000) user      (1000)     1759 2024-04-24 13:42:17.000000 onionprobe-1.2.0/containers/tor/Dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1983 2024-04-18 17:45:45.000000 onionprobe-1.2.0/containers/tor/torrc
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.078759 onionprobe-1.2.0/contrib/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-05-23 13:08:40.000000 onionprobe-1.2.0/contrib/.gitignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.190753 onionprobe-1.2.0/debian/
+-rw-r--r--   0 user      (1000) user      (1000)     1180 2022-04-19 18:24:30.000000 onionprobe-1.2.0/debian/README.Debian
+-rw-r--r--   0 user      (1000) user      (1000)     1777 2024-04-24 17:56:50.000000 onionprobe-1.2.0/debian/changelog
+-rw-r--r--   0 user      (1000) user      (1000)      940 2023-04-03 18:18:40.000000 onionprobe-1.2.0/debian/control
+-rw-r--r--   0 user      (1000) user      (1000)     1083 2024-04-18 17:48:26.000000 onionprobe-1.2.0/debian/copyright
+-rw-r--r--   0 user      (1000) user      (1000)       52 2022-04-13 16:18:45.000000 onionprobe-1.2.0/debian/gbp.conf
+-rw-r--r--   0 user      (1000) user      (1000)       22 2022-04-13 16:18:45.000000 onionprobe-1.2.0/debian/manpages
+-rw-r--r--   0 user      (1000) user      (1000)      319 2022-04-19 18:24:30.000000 onionprobe-1.2.0/debian/onionprobe.default
+-rw-r--r--   0 user      (1000) user      (1000)       10 2022-04-13 16:18:45.000000 onionprobe-1.2.0/debian/onionprobe.docs
+-rw-r--r--   0 user      (1000) user      (1000)     1897 2022-04-19 18:24:30.000000 onionprobe-1.2.0/debian/onionprobe.init
+-rw-r--r--   0 user      (1000) user      (1000)      161 2022-05-10 21:12:42.000000 onionprobe-1.2.0/debian/onionprobe.install
+-rw-r--r--   0 user      (1000) user      (1000)     1150 2022-04-19 19:46:54.000000 onionprobe-1.2.0/debian/onionprobe.service
+-rw-r--r--   0 user      (1000) user      (1000)      550 2022-05-11 16:14:16.000000 onionprobe-1.2.0/debian/postinst
+-rw-r--r--   0 user      (1000) user      (1000)      517 2022-05-11 16:14:16.000000 onionprobe-1.2.0/debian/postrm
+-rwxr-xr-x   0 user      (1000) user      (1000)      529 2024-04-23 17:58:54.000000 onionprobe-1.2.0/debian/rules
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.198752 onionprobe-1.2.0/debian/source/
+-rw-r--r--   0 user      (1000) user      (1000)       13 2022-04-13 16:18:45.000000 onionprobe-1.2.0/debian/source/format
+-rw-r--r--   0 user      (1000) user      (1000)     6023 2024-04-24 15:34:46.000000 onionprobe-1.2.0/docker-compose.yaml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.310747 onionprobe-1.2.0/docs/
+-rw-r--r--   0 user      (1000) user      (1000)      275 2022-03-23 13:59:34.000000 onionprobe-1.2.0/docs/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      310 2024-04-23 17:30:26.000000 onionprobe-1.2.0/docs/.pages
+-rw-r--r--   0 user      (1000) user      (1000)      537 2024-02-29 12:08:02.000000 onionprobe-1.2.0/docs/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      199 2023-03-13 15:44:25.000000 onionprobe-1.2.0/docs/acknowledgements.md
+-rw-r--r--   0 user      (1000) user      (1000)      903 2023-03-13 15:44:25.000000 onionprobe-1.2.0/docs/alternatives.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.350745 onionprobe-1.2.0/docs/api/
+-rw-r--r--   0 user      (1000) user      (1000)       52 2023-03-13 23:41:14.000000 onionprobe-1.2.0/docs/api/.pages
+-rw-r--r--   0 user      (1000) user      (1000)      823 2024-02-20 17:37:03.000000 onionprobe-1.2.0/docs/api/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      467 2023-03-13 23:55:53.000000 onionprobe-1.2.0/docs/api/helpers.md
+-rw-r--r--   0 user      (1000) user      (1000)       92 2023-03-13 23:56:08.000000 onionprobe-1.2.0/docs/api/onionprobe.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.358744 onionprobe-1.2.0/docs/assets/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.418741 onionprobe-1.2.0/docs/assets/dashboard/
+-rw-r--r--   0 user      (1000) user      (1000)    83311 2024-04-09 20:40:46.000000 onionprobe-1.2.0/docs/assets/dashboard/descriptors.png
+-rw-r--r--   0 user      (1000) user      (1000)    63370 2024-04-10 09:36:42.000000 onionprobe-1.2.0/docs/assets/dashboard/intros.png
+-rw-r--r--   0 user      (1000) user      (1000)   113260 2024-04-09 20:40:46.000000 onionprobe-1.2.0/docs/assets/dashboard/latency.png
+-rw-r--r--   0 user      (1000) user      (1000)   166837 2024-04-10 09:36:42.000000 onionprobe-1.2.0/docs/assets/dashboard/overview.png
+-rw-r--r--   0 user      (1000) user      (1000)    47138 2023-03-13 15:44:25.000000 onionprobe-1.2.0/docs/assets/logo.jpg
+-rw-r--r--   0 user      (1000) user      (1000)    19144 2024-04-24 17:55:21.000000 onionprobe-1.2.0/docs/changelog.md
+-rw-r--r--   0 user      (1000) user      (1000)     1496 2023-03-13 18:15:27.000000 onionprobe-1.2.0/docs/configurations.md
+-rw-r--r--   0 user      (1000) user      (1000)     1987 2024-04-24 17:56:06.000000 onionprobe-1.2.0/docs/development.md
+-rw-r--r--   0 user      (1000) user      (1000)      753 2024-02-29 12:09:39.000000 onionprobe-1.2.0/docs/installation.md
+-rw-r--r--   0 user      (1000) user      (1000)      149 2024-04-17 12:59:03.000000 onionprobe-1.2.0/docs/issues.md
+-rw-r--r--   0 user      (1000) user      (1000)     1022 2023-03-13 15:44:25.000000 onionprobe-1.2.0/docs/references.md
+-rw-r--r--   0 user      (1000) user      (1000)      687 2023-03-13 15:44:25.000000 onionprobe-1.2.0/docs/requirements.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.430741 onionprobe-1.2.0/docs/slides/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.726776 onionprobe-1.2.0/docs/slides/2022.Q1/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.446740 onionprobe-1.2.0/docs/slides/2022.Q1/demoday/
+-rw-r--r--   0 user      (1000) user      (1000)     2303 2023-03-13 20:47:53.000000 onionprobe-1.2.0/docs/slides/2022.Q1/demoday/demoday.md
+-rw-r--r--   0 user      (1000) user      (1000)      708 2023-03-14 11:29:44.000000 onionprobe-1.2.0/docs/slides/Makefile
+-rw-r--r--   0 user      (1000) user      (1000)     8750 2024-04-10 09:36:42.000000 onionprobe-1.2.0/docs/standalone.md
+-rw-r--r--   0 user      (1000) user      (1000)      626 2023-03-13 15:59:26.000000 onionprobe-1.2.0/docs/structure.md
+-rw-r--r--   0 user      (1000) user      (1000)     3411 2024-04-10 10:24:06.000000 onionprobe-1.2.0/docs/upgrading.md
+-rw-r--r--   0 user      (1000) user      (1000)      768 2024-04-23 18:08:49.000000 onionprobe-1.2.0/docs/usage.md
+-rw-r--r--   0 user      (1000) user      (1000)     9233 2023-10-03 16:50:11.000000 onionprobe-1.2.0/kvmxfile
+-rw-r--r--   0 user      (1000) user      (1000)      651 2023-12-04 13:12:12.000000 onionprobe-1.2.0/mkdocs.yml
+-rwxr-xr-x   0 user      (1000) user      (1000)      884 2024-04-18 17:45:45.000000 onionprobe-1.2.0/onionprobe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.474739 onionprobe-1.2.0/packages/
+-rwxr-xr-x   0 user      (1000) user      (1000)     2793 2024-04-23 17:59:12.000000 onionprobe-1.2.0/packages/manpage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.614731 onionprobe-1.2.0/packages/onionprobe/
+-rw-r--r--   0 user      (1000) user      (1000)       58 2023-03-21 12:02:25.000000 onionprobe-1.2.0/packages/onionprobe/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3571 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/app.py
+-rw-r--r--   0 user      (1000) user      (1000)    10281 2023-03-21 14:39:42.000000 onionprobe-1.2.0/packages/onionprobe/certificate.py
+-rw-r--r--   0 user      (1000) user      (1000)    19464 2024-04-24 16:13:27.000000 onionprobe-1.2.0/packages/onionprobe/config.py
+-rw-r--r--   0 user      (1000) user      (1000)    12069 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/descriptor.py
+-rw-r--r--   0 user      (1000) user      (1000)     8458 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/http.py
+-rw-r--r--   0 user      (1000) user      (1000)     4964 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/init.py
+-rw-r--r--   0 user      (1000) user      (1000)     2367 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/logger.py
+-rw-r--r--   0 user      (1000) user      (1000)     3521 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/main.py
+-rw-r--r--   0 user      (1000) user      (1000)    22914 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/metrics.py
+-rw-r--r--   0 user      (1000) user      (1000)     5493 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/prober.py
+-rw-r--r--   0 user      (1000) user      (1000)     1297 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/teardown.py
+-rw-r--r--   0 user      (1000) user      (1000)     2820 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/time.py
+-rw-r--r--   0 user      (1000) user      (1000)    10312 2023-04-03 17:20:38.000000 onionprobe-1.2.0/packages/onionprobe/tls.py
+-rw-r--r--   0 user      (1000) user      (1000)     8939 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/onionprobe/tor.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.750725 onionprobe-1.2.0/packages/onionprobe.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1981 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2914 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       63 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      102 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2024-04-24 18:00:02.000000 onionprobe-1.2.0/packages/onionprobe.egg-info/top_level.txt
+-rwxr-xr-x   0 user      (1000) user      (1000)     4185 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/real-world-onion-sites.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     4601 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/securedrop.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     5777 2024-04-18 17:45:45.000000 onionprobe-1.2.0/packages/tpo.py
+-rw-r--r--   0 user      (1000) user      (1000)       90 2023-03-30 21:34:32.000000 onionprobe-1.2.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      107 2024-04-17 15:54:13.000000 onionprobe-1.2.0/renovate.json
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.730726 onionprobe-1.2.0/scripts/
+-rwxr-xr-x   0 user      (1000) user      (1000)     3857 2024-04-18 17:45:45.000000 onionprobe-1.2.0/scripts/generate-auth-keys-for-all-onion-services
+-rwxr-xr-x   0 user      (1000) user      (1000)     2170 2023-03-29 19:00:58.000000 onionprobe-1.2.0/scripts/get-tor-debian-key
+-rwxr-xr-x   0 user      (1000) user      (1000)     1742 2023-12-11 15:44:28.000000 onionprobe-1.2.0/scripts/provision
+-rwxr-xr-x   0 user      (1000) user      (1000)      882 2023-03-30 21:05:53.000000 onionprobe-1.2.0/scripts/provision-onionprobe
+-rwxr-xr-x   0 user      (1000) user      (1000)      476 2023-03-30 21:18:45.000000 onionprobe-1.2.0/scripts/provision-packaging-debian
+-rwxr-xr-x   0 user      (1000) user      (1000)      422 2023-10-03 16:50:11.000000 onionprobe-1.2.0/scripts/provision-packaging-python
+-rwxr-xr-x   0 user      (1000) user      (1000)     1320 2023-03-30 21:18:27.000000 onionprobe-1.2.0/scripts/provision-packaging-sbuild
+-rwxr-xr-x   0 user      (1000) user      (1000)     2696 2023-04-03 22:09:31.000000 onionprobe-1.2.0/scripts/upgrade-postgresql-database
+-rw-r--r--   0 user      (1000) user      (1000)     1561 2024-04-24 18:00:03.758724 onionprobe-1.2.0/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:02.738776 onionprobe-1.2.0/tests/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-24 18:00:03.738725 onionprobe-1.2.0/tests/tpo/
+-rw-r--r--   0 user      (1000) user      (1000)     5820 2022-05-05 18:47:15.000000 onionprobe-1.2.0/tests/tpo/tpo.json
```

### Comparing `onionprobe-1.1.2/.github/gh-pages.yml` & `onionprobe-1.2.0/.github/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/CODE_OF_CONDUCT.md` & `onionprobe-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/ChangeLog.md` & `onionprobe-1.2.0/ChangeLog.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,112 @@
 # Onionprobe ChangeLog
 
+## v1.2.0 - 2024-04-24
+
+### Features
+
+* New metrics ([tpo/onion-services/onionprobe#78][]):
+    * From the outer descriptor wrapper:
+        * `descriptor-lifetime`.
+        * `revision-counter`.
+    * From the second layer of encryption:
+        * `single-onion-service`.
+        * `pow-params`.
+    * HSDir latency when fetching descriptors.
+
+* Enhanced Grafana Dashboard ([tpo/onion-services/onionprobe#80][]) with the
+  following new visualizations:
+    * Overview:
+        * Current failure rate of onionsites.
+        * Total expiring certificates in the next 7 days.
+        * List of certificate expirations up to the next 180 days.
+        * List of unreachable instances.
+        * Graph with the total unreachable instances.
+        * List of invalid HTTPS certificates.
+        * List of services with HTTPS errors.
+    * Performance:
+        * Total of minimum, average and maximum service connection latency.
+        * Total of minimum, average and maximum descriptor fetch latency.
+        * Chart of minimum, average and maximum service connection latency.
+        * Chart of minimum, average and maximum descriptor fetch latency.
+        * Rate of services using the single hop mode, relative to the total services monitored.
+        * List of slow services.
+    * Descriptors:
+        * List of services missing a published descriptor.
+        * Chart of the minimum, average and maximum descriptor sizes (decrypted outer layer).
+        * Chart of the minimum, average and maximum descriptor sizes (decrypted second layer).
+    * Introduction points:
+        * Chart of minimum, average and maximum number of introduction points per service.
+        * List of services and it's number of introduction points.
+    * HSDir:
+        * Total number of HSDirs tested.
+        * Chart of minimum, average and maximum HSDir latency for fetching descriptors.
+        * List of HSDirs sorted by descriptor fetch latency.
+    * Proof of Work (PoW):
+        * Ratio of services with PoW enabled, relative to the total services monitored.
+        * Total number of services with PoW enabled.
+        * Chart of minimum, average and maximum PoW v1 effort seem.
+        * List of services with PoW enabled.
+        * List of services with PoW enabled with effort greater than zero.
+
+* Improved log message for elapsed time.
+
+* New log messages for:
+    * Number of introduction points.
+    * HS_DESC events:
+        * Descriptor reachability.
+        * HSDir used.
+
+* Create a GitLab release at every new tag (experimental)
+  ([tpo/onion-services/onionprobe#82][]).
+
+* Running lintian on CI to check the generated Debian package.
+
+[tpo/onion-services/onionprobe#78]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/78
+[tpo/onion-services/onionprobe#80]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/80
+[tpo/onion-services/onionprobe#82]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/82
+
+### Fixes
+
+* Manpage generation is now compatible with the Onion Services
+  Ecosystem Portal ([tpo/onion-services/ecosystem#1][]).
+
+* Use the correct copyright line in source files.
+
+* Support for a wider range of [pyca/cryptography][] versions at `setup.cfg`.
+
+* Display Tor bootstrap messages only for the debug log level.
+
+* Disable stem logging if log level is below debug ([tpo/onion-services/onionprobe#63][]).
+
+* Exit codes now reflects reality ([tpo/onion-services/onionprobe#64][]).
+
+* Calculate the elapsed time for descriptors right after fetching.
+
+* Updated the [SecureDrop list][].
+
+* Upgraded Grafana image to 10.4.2.
+
+* Upgraded Alertmanager image to 0.27.0.
+
+* Upgraded Prometheus image to 2.51.2.
+
+* Upgraded PostgreSQL image to 16.
+  Please run the [needed upgrading steps](upgrading.md#major-upgrades).
+
+* Upgraded CI and container images to Debian bookworm.
+
+* Upgraded `vendors/onion-mkdocs`.
+
+[tpo/onion-services/ecosystem#1]: https://gitlab.torproject.org/tpo/onion-services/ecosystem/-/issues/1
+[pyca/cryptography]: https://cryptography.io
+[tpo/onion-services/onionprobe#63]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/63
+[tpo/onion-services/onionprobe#64]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/64
+[SecureDrop list]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/blob/main/configs/securedrop.yaml
+
 ## v1.1.2 - 2023-09-28
 
 ### Fixes
 
 * Make the tor process quiet when generating hashed passwords (reported by
   @anarcat): https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/81
 
@@ -63,15 +166,15 @@
   features for defense in depth.
 
   We recommend, for the prometheus format, that the only address that can
   access this port should be the Prometheus server itself. Remember that the
   connection is unencrypted (HTTP) hence consider using a tool like stunnel to
   secure the link from this port to the server.
 
-  Check the [standalone monitoring node docs](docs/standalone.md) for
+  Check the [standalone monitoring node docs](standalone.md) for
   detailed instructions in how to enable this additional metric collection.
 
 * TLS certificate verification:
   * Added a global `tls_verify` flag to check certificates during HTTP tests.
     Set it to `false` to ignore TLS certificate verification.
     By default all TLS certificates are checked.
```

### Comparing `onionprobe-1.1.2/LICENSE` & `onionprobe-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/Makefile` & `onionprobe-1.2.0/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -41,33 +41,24 @@
 	@./packages/securedrop.py
 	@./packages/tpo.py
 
 #
 # Documentation
 #
 
+ONION_MKDOCS_PATH = vendors/onion-mkdocs
+
 docs: compile-docs
 
 manpage:
 	@./packages/manpage.py
+	@sed -e '1i\\# Manual page' -e 's|^#|##|g' -e '/^%/d' docs/man/onionprobe.1.txt > docs/man/README.md
 
 compile-docs: manpage
-	@cp docs/man/onionprobe.1.md docs/man/onionprobe.1.md.orig
-	@sed -i -e '1i\\# ONIONPROBE(1) Onionprobe User Manual' -e 's|^#|##|g' -e '/^%/d' docs/man/onionprobe.1.md
-	@mkdocs build
-	@mv docs/man/onionprobe.1.md.orig docs/man/onionprobe.1.md
-
-serve-docs:
-	@mkdocs serve
-
-watch-docs:
-	@./scripts/watch-docs
-
-share-docs: compile
-	@onionshare-cli --disable_csp --website public
+	@make onion-mkdocs-build
 
 #
 # Packaging
 #
 
 clean:
 	@find -name __pycache__ -exec rm -rf {} \; &> /dev/null || true
@@ -95,7 +86,15 @@
 	@sbuild  -c unstable-amd64-sbuild
 
 #
 # Release
 #
 
 release: clean configs docs
+
+#
+# Other
+#
+
+# Include the Onion MkDocs Makefile
+# See https://www.gnu.org/software/make/manual/html_node/Include.html
+-include vendors/onion-mkdocs/Makefile.onion-mkdocs
```

### Comparing `onionprobe-1.1.2/PKG-INFO` & `onionprobe-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onionprobe
-Version: 1.1.2
+Version: 1.2.0
 Summary: Test and monitors the status of Tor Onion Services
 Home-page: https://tpo.pages.torproject.net/onion-services/onionprobe
 Author: Silvio Rhatto
 Author-email: rhatto@torproject.org
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.27.1
 Requires-Dist: stem>=1.8.0
 Requires-Dist: prometheus-client>=0.14.1
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pysocks>=1.7.1
-Requires-Dist: cryptography==3.3.2
+Requires-Dist: cryptography>=3.4.8
 
 # Onionprobe
 
 ![](docs/assets/logo.jpg "Onionprobe")
 
 Onionprobe is a tool for testing and monitoring the status of
 [Tor Onion Services](https://community.torproject.org/onion-services/) sites.
@@ -43,8 +43,8 @@
 endpoints and paths, optionally exporting to [Prometheus](https://prometheus.io)
 and with [Grafana](https://grafana.com/) support.
 
 The full documentation is available in the [docs/][] folder and at the
 [Onionprobe website][].
 
 [docs/]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/tree/main/docs
-[Onionprobe website]: https://tpo.pages.torproject.net/onion-services/onionprobe/
+[Onionprobe website]: https://community.torproject.org/onion-services/ecosystem/apps/web/onionprobe/
```

### Comparing `onionprobe-1.1.2/configs/alertmanager/alertmanager.yml` & `onionprobe-1.2.0/configs/alertmanager/alertmanager.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ---
 # Sample Alertmanager configuration to be used with Docker Compose
 #
 # Based on https://github.com/prometheus/alertmanager/blob/main/doc/examples/simple.yml
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/configs/apt/tor.list` & `onionprobe-1.2.0/configs/apt/tor.list`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Stable Tor packages
-deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org bullseye main
-deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org bullseye main
+deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org bookworm main
+deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org bookworm main
 
 # Uncomment the following lines if you want to try experimental packages
-#deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-experimental-bullseye main
-#deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-experimental-bullseye main
+#deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-experimental-bookworm main
+#deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-experimental-bookworm main
 
 # Uncomment the following lines if you want to try nightly builds
-#deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-nightly-main-bullseye main
-#deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-nightly-main-bullseye main
+#deb     [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-nightly-main-bookworm main
+#deb-src [signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org tor-nightly-main-bookworm main
```

### Comparing `onionprobe-1.1.2/configs/env.sample` & `onionprobe-1.2.0/configs/env.sample`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # Sample Docker Compose environment file for the Onionprobe monitoring node.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -76,14 +76,23 @@
 # Grafana Start TLS policy
 #GRAFANA_SMTP_STARTTLS_POLICY=
 
 # Grafana domain
 #GRAFANA_SERVER_DOMAIN=
 
 # Grafana root URL
+#
+# It's recommended to set this variable once Grafana's .onion address is available.
+# This ensures proper Grafana behavior behind a proxy, like proper WebSocket
+# connections, and seems to avoid some NS_BINDING_ABORTED errors in the
+# browser.
+#
+# Check https://github.com/grafana/grafana/issues/36929#issuecomment-883237258
+#       https://grafana.com/docs/grafana/latest/setup-grafana/set-up-grafana-live/#request-origin-check
+#       https://grafana.com/docs/grafana/latest/setup-grafana/configure-grafana/#root_url
 #GRAFANA_SERVER_ROOT_URL=
 
 # Toggle Grafana anonymous statistics submission
 #GRAFANA_ANALYTICS_REPORTING_ENABLED=false
 
 # Whether to automatically check for Grafana updates
 #GRAFANA_ANALYTICS_CHECK_FOR_UPDATES=false
```

### Comparing `onionprobe-1.1.2/configs/grafana/provisioning/datasources/prometheus.yml` & `onionprobe-1.2.0/configs/grafana/provisioning/datasources/prometheus.yml`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/configs/prometheus/prometheus-rules.yml` & `onionprobe-1.2.0/configs/prometheus/prometheus-rules.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 # Sample Prometheus rule file to be used with Docker Compose.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/configs/prometheus/prometheus.yml` & `onionprobe-1.2.0/configs/prometheus/prometheus.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 # Sample Prometheus configuration to be used with Docker Compose.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/configs/real-world-onion-sites.yaml` & `onionprobe-1.2.0/configs/real-world-onion-sites.yaml`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/configs/securedrop.yaml` & `onionprobe-1.2.0/configs/securedrop.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,14 @@
     address: cy6wj77vryhcyh6go576hxycjz4wxlo4s5vevdinkw3armwzty5jozyd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  ABC:
-    address: dqa4zahticcobfq5rmmmbewbdtyiznbl75hu23k4i37y7yfoosrh7mqd.onion
-    paths:
-    - allowed_statuses:
-      - 200
-      path: /
-    port: 80
-    protocol: http
   Aftenposten AS:
     address: tiykfvhb562gheutfnedysnhrxpxoztyszkqyroloyepwzxmxien77id.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
@@ -79,72 +71,72 @@
     address: qmifwf762qftydprw2adbg7hs2mkunac5xrz3cb5busaflji3rja5lid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Dagbladet:
-    address: udgkmwzb5jmucs2r2cjtfscgf6s6d6otbt2qfiinovtwknsxk5oyzeid.onion
+  DR - Danish Broadcasting Corporation:
+    address: hpaauqmv2wegiu4cz6st6hty4s7gwqol272xhcu3xmh6azw2f2zffgid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Financial Times:
-    address: nqu6crmtnzs2hs5abo2uqni53yqsnnwqnerdxuzyz5yxairxlzjzt6yd.onion
+  Dagbladet:
+    address: ydbpz5knb6ji3bdtahhm3wo7sed6lsy5vqnwfpnhpez4bquvoexbz7qd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Forbes:
-    address: 6zonlfhh7aqtfwoyvdlad3nxn6ljecx2k6tyyy3spt43nn54q6lvncid.onion
+  Der Spiegel:
+    address: q6vdlj2ukulrqk37piqgxucpcwtxzdjhvjzqrfbevuhrzimsgjltmpqd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Forbidden Stories:
-    address: fg25fqpu2dnxp24xs3jlcley4hp2inshpzek44q3czkhq3zffoqk26id.onion
+  Disclose:
+    address: 3tcbrdg2ejwu5nzbjg7xqixkis6mdbgkkthcyxmzv2q3oi6v7th5ahqd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  HuffPost:
-    address: ppw2pmtagxykinex6uubypsommtrcg6ytdh6bcr6agq2wxnrweao4cad.onion
+  Financial Times:
+    address: nqu6crmtnzs2hs5abo2uqni53yqsnnwqnerdxuzyz5yxairxlzjzt6yd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Institute for Quantitative Social Science at Harvard University:
-    address: 5kcyaqagvnrvyan7y5ntzreqsn2msowqlmtoo46qju2pctlbkzzztxqd.onion
+  Forbes:
+    address: 6zonlfhh7aqtfwoyvdlad3nxn6ljecx2k6tyyy3spt43nn54q6lvncid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  K-Tipp:
-    address: tukldpfzdizsrfyvdljnipmvix2dcb5hmfoemcidkw7bq56wxblk6did.onion
+  Forbidden Stories:
+    address: fg25fqpu2dnxp24xs3jlcley4hp2inshpzek44q3czkhq3zffoqk26id.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Lessig.law LLC:
-    address: o4nhtigrvss5wktskr5ph5m22ewmhk7nr5at2tac2wdsworcqz62vsqd.onion
+  Institute for Quantitative Social Science at Harvard University:
+    address: 5kcyaqagvnrvyan7y5ntzreqsn2msowqlmtoo46qju2pctlbkzzztxqd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
   NOYB:
@@ -175,22 +167,14 @@
     address: mzi5yynpd6qqq3lnh7vnaojy36v3hcorytsut47zwkguhnorduyxwead.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  ProPublica:
-    address: lvtu6mh6dd6ynqcxtd2mseqfkm7g2iuxvjobbyzpgx2jt427zvd7n3ad.onion
-    paths:
-    - allowed_statuses:
-      - 200
-      path: /
-    port: 80
-    protocol: http
   Public Intelligence:
     address: z4gd5t2g6u6kqeqjeddvmvlhhjtjgslg4elh4ztnct7snskcd7phbiyd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
@@ -215,24 +199,24 @@
     address: srumyob2jq5nvppzt66aaab333n2wmq6xgkg4khfe24ixdb7umf7mtyd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  TechCrunch:
-    address: vplxle7awnyvvvduv6exnwrxbf4gzsh7lv7fxosnfl2ecidkttcbfcqd.onion
+  Taz:
+    address: tazleakssvtc2lqrhkpvbzo6qwolcldzkzoexo7wombufd6a573bhlid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  The Center for Public Integrity:
-    address: ahgpmkiaqfde4innkotgz5q6bgt4gbxmelqod3tjtmpdt3zvxaxareyd.onion
+  TechCrunch:
+    address: vplxle7awnyvvvduv6exnwrxbf4gzsh7lv7fxosnfl2ecidkttcbfcqd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
   The Globe and Mail:
@@ -248,53 +232,37 @@
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
   The Intercept:
-    address: xpxduj55x2j27l2qytu2tcetykyfxbjbafin3x4i3ywddzphkbrd3jyd.onion
+    address: lhollo6vzrft3w77mgm67fhfv3fjadmf7oinmafa7tbmupc273oi7kid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
   The Washington Post:
     address: vfnmxpa6fo4jdpyq3yneqhglluweax2uclvxkytfpmpkp5rsl75ir5qd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  Thomson Reuters:
-    address: dvvbik7vtmvwwgj2cziqa36noa26l2pweghd26e5l5qwdnqtwmfhz5id.onion
-    paths:
-    - allowed_statuses:
-      - 200
-      path: /
-    port: 80
-    protocol: http
   Toronto Star:
     address: yj3b7rgmglcocbbvzrwfbo4d6j2aa7thwupra4yqutbd27v3vxcpvgid.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
     protocol: http
-  VICE Media:
-    address: a2c6mmacrmxtaspbolytfxm6q2zq7svtkuaog5xetbcxr3mpy4pmomid.onion
-    paths:
-    - allowed_statuses:
-      - 200
-      path: /
-    port: 80
-    protocol: http
   Whistleblower Aid:
     address: kogbxf4ysay2qzozmg7ar45ijqmj2vxrwqa4upzqq2i7sqj7wv7wcdqd.onion
     paths:
     - allowed_statuses:
       - 200
       path: /
     port: 80
```

### Comparing `onionprobe-1.1.2/configs/systemd/onionprobe-monitor.service` & `onionprobe-1.2.0/configs/systemd/onionprobe-monitor.service`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # Systemd service file to run the Onionprobe monitoring node using Docker
 # Compose
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/configs/test.yaml` & `onionprobe-1.2.0/configs/test.yaml`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/configs/tor.yaml` & `onionprobe-1.2.0/configs/tor.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ---
 # Sample config file for Onionprobe
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/containers/onionprobe/Dockerfile` & `onionprobe-1.2.0/containers/onionprobe/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # Dockerfile for Onionprobe.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-FROM debian:bullseye
+FROM debian:bookworm
 MAINTAINER Silvio Rhatto <rhatto@torproject.org>
 
 ENV APP="onionprobe"
 ENV APP_BASE="/srv/"
 ENV SHELL="/bin/bash"
 ENV ONIONPROBE_CONFIG="/srv/onionprobe/configs/tor.yaml"
```

### Comparing `onionprobe-1.1.2/containers/onionprobe/Dockerfile.pip` & `onionprobe-1.2.0/containers/onionprobe/Dockerfile.pip`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # Dockerfile for Onionprobe which uses the package available from PyPI.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-FROM debian:bullseye
+FROM debian:bookworm
 MAINTAINER Silvio Rhatto <rhatto@torproject.org>
 
 ENV APP="onionprobe"
 ENV APP_BASE="/srv/"
 ENV SHELL="/bin/bash"
 
 # Use the default configuration from the pip install
```

### Comparing `onionprobe-1.1.2/containers/tor/Dockerfile` & `onionprobe-1.2.0/containers/tor/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # Dockerfile for a Tor container.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -13,15 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-FROM debian:bullseye
+FROM debian:bookworm
 MAINTAINER Silvio Rhatto <rhatto@torproject.org>
 
 ENV APP="tor"
 ENV APP_BASE="/etc"
 ENV SHELL="/bin/bash"
 
 WORKDIR ${APP_BASE}/${APP}
@@ -46,15 +46,15 @@
     apt-get install -y \
     deb.torproject.org-keyring \
     tor basez \
     && rm -rf /var/lib/apt/lists/*
 
 COPY containers/tor/torrc ${APP_BASE}/${APP}/torrc
 
-RUN chown -R debian-tor. ${APP_BASE}/${APP}/torrc
+RUN chown -R debian-tor: ${APP_BASE}/${APP}/torrc
 
 RUN chmod 600 ${APP_BASE}/${APP}/torrc
 
 USER debian-tor
 
 ENTRYPOINT [ "/usr/bin/tor", "-f", "/etc/tor/torrc" ]
```

### Comparing `onionprobe-1.1.2/containers/tor/torrc` & `onionprobe-1.2.0/containers/tor/torrc`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Containerized Tor daemon configuration for Onionprobe.
 #
 # This is a sample Tor configuration for a containerized service to be used
 # along with Onionprobe to access a Grafana Dashboard via an Onion Service and
 # to optionally route Onionprobe's traffic via a persistent daemon.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/debian/README.Debian` & `onionprobe-1.2.0/debian/README.Debian`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/changelog` & `onionprobe-1.2.0/debian/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+onionprobe (1.2.0) unstable; urgency=medium
+
+  * New upstream version.
+
+ -- Silvio Rhatto <rhatto@torproject.org>  Wed, 24 Apr 2024 14:56:11 -0300
+
 onionprobe (1.1.2) unstable; urgency=medium
 
   * New upstream version.
 
  -- Silvio Rhatto <rhatto@torproject.org>  Thu, 28 Sep 2023 18:10:45 -0300
 
 onionprobe (1.1.1) unstable; urgency=medium
```

### Comparing `onionprobe-1.1.2/debian/control` & `onionprobe-1.2.0/debian/control`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/copyright` & `onionprobe-1.2.0/debian/copyright`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Format: https://www.debian.org/doc/packaging-manuals/copyright-format/1.0/
 Upstream-Name: onionprobe
 Source: https://gitlab.torproject.org/tpo/onion-services/onionprobe
 
 Files: *
-Copyright: 2022 Silvio Rhatto <rhatto@torproject.org>
+Copyright: 2024 The Tor Project, Inc.
 License: GPL-3.0+
 
 License: GPL-3.0+
- Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+ Copyright (C) 2024 The Tor Project, Inc.
  .
  This program is free software: you can redistribute it and/or modify
  it under the terms of the GNU General Public License as
  published by the Free Software Foundation, either version 3 of the
  License, or (at your option) any later version.
  .
  This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/debian/onionprobe.init` & `onionprobe-1.2.0/debian/onionprobe.init`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/onionprobe.service` & `onionprobe-1.2.0/debian/onionprobe.service`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/postinst` & `onionprobe-1.2.0/debian/postinst`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/postrm` & `onionprobe-1.2.0/debian/postrm`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/debian/rules` & `onionprobe-1.2.0/debian/rules`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,13 @@
 
 %:
 	dh $@ --with=python3 --buildsystem=pybuild
 
 override_dh_auto_build:
 	# Pipe output to sed to avoid http://lintian.debian.org/tags/hyphen-used-as-minus-sign.html
 	# Fixed in http://johnmacfarlane.net/pandoc/releases.html#pandoc-1.10-2013-01-19
-	pandoc -s -w man docs/man/onionprobe.1.md -o docs/man/onionprobe.1
+	pandoc -s -f markdown -w man docs/man/onionprobe.1.txt -o docs/man/onionprobe.1
 	sed -i -e 's/--/\\-\\-/g' docs/man/onionprobe.1
 	dh_auto_build
 
-override_dh_auto_install:
-	dh_auto_install
-	# Remove duplicate configs created by the Python packaging procedure
-	rm -rf debian/onionprobe/usr/etc
-
 override_dh_installinit:
 	dh_installinit --no-enable
```

### Comparing `onionprobe-1.1.2/docker-compose.yaml` & `onionprobe-1.2.0/docker-compose.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Docker Compose configuration for the Onionprobe Standalone Monitoring node.
 # See docs/standalone.md for details.
 #
 version: '3'
 
 services:
   prometheus:
-    image: docker.io/prom/prometheus:v2.43.0
+    image: docker.io/prom/prometheus:v2.51.2
 
     volumes:
       - ./${PROMETHEUS_CONFIG:-configs/prometheus/prometheus.yml}:/etc/prometheus/prometheus.yml
       - ./${PROMETHEUS_RULES:-configs/prometheus/prometheus-rules.yml}:/etc/prometheus/prometheus-rules.yml
       - prometheus:/prometheus
 
     ports:
@@ -23,15 +23,15 @@
       - '--web.console.libraries=/usr/share/prometheus/console_libraries'
       - '--web.console.templates=/usr/share/prometheus/consoles'
       - '--web.enable-admin-api'
       - '--web.enable-lifecycle'
       - '--web.external-url=${PROMETHEUS_WEB_EXTERNAL_URL:-http://hostname:9090}'
 
     healthcheck:
-      test    : ["CMD-SHELL", "/bin/wget http://localhost:9090/-/healthy -q -O - | /bin/grep -q 'Prometheus is Healthy'"]
+      test    : ["CMD-SHELL", "/bin/wget http://localhost:9090/-/healthy -q -O - | /bin/grep -q 'Prometheus Server is Healthy'"]
       interval: 10s
       timeout : 30s
       retries : 50
 
     restart: always
 
     # Use a static network IP to allow Prometheus to collect MetricsPort data
@@ -42,15 +42,15 @@
     #    ipv4_address: 172.19.0.100
 
     # Profiles
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: ["prometheus", "all"]
 
   alertmanager:
-    image: docker.io/prom/alertmanager:v0.25.0
+    image: docker.io/prom/alertmanager:v0.27.0
 
     volumes:
       - ./${ALERTMANAGER_CONFIG:-configs/alertmanager/alertmanager.yml}:/etc/alertmanager/alertmanager.yml
       - alertmanager:/alertmanager
 
     ports:
       - 9093:9093
@@ -62,15 +62,15 @@
     restart: always
 
     # Profiles
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: ["alertmanager", "all"]
 
   postgres:
-    image: postgres:15
+    image: postgres:16
 
     environment:
       POSTGRES_USER: grafana
       POSTGRES_DB: grafana
       POSTGRES_PASSWORD: ${GRAFANA_DATABASE_PASSWORD:-unsafe-password-please-change}
 
     volumes:
@@ -79,15 +79,15 @@
     restart: always
 
     # Profiles
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: [ "grafana", "all" ]
 
   grafana:
-    image: docker.io/grafana/grafana:9.4.7
+    image: docker.io/grafana/grafana:10.4.2
 
     volumes:
       - ./${GRAFANA_PROVISIONING:-configs/grafana/provisioning}:/etc/grafana/provisioning
       - ./${GRAFANA_HOME_DASHBOARD:-configs/grafana/home.json}:${GRAFANA_DASHBOARDS_DEFAULT_HOME_DASHBOARD:-/etc/grafana/home.json}
       - grafana:/var/lib/grafana
 
     environment:
@@ -119,15 +119,15 @@
       - postgres
 
     # Profile
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: ["grafana", "all"]
 
   tor:
-    image: "onionprobe/tor:1.1.0"
+    image: "onionprobe/tor:1.2.0"
 
     build:
       context: .
       dockerfile: containers/tor/Dockerfile
 
     volumes:
       - ./scripts/generate-auth-keys-for-all-onion-services:/usr/local/bin/generate-auth-keys-for-all-onion-services
@@ -137,15 +137,15 @@
 
     # Profile
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: ["tor", "all"]
 
   # Service that periodically compiles an Onionprobe configuration
   configurator:
-    image: "onionprobe/onionprobe:1.1.0"
+    image: "onionprobe/onionprobe:1.2.0"
 
     build:
       context: .
       dockerfile: containers/onionprobe/Dockerfile
 
     tty: true
     stdin_open: true
@@ -159,15 +159,15 @@
     restart: always
 
     # Profile
     # This needs a newer Docker Compose (>= 1.28)
     #profiles: ["configurator", "all"]
 
   onionprobe:
-    image: "onionprobe/onionprobe:1.1.0"
+    image: "onionprobe/onionprobe:1.2.0"
 
     build:
       context: .
       dockerfile: containers/onionprobe/Dockerfile
 
     tty: true
     stdin_open: true
```

### Comparing `onionprobe-1.1.2/docs/README.md` & `onionprobe-1.2.0/docs/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # Onionprobe
 
 ![](assets/logo.jpg "Onionprobe")
 
-Onionprobe is a tool for testing and monitoring the status of
+[Onionprobe][] is a tool for testing and monitoring the status of
 [Tor Onion Services](https://community.torproject.org/onion-services/) sites.
 
 It can run a single time or continuously to probe a set of onion services
 endpoints and paths, optionally exporting to
 [Prometheus](https://prometheus.io) and with [Grafana](https://grafana.com/)
 and [Alertmanager](https://github.com/prometheus/alertmanager) support.
 
-The Onionprobe repository is located at
-[https://gitlab.torproject.org/tpo/onion-services/onionprobe][].
-
-[https://gitlab.torproject.org/tpo/onion-services/onionprobe]: https://gitlab.torproject.org/tpo/onion-services/onionprobe
+[Onionprobe]: https://gitlab.torproject.org/tpo/onion-services/onionprobe
```

### Comparing `onionprobe-1.1.2/docs/alternatives.md` & `onionprobe-1.2.0/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/api/README.md` & `onionprobe-1.2.0/docs/api/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This section documents the Onionprobe API.
 
 ## Basic usage
 
 Onionprobe can be easily run as a library.
 
-If you [installed it](installation.md) as a package, you can just import it
+If you [installed it](../installation.md) as a package, you can just import it
 directly on your code like any other installed Python package:
 
 ```python
 from onionprobe.app import run_from_cmdline
 
 if __name__ == "__main__":
     run_from_cmdline()
@@ -24,9 +24,9 @@
 ```python
 from vendors.onionprobe.packages.onionprobe.app import run_from_cmdline
 
 if __name__ == "__main__":
     run_from_cmdline()
 ```
 
-The [package API page](api/onionprobe.md) details all the available
+The [package API page](onionprobe.md) details all the available
 modules and functionality for developing with Onionprobe.
```

### Comparing `onionprobe-1.1.2/docs/assets/logo.jpg` & `onionprobe-1.2.0/docs/assets/logo.jpg`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/configurations.md` & `onionprobe-1.2.0/docs/configurations.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/installation.md` & `onionprobe-1.2.0/docs/installation.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 A package should be available for [Debian bookworm][].
 
     sudo apt-get install onionprobe
 
 An Arch Linux package is [available on AUR][][^arch-linux-package]:
 
-It's also possible to run it directly from the Git repository:
+It's also possible to run it directly from the [Git repository][]:
 
     git clone https://gitlab.torproject.org/tpo/onion-services/onionprobe
     cd onionprobe
 
 [Debian bookworm]: https://www.debian.org/releases/bookworm/
 [available on AUR]: https://aur.archlinux.org/packages/onionprobe-git
 [^arch-linux-package]: See also https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/issues/16
+[Git repository]: https://gitlab.torproject.org/tpo/onion-services/onionprobe
```

### Comparing `onionprobe-1.1.2/docs/references.md` & `onionprobe-1.2.0/docs/references.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/requirements.md` & `onionprobe-1.2.0/docs/requirements.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/slides/Makefile` & `onionprobe-1.2.0/docs/slides/Makefile`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/standalone.md` & `onionprobe-1.2.0/docs/standalone.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 * A [Grafana](https://grafana.com) Dashboard is available for browsing the
   metrics and using a PostgreSQL service container as the database backend.
 
 ## Configuring the monitoring node
 
 By default, the monitoring node periodically compiles the Onionprobe configuration
 from the official Tor Project Onion Services into `contrib/tpo.yaml`, by using
-the [tpo.py script][packages.tpo].
+the [tpo.py script][].
 
 This and other configurations can be changed by creating an `.env` file in the
 toplevel project folder.
 
 Check the [sample .env][] for an example.
 
+[tpo.py script]: api/helpers.md#tpo
 [sample .env]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/blob/main/configs/env.sample
 
 ## Starting the monitoring node
 
 The monitoring node may be started using `docker-compose`:
 
     docker-compose up -d   # Remove "-d" to not fork into the background
@@ -65,21 +66,21 @@
 
 You can protect them by [setting up Client
 Authorization](https://community.torproject.org/onion-services/advanced/client-auth/):
 
 0. Enter in the `tor` service container: `docker exec -ti onionprobe_tor_1 /bin/bash`.
 1. Setup your client credentials [according to the docs](https://community.torproject.org/onion-services/advanced/client-auth/).
    The `tor` service container already comes with all programs to generate it.
-   Onionprobe ships with a handy
-   [generate-auth-keys-for-all-onion-services](scripts/generate-auth-keys-for-all-onion-services)
+   Onionprobe ships with a handy [generate-auth-keys-for-all-onion-services][]
    available at the `tor` service container and which can be invoked with
-  `docker exec -ti onionprobe_tor_1 /usr/local/bin/generate-auth-keys-for-all-onion-services`
-  (it also accepts an optional auth name parameter allowing multiple credentials to be deployed).
+   `docker exec -ti onionprobe_tor_1
+   /usr/local/bin/generate-auth-keys-for-all-onion-services`
+   (it also accepts an optional auth name parameter allowing multiple credentials to be deployed).
 2. Place the `.auth` files at the Onion Services `authorized_clients` folder if you did not
-   created them with the `generate-auth-keys-for-all-onion-services` script:
+   create them with the `generate-auth-keys-for-all-onion-services` script:
     * Prometheus: `/var/lib/tor/prometheus/authorized_clients`.
     * Alertmanager: `/var/lib/tor/alertmanager/authorized_clients`.
     * Grafana: `/var/lib/tor/grafana/authorized_clients`.
     * Onionprobe: `/var/lib/tor/onionprobe/authorized_clients`.
 3. Restart the `tor` service container from the host to ensure that this new
    configuration is applied:
 
@@ -87,31 +88,47 @@
         docker compose up -d
 
 Note that the Grafana dashboard also comes with it's own user management system,
 whose default user and password is `admin`. You might change this default user
 and not setup the Client Authorization for Grafana, or maybe use both depending
 or your security needs.
 
+[generate-auth-keys-for-all-onion-services]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/blob/main/scripts/generate-auth-keys-for-all-onion-services
+
 ## Managing the monitoring node with systemd
 
 The monitoring node can be managed with systemd.
 A [sample service file][] is provided
 and can be adapted..
 
 [sample service file]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/blob/main/configs/systemd/onionprobe-monitor.service
 
 ## Using the monitoring node
 
 Once your monitoring node is up and running, you can create your dashboards an
 visualizations as usual, getting the data compiled by Onionprobe using
 Prometheus as the data source.
 
-Grafana already comes with a basic default dashboard as it's homepage:
+Grafana already comes with a basic default dashboard as it's homepage.
+
+Overview:
+
+![](assets/dashboard/overview.png "Grafana Dashboard - Overview")
+
+Onion Service latency:
+
+![](assets/dashboard/latency.png "Grafana Dashboard - Latency")
+
+Onion Service descriptors:
+
+![](assets/dashboard/descriptors.png "Grafana Dashboard - Descriptors")
+
+Introduction Points:
 
-![](assets/dashboard.png "Grafana Onion Services Dashboard")
+![](assets/dashboard/intros.png "Grafana Dashboard - Introduction Points")
 
 ## Enabling Tor's Prometheus metrics exporter
 
 For debugging and research purposes, Onionprobe support Tor's `MetricsPort` and
 `MetricsPortPolicy` configuration parameters, along with a Prometheus,
 Alertmanager and Grafana integrations.
```

### Comparing `onionprobe-1.1.2/docs/structure.md` & `onionprobe-1.2.0/docs/structure.md`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/docs/usage.md` & `onionprobe-1.2.0/docs/usage.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 be invoked with:
 
     onionprobe -c configs/tor.yaml
 
 By default, Onionprobe starts it's own Tor daemon instance, so the `tor` binary
 must be available in the system.
 
-See the [manual page](man/onionprobe.1.md) for the complete list of options and
+See the [manual page](man/README.md) for the complete list of options and
 available metrics.
 
 [detailed sample config]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/blob/main/configs/tor.yaml
```

### Comparing `onionprobe-1.1.2/kvmxfile` & `onionprobe-1.2.0/kvmxfile`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Sample kvmx file - https://0xacab.org/rhatto/kvmx
 #
 
 # Hostname
 hostname="onionprobe"
 
 # Which base box you should use. Leave unconfigured to use kvmx-create instead.
-#basebox="bullseye"
+#basebox="bookworm"
 
 # First user name
 user="user"
 
 # First user password
 password="`head -c 40 /dev/urandom | base64`"
 
@@ -174,15 +174,15 @@
 # Domain
 domain="example.org"
 
 # System arch
 arch="amd64"
 
 # Box distribution when bootstraping a new image
-version="bullseye"
+version="bookworm"
 
 # Debian mirror
 mirror="https://deb.debian.org/debian/"
 
 # Memory
 memory="2048"
```

### Comparing `onionprobe-1.1.2/onionprobe` & `onionprobe-1.2.0/onionprobe`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/manpage.py` & `onionprobe-1.2.0/packages/manpage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Generates Onionprobe manpage from CLI usage and templates.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -59,18 +59,21 @@
     Produces the manpage in Markdown format.
 
     Apply argument parser usage and help into a template.
 
     """
 
     # Set inputs and outputs
-    template   = os.path.join(basepath, 'docs', 'man', 'onionprobe.1.md.tmpl')
-    output     = os.path.join(basepath, 'docs', 'man', 'onionprobe.1.md')
+    template   = os.path.join(basepath, 'docs', 'man', 'onionprobe.1.txt.tmpl')
+    output     = os.path.join(basepath, 'docs', 'man', 'onionprobe.1.txt')
     config     = os.path.join(basepath, 'configs', 'tor.yaml')
 
+    # Assume a 80 columm terminal to compile the usage and help texts
+    os.environ["COLUMNS"] = "80"
+
     # Initialize the command line parser
     parser     = cmdline_parser()
 
     # Compile template variables
     usage      = remove_usage_prefix(parser.format_usage())
     invocation = remove_usage_prefix(format_as_markdown_verbatim(parser.format_help()))
     date       = datetime.datetime.now().strftime('%b %d, %Y')
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/app.py` & `onionprobe-1.2.0/packages/onionprobe/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -93,22 +93,23 @@
     :param args: Instance arguments.
     """
 
     # Register signal handling
     #signal.signal(signal.SIGINT, finish_handler)
     signal.signal(signal.SIGTERM, finish_handler)
 
+    # Exit status (shell convention means 0 is success, failure otherwise)
     status = 0
 
     # Dispatch
     try:
         probe = Onionprobe(args)
 
         if probe.initialize() is not False:
-            probe.run()
+            status = 0 if probe.run() else 1
         else:
             status = 1
 
             print('Error: could not initialize')
 
     # Handle user interruption
     # See https://stackoverflow.com/questions/21120947/catching-keyboardinterrupt-in-python-during-program-shutdown
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/certificate.py` & `onionprobe-1.2.0/packages/onionprobe/certificate.py`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/packages/onionprobe/config.py` & `onionprobe-1.2.0/packages/onionprobe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Handle Onionprobe configurations.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -27,15 +27,15 @@
 except ImportError:
     print("Please install pyaml first!")
     raise ImportError
 
 # The Onionprobe version string
 # Uses Semantic Versioning 2.0.0
 # See https://semver.org
-onionprobe_version = '1.1.2'
+onionprobe_version = '1.2.0'
 
 # The base path for this project
 basepath = os.path.join(os.path.dirname(os.path.abspath(__file__)), os.pardir, os.pardir) + os.sep
 
 # Describe configuration options
 config = {
         'log_level': {
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/http.py` & `onionprobe-1.2.0/packages/onionprobe/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -131,15 +131,15 @@
 
         try:
             self.log('Trying to connect to {} (attempt {})...'.format(url, attempt))
             self.inc_metric('onion_service_fetch_requests_total', 1, labels)
 
             # Fetch results and calculate the elapsed time
             result  = requests.get(url, proxies=proxies, timeout=timeout, verify=tls_verify)
-            elapsed = self.elapsed(init_time, True)
+            elapsed = self.elapsed(init_time, True, "HTTP fetch")
 
             # Update metrics
             self.set_metric('onion_service_latency_seconds', elapsed, labels)
 
         except requests.exceptions.TooManyRedirects as e:
             result    = False
             exception = 'too_many_redirects'
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/init.py` & `onionprobe-1.2.0/packages/onionprobe/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/logger.py` & `onionprobe-1.2.0/packages/onionprobe/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/metrics.py` & `onionprobe-1.2.0/packages/onionprobe/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -110,20 +110,76 @@
     'onion_service_descriptor_fetch_attempts': Gauge(
             'onion_service_descriptor_fetch_attempts',
             "Register the number of attempts required when trying to get an " + \
                     "Onion Service descriptor in a probing round",
             ['name', 'address', 'reachable']
         ),
 
+    'onion_service_descriptor_revision_counter': Gauge(
+            'onion_service_descriptor_revision_counter',
+            'Register Onion Service descriptor revision counter',
+            ['name', 'address']
+        ),
+
+    'onion_service_descriptor_lifetime_seconds': Gauge(
+            'onion_service_descriptor_lifetime_seconds',
+            'Register Onion Service descriptor lifetime in seconds',
+            ['name', 'address']
+        ),
+
+    'onion_service_descriptor_outer_wrapper_size_bytes': Gauge(
+            'onion_service_descriptor_outer_wrapper_size_bytes',
+            'Register Onion Service outer wrapper descriptor size in bytes (decrypted)',
+            ['name', 'address']
+        ),
+
+    'onion_service_descriptor_second_layer_size_bytes': Gauge(
+            'onion_service_descriptor_second_layer_size_bytes',
+            'Register Onion Service second layer descriptor size in bytes (decrypted)',
+            ['name', 'address']
+        ),
+
+    'onion_service_is_single': Gauge(
+            'onion_service_is_single',
+            "Indicates whether the server is using the single hop Onion Service circuit mode: value is " + \
+                    "1 if this is a single onion service, 0 otherwise",
+            ['name', 'address']
+        ),
+
     'onion_service_introduction_points_number': Gauge(
             'onion_service_introduction_points_number',
             'Register the number of introduction points in the Onion Service descriptor',
             ['name', 'address']
         ),
 
+    'onion_service_pow_enabled': Gauge(
+            'onion_service_pow_enabled',
+            "Whether Proof of Work (PoW) defense is enabled in the Onion Service: value is " + \
+                    "1 when PoW is enabled, 0 otherwise",
+            ['name', 'address']
+        ),
+
+    'onion_service_pow_v1_seed': Gauge(
+            'onion_service_pow_v1_seed',
+            'The Proof of Work (PoW) decoded seed for the v1 scheme',
+            ['name', 'address']
+        ),
+
+    'onion_service_pow_v1_effort': Gauge(
+            'onion_service_pow_v1_effort',
+            'The Proof of Work (PoW) suggested effort for the v1 scheme',
+            ['name', 'address']
+        ),
+
+    'onion_service_pow_v1_expiration_seconds': Gauge(
+            'onion_service_pow_v1_expiration_seconds',
+            'The Proof of Work (PoW) seed expiration time for the v1 scheme',
+            ['name', 'address']
+        ),
+
     'onion_service_match_pattern_matched': Gauge(
             'onion_service_pattern_matched',
             "Register whether a regular expression pattern is matched when " + \
                     "connection to the Onion Service: value is 1 for matched pattern and " + \
                     "0 otherwise",
             ['name', 'address', 'protocol', 'port', 'path', 'pattern']
         ),
@@ -164,14 +220,20 @@
             "Register whether a provided server certificate matches the server hostname " + \
             "in a TLS connection: value is 1 for matched hostname and 0 otherwise. " + \
             "Check is done both on the commonName and subjectAltName fields. " + \
             "A value of 1 does not mean necessarily that the certificate is CA-validated.",
             ['name', 'address', 'port']
         ),
 
+    'hsdir_latency_seconds': Gauge(
+            'hsdir_latency_seconds',
+            'Register HSDir latency in seconds to fetch a descriptor',
+            ['name', 'id', ]
+        ),
+
     #
     # Probing counters
     #
 
     # Prometheus documentation says:
     #
     # > "When you have a successful request count and a failed request count, the
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/prober.py` & `onionprobe-1.2.0/packages/onionprobe/prober.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/teardown.py` & `onionprobe-1.2.0/packages/onionprobe/teardown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/time.py` & `onionprobe-1.2.0/packages/onionprobe/time.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -53,35 +53,43 @@
 
         # Sleep, collecting metrics about it
         self.log('Waiting {} seconds...'.format(str(round(value))))
         self.metrics['onionprobe_wait_seconds'].set(value)
         self.metrics['onionprobe_state'].state('sleeping')
         time.sleep(value)
 
-    def elapsed(self, init_time, verbose = False):
+    def elapsed(self, init_time, verbose = False, label = ''):
         """
         Calculate the time elapsed since an initial time.
 
         :type  init_time: datetime.datetime
         :param init_time: Initial time.
 
         :type  verbose: bol
         :param verbose: If verbose is True, logs the elapsed time.
                         Defaults to False.
 
+        :type  label: str
+        :param label: A label to add in the elapsed time log message.
+                      Only used if verbose is set to true.
+                      Defaults to an empty string.
+
         :rtype: int
         :return: Number of elapsed time in seconds
         """
 
         # Calculate the elapsed time
         elapsed = (datetime.now() - init_time)
 
         # Log the elapsed time
         if verbose:
-            self.log("Elapsed time: " + str(elapsed))
+            if label != '':
+                label = ' (' + str(label) + ')'
+
+            self.log("Elapsed time" + label + ": " + str(elapsed))
 
         return timedelta.total_seconds(elapsed)
 
     def timestamp(self):
         """
         Wrapper around datetime.now().timestamp()
```

### Comparing `onionprobe-1.1.2/packages/onionprobe/tls.py` & `onionprobe-1.2.0/packages/onionprobe/tls.py`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/packages/onionprobe/tor.py` & `onionprobe-1.2.0/packages/onionprobe/tor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Onionprobe test/monitor tool.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -50,14 +50,18 @@
         # Ensure control_address is an IP address, which is the
         # only type currently supported by stem
         #
         # Right now only IPv4 is supported
         import socket
         control_address = socket.gethostbyname(control_address)
 
+        # Workaround for https://github.com/torproject/stem/issues/112
+        if self.get_config('log_level') != 'debug':
+            stem.util.log.get_logger().propagate = False
+
         if self.get_config('launch_tor'):
             if self.launch_tor() is False:
                 self.log("Error initializing Tor", "critical")
 
                 return False
 
         try:
@@ -190,17 +194,17 @@
         # Helper function to print bootstrap lines
         def print_bootstrap_lines(line):
             level = self.get_config('log_level')
 
             if '[debug]' in line:
                 self.log(term.format(line), 'debug')
             elif '[info]' in line:
-                self.log(term.format(line), 'info')
+                self.log(term.format(line), 'debug')
             elif '[notice]' in line:
-                self.log(term.format(line), 'info')
+                self.log(term.format(line), 'debug')
             elif '[warn]' in line:
                 self.log(term.format(line), 'warning')
             elif '[err]' in line:
                 self.log(term.format(line), 'error')
 
         try:
             self.log('Initializing Tor process...')
```

### Comparing `onionprobe-1.1.2/packages/onionprobe.egg-info/PKG-INFO` & `onionprobe-1.2.0/packages/onionprobe.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onionprobe
-Version: 1.1.2
+Version: 1.2.0
 Summary: Test and monitors the status of Tor Onion Services
 Home-page: https://tpo.pages.torproject.net/onion-services/onionprobe
 Author: Silvio Rhatto
 Author-email: rhatto@torproject.org
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.27.1
 Requires-Dist: stem>=1.8.0
 Requires-Dist: prometheus-client>=0.14.1
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pysocks>=1.7.1
-Requires-Dist: cryptography==3.3.2
+Requires-Dist: cryptography>=3.4.8
 
 # Onionprobe
 
 ![](docs/assets/logo.jpg "Onionprobe")
 
 Onionprobe is a tool for testing and monitoring the status of
 [Tor Onion Services](https://community.torproject.org/onion-services/) sites.
@@ -43,8 +43,8 @@
 endpoints and paths, optionally exporting to [Prometheus](https://prometheus.io)
 and with [Grafana](https://grafana.com/) support.
 
 The full documentation is available in the [docs/][] folder and at the
 [Onionprobe website][].
 
 [docs/]: https://gitlab.torproject.org/tpo/onion-services/onionprobe/-/tree/main/docs
-[Onionprobe website]: https://tpo.pages.torproject.net/onion-services/onionprobe/
+[Onionprobe website]: https://community.torproject.org/onion-services/ecosystem/apps/web/onionprobe/
```

### Comparing `onionprobe-1.1.2/packages/onionprobe.egg-info/SOURCES.txt` & `onionprobe-1.2.0/packages/onionprobe.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Makefile
 README.md
 docker-compose.yaml
 kvmxfile
 mkdocs.yml
 onionprobe
 pyproject.toml
+renovate.json
 setup.cfg
 .github/gh-pages.yml
 configs/env.sample
 configs/onionprobe.yaml
 configs/real-world-onion-sites.yaml
 configs/securedrop.yaml
 configs/test.yaml
@@ -53,32 +54,36 @@
 debian/rules
 debian/source/format
 docs/.gitignore
 docs/.pages
 docs/README.md
 docs/acknowledgements.md
 docs/alternatives.md
+docs/changelog.md
 docs/configurations.md
+docs/development.md
 docs/installation.md
 docs/issues.md
 docs/references.md
 docs/requirements.md
 docs/standalone.md
 docs/structure.md
 docs/upgrading.md
 docs/usage.md
 docs/api/.pages
 docs/api/README.md
 docs/api/helpers.md
 docs/api/onionprobe.md
-docs/assets/dashboard.png
 docs/assets/logo.jpg
-docs/man/onionprobe.1.md
-docs/man/onionprobe.1.md.tmpl
+docs/assets/dashboard/descriptors.png
+docs/assets/dashboard/intros.png
+docs/assets/dashboard/latency.png
+docs/assets/dashboard/overview.png
 docs/slides/Makefile
+docs/slides/2022.Q1/demoday/demoday.md
 packages/manpage.py
 packages/real-world-onion-sites.py
 packages/securedrop.py
 packages/tpo.py
 packages/onionprobe/__init__.py
 packages/onionprobe/app.py
 packages/onionprobe/certificate.py
@@ -102,9 +107,10 @@
 packages/onionprobe.egg-info/top_level.txt
 scripts/generate-auth-keys-for-all-onion-services
 scripts/get-tor-debian-key
 scripts/provision
 scripts/provision-onionprobe
 scripts/provision-packaging-debian
 scripts/provision-packaging-python
+scripts/provision-packaging-sbuild
 scripts/upgrade-postgresql-database
 tests/tpo/tpo.json
```

### Comparing `onionprobe-1.1.2/packages/real-world-onion-sites.py` & `onionprobe-1.2.0/packages/real-world-onion-sites.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Compile an Onionprobe configuration file from the "Real-World Onion Sites"
 # repository.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/securedrop.py` & `onionprobe-1.2.0/packages/securedrop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Compile an Onionprobe configuration file from the Secure Drop API.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/packages/tpo.py` & `onionprobe-1.2.0/packages/tpo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Compile an Onionprobe configuration file from The Tor Project official
 # Onion Services list.
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/scripts/generate-auth-keys-for-all-onion-services` & `onionprobe-1.2.0/scripts/generate-auth-keys-for-all-onion-services`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env bash
 #
 # Generate a Client Authorization keypair and apply to all Onion Services.
 #
 # Based on https://community.torproject.org/onion-services/advanced/client-auth/
 # See also https://gist.github.com/mtigas/9c2386adf65345be34045dace134140b
 #
-# Copyright (C) 2022 Silvio Rhatto <rhatto@torproject.org>
+# Copyright (C) 2022 The Tor Project, Inc.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, either version 3 of the License,
 # or any later version.
 #
 # This program is distributed in the hope that it will be useful,
```

### Comparing `onionprobe-1.1.2/scripts/get-tor-debian-key` & `onionprobe-1.2.0/scripts/get-tor-debian-key`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/scripts/provision` & `onionprobe-1.2.0/scripts/provision`

 * *Files 24% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 $SUDO apt-get upgrade -y
 $SUDO apt-get install -y docker.io docker-compose
 
 # Put the regular user into docker group
 $SUDO usermod -a -G docker $(whoami)
 
 # Provision documentation requirements
-$BASEPATH/vendors/onion-mkdocs/scripts/provision-docs-build
-$BASEPATH/vendors/onion-tex-slim/scripts/provision-docs-build
+$BASEPATH/vendors/onion-mkdocs/scripts/onion-mkdocs-provision-build
+$BASEPATH/vendors/onion-tex-slim/scripts/onion-tex-slim-provision-build
 
 # Provision Python packaging requirements
 $DIRNAME/provision-packaging-python
 
 # Provision Debian packaging requirements
 $DIRNAME/provision-packaging-debian
```

### Comparing `onionprobe-1.1.2/scripts/provision-onionprobe` & `onionprobe-1.2.0/scripts/provision-onionprobe`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/scripts/upgrade-postgresql-database` & `onionprobe-1.2.0/scripts/upgrade-postgresql-database`

 * *Files identical despite different names*

### Comparing `onionprobe-1.1.2/setup.cfg` & `onionprobe-1.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = onionprobe
-version = 1.1.2
+version = 1.2.0
 url = https://tpo.pages.torproject.net/onion-services/onionprobe
 author = Silvio Rhatto
 author_email = rhatto@torproject.org
 license = GPLv3
 description = Test and monitors the status of Tor Onion Services
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -32,27 +32,27 @@
 	= packages
 install_requires = 
 	requests >= 2.27.1
 	stem >= 1.8.0
 	prometheus-client >= 0.14.1
 	pyyaml >= 6.0
 	pysocks >= 1.7.1
-	cryptography == 3.3.2
+	cryptography >= 3.4.8
 python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	onionprobe = onionprobe.app:run_from_cmdline
 
 [options.data_files]
-onionprobe/configs/ = 
+share/onionprobe/configs/ = 
 	configs/tor.yaml
 	configs/real-world-onion-sites.yaml
 	configs/securedrop.yaml
-onionprobe/examples/ = 
+share/onionprobe/examples/ = 
 	packages/real-world-onion-sites.py
 	packages/securedrop.py
 	packages/tpo.py
 
 [options.packages.find]
 where = packages
```

### Comparing `onionprobe-1.1.2/tests/tpo/tpo.json` & `onionprobe-1.2.0/tests/tpo/tpo.json`

 * *Files identical despite different names*

