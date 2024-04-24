# Comparing `tmp/jupyter_environment_manager-0.2.0rc8.tar.gz` & `tmp/jupyter_environment_manager-0.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_environment_manager-0.2.0rc8.tar", last modified: Wed Apr 17 16:41:04 2024, max compression
+gzip compressed data, was "jupyter_environment_manager-0.2.0rc9.tar", last modified: Fri Apr 19 22:02:51 2024, max compression
```

## Comparing `jupyter_environment_manager-0.2.0rc8.tar` & `jupyter_environment_manager-0.2.0rc9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/install.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.968308 jupyter_environment_manager-0.2.0rc8/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.976308 jupyter_environment_manager-0.2.0rc8/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter-config/nb-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.976308 jupyter_environment_manager-0.2.0rc8/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter-config/server-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.980308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_pkgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.980308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.996308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   195536 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js
--rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
--rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
--rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
--rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 16:40:13.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:38:28.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-17 16:38:16.000000 jupyter_environment_manager-0.2.0rc8/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.000308 jupyter_environment_manager-0.2.0rc8/src/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/EnvironmentsSidebarWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/Flux.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.000308 jupyter_environment_manager-0.2.0rc8/src/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/ApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/AuthActions.js
--rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/EnvironmentActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/JupyterApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/UserActions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.968308 jupyter_environment_manager-0.2.0rc8/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.004308 jupyter_environment_manager-0.2.0rc8/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/BackIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/CloseIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/ConfirmIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/DescriptionIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/EnvIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/IconString.js
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/LinkIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/Loading.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/RefreshIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/SearchIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/UserIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/WhiteCube.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.008308 jupyter_environment_manager-0.2.0rc8/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EndUserAgreement.js
--rw-r--r--   0 runner    (1001) docker     (127)    97122 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentEditor.js
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentTile.js
--rw-r--r--   0 runner    (1001) docker     (127)    96041 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentsSidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/Loading.js
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/LogoLoader.js
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/MuiStyledComponents.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/UserNotFound.js
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/contextTypes.js
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/global.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.012308 jupyter_environment_manager-0.2.0rc8/src/stores/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/AuthStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/EnvironmentStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/UserStore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.012308 jupyter_environment_manager-0.2.0rc8/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/utils/googleAnalytics.js
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/utils/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.016308 jupyter_environment_manager-0.2.0rc8/style/
--rw-r--r--   0 runner    (1001) docker     (127)    19395 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentEditor.css
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentTile.css
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentsSidebar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/Loading.css
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/LogoLoader.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/base.css
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/index.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tools/stamp_pre_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/install.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.890205 jupyter_environment_manager-0.2.0rc9/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.902205 jupyter_environment_manager-0.2.0rc9/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter-config/nb-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.902205 jupyter_environment_manager-0.2.0rc9/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter-config/server-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.910205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_pkgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.910205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.930205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   202661 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 22:02:02.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:01:42.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-19 22:01:29.000000 jupyter_environment_manager-0.2.0rc9/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.930205 jupyter_environment_manager-0.2.0rc9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/EnvironmentsSidebarWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/Flux.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.934205 jupyter_environment_manager-0.2.0rc9/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/ApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/AuthActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29226 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/EnvironmentActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/JupyterApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/UserActions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.894205 jupyter_environment_manager-0.2.0rc9/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.942205 jupyter_environment_manager-0.2.0rc9/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/BackIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/CloseIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/ConfirmIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/DescriptionIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/EnvIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/IconString.js
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/LinkIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/Loading.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/RefreshIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/SearchIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/UserIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/WhiteCube.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.946205 jupyter_environment_manager-0.2.0rc9/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EndUserAgreement.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107258 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentEditor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentTile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    99350 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentsSidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/LogoLoader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/MuiStyledComponents.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/UserNotFound.js
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/contextTypes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/global.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.946205 jupyter_environment_manager-0.2.0rc9/src/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/AuthStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/EnvironmentStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/UserStore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.950205 jupyter_environment_manager-0.2.0rc9/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/utils/googleAnalytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/utils/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.950205 jupyter_environment_manager-0.2.0rc9/style/
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentEditor.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentTile.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentsSidebar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/Loading.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/LogoLoader.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tools/stamp_pre_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/yarn.lock
```

### Comparing `jupyter_environment_manager-0.2.0rc8/CONTRIBUTING.md` & `jupyter_environment_manager-0.2.0rc9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/LICENSE` & `jupyter_environment_manager-0.2.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/MANIFEST.in` & `jupyter_environment_manager-0.2.0rc9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/PKG-INFO` & `jupyter_environment_manager-0.2.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
@@ -12,14 +12,15 @@
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
@@ -29,15 +30,15 @@
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server<2,>=1.6
 Requires-Dist: jupyter_client~=7.1.0
 Requires-Dist: tornado>=6.1.0
 Requires-Dist: notebook<7
