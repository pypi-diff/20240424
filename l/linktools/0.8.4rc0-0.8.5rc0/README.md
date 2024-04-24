# Comparing `tmp/linktools-0.8.4rc0.tar.gz` & `tmp/linktools-0.8.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktools-0.8.4rc0.tar", last modified: Tue Apr 16 08:50:18 2024, max compression
+gzip compressed data, was "linktools-0.8.5rc0.tar", last modified: Wed Apr 24 02:46:12 2024, max compression
```

## Comparing `linktools-0.8.4rc0.tar` & `linktools-0.8.5rc0.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32997 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:50:18.993133 linktools-0.8.4rc0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.973134 linktools-0.8.4rc0/src/linktools/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_environ.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/android/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23929 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/android/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.apk
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 08:50:09.000000 linktools-0.8.4rc0/src/linktools/assets/android-tools.json
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/http.conf
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/https.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.977134 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json
--rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.js
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-16 08:48:13.000000 linktools-0.8.4rc0/src/linktools/assets/frida.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.969134 linktools-0.8.4rc0/src/linktools/assets/objection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/assets/tools.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/android/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15337 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4595 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.981134 linktools-0.8.4rc0/src/linktools/cli/commands/common/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/cntr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/cli/commands/ios/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/cli/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/container/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/frida/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/android.py
--rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/frida/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ida/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ida/ida.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/ios/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ios/sib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/reactor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.985134 linktools-0.8.4rc0/src/linktools/references/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/references/fake_useragent/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/rich.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-16 08:48:03.000000 linktools-0.8.4rc0/src/linktools/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:50:18.989133 linktools-0.8.4rc0/src/linktools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 08:50:18.000000 linktools-0.8.4rc0/src/linktools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:46:12.554604 linktools-0.8.5rc0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4278 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.538604 linktools-0.8.5rc0/src/linktools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21680 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.538604 linktools-0.8.5rc0/src/linktools/android/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/android/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    82987 2024-04-24 02:46:03.000000 linktools-0.8.5rc0/src/linktools/assets/android-tools.apk
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 02:46:03.000000 linktools-0.8.5rc0/src/linktools/assets/android-tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/chrome-driver.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/linktools/assets/containers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47272 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/http.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/https.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/nginx.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/fake_useragent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44744 2024-04-24 02:44:10.000000 linktools-0.8.5rc0/src/linktools/assets/frida.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-04-24 02:44:10.000000 linktools-0.8.5rc0/src/linktools/assets/frida.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.534603 linktools-0.8.5rc0/src/linktools/assets/objection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/assets/objection/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/assets/objection/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools/assets/tools.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31589 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.542604 linktools-0.8.5rc0/src/linktools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/android/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2494 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/adb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2140 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15066 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2614 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/debug.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6205 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4881 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/objection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15517 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/pidcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4522 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/android/top.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15194 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/cntr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/grep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4134 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/common/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/cli/commands/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/frida.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/objection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/commands/ios/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/cli/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.546604 linktools-0.8.5rc0/src/linktools/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21050 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/container/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/frida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29987 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/frida/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/ida/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ida/ida.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/sib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ios/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/reactor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/references/fake_useragent/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/references/fake_useragent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19460 2024-04-24 02:43:58.000000 linktools-0.8.5rc0/src/linktools/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:46:12.550604 linktools-0.8.5rc0/src/linktools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 02:46:12.000000 linktools-0.8.5rc0/src/linktools.egg-info/top_level.txt
```

### Comparing `linktools-0.8.4rc0/LICENSE` & `linktools-0.8.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/PKG-INFO` & `linktools-0.8.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.4rc0
+Version: 0.8.5rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -71,15 +71,15 @@
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
-eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
```

### Comparing `linktools-0.8.4rc0/README.md` & `linktools-0.8.5rc0/README.md`

 * *Files identical despite different names*

```diff
@@ -20,15 +20,15 @@
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
-eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
```

### Comparing `linktools-0.8.4rc0/pyproject.toml` & `linktools-0.8.5rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/setup.py` & `linktools-0.8.5rc0/setup.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/__init__.py` & `linktools-0.8.5rc0/src/linktools/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/__main__.py` & `linktools-0.8.5rc0/src/linktools/__main__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/_config.py` & `linktools-0.8.5rc0/src/linktools/_config.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/_environ.py` & `linktools-0.8.5rc0/src/linktools/_environ.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/_tools.py` & `linktools-0.8.5rc0/src/linktools/_tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/_url.py` & `linktools-0.8.5rc0/src/linktools/_url.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/android/__init__.py` & `linktools-0.8.5rc0/src/linktools/container/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : __init__.py
-@time    : 2020/03/01
+@file    : __init__.py.py 
+@time    : 2023/05/21
 @site    :  
 @software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
@@ -23,9 +23,9 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .adb import Adb, Device, AdbError
-from .struct import Package, Permission, Component, Activity, Service, Receiver, Provider, IntentFilter
+from .container import ContainerError, BaseContainer, ExposeLink, ExposeCategory
+from .manager import ContainerManager
```

### Comparing `linktools-0.8.4rc0/src/linktools/android/adb.py` & `linktools-0.8.5rc0/src/linktools/android/adb.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 import json
 import re
 import time
 from typing import Optional, Any, Generator, List
 
-from .struct import Package, UnixSocket, InetSocket, Process
+from .struct import App, UnixSocket, InetSocket, Process
 from .. import utils, environ
 from ..decorator import cached_property, cached_classproperty
 from ..device import BridgeError, Bridge, BaseDevice
 from ..reactor import Stoppable
 
 _logger = environ.get_logger("android.adb")
 
@@ -368,18 +368,18 @@
         """
         启动app的launcher页面
         :param package_name: 包名
         :param activity_name: activity名
         :return: adb输出结果
         """
         if not activity_name:
-            package = self.get_package(package_name, **kwargs)
-            activity = package.get_launch_activity()
+            app = self.get_app(package_name, detail=True, **kwargs)
+            activity = app.get_launch_activity()
             if not activity:
-                raise AdbError(f"Package {package.name} does not have a launch activity")
+                raise AdbError(f"App {app.name} does not have a launch activity")
             activity_name = activity.name
 
         return self.shell(
             "am", "start",
             "-a", "android.intent.action.MAIN",
             "-c", "android.intent.category.LAUNCHER",
             "-n", f"{package_name}/{activity_name}",
@@ -528,107 +528,107 @@
         result = self.shell(*args, **kwargs)
         items = result.splitlines()[-1].split()
         if items is not None and len(items) >= 2:
             return items[1].rstrip()
         raise AdbError("can not fetch top activity")
 
     @utils.timeoutable
-    def get_apk_path(self, package: str, **kwargs) -> str:
+    def get_apk_path(self, package_name: str, **kwargs) -> str:
         """
         获取apk路径
         :return: apk路径
         """
         if self.uid < 10000:
-            out = self.shell("pm", "path", package, **kwargs)
+            out = self.shell("pm", "path", package_name, **kwargs)
             match = re.search(r"^.*package:\s*(.*)[\s\S]*$", out)
             if match is not None:
                 return match.group(1).strip()
-        obj = self.get_packages(package, simple=True, **kwargs)
+        obj = self.get_apps(package_name, **kwargs)
         return utils.get_item(obj, 0, "sourceDir", default="")
 
     @utils.timeoutable
     def get_uid(self, package_name: str = None, timeout: utils.Timeout = None) -> Optional[int]:
         """
         根据包名获取uid
         :param package_name: 包名
         :param timeout: 超时时间
         :return: uid
         """
         if package_name:
-            info = self.get_package(package_name, simple=True, timeout=timeout)
-            return info.user_id if info else None
+            app = self.get_app(package_name, timeout=timeout)
+            return app.user_id if app else None
         else:
             default = -1
             out = self.shell("id", "-u", timeout=timeout)
             uid = utils.int(out, default=default)
             if uid != default:
                 return uid
             out = self.shell("echo", "-n", "${USER_ID}", timeout=timeout)
             uid = utils.int(out, default=default)
             if uid != default:
                 return uid
             raise AdbError("unknown adb uid: %s" % out)
 
     @utils.timeoutable
-    def get_package(self, package_name: str, simple: bool = None, **kwargs) -> Optional[Package]:
+    def get_app(self, package_name: str, detail: bool = None, **kwargs) -> Optional[App]:
         """
         根据包名获取包信息
         :param package_name: 包名
-        :param simple: 只获取基本信息
+        :param detail: 获取详细信息
         :return: 包信息
         """
         args = ["package", "--packages", package_name]
-        if simple is True:
+        if detail is not True:
             args.append("--simple")
         objs = json.loads(self.call_agent(*args, **kwargs))
-        return Package(objs[0]) if len(objs) > 0 else None
+        return App(objs[0]) if len(objs) > 0 else None
 
     @utils.timeoutable
-    def get_packages(self, *package_names: str, system: bool = None, simple: bool = None, **kwargs) -> [Package]:
+    def get_apps(self, *package_names: str, system: bool = None, detail: bool = False, **kwargs) -> [App]:
         """
         获取包信息
         :param package_names: 需要匹配的所有包名，为空则匹配所有
         :param system: true只匹配系统应用，false只匹配非系统应用，为空则全匹配
-        :param simple: 只获取基本信息
+        :param detail: 获取详细信息
         :return: 包信息
         """
         result = []
         agent_args = ["package"]
         if not utils.is_empty(package_names):
             agent_args.append("--packages")
             agent_args.extend(package_names)
         if system is True:
             agent_args.append("--system")
         elif system is False:
             agent_args.append("--non-system")
-        if simple is True:
+        if detail is not True:
             agent_args.append("--simple")
         objs = json.loads(self.call_agent(*agent_args, **kwargs))
         for obj in objs:
-            result.append(Package(obj))
+            result.append(App(obj))
         return result
 
     @utils.timeoutable
-    def get_packages_for_uid(self, *uids: int, simple: bool = None, **kwargs) -> [Package]:
+    def get_apps_for_uid(self, *uids: int, detail: bool = False, **kwargs) -> [App]:
         """
         获取指定uid包信息
         :param uids: 需要匹配的所有uid
-        :param simple: 只获取基本信息
+        :param detail: 获取详细信息
         :return: 包信息
         """
         result = []
         agent_args = ["package"]
         if not utils.is_empty(uids):
             agent_args.append("--uids")
             agent_args.extend([str(uid) for uid in uids])
-        if simple is True:
+        if detail is not True:
             agent_args.append("--simple")
         objs = json.loads(self.call_agent(*agent_args, **kwargs))
         for obj in objs:
-            result.append(Package(obj))
+            result.append(App(obj))
         return result
 
     @utils.timeoutable
     def get_tcp_sockets(self, **kwargs) -> [InetSocket]:
         """
         同netstat命令，获取设备tcp连接情况，需要读取/proc/net/tcp文件，高版本设备至少需要shell权限
         :return: tcp连接列表
```

### Comparing `linktools-0.8.4rc0/src/linktools/android/struct.py` & `linktools-0.8.5rc0/src/linktools/android/struct.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,48 +36,60 @@
     def __init__(self, obj: dict):
         self.path = utils.get_item(obj, "path", type=str, default="")
         self.type = utils.get_item(obj, "type", type=str, default="literal")
 
     def __str__(self):
         return "path=%s, type=%s" % (self.path, self.type)
 
+    def __repr__(self):
+        return f"PatternMatcher<{self.path}>"
+
 
 class PathPermission(PatternMatcher):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.read_permission = utils.get_item(obj, "readPermission", type=Permission, default=Permission.default())
         self.write_permission = utils.get_item(obj, "writePermission", type=Permission, default=Permission.default())
 
     def is_dangerous(self):
         return self.read_permission.is_dangerous() or self.write_permission.is_dangerous()
 
+    def __repr__(self):
+        return f"PathPermission<{self.path}>"
+
 
 class AuthorityEntry:
 
     def __init__(self, obj: dict):
         self.host = utils.get_item(obj, "host", type=str, default="")
         self.port = utils.get_item(obj, "port", type=int, default=0)
 
     def __str__(self):
         return "host=%s, port=%s" % (self.host, self.port)
 
+    def __repr__(self):
+        return f"AuthorityEntry<{self.host}>"
+
 
 class IntentFilter:
 
     def __init__(self, obj: dict):
         self.actions = utils.get_list_item(obj, "actions", type=str, default=[])
         self.categories = utils.get_list_item(obj, "categories", type=str, default=[])
         self.data_schemes = utils.get_list_item(obj, "dataSchemes", type=str, default=[])
         self.data_scheme_specific_parts = utils.get_list_item(obj, "dataSchemeSpecificParts", type=PatternMatcher,
                                                               default=[])
         self.data_authorities = utils.get_list_item(obj, "dataAuthorities", type=AuthorityEntry, default=[])
         self.data_paths = utils.get_list_item(obj, "dataPaths", type=PatternMatcher, default=[])
         self.data_types = utils.get_list_item(obj, "dataTypes", type=str, default=[])
 
+    def __repr__(self):
+        return f"IntentFilter<{self.actions}>"
+
 
 class Permission:
 
     @staticmethod
     def default() -> "Permission":
         return Permission({"name": "", "protection": "normal"})
 
@@ -90,14 +102,17 @@
 
     def is_dangerous(self):
         return self.protection in ["dangerous", "normal"]
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return f"Permission<{self.name}>"
+
 
 class Component:
 
     def __init__(self, obj: dict):
         self.name = utils.get_item(obj, "name", type=str, default="")
         self.exported = utils.get_item(obj, "exported", type=bool, default=False)
         self.enabled = utils.get_item(obj, "enabled", type=bool, default=False)
@@ -105,44 +120,65 @@
 
     def is_dangerous(self):
         return True
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return f"Component<{self.name}>"
+
 
 class Activity(Component):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.permission = utils.get_item(obj, "permission", type=Permission, default=Permission.default())
 
     def is_dangerous(self):
         return self.exported and self.permission.is_dangerous()
 
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return f"Activity<{self.name}>"
+
 
 class Service(Component):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.permission = utils.get_item(obj, "permission", type=Permission, default=Permission.default())
 
     def is_dangerous(self):
         return self.exported and self.permission.is_dangerous()
 
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return f"Service<{self.name}>"
+
 
 class Receiver(Component):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.permission = utils.get_item(obj, "permission", type=Permission, default=Permission.default())
 
     def is_dangerous(self):
         return self.exported and self.permission.is_dangerous()
 
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return f"Receiver<{self.name}>"
+
 
 class Provider(Component):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.authority = utils.get_item(obj, "authority", type=str, default="")
         self.read_permission = utils.get_item(obj, "readPermission", type=Permission, default=Permission.default())
@@ -157,16 +193,22 @@
         if self.read_permission.is_dangerous() or self.write_permission.is_dangerous():
             return True
         for path_permission in self.path_permissions:
             if path_permission.is_dangerous():
                 return True
         return False
 
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return f"Provider<{self.name}>"
 
-class Package:
+
+class App:
 
     def __init__(self, obj: dict):
         self.name = utils.get_item(obj, "name", type=str, default="")
         self.app_name = utils.get_item(obj, "appName", type=str, default="")
         self.user_id = utils.get_item(obj, "userId", type=int, default=0)
         self.gids = utils.get_list_item(obj, "gids", type=int, default=[])
         self.source_dir = utils.get_item(obj, "sourceDir", type=str, default="")
@@ -236,39 +278,48 @@
             if provider.is_dangerous():
                 return True
         return False
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return f"App<{self.name}>"
+
 
 class Socket:
 
     def __init__(self, obj: dict):
         self.proto = utils.get_item(obj, "proto", type=str, default="")
         self.state = utils.get_item(obj, "state", type=str, default="")
         self.inode = utils.get_item(obj, "inode", type=int, default=0)
         self.listening = utils.get_item(obj, "listening", type=bool, default=False)
 
     def is_dangerous(self):
         return self.listening
 
+    def __repr__(self):
+        return f"Socket<{self.proto}>"
+
 
 class InetSocket(Socket):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.local_address = utils.get_item(obj, "localAddress", type=str, default="")
         self.local_port = utils.get_item(obj, "localPort", type=int, default=0)
         self.remote_address = utils.get_item(obj, "remoteAddress", type=str, default="")
         self.remote_port = utils.get_item(obj, "remotePort", type=int, default=0)
         self.uid = utils.get_item(obj, "uid", type=int, default=0)
         self.transmit_queue = utils.get_item(obj, "transmitQueue", type=int, default=0)
         self.receive_queue = utils.get_item(obj, "receiveQueue", type=int, default=0)
 
+    def __repr__(self):
+        return f"InetSocket<{self.local_address}:{self.local_port}>"
+
 
 class UnixSocket(Socket):
 
     def __init__(self, obj: dict):
         super().__init__(obj)
         self.ref_cnt = utils.get_item(obj, "refCnt", type=int, default=0)
         self.flags = utils.get_item(obj, "flags", type=str, default="")
@@ -276,14 +327,17 @@
         self.path = utils.get_item(obj, "path", type=str, default="")
         self.readable = utils.get_item(obj, "readable", type=bool, default=False)
         self.writable = utils.get_item(obj, "writable", type=bool, default=False)
 
     def is_dangerous(self):
         return super().is_dangerous() and (self.readable or self.writable)
 
+    def __repr__(self):
+        return f"UnixSocket<{self.path}>"
+
 
 class Process:
 
     def __init__(self, obj: dict):
         self.pid = utils.get_item(obj, "pid", type=int, default=0)
         self.uid = utils.get_item(obj, "uid", type=int, default=0)
         self.gid = utils.get_item(obj, "gid", type=int, default=0)
@@ -296,7 +350,10 @@
         self.tty = utils.get_item(obj, "tty", type=int, default=0)
         self.utime = utils.get_item(obj, "utime", type=int, default=0)
         self.stime = utils.get_item(obj, "stime", type=int, default=0)
         self.nice = utils.get_item(obj, "nice", type=int, default=0)
         self.start_time = utils.get_item(obj, "startTime", type=int, default=0)
         self.vsz = utils.get_item(obj, "vsz", type=int, default=0)
         self.rss = utils.get_item(obj, "rss", type=int, default=0)
+
+    def __repr__(self):
+        return f"Process<{self.name}>"
```

### Comparing `linktools-0.8.4rc0/src/linktools/assets/android-tools.json` & `linktools-0.8.5rc0/src/linktools/assets/android-tools.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'ANDROID_TOOL_BRIDGE_APK'": "{'md5': 'c419cb85594b69ee31bae8730718c425', 'time': '2024-04-24 "*

 * *                              "10:46:03'}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "ANDROID_TOOL_BRIDGE_APK": {
         "main": "android.tools.Main",
-        "md5": "3097e19b66070036181860877768b952",
+        "md5": "c419cb85594b69ee31bae8730718c425",
         "name": "android-tools.apk",
         "size": 82987,
-        "time": "2024-04-16 16:50:09"
+        "time": "2024-04-24 10:46:03"
     },
     "ANDROID_TOOL_FRIDA_SERVER": [
         {
             "min_version": "15.1.8",
             "name": "strong-frida-server-{version}-android-{abi}",
             "url": "https://github.com/hzzheyang/strongR-frida-android/releases/download/{version}/hluda-server-{version}-android-{abi}.xz"
         },
```

### Comparing `linktools-0.8.4rc0/src/linktools/assets/chrome-driver.json` & `linktools-0.8.5rc0/src/linktools/assets/chrome-driver.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/Dockerfile` & `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
 RUN acme.sh --issue --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} --dns {{ ACME_DNS_API }} --debug 2
 
 RUN acme.sh --install-cert --domain {{ ROOT_DOMAIN }} --domain *.{{ ROOT_DOMAIN }} \
     --cert-file /etc/certs/{{ ROOT_DOMAIN }}_cert.pem \
     --key-file /etc/certs/{{ ROOT_DOMAIN }}_key.pem \
     --fullchain-file /etc/certs/{{ ROOT_DOMAIN }}_fullchain.pem \
-    --reloadcmd "nginx -s reload 2>/dev/null || true"
+    --reloadcmd "killall nginx 2>/dev/null || true"
```

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/container.py` & `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,7 +77,11 @@
                 utils.ignore_error(os.remove, args=(target_path,))
 
     def on_started(self):
         self.manager.change_owner(
             self.get_app_path(),
             self.manager.user
         )
+        self.manager.create_docker_process(
+            "exec", "-it", "nginx",
+            "sh", "-c", "killall nginx 1>/dev/null 2>&1"
+        ).call()
```

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt` & `linktools-0.8.5rc0/src/linktools/assets/containers/100-nginx/dnsapi.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/110-portainer/container.py` & `linktools-0.8.5rc0/src/linktools/assets/containers/110-portainer/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/compose.yml` & `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/compose.yml`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/container.py` & `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/container.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/containers/120-flare/nginx.conf` & `linktools-0.8.5rc0/src/linktools/assets/containers/120-flare/nginx.conf`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/fake_useragent.json` & `linktools-0.8.5rc0/src/linktools/assets/fake_useragent.json`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/frida.js` & `linktools-0.8.5rc0/src/linktools/assets/frida.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/frida.min.js` & `linktools-0.8.5rc0/src/linktools/assets/frida.min.js`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/objection/plugins/__init__.py` & `linktools-0.8.5rc0/src/linktools/assets/objection/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/assets/tools.json` & `linktools-0.8.5rc0/src/linktools/assets/tools.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920454545454546%*

 * *Differences: {"'TOOL_JADX'": "{'version': '1.5.0'}",*

 * * "'TOOL_JADX_GUI'": "{'version': '1.5.0'}",*

 * * "'TOOL_SIB'": "{'version': '1.3.18-20240423'}"}*

```diff
@@ -426,15 +426,15 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
-        "version": "1.4.7"
+        "version": "1.5.0"
     },
     "TOOL_JADX_GUI": {
         "download_url": "https://github.com/skylot/jadx/releases/download/v{version}/jadx-{version}.zip",
         "name": "jadx-gui",
         "target_path": {
             "case": [
                 {
@@ -454,15 +454,15 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "jadx-{version}",
-        "version": "1.4.7"
+        "version": "1.5.0"
     },
     "TOOL_JAR2DEX": {
         "download_url": "https://github.com/pxb1988/dex2jar/releases/download/v{version}{version_suffix}/dex-tools-{version}{version_suffix}.zip",
         "target_path": {
             "case": [
                 {
                     "then": "dex-tools-{version}/d2j-{name}.sh",
@@ -671,15 +671,15 @@
                 },
                 {
                     "else": null
                 }
             ]
         },
         "unpack_path": "sib-{version}",
-        "version": "1.3.17-20240112"
+        "version": "1.3.18-20240423"
     },
     "TOOL_SMALI": {
         "depends_on": "java",
         "download_url": "https://bitbucket.org/JesusFreke/smali/downloads/smali-{version}.jar",
         "executable_cmdline": [
             "java",
             "-jar",
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/__init__.py` & `linktools-0.8.5rc0/src/linktools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/argparse.py` & `linktools-0.8.5rc0/src/linktools/cli/argparse.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,66 +24,50 @@
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 import abc
 import argparse
+import sys
 import typing
 
 from .. import utils
 
-if typing.TYPE_CHECKING:
-    import argcomplete
-
-auto_complete: "typing.Optional[argcomplete]" = None
-try:
-    import argcomplete
-
-    auto_complete = argcomplete
-except ModuleNotFoundError:
-    pass
-
-
-if auto_complete:
-
-    class ParserCompleter(abc.ABC):
-
-        @abc.abstractmethod
-        def get_parser(self) -> argparse.ArgumentParser:
-            pass
-
-        @abc.abstractmethod
-        def get_args(self, parsed_args: argparse.Namespace, **kwargs) -> typing.Optional[typing.List[str]]:
-            pass
-
-        def __call__(self, *, parsed_args, **kwargs):
-            completions = {}
+if sys.version_info < (3, 10):
 
-            args = self.get_args(parsed_args, **kwargs)
-            if args is None:
-                return completions
+    _orig_get_action_name = getattr(argparse, "_get_action_name", None)
+    if _orig_get_action_name is not None and callable(_orig_get_action_name):
+        def _get_action_name(argument):
+            result = _orig_get_action_name(argument)
+            if result is None:
+                if argument.choices:
+                    return '{' + ','.join(argument.choices) + '}'
+            return result
+
+        setattr(argparse, "_get_action_name", _get_action_name)
+
+
+##############################
+# argparse types
+##############################
 
-            finder = auto_complete.CompletionFinder(self.get_parser())
-            cmdline = f"{utils.list2cmdline(args)} "
-
-            state = 0
-            while True:
-                item = finder.rl_complete(cmdline, state)
-                if item is None:
-                    break
-                key = item[len(cmdline):]
-                completions[key] = finder.get_display_completions().get(key, "")
-                state += 1
+def range_type(min: int, max: int):
+    def wrapper(o):
+        value = utils.int(o)
+        if min <= value <= max:
+            return value
+        raise ValueError("value not in range %s-%s" % (min, max))
 
-            return completions
+    return wrapper
 
-else:
-    ParserCompleter = None
 
+##############################
+# argparse actions
+##############################
 
 if not hasattr(argparse, "BooleanOptionalAction"):
     class BooleanOptionalAction(argparse.Action):
         def __init__(self,
                      option_strings,
                      dest,
                      default=None,
@@ -161,15 +145,57 @@
                         raise argparse.ArgumentError(self, str(e))
                 else:
                     dest[k] = v
 
         setattr(namespace, self.dest, dest)
 
 
-def range_type(min: int, max: int):
-    def wrapper(o):
-        value = utils.int(o)
-        if min <= value <= max:
-            return value
-        raise ValueError("value not in range %s-%s" % (min, max))
+##############################
+# auto complete
+##############################
 
-    return wrapper
+if typing.TYPE_CHECKING:
+    import argcomplete
+
+auto_complete: "typing.Optional[argcomplete]" = None
+try:
+    import argcomplete
+
+    auto_complete = argcomplete
+except ModuleNotFoundError:
+    pass
+
+if auto_complete:
+
+    class ParserCompleter(abc.ABC):
+
+        @abc.abstractmethod
+        def get_parser(self) -> argparse.ArgumentParser:
+            pass
+
+        @abc.abstractmethod
+        def get_args(self, parsed_args: argparse.Namespace, **kwargs) -> typing.Optional[typing.List[str]]:
+            pass
+
+        def __call__(self, *, parsed_args, **kwargs):
+            completions = {}
+
+            args = self.get_args(parsed_args, **kwargs)
+            if args is None:
+                return completions
+
+            finder = auto_complete.CompletionFinder(self.get_parser())
+            cmdline = f"{utils.list2cmdline(args)} "
+
+            state = 0
+            while True:
+                item = finder.rl_complete(cmdline, state)
+                if item is None:
+                    break
+                key = item[len(cmdline):]
+                completions[key] = finder.get_display_completions().get(key, "")
+                state += 1
+
+            return completions
+
+else:
+    ParserCompleter = None
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/command.py` & `linktools-0.8.5rc0/src/linktools/cli/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,15 +531,15 @@
             if subcommand.has_parent:
                 parent_subparsers = subparsers_map.get(subcommand.parent_id, None)
                 if not parent_subparsers:
                     raise SubCommandError(f"Subcommand {subcommand} has no parent subparser")
 
             parser = subcommand.create_parser(type=parent_subparsers.add_parser)
             parser.set_defaults(**{f"__subcommand_{id(self):x}__": subcommand})
-            self.init_common_arguments(parser)
+            self.init_global_arguments(parser)
 
             if subcommand.is_group:
                 _subparsers = parser.add_subparsers(metavar="COMMAND", help="Command Help")
                 _subparsers.required = False
                 subparsers_map[subcommand.id] = _subparsers
 
             # BaseCommand 类型单独处理，因为有可能在init_arguments中添加了子命令
@@ -731,24 +731,24 @@
         self.init_base_arguments(parser)
         self.init_arguments(parser)
         return parser
 
     @cached_property
     def _argument_parser(self) -> ArgumentParser:
         parser = self.create_parser()
-        self.init_common_arguments(parser)
+        self.init_global_arguments(parser)
         return parser
 
     def init_base_arguments(self, parser: ArgumentParser) -> None:
         """
         初始化基础参数，在调用create_parser时执行
         """
         pass
 
-    def init_common_arguments(self, parser: ArgumentParser) -> None:
+    def init_global_arguments(self, parser: ArgumentParser) -> None:
         """
         初始化公共参数，会在命令本身和所有子命令中调用
         """
         environ = self.environ
         prefix = parser.prefix_chars[0] if parser.prefix_chars else "-"
 
         class VerboseAction(Action):
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/adb.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/adb.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/agent.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/agent.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/app.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 from linktools import utils, environ
-from linktools.android import Package, Permission, \
+from linktools.android import App, Permission, \
     Component, Activity, Service, Receiver, Provider, IntentFilter
 from linktools.cli import AndroidCommand
 
 
 class PrintLevel:
     min = 0
     useless = 100
@@ -89,103 +89,103 @@
         if max_level > self.max_level:
             max_level = self.max_level
         elif min_level < self.min_level:
             min_level = self.min_level
         return PrintStreamWrapper(self.stream, max_level=max_level, min_level=min_level)
 
 
-class PackagePrinter:
+class AppPrinter:
 
-    def __init__(self, stream: PrintStream, package: Package):
-        self.package = package
-        self.max_level = PrintLevel.max if self.package.enabled else PrintLevel.useless
+    def __init__(self, stream: PrintStream, app: App):
+        self.app = app
+        self.max_level = PrintLevel.max if self.app.enabled else PrintLevel.useless
         self.min_level = PrintLevel.min
         self.stream = PrintStreamWrapper(stream, max_level=self.max_level, min_level=self.min_level)
 
-    def print_package(self, indent: int = 0):
-        self.stream.print("Package [%s]" % self.package, indent=indent, level=self.stream.title)
-        self.stream.print("name=%s" % self.package.app_name, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("userId=%s" % self.package.user_id, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("gids=%s" % self.package.gids, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("sourceDir=%s" % self.package.source_dir, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("versionCode=%s" % self.package.version_code, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("versionName=%s" % self.package.version_name, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("enabled=%s" % self.package.enabled, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("system=%s" % self.package.system, indent=indent + 4, level=self.stream.normal)
-        self.stream.print("debuggable=%s" % self.package.debuggable, indent=indent + 4,
-                          level=self.stream.dangerous if self.package.debuggable else self.stream.normal)
-        self.stream.print("allowBackup=%s" % self.package.allow_backup, indent=indent + 4,
-                          level=self.stream.dangerous if self.package.allow_backup else self.stream.normal)
+    def print_app(self, indent: int = 0):
+        self.stream.print("App [%s]" % self.app, indent=indent, level=self.stream.title)
+        self.stream.print("name=%s" % self.app.app_name, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("userId=%s" % self.app.user_id, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("gids=%s" % self.app.gids, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("sourceDir=%s" % self.app.source_dir, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("versionCode=%s" % self.app.version_code, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("versionName=%s" % self.app.version_name, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("enabled=%s" % self.app.enabled, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("system=%s" % self.app.system, indent=indent + 4, level=self.stream.normal)
+        self.stream.print("debuggable=%s" % self.app.debuggable, indent=indent + 4,
+                          level=self.stream.dangerous if self.app.debuggable else self.stream.normal)
+        self.stream.print("allowBackup=%s" % self.app.allow_backup, indent=indent + 4,
+                          level=self.stream.dangerous if self.app.allow_backup else self.stream.normal)
         self.stream.print_line()
 
     def print_requested_permissions(self, indent: int = 4):
-        if not utils.is_empty(self.package.requested_permissions):
+        if not utils.is_empty(self.app.requested_permissions):
             stream = self.stream.create(max_level=PrintLevel.normal)
             self.stream.print("RequestedPermissions:", indent=indent, level=self.stream.title)
-            for permission in self.package.requested_permissions:
+            for permission in self.app.requested_permissions:
                 self._print_permission(stream, permission, indent=indent + 4, identity="RequestedPermission")
             self.stream.print_line()
 
     def print_permissions(self, indent: int = 4):
-        if not utils.is_empty(self.package.permissions):
+        if not utils.is_empty(self.app.permissions):
             self.stream.print("Permissions:", indent=indent, level=self.stream.title)
-            for permission in self.package.permissions:
+            for permission in self.app.permissions:
                 self._print_permission(self.stream, permission, indent=indent + 4, identity="Permission")
             self.stream.print_line()
 
     def print_activities(self, indent: int = 4):
-        if not utils.is_empty(self.package.activities):
+        if not utils.is_empty(self.app.activities):
             self.stream.print("Activities:", indent=indent, level=self.stream.title)
-            for activity in self.package.activities:
-                self._print_component(self.stream, self.package, activity, indent=indent + 4, identity="Activity")
+            for activity in self.app.activities:
+                self._print_component(self.stream, self.app, activity, indent=indent + 4, identity="Activity")
             self.stream.print_line()
 
     def print_services(self, indent: int = 4):
-        if not utils.is_empty(self.package.services):
+        if not utils.is_empty(self.app.services):
             self.stream.print("Services:", indent=indent, level=self.stream.title)
-            for service in self.package.services:
-                self._print_component(self.stream, self.package, service, indent=indent + 4, identity="Service")
+            for service in self.app.services:
+                self._print_component(self.stream, self.app, service, indent=indent + 4, identity="Service")
             self.stream.print_line()
 
     def print_receivers(self, indent: int = 4):
-        if not utils.is_empty(self.package.receivers):
+        if not utils.is_empty(self.app.receivers):
             self.stream.print("Receivers:", indent=indent, level=self.stream.title)
-            for receiver in self.package.receivers:
-                self._print_component(self.stream, self.package, receiver, indent=indent + 4, identity="Receiver")
+            for receiver in self.app.receivers:
+                self._print_component(self.stream, self.app, receiver, indent=indent + 4, identity="Receiver")
             self.stream.print_line()
 
     def print_providers(self, indent: int = 4):
-        if not utils.is_empty(self.package.providers):
+        if not utils.is_empty(self.app.providers):
             self.stream.print("Providers:", indent=indent, level=self.stream.title)
-            for provider in self.package.providers:
-                self._print_component(self.stream, self.package, provider, indent=indent + 4, identity="Provider")
+            for provider in self.app.providers:
+                self._print_component(self.stream, self.app, provider, indent=indent + 4, identity="Provider")
             self.stream.print_line()
 
     @classmethod
     def _print_permission(cls, stream: PrintStreamWrapper, permission: Permission, indent: int = 0,
                           identity: str = None):
         if permission.is_defined():
             stream.print("%s [%s] %s" % (identity, permission, permission.protection), indent=indent,
                          level=stream.dangerous if permission.is_dangerous() else stream.normal)
 
     @classmethod
-    def _print_component(cls, stream: PrintStreamWrapper, package: Package, component: Component, indent: int = 0, identity: str = None):
+    def _print_component(cls, stream: PrintStreamWrapper, app: App, component: Component, indent: int = 0, identity: str = None):
         if not component.enabled:
             description = "disabled"
             level = stream.useless
             stream = stream.create(max_level=stream.useless)
         elif component.is_dangerous():
             description = "exported"
             level = stream.dangerous if component.is_dangerous() else stream.normal
             stream = stream.create(min_level=stream.dangerous_normal)
         else:
             description = "exported" if component.exported else ""
             level = stream.normal
             stream = stream.create(max_level=stream.normal)
-        stream.print("%s [%s/%s] %s" % (identity, package, component, description), indent=indent, level=level)
+        stream.print("%s [%s/%s] %s" % (identity, app, component, description), indent=indent, level=level)
 
         if isinstance(component, Activity) or isinstance(component, Service) or isinstance(component, Receiver):
             cls._print_permission(stream, component.permission, indent=indent + 4, identity="Permission")
         elif isinstance(component, Provider):
             stream.print("Authority [%s]" % component.authority, indent=indent + 4, level=level)
             cls._print_permission(stream, component.read_permission, indent=indent + 4,
                                   identity="ReadPermission")
@@ -241,70 +241,70 @@
         group.add_argument('-u', '--uids', metavar="uid", action='store', nargs='+', type=int, default=None,
                            help='fetch apps with specified uids only')
         group.add_argument('--system', action='store_true', default=False,
                            help='fetch system apps only')
         group.add_argument('--non-system', action='store_true', default=False,
                            help='fetch non-system apps only')
 
-        parser.add_argument('--simple', action='store_true', default=False,
-                            help='display simple info only')
+        parser.add_argument('--detail', action='store_true', default=False,
+                            help='show app detail info')
         parser.add_argument('--dangerous', action='store_true', default=False,
-                            help='display dangerous permissions and components only')
+                            help='show app dangerous permissions and components only')
         parser.add_argument('-o', '--order-by', metavar="field", action='store', nargs='+', default=['userId', 'name'],
                             choices=['name', 'appName', 'userId', 'sourceDir',
                                      'enabled', 'system', 'debuggable', 'allowBackup'],
                             help='order by target field')
 
     def run(self, args: Namespace) -> Optional[int]:
         device = args.device_picker.pick()
 
         if not utils.is_empty(args.packages):
-            packages = device.get_packages(*args.packages, simple=args.simple)
+            apps = device.get_apps(*args.packages, detail=args.detail)
         elif not utils.is_empty(args.uids):
-            packages = device.get_packages_for_uid(*args.uids, simple=args.simple)
+            apps = device.get_apps_for_uid(*args.uids, detail=args.detail)
         elif args.system:
-            packages = device.get_packages(system=True, simple=args.simple)
+            apps = device.get_apps(system=True, detail=args.detail)
         elif args.non_system:
-            packages = device.get_packages(system=False, simple=args.simple)
+            apps = device.get_apps(system=False, detail=args.detail)
         elif args.all:
-            packages = device.get_packages(simple=args.simple)
+            apps = device.get_apps(detail=args.detail)
         else:
-            packages = device.get_packages(device.get_current_package(), simple=args.simple)
+            apps = device.get_apps(device.get_current_package(), detail=args.detail)
 
         if not utils.is_empty(args.order_by):
-            packages = sorted(packages, key=lambda x: [utils.get_item(x, k, default="") for k in args.order_by])
+            apps = sorted(apps, key=lambda x: [utils.get_item(x, k, default="") for k in args.order_by])
 
         min_level = PrintLevel.min
         if args.dangerous:
             min_level = PrintLevel.dangerous_normal
         stream = PrintStream(min_level=min_level)
 
-        for package in packages:
-            printer = PackagePrinter(stream, package)
+        for app in apps:
+            printer = AppPrinter(stream, app)
             if not args.dangerous:
-                printer.print_package()
+                printer.print_app()
                 printer.print_requested_permissions()
                 printer.print_permissions()
                 printer.print_activities()
                 printer.print_services()
                 printer.print_receivers()
                 printer.print_providers()
                 continue
 
-            if package.is_dangerous():
-                printer.print_package()
-                if package.has_dangerous_permission():
+            if app.is_dangerous():
+                printer.print_app()
+                if app.has_dangerous_permission():
                     printer.print_permissions()
-                if package.has_dangerous_activity():
+                if app.has_dangerous_activity():
                     printer.print_activities()
-                if package.has_dangerous_service():
+                if app.has_dangerous_service():
                     printer.print_services()
-                if package.has_dangerous_receiver():
+                if app.has_dangerous_receiver():
                     printer.print_receivers()
-                if package.has_dangerous_provider():
+                if app.has_dangerous_provider():
                     printer.print_providers()
 
         return
 
 
 command = Command()
 if __name__ == "__main__":
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/debug.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/debug.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/frida.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/info.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/info.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/intent.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/intent.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                      log_output=True)
 
     @subcommand("setting-app", help="start application setting activity (default: current running package)",
                 pass_args=True)
     @subcommand_argument("package")
     def on_setting_app(self, args: Namespace, package: str = None):
         device = args.device_picker.pick()
-        package = package if not utils.is_empty(package) else device.get_current_package()
+        package = package or device.get_current_package()
         device.shell("am", "start", "--user", "0",
                      "-a", "android.settings.APPLICATION_DETAILS_SETTINGS",
                      "-d", "package:%s" % package,
                      log_output=True)
 
     @subcommand("setting-cert", help="install cert (require \'/data/local/tmp\' write permission)", pass_args=True)
     @subcommand_argument("path")
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/objection.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/objection.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,16 @@
             if args.plugin_folder:
                 objection_args += ["--plugin-folder", args.plugin_folder]
 
             if args.redirect_address or args.redirect_port:
                 # 如果需要重定向到本地端口
                 address = args.redirect_address
                 port = args.redirect_port or 8080
-                info = device.get_package(package)
-                uid = info.user_id if info else None
+                app = device.get_app(package)
+                uid = app.user_id if app else None
                 with device.redirect(address, port, uid):
                     return utils.Process(*objection_args).call()
             else:
                 return utils.Process(*objection_args).call()
 
 
 command = Command()
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/pidcat.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/pidcat.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/android/top.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/android/top.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,36 +66,36 @@
         elif args.path:
             environ.logger.info(device.get_apk_path(device.get_current_package()))
         elif args.kill:
             device.shell("am", "force-stop", device.get_current_package(), log_output=True)
         elif "--apk" in sys.argv:
             package_name = device.get_current_package()
             environ.logger.info("find current package: {}".format(package_name))
-            package = utils.get_item(device.get_packages(package_name, simple=True), 0)
-            if package is not None:
-                environ.logger.info("find current apk path: {}".format(package.source_dir))
-                path = device.get_storage_path("{}_{}.apk".format(package.name, package.version_name))
+            app = device.get_app(package_name)
+            if app is not None:
+                environ.logger.info("find current apk path: {}".format(app.source_dir))
+                path = device.get_storage_path("{}_{}.apk".format(app.name, app.version_name))
                 dest = args.apk if not utils.is_empty(args.apk) else "."
                 device.shell("mkdir", "-p", device.get_storage_path(), log_output=True)
-                device.shell("cp", package.source_dir, path, log_output=True)
+                device.shell("cp", app.source_dir, path, log_output=True)
                 device.pull(path, dest, log_output=True)
                 device.shell("rm", path)
         elif "--screen" in sys.argv:
             now = datetime.datetime.now()
             path = device.get_storage_path("screenshot-" + now.strftime("%Y-%m-%d-%H-%M-%S") + ".png")
             dest = args.screen if not utils.is_empty(args.screen) else "."
             device.shell("mkdir", "-p", device.get_storage_path(), log_output=True)
             device.shell("screencap", "-p", path, log_output=True)
             device.pull(path, dest, log_output=True)
             device.shell("rm", path)
         else:
-            package = device.get_current_package()
-            environ.logger.info("package:  ", package)
+            app = device.get_current_package()
+            environ.logger.info("package:  ", app)
             environ.logger.info("activity: ", device.get_current_activity())
-            environ.logger.info("path:     ", device.get_apk_path(package))
+            environ.logger.info("path:     ", device.get_apk_path(app))
 
         return
 
 
 command = Command()
 if __name__ == "__main__":
     command.main()
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/common/cert.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/common/cert.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/common/cntr.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/common/cntr.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/common/env.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/common/env.py`

 * *Files 19% similar despite different names*

```diff
@@ -93,66 +93,84 @@
         if command:
             process = utils.Process(command, shell=True)
             return process.call()
 
         process = shell.popen()
         return process.call()
 
-    @subcommand("complete", help="generate shell auto complete script")
+    @subcommand("completion", help="generate shell auto complete script")
     @subcommand_argument("-s", "--shell", help="output code for the specified shell",
                          choices=["bash", "zsh", "tcsh", "fish", "powershell"])
-    def on_complete(self, shell: str = DEFAULT_SHELL):
+    @subcommand_argument("--sync", action="store_true", help="sync complete script")
+    def on_completion(self, shell: str = DEFAULT_SHELL, sync: bool = False):
         if not auto_complete:
             self.logger.warning("argcomplete module not found")
             return
 
+        path = self.environ.get_data_path("scripts", "complete", create_parent=True)
+        if not sync and os.path.exists(path):
+            self.logger.info(f"Found complete script: {path}")
+            print(utils.read_file(path, text=True), flush=True)
+            return 0
+
         executables = []
         modules = {c.name: c for c in iter_command_modules(commands, onerror="warn")}
         for module in modules.values():
             if module.command:
                 temp = module
                 names = [module.command_name]
                 while temp.parent_name in modules:
                     temp = modules[temp.parent_name]
                     names.append(temp.command_name)
                 executable = "-".join(reversed(names))
                 executables.append(executable)
-                self.logger.info(f"found executable: {executable}")
+                self.logger.info(f"Found executable: {executable}")
 
-        print(auto_complete.shellcode(executables, shell=shell), flush=True)
+        result = auto_complete.shellcode(executables, shell=shell)
+        utils.write_file(path, result)
+        print(result, flush=True)
 
     @subcommand("alias", help="generate shell alias script")
     @subcommand_argument("-s", "--shell", help="output code for the specified shell",
                          choices=["bash", "zsh", "tcsh", "fish", "powershell"])
-    def on_alias(self, shell: str = DEFAULT_SHELL):
+    @subcommand_argument("--sync", action="store_true", help="sync alias script")
+    def on_alias(self, shell: str = DEFAULT_SHELL, sync: bool = False):
+        path = self.environ.get_data_path("scripts", "alias", create_parent=True)
+        if not sync and os.path.exists(path):
+            self.logger.info(f"Found alias script: {path}")
+            print(utils.read_file(path, text=True), flush=True)
+            return 0
+
         lines = []
         if shell not in ("powershell",):
             lines.append(f"#!/usr/bin/env {shell}")
 
         modules = {c.name: c for c in iter_command_modules(commands, onerror="warn")}
         for module in modules.values():
             if module.command:
                 temp = module
                 names = [module.command_name]
                 while temp.parent_name in modules:
                     temp = modules[temp.parent_name]
                     names.append(temp.command_name)
                 executable = "-".join(reversed(names))
                 cmdline = list2cmdline([sys.executable, "-m", module.module.__name__])
-                self.logger.info(f"found alias: {executable} -> {cmdline}")
+                self.logger.info(f"Found alias: {executable} -> {cmdline}")
 
                 if shell in ("bash", "zsh"):
                     lines.append(f"alias {executable}='{cmdline}'")
                 elif shell in ("tcsh", "fish"):
                     lines.append(f"alias {executable} '{cmdline}'")
                 elif shell in ("powershell",):
                     lines.append(f"function __{executable}__ {{ {cmdline} $args }}")
                     lines.append(f"Set-Alias -Name {executable} -Value __{executable}__")
 
-        print(os.linesep.join(lines), flush=True)
+        result = os.linesep.join(lines)
+        utils.write_file(path, result)
+        print(result, flush=True)
 
     @subcommand("clean", help="clean temporary files")
     @subcommand_argument("days", metavar="DAYS", nargs="?", help="expire days")
     def on_clean(self, days: int = 7):
         self.environ.clean_temp_files(days)
```

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/common/grep.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/common/grep.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/common/tools.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/common/tools.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/frida.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/frida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ipa.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/objection.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/objection.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/scp.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/scp.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/sib.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/sib.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/commands/ios/ssh.py` & `linktools-0.8.5rc0/src/linktools/cli/commands/ios/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/cli/device.py` & `linktools-0.8.5rc0/src/linktools/cli/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/container/__init__.py` & `linktools-0.8.5rc0/src/linktools/frida/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : __init__.py.py 
-@time    : 2023/05/21
-@site    :  
-@software: PyCharm 
+@file    : frida.py
+@time    : 2018/11/25
+@site    :
+@software: PyCharm
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -23,9 +23,10 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .container import ContainerError, BaseContainer, ExposeLink, ExposeCategory
-from .manager import ContainerManager
+from .app import FridaApplication
+from .script import FridaScriptFile, FridaShareScript, FridaEvalCode
+from .server import FridaServer
```

### Comparing `linktools-0.8.4rc0/src/linktools/container/container.py` & `linktools-0.8.5rc0/src/linktools/container/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,20 +89,18 @@
             return f"{'https' if https else 'http'}://{domain}:{port}/"
         return None
 
 
 class NginxMixin:
 
     def get_nginx_domain(self: "BaseContainer", name: str = None):
-        if not self.manager.containers["nginx"].enable:
-            return ""
-        if not self.is_depend_on("nginx"):
-            return ""
 
         def get_domain(cfg: Config):
+            if not self.manager.containers["nginx"].enable:
+                return ""
             if not cfg.get("WILDCARD_DOMAIN", type=bool):
                 return cfg.get("ROOT_DOMAIN")
             if name is None:
                 return f"{self.name}.{cfg.get('ROOT_DOMAIN')}"
             elif name.strip() == "":
                 return cfg.get("ROOT_DOMAIN")
             return f"{name}.{cfg.get('ROOT_DOMAIN')}"
```

### Comparing `linktools-0.8.4rc0/src/linktools/container/manager.py` & `linktools-0.8.5rc0/src/linktools/container/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
         for url, meta in self.get_all_repos().items():
             self.logger.debug(f"Load containers from repository `{url}`")
             repo_path = meta.get("repo_path")
             if not repo_path or not os.path.exists(repo_path) or not os.path.isdir(repo_path):
                 self.logger.warning(f"Repository `{url}` not found, skip.")
                 continue
-            for container in self._walk_containers(repo_path, max_level=1):
+            for container in self._walk_containers(repo_path, max_level=2):
                 containers.append(container)
 
         return containers
 
     def _walk_containers(self, path: str, max_level: int):
         if not os.path.isdir(path):
             return
```

### Comparing `linktools-0.8.4rc0/src/linktools/container/repository.py` & `linktools-0.8.5rc0/src/linktools/container/repository.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/decorator.py` & `linktools-0.8.5rc0/src/linktools/decorator.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/device.py` & `linktools-0.8.5rc0/src/linktools/device.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/frida/__init__.py` & `linktools-0.8.5rc0/src/linktools/android/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 @author  : Hu Ji
-@file    : frida.py
-@time    : 2018/11/25
-@site    :
-@software: PyCharm
+@file    : __init__.py
+@time    : 2020/03/01
+@site    :  
+@software: PyCharm 
 
               ,----------------,              ,---------,
          ,-----------------------,          ,"        ,"|
        ,"                      ,"|        ,"        ,"  |
       +-----------------------+  |      ,"        ,"    |
       |  .-----------------.  |  |     +---------+      |
       |  |                 |  |  |     | -==----'|      |
@@ -23,10 +23,9 @@
          /_)______________(_/  //'   | +---------+
     ___________________________/___  `,
    /  oooooooooooooooo  .o.  oooo /,   \,"-----------
   / ==ooooooooooooooo==.o.  ooo= //   ,`\--{)B     ,"
  /_==__==========__==_ooo__ooo=_/'   /___________,"
 """
 
-from .app import FridaApplication
-from .script import FridaScriptFile, FridaShareScript, FridaEvalCode
-from .server import FridaServer
+from .adb import Adb, Device, AdbError
+from .struct import App, Permission, Component, Activity, Service, Receiver, Provider, IntentFilter
```

### Comparing `linktools-0.8.4rc0/src/linktools/frida/android.py` & `linktools-0.8.5rc0/src/linktools/frida/android.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/frida/app.py` & `linktools-0.8.5rc0/src/linktools/frida/app.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/frida/ios.py` & `linktools-0.8.5rc0/src/linktools/frida/ios.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/frida/script.py` & `linktools-0.8.5rc0/src/linktools/frida/script.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/frida/server.py` & `linktools-0.8.5rc0/src/linktools/frida/server.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/ida/__init__.py` & `linktools-0.8.5rc0/src/linktools/ida/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/ida/ida.py` & `linktools-0.8.5rc0/src/linktools/ida/ida.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/ios/ipa.py` & `linktools-0.8.5rc0/src/linktools/ios/ipa.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/ios/sib.py` & `linktools-0.8.5rc0/src/linktools/ios/sib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import json
 import subprocess
 import time
 from subprocess import TimeoutExpired
-from typing import Any, Generator, List
+from typing import Any, Generator, List, Optional
 
+from .struct import Process, App
 from .. import utils
 from .._environ import environ
 from ..decorator import cached_property
 from ..device import BridgeError, Bridge, BaseDevice
 from ..reactor import Stoppable
 
 _logger = environ.get_logger("android.adb")
@@ -125,14 +126,76 @@
     def install(self, path: str, **kwargs) -> str:
         return self.exec("app", "install", "--path", path, **kwargs)
 
     @utils.timeoutable
     def uninstall(self, bundle_id: str, **kwargs) -> str:
         return self.exec("app", "uninstall", "--bundleId", bundle_id, **kwargs)
 
+    @utils.timeoutable
+    def kill(self, bundle_id: str, **kwargs) -> str:
+        return self.exec("app", "kill", "--bundleId", bundle_id, **kwargs)
+
+    @utils.timeoutable
+    def get_app(self, bundle_id: str, detail: bool = None, **kwargs) -> Optional[App]:
+        """
+        根据包名获取包信息
+        :param bundle_id: 包名
+        :param detail: 获取详细信息
+        :return: 包信息
+        """
+        options = ["--format", "--system"]
+        if detail is True:
+            options.append("--icon")
+
+        out = json.loads(self.exec("app", "list", *options, **kwargs))
+        for obj in utils.get_list_item(out, "appList"):
+            app = App(obj)
+            if bundle_id == app.bundle_id:
+                return app
+
+        return None
+
+    @utils.timeoutable
+    def get_apps(self, *bundle_ids: str, system: bool = None, detail: bool = False, **kwargs) -> [App]:
+        """
+        获取包信息
+        :param bundle_ids: 需要匹配的所有包名，为空则匹配所有
+        :param system: true只匹配系统应用，false只匹配非系统应用，为空则全匹配
+        :param detail: 获取详细信息
+        :return: 包信息
+        """
+        options = ["--format"]
+        if detail is True:
+            options.append("--icon")
+        if system is not False:
+            options.append("--system")
+
+        exclude = []
+        if system is True:
+            exclude = [o.bundle_id for o in self.get_apps(system=False, detail=False, **kwargs)]
+
+        result = []
+        out = json.loads(self.exec("app", "list", *options, **kwargs))
+        for obj in utils.get_list_item(out, "appList"):
+            app = App(obj)
+            if app.bundle_id in bundle_ids:
+                result.append(app)
+            elif app.bundle_id not in exclude:
+                result.append(app)
+
+        return result
+
+    @utils.timeoutable
+    def get_processes(self, **kwargs):
+        result = []
+        objs = json.loads(self.exec("ps", "-f", **kwargs))
+        for obj in objs:
+            result.append(Process(obj))
+        return result
+
     def forward(self, local_port: int, remote_port: int):
         process = self.popen(
             "proxy",
             "--local-port", local_port,
             "--remote-port", remote_port,
             text=True,
             bufsize=1,
```

### Comparing `linktools-0.8.4rc0/src/linktools/metadata.py` & `linktools-0.8.5rc0/src/linktools/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 class __MissingType:
     __eq__ = lambda l, r: \
         l is r or type(l) is type(r)
 
 
 __name__ = "linktools"
 __release__ = True
-__version__ = "0.8.4rc0"
+__version__ = "0.8.5rc0"
 __missing__ = __MissingType()
 __description__ = f"""\
     ___       __   __              __
    / (_)___  / /__/ /_____  ____  / /____
-  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.4rc0)
+  / / / __ \\/ //_/ __/ __ \\/ __ \\/ / ___/  linktools toolkit (v0.8.5rc0)
  / / / / / / ,< / /_/ /_/ / /_/ / (__  )   by: Hu Ji <669898595@qq.com>
 /_/_/_/ /_/_/|_|\\__/\\____/\\____/_/____/
 """
```

### Comparing `linktools-0.8.4rc0/src/linktools/reactor.py` & `linktools-0.8.5rc0/src/linktools/reactor.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/references/fake_useragent/fake.py` & `linktools-0.8.5rc0/src/linktools/references/fake_useragent/fake.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/references/fake_useragent/utils.py` & `linktools-0.8.5rc0/src/linktools/references/fake_useragent/utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/rich.py` & `linktools-0.8.5rc0/src/linktools/rich.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/ssh.py` & `linktools-0.8.5rc0/src/linktools/ssh.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/utils/__init__.py` & `linktools-0.8.5rc0/src/linktools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/utils/_port.py` & `linktools-0.8.5rc0/src/linktools/utils/_port.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/utils/_proxy.py` & `linktools-0.8.5rc0/src/linktools/utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/utils/_subprocess.py` & `linktools-0.8.5rc0/src/linktools/utils/_subprocess.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools/utils/_utils.py` & `linktools-0.8.5rc0/src/linktools/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools.egg-info/PKG-INFO` & `linktools-0.8.5rc0/src/linktools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linktools
-Version: 0.8.4rc0
+Version: 0.8.5rc0
 Summary: linktools toolkit
 Author-email: Hu Ji <669898595@qq.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/ice-black-tea/linktools
 Project-URL: Repository, https://github.com/ice-black-tea/linktools.git
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -71,15 +71,15 @@
 额外的依赖项以及相应功能可通过[requirements.yml](https://raw.githubusercontent.com/ice-black-tea/linktools/master/requirements.yml)查看
 
 ### 配置alias（推荐）
 
 对于*nix等系统，推荐在~/.bashrc 或 ~/.bash_profile 或 ~/.zshrc等文件中配置alias，简化调用方式：
 
 ```bash
-eval "$(ct-env --silent complete --shell bash)" # 给命令添加自动补全功能
+eval "$(ct-env --silent completion --shell bash)" # 给命令添加自动补全功能
 
 alias adb="at-adb"
 alias pidcat="at-pidcat"
 alias sib="it-sib"
 
 alias apktool="ct-tools apktool"
 alias burpsuite="ct-tools --set version=2023.10 burpsuite"
```

### Comparing `linktools-0.8.4rc0/src/linktools.egg-info/SOURCES.txt` & `linktools-0.8.5rc0/src/linktools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 src/linktools/frida/script.py
 src/linktools/frida/server.py
 src/linktools/ida/__init__.py
 src/linktools/ida/ida.py
 src/linktools/ios/__init__.py
 src/linktools/ios/ipa.py
 src/linktools/ios/sib.py
+src/linktools/ios/struct.py
 src/linktools/references/__init__.py
 src/linktools/references/fake_useragent/__init__.py
 src/linktools/references/fake_useragent/errors.py
 src/linktools/references/fake_useragent/fake.py
 src/linktools/references/fake_useragent/log.py
 src/linktools/references/fake_useragent/settings.py
 src/linktools/references/fake_useragent/utils.py
```

### Comparing `linktools-0.8.4rc0/src/linktools.egg-info/entry_points.txt` & `linktools-0.8.5rc0/src/linktools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `linktools-0.8.4rc0/src/linktools.egg-info/requires.txt` & `linktools-0.8.5rc0/src/linktools.egg-info/requires.txt`

 * *Files identical despite different names*