-Requires-Dist: qbraid-core<0.2,>=0.1.3
+Requires-Dist: qbraid-core<0.2,>=0.1.4.dev1
 
 # jupyter-environment-manager
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html)
 [![PyPI version](https://img.shields.io/pypi/v/jupyter-environment-manager.svg?color=blue)](https://pypi.org/project/jupyter-environment-manager/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/TPBU2sa8Et)
```

### Comparing `jupyter_environment_manager-0.2.0rc8/README.md` & `jupyter_environment_manager-0.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/__init__.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/_version.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/configure.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/configure.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import time
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 import tornado
 from notebook.base.handlers import APIHandler
+from qbraid_core.config import USER_CONFIG_PATH
 from qbraid_core.system.executables import is_valid_python
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
@@ -35,33 +36,31 @@
     def get(self):
         """Get locally stored credentials from qbraidrc."""
         credentials = self.read_qbraidrc()
         self.finish(json.dumps(credentials))
 
     def read_qbraidrc(self):
         """Read the qbraidrc file and return the contents as a dictionary."""
-        home = os.getenv("HOME") or os.path.expanduser("~")
-        filepath = os.path.join(home, ".qbraid", "qbraidrc")
         config = configparser.ConfigParser()
 
         # Dictionary to store the results
         result = {
             "pythonVersion": self.get_python_version(),
             "email": os.getenv("JUPYTERHUB_USER"),
             "apiKey": os.getenv("QBRAID_API_KEY"),
             "refreshToken": os.getenv("REFRESH"),
             "url": "https://api.qbraid.com/api",
         }
 
         # Check if the file exists
-        if not os.path.exists(filepath):
+        if not os.path.exists(USER_CONFIG_PATH):
             return result
 
         # Read the configuration file
-        config.read(filepath)
+        config.read(USER_CONFIG_PATH)
 
         # Extract email and refresh-token
         if "default" in config:
             result["url"] = config["default"].get("url", result["url"])
             result["email"] = config["default"].get("email", result["email"])
             result["apiKey"] = config["default"].get("api-key", result["apiKey"])
             result["refreshToken"] = config["default"].get("refresh-token", result["refreshToken"])
@@ -99,18 +98,15 @@
         try:
             Path(filepath).unlink()
         except (FileNotFoundError, OSError) as err:
             logging.error("Error deleting file: %s", err)
 
     @staticmethod
     def get_python_version(python_path: Optional[str] = None) -> str:
-        """Gets the Python version of the given executable.
-
-        # TODO: replace with qbraid.api.system.get_python_version_from_exe
-        """
+        """Gets the Python version of the given executable."""
         executable = python_path or sys.executable
         if not is_valid_python(executable):
             raise ValueError(f"Invalid Python executable: {executable}")
 
         try:
             result = subprocess.run(
                 [executable, "--version"], capture_output=True, text=True, check=True
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/devices.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/devices.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_create.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_create.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 
 import base64
 import json
 import logging
 import os
 import re
 import shutil
-import subprocess
 import sys
 import threading
 from pathlib import Path
 
 import tornado
 from jupyter_client.kernelspec import KernelSpecManager
 from notebook.base.handlers import APIHandler
+from qbraid_core.services.environments.create import create_local_venv
 from qbraid_core.services.environments.paths import DEFAULT_LOCAL_ENVS_PATH
 from qbraid_core.services.environments.state import update_install_status
-from qbraid_core.system.generic import replace_str
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 
@@ -46,15 +45,15 @@
         os.makedirs(local_resource_dir, exist_ok=True)
 
         try:
             # create state.json
             update_install_status(slug_path, 0, 0)
 
             # create python venv
-            thread = threading.Thread(target=self.create_venv, args=(slug_path, prompt))
+            thread = threading.Thread(target=create_local_venv, args=(slug_path, prompt))
             thread.start()
 
             # create kernel.json
             kernel_json_path = os.path.join(local_resource_dir, "kernel.json")
             kernel_spec_manager = KernelSpecManager()
             kernelspec_dict = kernel_spec_manager.get_all_specs()
             kernel_data = kernelspec_dict["python3"]["spec"]
@@ -99,30 +98,7 @@
 
         # Ensure the output directory exists
         Path(output_path).parent.mkdir(parents=True, exist_ok=True)
 
         # Write the image data to a file
         with open(output_path, "wb") as file:
             file.write(image_data)
-
-    def create_venv(self, slug_path: str, prompt: str) -> None:
-        """Create virtual environment and swap PS1 display name."""
-        try:
-            venv_path = os.path.join(slug_path, "pyenv")
-            subprocess.run([sys.executable, "-m", "venv", venv_path], check=True)
-
-            # Determine the correct directory for activation scripts based on the operating system
-            if sys.platform == "win32":
-                scripts_path = os.path.join(venv_path, "Scripts")
-                activate_files = ["activate.bat", "Activate.ps1"]
-            else:
-                scripts_path = os.path.join(venv_path, "bin")
-                activate_files = ["activate", "activate.csh", "activate.fish"]
-
-            for file in activate_files:
-                file_path = os.path.join(scripts_path, file)
-                replace_str("(pyenv)", f"({prompt})", file_path)
-
-            update_install_status(slug_path, 1, 1)
-        except Exception as err:  # pylint: disable=broad-exception-caught
-            logging.error("Error creating virtual environment: %s", err)
-            update_install_status(slug_path, 1, 0, message=str(err))
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_list.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,17 @@
     get_default_envs_paths,
     get_env_path,
     get_next_tmpn,
     get_tmp_dir_names,
     which_python,
 )
 from qbraid_core.services.environments.state import install_status_codes
-from qbraid_core.system.executables import is_valid_python
-from qbraid_core.system.generic import replace_str
+from qbraid_core.services.environments.validate import is_valid_slug
+from qbraid_core.system.executables import is_valid_python, python_paths_equivalent
+from qbraid_core.system.packages import set_include_sys_site_pkgs_value
 
 from .jobs import quantum_jobs_supported_enabled
 from .kernels import get_kernels
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
@@ -169,29 +170,29 @@
 
     return pip_list
 
 
 def put_pip_list(slug: str, system_site_packages: Optional[bool] = True) -> List[str]:
     """Update/insert requirements.txt and return pip list."""
     python = which_python(slug)
-    if is_valid_python(python) and python != sys.executable:
+    if is_valid_python(python) and not python_paths_equivalent(python, sys.executable):
         slug_path = str(get_env_path(slug))
         cfg = os.path.join(slug_path, "pyenv", "pyvenv.cfg")
         reqs_txt = os.path.join(slug_path, "requirements.txt")
-        replace_str("true", "false", cfg)
+        set_include_sys_site_pkgs_value(False, cfg)
         with open(reqs_txt, "w", encoding="utf-8") as file:
             subprocess.run(
                 [python, "-m", "pip", "freeze"],
                 stdout=file,
                 text=True,
                 check=True,
             )
         _rewrite_requirements_file(reqs_txt)
         if system_site_packages:
-            replace_str("false", "true", cfg)
+            set_include_sys_site_pkgs_value(True, cfg)
 
     return get_pip_list(slug)
 
 
 class PipListEnvironmentHandler(APIHandler):
     """Handler for managing environment package list data."""
 
@@ -244,15 +245,16 @@
                 # Skip if the path is not a directory or if it's not a valid slug directory
                 if not self.validate_slug_env(slug_path) or slug in uninstalling:
                     continue
 
                 # Add to installed environments list
                 installed.append(slug)
 
-                if which_python(slug) == sys.executable:
+                env_python = which_python(slug)
+                if python_paths_equivalent(env_python, sys.executable):
                     sys_python.append(slug)
 
                 # Check if the environment is active
                 if self.is_active(slug_path, kernels_list):
                     active.append(slug)
 
                 # Initialize 'installing' status if it's None
@@ -305,15 +307,15 @@
         for cancel install environment.
 
         """
         if not os.path.isdir(slug_path):
             return False
 
         slug = os.path.basename(slug_path)
-        if len(slug) <= 7 or len(slug) > 20 or slug[-7] != "_":
+        if not is_valid_slug(slug):
             return False
 
         persistent_files = ["state.json", "install_status.txt"]
         if any(os.path.isfile(os.path.join(slug_path, file)) for file in persistent_files):
             return True
 
         if os.path.dirname(slug_path) == str(DEFAULT_LOCAL_ENVS_PATH):
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_pkgs.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_pkgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from notebook.base.handlers import APIHandler
 from qbraid_core.services.environments.paths import (
     DEFAULT_LOCAL_ENVS_PATH,
     get_env_path,
     which_python,
 )
 from qbraid_core.services.environments.state import update_install_status
-from qbraid_core.system.generic import replace_str
+from qbraid_core.system.executables import python_paths_equivalent
+from qbraid_core.system.packages import set_include_sys_site_pkgs_value
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 
@@ -88,23 +89,23 @@
 
         reqs_tmp = os.path.join(slug_path, "reqs_tmp.txt")
         install_command = [python, "-m", "pip", "install", "-r", reqs_tmp]
         with open(reqs_tmp, "w", encoding="utf-8") as file:
             for package in packages:
                 file.write(package + "\n")
 
-        if python == sys.executable:
+        if python_paths_equivalent(python, sys.executable):
             result = subprocess.run(install_command, capture_output=True, check=False)
         else:
             cfg = os.path.join(slug_path, "pyenv", "pyvenv.cfg")
-            replace_str("true", "false", cfg)
+            set_include_sys_site_pkgs_value(False, cfg)
             # Run the command and capture stderr
             result = subprocess.run(install_command, capture_output=True, check=False)
             if system_site_packages:
-                replace_str("false", "true", cfg)
+                set_include_sys_site_pkgs_value(True, cfg)
         stderr_msg = result.stderr.decode("utf-8")
         stdout_msg = result.stdout.decode("utf-8")
         install_msg += stderr_msg + stdout_msg.strip("\n").split("\n")[-1]
         try:
             os.remove(reqs_tmp)
         except FileNotFoundError as err:
             logging.error("Error removing tmp file: %s", err)
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_remove.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_remove.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_state.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_state.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/handlers.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/kernels.py` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/kernels.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/package.json` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.5fd255ae2892e93a3890.js'}}",*

 * * "'version'": "'0.2.0-rc.9'"}*

```diff
@@ -51,15 +51,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.64b15d2280d9c5210de7.js",
+            "load": "static/remoteEntry.5fd255ae2892e93a3890.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_environment_manager"
                 },
@@ -112,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.8"
+    "version": "0.2.0-rc.9"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,17 +4,17 @@
         4185: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Fe
             });
             var i = n(6880),
                 a = n(6271),
                 s = n.n(a),
-                r = n(7583),
-                o = n(5697),
-                l = n.n(o);
+                o = n(7583),
+                r = n(5697),
+                l = n.n(r);
             const c = {
                 getActions: l().func,
                 getStore: l().func,
                 apiBaseUrl: l().string,
                 jupyterlab: l().any
             };
             var d = n(3508),
@@ -157,16 +157,16 @@
                     super(e, t), this.toggleCollapsed = e => {
                         const {
                             isInstalled: t,
                             packageInstallingEnv: n,
                             environment: i,
                             isInstalling: a,
                             expandedEnvs: s
-                        } = this.props, r = (null == i ? void 0 : i.isExpanded) || (null == s ? void 0 : s.includes(e)), o = n === e, l = i.sysPython;
-                        a || !t || !r || o || l || this.props.flux.getActions("EnvironmentActions").updatePackagesList(e).catch((e => {
+                        } = this.props, o = null == s ? void 0 : s.includes(e), r = n === e, l = i.sysPython;
+                        a || !t || !o || r || l || this.props.flux.getActions("EnvironmentActions").updatePackagesList(e).catch((e => {
                             console.log("Error at update package in toggle collapsed at envTile ", e)
                         })), this.props.onToggleExpand(e)
                     }, this.renderVerifyLoader = () => s().createElement(v.Box, {
                         position: "absolute",
                         width: "100%",
                         height: "100%",
                         className: "env_verification-loader",
@@ -217,56 +217,56 @@
                             lockedTile: !1
                         }) : Object.assign(Object.assign({}, t), {
                             lockedTile: !0
                         })
                     }
                 }
                 render() {
-                    var e, t, n, i, a, r, o, l, c, m;
-                    let g = this.props.environment,
+                    var e, t, n, i, a, o, r, l, c, m, g, u;
+                    let b = this.props.environment,
                         {
-                            user: u
+                            user: f
                         } = this.props.qbUser,
-                        b = {};
-                    return this.props.isActive && (b.backgroundColor = "#dad4e7", b.border = "1px solid #673ab7"), this.state.lockedTile && (b.border = "none"), g.isExpanded || this.props.isNewEnv || (null === (e = this.props.expandedEnvs) || void 0 === e ? void 0 : e.includes(g._id)) ? (b.maxHeight = 9999, b.padding = "0 10px 60px 10px") : (b.maxHeight = 0, b.padding = "0 10px 40px 10px"), s().createElement("div", {
+                        x = {};
+                    return this.props.isActive && (x.backgroundColor = "#dad4e7", x.border = "1px solid #673ab7"), this.state.lockedTile && (x.border = "none"), this.props.isNewEnv || (null === (e = this.props.expandedEnvs) || void 0 === e ? void 0 : e.includes(b._id)) ? (x.maxHeight = 9999, x.padding = "0 10px 60px 10px") : (x.maxHeight = 0, x.padding = "0 10px 40px 10px"), s().createElement("div", {
                         className: "env-tile",
-                        style: Object.assign({}, b)
+                        style: Object.assign({}, x)
                     }, s().createElement("div", {
-                        className: `env-name flex-box ${(this.props.isNewEnv||g.isExpanded||(null===(t=this.props.expandedEnvs)||void 0===t?void 0:t.includes(g._id)))&&"env-name-border"}`,
+                        className: `env-name flex-box ${(this.props.isNewEnv||(null===(t=this.props.expandedEnvs)||void 0===t?void 0:t.includes(b._id)))&&"env-name-border"}`,
                         style: {
                             color: this.props.isActive ? "black" : "var(--jp-ui-font-color0)"
                         }
                     }, s().createElement("span", {
                         className: "env-tile-display-name flex-box_start",
                         style: {
                             cursor: "pointer"
                         },
-                        onClick: () => this.toggleCollapsed(g._id)
-                    }, (null == g ? void 0 : g.logo) && "object" == typeof(null == g ? void 0 : g.logo) && !Array.isArray(null == g ? void 0 : g.logo) && null !== (null == g ? void 0 : g.logo) ? s().createElement("span", {
-                        onClick: () => this.toggleCollapsed(g._id)
+                        onClick: () => this.toggleCollapsed(b._id)
+                    }, (null == b ? void 0 : b.logo) && "object" == typeof(null == b ? void 0 : b.logo) && !Array.isArray(null == b ? void 0 : b.logo) && null !== (null == b ? void 0 : b.logo) ? s().createElement("span", {
+                        onClick: () => this.toggleCollapsed(b._id)
                     }, s().createElement("img", {
                         style: {
                             height: 18,
                             maxWidth: 45,
                             marginRight: 5
                         },
-                        src: (null === (n = null == this ? void 0 : this.props) || void 0 === n ? void 0 : n.isDarkTheme) ? g.logo.dark : g.logo.light
+                        src: (null === (n = null == this ? void 0 : this.props) || void 0 === n ? void 0 : n.isDarkTheme) ? b.logo.dark : b.logo.light
                     })) : s().createElement("span", {
-                        onClick: () => this.toggleCollapsed(g._id)
+                        onClick: () => this.toggleCollapsed(b._id)
                     }, s().createElement("img", {
                         key: 0,
                         style: {
                             height: 18,
                             maxWidth: 45,
                             marginRight: 5
                         },
-                        src: localStorage.getItem(g.displayName) || (null === (i = null == this ? void 0 : this.props) || void 0 === i ? void 0 : i.isDarkTheme) ? g.logo.dark : g.logo.light
+                        src: localStorage.getItem(b.displayName) || (null === (i = null == this ? void 0 : this.props) || void 0 === i ? void 0 : i.isDarkTheme) ? null === (a = null == b ? void 0 : b.logo) || void 0 === a ? void 0 : a.dark : null === (o = null == b ? void 0 : b.logo) || void 0 === o ? void 0 : o.light
                     })), s().createElement("p", {
                         className: "env-tile-display-name"
-                    }, g.displayName), this.state.lockedTile && s().createElement(v.Tooltip, {
+                    }, b.displayName), this.state.lockedTile && s().createElement(v.Tooltip, {
                         title: this.props.isInstalled ? "Upgrade to access environment" : "Upgrade to install environment",
                         arrow: !0
                     }, s().createElement(p.Z, {
                         sx: {
                             fontSize: "1rem!important",
                             color: "var(--jp-ui-font-color0)",
                             marginLeft: "5px",
@@ -274,60 +274,60 @@
                             cursor: "pointer"
                         }
                     }))), s().createElement("span", {
                         className: "env-tile_right-flex-box"
                     }, this.props.isActive && s().createElement("span", {
                         className: "env-tile-active-label"
                     }, "active"), s().createElement("img", {
-                        src: g.pinned ? "https://qbraid-static.s3.amazonaws.com/bookmark-solid-pink.svg" : "https://qbraid-static.s3.amazonaws.com/bookmark-solid-gray.svg",
+                        src: b.pinned ? "https://qbraid-static.s3.amazonaws.com/bookmark-solid-pink.svg" : "https://qbraid-static.s3.amazonaws.com/bookmark-solid-gray.svg",
                         style: {
                             width: 15,
                             height: 15,
                             cursor: this.state.lockedTile ? "not-allowed" : "pointer"
                         },
                         onClick: () => {
-                            this.state.lockedTile || this.props.onTogglePinned(g._id)
+                            this.state.lockedTile || this.props.onTogglePinned(b._id)
                         }
                     }), s().createElement(d.Z, {
                         sx: {
                             fontSize: "1rem!important",
-                            transform: this.props.isNewEnv || g.isExpanded || (null === (a = this.props.expandedEnvs) || void 0 === a ? void 0 : a.includes(g._id)) ? "rotateX(180deg)" : "rotateX(0deg)",
+                            transform: this.props.isNewEnv || (null === (r = this.props.expandedEnvs) || void 0 === r ? void 0 : r.includes(b._id)) ? "rotateX(180deg)" : "rotateX(0deg)",
                             transition: "transform 300ms ease",
                             cursor: "pointer",
                             zIndex: "99"
                         },
-                        onClick: () => this.toggleCollapsed(g._id)
+                        onClick: () => this.toggleCollapsed(b._id)
                     }))), s().createElement("span", {
                         style: {
-                            visibility: g.isExpanded || this.props.isNewEnv || (null === (r = this.props.expandedEnvs) || void 0 === r ? void 0 : r.includes(g._id)) ? "visible" : "hidden"
+                            visibility: this.props.isNewEnv || (null === (l = this.props.expandedEnvs) || void 0 === l ? void 0 : l.includes(b._id)) ? "visible" : "hidden"
                         }
                     }, s().createElement("div", {
                         className: "env-content"
-                    }, (null === (l = null === (o = this.props) || void 0 === o ? void 0 : o.verifyLoading) || void 0 === l ? void 0 : l.loading) && (null === (m = null === (c = this.props) || void 0 === c ? void 0 : c.verifyLoading) || void 0 === m ? void 0 : m.envId) === g._id && this.renderVerifyLoader(), s().createElement("div", {
+                    }, (null === (m = null === (c = this.props) || void 0 === c ? void 0 : c.verifyLoading) || void 0 === m ? void 0 : m.loading) && (null === (u = null === (g = this.props) || void 0 === g ? void 0 : g.verifyLoading) || void 0 === u ? void 0 : u.envId) === b._id && this.renderVerifyLoader(), s().createElement("div", {
                         className: "env-tags"
                     }, s().createElement("div", null, this.renderTags()), s().createElement("div", null, s().createElement(v.Tooltip, {
                         title: "Clone",
                         arrow: !0
                     }, s().createElement(h.Z, {
                         onClick: () => {
-                            this.state.lockedTile || this.props.cloneEnvironment(g)
+                            this.state.lockedTile || this.props.cloneEnvironment(b)
                         },
                         sx: {
                             cursor: this.state.lockedTile ? "not-allowed" : "pointer",
                             color: "gray",
                             fontSize: "1.5em"
                         }
                     })))), s().createElement("div", {
                         className: "env-details"
                     }, s().createElement("p", {
                         className: "env-description",
                         style: {
                             color: this.props.isActive ? "rgba(0, 0, 0, 0.54)" : "var(--jp-ui-font-color2)"
                         }
-                    }, g.description || "No description"), this.props.packageInstallingEnv === g._id && this.props.packageProgress > 0 ? s().createElement("div", null, s().createElement("div", {
+                    }, b.description || "No description"), this.props.packageInstallingEnv === b._id && this.props.packageProgress > 0 ? s().createElement("div", null, s().createElement("div", {
                         style: {
                             display: "flex",
                             justifyContent: "flex-start",
                             alignItems: "center"
                         }
                     }, s().createElement("img", {
                         src: "https://qbraid-static.s3.amazonaws.com/python.svg",
@@ -362,15 +362,15 @@
                         }
                     }, s().createElement("span", {
                         style: {
                             verticalAlign: "middle"
                         }
                     }, s().createElement("img", {
                         src: "https://qbraid-static.s3.amazonaws.com/python.svg"
-                    })), s().createElement("span", null, `${g.packagesInImage.length} packages`))))), s().createElement("div", {
+                    })), s().createElement("span", null, `${b.packagesInImage.length} packages`))))), s().createElement("div", {
                         className: "env-actions"
                     }, this.state.lockedTile ? s().createElement("p", {
                         className: "env-action",
                         style: {
                             width: "100%",
                             marginRight: 10,
                             background: "#673AB7",
@@ -409,16 +409,16 @@
                 strokeLinecap: "round"
             }));
             j.defaultProps = {
                 width: "16",
                 height: "16",
                 color: "#ABABAB"
             };
-            const O = j,
-                U = e => s().createElement("svg", {
+            const U = j,
+                O = e => s().createElement("svg", {
                     width: e.width,
                     height: e.height,
                     style: {
                         minHeight: e.height,
                         minWidth: e.width,
                         filter: e.filter
                     },
@@ -504,23 +504,23 @@
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 v 18.28268 l -15.55544,-5.66171 z"
                 })))));
-            U.defaultProps = {
+            O.defaultProps = {
                 width: "34",
                 height: "36",
                 filter: "none"
             };
-            const L = U;
-            var _ = n(9845);
+            const L = O;
+            var z = n(9845);
 
-            function z(e) {
+            function _(e) {
                 return a.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: "1em",
                     height: "1em",
                     viewBox: "0 0 24 24"
                 }, e), a.createElement("path", {
                     fill: "none",
@@ -554,15 +554,15 @@
                     minute: "2-digit",
                     hour12: !1,
                     timeZone: "UTC"
                 })
             }
             class R extends a.Component {
                 constructor(e, t) {
-                    var n, i, a, r, o;
+                    var n, i, a, o, r, l;
                     super(e, t), this.load = () => this.setState({
                         loaded: !0
                     }), this.shareEnvironment = e => {
                         this.setState({
                             shareEmailBtnDis: !0
                         });
                         let t = {
@@ -594,15 +594,20 @@
                             }), setTimeout((() => {
                                 this.setState({
                                     shareEmail: "",
                                     shareEmailBtnDis: !1,
                                     shareSuccess: !1
                                 })
                             }), B)), 304 !== t.status || e || this.setState({
-                                resharePopUp: !0
+                                resharePopUp: !0,
+                                resharePopUpContent: {
+                                    content: "reShareEnv",
+                                    title: "Update Shared Environment?",
+                                    body: `You have already shared this environment with ${this.state.shareEmail?`${this.state.shareEmail}, or another user`:"one or more users"}. Would you like to update the existing version? Doing so will overwrite the globally shared environment, but will not affect any local copies that users have already installed.`
+                                }
                             })
                         })).then((() => {
                             this.props.flux.getActions("EnvironmentActions").updateAll().then((() => {
                                 this.props.updateReadUserAccessData(this.props.env._id), this.props.flux.getActions("EnvironmentActions").registerInstalled()
                             }))
                         })).catch((t => {
                             (null == t ? void 0 : t.status) ? 404 === t.status ? this.setState({
@@ -758,15 +763,15 @@
                                 msg: `Failed to uninstall ${t}`,
                                 type: "error"
                             }
                         })
                     }, this.updateCustomPackageListInMongo = async () => {
                         var e, t;
                         if (this.state.isCustom) {
-                            const n = (await this.context.getActions("EnvironmentActions").fetchAllEnv()).filter((e => e.slug === l.slug))[0];
+                            const n = (await this.context.getActions("EnvironmentActions").fetchAllEnv()).filter((e => e.slug === c.slug))[0];
                             this.comparePackageList(n) || await this.context.getActions("EnvironmentActions").updateCustomPackageListInMongoDB({
                                 slug: null === (t = null === (e = null == this ? void 0 : this.props) || void 0 === e ? void 0 : e.env) || void 0 === t ? void 0 : t.slug,
                                 packageList: this.state.packagesInImage
                             })
                         }
                     }, this.comparePackageList = e => q().isEqual(null == e ? void 0 : e.packagesInImage, this.state.packagesInImage), this.handleChangePackageFilter = (e, t) => {
                         this.setState({
@@ -918,34 +923,34 @@
                         if (!q().isEmpty(this.state.selectedPkg)) {
                             this.setState({
                                 pkgListBusy: !0
                             }), this.closeAddPackageDialog();
                             let i = e;
                             const a = /(==|~=|<|<=|>|>=)/,
                                 s = /[\d|,|.|e|E|\+]+/g,
-                                r = this.state.packagesInImage.map((e => {
+                                o = this.state.packagesInImage.map((e => {
                                     var t, n, i;
                                     return {
                                         name: e.split(a)[0].toLowerCase().trim(),
                                         version: null === (i = null === (n = null === (t = null == e ? void 0 : e.split(a)[2]) || void 0 === t ? void 0 : t.toLowerCase()) || void 0 === n ? void 0 : n.trim()) || void 0 === i ? void 0 : i.match(s)[0],
                                         pkg: e
                                     }
                                 })),
-                                o = Object.keys(this.state.selectedPkg.releases);
+                                r = Object.keys(this.state.selectedPkg.releases);
                             if ("==" !== this.state.selectedOperator) {
                                 let e = this.state.selectedPkgVersion;
-                                ">" === this.state.selectedOperator ? e = o.filter((e => e > this.state.selectedPkgVersion)).slice(-1) : ">=" === this.state.selectedOperator ? e = o.filter((e => e >= this.state.selectedPkgVersion)).slice(-1) : "<" === this.state.selectedOperator ? e = o.filter((e => e < this.state.selectedPkgVersion)).slice(-1) : "<=" === this.state.selectedOperator && (e = o.filter((e => e <= this.state.selectedPkgVersion)).slice(-1)), e ? i = i.replace(this.state.selectedPkgVersion, e).split(this.state.selectedOperator).join("==") : this.setState({
+                                ">" === this.state.selectedOperator ? e = r.filter((e => e > this.state.selectedPkgVersion)).slice(-1) : ">=" === this.state.selectedOperator ? e = r.filter((e => e >= this.state.selectedPkgVersion)).slice(-1) : "<" === this.state.selectedOperator ? e = r.filter((e => e < this.state.selectedPkgVersion)).slice(-1) : "<=" === this.state.selectedOperator && (e = r.filter((e => e <= this.state.selectedPkgVersion)).slice(-1)), e ? i = i.replace(this.state.selectedPkgVersion, e).split(this.state.selectedOperator).join("==") : this.setState({
                                     popupOpen: !0,
                                     popupMsg: {
                                         msg: "Package version is not available",
                                         type: "error"
                                     }
                                 })
                             } else "==" === this.state.selectedOperator && "any" === this.state.selectedPkgVersion && (i = this.state.selectedPkg.info.name);
-                            const l = r.find((e => e.name === this.state.selectedPkg.info.name)),
+                            const l = o.find((e => e.name === this.state.selectedPkg.info.name)),
                                 c = "any" === this.state.selectedPkgVersion ? "" : this.state.selectedPkgVersion.match(s)[0];
                             if (l && "" !== c && c > l.version) this.setState({
                                 popupOpen: !0,
                                 popupMsg: {
                                     msg: `Upgrading to version ${null===(n=null===(t=this.state.selectedPkg)||void 0===t?void 0:t.info)||void 0===n?void 0:n.version}`,
                                     type: "success"
                                 }
@@ -1080,20 +1085,20 @@
                     }, this.handleCancelReq = () => {
                         this.setState({
                             cancelRequest: !0
                         }), this.handleUninstallAlertOpen()
                     }, this.renderEditTags = () => {
                         if (this.state.isOwner) return this.state.editOpen ? s().createElement(s().Fragment, null, s().createElement(v.Tooltip, {
                             title: "Turn editing tags off"
-                        }, s().createElement(_.EditOff, {
+                        }, s().createElement(z.EditOff, {
                             className: "env-edit-icon",
                             onClick: this.handleEditState
                         })), this.renderAddTags()) : s().createElement(v.Tooltip, {
                             title: "Turn editing tags on"
-                        }, s().createElement(_.Edit, {
+                        }, s().createElement(z.Edit, {
                             className: "env-edit-icon",
                             onClick: this.handleEditState
                         }))
                     }, this.renderAddTags = () => s().createElement("div", {
                         className: "env-add-tags",
                         style: {
                             backgroundColor: this.state.inputBoxVisible && "#673ab7"
@@ -1106,15 +1111,15 @@
                             })))
                         },
                         sx: {
                             padding: 0,
                             fontSize: 14,
                             color: this.state.inputBoxVisible && "white"
                         }
-                    }, s().createElement(_.AddCircleOutlined, {
+                    }, s().createElement(z.AddCircleOutlined, {
                         fontSize: "inherit",
                         color: "inherit"
                     })), this.state.inputBoxVisible && s().createElement("input", {
                         className: "env-tags-input",
                         type: "text",
                         value: this.state.tagInput,
                         placeholder: "Enter tags",
@@ -1173,15 +1178,15 @@
                                         fontSize: "12px"
                                     },
                                     "& .MuiTooltip-arrow": {
                                         color: e.palette.warning.main
                                     }
                                 })
                             }
-                        }, s().createElement(_.ReportProblemOutlined, {
+                        }, s().createElement(z.ReportProblemOutlined, {
                             color: "inherit",
                             sx: {
                                 color: "warning.main",
                                 fontSize: "16px"
                             }
                         })), !e && !this.state.quantumJobsAdditionSuccess && s().createElement(v.Tooltip, {
                             title: "Add quantum jobs",
@@ -1217,27 +1222,27 @@
                                             })
                                         }))
                                     }), 1750))
                                 } catch (e) {
                                     console.log("Error adding quantum jobs. ", e), alert("Unable to add quantum jobs at this time. Please try again later, and verify that qbraid-core is installed and configured correctly.")
                                 }
                             })
-                        }, s().createElement(_.AddCircleOutlineOutlined, {
+                        }, s().createElement(z.AddCircleOutlineOutlined, {
                             fontSize: "inherit"
                         }))), this.state.quantumJobsAdditionSuccess && s().createElement(v.Box, {
                             display: "flex",
                             alignItems: "center",
                             justifyContent: "center",
                             gap: 1,
                             borderRadius: 1,
                             px: 1,
                             sx: e => ({
                                 userSelect: "none"
                             })
-                        }, s().createElement(z, {
+                        }, s().createElement(_, {
                             color: "green"
                         }), s().createElement(v.Typography, {
                             fontSize: 14,
                             sx: e => ({
                                 color: e.palette.success.main
                             })
                         }, "Successfully added!")))
@@ -1272,15 +1277,15 @@
                                 onMouseLeave: () => {
                                     this.setState({
                                         showCopyIcon: !1
                                     })
                                 }
                             }, `ID: ${this.props.env.slug}`, this.state.showCopyIcon && s().createElement(v.Tooltip, {
                                 title: this.state.textCopied ? "Slug Copied" : "Click to copy the Slug ID"
-                            }, s().createElement(_.Link, {
+                            }, s().createElement(z.Link, {
                                 sx: {
                                     fontSize: "1rem",
                                     transform: "rotateZ(-45deg)",
                                     marginLeft: "5px",
                                     cursor: "pointer"
                                 },
                                 onClick: () => {
@@ -1319,15 +1324,15 @@
                         size: "small",
                         variant: "filled",
                         onDelete: "custom" === e.toLowerCase() ? "" : this.state.editOpen ? () => this.handleRemoveTags(t) : ""
                     }))), this.state.isOwner && this.state.editOpen && this.renderAddTags()), this.state.canModify && s().createElement(v.Stack, {
                         flexDirection: "row",
                         gap: 1,
                         justifyContent: "flex-end"
-                    }, this.state.saveSuccess ? s().createElement(z, {
+                    }, this.state.saveSuccess ? s().createElement(_, {
                         width: "2em",
                         height: "2em",
                         color: "green",
                         style: {
                             paddingRight: "8px"
                         }
                     }) : s().createElement(v.Tooltip, {
@@ -1335,56 +1340,128 @@
                         arrow: !0,
                         placement: "left"
                     }, s().createElement(v.IconButton, {
                         size: "small",
                         variant: "slide",
                         color: "text.secondary",
                         onClick: this.state.editOpen ? () => this.handleEditStateClose() : () => this.handleEditStateOpen()
-                    }, this.state.editOpen ? s().createElement(_.EditOff, {
+                    }, this.state.editOpen ? s().createElement(z.EditOff, {
                         fontSize: "inherit",
                         color: "inherit"
-                    }) : s().createElement(_.Edit, {
+                    }) : s().createElement(z.Edit, {
                         fontSize: "inherit",
                         color: "inherit"
                     }))), this.state.editOpen && s().createElement(v.Tooltip, {
                         title: "Save",
                         arrow: !0,
                         placement: "top"
                     }, s().createElement(v.IconButton, {
                         size: "small",
                         variant: "slide",
                         color: "text.secondary",
                         disabled: this.state.saveLoading,
                         onClick: this.handleSubmit
-                    }, this.state.saveLoading ? s().createElement(S, null) : s().createElement(_.SaveOutlined, {
+                    }, this.state.saveLoading ? s().createElement(S, null) : s().createElement(z.SaveOutlined, {
                         fontSize: "inherit"
-                    }))))), this.renderSharingPane = () => {
+                    }))))), this.handleGenerateAccessKey = e => {
+                        this.setState({
+                            accessKeyLoading: !0
+                        }), this.context.getActions("EnvironmentActions").generateAccessKey(e).then((t => {
+                            var n;
+                            this.setState({
+                                accessKey: null === (n = null == t ? void 0 : t.body) || void 0 === n ? void 0 : n.accessKey
+                            });
+                            const i = {
+                                environmentId: e,
+                                overwrite: !0,
+                                isAccessKeyEnv: !0
+                            };
+                            this.context.getActions("EnvironmentActions").shareEnvironment(i).then((e => this.setState({
+                                accessKeyLoading: !1
+                            }))).catch((e => {
+                                console.log(e), this.setState({
+                                    accessKeyLoading: !1
+                                })
+                            }))
+                        })).catch((e => {
+                            console.log(e), this.setState({
+                                accessKeyLoading: !1
+                            })
+                        }))
+                    }, this.renderSharingPane = () => {
                         var e;
                         const t = e => {
-                            let t, n = 0;
-                            for (t = 0; t < (null == e ? void 0 : e.length); t += 1) n = e.charCodeAt(t) + ((n << 5) - n);
-                            let i = "#";
-                            for (t = 0; t < 3; t += 1) i += `00${(n>>8*t&255).toString(16)}`.slice(-2);
-                            return i
-                        };
+                                let t, n = 0;
+                                for (t = 0; t < (null == e ? void 0 : e.length); t += 1) n = e.charCodeAt(t) + ((n << 5) - n);
+                                let i = "#";
+                                for (t = 0; t < 3; t += 1) i += `00${(n>>8*t&255).toString(16)}`.slice(-2);
+                                return i
+                            },
+                            n = {
+                                accessCode: {
+                                    confirm: () => {
+                                        this.setState({
+                                            resharePopUp: !1,
+                                            accessKey: ""
+                                        }), this.handleGenerateAccessKey(this.props.env._id)
+                                    },
+                                    cancel: () => {
+                                        this.setState({
+                                            resharePopUp: !1,
+                                            resharePopUpContent: {
+                                                content: "",
+                                                title: "",
+                                                body: ""
+                                            }
+                                        })
+                                    }
+                                },
+                                reShareEnv: {
+                                    confirm: () => {
+                                        this.setState({
+                                            resharePopUp: !1
+                                        }), this.setState({
+                                            shareEmailBtnDis: !0
+                                        }), this.shareEnvironment(!0)
+                                    },
+                                    cancel: () => {
+                                        this.setState({
+                                            resharePopUp: !1,
+                                            shareEmail: "",
+                                            shareEmailBtnDis: !1
+                                        })
+                                    }
+                                }
+                            };
                         return s().createElement("div", {
                             className: "env-editor-pane",
-                            id: "sharing-pane"
+                            id: "sharing-pane",
+                            style: {
+                                marginTop: "0px !important"
+                            }
                         }, s().createElement("p", {
                             className: "env-editor-pane-title"
-                        }, "Share Environment"), s().createElement("div", {
+                        }, "Share Environment"), s().createElement(v.Box, {
                             className: "env-pane-content",
-                            style: {
-                                flex: 1
-                            }
-                        }, this.state.isMount ? this.state.isOwner ? this.state.isCustom ? this.state.isInstalled ? s().createElement(v.Grid, {
+                            flex: 1,
+                            mt: 0
+                        }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && s().createElement(v.Typography, {
+                            fontSize: 14
+                        }, "Enable other qBraid users to discover this environment and install a copy into their own Lab instance."), this.state.isMount ? this.state.isOwner ? this.state.isCustom ? this.state.isInstalled ? s().createElement(v.Grid, {
                             container: !0,
                             justifyContent: "space-between",
-                            gap: 1,
                             alignItems: "flex-start",
+                            position: "relative",
+                            spacing: 1,
+                            mt: 1
+                        }, s().createElement(v.Grid, {
+                            item: !0,
+                            container: !0,
+                            xs: 12,
+                            spacing: 1,
                             position: "relative"
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             sm: 12,
                             md: 8,
                             lg: 8
@@ -1441,16 +1518,16 @@
                                     fontSize: "14px"
                                 }
                             }
                         })), s().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             sm: 12,
-                            md: 3,
-                            lg: 3
+                            md: 4,
+                            lg: 4
                         }, s().createElement(v.Button, {
                             fullWidth: !0,
                             className: "env-editor-pane-action",
                             onClick: () => {
                                 this.setState({
                                     shareEmailApiError: ""
                                 }), "" !== this.state.shareEmail ? this.state.isCustom ? this.state.uninstalling || this.state.cancelling || this.state.deleting || this.props.installing || this.props.packageInstallingEnv === this.props.env._id ? this.setState({
@@ -1478,68 +1555,208 @@
                             style: {
                                 background: this.state.shareSuccess ? "green" : "#673AB7",
                                 cursor: this.state.shareEmailBtnDis ? "not-allowed !important" : "pointer !important",
                                 marginBottom: (null === (e = this.state.shareEmail) || void 0 === e ? void 0 : e.length) > 2 && !this.state.shareEmail.match(/^[A-Za-z\._\-[0-9]*[@][A-Za-z]*[\.][a-z]{2,4}$/) ? "25px" : "0px"
                             },
                             disabled: this.state.shareEmailBtnDis,
                             size: "small",
-                            startIcon: this.state.shareSuccess ? s().createElement(_.Check, {
+                            startIcon: this.state.shareSuccess ? s().createElement(z.Check, {
                                 color: "green"
-                            }) : s().createElement(_.Send, {
+                            }) : s().createElement(z.Send, {
                                 sx: {
                                     transform: "rotateZ(-45deg)"
                                 }
                             })
                         }, this.state.shareSuccess ? "Sent" : "Share")), s().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             position: "absolute",
-                            top: "32px"
+                            bottom: "4px"
                         }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareEmailApiError && s().createElement("p", {
                             className: "env-pane-email-error"
                         }, this.state.shareEmailApiError), this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareSuccess && s().createElement("p", {
                             className: "env-pane-email-success"
-                        }, "Environment shared succesfully..."))) : s().createElement(v.Grid, {
+                        }, "Environment shared succesfully..."))), s().createElement(v.Grid, {
+                            item: !0,
+                            xs: 12
+                        }, s().createElement(v.Divider, {
+                            textAlign: "center"
+                        }, "OR")), s().createElement(v.Grid, {
+                            item: !0,
+                            display: "flex",
+                            justifyContent: "center",
+                            alignItems: "center",
+                            xs: 12
+                        }, "" === this.state.accessKey ? s().createElement(v.Button, {
+                            fullWidth: !0,
+                            variant: "outlined",
+                            color: "success",
+                            onClick: () => this.handleGenerateAccessKey(this.props.env._id),
+                            sx: {
+                                textTransform: "none",
+                                fontSize: 12,
+                                cursor: this.state.accessKeyLoading ? "progress" : "pointer"
+                            },
+                            disabled: this.state.accessKeyLoading
+                        }, this.state.accessKeyLoading ? "Generating ..." : "Generate Access Code") : s().createElement(v.Grid, {
+                            item: !0,
+                            xs: 12
+                        }, s().createElement(v.Paper, {
+                            elevation: 0,
+                            sx: e => ({
+                                display: "flex",
+                                alignItems: "center",
+                                width: "100%",
+                                backgroundColor: `${e.palette.success.light}30`
+                            })
+                        }, s().createElement(v.Typography, {
+                            fontSize: 12,
+                            color: "success",
+                            px: 1.5
+                        }, "Share via access code"), s().createElement(v.Divider, {
+                            orientation: "vertical",
+                            sx: {
+                                m: .5,
+                                height: 28
+                            }
+                        }), s().createElement(v.InputBase, {
+                            size: "small",
+                            sx: {
+                                ml: 1,
+                                flex: 1,
+                                fontSize: 12,
+                                fontWeight: 600,
+                                "&.MuiInputBase-input": {
+                                    p: 0
+                                }
+                            },
+                            value: this.state.accessKey,
+                            type: this.state.accessKeyVisibility ? "text" : "password"
+                        }), s().createElement(v.IconButton, {
+                            size: "small",
+                            onClick: () => {
+                                this.setState((e => ({
+                                    accessKeyVisibility: !e.accessKeyVisibility
+                                })))
+                            }
+                        }, this.state.accessKeyVisibility ? s().createElement(z.VisibilityOff, {
+                            fontSize: "inherit"
+                        }) : s().createElement(z.Visibility, {
+                            fontSize: "inherit"
+                        })), s().createElement(v.Divider, {
+                            orientation: "vertical",
+                            sx: {
+                                m: .5,
+                                height: 28
+                            }
+                        }), s().createElement(v.Tooltip, {
+                            arrow: !0,
+                            placement: "left",
+                            title: "Copy"
+                        }, s().createElement(v.IconButton, {
+                            size: "small",
+                            sx: {
+                                mx: 1.5
+                            },
+                            onClick: () => {
+                                this.setState({
+                                    copyCooldown: !0
+                                }), navigator.clipboard.writeText(this.state.accessKey), setTimeout((() => this.setState({
+                                    copyCooldown: !1
+                                })), 1500)
+                            }
+                        }, this.state.copyCooldown ? s().createElement(_, {
+                            color: "green"
+                        }) : s().createElement(z.ContentCopy, {
+                            fontSize: "inherit"
+                        })))))), s().createElement(v.Grid, {
+                            item: !0,
+                            xs: 12,
+                            display: "flex",
+                            justifyContent: "flex-end",
+                            alignItems: "center",
+                            gap: 1
+                        }, "" !== this.state.accessKey && s().createElement(s().Fragment, null, s().createElement(v.Button, {
+                            variant: "text",
+                            color: "success",
+                            size: "small",
+                            startIcon: s().createElement(z.Refresh, {
+                                fontSize: "inherit"
+                            }),
+                            sx: {
+                                padding: "0px !important",
+                                textTransform: "none"
+                            },
+                            onClick: () => {
+                                this.setState({
+                                    resharePopUp: !0,
+                                    resharePopUpContent: {
+                                        content: "accessCode",
+                                        title: "Are you sure?",
+                                        body: "Generating a new access code will invalidate the current code, and update the global shared copy of this environment."
+                                    }
+                                })
+                            }
+                        }, "Regenerate access code?"), s().createElement(v.Tooltip, {
+                            title: s().createElement(s().Fragment, null, "The existing access code will be invalidated and your current environment will replace the global shared copy."),
+                            PopperProps: {
+                                sx: e => ({
+                                    [`& .${v.tooltipClasses.tooltip}`]: {
+                                        background: e.palette.background.alternate,
+                                        color: e.palette.text.primary,
+                                        fontSize: 12,
+                                        boxShadow: e.shadows[10]
+                                    }
+                                })
+                            }
+                        }, s().createElement(z.InfoOutlined, {
+                            fontSize: "small",
+                            color: "action",
+                            sx: {
+                                width: 14,
+                                height: 14
+                            }
+                        }))))) : s().createElement(v.Grid, {
                             container: !0
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
                         }, s().createElement("p", {
                             className: "env-pane-prompt"
                         }, "To share an environment, it must be installed. To install this environment, click ", s().createElement("b", null, "Install"), " in the panel drop-down."))) : s().createElement(v.Grid, {
                             container: !0
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
                         }, s().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "This environment is not shareable. To create a shareable, custom environment, click", " ", s().createElement("b", null, "+ Add ", "→", " + Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
+                        }, "This environment is not shareable. To create a shareable, custom environment, click", " ", s().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
                             container: !0
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
                         }, s().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "To share an environment, you must be the environment owner. To create your own shareable, custom environment, click", " ", s().createElement("b", null, "+ Add ", "→", " + Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
+                        }, "To share an environment, you must be the environment owner. To create your own shareable, custom environment, click", " ", s().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
                             container: !0
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
                         }, s().createElement("p", {
                             className: "env-pane-prompt"
                         }, "Sharing environments is only available within the cloud-based qBraid Lab platform. Launch an instance at", " ", s().createElement("a", {
                             href: "https://lab.qbraid.com",
                             style: {
                                 color: "blue"
                             },
                             target: "_blank",
                             rel: "noopener noreferrer"
-                        }, "lab.qbraid.com"), " ", "to share environments with other users."))), this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && s().createElement("p", {
-                            className: "env-pane-email-normal"
-                        }, "Share this environment to make it visible to another qBraid user, and allow them to install it directly in to their own Lab instance."), this.renderReshareEnvModal(), this.renderUpgradeEnvModal()))
+                        }, "lab.qbraid.com"), " ", "to share environments with other users."))), this.renderReshareEnvModal({
+                            action: n
+                        }), this.renderUpgradeEnvModal()))
                     }, this.renderUpgradeEnvModal = () => s().createElement(v.Modal, {
                         open: this.state.upgradePopUp,
                         onClose: () => this.setState({
                             upgradePopUp: !1
                         }),
                         sx: {
                             display: "flex",
@@ -1604,22 +1821,18 @@
                         variant: "slide",
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         },
                         fullWidth: !0,
                         onClick: () => window.open(`${y}/billing`, "_blank")
-                    }, "Upgrade"))))), this.renderReshareEnvModal = () => {
-                        const e = () => {
-                            this.setState({
-                                resharePopUp: !1
-                            }), this.setState({
-                                shareEmailBtnDis: !0
-                            }), this.shareEnvironment(!0)
-                        };
+                    }, "Upgrade"))))), this.renderReshareEnvModal = ({
+                        action: e
+                    }) => {
+                        var t, n;
                         return s().createElement(v.Modal, {
                             open: this.state.resharePopUp,
                             onClose: () => this.setState({
                                 resharePopUp: !1,
                                 shareEmailBtnDis: !1,
                                 shareEmail: ""
                             }),
@@ -1634,65 +1847,56 @@
                             container: !0,
                             sx: {
                                 width: "700px",
                                 minWidth: "200px",
                                 minHeight: "150px",
                                 padding: "1em"
                             },
-                            className: "env-pane-re-share"
+                            className: "env-pane-re-share",
+                            spacing: 1
                         }, s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("h3", {
-                            style: {
-                                margin: "0px"
-                            }
-                        }, "Update Shared Environment?")), s().createElement(v.Grid, {
+                        }, s().createElement(v.Typography, {
+                            fontSize: 18,
+                            fontWeight: 600,
+                            color: "text.primary"
+                        }, this.state.resharePopUpContent.title)), s().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("p", {
-                            className: "env-pane-email-normal"
-                        }, `You have already shared this environment with ${this.state.shareEmail}, or another user. Would you like to update the existing version? Doing so will overwrite the globally shared environment, but will not effect any local copies that users have already installed.`)), s().createElement(v.Grid, {
+                        }, s().createElement(v.Typography, {
+                            fontSize: 14,
+                            color: "text.primary"
+                        }, this.state.resharePopUpContent.body)), s().createElement(v.Grid, {
                             item: !0,
                             container: !0,
                             xs: 12,
-                            sx: {
-                                display: "flex",
-                                justifyContent: "flex-end",
-                                alignItems: "center",
-                                gap: "10px"
-                            }
+                            justifyContent: "flex-end",
+                            alignItems: "center",
+                            spacing: 1
                         }, s().createElement(v.Grid, {
-                            item: !0,
-                            xs: 2
+                            item: !0
                         }, s().createElement(v.Button, {
                             variant: "slide",
                             type: "decline",
-                            fullWidth: !0,
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             },
-                            onClick: () => this.setState({
-                                resharePopUp: !1,
-                                shareEmail: "",
-                                shareEmailBtnDis: !1
-                            })
+                            onClick: null === (t = e[this.state.resharePopUpContent.content]) || void 0 === t ? void 0 : t.cancel
                         }, "Cancel")), s().createElement(v.Grid, {
-                            item: !0,
-                            xs: 2
+                            item: !0
                         }, s().createElement(v.Button, {
                             variant: "slide",
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             },
-                            fullWidth: !0,
-                            onClick: () => e()
-                        }, "Share")))))
+                            onClick: null === (n = e[this.state.resharePopUpContent.content]) || void 0 === n ? void 0 : n.confirm
+                        }, "Confirm")))))
                     }, this.renderShareMsg = ({
                         msg: e,
                         type: t
                     }) => s().createElement(v.Snackbar, {
                         open: this.state.sharePopupOpen,
                         autoHideDuration: B,
                         onClose: this.handleSharePopupClose,
@@ -1862,15 +2066,15 @@
                             }, s().createElement(v.IconButton, {
                                 size: "small",
                                 color: "error",
                                 disabled: this.props.installing || this.props.env.isPreInstalled || this.state.lockedEnv,
                                 onClick: () => {
                                     !this.props.installing && !this.props.env.isPreInstalled && this.handleRemovePkg(e)
                                 }
-                            }, s().createElement(_.Close, null)))))
+                            }, s().createElement(z.Close, null)))))
                         })), (this.props.packageLoading || this.state.packageListLoading) && Array.from({
                             length: 4
                         }, ((e, t) => t + 1)).map((e => s().createElement(v.TableRow, {
                             key: e
                         }, s().createElement(v.TableCell, {
                             colSpan: 3
                         }, s().createElement(v.Skeleton, {
@@ -1963,18 +2167,18 @@
                                     marginBottom: "-8px !important"
                                 }
                             }
                         }
                     }, s().createElement("div", {
                         onClick: this.handleSearchSubmit,
                         className: this.state.searchInput.length >= 3 ? "shake-bottom" : ""
-                    }, s().createElement(O, {
+                    }, s().createElement(U, {
                         color: this.state.searchInput.length >= 3 ? "#673ab7" : "#ABABAB"
                     })))), q().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderErrorDropdown(), !q().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderDropdown(), this.state.packageNotInList && this.renderAlertDropDown()), this.renderDropdown = () => {
-                        var e, t, n, i, a, r, o, l, c, d, p, h, m;
+                        var e, t, n, i, a, o, r, l, c, d, p, h, m;
                         const g = ["==", "~=", "<", "<=", ">", ">="];
                         return s().createElement("div", {
                             className: "env-pane-dropdown slide-in-top"
                         }, s().createElement("ul", {
                             className: "env-pane-dropdown-list"
                         }, s().createElement("li", {
                             className: (null === (e = this.state.selectedPkg) || void 0 === e ? void 0 : e.last_serial) === (null === (t = this.state.searchResults) || void 0 === t ? void 0 : t.last_serial) ? "filled" : "",
@@ -1983,15 +2187,15 @@
                             width: "34",
                             height: "36",
                             filter: (null === (n = this.state.selectedPkg) || void 0 === n ? void 0 : n.last_serial) === (null === (i = this.state.searchResults) || void 0 === i ? void 0 : i.last_serial) ? "drop-shadow(2px 4px 6px rgba(0,0,0,0.2))" : ""
                         }), s().createElement("span", {
                             className: "env-pane-flexrow"
                         }, s().createElement("p", {
                             className: "env-pane-dropdown-name"
-                        }, null === (r = null === (a = this.state.searchResults) || void 0 === a ? void 0 : a.info) || void 0 === r ? void 0 : r.name), s().createElement("p", {
+                        }, null === (o = null === (a = this.state.searchResults) || void 0 === a ? void 0 : a.info) || void 0 === o ? void 0 : o.name), s().createElement("p", {
                             className: "env-pane-dropdown-version"
                         }, s().createElement("select", {
                             className: "operator-selector",
                             name: "operatorSelector",
                             value: this.state.selectedOperator,
                             disabled: "any" === this.state.selectedPkgVersion,
                             onChange: e => this.setState({
@@ -2002,15 +2206,15 @@
                         }, e))))), s().createElement("p", {
                             className: "env-pane-dropdown-version"
                         }, s().createElement("select", {
                             style: {
                                 fontWeight: "600",
                                 width: "70px",
                                 padding: ".3em",
-                                border: (null === (o = this.state.selectedPkg) || void 0 === o ? void 0 : o.last_serial) === (null === (l = this.state.searchResults) || void 0 === l ? void 0 : l.last_serial) ? "1px solid white" : "1px solid #673ab7",
+                                border: (null === (r = this.state.selectedPkg) || void 0 === r ? void 0 : r.last_serial) === (null === (l = this.state.searchResults) || void 0 === l ? void 0 : l.last_serial) ? "1px solid white" : "1px solid #673ab7",
                                 backgroundColor: (null === (c = this.state.selectedPkg) || void 0 === c ? void 0 : c.last_serial) === (null === (d = this.state.searchResults) || void 0 === d ? void 0 : d.last_serial) ? "#ffffff" : "#673ab7",
                                 borderRadius: "5px",
                                 color: (null === (p = this.state.selectedPkg) || void 0 === p ? void 0 : p.last_serial) === (null === (h = this.state.searchResults) || void 0 === h ? void 0 : h.last_serial) ? "#673ab7" : "#ffffff"
                             },
                             className: "package-selector",
                             name: "packageVersion",
                             id: "packageVersion",
@@ -2040,15 +2244,15 @@
                         className: "env-pane-dropdown-name"
                     }, "No package found!"))))), this.renderAlertDropDown = () => s().createElement("div", {
                         className: "env-pane-dropdown slide-in-top"
                     }, s().createElement("ul", {
                         className: "env-pane-dropdown-list"
                     }, s().createElement("li", {
                         className: "env-pane-dropdown-over-ride"
-                    }, s().createElement(_.InfoOutlined, {
+                    }, s().createElement(z.InfoOutlined, {
                         width: "34",
                         height: "36"
                     }), s().createElement("span", null, s().createElement("p", {
                         style: {
                             fontSize: "12px",
                             fontWeight: "400"
                         }
@@ -2145,15 +2349,15 @@
                             }
                         }, s().createElement("div", {
                             className: "env-pane-content"
                         }, s().createElement(v.Stack, {
                             direction: "row",
                             alignItems: "flex-start",
                             gap: 2
-                        }, this.props.env.canUpdate ? s().createElement(_.Update, null) : s().createElement(_.UpdateDisabled, null), s().createElement(v.Typography, {
+                        }, this.props.env.canUpdate ? s().createElement(z.Update, null) : s().createElement(z.UpdateDisabled, null), s().createElement(v.Typography, {
                             className: "env-pane-prompt"
                         }, n)), this.state.uninstalling && s().createElement(v.Stack, {
                             gap: 1
                         }, s().createElement(v.Typography, {
                             className: "env-pane-prompt"
                         }, `Uninstalling ${this.props.env.displayName}`), s().createElement(v.LinearProgress, {
                             sx: {
@@ -2302,15 +2506,15 @@
                             textTransform: "none",
                             backgroundColor: "darkred",
                             borderRadius: "6px",
                             "&:hover": {
                                 backgroundColor: "red"
                             }
                         },
-                        startIcon: s().createElement(_.NotInterested, null),
+                        startIcon: s().createElement(z.NotInterested, null),
                         onClick: !this.state.cancelling && this.handleCancelReq,
                         disabled: this.state.cancelling || this.props.packageInstallingEnv === this.props.env._id
                     }, this.state.cancelling ? "Cancelling..." : "Cancel Installation")))), this.renderExtraUninsConfirmAlert = () => {
                         var e;
                         return s().createElement(v.Dialog, {
                             open: this.state.extraUninstallAlert,
                             onClose: this.handleExtraUninsConfirmClose,
@@ -2320,15 +2524,15 @@
                             transitionDuration: 100
                         }, s().createElement(v.DialogTitle, {
                             id: "alert-dialog-title"
                         }, "Are you sure?"), s().createElement(v.DialogContent, {
                             id: "alert-dialog-content"
                         }, s().createElement(v.DialogContentText, {
                             id: "alert-dialog-description"
-                        }, `${this.state.cancelRequest?"Cancelling":"Uninstalling"} will lead to permanent deletion of environment '${l.displayName}'${(null===(e=this.props.env.readAccessUsers)||void 0===e?void 0:e.length)>0?" and remove access from all users that it has been shared with":""}. This action cannot be undone.`)), s().createElement(v.DialogActions, {
+                        }, `${this.state.cancelRequest?"Cancelling":"Uninstalling"} will lead to permanent deletion of environment '${c.displayName}'${(null===(e=this.props.env.readAccessUsers)||void 0===e?void 0:e.length)>0?" and remove access from all users that it has been shared with":""}. This action cannot be undone.`)), s().createElement(v.DialogActions, {
                             id: "alert-dialog-actions"
                         }, s().createElement(v.Button, {
                             variant: "slide",
                             type: "decline",
                             onClick: this.handleExtraUninsConfirmClose,
                             sx: {
                                 textTransform: "none",
@@ -2364,15 +2568,15 @@
                     }, "cancel"), s().createElement(v.Button, {
                         sx: {
                             padding: "0.3rem 2.5rem",
                             minWidth: "100px"
                         },
                         variant: "slide",
                         onClick: this.handleSubmit
-                    }, l ? "Save" : "Create")) : s().createElement(v.DialogActions, {
+                    }, c ? "Save" : "Create")) : s().createElement(v.DialogActions, {
                         sx: {
                             justifyContent: "center",
                             padding: "10px",
                             background: "linear-gradient(120deg, #35383a 10%, #5e5f61 100%)"
                         }
                     }, s().createElement(v.Button, {
                         sx: {
@@ -2382,28 +2586,28 @@
                         variant: "slide",
                         type: "decline",
                         onClick: () => {
                             this.props.onClose()
                         }
                     }, "Close"));
                     let {
-                        env: l
-                    } = e, c = t.getStore("EnvironmentStore").getState(), d = t.getStore("UserStore").getState(), p = null == d ? void 0 : d.user, h = !l || !!p && l.owner === p._id;
+                        env: c
+                    } = e, d = t.getStore("EnvironmentStore").getState(), p = t.getStore("UserStore").getState(), h = null == p ? void 0 : p.user, m = !c || !!h && c.owner === h._id;
                     this.state = {
-                        tags: l ? l.tags : [],
-                        packagesInImage: l ? [...l.packagesInImage] : [],
-                        readAccessUsers: l ? [...l.readAccessUsers] : [],
-                        writeAccessUsers: l ? [...l.writeAccessUsers] : [],
-                        quantumJobs: !!l && l.quantumJobs,
-                        quantumJobsEnabled: !!l && l.quantumJobsEnabled,
+                        tags: c ? c.tags : [],
+                        packagesInImage: c ? [...c.packagesInImage] : [],
+                        readAccessUsers: c ? [...c.readAccessUsers] : [],
+                        writeAccessUsers: c ? [...c.writeAccessUsers] : [],
+                        quantumJobs: !!c && c.quantumJobs,
+                        quantumJobsEnabled: !!c && c.quantumJobsEnabled,
                         quantumJobsAdditionSuccess: !1,
-                        isMount: null !== (n = null == d ? void 0 : d.isMount) && void 0 !== n && n,
-                        user: p,
-                        isOwner: h,
-                        canModify: !(l && !h) || !!p && -1 !== l.writeAccessUsers.map((e => e._id)).indexOf(p._id),
+                        isMount: null !== (n = null == p ? void 0 : p.isMount) && void 0 !== n && n,
+                        user: h,
+                        isOwner: m,
+                        canModify: !(c && !m) || !!h && -1 !== c.writeAccessUsers.map((e => e._id)).indexOf(h._id),
                         loaded: !1,
                         collaboratorFilter: "",
                         packageFilter: "",
                         addPackageDialogOpen: !1,
                         searchInput: "",
                         searchResults: {},
                         isDropdownVisible: !1,
@@ -2439,28 +2643,37 @@
                         resharePopUp: !1,
                         upgradePopUp: !1,
                         qjobsStatus: {
                             open: !1,
                             error: !1,
                             message: ""
                         },
-                        isCustom: null !== (i = l.tags.includes("custom")) && void 0 !== i && i,
-                        isShareNode: null !== (r = null === (a = null == p ? void 0 : p.permissionsNodes) || void 0 === a ? void 0 : a.includes("qbraid.environments.share")) && void 0 !== r && r,
+                        isCustom: null !== (i = c.tags.includes("custom")) && void 0 !== i && i,
+                        isShareNode: null !== (o = null === (a = null == h ? void 0 : h.permissionsNodes) || void 0 === a ? void 0 : a.includes("qbraid.environments.share")) && void 0 !== o && o,
                         textCopied: !1,
-                        isInstalled: !!(null === (o = null == c ? void 0 : c.environmentCache[null == l ? void 0 : l._id]) || void 0 === o ? void 0 : o.installed),
+                        isInstalled: !!(null === (r = null == d ? void 0 : d.environmentCache[null == c ? void 0 : c._id]) || void 0 === r ? void 0 : r.installed),
                         showCopyIcon: !1,
                         cancelling: !1,
                         cancelRequest: !1,
                         inputBoxVisible: !1,
                         saveSuccess: !1,
                         saveLoading: !1,
                         deleting: !1,
                         deleteAlert: !1,
                         loadingPackages: !0,
-                        lockedEnv: !0
+                        lockedEnv: !0,
+                        accessKeyVisibility: !1,
+                        accessKey: (null === (l = this.props.env) || void 0 === l ? void 0 : l.accessKey) || "",
+                        accessKeyLoading: !1,
+                        copyCooldown: !1,
+                        resharePopUpContent: {
+                            content: "",
+                            title: "",
+                            body: ""
+                        }
                     }
                 }
                 componentDidMount() {
                     setTimeout(this.load, 1), this.props.env && setTimeout((() => {
                         this._nameInput && (this._nameInput.value = this.props.env.displayName || ""), this._descriptionInput && (this._descriptionInput.value = this.props.env.description || "")
                     }), 1);
                     const e = JSON.parse(localStorage.getItem("recent-email"));
@@ -2527,15 +2740,15 @@
                             this.props.onClose()
                         },
                         sx: {
                             position: "absolute",
                             right: 8,
                             top: 12
                         }
-                    }, s().createElement(_.Close, null))), s().createElement(v.DialogContent, {
+                    }, s().createElement(z.Close, null))), s().createElement(v.DialogContent, {
                         sx: {
                             backgroundColor: "var(--jp-layout-color2)",
                             padding: "16px"
                         },
                         dividers: !0
                     }, s().createElement(v.Grid, {
                         container: !0,
@@ -2581,17 +2794,17 @@
             }, a.createElement("path", {
                 d: "M 15 3 C 12.031398 3 9.3028202 4.0834384 7.2070312 5.875 A 1.0001 1.0001 0 1 0 8.5058594 7.3945312 C 10.25407 5.9000929 12.516602 5 15 5 C 20.19656 5 24.450989 8.9379267 24.951172 14 L 22 14 L 26 20 L 30 14 L 26.949219 14 C 26.437925 7.8516588 21.277839 3 15 3 z M 4 10 L 0 16 L 3.0507812 16 C 3.562075 22.148341 8.7221607 27 15 27 C 17.968602 27 20.69718 25.916562 22.792969 24.125 A 1.0001 1.0001 0 1 0 21.494141 22.605469 C 19.74593 24.099907 17.483398 25 15 25 C 9.80344 25 5.5490109 21.062074 5.0488281 16 L 8 16 L 4 10 z"
             }));
             var $ = n(2761),
                 V = n(3343),
                 H = n(5384),
                 J = n(3888),
-                Y = n.n(J),
-                Z = (n(4007), n(2270), n(49), n(787), n(471));
-            const Q = {
+                K = n.n(J),
+                Y = (n(4007), n(2270), n(49), n(787), n(471));
+            const Z = {
                     palette: {
                         mode: "light",
                         primary: {
                             main: "#d30982"
                         },
                         secondary: {
                             main: "#673ab7",
@@ -2599,14 +2812,17 @@
                         },
                         secondaryHighlight: {
                             main: "#562944",
                             contrastText: "#ffffff"
                         },
                         typography: {
                             fontFamily: ["var(--jp-ui-font-family)"].join(",")
+                        },
+                        background: {
+                            alternate: "linear-gradient(120deg, #fdfbfb 0%, #ebedee 100%)"
                         }
                     },
                     components: {
                         MuiButton: {
                             variants: [{
                                 props: {
                                     variant: "slide"
@@ -2647,15 +2863,15 @@
                                         color: "white"
                                     }
                                 }
                             }]
                         }
                     }
                 },
-                X = Object.assign(Object.assign({}, Q), {
+                Q = Object.assign(Object.assign({}, Z), {
                     palette: {
                         mode: "dark",
                         primary: {
                             main: "#d30982"
                         },
                         secondary: {
                             main: "#673ab7",
@@ -2663,19 +2879,22 @@
                         },
                         secondaryHighlight: {
                             main: "#562944",
                             contrastText: "#ffffff"
                         },
                         typography: {
                             fontFamily: ["var(--jp-ui-font-family)"].join(",")
+                        },
+                        background: {
+                            alternate: "#1e1e1e"
                         }
                     }
                 }),
-                K = (0, Z.Z)(Q),
-                ee = (0, Z.Z)(X);
+                X = (0, Y.Z)(Z),
+                ee = (0, Y.Z)(Q);
             var te = n(6513);
             g()(te.Z, {
                 insert: "head",
                 singleton: !1
             }), te.Z.locals;
             const ne = ({
                 timeOverMsg: e,
@@ -2780,19 +2999,19 @@
                     fontSize: 14
                 }, "EXPORT LAWS. The Software and all related technical information or materials are subject to export controls and (are or may be) licensable under U.S. Government export regulations. qBraid Customer will not export, re-export, divert, transfer or disclose, directly or indirectly, the Software, Documentation and any related technical information or materials without complying strictly with all legal requirements including, without limitation, obtaining the prior approval of the U.S. Department of Commerce and, if necessary, other agencies or departments of the U.S. Government. Upon request, Intel will provide qBraid Customer with information regarding the export classification of the Software that may be necessary to assist qBraid Customer's compliance with this provision. qBraid Customer will execute and deliver to Intel “Letters of Assurance,” confirming compliance with applicable export regulations. qBraid Customer will indemnify Intel against any loss related to qBraid Customer's failure to conform to these requirements."), s().createElement(v.Typography, {
                     fontSize: 14
                 }, "APPLICABLE LAWS. This Agreement is governed by the laws of the state of Delaware, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. qBraid Customer may not export the Software in violation of applicable export laws and regulations."), s().createElement(v.Typography, {
                     fontSize: 14
                 }, "qBraid Customer's specific rights may vary from country to country."));
             var se = n(948),
-                re = n(1596),
-                oe = n(6532),
+                oe = n(1596),
+                re = n(6532),
                 le = n(1250),
                 ce = n(3083);
-            const de = (0, se.ZP)((e => a.createElement(oe.Z, Object.assign({
+            const de = (0, se.ZP)((e => a.createElement(re.Z, Object.assign({
                     disableGutters: !0,
                     elevation: 0,
                     square: !0
                 }, e))))((({
                     theme: e
                 }) => ({
                     border: 0,
@@ -2802,15 +3021,15 @@
                         borderBottom: 0
                     },
                     "&:before": {
                         display: "none"
                     }
                 }))),
                 pe = (0, se.ZP)((e => a.createElement(le.Z, Object.assign({
-                    expandIcon: a.createElement(re.Z, {
+                    expandIcon: a.createElement(oe.Z, {
                         sx: {
                             fontSize: "1.5rem",
                             color: "var(--jp-layout-color4)"
                         }
                     })
                 }, e))))((({
                     theme: e
@@ -2835,15 +3054,15 @@
                     display: "flex",
                     flexDirection: "column",
                     justifyContent: "center",
                     alignItems: "center",
                     position: "absolute",
                     top: "45%",
                     left: "35%"
-                }, s().createElement(_.PersonOff, {
+                }, s().createElement(z.PersonOff, {
                     color: "disabled",
                     sx: {
                         width: "64px",
                         height: "64px"
                     }
                 }), s().createElement(v.Typography, {
                     color: "InactiveCaptionText",
@@ -2899,15 +3118,15 @@
                         isLocked: !1
                     }) : e
                 })).reduce(((e, t, n) => (!t.isLocked && n > 0 ? e.unshift(t) : e.push(t), e)), [])
             }
             var Ee;
             class ye extends s().Component {
                 constructor(e) {
-                    var t, n, i, a, o, l, c, d;
+                    var t, n, i, a, r, l, c, d;
                     super(e), this.resizeEditor = () => {
                         var e, t, n;
                         null === (n = null === (t = null === (e = this.aceRef) || void 0 === e ? void 0 : e.current) || void 0 === t ? void 0 : t.editor) || void 0 === n || n.resize()
                     }, this.handleChangeCode = e => {
                         this.setState({
                             newEnvCode: e
                         }, (() => {
@@ -2941,30 +3160,30 @@
                     }, this.highlightKernelSelector = e => {
                         let t, n;
                         const i = this.state.environments.filter((e => e.installed && e.active)),
                             {
                                 app: a
                             } = this.props,
                             s = a.shell.currentWidget,
-                            r = s.toolbar.layout.widgets.filter((e => e.node.classList.contains("jp-KernelName")))[0];
-                        if (r) try {
+                            o = s.toolbar.layout.widgets.filter((e => e.node.classList.contains("jp-KernelName")))[0];
+                        if (o) try {
                             const a = document.querySelector(".lm-Widget.p-Widget.jp-KernelName.jp-Toolbar-item");
                             if (e) {
-                                r.addClass("highlight-kernel");
+                                o.addClass("highlight-kernel");
                                 const e = document.createElement("p"),
                                     i = document.createTextNode("Change kernel");
                                 e.appendChild(i), e.setAttribute("id", "kernel-change-text"), e.setAttribute("class", "pos-fixed-kernel_message"), a.appendChild(e), n = setInterval((() => {
                                     var t;
                                     const n = (null === (t = null === document || void 0 === document ? void 0 : document.getElementById("jp-left-stack")) || void 0 === t ? void 0 : t.offsetWidth) || 0,
                                         i = s.node.offsetWidth;
                                     e.style.right = `calc(100vw - ${i}px - ${n}px)`, e.style.opacity = 1
                                 }), 500), t = setTimeout((() => {
                                     a.removeChild(e), clearInterval(n)
                                 }), 5e3)
-                            } else i.length || r.removeClass("highlight-kernel")
+                            } else i.length || o.removeClass("highlight-kernel")
                         } catch (e) {
                             console.log("Can't highlight", e), n && clearInterval(n)
                         } finally {
                             n && setTimeout((() => {
                                 clearInterval(n)
                             }), 5e3)
                         }
@@ -3086,15 +3305,15 @@
                         return e && (s = Object.assign(Object.assign({}, s), {
                             checkbox: {
                                 label: "Don't ask me again",
                                 caption: "Reminder",
                                 className: "gpu_warn_dialog-checkbox",
                                 checked: !1
                             }
-                        })), (0, r.showDialog)(s)
+                        })), (0, o.showDialog)(s)
                     }, this.handleOpenIntelPermissionModal = () => {
                         this.setState({
                             intelPermissionModal: !0
                         })
                     }, this.handleCloseIntelPermissionModal = () => {
                         this.setState({
                             intelPermissionModal: !1
@@ -3113,15 +3332,15 @@
                     }, s().createElement(v.Stack, {
                         px: "24px",
                         pt: "16px",
                         gap: 1,
                         sx: {
                             userSelect: "none"
                         }
-                    }, s().createElement(_.ReceiptLongOutlined, {
+                    }, s().createElement(z.ReceiptLongOutlined, {
                         fontSize: "inherit",
                         sx: e => ({
                             width: 48,
                             height: 48,
                             marginInline: "auto",
                             rotate: "25deg",
                             color: e.palette.secondary.light
@@ -3229,18 +3448,20 @@
                         const e = this.state.installingEnvironment;
                         e && (this.setState({
                             progress: 0,
                             timeToInstall: 0
                         }), this.resetNewEnvData(), this.props.flux.getActions("EnvironmentActions").uninstall(e.slug).then((t => {
                             this.props.flux.getActions("EnvironmentActions").registerInstalled().then((t => (this.handleOpenPopup("Installation Failure", "error"), alert("Your environment " + e.displayName + " could not be installed at this time.")))).catch((t => (console.log(t), this.handleOpenPopup("Installation Failure", "error"), alert("Your environment " + e.displayName + " could not be installed at this time."))))
                         })).catch((t => (console.log(t), this.handleOpenPopup("Uninstallation Failure", "error"), alert("Your environment " + e.displayName + " could not be uninstalled at this time.")))))
-                    }, this.handleRefreshEnvironments = () => {
-                        this.setState((e => ({
+                    }, this.handleRefreshEnvironments = ({
+                        clickedRefresh: e
+                    }) => {
+                        e && this.setState((e => ({
                             togglesCount: ++e.togglesCount
-                        }))), this.state.noUser || (this.setState({
+                        }))), this.state.noUser || (e && this.setState({
                             isClickedRefresh: !0
                         }), this.props.flux.getActions("EnvironmentActions").updateAll().then((e => {
                             this.props.flux.getActions("EnvironmentActions").registerInstalled().then((e => {
                                 if (this.setState({
                                         isClickedRefresh: !1
                                     }), this.state.installingEnvironment && !this.state.packageInstallingEnv) {
                                     const e = this.state.qbUser.user._id,
@@ -3368,29 +3589,22 @@
                             }), await this.props.flux.getActions("EnvironmentActions").updateCustomPackageListInMongoDB({
                                 slug: n.slug,
                                 packageList: n.packagesInImage
                             }), this.handleFinishInstallSuccess()
                         } catch (e) {
                             return console.log(e), this.handleFinishInstallFailure()
                         }
-                    }, this.toggleExpandedEnv = e => {
-                        this.state.expandedEnvs.includes(e) ? this.setState((t => Object.assign(Object.assign({}, t), {
+                    }, this.onToggleExpand = e => {
+                        this.setState({
+                            newCustomEnvId: null
+                        }), this.state.expandedEnvs.includes(e) ? this.setState((t => Object.assign(Object.assign({}, t), {
                             expandedEnvs: t.expandedEnvs.filter((t => t !== e))
                         }))) : this.setState((t => Object.assign(Object.assign({}, t), {
                             expandedEnvs: [...t.expandedEnvs, e]
                         })))
-                    }, this.onToggleExpand = e => {
-                        let t = this.state.environments.map((t => {
-                            let n = t;
-                            return t._id !== e && t._id !== this.state.newCustomEnvId || (n.isExpanded = !n.isExpanded), n
-                        }));
-                        this.setState({
-                            environments: t,
-                            newCustomEnvId: null
-                        }), this.toggleExpandedEnv(e)
                     }, this.onTogglePinned = e => {
                         let t = this.state.environments.map((t => {
                             let n = t;
                             return t._id === e && (n.pinned ? this.handleRemovePinned(e) : this.handleAddPinned(e), n.pinned = !n.pinned), n
                         }));
                         this.setState({
                             environments: t
@@ -3687,68 +3901,149 @@
                         onChange: this.handleImageUpload
                     })), this.state.img !== ve && s().createElement(v.Button, {
                         variant: "contained",
                         sx: {
                             backgroundColor: "#673ab7!important"
                         },
                         onClick: this.handleImageUploadBoxClose
-                    }, "Save"))), this.renderInstalledEnvironments = () => (this.state.environments.sort(((e, t) => e.pinned || t.pinned ? !e.pinned - !t.pinned : (t.priority || 0) - (e.priority || 0))), this.state.environments.filter((e => e.installed)).length < 1 ? s().createElement(ie, null) : this.state.environments.filter((e => e.installed)).map(((e, t) => {
-                        let n = e.active,
-                            i = this.state.installingEnvironment && (this.state.installingEnvironment._id === e._id || this.state.newEnvSlug === (null == e ? void 0 : e.slug));
+                    }, "Save"))), this.renderInstalledEnvironments = () => (this.state.environments.sort(((e, t) => e.pinned || t.pinned ? !e.pinned - !t.pinned : (t.priority || 0) - (e.priority || 0))), this.state.environments.filter((e => e.installed)).length < 1 ? s().createElement(ie, null) : this.state.environments.filter((e => e.installed)).map((e => {
+                        let t = e.active,
+                            n = this.state.installingEnvironment && (this.state.installingEnvironment._id === e._id || this.state.newEnvSlug === (null == e ? void 0 : e.slug));
                         return s().createElement(N, {
                             qbUser: this.state.qbUser,
-                            key: t,
+                            key: e._id,
                             expandedEnvs: this.state.expandedEnvs,
                             onTogglePinned: this.onTogglePinned,
                             onToggleExpand: this.onToggleExpand,
                             environment: e,
-                            isActive: n,
+                            isActive: t,
                             isNewEnv: e._id === this.state.newCustomEnvId,
-                            isInstalling: i,
-                            isInstalled: !i,
+                            isInstalling: n,
+                            isInstalled: !n,
                             activateButton: s().createElement("p", {
                                 className: "env-action",
                                 style: {
                                     width: "100%",
                                     marginRight: 10,
-                                    background: i ? `linear-gradient(to right ,#673AB7 ${this.state.progress}% , #9070C8 0%)` : "#673AB7",
-                                    cursor: i || "qbraid_000000" === e.slug ? "not-allowed" : "pointer"
+                                    background: n ? `linear-gradient(to right ,#673AB7 ${this.state.progress}% , #9070C8 0%)` : "#673AB7",
+                                    cursor: n || "qbraid_000000" === e.slug ? "not-allowed" : "pointer"
                                 },
                                 onClick: () => {
                                     this.handleCheckAndActivateEnv(e)
                                 }
-                            }, i ? "Installing..." : n ? "Remove kernel" : "Add kernel"),
-                            edit: () => this.handleOpenEnvEditorInstalled(e, i),
+                            }, n ? "Installing..." : t ? "Remove kernel" : "Add kernel"),
+                            edit: () => this.handleOpenEnvEditorInstalled(e, n),
                             flux: this.props.flux,
                             packageInstallingEnv: this.state.packageInstallingEnv,
                             packageProgress: this.state.packageProgress,
                             cloneEnvironment: this.cloneEnvironment,
                             isDarkTheme: this.state.isDarkTheme
                         })
                     }))), this.updateReadUserAccessData = e => {
                         const t = this.state.environments.filter((t => t._id === e));
                         this.setState({
                             selectedEnvironment: Object.assign(Object.assign({}, this.state.selectedEnvironment), {
                                 readAccessUsers: t[0].readAccessUsers
                             })
                         })
+                    }, this.handleAccessCodeVisibility = () => {
+                        this.setState((e => ({
+                            accessCodeInputVisible: !e.accessCodeInputVisible
+                        })))
+                    }, this.handleAccessCodeInputChange = e => {
+                        this.setState({
+                            accessCodeInput: e.target.value
+                        })
+                    }, this.handleDiscoverEnvWithAccessCode = () => {
+                        "" !== this.state.accessCodeInput && (this.setState({
+                            accessCodeLoading: !0
+                        }), this.props.flux.getActions("EnvironmentActions").searchAccessCodeAndAccept(this.state.accessCodeInput).then((e => {
+                            200 === (null == e ? void 0 : e.status) && (this.setState({
+                                accessCodeInput: "",
+                                accessCodeLoading: !1
+                            }), this.handleOpenPopup("Access Code redeemed!", "success"), this.handleRefreshEnvironments({
+                                clickedRefresh: !1
+                            }))
+                        })).catch((e => {
+                            var t, n;
+                            this.handleOpenPopup(null === (n = null === (t = null == e ? void 0 : e.response) || void 0 === t ? void 0 : t.body) || void 0 === n ? void 0 : n.message, "error"), this.setState({
+                                accessCodeLoading: !1
+                            })
+                        })))
                     }, this.renderUninstalledEnvironments = () => {
                         let e = this.state.filterQuery || this.state.tagFilter ? this.state.filteredEnvironments : this.state.environments;
-                        return e.sort(((e, t) => this.compareEnvs(e, t))), [s().createElement("div", {
+                        return e.sort(((e, t) => this.compareEnvs(e, t))), [s().createElement(v.Box, {
+                            m: "10px"
+                        }, s().createElement(v.Paper, {
+                            elevation: 0,
+                            sx: e => ({
+                                display: "flex",
+                                flexDirection: "row",
+                                flex: 1,
+                                borderWidth: "1px",
+                                borderStyle: "solid",
+                                borderColor: e.palette.grey[400],
+                                backgroundColor: e.palette.background.default,
+                                "&:hover": {
+                                    borderColor: `${e.palette.action}!important`
+                                },
+                                "&:focus-within, &:focus-visible": {
+                                    borderColor: e.palette.primary.main,
+                                    outline: `1px solid ${e.palette.primary.main}`
+                                }
+                            })
+                        }, s().createElement(v.InputBase, {
+                            sx: {
+                                ml: 1,
+                                flex: 1,
+                                fontSize: 18,
+                                fontWeight: 400
+                            },
+                            inputProps: {
+                                style: {
+                                    height: "19px",
+                                    fontSize: "14px"
+                                }
+                            },
+                            value: this.state.accessCodeInput,
+                            placeholder: "Discover via access code...",
+                            onChange: this.handleAccessCodeInputChange,
+                            type: this.state.accessCodeInputVisible ? "text" : "password"
+                        }), s().createElement(v.IconButton, {
+                            size: "small",
+                            onClick: this.handleAccessCodeVisibility
+                        }, this.state.accessCodeInputVisible ? s().createElement(z.Visibility, {
+                            fontSize: "inherit"
+                        }) : s().createElement(z.VisibilityOff, {
+                            fontSize: "inherit"
+                        })), s().createElement(v.Button, {
+                            color: "secondary",
+                            variant: "contained",
+                            size: "small",
+                            sx: {
+                                fontSize: 14,
+                                textTransform: "inherit",
+                                ml: 1,
+                                cursor: this.state.accessCodeLoading ? "wait" : "pointer"
+                            },
+                            onClick: this.handleDiscoverEnvWithAccessCode,
+                            disabled: this.state.accessCodeLoading
+                        }, s().createElement(z.AddCircleOutline, null)))), s().createElement("div", {
                             className: "environments-sidebar-create-env",
                             onClick: this.handleNewEnvironmentClick
                         }, s().createElement("p", {
                             style: {
                                 marginRight: 8,
                                 fontSize: 24,
                                 paddingBottom: 4
                             }
-                        }, "+"), s().createElement("p", null, "Create Environment"))].concat(e.filter((e => !e.installed)).map(((e, t) => s().createElement(N, {
+                        }, "+"), s().createElement("p", null, "Create Environment"))].concat(e.filter((e => !e.installed)).map((e => s().createElement(N, {
                             qbUser: this.state.qbUser,
-                            key: t,
+                            key: e._id,
+                            expandedEnvs: this.state.expandedEnvs,
                             onToggleExpand: this.onToggleExpand,
                             onTogglePinned: this.onTogglePinned,
                             environment: e,
                             isInstalling: !1,
                             isNewEnv: !1,
                             isInstalled: !1,
                             verifyLoading: this.state.verifyLoading,
@@ -3848,16 +4143,16 @@
                         },
                         imgAsIpykernelLogo: !1,
                         popupOpen: !1,
                         popupMsg: {
                             msg: "",
                             type: ""
                         },
-                        currentTheme: (null === (a = null === (i = null === (n = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === n ? void 0 : n.getAttribute("data-jp-theme-name")) || void 0 === i ? void 0 : i.toLowerCase()) || void 0 === a ? void 0 : a.includes("dark")) ? ee : K,
-                        isDarkTheme: !!(null === (c = null === (l = null === (o = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === o ? void 0 : o.getAttribute("data-jp-theme-name")) || void 0 === l ? void 0 : l.toLowerCase()) || void 0 === c ? void 0 : c.includes("dark")),
+                        currentTheme: (null === (a = null === (i = null === (n = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === n ? void 0 : n.getAttribute("data-jp-theme-name")) || void 0 === i ? void 0 : i.toLowerCase()) || void 0 === a ? void 0 : a.includes("dark")) ? ee : X,
+                        isDarkTheme: !!(null === (c = null === (l = null === (r = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === r ? void 0 : r.getAttribute("data-jp-theme-name")) || void 0 === l ? void 0 : l.toLowerCase()) || void 0 === c ? void 0 : c.includes("dark")),
                         newCustomEnvId: null,
                         refreshEnvData: !1,
                         makeNewEnv: !1,
                         timeToInstall: 0,
                         showFilter: !1,
                         sortBy: "highest_to_lowest_priority",
                         tagFilter: !1,
@@ -3869,15 +4164,18 @@
                         },
                         intelPermissionModal: !1,
                         currentEnv: null,
                         returnToMyenv: !1,
                         expandedEnvs: [],
                         noUser: !(null === (d = e.flux.getStore("UserStore").getState()) || void 0 === d ? void 0 : d.user),
                         packageLoading: !1,
-                        containerWidth: 300
+                        containerWidth: 300,
+                        accessCodeInput: "",
+                        accessCodeInputVisible: !1,
+                        accessCodeLoading: !1
                     }
                 }
                 getChildContext() {
                     const {
                         flux: e
                     } = this.props;
                     return {
@@ -3892,28 +4190,28 @@
                     this.props.flux.getStore("EnvironmentStore").listen(this.handleUpdateEnvironments);
                     let n = document.getElementsByTagName("BODY")[0];
                     new MutationObserver((() => {
                         n.getAttribute("data-jp-theme-name").toLowerCase().includes("dark") ? this.setState({
                             currentTheme: ee,
                             isDarkTheme: !0
                         }) : this.setState({
-                            currentTheme: K,
+                            currentTheme: X,
                             isDarkTheme: !1
                         })
                     })).observe(n, {
                         attributesFilter: ["data-jp-theme-name"],
                         attributeOldValue: !0
                     }), this.setState({
                         containerWidth: null === (t = null === (e = this.aceContainerRef) || void 0 === e ? void 0 : e.current) || void 0 === t ? void 0 : t.offsetWidth
                     })
                 }
                 componentDidUpdate(e, t) {
-                    var n, i, a, s, r;
+                    var n, i, a, s, o;
                     (null === (i = null === (n = this.aceContainerRef) || void 0 === n ? void 0 : n.current) || void 0 === i ? void 0 : i.offsetWidth) !== (null === (a = null == this ? void 0 : this.state) || void 0 === a ? void 0 : a.containerWidth) && (this.resizeEditor(), this.setState({
-                        containerWidth: null === (r = null === (s = this.aceContainerRef) || void 0 === s ? void 0 : s.current) || void 0 === r ? void 0 : r.offsetWidth
+                        containerWidth: null === (o = null === (s = this.aceContainerRef) || void 0 === s ? void 0 : s.current) || void 0 === o ? void 0 : o.offsetWidth
                     }))
                 }
                 componentWillUnmount() {
                     this.props.flux.getStore("EnvironmentStore").unlisten(this.handleUpdateEnvironments)
                 }
                 render() {
                     return s().createElement(v.ThemeProvider, {
@@ -3946,15 +4244,17 @@
                             display: "inline-flex"
                         }
                     }, "My Environments", s().createElement("div", {
                         style: {
                             transition: "transform 1s",
                             transform: `rotateZ(${180*this.state.togglesCount+"deg"})`
                         },
-                        onClick: this.handleRefreshEnvironments,
+                        onClick: () => this.handleRefreshEnvironments({
+                            clickedRefresh: !0
+                        }),
                         className: "div-refresh-btn"
                     }, s().createElement(G, null)))), s().createElement("span", {
                         className: "environments-sidebar-add-btn",
                         style: this.state.browsing ? {
                             opacity: 0,
                             cursor: "default"
                         } : this.state.noUser ? {
@@ -3992,20 +4292,20 @@
                         sx: {
                             "& .MuiOutlinedInput-root": {
                                 "&.Mui-focused fieldset": {
                                     borderColor: "#d30982"
                                 },
                                 paddingLeft: "10px",
                                 paddingRight: "10px"
-                            },
-                            fontSize: "14px"
+                            }
                         },
                         inputProps: {
                             style: {
-                                height: "19px"
+                                height: "19px",
+                                fontSize: "14px"
                             }
                         },
                         InputProps: {
                             startAdornment: s().createElement(v.InputAdornment, {
                                 position: "start"
                             }, s().createElement(v.IconButton, {
                                 "aria-label": "search icon",
@@ -4034,15 +4334,15 @@
                                 arrow: !0
                             }, s().createElement(v.IconButton, {
                                 "aria-label": "filter icon",
                                 edge: "end",
                                 onClick: () => this.setState((e => ({
                                     showFilter: !e.showFilter
                                 })))
-                            }, s().createElement(_.FilterList, null))))
+                            }, s().createElement(z.FilterList, null))))
                         },
                         variant: "outlined",
                         fullWidth: !0,
                         onChange: this.handleChangeFilterQuery,
                         value: this.state.filterQuery
                     })), this.state.showFilter && s().createElement(v.Grid, {
                         item: !0,
@@ -4335,15 +4635,15 @@
                                 height: "80%"
                             }
                         }
                     }), s().createElement("button", {
                         className: "envSidebar-custom-button envSidebar-flex-btn envSidebar-btn-upload " + (this.state.newEnvName.length < 1 ? "envSidebar-btn-disabled" : ""),
                         onClick: this.handleImageUploadBoxOpen,
                         disabled: this.state.newEnvName.length < 1
-                    }, "Upload Icon", s().createElement(_.FileUpload, {
+                    }, "Upload Icon", s().createElement(z.FileUpload, {
                         fontSize: "16px"
                     })), this.renderImageUploadModal()), s().createElement("p", {
                         className: "environment-editor-section-label"
                     }, "Python Packages", " ", s().createElement("span", {
                         style: {
                             color: "var(--jp-layout-color4)"
                         }
@@ -4353,20 +4653,20 @@
                             fontSize: "0.7em",
                             marginTop: "5px",
                             marginLeft: "10px"
                         }
                     }, "Warning: Environment creation will fail in the case of dependency conflicts or installation errors."), s().createElement("div", {
                         ref: this.aceContainerRef,
                         className: `environment-editor-ace-wrapper ${this.state.newEnvFormHelperTexts.newEnvCode.length&&"environment-editor-ace-wrapper-error"}`
-                    }, s().createElement(Y(), {
+                    }, s().createElement(K(), {
                         ref: this.aceRef,
                         onChange: this.handleChangeCode,
                         placeholder: "# requirements.txt",
                         mode: "python",
-                        theme: this.state.currentTheme === K ? "github" : "monokai",
+                        theme: this.state.currentTheme === X ? "github" : "monokai",
                         name: "newEnvCode",
                         style: {
                             position: "relative",
                             flex: 1,
                             paddingBottom: 60,
                             margin: 0,
                             maxHeight: "unset",
@@ -4431,23 +4731,23 @@
                                 padding: "6px 14px 6px 0px",
                                 fontSize: "14px",
                                 height: "28px",
                                 textTransform: "lowercase"
                             }
                         },
                         inputProps: {
-                            maxLength: 80
+                            maxLength: 30
                         }
                     }), s().createElement("div", {
                         className: "text-area-warning"
                     }, s().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvKernelName.length >= 80 && "Max length = 80"), s().createElement("p", {
-                        className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvKernelName.length>=80&&"text-area-error-text"}`
-                    }, 80 - this.state.newEnvKernelName.length))), s().createElement(v.Grid, {
+                    }, this.state.newEnvKernelName.length >= 30 && "Max length = 30"), s().createElement("p", {
+                        className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvKernelName.length>=30&&"text-area-error-text"}`
+                    }, 30 - this.state.newEnvKernelName.length))), s().createElement(v.Grid, {
                         item: !0,
                         xs: 12
                     }, s().createElement(v.Typography, {
                         variant: "subtitle2",
                         fontSize: 12,
                         fontWeight: 400,
                         color: "var(--jp-layout-color4)",
@@ -4476,23 +4776,23 @@
                                 padding: "6px 14px 6px 0px",
                                 fontSize: "14px",
                                 height: "28px",
                                 textTransform: "lowercase"
                             }
                         },
                         inputProps: {
-                            maxLength: 80
+                            maxLength: 20
                         }
                     }), s().createElement("div", {
                         className: "text-area-warning"
                     }, s().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvShellPrompt.length >= 80 && "Max length = 80"), s().createElement("p", {
-                        className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvShellPrompt.length>=80&&"text-area-error-text"}`
-                    }, 80 - this.state.newEnvShellPrompt.length))), s().createElement(v.Grid, {
+                    }, this.state.newEnvShellPrompt.length >= 20 && "Max length = 20"), s().createElement("p", {
+                        className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvShellPrompt.length>=20&&"text-area-error-text"}`
+                    }, 20 - this.state.newEnvShellPrompt.length))), s().createElement(v.Grid, {
                         item: !0,
                         xs: 12
                     }, s().createElement(v.FormControl, {
                         fullWidth: !0
                     }, s().createElement(v.Select, {
                         onChange: e => {
                             e.preventDefault(), this.state.pythonVersions.filter((t => t.label === e.target.value))[0].isLocked || this.setState({
@@ -4545,15 +4845,15 @@
                         disabled: this.state.installingEnvironment
                     }, s().createElement(H.Z, {
                         fontSize: "16px"
                     }), this.state.makeNewEnv ? "Creating..." : "Create"))))), this.renderIntelTermsAndConditionModal(), this.renderUpgradeDialogue(), this.renderPopupMsg(this.state.popupMsg)))
                 }
             }
             ye.childContextTypes = c;
-            class we extends r.ReactWidget {
+            class we extends o.ReactWidget {
                 constructor(e, t) {
                     super(), this.flux = e, this.app = t
                 }
                 render() {
                     return s().createElement(ye, {
                         flux: this.flux,
                         app: this.app
@@ -4611,19 +4911,19 @@
                         }))
                     }))), this.toggleActive = e => (this.alt.dispatch(this), new Promise(((t, n) => {
                         let i = this.alt.getStore("EnvironmentStore").getState().environmentCache[e];
                         if (!i) return n("No environment with id " + e);
                         let a = this.alt.getStore("EnvironmentStore").getState().installingEnvironment;
                         if (a && i.slug === a.slug) return n("Cannot activate environment while it is being installed");
                         let s = i.active,
-                            r = {
+                            o = {
                                 slug: i.slug
                             };
                         this.alt.getActions("JupyterApiActions").query("toggle-kernel", {
-                            body: JSON.stringify(r),
+                            body: JSON.stringify(o),
                             method: "POST"
                         }).then((n => {
                             if (this.alt.jupyterlab) {
                                 let e = this.alt.jupyterlab.serviceManager.kernelspecs;
                                 e.refreshSpecs().then((() => {
                                     e.specs.default && this.alt.jupyterlab.serviceManager.sessions._sessionConnections.forEach((t => {
                                         try {
@@ -4669,20 +4969,20 @@
                                     n(e)
                                 } else t(i.body.canUpdate)
                             }))
                         }));
                         return new Promise(((n, i) => {
                             let a = this.alt.getStore("EnvironmentStore").getState().environmentCache[e],
                                 s = null === a.systemSitePackages || a.systemSitePackages,
-                                r = {
+                                o = {
                                     slug: a.slug,
                                     systemSitePackages: Number(s)
                                 };
                             this.alt.getActions("JupyterApiActions").query("pip-freeze", {
-                                body: JSON.stringify(r),
+                                body: JSON.stringify(o),
                                 method: "POST"
                             }).then((a => {
                                 t(e).then((t => {
                                     let i = this.alt.getStore("EnvironmentStore").getState().environments;
                                     i = i.map((n => {
                                         var i;
                                         return n._id === e && (n.packagesInImage = null !== (i = null == a ? void 0 : a.packages) && void 0 !== i ? i : n.packagesInImage, n.canUpdate = t), n
@@ -4722,22 +5022,22 @@
                                 this.alt.getActions("JupyterApiActions").query("installed-environments", {
                                     method: "GET"
                                 }).then((n => {
                                     const {
                                         installed: i,
                                         active: a,
                                         installing: s,
-                                        quantumJobs: r,
-                                        quantumJobsEnabled: o,
+                                        quantumJobs: o,
+                                        quantumJobsEnabled: r,
                                         sysPython: l
                                     } = n, c = this.alt.getStore("EnvironmentStore").getState().environments;
                                     (null == i ? void 0 : i.includes(s)) || this.actions._registerInstalling(null);
                                     const d = c.reduce(((t, n) => {
                                         var c, d, p, h, m, g;
-                                        return n.installed = null !== (c = null == i ? void 0 : i.includes(n.slug)) && void 0 !== c && c, n.active = null !== (d = null == a ? void 0 : a.includes(n.slug)) && void 0 !== d && d, n.pinned = null !== (p = null == e ? void 0 : e.includes(n.slug)) && void 0 !== p && p, n.quantumJobs = null !== (h = null == r ? void 0 : r.includes(n.slug)) && void 0 !== h && h, n.quantumJobsEnabled = null !== (m = null == o ? void 0 : o.includes(n.slug)) && void 0 !== m && m, n.sysPython = null !== (g = null == l ? void 0 : l.includes(n.slug)) && void 0 !== g && g, n.slug === s && this.actions._registerInstalling(n), !n.installed && n.isPreInstalled || t.push(n), t
+                                        return n.installed = null !== (c = null == i ? void 0 : i.includes(n.slug)) && void 0 !== c && c, n.active = null !== (d = null == a ? void 0 : a.includes(n.slug)) && void 0 !== d && d, n.pinned = null !== (p = null == e ? void 0 : e.includes(n.slug)) && void 0 !== p && p, n.quantumJobs = null !== (h = null == o ? void 0 : o.includes(n.slug)) && void 0 !== h && h, n.quantumJobsEnabled = null !== (m = null == r ? void 0 : r.includes(n.slug)) && void 0 !== m && m, n.sysPython = null !== (g = null == l ? void 0 : l.includes(n.slug)) && void 0 !== g && g, n.slug === s && this.actions._registerInstalling(n), !n.installed && n.isPreInstalled || t.push(n), t
                                     }), []);
                                     this.actions._updateAll(d), t(d)
                                 })).catch((e => {
                                     n(e)
                                 }))
                             })).catch((e => {
                                 n(e)
@@ -4879,25 +5179,26 @@
                             let n = e.status;
                             e.message, t(n)
                         })).catch((e => {
                             console.log(`Uninstall Error: ${e}`), n(e)
                         }))
                     }))), this.shareEnvironment = e => (this.alt.dispatch(this), new Promise(((t, n) => {
                         if (!e.environmentId) return n("Must provide environment id");
-                        if (!e.collabEmail) return n("Must provide qBraid collaborator email");
+                        if (!e.collabEmail && !e.isAccessKeyEnv) return n("Must provide qBraid collaborator email");
                         let i = this.alt.getStore("EnvironmentStore").getState().environmentCache[e.environmentId];
                         if (!i) return n("No environment with id " + environmentId);
                         if (!i.slug) return n("Environment is missing a slug value");
                         if (!i.installed) return n("Environment must be installed to share");
                         let a = {
-                            slug: `${i.slug}`,
-                            collabEmail: `${e.collabEmail}`,
-                            overwrite: `${e.overwrite}`
+                            slug: i.slug,
+                            collabEmail: null == e ? void 0 : e.collabEmail,
+                            overwrite: (null == e ? void 0 : e.overwrite) || !1,
+                            isAccessKeyEnv: (null == e ? void 0 : e.isAccessKeyEnv) || !1
                         };
-                        e.hasOwnProperty("overwrite") && (a.overwrite = e.overwrite), this.alt.getActions("ApiActions").query().post("/environments/share").send(a).end(((e, i) => {
+                        this.alt.getActions("ApiActions").query().post("/environments/share").send(a).end(((e, i) => {
                             if (e) return console.log(e), n({
                                 status: i.status,
                                 message: e
                             });
                             if (200 !== i.status && 202 !== i.status && 304 !== i.status) return console.log(`Share environment action rejected, status: ${i.status}`), n({
                                 status: i.status,
                                 message: JSON.stringify(i.body)
@@ -4926,21 +5227,21 @@
                                     console.log(e), n(e)
                                 }))
                             }));
                         return new Promise(((e, n) => {
                             let i = 0,
                                 a = null,
                                 s = null,
-                                r = null;
-                            setTimeout((function o() {
+                                o = null;
+                            setTimeout((function r() {
                                 t().then((t => {
-                                    a = 1 === (null == t ? void 0 : t.complete), s = 1 === (null == t ? void 0 : t.success) || 0 !== (null == t ? void 0 : t.success) && s, r = t.message ? t.message : "", a ? e({
+                                    a = 1 === (null == t ? void 0 : t.complete), s = 1 === (null == t ? void 0 : t.success) || 0 !== (null == t ? void 0 : t.success) && s, o = t.message ? t.message : "", a ? e({
                                         success: s,
-                                        message: r
-                                    }) : ++i > 100 ? n("Timeout exceeded while polling install status") : setTimeout(o, 5e3)
+                                        message: o
+                                    }) : ++i > 100 ? n("Timeout exceeded while polling install status") : setTimeout(r, 5e3)
                                 })).catch((e => n(e)))
                             }), 5e3)
                         }))
                     }, this.uninstall = e => {
                         this.alt.dispatch(this);
                         let t = this.alt.getStore("EnvironmentStore").getState().installingEnvironment;
                         t && e === t.slug && this.actions._registerInstalling(null);
@@ -4989,39 +5290,59 @@
                                 202 === (null == e ? void 0 : e.status) || 200 === (null == e ? void 0 : e.status) ? t(e.message) : n(e.message)
                             })).catch((e => {
                                 n(e)
                             }))
                         } catch (e) {
                             console.log(e), n(e)
                         }
+                    }))), this.generateAccessKey = e => (this.alt.dispatch(this), new Promise(((t, n) => {
+                        try {
+                            this.alt.getActions("ApiActions").query().post(`/environments/access-key/${e}`).then((e => {
+                                200 === (null == e ? void 0 : e.status) ? t(e) : n(e.message)
+                            })).catch((e => {
+                                n(e)
+                            }))
+                        } catch (e) {
+                            console.log(e), n(e)
+                        }
+                    }))), this.searchAccessCodeAndAccept = e => (this.alt.dispatch(this), new Promise(((t, n) => {
+                        try {
+                            this.alt.getActions("ApiActions").query().put(`/environments/permissions/${e}`).then((e => {
+                                200 === (null == e ? void 0 : e.status) ? t(e) : n(e.message)
+                            })).catch((e => {
+                                n(e)
+                            }))
+                        } catch (e) {
+                            console.log(e), n(e)
+                        }
                     })))
                 };
             var Ne = n(2046),
                 Te = n(4582);
 
             function je() {
                 this.registerAlt = e => {
                     this.alt = e
                 }, this.query = (e, t) => new Promise((async (n, i) => {
                     const a = Te.ServerConnection.makeSettings(),
                         s = Ne.URLExt.join(a.baseUrl, "jupyter-environment-manager", e);
-                    let r;
+                    let o;
                     try {
-                        r = await Te.ServerConnection.makeRequest(s, t, a)
+                        o = await Te.ServerConnection.makeRequest(s, t, a)
                     } catch (e) {
                         console.log(e), i(e)
                     }
-                    const o = await r.json();
-                    r.ok || i({
-                        response: r,
-                        data: o
-                    }), n(o)
+                    const r = await o.json();
+                    o.ok || i({
+                        response: o,
+                        data: r
+                    }), n(r)
                 }))
             }
-            const Oe = function() {
+            const Ue = function() {
                     this.registerAlt = e => {
                         this.alt = e, this.actions = e.getActions(this.__proto__.constructor.__proto__.name)
                     }, this._updateUser = e => e, this._updateConfig = e => e, this._updateIsMount = e => e, this.getUser = () => (this.alt.dispatch(this), new Promise(((e, t) => {
                         this.alt.getActions("ApiActions").query().get("/identity").end(((t, n) => {
                             t ? (this.actions._updateUser(null), e(null)) : (this.actions._updateUser(n.body), e(n.body))
                         }))
                     }))), this.getLocalConfig = () => (this.alt.dispatch(this), new Promise(((e, t) => {
@@ -5068,15 +5389,15 @@
                                 message: "User session verification complete."
                             })
                         } catch (t) {
                             console.error(t), e(null)
                         }
                     })))
                 },
-                Ue = function e() {
+                Oe = function e() {
                     this.state = {
                         isAuthenticated: !1,
                         user: null
                     }, e.prototype.handleUpdateUser = e => {
                         this.setState({
                             isAuthenticated: !0,
                             user: e
@@ -5119,15 +5440,15 @@
                         _registerInstalling: n
                     } = this.alt.getActions("EnvironmentActions");
                     this.bindListeners({
                         handleUpdateAll: t,
                         handleRegisterInstalling: n
                     })
                 },
-                _e = function e() {
+                ze = function e() {
                     this.state = {
                         user: null,
                         config: null,
                         isMount: null
                     }, e.prototype.handleUpdateUser = e => {
                         this.setState({
                             user: e
@@ -5148,22 +5469,22 @@
                     } = this.alt.getActions("UserActions");
                     this.bindListeners({
                         handleUpdateUser: t,
                         handleUpdateConfig: n,
                         handleUpdateIsMount: i
                     })
                 };
-            class ze extends(Se()) {
+            class _e extends(Se()) {
                 constructor(e) {
                     super(), this.registerAltWithActions = () => {
                         for (const e in this.actions) "global" !== e && this.actions[e].registerAlt(this)
-                    }, this.apiBaseUrl = e.apiBaseUrl, this.jupyterlab = e.jupyterlab, this.addActions("ApiActions", k), this.addActions("AuthActions", Ie), this.addActions("EnvironmentActions", Pe), this.addActions("JupyterApiActions", je), this.addActions("UserActions", Oe), this.registerAltWithActions(), this.addStore("AuthStore", Ue), this.addStore("EnvironmentStore", Le), this.addStore("UserStore", _e)
+                    }, this.apiBaseUrl = e.apiBaseUrl, this.jupyterlab = e.jupyterlab, this.addActions("ApiActions", k), this.addActions("AuthActions", Ie), this.addActions("EnvironmentActions", Pe), this.addActions("JupyterApiActions", je), this.addActions("UserActions", Ue), this.registerAltWithActions(), this.addStore("AuthStore", Oe), this.addStore("EnvironmentStore", Le), this.addStore("UserStore", ze)
                 }
             }
-            const De = ze,
+            const De = _e,
                 qe = new i.LabIcon({
                     name: "environments-sidebar:icon",
                     svgstr: '<svg class="env_icon" height="512pt" viewBox="0 0 512 512" width="512pt" xmlns="http://www.w3.org/2000/svg" fill="white"><path d="m306 150c0-27.570312-22.429688-50-50-50s-50 22.429688-50 50 22.429688 50 50 50 50-22.429688 50-50zm-80 0c0-16.542969 13.457031-30 30-30s30 13.457031 30 30-13.457031 30-30 30-30-13.457031-30-30zm0 0"/><path d="m266.003906 150c0-5.523438-4.476562-10-10-10h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480469 10 10.003906 10c5.523438 0 10-4.476562 10-10zm0 0"/><path d="m110 402h-30v-31c0-5.515625 4.484375-10 10-10h20c5.523438 0 10-4.476562 10-10s-4.476562-10-10-10h-20c-16.542969 0-30 13.457031-30 30v31h-30c-16.542969 0-30 13.457031-30 30v50c0 16.542969 13.457031 30 30 30h80c16.542969 0 30-13.457031 30-30v-50c0-16.542969-13.457031-30-30-30zm10 80c0 5.515625-4.488281 10-10 10h-80c-5.515625 0-10-4.484375-10-10v-50c0-5.511719 4.484375-10 10-10h80c5.511719 0 10 4.488281 10 10zm0 0"/><path d="m482 402h-30v-31c0-16.542969-13.457031-30-30-30h-156v-41h13.332031c5.523438 0 10-4.476562 10-10v-23.828125c8.789063-2.515625 17.230469-6.015625 25.234375-10.464844l16.855469 16.855469c1.875 1.875 4.421875 2.929688 7.074219 2.929688s5.195312-1.054688 7.070312-2.929688l32.996094-33c3.90625-3.902344 3.90625-10.234375 0-14.140625l-16.855469-16.855469c4.445313-8.003906 7.945313-16.445312 10.460938-25.234375h23.832031c5.519531 0 10-4.476562 10-10v-46.667969c0-5.523437-4.480469-10-10-10h-23.828125c-2.511719-8.789062-6.015625-17.230468-10.464844-25.238281l16.855469-16.851562c1.875-1.875 2.929688-4.417969 2.929688-7.070313s-1.054688-5.195312-2.929688-7.070312l-32.996094-33c-1.875-1.875-4.421875-2.929688-7.074218-2.929688-2.652344 0-5.195313 1.054688-7.070313 2.929688l-16.851563 16.855468c-8.007812-4.449218-16.449218-7.949218-25.238281-10.464843v-23.824219c0-5.523438-4.476562-10-10-10h-46.664062c-5.523438 0-10 4.476562-10 10v23.828125c-8.789063 2.515625-17.230469 6.015625-25.234375 10.464844l-16.859375-16.859375c-1.875-1.875-4.417969-2.925782-7.070313-2.925782s-5.195312 1.050782-7.070312 2.925782l-33 33c-3.902344 3.902344-3.902344 10.234375 0 14.140625l16.859375 16.859375c-4.445313 8-7.945313 16.445312-10.460938 25.234375h-23.832031c-5.523438 0-10 4.476562-10 10v46.664062c0 5.523438 4.476562 10 10 10h23.828125c2.511719 8.789063 6.011719 17.230469 10.460937 25.238281l-16.855468 16.851563c-3.902344 3.90625-3.902344 10.238281 0 14.144531l33 33c1.875 1.875 4.417968 2.925782 7.070312 2.925782s5.195313-1.050782 7.070313-2.925782l16.855469-16.855468c8.003906 4.449218 16.445312 7.949218 25.234374 10.464843v23.824219c0 5.523438 4.476563 10 10 10h13.332032v41h-45.996094c-5.523438 0-10 4.476562-10 10s4.476562 10 10 10h45.996094v41h-29.996094c-16.542969 0-30 13.457031-30 30v50c0 16.542969 13.457031 30 30 30h79.996094c16.542968 0 30-13.457031 30-30v-50c0-16.542969-13.457032-30-30-30h-30v-41h156.003906c5.511719 0 10 4.484375 10 10v31h-30c-16.542969 0-30 13.457031-30 30v50c0 13.65625 9.242188 25.601562 22.476562 29.039062 5.347657 1.390626 10.808594-1.816406 12.195313-7.160156 1.390625-5.347656-1.816406-10.804687-7.160156-12.195312-4.425781-1.148438-7.511719-5.132813-7.511719-9.683594v-50c0-5.511719 4.484375-10 10-10h80c5.511719 0 10 4.488281 10 10v50c0 4.554688-3.09375 8.535156-7.519531 9.683594-5.34375 1.390625-8.550781 6.847656-7.164063 12.195312 1.167969 4.5 5.226563 7.488282 9.671875 7.488282.832031 0 1.679688-.105469 2.519531-.324219 13.242188-3.4375 22.488282-15.382813 22.488282-29.042969v-50c.003906-16.542969-13.453125-30-29.996094-30zm-247.238281-153.40625c-11.921875-2.558594-23.179688-7.222656-33.453125-13.871094-3.957032-2.5625-9.167969-2.007812-12.503906 1.324219l-15.300782 15.304687-18.855468-18.855468 15.300781-15.304688c3.335937-3.332031 3.886719-8.542968 1.324219-12.503906-6.644532-10.269531-11.3125-21.527344-13.867188-33.449219-.988281-4.609375-5.0625-7.90625-9.777344-7.90625h-21.628906v-26.664062h21.636719c4.714843 0 8.789062-3.296875 9.777343-7.90625 2.554688-11.925781 7.21875-23.179688 13.863282-33.449219 2.5625-3.957031 2.011718-9.167969-1.324219-12.503906l-15.304687-15.304688 18.855468-18.855468 15.304688 15.304687c3.335937 3.335937 8.546875 3.886719 12.503906 1.324219 10.273438-6.644532 21.527344-11.3125 33.453125-13.871094 4.609375-.988281 7.902344-5.0625 7.902344-9.777344v-21.628906h26.664062v21.628906c0 4.714844 3.292969 8.789063 7.90625 9.777344 11.921875 2.554688 23.179688 7.222656 33.453125 13.871094 3.957032 2.558594 9.167969 2.007812 12.5-1.328125l15.304688-15.300781 18.855468 18.855468-15.304687 15.300782c-3.332031 3.335937-3.882813 8.546874-1.324219 12.503906 6.648438 10.273437 11.316406 21.527344 13.871094 33.453125.988281 4.609375 5.0625 7.902343 9.777344 7.902343h21.628906v26.667969h-21.636719c-4.714843 0-8.789062 3.292969-9.777343 7.90625-2.554688 11.921875-7.21875 23.179688-13.863282 33.449219-2.5625 3.957031-2.011718 9.167969 1.324219 12.5l15.304687 15.304688-18.855468 18.855468-15.304688-15.304687c-3.335937-3.332031-8.546875-3.886719-12.503906-1.324219-10.273438 6.648438-21.527344 11.316406-33.449219 13.871094-4.613281.988281-7.90625 5.0625-7.90625 9.777344v21.632812h-26.664062v-21.628906c0-4.714844-3.292969-8.789063-7.90625-9.777344zm71.238281 183.40625v50c0 5.511719-4.484375 10-10 10h-80c-5.515625 0-10-4.488281-10-10v-50c0-5.515625 4.484375-10 10-10h80c5.515625 0 10 4.488281 10 10zm0 0"/><path d="m155.003906 341h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480469 10 10.003906 10c5.523438 0 10-4.476562 10-10s-4.476562-10-10-10zm0 0"/><path d="m442 492h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480468 10 10.003906 10 10-4.476562 10-10-4.476562-10-10-10zm0 0"/></svg>'
                 }),
                 Be = (e, t) => {
                     const n = new we(e, t);
                     return n.id = "environments-sidebar", n.title.label = "ENVS", n.title.caption = "Environment Manager", n.title.className = "environment_sidebar_li", n.title.icon = qe, n.title.iconClass = "env_icon_parent", n
@@ -5177,32 +5498,32 @@
                         } = e, i = new De({
                             apiBaseUrl: w,
                             jupyterlab: e
                         });
                         try {
                             const a = i.getActions("AuthActions"),
                                 s = i.getActions("UserActions"),
-                                r = i.getActions("EnvironmentActions");
+                                o = i.getActions("EnvironmentActions");
                             await a.getUser(), await s.getLocalConfig(), await s.getUser(), await s.checkFileMount();
                             try {
-                                await r.updateAll(), await r.registerInstalled(), s.verifyUserSession()
+                                await o.updateAll(), await o.registerInstalled(), s.verifyUserSession()
                             } catch (e) {
                                 console.error("Error updating environments", e)
                             }
-                            let o = Be(i, e);
-                            e.shell.add(o, "right", {
+                            let r = Be(i, e);
+                            e.shell.add(r, "right", {
                                 rank: 1
                             }), e.shell.activateById("environments-sidebar");
                             const l = "environment-manager:open-sidebar";
                             n.addCommand(l, {
                                 caption: "Environments",
                                 label: "Environments",
                                 icon: null,
                                 execute: () => {
-                                    o && o.dispose(), o = Be(i, e), e.shell.add(o, "right", {
+                                    r && r.dispose(), r = Be(i, e), e.shell.add(r, "right", {
                                         rank: 1
                                     }), e.shell.activateById("environments-sidebar")
                                 }
                             }), t && t.addItem({
                                 command: l,
                                 category: "qBraid Ecosystem",
                                 args: {
@@ -5211,15 +5532,15 @@
                             });
                             const c = "environment-manager:close-sidebar";
                             n.addCommand(c, {
                                 caption: "Environments",
                                 label: "Environments",
                                 icon: null,
                                 execute: () => {
-                                    o && o.dispose(), o = Be(i, e), e.shell.add(o, "right", {
+                                    r && r.dispose(), r = Be(i, e), e.shell.add(r, "right", {
                                         rank: 1
                                     })
                                 }
                             }), t && t.addItem({
                                 command: c,
                                 category: "qBraid Ecosystem",
                                 args: {
@@ -5236,15 +5557,15 @@
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
                 a = n.n(i)()((function(e) {
                     return e[1]
                 }));
-            a.push([e.id, ".env-editor {\n  /* position: fixed;\n  left: 50vw;\n  top: 50vh;\n  margin-left: -150px;\n  margin-top: -220px;\n  overflow: visible; */\n  width: 820px;\n  /* height: 87vh; */\n  position: relative;\n  margin-top: -40px;\n  padding-bottom: 0;\n  opacity: 0;\n  transition: margin-top 0.25s ease, opacity 0.25s ease;\n  border-radius: 20px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.editor-header {\n  text-align: center;\n  background: linear-gradient(120deg, #673ab7 10%, #9909e091 100%);\n  color: white;\n}\n\n.editor-scrollview {\n  height: 75vh;\n  /* height: calc(90vh - 122px); */\n  /* max-height: calc(90vh - 122px); /* leave room for 2 x 61px vertical bookend sections */\n  min-height: auto;\n  padding: 0px 10px;\n  overflow: auto;\n}\n\n.env-editor-col {\n  display: inline-block;\n  vertical-align: top;\n  width: 50%;\n}\n\n.env-editor-col-full {\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: white;\n  box-shadow: 0px 1px 4px -3px #000;\n  vertical-align: top;\n  display: flex;\n  margin: 0px 5px;\n}\n\n.env-editor-pane-new {\n  /* vertical-align: top; */\n  /* min-height: 180px; */\n  /* margin: 20px auto; */\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z2);\n  color: var(--jp-ui-font-color0);\n  height: 100%;\n  display: flex;\n  flex-direction: column;\n  justify-content: flex-start;\n}\n\n.env-editor-pane {\n  /* vertical-align: top; */\n  /* min-height: 180px; */\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z2);\n  color: var(--jp-ui-font-color0);\n  height: 100%;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  /* padding-bottom: 8px; */\n  /* #555 */\n}\n\n.env-editor-pane-title {\n  margin: 10px 0;\n  text-align: center;\n  font-size: 14px;\n}\n\n.env-info-input {\n  width: -webkit-fill-available;\n  width: -moz-available;\n  margin: 10px;\n  border: 1px solid var(--jp-border-color1);\n  background-color: var(--jp-input-background);\n  border-radius: 4px;\n  padding: 6px 10px;\n  color: var(--jp-ui-font-color1);\n  outline: none !important;\n  resize: none;\n  font-family: unset;\n  /* width:100%; */\n  box-sizing: border-box;\n}\n.env-info-input::placeholder {\n  font-style: italic;\n}\n\n.env-editor-input-data-text {\n  width: -webkit-fill-available;\n  margin: 10px !important;\n  border: 1px solid var(--jp-border-color1) !important;\n  background-color: var(--jp-input-background) !important;\n  border-radius: 4px !important;\n  /* padding: 6px 10px; */\n  color: var(--jp-ui-font-color1) !important;\n  outline: none !important;\n  resize: none !important;\n  font-family: unset !important;\n}\n\n.env-info-input:focus {\n  border: 1px solid #de2b8e;\n  background-color: var(--jp-input-active-background);\n}\n\n.env-info-input::placeholder {\n  color: #8e8e8e;\n}\n\n.env-info-input:-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-info-input::-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-pane-content {\n  margin: 15px 30px;\n  display: flex;\n  flex-direction: column;\n}\n\n.env-pane-label {\n  padding: 0;\n  font-weight: 500;\n  font-size: 14px;\n  text-align: left;\n  color: #424242;\n}\n\n.env-pane-prompt {\n  font-size: 14px;\n  color: #848484;\n  text-align: left;\n}\n\n.env-pane-share-holder {\n  width: 100%;\n  display: flex;\n  flex-direction: row;\n  justify-content: space-between;\n  align-items: center;\n}\n\n.env-pane-email {\n  border-radius: 5px !important;\n  border: 1px solid var(--jp-border-color1) !important;\n}\n.env-pane-email-error {\n  margin-top: 1em;\n  width: 100%;\n  color: lightcoral;\n}\n.env-pane-email-success {\n  margin-top: 1em;\n  width: 100%;\n  color: green;\n}\n.env-pane-email-normal {\n  margin-top: 0.5em;\n  width: 100%;\n  color: var(--jp-ui-font-color1);\n}\n.env-editor-pane-action {\n  font-size: 15px !important;\n  text-transform: none !important;\n  color: #f5f5f5 !important;\n}\n.env-pane-re-share {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.env-table {\n  width: 100%;\n  table-layout: fixed;\n}\n\n.env-table tbody {\n  display: block;\n  width: max-content;\n  overflow-y: auto;\n}\n\n.env-table th {\n  padding: 0;\n  font-weight: 500;\n  font-size: 14px;\n  text-align: left;\n  color: #424242;\n}\n\n.env-table td {\n  font-size: 14px;\n  text-align: left;\n  color: #6c6c6c;\n  padding: 6px 0;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n}\n\n.env-table-filter {\n  position: relative;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  height: 30px;\n  margin: 0;\n  padding: 0 !important;\n  overflow: visible !important;\n  border: none;\n}\n\n.env-table-filter input {\n  display: block;\n  width: 300px;\n  position: absolute;\n  /* top: 0; */\n  border: none !important;\n  outline: none !important;\n  color: #424242;\n}\n\n.env-table-filter input::placeholder {\n  color: #8e8e8e;\n}\n\n.env-table-filter input:-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-table-filter input::-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-editor-actions {\n  /* total height should be 61px, incluing the 1px border-bottom  */\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  width: 100%;\n  border-radius: 0 0 20px 20px;\n  border-top: 1px solid #696969;\n  /* border-top: 1px solid #aaa; */\n  background: linear-gradient(120deg, #35383a 10%, #5e5f61 100%);\n}\n\n.editor-action {\n  display: inline-block;\n  vertical-align: top;\n  width: 120px !important;\n  margin: 12px 10px !important;\n  padding: 9px 0 !important;\n}\n\n.editor-action-alt {\n  width: 100%;\n  margin: 10px auto;\n  padding: 9px 0;\n  border-radius: 6px;\n  text-align: center;\n  background-color: darkred;\n  color: white;\n  cursor: pointer;\n}\n\n.environment-editor {\n  display: flex;\n  flex-direction: column;\n  flex: 1;\n  overflow: hidden;\n}\n\n.environment-editor-section-label {\n  margin: 10px 0 2px 10px;\n  color: var(--jp-ui-font-color2);\n  font-size: 12px;\n}\n.environment-editor-code-error {\n  margin: 0px 0 2px 10px;\n  color: var(--jp-error-color1);\n  font-size: 12px;\n}\ntextarea {\n  resize: none;\n  font-family: unset;\n}\n.text-area-warning {\n  margin: 0px 10px;\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n}\n.text-area-warning-text {\n  margin: 0 !important;\n  color: indianred !important;\n}\n.text-area-error-text {\n  background: indianred !important;\n  color: white !important;\n  padding: 0 0.2em !important;\n  text-align: center !important;\n  border-radius: 0.3em !important;\n}\n.text-area-error-input {\n  outline: 1px solid indianred !important;\n  border-color: indianred !important;\n}\n.environment-editor-input {\n  margin: 5px 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  outline: transparent;\n  color: var(--jp-ui-font-color0);\n  background-color: var(--jp-layout-color1);\n  padding: 4px;\n  background-size: 16px;\n  box-sizing: content-box !important;\n  transition: border 0.2s linear;\n}\n\n.environment-editor-input:hover {\n  border-color: var(--jp-inverse-layout-color0);\n}\n\n.environment-editor-input:focus,\n.environment-editor-input:active,\n.environment-editor-input:focus-within {\n  outline: 1px solid #d30982;\n  border-color: #d30982;\n}\n\n.environment-editor-input.all_lowercase {\n  text-transform: lowercase;\n}\n\n.environment-editor-ace-wrapper {\n  position: relative;\n  border-radius: 4px;\n  overflow: auto;\n  width: 95%;\n  margin-inline: auto;\n  margin-block: 10px;\n  border: 1px solid var(--jp-border-color1);\n}\n.environment-editor-ace-wrapper-error {\n  border: 1px solid var(--jp-error-color1);\n}\n\n.environment-editor-save,\n.environment-editor-discard {\n  border: 1px solid #bdbdbd;\n  display: inline-block;\n  vertical-align: top;\n  width: calc(50% - 20px);\n  margin: 8px;\n  padding: 10px 0;\n  text-align: center;\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  transition: 200ms color ease, 200ms background-color ease;\n  cursor: pointer;\n  user-select: none;\n}\n\n.environment-editor-save {\n  background-color: var(--jp-layout-color3);\n}\n\n.environment-editor-save:hover {\n  color: #eee;\n  background-color: #46c146;\n}\n\n.environment-editor-active {\n  color: white;\n  background: linear-gradient(90deg, #673ab7 50%, #46c146 50%);\n  background-size: 200%;\n  background-position: left;\n  animation: bgAnimate 5s 1;\n}\n\n.environment-editor-discard:hover {\n  color: #e03333;\n}\n\n.env-pane-search-container {\n  display: flex;\n  flex-direction: column;\n  position: relative;\n}\n\n.env-pane-button-group {\n  display: flex;\n  flex: wrap;\n  justify-content: space-between;\n  gap: 1em;\n  margin-top: 10px;\n}\n\n.env-pane-button {\n  flex: 1;\n  height: 3em;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  background-color: transparent;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n  box-sizing: border-box;\n  font-size: 1em;\n}\n\n.outlined {\n  border-color: #673ab7;\n  color: #673ab7;\n  transition: color ease-in-out 150ms, border-color ease-in-out 150ms;\n}\n\n.outlined:hover {\n  border-color: indianred;\n  color: indianred;\n}\n\n.disabled {\n  background-color: lightgrey;\n  color: rgba(0, 0, 0, 0.6);\n  cursor: not-allowed;\n}\n\n.filled {\n  background-color: #673ab7 !important;\n  color: white !important;\n}\n\n.env-pane-searchbox {\n  width: -webkit-fill-available;\n  margin: 5px 0px;\n  border: 1px solid #aaa;\n  border-radius: 4px;\n  padding: 6px 10px;\n  color: var(--jp-ui-font-color1);\n  outline: none !important;\n  resize: none;\n  font-family: unset;\n  display: flex;\n  align-items: center;\n  height: 1.3em;\n  background-color: var(--jp-input-background);\n}\n\n.env-pane-searchbox:has(.env-page-input-bar:focus) {\n  background-color: var(--jp-input-active-background);\n}\n\n.env-pane-input-bar {\n  height: 1.5em;\n  width: 100%;\n  outline: none;\n  border: none;\n  background-color: transparent;\n  margin-inline: 0.5em;\n  color: inherit;\n}\n\n.env-pane-dropdown {\n  position: absolute;\n  height: auto;\n  top: 2.7em;\n  z-index: 50;\n  width: -webkit-fill-available;\n  background-color: var(--jp-layout-color2);\n  max-height: 250px;\n  min-height: 0;\n  display: flex;\n  flex-direction: row;\n  box-shadow: 0 0.25em 0.25em rgb(0 0 0 / 10%);\n  border-radius: 10px;\n}\n\n.env-pane-dropdown-list {\n  list-style: none;\n  display: flex;\n  flex-direction: column;\n  gap: 0.75em;\n  padding: 1em;\n  margin: 0 0 10px 0;\n  font-size: 1em;\n  font-weight: 400;\n  overflow-y: auto;\n  width: 100%;\n}\n\n.env-pane-dropdown-list > li {\n  background: var(--jp-layout-color1);\n  box-shadow: 0px 1px 4px -2px #555;\n  padding: 0.5em;\n  border-radius: 10px;\n  overflow: hidden;\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  gap: 1em;\n  min-height: 2.5em;\n  max-height: 3em;\n  cursor: pointer;\n  user-select: none;\n  transition: transform ease-in-out 200ms;\n}\n.env-pane-dropdown-over-ride {\n  min-height: 4.5em !important;\n}\n\n.env-pane-dropdown-list > li:hover {\n  transform: scale(1.01);\n}\n\n.env-pane-flexrow {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  gap: 0.25em;\n  line-height: 16px;\n  justify-content: space-between;\n  width: 100%;\n}\n\n.env-pane-flexcol {\n  display: flex;\n  flex-direction: column;\n  gap: 0.25em;\n  justify-content: space-between;\n}\n\n.env-pane-dropdown-name {\n  font-size: 16px;\n  font-weight: 600;\n}\n\n.env-pane-dropdown-desc {\n  font-size: 12px;\n}\n\n.env-pane-msg-popup {\n  position: absolute;\n  width: calc(100% - 3em);\n  margin: 0px 1em;\n  min-height: 2em;\n  max-height: 3em;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.warning {\n  background-color: rgb(179, 101, 13);\n  color: white;\n}\n\n.env-editor-tag-area {\n  width: calc(100% - 20px);\n  margin-inline: auto;\n  margin-bottom: 10px;\n}\n\n.env-tag-header {\n  margin-bottom: 5px;\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: flex-start;\n  gap: 10px;\n  min-height: 1.8em;\n}\n\n.env-slug-header {\n  margin-bottom: 5px;\n  display: flex;\n  flex-direction: row;\n  justify-content: flex-start;\n  gap: 10px;\n  min-height: 1.8em;\n}\n.env-tag-flex {\n  display: inline-flex !important;\n  flex-direction: row;\n  align-items: center;\n  justify-content: space-between;\n  gap: 5px;\n}\n\n.env-tag-icon {\n  width: 12px !important;\n  height: 12px !important;\n  color: currentColor;\n  cursor: pointer;\n}\n\n.env-add-tags {\n  display: flex;\n  flex-direction: row;\n  padding: 3px 3px 3px 6px;\n  align-items: center;\n  border-radius: 1.5em;\n  gap: 5px;\n  width: fit-content;\n}\n\n.env-plus-icon {\n  width: 16px !important;\n  height: 16px !important;\n  color: white;\n}\n\n.env-tags-input {\n  border-radius: 1em;\n  outline: none;\n  border: none;\n  padding: 2px 8px;\n  background: var(--jp-input-background);\n  color: var(--jp-ui-font-color0);\n  text-transform: lowercase;\n  width: 100%;\n  max-width: 100px;\n}\n\n.env-tags-input:active,\n.env-tags-input:focus {\n  background: var(--jp-input-active-background);\n}\n\n.env-edit-icon {\n  color: var(--jp-ui-font-color2);\n  width: 16px !important;\n  height: 16px !important;\n  cursor: pointer;\n}\n\n.env-jobs-toggle-area {\n  position: relative;\n  display: flex;\n  align-items: center;\n  width: calc(100% - 20px);\n  margin-inline: auto;\n  margin-bottom: 8px;\n  flex-wrap: wrap;\n}\n\n.env-jobs-toggle-switch-text {\n  font-weight: 500;\n}\n\n.env-unins-dialog-box #alert-dialog-title,\n.env-unins-dialog-box #alert-dialog-content,\n.env-unins-dialog-box #alert-dialog-description,\n.env-unins-dialog-box #alert-dialog-actions {\n  background-color: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color0);\n}\n\n.envSidebar-flex-container {\n  display: flex;\n  flex-wrap: wrap;\n  padding: 8px;\n  gap: 4px;\n}\n\n.envSidebar-flex-btn {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: center;\n  gap: 4px;\n}\n\n.envSidebar-btn-upload {\n  max-width: 120px;\n}\n\n.envSidebar-custom-button {\n  --fill-color1: #b767ff;\n  --fill-color2: #673ab7;\n  flex: 1;\n  height: 26px;\n  font-size: 14px;\n  outline: transparent;\n  border: none;\n  color: white;\n  border-radius: 4px;\n  background-image: linear-gradient(\n    110deg,\n    var(--fill-color1) 50%,\n    var(--fill-color2) 50%\n  );\n  background-size: 222%;\n  background-position: right;\n  transition: background-position 200ms linear, letter-spacing 200ms linear;\n  cursor: pointer;\n}\n\n.envSidebar-custom-button:hover {\n  background-position: left;\n  letter-spacing: 1.5px;\n  box-shadow: 0em 0em 0.2em var(--fill-color1);\n}\n\n.envSidebar-btn-discard {\n  --fill-color1: #d32f2f;\n  --fill-color2: transparent;\n  border: 1px solid #d32f2f;\n  color: #d32f2f;\n}\n.envSidebar-btn-discard:hover {\n  color: white;\n}\n.envSidebar-btn-save {\n  --fill-color1: #8ab73a;\n  --fill-color2: #673ab7;\n}\n.envSidebar-btn-delete {\n  --fill-color1: #562944;\n  --fill-color2: #d32f2f;\n}\n.envSidebar-btn-disabled {\n  --fill-color1: gray;\n  --fill-color2: gray;\n  cursor: not-allowed;\n}\n.envSidebar-btn-disabled:hover {\n  letter-spacing: normal !important;\n}\n\n.operator-selector {\n  width: 55px;\n  padding: 0.32em;\n  border-radius: 6px;\n  border: 1px solid #673ab7;\n  font-weight: 600;\n  color: #673ab7;\n}\n\n.package-selector::-webkit-scrollbar,\n.operator-selector::-webkit-scrollbar {\n  width: 6px;\n}\n.package-selector::-webkit-scrollbar-track,\n.operator-selector::-webkit-scrollbar-track {\n  background: transparent;\n}\n.package-selector::-webkit-scrollbar-thumb,\n.operator-selector::-webkit-scrollbar-track {\n  background-color: rgb(158, 156, 156);\n  border-radius: 20px;\n  border: transparent;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n}\n\n.env-edior-slide-in-top {\n  -webkit-animation: slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;\n  animation: ani-slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;\n}\n\n.shake-bottom {\n  -webkit-animation: shake-bottom 0.8s cubic-bezier(0.455, 0.03, 0.515, 0.955)\n    both;\n  animation: shake-bottom 0.8s cubic-bezier(0.455, 0.03, 0.515, 0.955) both;\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@-webkit-keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-top\n * ----------------------------------------\n */\n@-webkit-keyframes ani-slide-in-top {\n  0% {\n    -webkit-transform: translateY(-20px);\n    transform: translateY(-20px);\n    opacity: 0;\n  }\n  100% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n}\n@keyframes ani-slide-in-top {\n  0% {\n    -webkit-transform: translateY(-20px);\n    transform: translateY(-20px);\n    opacity: 0;\n  }\n  100% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation shake-bottom\n * ----------------------------------------\n */\n@-webkit-keyframes shake-bottom {\n  0%,\n  100% {\n    -webkit-transform: rotate(0deg);\n    transform: rotate(0deg);\n    -webkit-transform-origin: 50% 100%;\n    transform-origin: 50% 100%;\n  }\n  10% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n  20%,\n  40%,\n  60% {\n    -webkit-transform: rotate(-4deg);\n    transform: rotate(-4deg);\n  }\n  30%,\n  50%,\n  70% {\n    -webkit-transform: rotate(4deg);\n    transform: rotate(4deg);\n  }\n  80% {\n    -webkit-transform: rotate(-2deg);\n    transform: rotate(-2deg);\n  }\n  90% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n}\n@keyframes shake-bottom {\n  0%,\n  100% {\n    -webkit-transform: rotate(0deg);\n    transform: rotate(0deg);\n    -webkit-transform-origin: 50% 100%;\n    transform-origin: 50% 100%;\n  }\n  10% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n  20%,\n  40%,\n  60% {\n    -webkit-transform: rotate(-4deg);\n    transform: rotate(-4deg);\n  }\n  30%,\n  50%,\n  70% {\n    -webkit-transform: rotate(4deg);\n    transform: rotate(4deg);\n  }\n  80% {\n    -webkit-transform: rotate(-2deg);\n    transform: rotate(-2deg);\n  }\n  90% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n}\n\n/**\n * ----------------------------------------\n * animation bgAnimate of create button\n * ----------------------------------------\n */\n@keyframes bgAnimate {\n  0% {\n    background-position: right;\n  }\n  100% {\n    background-position: left;\n  }\n}\n", ""]);
+            a.push([e.id, ".env-editor {\n  /* position: fixed;\n  left: 50vw;\n  top: 50vh;\n  margin-left: -150px;\n  margin-top: -220px;\n  overflow: visible; */\n  width: 820px;\n  /* height: 87vh; */\n  position: relative;\n  margin-top: -40px;\n  padding-bottom: 0;\n  opacity: 0;\n  transition: margin-top 0.25s ease, opacity 0.25s ease;\n  border-radius: 20px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.editor-header {\n  text-align: center;\n  background: linear-gradient(120deg, #673ab7 10%, #9909e091 100%);\n  color: white;\n}\n\n.editor-scrollview {\n  height: 75vh;\n  /* height: calc(90vh - 122px); */\n  /* max-height: calc(90vh - 122px); /* leave room for 2 x 61px vertical bookend sections */\n  min-height: auto;\n  padding: 0px 10px;\n  overflow: auto;\n}\n\n.env-editor-col {\n  display: inline-block;\n  vertical-align: top;\n  width: 50%;\n}\n\n.env-editor-col-full {\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: white;\n  box-shadow: 0px 1px 4px -3px #000;\n  vertical-align: top;\n  display: flex;\n  margin: 0px 5px;\n}\n\n.env-editor-pane-new {\n  /* vertical-align: top; */\n  /* min-height: 180px; */\n  /* margin: 20px auto; */\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z2);\n  color: var(--jp-ui-font-color0);\n  height: 100%;\n  display: flex;\n  flex-direction: column;\n  justify-content: flex-start;\n}\n\n.env-editor-pane {\n  /* vertical-align: top; */\n  /* min-height: 180px; */\n  border-radius: 10px;\n  border: 1px solid transparent;\n  background: var(--jp-layout-color1);\n  box-shadow: var(--jp-elevation-z2);\n  color: var(--jp-ui-font-color0);\n  height: 100%;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  /* padding-bottom: 8px; */\n  /* #555 */\n}\n\n.env-editor-pane-title {\n  margin: 10px 0;\n  text-align: center;\n  font-size: 14px;\n}\n\n.env-info-input {\n  width: -webkit-fill-available;\n  width: -moz-available;\n  margin: 10px;\n  border: 1px solid var(--jp-border-color1);\n  background-color: var(--jp-input-background);\n  border-radius: 4px;\n  padding: 6px 10px;\n  color: var(--jp-ui-font-color1);\n  outline: none !important;\n  resize: none;\n  font-family: unset;\n  /* width:100%; */\n  box-sizing: border-box;\n}\n.env-info-input::placeholder {\n  font-style: italic;\n}\n\n.env-editor-input-data-text {\n  width: -webkit-fill-available;\n  margin: 10px !important;\n  border: 1px solid var(--jp-border-color1) !important;\n  background-color: var(--jp-input-background) !important;\n  border-radius: 4px !important;\n  /* padding: 6px 10px; */\n  color: var(--jp-ui-font-color1) !important;\n  outline: none !important;\n  resize: none !important;\n  font-family: unset !important;\n}\n\n.env-info-input:focus {\n  border: 1px solid #de2b8e;\n  background-color: var(--jp-input-active-background);\n}\n\n.env-info-input::placeholder {\n  color: #8e8e8e;\n}\n\n.env-info-input:-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-info-input::-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-pane-content {\n  margin: 15px 30px;\n  display: flex;\n  flex-direction: column;\n}\n\n.env-pane-label {\n  padding: 0;\n  font-weight: 500;\n  font-size: 14px;\n  text-align: left;\n  color: #424242;\n}\n\n.env-pane-prompt {\n  font-size: 14px;\n  color: #848484;\n  text-align: left;\n}\n\n.env-pane-share-holder {\n  width: 100%;\n  display: flex;\n  flex-direction: row;\n  justify-content: space-between;\n  align-items: center;\n}\n\n.env-pane-email {\n  border-radius: 5px !important;\n  border: 1px solid var(--jp-border-color1) !important;\n}\n.env-pane-email-error {\n  margin-top: 8px;\n  font-size: 12px;\n  width: 100%;\n  color: lightcoral;\n}\n.env-pane-email-success {\n  margin-top: 8px;\n  font-size: 12px;\n  width: 100%;\n  color: green;\n}\n.env-pane-email-normal {\n  margin-top: 8px;\n  font-size: 12px;\n  width: 100%;\n  color: var(--jp-ui-font-color1);\n}\n.env-editor-pane-action {\n  font-size: 15px !important;\n  text-transform: none !important;\n  color: #f5f5f5 !important;\n}\n.env-pane-re-share {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n}\n\n.env-table {\n  width: 100%;\n  table-layout: fixed;\n}\n\n.env-table tbody {\n  display: block;\n  width: max-content;\n  overflow-y: auto;\n}\n\n.env-table th {\n  padding: 0;\n  font-weight: 500;\n  font-size: 14px;\n  text-align: left;\n  color: #424242;\n}\n\n.env-table td {\n  font-size: 14px;\n  text-align: left;\n  color: #6c6c6c;\n  padding: 6px 0;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  white-space: nowrap;\n}\n\n.env-table-filter {\n  position: relative;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  height: 30px;\n  margin: 0;\n  padding: 0 !important;\n  overflow: visible !important;\n  border: none;\n}\n\n.env-table-filter input {\n  display: block;\n  width: 300px;\n  position: absolute;\n  /* top: 0; */\n  border: none !important;\n  outline: none !important;\n  color: #424242;\n}\n\n.env-table-filter input::placeholder {\n  color: #8e8e8e;\n}\n\n.env-table-filter input:-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-table-filter input::-ms-input-placeholder {\n  color: #8e8e8e;\n}\n\n.env-editor-actions {\n  /* total height should be 61px, incluing the 1px border-bottom  */\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  width: 100%;\n  border-radius: 0 0 20px 20px;\n  border-top: 1px solid #696969;\n  /* border-top: 1px solid #aaa; */\n  background: linear-gradient(120deg, #35383a 10%, #5e5f61 100%);\n}\n\n.editor-action {\n  display: inline-block;\n  vertical-align: top;\n  width: 120px !important;\n  margin: 12px 10px !important;\n  padding: 9px 0 !important;\n}\n\n.editor-action-alt {\n  width: 100%;\n  margin: 10px auto;\n  padding: 9px 0;\n  border-radius: 6px;\n  text-align: center;\n  background-color: darkred;\n  color: white;\n  cursor: pointer;\n}\n\n.environment-editor {\n  display: flex;\n  flex-direction: column;\n  flex: 1;\n  overflow: hidden;\n}\n\n.environment-editor-section-label {\n  margin: 10px 0 2px 10px;\n  color: var(--jp-ui-font-color2);\n  font-size: 12px;\n}\n.environment-editor-code-error {\n  margin: 0px 0 2px 10px;\n  color: var(--jp-error-color1);\n  font-size: 12px;\n}\ntextarea {\n  resize: none;\n  font-family: unset;\n}\n.text-area-warning {\n  margin: 0px 10px;\n  display: flex;\n  justify-content: space-between;\n  align-items: center;\n}\n.text-area-warning-text {\n  margin: 0 !important;\n  color: indianred !important;\n}\n.text-area-error-text {\n  background: indianred !important;\n  color: white !important;\n  padding: 0 0.2em !important;\n  text-align: center !important;\n  border-radius: 0.3em !important;\n}\n.text-area-error-input {\n  outline: 1px solid indianred !important;\n  border-color: indianred !important;\n}\n.environment-editor-input {\n  margin: 5px 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  outline: transparent;\n  color: var(--jp-ui-font-color0);\n  background-color: var(--jp-layout-color1);\n  padding: 4px;\n  background-size: 16px;\n  box-sizing: content-box !important;\n  transition: border 0.2s linear;\n}\n\n.environment-editor-input:hover {\n  border-color: var(--jp-inverse-layout-color0);\n}\n\n.environment-editor-input:focus,\n.environment-editor-input:active,\n.environment-editor-input:focus-within {\n  outline: 1px solid #d30982;\n  border-color: #d30982;\n}\n\n.environment-editor-input.all_lowercase {\n  text-transform: lowercase;\n}\n\n.environment-editor-ace-wrapper {\n  position: relative;\n  border-radius: 4px;\n  overflow: auto;\n  width: 95%;\n  margin-inline: auto;\n  margin-block: 10px;\n  border: 1px solid var(--jp-border-color1);\n}\n.environment-editor-ace-wrapper-error {\n  border: 1px solid var(--jp-error-color1);\n}\n\n.environment-editor-save,\n.environment-editor-discard {\n  border: 1px solid #bdbdbd;\n  display: inline-block;\n  vertical-align: top;\n  width: calc(50% - 20px);\n  margin: 8px;\n  padding: 10px 0;\n  text-align: center;\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  transition: 200ms color ease, 200ms background-color ease;\n  cursor: pointer;\n  user-select: none;\n}\n\n.environment-editor-save {\n  background-color: var(--jp-layout-color3);\n}\n\n.environment-editor-save:hover {\n  color: #eee;\n  background-color: #46c146;\n}\n\n.environment-editor-active {\n  color: white;\n  background: linear-gradient(90deg, #673ab7 50%, #46c146 50%);\n  background-size: 200%;\n  background-position: left;\n  animation: bgAnimate 5s 1;\n}\n\n.environment-editor-discard:hover {\n  color: #e03333;\n}\n\n.env-pane-search-container {\n  display: flex;\n  flex-direction: column;\n  position: relative;\n}\n\n.env-pane-button-group {\n  display: flex;\n  flex: wrap;\n  justify-content: space-between;\n  gap: 1em;\n  margin-top: 10px;\n}\n\n.env-pane-button {\n  flex: 1;\n  height: 3em;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  background-color: transparent;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n  box-sizing: border-box;\n  font-size: 1em;\n}\n\n.outlined {\n  border-color: #673ab7;\n  color: #673ab7;\n  transition: color ease-in-out 150ms, border-color ease-in-out 150ms;\n}\n\n.outlined:hover {\n  border-color: indianred;\n  color: indianred;\n}\n\n.disabled {\n  background-color: lightgrey;\n  color: rgba(0, 0, 0, 0.6);\n  cursor: not-allowed;\n}\n\n.filled {\n  background-color: #673ab7 !important;\n  color: white !important;\n}\n\n.env-pane-searchbox {\n  width: -webkit-fill-available;\n  margin: 5px 0px;\n  border: 1px solid #aaa;\n  border-radius: 4px;\n  padding: 6px 10px;\n  color: var(--jp-ui-font-color1);\n  outline: none !important;\n  resize: none;\n  font-family: unset;\n  display: flex;\n  align-items: center;\n  height: 1.3em;\n  background-color: var(--jp-input-background);\n}\n\n.env-pane-searchbox:has(.env-page-input-bar:focus) {\n  background-color: var(--jp-input-active-background);\n}\n\n.env-pane-input-bar {\n  height: 1.5em;\n  width: 100%;\n  outline: none;\n  border: none;\n  background-color: transparent;\n  margin-inline: 0.5em;\n  color: inherit;\n}\n\n.env-pane-dropdown {\n  position: absolute;\n  height: auto;\n  top: 2.7em;\n  z-index: 50;\n  width: -webkit-fill-available;\n  background-color: var(--jp-layout-color2);\n  max-height: 250px;\n  min-height: 0;\n  display: flex;\n  flex-direction: row;\n  box-shadow: 0 0.25em 0.25em rgb(0 0 0 / 10%);\n  border-radius: 10px;\n}\n\n.env-pane-dropdown-list {\n  list-style: none;\n  display: flex;\n  flex-direction: column;\n  gap: 0.75em;\n  padding: 1em;\n  margin: 0 0 10px 0;\n  font-size: 1em;\n  font-weight: 400;\n  overflow-y: auto;\n  width: 100%;\n}\n\n.env-pane-dropdown-list > li {\n  background: var(--jp-layout-color1);\n  box-shadow: 0px 1px 4px -2px #555;\n  padding: 0.5em;\n  border-radius: 10px;\n  overflow: hidden;\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  gap: 1em;\n  min-height: 2.5em;\n  max-height: 3em;\n  cursor: pointer;\n  user-select: none;\n  transition: transform ease-in-out 200ms;\n}\n.env-pane-dropdown-over-ride {\n  min-height: 4.5em !important;\n}\n\n.env-pane-dropdown-list > li:hover {\n  transform: scale(1.01);\n}\n\n.env-pane-flexrow {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  gap: 0.25em;\n  line-height: 16px;\n  justify-content: space-between;\n  width: 100%;\n}\n\n.env-pane-flexcol {\n  display: flex;\n  flex-direction: column;\n  gap: 0.25em;\n  justify-content: space-between;\n}\n\n.env-pane-dropdown-name {\n  font-size: 16px;\n  font-weight: 600;\n}\n\n.env-pane-dropdown-desc {\n  font-size: 12px;\n}\n\n.env-pane-msg-popup {\n  position: absolute;\n  width: calc(100% - 3em);\n  margin: 0px 1em;\n  min-height: 2em;\n  max-height: 3em;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.warning {\n  background-color: rgb(179, 101, 13);\n  color: white;\n}\n\n.env-editor-tag-area {\n  width: calc(100% - 20px);\n  margin-inline: auto;\n  margin-bottom: 10px;\n}\n\n.env-tag-header {\n  margin-bottom: 5px;\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: flex-start;\n  gap: 10px;\n  min-height: 1.8em;\n}\n\n.env-slug-header {\n  margin-bottom: 5px;\n  display: flex;\n  flex-direction: row;\n  justify-content: flex-start;\n  gap: 10px;\n  min-height: 1.8em;\n}\n.env-tag-flex {\n  display: inline-flex !important;\n  flex-direction: row;\n  align-items: center;\n  justify-content: space-between;\n  gap: 5px;\n}\n\n.env-tag-icon {\n  width: 12px !important;\n  height: 12px !important;\n  color: currentColor;\n  cursor: pointer;\n}\n\n.env-add-tags {\n  display: flex;\n  flex-direction: row;\n  padding: 3px 3px 3px 6px;\n  align-items: center;\n  border-radius: 1.5em;\n  gap: 5px;\n  width: fit-content;\n}\n\n.env-plus-icon {\n  width: 16px !important;\n  height: 16px !important;\n  color: white;\n}\n\n.env-tags-input {\n  border-radius: 1em;\n  outline: none;\n  border: none;\n  padding: 2px 8px;\n  background: var(--jp-input-background);\n  color: var(--jp-ui-font-color0);\n  text-transform: lowercase;\n  width: 100%;\n  max-width: 100px;\n}\n\n.env-tags-input:active,\n.env-tags-input:focus {\n  background: var(--jp-input-active-background);\n}\n\n.env-edit-icon {\n  color: var(--jp-ui-font-color2);\n  width: 16px !important;\n  height: 16px !important;\n  cursor: pointer;\n}\n\n.env-jobs-toggle-area {\n  position: relative;\n  display: flex;\n  align-items: center;\n  width: calc(100% - 20px);\n  margin-inline: auto;\n  margin-bottom: 8px;\n  flex-wrap: wrap;\n}\n\n.env-jobs-toggle-switch-text {\n  font-weight: 500;\n}\n\n.env-unins-dialog-box #alert-dialog-title,\n.env-unins-dialog-box #alert-dialog-content,\n.env-unins-dialog-box #alert-dialog-description,\n.env-unins-dialog-box #alert-dialog-actions {\n  background-color: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color0);\n}\n\n.envSidebar-flex-container {\n  display: flex;\n  flex-wrap: wrap;\n  padding: 8px;\n  gap: 4px;\n}\n\n.envSidebar-flex-btn {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: center;\n  gap: 4px;\n}\n\n.envSidebar-btn-upload {\n  max-width: 120px;\n}\n\n.envSidebar-custom-button {\n  --fill-color1: #b767ff;\n  --fill-color2: #673ab7;\n  flex: 1;\n  height: 26px;\n  font-size: 14px;\n  outline: transparent;\n  border: none;\n  color: white;\n  border-radius: 4px;\n  background-image: linear-gradient(\n    110deg,\n    var(--fill-color1) 50%,\n    var(--fill-color2) 50%\n  );\n  background-size: 222%;\n  background-position: right;\n  transition: background-position 200ms linear, letter-spacing 200ms linear;\n  cursor: pointer;\n}\n\n.envSidebar-custom-button:hover {\n  background-position: left;\n  letter-spacing: 1.5px;\n  box-shadow: 0em 0em 0.2em var(--fill-color1);\n}\n\n.envSidebar-btn-discard {\n  --fill-color1: #d32f2f;\n  --fill-color2: transparent;\n  border: 1px solid #d32f2f;\n  color: #d32f2f;\n}\n.envSidebar-btn-discard:hover {\n  color: white;\n}\n.envSidebar-btn-save {\n  --fill-color1: #8ab73a;\n  --fill-color2: #673ab7;\n}\n.envSidebar-btn-delete {\n  --fill-color1: #562944;\n  --fill-color2: #d32f2f;\n}\n.envSidebar-btn-disabled {\n  --fill-color1: gray;\n  --fill-color2: gray;\n  cursor: not-allowed;\n}\n.envSidebar-btn-disabled:hover {\n  letter-spacing: normal !important;\n}\n\n.operator-selector {\n  width: 55px;\n  padding: 0.32em;\n  border-radius: 6px;\n  border: 1px solid #673ab7;\n  font-weight: 600;\n  color: #673ab7;\n}\n\n.package-selector::-webkit-scrollbar,\n.operator-selector::-webkit-scrollbar {\n  width: 6px;\n}\n.package-selector::-webkit-scrollbar-track,\n.operator-selector::-webkit-scrollbar-track {\n  background: transparent;\n}\n.package-selector::-webkit-scrollbar-thumb,\n.operator-selector::-webkit-scrollbar-track {\n  background-color: rgb(158, 156, 156);\n  border-radius: 20px;\n  border: transparent;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n}\n\n.env-edior-slide-in-top {\n  -webkit-animation: slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;\n  animation: ani-slide-in-top 0.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) both;\n}\n\n.shake-bottom {\n  -webkit-animation: shake-bottom 0.8s cubic-bezier(0.455, 0.03, 0.515, 0.955)\n    both;\n  animation: shake-bottom 0.8s cubic-bezier(0.455, 0.03, 0.515, 0.955) both;\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@-webkit-keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-top\n * ----------------------------------------\n */\n@-webkit-keyframes ani-slide-in-top {\n  0% {\n    -webkit-transform: translateY(-20px);\n    transform: translateY(-20px);\n    opacity: 0;\n  }\n  100% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n}\n@keyframes ani-slide-in-top {\n  0% {\n    -webkit-transform: translateY(-20px);\n    transform: translateY(-20px);\n    opacity: 0;\n  }\n  100% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation shake-bottom\n * ----------------------------------------\n */\n@-webkit-keyframes shake-bottom {\n  0%,\n  100% {\n    -webkit-transform: rotate(0deg);\n    transform: rotate(0deg);\n    -webkit-transform-origin: 50% 100%;\n    transform-origin: 50% 100%;\n  }\n  10% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n  20%,\n  40%,\n  60% {\n    -webkit-transform: rotate(-4deg);\n    transform: rotate(-4deg);\n  }\n  30%,\n  50%,\n  70% {\n    -webkit-transform: rotate(4deg);\n    transform: rotate(4deg);\n  }\n  80% {\n    -webkit-transform: rotate(-2deg);\n    transform: rotate(-2deg);\n  }\n  90% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n}\n@keyframes shake-bottom {\n  0%,\n  100% {\n    -webkit-transform: rotate(0deg);\n    transform: rotate(0deg);\n    -webkit-transform-origin: 50% 100%;\n    transform-origin: 50% 100%;\n  }\n  10% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n  20%,\n  40%,\n  60% {\n    -webkit-transform: rotate(-4deg);\n    transform: rotate(-4deg);\n  }\n  30%,\n  50%,\n  70% {\n    -webkit-transform: rotate(4deg);\n    transform: rotate(4deg);\n  }\n  80% {\n    -webkit-transform: rotate(-2deg);\n    transform: rotate(-2deg);\n  }\n  90% {\n    -webkit-transform: rotate(2deg);\n    transform: rotate(2deg);\n  }\n}\n\n/**\n * ----------------------------------------\n * animation bgAnimate of create button\n * ----------------------------------------\n */\n@keyframes bgAnimate {\n  0% {\n    background-position: right;\n  }\n  100% {\n    background-position: left;\n  }\n}\n", ""]);
             const s = a
         },
         8222: (e, t, n) => {
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,15 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "5d7f6d37c97924a89805",
+        185: "c2e096475cfee897e1f9",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
@@ -77,15 +77,15 @@
     } [e] + ".js?v=" + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "5d7f6d37c97924a89805",
+        185: "c2e096475cfee897e1f9",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
@@ -154,15 +154,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     c = [];
-                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.0-rc.8", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(185)]).then((() => () => j(4185))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.0-rc.9", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(185)]).then((() => () => j(4185))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/third-party-licenses.json` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/PKG-INFO` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
@@ -12,14 +12,15 @@
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
@@ -29,15 +30,15 @@
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server<2,>=1.6
 Requires-Dist: jupyter_client~=7.1.0
 Requires-Dist: tornado>=6.1.0
 Requires-Dist: notebook<7
-Requires-Dist: qbraid-core<0.2,>=0.1.3
+Requires-Dist: qbraid-core<0.2,>=0.1.4.dev1
 
 # jupyter-environment-manager
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html)
 [![PyPI version](https://img.shields.io/pypi/v/jupyter-environment-manager.svg?color=blue)](https://pypi.org/project/jupyter-environment-manager/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/TPBU2sa8Et)
```

### Comparing `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/SOURCES.txt` & `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
-jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js
+jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js
 jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
 jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
 jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
 jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
@@ -53,15 +53,15 @@
 jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
 jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
-jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js
+jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js
 jupyter_environment_manager/labextension/static/style.js
 jupyter_environment_manager/labextension/static/third-party-licenses.json
 src/EnvironmentsSidebarWidget.tsx
 src/Flux.js
 src/assets.d.ts
 src/contextTypes.js
 src/global.d.ts
```

### Comparing `jupyter_environment_manager-0.2.0rc8/package.json` & `jupyter_environment_manager-0.2.0rc9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.2.0-rc.9'"}*

```diff
@@ -107,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.8"
+    "version": "0.2.0-rc.9"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc8/pyproject.toml` & `jupyter_environment_manager-0.2.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/setup.py` & `jupyter_environment_manager-0.2.0rc9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,26 +69,27 @@
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "jupyter_server>=1.6,<2",
         "jupyter_client~=7.1.0",
         "tornado>=6.1.0",
         "notebook<7",
-        "qbraid-core>=0.1.3,<0.2",
+        "qbraid-core>=0.1.4.dev1,<0.2",
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">= 3.9",
     platforms="Linux, Mac OS X, Windows",
     keywords=["IPython", "Jupyter", "JupyterLab"],
     classifiers=[
         "License :: Other/Proprietary License",
         "Natural Language :: English",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
+        "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Framework :: IPython",
         "Framework :: Jupyter",
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/EnvironmentsSidebarWidget.tsx` & `jupyter_environment_manager-0.2.0rc9/src/EnvironmentsSidebarWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/Flux.js` & `jupyter_environment_manager-0.2.0rc9/src/Flux.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/actions/ApiActions.js` & `jupyter_environment_manager-0.2.0rc9/src/actions/ApiActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/actions/AuthActions.js` & `jupyter_environment_manager-0.2.0rc9/src/actions/AuthActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/actions/EnvironmentActions.js` & `jupyter_environment_manager-0.2.0rc9/src/actions/EnvironmentActions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -714,15 +714,15 @@
         this.alt.dispatch(this);
 
         return new Promise((resolve, reject) => {
             if (!shareData.environmentId) {
                 return reject('Must provide environment id');
             }
 
-            if (!shareData.collabEmail) {
+            if (!shareData.collabEmail && !shareData.isAccessKeyEnv) {
                 return reject('Must provide qBraid collaborator email');
             }
 
             let env = this.alt.getStore('EnvironmentStore').getState()
                 .environmentCache[shareData.environmentId];
 
             if (!env) {
@@ -734,23 +734,20 @@
             }
 
             if (!env.installed) {
                 return reject('Environment must be installed to share');
             }
 
             let requestBody = {
-                slug: `${env.slug}`,
-                collabEmail: `${shareData.collabEmail}`,
-                overwrite: `${shareData.overwrite}`
+                slug: env.slug,
+                collabEmail: shareData?.collabEmail,
+                overwrite: shareData?.overwrite || false,
+                isAccessKeyEnv: shareData?.isAccessKeyEnv || false
             };
 
-            if (shareData.hasOwnProperty('overwrite')) {
-                requestBody.overwrite = shareData.overwrite;
-            }
-
             this.alt
                 .getActions('ApiActions')
                 .query()
                 .post('/environments/share')
                 .send(requestBody)
                 .end((err, res) => {
                     if (err) {
@@ -958,14 +955,64 @@
                         } else {
                             reject(res.message);
                         }
                     })
                     .catch(err => {
                         reject(err);
                     });
+            } catch (err) {
+                console.log(err);
+                reject(err);
+            }
+        });
+    };
+
+    this.generateAccessKey = id => {
+        this.alt.dispatch(this);
+        return new Promise((resolve, reject) => {
+            try {
+                this.alt
+                    .getActions('ApiActions')
+                    .query()
+                    .post(`/environments/access-key/${id}`)
+                    .then(res => {
+                        if (res?.status === 200) {
+                            resolve(res);
+                        } else {
+                            reject(res.message);
+                        }
+                    })
+                    .catch(err => {
+                        reject(err);
+                    });
+            } catch (err) {
+                console.log(err);
+                reject(err);
+            }
+        });
+    };
+
+    this.searchAccessCodeAndAccept = accessKey => {
+        this.alt.dispatch(this);
+        return new Promise((resolve, reject) => {
+            try {
+                this.alt
+                    .getActions('ApiActions')
+                    .query()
+                    .put(`/environments/permissions/${accessKey}`)
+                    .then(res => {
+                        if (res?.status === 200) {
+                            resolve(res);
+                        } else {
+                            reject(res.message);
+                        }
+                    })
+                    .catch(err => {
+                        reject(err);
+                    });
             } catch (err) {
                 console.log(err);
                 reject(err);
             }
         });
     };
     // END ACTION CREATORS
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/actions/JupyterApiActions.js` & `jupyter_environment_manager-0.2.0rc9/src/actions/JupyterApiActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/actions/UserActions.js` & `jupyter_environment_manager-0.2.0rc9/src/actions/UserActions.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -96,14 +96,15 @@
                             .get('/lab/is-mounted/' + filename)
                             .end((err, res) => {
                                 if (err) {
                                     console.log(err);
                                     this.actions._updateIsMount(false);
                                     resolve(false);
                                 } else {
+                                    // const isMounted = true;
                                     const isMounted = res.body?.isMounted;
                                     this.actions._updateIsMount(isMounted);
                                     resolve(isMounted);
                                 }
                             });
                     }
                 })
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/BackIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/BackIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/CloseIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/CloseIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/ConfirmIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/ConfirmIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/DescriptionIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/DescriptionIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/EnvIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/EnvIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/IconString.js` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/IconString.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/LinkIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/LinkIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/Loading.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/Loading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/RefreshIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/RefreshIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/SearchIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/SearchIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/UserIcon.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/UserIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/assets/icons/WhiteCube.tsx` & `jupyter_environment_manager-0.2.0rc9/src/assets/icons/WhiteCube.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/EndUserAgreement.js` & `jupyter_environment_manager-0.2.0rc9/src/components/EndUserAgreement.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentEditor.js` & `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentEditor.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -5,14 +5,15 @@
 import contextTypes from '../contextTypes';
 import '../../style/EnvironmentEditor.css';
 import {
     Dialog,
     DialogActions,
     DialogTitle,
     DialogContent,
+    Divider,
     IconButton,
     Grid,
     Button,
     Typography,
     Stack,
     TableContainer,
     Table,
@@ -24,41 +25,48 @@
     Paper,
     Snackbar,
     Switch,
     DialogContentText,
     Modal,
     TextField,
     InputAdornment,
+    InputBase,
     LinearProgress,
     Autocomplete,
     Avatar,
     Chip,
     Box,
     FormGroup,
     FormControlLabel,
     Skeleton,
-    Alert
+    Alert,
+    Icon,
+    tooltipClasses
 } from '@mui/material';
 import SearchIcon from '../assets/icons/SearchIcon';
 import WhiteCube from '../assets/icons/WhiteCube';
 import {
     AddCircleOutlined,
     AddCircleOutlineOutlined,
     Check,
     Close,
+    ContentCopy,
     Edit,
     EditOff,
     InfoOutlined,
     Link,
     NotInterested,
+    Refresh,
     ReportProblemOutlined,
     SaveOutlined,
     Send,
     Update,
-    UpdateDisabled
+    UpdateDisabled,
+    Visibility,
+    VisibilityOff
 } from '@mui/icons-material';
 import {
     env
 } from 'process';
 import {
     ACCOUNT_URL
 } from '../actions/ApiActions';
@@ -179,15 +187,24 @@
             cancelRequest: false,
             inputBoxVisible: false,
             saveSuccess: false,
             saveLoading: false,
             deleting: false,
             deleteAlert: false,
             loadingPackages: true,
-            lockedEnv: true
+            lockedEnv: true,
+            accessKeyVisibility: false,
+            accessKey: this.props.env?.accessKey || '',
+            accessKeyLoading: false,
+            copyCooldown: false,
+            resharePopUpContent: {
+                content: '',
+                title: '',
+                body: ''
+            }
         };
     }
 
     componentDidMount() {
         setTimeout(this.load, 1);
         if (this.props.env) {
             setTimeout(() => {
@@ -335,15 +352,24 @@
                             shareEmailBtnDis: false,
                             shareSuccess: false
                         });
                     }, SHARE_ENV_TIMER);
                 }
                 if (response.status === 304 && !reShare) {
                     this.setState({
-                        resharePopUp: true
+                        resharePopUp: true,
+                        resharePopUpContent: {
+                            content: 'reShareEnv',
+                            title: 'Update Shared Environment?',
+                            body: `You have already shared this environment with ${
+                this.state.shareEmail
+                  ? `${this.state.shareEmail}, or another user`
+                  : 'one or more users'
+              }. Would you like to update the existing version? Doing so will overwrite the globally shared environment, but will not affect any local copies that users have already installed.`
+                        }
                     });
                 }
             })
             .then(() => {
                 this.props.flux
                     .getActions('EnvironmentActions')
                     .updateAll()
@@ -1765,14 +1791,51 @@
                     /Stack>
                 )
             } <
             /div>
         );
     };
 
+    handleGenerateAccessKey = environementId => {
+        this.setState({
+            accessKeyLoading: true
+        });
+        this.context
+            .getActions('EnvironmentActions')
+            .generateAccessKey(environementId)
+            .then(res => {
+                this.setState({
+                    accessKey: res?.body?.accessKey
+                });
+                const shareData = {
+                    environmentId: environementId,
+                    overwrite: true,
+                    isAccessKeyEnv: true
+                };
+                this.context
+                    .getActions('EnvironmentActions')
+                    .shareEnvironment(shareData)
+                    .then(_res => this.setState({
+                        accessKeyLoading: false
+                    }))
+                    .catch(err => {
+                        console.log(err);
+                        this.setState({
+                            accessKeyLoading: false
+                        });
+                    });
+            })
+            .catch(err => {
+                console.log(err);
+                this.setState({
+                    accessKeyLoading: false
+                });
+            });
+    };
+
     renderSharingPane = () => {
         const handleEnvShare = () => {
             this.setState({
                 shareEmailApiError: ''
             });
             if (this.state.shareEmail === '') {
                 this.setState({
@@ -1876,36 +1939,139 @@
                     height: '26px',
                     fontSize: '18px'
                 },
                 children: `${name?.slice(0, 1)?.toUpperCase()}`
             };
         };
 
+        const handleCopyAccessKey = () => {
+            this.setState({
+                copyCooldown: true
+            });
+            navigator.clipboard.writeText(this.state.accessKey);
+            setTimeout(() => this.setState({
+                copyCooldown: false
+            }), 1500);
+        };
+
+        const handleAccessKeyVisibility = () => {
+            this.setState(prevState => ({
+                accessKeyVisibility: !prevState.accessKeyVisibility
+            }));
+        };
+
+        const handleReShareEnv = () => {
+            this.setState({
+                resharePopUp: false
+            });
+            this.setState({
+                shareEmailBtnDis: true
+            });
+            this.shareEnvironment(true);
+        };
+
+        const handleCancelReShareEnv = () => {
+            this.setState({
+                resharePopUp: false,
+                shareEmail: '',
+                shareEmailBtnDis: false
+            });
+        };
+
+        const handleOpenSharingDialog = () => {
+            this.setState({
+                resharePopUp: true,
+                resharePopUpContent: {
+                    content: 'accessCode',
+                    title: 'Are you sure?',
+                    body: 'Generating a new access code will invalidate the current code, and update the global shared copy of this environment.'
+                }
+            });
+        };
+
+        const handleRegenerateAccessKey = () => {
+            this.setState({
+                resharePopUp: false,
+                accessKey: ''
+            });
+            this.handleGenerateAccessKey(this.props.env._id);
+        };
+
+        const handleCancelRegenrateAccessKey = () => {
+            this.setState({
+                resharePopUp: false,
+                resharePopUpContent: {
+                    content: '',
+                    title: '',
+                    body: ''
+                }
+            });
+        };
+
+        const actions = {
+            accessCode: {
+                confirm: handleRegenerateAccessKey,
+                cancel: handleCancelRegenrateAccessKey
+            },
+            reShareEnv: {
+                confirm: handleReShareEnv,
+                cancel: handleCancelReShareEnv
+            }
+        };
+
         return ( <
             div className = "env-editor-pane"
-            id = "sharing-pane" >
+            id = "sharing-pane"
+            style = {
+                {
+                    marginTop: '0px !important'
+                }
+            } >
             <
             p className = "env-editor-pane-title" > Share Environment < /p>
 
             <
-            div className = "env-pane-content"
-            style = {
-                {
-                    flex: 1
-                }
+            Box className = "env-pane-content"
+            flex = {
+                1
+            }
+            mt = {
+                0
             } > {
+                this.state.isCustom &&
+                this.state.isOwner &&
+                this.state.isInstalled &&
+                this.state.isMount && ( <
+                    Typography fontSize = {
+                        14
+                    } >
+                    Enable other qBraid users to discover this environment and install a copy into their own Lab instance. <
+                    /Typography>
+                )
+            } {
                 this.state.isMount ? (
                     this.state.isOwner ? (
                         this.state.isCustom ? (
                             this.state.isInstalled ? ( <
                                 Grid container justifyContent = "space-between"
-                                gap = {
+                                alignItems = "flex-start"
+                                position = "relative"
+                                spacing = {
+                                    1
+                                }
+                                mt = {
+                                    1
+                                } >
+                                <
+                                Grid item container xs = {
+                                    12
+                                }
+                                spacing = {
                                     1
                                 }
-                                alignItems = "flex-start"
                                 position = "relative" >
                                 <
                                 Grid item xs = {
                                     12
                                 }
                                 sm = {
                                     12
@@ -1990,18 +2156,18 @@
                                 Grid item xs = {
                                     12
                                 }
                                 sm = {
                                     12
                                 }
                                 md = {
-                                    3
+                                    4
                                 }
                                 lg = {
-                                    3
+                                    4
                                 } >
                                 <
                                 Button fullWidth className = "env-editor-pane-action"
                                 onClick = {
                                     handleEnvShare
                                 }
                                 style = {
@@ -2041,15 +2207,15 @@
                                 } <
                                 /Button> <
                                 /Grid> <
                                 Grid item xs = {
                                     12
                                 }
                                 position = "absolute"
-                                top = "32px" > {
+                                bottom = "4px" > {
                                     this.state.isCustom &&
                                     this.state.isOwner &&
                                     this.state.isInstalled &&
                                     this.state.isMount &&
                                     this.state.shareEmailApiError && ( <
                                         p className = "env-pane-email-error" > {
                                             this.state.shareEmailApiError
@@ -2065,14 +2231,219 @@
                                             p className = "env-pane-email-success" >
                                             Environment shared succesfully...
                                             <
                                             /p>
                                         )
                                 } <
                                 /Grid> <
+                                /Grid> <
+                                Grid item xs = {
+                                    12
+                                } >
+                                <
+                                Divider textAlign = "center" > OR < /Divider> <
+                                /Grid> <
+                                Grid item display = "flex"
+                                justifyContent = "center"
+                                alignItems = "center"
+                                xs = {
+                                    12
+                                } >
+                                {
+                                    this.state.accessKey === '' ? ( <
+                                        Button fullWidth variant = "outlined"
+                                        color = "success"
+                                        onClick = {
+                                            () =>
+                                            this.handleGenerateAccessKey(this.props.env._id)
+                                        }
+                                        sx = {
+                                            {
+                                                textTransform: 'none',
+                                                fontSize: 12,
+                                                cursor: this.state.accessKeyLoading ?
+                                                    'progress' :
+                                                    'pointer'
+                                            }
+                                        }
+                                        disabled = {
+                                            this.state.accessKeyLoading
+                                        } >
+                                        {
+                                            this.state.accessKeyLoading ?
+                                            'Generating ...' :
+                                                'Generate Access Code'
+                                        } <
+                                        /Button>
+                                    ) : ( <
+                                        Grid item xs = {
+                                            12
+                                        } >
+                                        <
+                                        Paper elevation = {
+                                            0
+                                        }
+                                        sx = {
+                                            theme => ({
+                                                display: 'flex',
+                                                alignItems: 'center',
+                                                width: '100%',
+                                                backgroundColor: `${theme.palette.success.light}30`
+                                            })
+                                        } >
+                                        <
+                                        Typography fontSize = {
+                                            12
+                                        }
+                                        color = "success"
+                                        px = {
+                                            1.5
+                                        } >
+                                        Share via access code <
+                                        /Typography> <
+                                        Divider orientation = "vertical"
+                                        sx = {
+                                            {
+                                                m: 0.5,
+                                                height: 28
+                                            }
+                                        }
+                                        /> <
+                                        InputBase size = "small"
+                                        sx = {
+                                            {
+                                                ml: 1,
+                                                flex: 1,
+                                                fontSize: 12,
+                                                fontWeight: 600,
+                                                '&.MuiInputBase-input': {
+                                                    p: 0
+                                                }
+                                            }
+                                        }
+                                        value = {
+                                            this.state.accessKey
+                                        }
+                                        type = {
+                                            !this.state.accessKeyVisibility ?
+                                            'password' :
+                                                'text'
+                                        }
+                                        /> <
+                                        IconButton size = "small"
+                                        onClick = {
+                                            handleAccessKeyVisibility
+                                        } >
+                                        {
+                                            !this.state.accessKeyVisibility ? ( <
+                                                Visibility fontSize = "inherit" / >
+                                            ) : ( <
+                                                VisibilityOff fontSize = "inherit" / >
+                                            )
+                                        } <
+                                        /IconButton> <
+                                        Divider orientation = "vertical"
+                                        sx = {
+                                            {
+                                                m: 0.5,
+                                                height: 28
+                                            }
+                                        }
+                                        /> <
+                                        Tooltip arrow placement = "left"
+                                        title = "Copy" >
+                                        <
+                                        IconButton size = "small"
+                                        sx = {
+                                            {
+                                                mx: 1.5
+                                            }
+                                        }
+                                        onClick = {
+                                            handleCopyAccessKey
+                                        } >
+                                        {
+                                            this.state.copyCooldown ? ( <
+                                                ConfirmIcon color = "green" / >
+                                            ) : ( <
+                                                ContentCopy fontSize = "inherit" / >
+                                            )
+                                        } <
+                                        /IconButton> <
+                                        /Tooltip> <
+                                        /Paper> <
+                                        /Grid>
+                                    )
+                                } <
+                                /Grid> <
+                                Grid item xs = {
+                                    12
+                                }
+                                display = "flex"
+                                justifyContent = "flex-end"
+                                alignItems = "center"
+                                gap = {
+                                    1
+                                } >
+                                {
+                                    this.state.accessKey !== '' && ( <
+                                        >
+                                        <
+                                        Button variant = "text"
+                                        color = "success"
+                                        size = "small"
+                                        startIcon = {
+                                            < Refresh fontSize = "inherit" / >
+                                        }
+                                        sx = {
+                                            {
+                                                padding: '0px !important',
+                                                textTransform: 'none'
+                                            }
+                                        }
+                                        onClick = {
+                                            handleOpenSharingDialog
+                                        } >
+                                        Regenerate access code ?
+                                        <
+                                        /Button> <
+                                        Tooltip title = {
+                                            <
+                                            React.Fragment > {
+                                                'The existing access code will be invalidated and your current environment will replace the global shared copy.'
+                                            } <
+                                            /React.Fragment>
+                                        }
+                                        PopperProps = {
+                                            {
+                                                sx: theme => ({
+                                                    [`& .${tooltipClasses.tooltip}`]: {
+                                                        background: theme.palette.background.alternate,
+                                                        color: theme.palette.text.primary,
+                                                        fontSize: 12,
+                                                        boxShadow: theme.shadows[10]
+                                                    }
+                                                })
+                                            }
+                                        } >
+                                        <
+                                        InfoOutlined fontSize = "small"
+                                        color = "action"
+                                        sx = {
+                                            {
+                                                width: 14,
+                                                height: 14
+                                            }
+                                        }
+                                        /> <
+                                        /Tooltip> <
+                                        />
+                                    )
+                                } <
+                                /Grid> <
                                 /Grid>
                             ) : ( <
                                 Grid container >
                                 <
                                 Grid item xs = {
                                     12
                                 } >
@@ -2092,18 +2463,19 @@
                             } >
                             <
                             p className = "env-pane-prompt" >
                             This environment is not shareable.To create a shareable,
                             custom environment, click {
                                 ' '
                             } <
-                            b > +Add {
+                            b > Add {
                                 '→'
-                            } + Create Environment < /b> in the
-                            environments sidebar. <
+                            }
+                            Create Environment < /b> in the environments
+                            sidebar. <
                             /p> <
                             /Grid> <
                             /Grid>
                         )
                     ) : ( <
                         Grid container >
                         <
@@ -2111,17 +2483,18 @@
                             12
                         } >
                         <
                         p className = "env-pane-prompt" >
                         To share an environment, you must be the environment owner.To create your own shareable, custom environment, click {
                             ' '
                         } <
-                        b > +Add {
+                        b > Add {
                             '→'
-                        } + Create Environment < /b> in the environments
+                        }
+                        Create Environment < /b> in the environments
                         sidebar. <
                         /p> <
                         /Grid> <
                         /Grid>
                     )
                 ) : ( <
                     Grid container >
@@ -2148,29 +2521,22 @@
                     /p> <
                     /Grid> <
                     /Grid>
                 )
             }
 
             {
-                this.state.isCustom &&
-                    this.state.isOwner &&
-                    this.state.isInstalled &&
-                    this.state.isMount && ( <
-                        p className = "env-pane-email-normal" >
-                        Share this environment to make it visible to another qBraid user, and allow them to install it directly in to their own Lab instance. <
-                        /p>
-                    )
-            } {
                 /* {this.renderShareMsg(this.state.sharePopupMsg)} */ } {
-                this.renderReshareEnvModal()
+                this.renderReshareEnvModal({
+                    action: actions
+                })
             } {
                 this.renderUpgradeEnvModal()
             } <
-            /div> <
+            /Box> <
             /div>
         );
     };
     // upgrade modal for share node
     renderUpgradeEnvModal = () => {
         return ( <
             Modal open = {
@@ -2282,24 +2648,17 @@
             /Grid> <
             /Grid> <
             /Grid> <
             /Modal>
         );
     };
     // resharing modal for environment sharing
-    renderReshareEnvModal = () => {
-        const reShareEnv = () => {
-            this.setState({
-                resharePopUp: false
-            });
-            this.setState({
-                shareEmailBtnDis: true
-            });
-            this.shareEnvironment(true);
-        };
+    renderReshareEnvModal = ({
+        action
+    }) => {
         return ( <
             Modal open = {
                 this.state.resharePopUp
             }
             onClose = {
                 () =>
                 this.setState({
@@ -2322,84 +2681,84 @@
                 {
                     width: '700px',
                     minWidth: '200px',
                     minHeight: '150px',
                     padding: '1em'
                 }
             }
-            className = "env-pane-re-share" >
+            className = "env-pane-re-share"
+            spacing = {
+                1
+            } >
             <
             Grid item xs = {
                 12
             } >
             <
-            h3 style = {
-                {
-                    margin: '0px'
-                }
-            } > Update Shared Environment ? < /h3> <
+            Typography fontSize = {
+                18
+            }
+            fontWeight = {
+                600
+            }
+            color = "text.primary" > {
+                this.state.resharePopUpContent.title
+            } <
+            /Typography> <
             /Grid> <
             Grid item xs = {
                 12
             } >
             <
-            p className = "env-pane-email-normal" > {
-                `You have already shared this environment with ${this.state.shareEmail}, or another user. Would you like to update the existing version? Doing so will overwrite the globally shared environment, but will not effect any local copies that users have already installed.`
-            } < /p> <
+            Typography fontSize = {
+                14
+            }
+            color = "text.primary" > {
+                this.state.resharePopUpContent.body
+            } <
+            /Typography> <
             /Grid> <
             Grid item container xs = {
                 12
             }
-            sx = {
-                {
-                    display: 'flex',
-                    justifyContent: 'flex-end',
-                    alignItems: 'center',
-                    gap: '10px'
-                }
+            justifyContent = "flex-end"
+            alignItems = "center"
+            spacing = {
+                1
             } >
             <
-            Grid item xs = {
-                2
-            } >
+            Grid item >
             <
             Button variant = "slide"
             type = "decline"
-            fullWidth sx = {
+            sx = {
                 {
                     textTransform: 'none',
                     minWidth: '120px'
                 }
             }
             onClick = {
-                () =>
-                this.setState({
-                    resharePopUp: false,
-                    shareEmail: '',
-                    shareEmailBtnDis: false
-                })
+                action[this.state.resharePopUpContent.content]?.cancel
             } >
             Cancel <
             /Button> <
             /Grid> <
-            Grid item xs = {
-                2
-            } >
+            Grid item >
             <
             Button variant = "slide"
             sx = {
                 {
                     textTransform: 'none',
                     minWidth: '120px'
                 }
             }
-            fullWidth onClick = {
-                () => reShareEnv()
+            onClick = {
+                action[this.state.resharePopUpContent.content]?.confirm
             } >
-            Share <
+            Confirm <
             /Button> <
             /Grid> <
             /Grid> <
             /Grid> <
             /Modal>
         );
     };
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentTile.js` & `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentTile.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -96,16 +96,16 @@
         const {
             isInstalled,
             packageInstallingEnv,
             environment,
             isInstalling,
             expandedEnvs
         } = this.props;
-        const isTileExpanded =
-            environment?.isExpanded || expandedEnvs?.includes(envId);
+        const isTileExpanded = expandedEnvs?.includes(envId);
+        // environment?.isExpanded ||
         const isInstallingPackage = packageInstallingEnv === envId;
         const isSystemPython = environment.sysPython;
 
         if (
             !isInstalling &&
             isInstalled &&
             isTileExpanded &&
@@ -193,15 +193,15 @@
             tileStyle.border = '1px solid #673ab7';
         }
         if (this.state.lockedTile) {
             tileStyle.border = 'none';
         }
 
         if (
-            env.isExpanded ||
+            // env.isExpanded ||
             this.props.isNewEnv ||
             this.props.expandedEnvs?.includes(env._id)
         ) {
             tileStyle.maxHeight = 9999;
             tileStyle.padding = '0 10px 60px 10px';
         } else {
             tileStyle.maxHeight = 0;
@@ -215,15 +215,15 @@
                     ...tileStyle
                 }
             } >
             <
             div className = {
                 `env-name flex-box ${
             (this.props.isNewEnv ||
-              env.isExpanded ||
+              // env.isExpanded ||
               this.props.expandedEnvs?.includes(env._id)) &&
             'env-name-border'
           }`
             }
             style = {
                 {
                     color: this.props.isActive ? 'black' : 'var(--jp-ui-font-color0)'
@@ -278,16 +278,16 @@
                             maxWidth: 45,
                             marginRight: 5
                         }
                     }
                     src = {
                         localStorage.getItem(env.displayName) ||
                         this?.props?.isDarkTheme ?
-                        env.logo.dark :
-                            env.logo.light
+                        env?.logo?.dark :
+                            env?.logo?.light
                     }
                     /> <
                     /span>
                 )
             } <
             p className = "env-tile-display-name" > {
                 env.displayName
@@ -345,15 +345,15 @@
             />
 
             <
             ExpandMoreIcon sx = {
                 {
                     fontSize: '1rem!important',
                     transform: this.props.isNewEnv ||
-                        env.isExpanded ||
+                        // env.isExpanded ||
                         this.props.expandedEnvs?.includes(env._id) ?
                         'rotateX(180deg)' :
                         'rotateX(0deg)',
                     transition: 'transform 300ms ease',
                     cursor: 'pointer',
                     zIndex: '99'
                 }
@@ -362,17 +362,17 @@
                 () => this.toggleCollapsed(env._id)
             }
             /> <
             /span> <
             /div> <
             span style = {
                 {
-                    visibility: env.isExpanded ||
-                        this.props.isNewEnv ||
-                        this.props.expandedEnvs?.includes(env._id) ?
+                    visibility:
+                        // env.isExpanded ||
+                        this.props.isNewEnv || this.props.expandedEnvs?.includes(env._id) ?
                         'visible' :
                         'hidden'
                 }
             }
             // style={{ visibility: this.state.collapsed ? 'hidden' : 'visible' }}
             >
             <
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentsSidebar.js` & `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentsSidebar.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,15 @@
 import ClearIcon from '@mui/icons-material/Clear';
 import DataSaverOnIcon from '@mui/icons-material/DataSaverOn';
 import HttpsIcon from '@mui/icons-material/Https';
 
 import {
     Avatar,
     Button,
+    Box,
     Chip,
     Dialog,
     DialogActions,
     DialogContent,
     DialogContentText,
     DialogTitle,
     Divider,
@@ -37,25 +38,30 @@
     Snackbar,
     Stack,
     TextField,
     ThemeProvider,
     Tooltip,
     Typography,
     FormControlLabel,
-    Checkbox
+    Paper,
+    Checkbox,
+    InputBase
 } from '@mui/material';
 import AceEditor from 'react-ace';
 import 'ace-builds/src-noconflict/mode-python';
 import 'ace-builds/src-noconflict/theme-monokai';
 import 'ace-builds/src-noconflict/theme-kuroir';
 import 'ace-builds/src-noconflict/theme-terminal';
 import {
+    AddCircleOutline,
     FileUpload,
     FilterList,
-    ReceiptLongOutlined
+    ReceiptLongOutlined,
+    Visibility,
+    VisibilityOff
 } from '@mui/icons-material';
 import {
     darkTheme,
     lightTheme
 } from '../utils/theme';
 import Loading from './Loading';
 import {
@@ -248,15 +254,18 @@
             },
             intelPermissionModal: false,
             currentEnv: null,
             returnToMyenv: false, // determine return path from clone
             expandedEnvs: [], // array of envid, contains id for the last environment which has been expanded.
             noUser: props.flux.getStore('UserStore').getState()?.user ? false : true,
             packageLoading: false, // When "More..." is clicked, load packages and show loader as per this state
-            containerWidth: 300 // For aceEditor width changes, affects only specific version of safari
+            containerWidth: 300, // For aceEditor width changes, affects only specific version of safari
+            accessCodeInput: '',
+            accessCodeInputVisible: false,
+            accessCodeLoading: false
         };
     }
 
     componentDidMount() {
         this.props.flux
             .getStore('EnvironmentStore')
             .listen(this.handleUpdateEnvironments);
@@ -982,20 +991,24 @@
                     'Your environment ' +
                     env.displayName +
                     ' could not be uninstalled at this time.'
                 );
             });
     };
 
-    handleRefreshEnvironments = () => {
-        this.setState(prev => ({
-            togglesCount: ++prev.togglesCount
-        }));
+    handleRefreshEnvironments = ({
+        clickedRefresh
+    }) => {
+        if (clickedRefresh) {
+            this.setState(prev => ({
+                togglesCount: ++prev.togglesCount
+            }));
+        }
         if (this.state.noUser) return;
-        this.setState({
+        if (clickedRefresh) this.setState({
             isClickedRefresh: true
         });
         this.props.flux
             .getActions('EnvironmentActions')
             .updateAll()
             .then(res => {
                 this.props.flux
@@ -1269,15 +1282,29 @@
             return this.handleFinishInstallSuccess();
         } catch (err) {
             console.log(err);
             return this.handleFinishInstallFailure();
         }
     };
 
-    toggleExpandedEnv = _id => {
+    onToggleExpand = _id => {
+        // let newEnvironment = this.state.environments.map(row => {
+        //   let cloneItem = row;
+        //   if (row._id === _id || row._id === this.state.newCustomEnvId) {
+        //     cloneItem.isExpanded = cloneItem.isExpanded ? false : true;
+        //   }
+        //   return cloneItem;
+        // });
+        // this.setState({
+        //   environments: newEnvironment,
+        //   newCustomEnvId: null
+        // });
+        this.setState({
+            newCustomEnvId: null
+        });
         if (this.state.expandedEnvs.includes(_id)) {
             this.setState(prev => {
                 return {
                     ...prev,
                     expandedEnvs: prev.expandedEnvs.filter(envid => envid !== _id)
                 };
             });
@@ -1287,29 +1314,14 @@
             return {
                 ...prev,
                 expandedEnvs: [...prev.expandedEnvs, _id]
             };
         });
     };
 
-    onToggleExpand = _id => {
-        let newEnvironment = this.state.environments.map(row => {
-            let cloneItem = row;
-            if (row._id === _id || row._id === this.state.newCustomEnvId) {
-                cloneItem.isExpanded = cloneItem.isExpanded ? false : true;
-            }
-            return cloneItem;
-        });
-        this.setState({
-            environments: newEnvironment,
-            newCustomEnvId: null
-        });
-        this.toggleExpandedEnv(_id);
-    };
-
     onTogglePinned = _id => {
         let newEnvironment = this.state.environments.map(row => {
             let cloneItem = row;
             if (row._id === _id) {
                 if (cloneItem.pinned) {
                     this.handleRemovePinned(_id);
                 } else {
@@ -1917,26 +1929,26 @@
             }
         });
         if (this.state.environments.filter(env => env.installed).length < 1) {
             return < Loading / > ;
         } else {
             return this.state.environments
                 .filter(env => env.installed)
-                .map((env, index) => {
+                .map(env => {
                     let active = env.active;
                     let installing =
                         this.state.installingEnvironment &&
                         (this.state.installingEnvironment._id === env._id ||
                             this.state.newEnvSlug === env?.slug);
                     return ( <
                         EnvironmentTile qbUser = {
                             this.state.qbUser
                         }
                         key = {
-                            index
+                            env._id
                         }
                         expandedEnvs = {
                             this.state.expandedEnvs
                         }
                         onTogglePinned = {
                             this.onTogglePinned
                         }
@@ -2021,22 +2033,151 @@
             selectedEnvironment: {
                 ...this.state.selectedEnvironment,
                 readAccessUsers: updatedEnv[0].readAccessUsers
             }
         });
     };
 
+    handleAccessCodeVisibility = () => {
+        this.setState(prev => ({
+            accessCodeInputVisible: !prev.accessCodeInputVisible
+        }));
+    };
+
+    handleAccessCodeInputChange = event => {
+        this.setState({
+            accessCodeInput: event.target.value
+        });
+    };
+
+    handleDiscoverEnvWithAccessCode = () => {
+        if (this.state.accessCodeInput === '') return;
+        this.setState({
+            accessCodeLoading: true
+        });
+
+        this.props.flux
+            .getActions('EnvironmentActions')
+            .searchAccessCodeAndAccept(this.state.accessCodeInput)
+            .then(res => {
+                if (res?.status === 200) {
+                    this.setState({
+                        accessCodeInput: '',
+                        accessCodeLoading: false
+                    });
+                    this.handleOpenPopup('Access Code redeemed!', 'success');
+                    this.handleRefreshEnvironments({
+                        clickedRefresh: false
+                    });
+                }
+            })
+            .catch(err => {
+                this.handleOpenPopup(err?.response?.body?.message, 'error');
+                this.setState({
+                    accessCodeLoading: false
+                });
+            });
+    };
+
     // Shows the list of all public packages that are not installed
     renderUninstalledEnvironments = () => {
         let envs =
             this.state.filterQuery || this.state.tagFilter ?
             this.state.filteredEnvironments :
             this.state.environments;
         envs.sort((a, b) => this.compareEnvs(a, b));
         return [ <
+                Box m = "10px" >
+                <
+                Paper
+                elevation = {
+                    0
+                }
+                sx = {
+                    theme => ({
+                        display: 'flex',
+                        flexDirection: 'row',
+                        flex: 1,
+                        borderWidth: '1px',
+                        borderStyle: 'solid',
+                        borderColor: theme.palette.grey[400],
+                        backgroundColor: theme.palette.background.default,
+                        '&:hover': {
+                            borderColor: `${theme.palette.action}!important`
+                        },
+                        '&:focus-within, &:focus-visible': {
+                            borderColor: theme.palette.primary.main,
+                            outline: `1px solid ${theme.palette.primary.main}`
+                        }
+                    })
+                } >
+                <
+                InputBase
+                sx = {
+                    {
+                        ml: 1,
+                        flex: 1,
+                        fontSize: 18,
+                        fontWeight: 400
+                    }
+                }
+                inputProps = {
+                    {
+                        style: {
+                            height: '19px',
+                            fontSize: '14px'
+                        }
+                    }
+                }
+                value = {
+                    this.state.accessCodeInput
+                }
+                placeholder = "Discover via access code..."
+                onChange = {
+                    this.handleAccessCodeInputChange
+                }
+                type = {
+                    !this.state.accessCodeInputVisible ? 'password' : 'text'
+                }
+                /> <
+                IconButton size = "small"
+                onClick = {
+                    this.handleAccessCodeVisibility
+                } > {
+                    this.state.accessCodeInputVisible ? ( <
+                        Visibility fontSize = "inherit" / >
+                    ) : ( <
+                        VisibilityOff fontSize = "inherit" / >
+                    )
+                } <
+                /IconButton> <
+                Button
+                color = "secondary"
+                variant = "contained"
+                size = "small"
+                sx = {
+                    {
+                        fontSize: 14,
+                        textTransform: 'inherit',
+                        ml: 1,
+                        cursor: this.state.accessCodeLoading ? 'wait' : 'pointer'
+                    }
+                }
+                onClick = {
+                    this.handleDiscoverEnvWithAccessCode
+                }
+                disabled = {
+                    this.state.accessCodeLoading
+                } >
+                <
+                AddCircleOutline / >
+                <
+                /Button> <
+                /Paper> <
+                /Box>, <
                 div
                 className = "environments-sidebar-create-env"
                 onClick = {
                     this.handleNewEnvironmentClick
                 } >
                 <
                 p style = {
@@ -2048,21 +2189,24 @@
                 } > + < /p> <
                 p > Create Environment < /p> <
                 /div>
             ]
             .concat(
                 envs
                 .filter(env => !env.installed)
-                .map((env, index) => {
+                .map(env => {
                     return ( <
                         EnvironmentTile qbUser = {
                             this.state.qbUser
                         }
                         key = {
-                            index
+                            env._id
+                        }
+                        expandedEnvs = {
+                            this.state.expandedEnvs
                         }
                         onToggleExpand = {
                             this.onToggleExpand
                         }
                         onTogglePinned = {
                             this.onTogglePinned
                         }
@@ -2266,15 +2410,18 @@
                             transition: 'transform 1s',
                             transform: `rotateZ(${`${
                         this.state.togglesCount * 180
                       }deg`})`
                         }
                     }
                     onClick = {
-                        this.handleRefreshEnvironments
+                        () =>
+                        this.handleRefreshEnvironments({
+                            clickedRefresh: true
+                        })
                     }
                     className = "div-refresh-btn" >
                     <
                     RefreshIcon / >
                     <
                     /div> <
                     /div>
@@ -2359,22 +2506,22 @@
                 {
                     '& .MuiOutlinedInput-root': {
                         '&.Mui-focused fieldset': {
                             borderColor: '#d30982'
                         },
                         paddingLeft: '10px',
                         paddingRight: '10px'
-                    },
-                    fontSize: '14px'
+                    }
                 }
             }
             inputProps = {
                 {
                     style: {
-                        height: '19px'
+                        height: '19px',
+                        fontSize: '14px'
                     }
                 }
             }
             InputProps = {
                 {
                     startAdornment: ( <
                         InputAdornment position = "start" >
@@ -3191,33 +3338,33 @@
                                 height: '28px',
                                 textTransform: 'lowercase'
                             }
                         }
                     }
                     inputProps = {
                         {
-                            maxLength: 80
+                            maxLength: 30
                         }
-                    } // sets the max number of character to 80 issue#116
+                    } // sets the max number of characters
                     /> <
                     div className = "text-area-warning" >
                     <
                     p className = "environment-editor-section-label text-area-warning-text" > {
-                        this.state.newEnvKernelName.length >= 80 &&
-                        'Max length = 80'
+                        this.state.newEnvKernelName.length >= 30 &&
+                        'Max length = 30'
                     } <
                     /p> <
                     p className = {
                         `environment-editor-section-label text-area-warning-text ${
-                                this.state.newEnvKernelName.length >= 80 &&
+                                this.state.newEnvKernelName.length >= 30 &&
                                 'text-area-error-text'
                               }`
                     } >
                     {
-                        80 - this.state.newEnvKernelName.length
+                        30 - this.state.newEnvKernelName.length
                     } <
                     /p> <
                     /div> <
                     /Grid> <
                     Grid item xs = {
                         12
                     } >
@@ -3269,33 +3416,33 @@
                                 height: '28px',
                                 textTransform: 'lowercase'
                             }
                         }
                     }
                     inputProps = {
                         {
-                            maxLength: 80
+                            maxLength: 20
                         }
-                    } // sets the max number of character to 80 issue#116
+                    } // sets the max number of characters
                     /> <
                     div className = "text-area-warning" >
                     <
                     p className = "environment-editor-section-label text-area-warning-text" > {
-                        this.state.newEnvShellPrompt.length >= 80 &&
-                        'Max length = 80'
+                        this.state.newEnvShellPrompt.length >= 20 &&
+                        'Max length = 20'
                     } <
                     /p> <
                     p className = {
                         `environment-editor-section-label text-area-warning-text ${
-                                this.state.newEnvShellPrompt.length >= 80 &&
+                                this.state.newEnvShellPrompt.length >= 20 &&
                                 'text-area-error-text'
                               }`
                     } >
                     {
-                        80 - this.state.newEnvShellPrompt.length
+                        20 - this.state.newEnvShellPrompt.length
                     } <
                     /p> <
                     /div> <
                     /Grid> <
                     Grid item xs = {
                         12
                     } >
```

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/Loading.js` & `jupyter_environment_manager-0.2.0rc9/src/components/Loading.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/LogoLoader.js` & `jupyter_environment_manager-0.2.0rc9/src/components/LogoLoader.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/MuiStyledComponents.js` & `jupyter_environment_manager-0.2.0rc9/src/components/MuiStyledComponents.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/components/UserNotFound.js` & `jupyter_environment_manager-0.2.0rc9/src/components/UserNotFound.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/index.ts` & `jupyter_environment_manager-0.2.0rc9/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/stores/AuthStore.js` & `jupyter_environment_manager-0.2.0rc9/src/stores/AuthStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/stores/EnvironmentStore.js` & `jupyter_environment_manager-0.2.0rc9/src/stores/EnvironmentStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/stores/UserStore.js` & `jupyter_environment_manager-0.2.0rc9/src/stores/UserStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/utils/googleAnalytics.js` & `jupyter_environment_manager-0.2.0rc9/src/utils/googleAnalytics.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/src/utils/theme.js` & `jupyter_environment_manager-0.2.0rc9/src/utils/theme.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -14,14 +14,17 @@
         },
         secondaryHighlight: {
             main: '#562944', // dark violet
             contrastText: '#ffffff'
         },
         typography: {
             fontFamily: ['var(--jp-ui-font-family)'].join(',')
+        },
+        background: {
+            alternate: 'linear-gradient(120deg, #fdfbfb 0%, #ebedee 100%)'
         }
     },
     components: {
         MuiButton: {
             variants: [{
                 props: {
                     variant: 'slide'
@@ -80,13 +83,16 @@
         },
         secondaryHighlight: {
             main: '#562944',
             contrastText: '#ffffff'
         },
         typography: {
             fontFamily: ['var(--jp-ui-font-family)'].join(',')
+        },
+        background: {
+            alternate: '#1e1e1e'
         }
     }
 };
 
 export const lightTheme = createTheme(lightThemeStyle);
 export const darkTheme = createTheme(darkThemeStyle);
```

### Comparing `jupyter_environment_manager-0.2.0rc8/style/EnvironmentEditor.css` & `jupyter_environment_manager-0.2.0rc9/style/EnvironmentEditor.css`

 * *Files 1% similar despite different names*

```diff
@@ -165,25 +165,28 @@
 }
 
 .env-pane-email {
   border-radius: 5px !important;
   border: 1px solid var(--jp-border-color1) !important;
 }
 .env-pane-email-error {
-  margin-top: 1em;
+  margin-top: 8px;
+  font-size: 12px;
   width: 100%;
   color: lightcoral;
 }
 .env-pane-email-success {
-  margin-top: 1em;
+  margin-top: 8px;
+  font-size: 12px;
   width: 100%;
   color: green;
 }
 .env-pane-email-normal {
-  margin-top: 0.5em;
+  margin-top: 8px;
+  font-size: 12px;
   width: 100%;
   color: var(--jp-ui-font-color1);
 }
 .env-editor-pane-action {
   font-size: 15px !important;
   text-transform: none !important;
   color: #f5f5f5 !important;
```

### Comparing `jupyter_environment_manager-0.2.0rc8/style/EnvironmentTile.css` & `jupyter_environment_manager-0.2.0rc9/style/EnvironmentTile.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/style/EnvironmentsSidebar.css` & `jupyter_environment_manager-0.2.0rc9/style/EnvironmentsSidebar.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/style/Loading.css` & `jupyter_environment_manager-0.2.0rc9/style/Loading.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/style/LogoLoader.css` & `jupyter_environment_manager-0.2.0rc9/style/LogoLoader.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/tools/create_dev_build.sh` & `jupyter_environment_manager-0.2.0rc9/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/tools/stamp_pre_release.py` & `jupyter_environment_manager-0.2.0rc9/tools/stamp_pre_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/tsconfig.json` & `jupyter_environment_manager-0.2.0rc9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc8/yarn.lock` & `jupyter_environment_manager-0.2.0rc9/yarn.lock`

 * *Files identical despite different names*

