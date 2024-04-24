# Comparing `tmp/nixos_compose-0.5.5.tar.gz` & `tmp/nixos_compose-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixos_compose-0.5.5.tar", max compression
+gzip compressed data, was "nixos_compose-0.5.6.tar", max compression
```

## Comparing `nixos_compose-0.5.5.tar` & `nixos_compose-0.5.6.tar`

### file list

```diff
@@ -1,123 +1,126 @@
--rw-r--r--   0        0        0     1094 2022-02-22 14:04:48.131501 nixos_compose-0.5.5/LICENSE
--rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/basic/composition.nix
--rw-r--r--   0        0        0      561 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic/nxc.json
--rw-r--r--   0        0        0      216 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/basic-nur/composition.nix
--rw-r--r--   0        0        0     1043 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic-nur/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/basic-nur/nxc.json
--rw-r--r--   0        0        0      214 2023-01-26 10:45:07.461353 nixos_compose-0.5.5/examples/execo/composition.nix
--rw-r--r--   0        0        0     2543 2022-03-05 16:55:24.727775 nixos_compose-0.5.5/examples/execo/execo_script.py
--rw-r--r--   0        0        0      963 2022-11-24 15:29:17.851309 nixos_compose-0.5.5/examples/execo/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/execo/nxc.json
--rw-r--r--   0        0        0      569 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/flake.lock
--rw-r--r--   0        0        0      200 2023-06-01 07:45:30.792496 nixos_compose-0.5.5/examples/kernel/#linux_5_4.nix#
--rw-r--r--   0        0        0       96 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/kernel/compositions.nix
--rw-r--r--   0        0        0      577 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/kernel/flake.nix
--rw-r--r--   0        0        0      200 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/kernel/linux_5_4.nix
--rw-r--r--   0        0        0      907 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/kernel/linux_ipanema_5_4.nix
--rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/kernel/nxc.json
--rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/multi-compositions/bar-composition.nix
--rw-r--r--   0        0        0       80 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/multi-compositions/compositions.nix
--rw-r--r--   0        0        0      571 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/multi-compositions/flake.nix
--rw-r--r--   0        0        0      132 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/multi-compositions/foo-composition.nix
--rw-r--r--   0        0        0       51 2022-02-22 14:04:48.132501 nixos_compose-0.5.5/examples/multi-compositions/nxc.json
--rw-r--r--   0        0        0      569 2022-12-07 13:41:00.974492 nixos_compose-0.5.5/examples/nbp-mpi/composition.nix
--rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.5/examples/nbp-mpi/flake.nix
--rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.5/examples/nbp-mpi/nxc.json
--rw-r--r--   0        0        0     1113 2022-12-13 15:48:10.081561 nixos_compose-0.5.5/examples/nix_flake_templates.nix
--rw-r--r--   0        0        0     2141 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/nixos-cluster/composition.nix
--rw-r--r--   0        0        0      703 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/nixos-cluster/flake.nix
--rw-r--r--   0        0        0       49 2022-06-14 14:20:20.160507 nixos_compose-0.5.5/examples/nixos-cluster/nodes.yaml
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/nixos-cluster/nxc.json
--rw-r--r--   0        0        0     4455 2022-06-14 14:20:20.160507 nixos_compose-0.5.5/examples/nixos-cluster/ssh-keys.nix
--rw-r--r--   0        0        0      499 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/scripts/composition.nix
--rw-r--r--   0        0        0      563 2022-11-24 15:29:17.852309 nixos_compose-0.5.5/examples/scripts/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/scripts/nxc.json
--rw-r--r--   0        0        0      484 2022-04-14 09:01:13.303530 nixos_compose-0.5.5/examples/scripts/scripts/scripts.nix
--rw-r--r--   0        0        0       83 2022-04-14 09:01:13.303530 nixos_compose-0.5.5/examples/scripts/scripts/test_python.py
--rw-r--r--   0        0        0      465 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/setup/composition.nix
--rw-r--r--   0        0        0      593 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/setup/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/setup/nxc.json
--rw-r--r--   0        0        0     2917 2022-11-29 09:02:17.732640 nixos_compose-0.5.5/examples/setup/setup.toml
--rw-r--r--   0        0        0      691 2022-12-13 15:48:45.830622 nixos_compose-0.5.5/examples/shared-directories-users/composition.nix
--rw-r--r--   0        0        0      807 2022-12-06 21:39:45.820352 nixos_compose-0.5.5/examples/shared-directories-users/flake.nix
--rw-r--r--   0        0        0       60 2022-12-06 21:41:04.858427 nixos_compose-0.5.5/examples/shared-directories-users/nxc.json
--rw-r--r--   0        0        0      561 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/spark/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/spark/nxc.json
--rw-r--r--   0        0        0     1321 2022-02-22 14:04:48.133501 nixos_compose-0.5.5/examples/spark/spark_sample.py
--rw-r--r--   0        0        0      600 2023-01-26 10:45:07.462353 nixos_compose-0.5.5/examples/webserver/composition.nix
--rw-r--r--   0        0        0      571 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/webserver/flake.nix
--rw-r--r--   0        0        0       60 2022-11-24 15:29:17.853309 nixos_compose-0.5.5/examples/webserver/nxc.json
--rw-r--r--   0        0        0     1262 2022-12-02 16:34:24.566369 nixos_compose-0.5.5/nix/all-in-one.nix
--rw-r--r--   0        0        0     4160 2022-12-13 14:43:53.255994 nixos_compose-0.5.5/nix/compose.nix
--rw-r--r--   0        0        0     3246 2022-12-14 09:39:16.792209 nixos_compose-0.5.5/nix/flavours/docker/generate_docker_compose.nix
--rw-r--r--   0        0        0      569 2023-02-04 17:11:24.096024 nixos_compose-0.5.5/nix/flavours/docker/generate_image.nix
--rw-r--r--   0        0        0      816 2022-12-14 09:39:18.846217 nixos_compose-0.5.5/nix/flavours/docker/nxc-shared-dirs-docker.nix
--rw-r--r--   0        0        0      864 2022-07-15 20:53:49.903272 nixos_compose-0.5.5/nix/flavours/docker/systemd.nix
--rw-r--r--   0        0        0      229 2022-12-13 14:44:36.394071 nixos_compose-0.5.5/nix/flavours/docker.nix
--rw-r--r--   0        0        0      598 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/g5k-image.nix
--rw-r--r--   0        0        0     1966 2022-10-16 19:45:24.422173 nixos_compose-0.5.5/nix/flavours/g5k-nfs-store.nix
--rw-r--r--   0        0        0      273 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/g5k-ramdisk.nix
--rw-r--r--   0        0        0     1572 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/shared/base-hardware.nix
--rw-r--r--   0        0        0     1595 2022-12-12 21:04:21.027452 nixos_compose-0.5.5/nix/flavours/shared/base-vm.nix
--rw-r--r--   0        0        0      233 2023-02-04 17:12:54.022653 nixos_compose-0.5.5/nix/flavours/shared/base.nix
--rw-r--r--   0        0        0     5325 2023-02-04 17:14:20.565360 nixos_compose-0.5.5/nix/flavours/shared/common.nix
--rw-r--r--   0        0        0     1080 2023-03-22 14:08:21.310405 nixos_compose-0.5.5/nix/flavours/shared/g5k-common.nix
--rw-r--r--   0        0        0     1034 2023-02-23 08:34:27.688629 nixos_compose-0.5.5/nix/flavours/shared/g5k-ssh-host-keys.nix
--rw-r--r--   0        0        0     3508 2023-02-04 17:12:54.022653 nixos_compose-0.5.5/nix/flavours/shared/installation-device.nix
--rw-r--r--   0        0        0     2164 2022-02-22 14:04:48.134501 nixos_compose-0.5.5/nix/flavours/shared/netboot.nix
--rw-r--r--   0        0        0     1117 2022-12-13 15:41:18.469931 nixos_compose-0.5.5/nix/flavours/shared/nxc-shared-dirs-nfs.nix
--rw-r--r--   0        0        0     6669 2022-12-13 14:59:40.067304 nixos_compose-0.5.5/nix/flavours/shared/nxc.nix
--rw-r--r--   0        0        0     4183 2022-03-31 15:28:32.595831 nixos_compose-0.5.5/nix/flavours/shared/ssh-keys.nix
--rw-r--r--   0        0        0     6531 2022-12-02 16:37:56.969166 nixos_compose-0.5.5/nix/flavours/shared/stage-1-cmds.nix
--rw-r--r--   0        0        0     4044 2022-12-02 16:44:37.256556 nixos_compose-0.5.5/nix/flavours/shared/vm-stage-1-cmds.nix
--rw-r--r--   0        0        0      435 2022-04-08 15:45:40.641198 nixos_compose-0.5.5/nix/flavours/vm-ramdisk.nix
--rw-r--r--   0        0        0     1440 2023-07-10 15:40:24.993694 nixos_compose-0.5.5/nix/flavours/vm.nix
--rw-r--r--   0        0        0      982 2022-11-24 15:29:17.854309 nixos_compose-0.5.5/nix/flavours.json
--rw-r--r--   0        0        0      280 2022-11-24 15:29:17.854309 nixos_compose-0.5.5/nix/flavours.nix
--rw-r--r--   0        0        0      485 2022-02-22 14:08:06.721066 nixos_compose-0.5.5/nix/flavours2json.nix
--rw-r--r--   0        0        0     1970 2022-12-06 21:37:58.348959 nixos_compose-0.5.5/nix/generate_one_composition_info.nix
--rw-r--r--   0        0        0     1830 2022-03-09 21:28:29.653733 nixos_compose-0.5.5/nix/helpers.nix
--rw-r--r--   0        0        0      421 2022-03-07 19:13:07.567657 nixos_compose-0.5.5/nix/lib.nix
--rw-r--r--   0        0        0     1625 2022-02-22 14:04:48.135501 nixos_compose-0.5.5/nix/make-system-tarball.nix
--rw-r--r--   0        0        0     1540 2022-02-22 14:04:48.135501 nixos_compose-0.5.5/nix/make-system-tarball.sh
--rw-r--r--   0        0        0     6485 2022-12-01 14:50:43.355868 nixos_compose-0.5.5/nix/multiple_compositions.nix
--rw-r--r--   0        0        0      989 2023-03-22 14:08:21.286405 nixos_compose-0.5.5/nix/nur.nix
--rw-r--r--   0        0        0      795 2022-11-24 15:29:17.856309 nixos_compose-0.5.5/nix/one_composition.nix
--rw-r--r--   0        0        0     7234 2022-08-18 12:16:09.421462 nixos_compose-0.5.5/nix/setup.nix
--rw-r--r--   0        0        0        0 2022-09-22 15:03:49.416636 nixos_compose-0.5.5/nixos_compose/__init__.py
--rw-r--r--   0        0        0    30734 2023-01-26 14:02:56.121415 nixos_compose-0.5.5/nixos_compose/actions.py
--rw-r--r--   0        0        0     1877 2023-01-26 10:36:12.287610 nixos_compose-0.5.5/nixos_compose/cli.py
--rw-r--r--   0        0        0        0 2022-09-22 15:03:49.417636 nixos_compose-0.5.5/nixos_compose/commands/__init__.py
--rw-r--r--   0        0        0     9282 2023-04-12 07:53:33.247814 nixos_compose-0.5.5/nixos_compose/commands/cmd_build.py
--rw-r--r--   0        0        0      553 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/commands/cmd_clean.py
--rw-r--r--   0        0        0     1923 2022-10-28 08:47:49.562457 nixos_compose-0.5.5/nixos_compose/commands/cmd_connect.py
--rw-r--r--   0        0        0     2946 2022-10-20 15:49:47.707461 nixos_compose-0.5.5/nixos_compose/commands/cmd_driver.py
--rw-r--r--   0        0        0     2415 2023-03-22 14:08:21.301405 nixos_compose-0.5.5/nixos_compose/commands/cmd_helper.py
--rw-r--r--   0        0        0     4946 2023-01-26 10:36:12.284609 nixos_compose-0.5.5/nixos_compose/commands/cmd_init.py
--rw-r--r--   0        0        0    11838 2023-06-02 12:45:49.039451 nixos_compose-0.5.5/nixos_compose/commands/cmd_start.py
--rw-r--r--   0        0        0     1794 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/commands/cmd_stop.py
--rw-r--r--   0        0        0     9295 2023-02-01 16:48:32.365354 nixos_compose-0.5.5/nixos_compose/context.py
--rw-r--r--   0        0        0      388 2022-10-16 19:36:37.501675 nixos_compose-0.5.5/nixos_compose/default_role.py
--rwxr-xr-x   0        0        0      522 2022-02-22 14:04:48.136501 nixos_compose-0.5.5/nixos_compose/driver/__init__.py
--rw-r--r--   0        0        0     5210 2023-01-26 10:34:01.481292 nixos_compose-0.5.5/nixos_compose/driver/driver.py
--rw-r--r--   0        0        0     3250 2022-02-22 14:04:48.137501 nixos_compose-0.5.5/nixos_compose/driver/logger.py
--rw-r--r--   0        0        0    31187 2022-12-07 22:00:33.217394 nixos_compose-0.5.5/nixos_compose/driver/machine.py
--rw-r--r--   0        0        0     3395 2022-11-24 15:29:17.857309 nixos_compose-0.5.5/nixos_compose/driver/vlan.py
--rw-r--r--   0        0        0      706 2022-12-07 08:44:23.047801 nixos_compose-0.5.5/nixos_compose/flavour.py
--rw-r--r--   0        0        0     1568 2022-11-24 15:29:17.857309 nixos_compose-0.5.5/nixos_compose/flavours/__init__.py
--rw-r--r--   0        0        0     9765 2022-12-14 10:02:34.320312 nixos_compose-0.5.5/nixos_compose/flavours/docker.py
--rw-r--r--   0        0        0     7864 2023-07-10 15:36:50.778526 nixos_compose-0.5.5/nixos_compose/flavours/grid5000.py
--rw-r--r--   0        0        0     7077 2022-12-07 11:22:38.116441 nixos_compose-0.5.5/nixos_compose/flavours/vm.py
--rw-r--r--   0        0        0      602 2023-03-22 14:08:21.301405 nixos_compose-0.5.5/nixos_compose/g5k.py
--rw-r--r--   0        0        0     2187 2022-11-24 15:29:17.858309 nixos_compose-0.5.5/nixos_compose/httpd.py
--rw-r--r--   0        0        0     4285 2023-06-02 12:45:49.039451 nixos_compose-0.5.5/nixos_compose/nxc_execo.py
--rw-r--r--   0        0        0     3748 2022-11-24 15:29:17.858309 nixos_compose-0.5.5/nixos_compose/platform.py
--rw-r--r--   0        0        0     4034 2022-12-14 12:23:12.769245 nixos_compose-0.5.5/nixos_compose/setup.py
--rw-r--r--   0        0        0      953 2022-08-05 16:00:06.477496 nixos_compose-0.5.5/nixos_compose/state.py
--rw-r--r--   0        0        0        0 2022-03-26 18:59:34.690617 nixos_compose-0.5.5/nixos_compose/tools/__init__.py
--rwxr-xr-x   0        0        0      248 2022-03-26 19:00:47.951249 nixos_compose-0.5.5/nixos_compose/tools/g5k_set_pub_key_sleep.sh
--rwxr-xr-x   0        0        0     5010 2022-02-22 14:04:48.138501 nixos_compose-0.5.5/nixos_compose/tools/kataract.py
--rw-r--r--   0        0        0     2372 2022-02-22 14:04:48.138501 nixos_compose-0.5.5/nixos_compose/utils.py
--rw-r--r--   0        0        0     1064 2023-07-10 15:43:11.937605 nixos_compose-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 nixos_compose-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-01-11 17:28:25.788006 nixos_compose-0.5.6/LICENSE
+-rw-r--r--   0        0        0      216 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/composition.nix
+-rw-r--r--   0        0        0      561 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic/nxc.json
+-rw-r--r--   0        0        0      216 2024-01-11 17:28:25.797006 nixos_compose-0.5.6/examples/basic-nur/composition.nix
+-rw-r--r--   0        0        0     1043 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic-nur/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/basic-nur/nxc.json
+-rw-r--r--   0        0        0      214 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/composition.nix
+-rw-r--r--   0        0        0     2964 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/execo_script.py
+-rw-r--r--   0        0        0      963 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/execo/nxc.json
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/flake.lock
+-rw-r--r--   0        0        0       96 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/compositions.nix
+-rw-r--r--   0        0        0      577 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/flake.nix
+-rw-r--r--   0        0        0      200 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/linux_5_4.nix
+-rw-r--r--   0        0        0      907 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/linux_ipanema_5_4.nix
+-rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/kernel/nxc.json
+-rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/bar-composition.nix
+-rw-r--r--   0        0        0       80 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/compositions.nix
+-rw-r--r--   0        0        0      571 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/flake.nix
+-rw-r--r--   0        0        0      132 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/foo-composition.nix
+-rw-r--r--   0        0        0       51 2024-01-11 17:28:25.798006 nixos_compose-0.5.6/examples/multi-compositions/nxc.json
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/composition.nix
+-rw-r--r--   0        0        0      807 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nbp-mpi/nxc.json
+-rw-r--r--   0        0        0     1113 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nix_flake_templates.nix
+-rw-r--r--   0        0        0     2141 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/composition.nix
+-rw-r--r--   0        0        0      703 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/flake.nix
+-rw-r--r--   0        0        0       49 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/nodes.yaml
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/nxc.json
+-rw-r--r--   0        0        0     4455 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/nixos-cluster/ssh-keys.nix
+-rw-r--r--   0        0        0      499 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/composition.nix
+-rw-r--r--   0        0        0      563 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/nxc.json
+-rw-r--r--   0        0        0      484 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/scripts/scripts.nix
+-rw-r--r--   0        0        0       83 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/scripts/scripts/test_python.py
+-rw-r--r--   0        0        0      465 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/composition.nix
+-rw-r--r--   0        0        0      593 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.799006 nixos_compose-0.5.6/examples/setup/nxc.json
+-rw-r--r--   0        0        0     2917 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/setup/setup.toml
+-rw-r--r--   0        0        0      691 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/composition.nix
+-rw-r--r--   0        0        0      807 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/shared-directories-users/nxc.json
+-rw-r--r--   0        0        0      600 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/composition.nix
+-rw-r--r--   0        0        0      571 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/flake.nix
+-rw-r--r--   0        0        0       60 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/examples/webserver/nxc.json
+-rw-r--r--   0        0        0     1262 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/all-in-one.nix
+-rw-r--r--   0        0        0     4160 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/compose.nix
+-rw-r--r--   0        0        0     3246 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/generate_docker_compose.nix
+-rw-r--r--   0        0        0      569 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/generate_image.nix
+-rw-r--r--   0        0        0      816 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/nxc-shared-dirs-docker.nix
+-rw-r--r--   0        0        0      864 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/docker/systemd.nix
+-rw-r--r--   0        0        0      229 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours/docker.nix
+-rw-r--r--   0        0        0      731 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-image.nix
+-rw-r--r--   0        0        0     1966 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-nfs-store.nix
+-rw-r--r--   0        0        0      273 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/g5k-ramdisk.nix
+-rw-r--r--   0        0        0      533 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn/base.nix
+-rw-r--r--   0        0        0     1982 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn/generate_nspawn_compose.nix
+-rw-r--r--   0        0        0      469 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/nspawn.nix
+-rw-r--r--   0        0        0     1572 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base-hardware.nix
+-rw-r--r--   0        0        0     1595 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base-vm.nix
+-rw-r--r--   0        0        0      233 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/base.nix
+-rw-r--r--   0        0        0     5217 2024-03-24 20:19:40.908081 nixos_compose-0.5.6/nix/flavours/shared/common.nix
+-rw-r--r--   0        0        0     1081 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/g5k-common.nix
+-rw-r--r--   0        0        0     1034 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/g5k-ssh-host-keys.nix
+-rw-r--r--   0        0        0     3548 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/installation-device.nix
+-rw-r--r--   0        0        0     2164 2024-01-11 17:28:25.801006 nixos_compose-0.5.6/nix/flavours/shared/netboot.nix
+-rw-r--r--   0        0        0     1117 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/nxc-shared-dirs-nfs.nix
+-rw-r--r--   0        0        0     6708 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/nxc.nix
+-rw-r--r--   0        0        0     4183 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/ssh-keys.nix
+-rw-r--r--   0        0        0     6531 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/stage-1-cmds.nix
+-rw-r--r--   0        0        0     4044 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/shared/vm-stage-1-cmds.nix
+-rw-r--r--   0        0        0      435 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/vm-ramdisk.nix
+-rw-r--r--   0        0        0     1440 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours/vm.nix
+-rw-r--r--   0        0        0     1076 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours.json
+-rw-r--r--   0        0        0      321 2024-01-11 17:28:25.800006 nixos_compose-0.5.6/nix/flavours.nix
+-rw-r--r--   0        0        0      485 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/flavours2json.nix
+-rw-r--r--   0        0        0     1970 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/generate_one_composition_info.nix
+-rw-r--r--   0        0        0     1830 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/helpers.nix
+-rw-r--r--   0        0        0      421 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/lib.nix
+-rw-r--r--   0        0        0     1625 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/make-system-tarball.nix
+-rw-r--r--   0        0        0     1540 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/make-system-tarball.sh
+-rw-r--r--   0        0        0     6485 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/multiple_compositions.nix
+-rw-r--r--   0        0        0      989 2024-01-11 17:28:25.802006 nixos_compose-0.5.6/nix/nur.nix
+-rw-r--r--   0        0        0      973 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nix/one_composition.nix
+-rw-r--r--   0        0        0     7234 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nix/setup.nix
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/__init__.py
+-rw-r--r--   0        0        0    32412 2024-04-24 15:55:13.623282 nixos_compose-0.5.6/nixos_compose/actions.py
+-rw-r--r--   0        0        0     1851 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/cli.py
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/commands/__init__.py
+-rw-r--r--   0        0        0     9271 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_build.py
+-rw-r--r--   0        0        0      553 2024-01-11 17:28:25.803006 nixos_compose-0.5.6/nixos_compose/commands/cmd_clean.py
+-rw-r--r--   0        0        0     2800 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_connect.py
+-rw-r--r--   0        0        0     3455 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_driver.py
+-rw-r--r--   0        0        0     2646 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_helper.py
+-rw-r--r--   0        0        0     4974 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_init.py
+-rw-r--r--   0        0        0    15072 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/commands/cmd_start.py
+-rw-r--r--   0        0        0     1829 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/commands/cmd_stop.py
+-rw-r--r--   0        0        0     9518 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/context.py
+-rw-r--r--   0        0        0      391 2024-01-11 17:28:25.804006 nixos_compose-0.5.6/nixos_compose/default_role.py
+-rwxr-xr-x   0        0        0      522 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/__init__.py
+-rw-r--r--   0        0        0     5389 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/driver.py
+-rw-r--r--   0        0        0     3250 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/logger.py
+-rw-r--r--   0        0        0    31276 2024-01-11 17:28:25.805006 nixos_compose-0.5.6/nixos_compose/driver/machine.py
+-rw-r--r--   0        0        0     3424 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/driver/vlan.py
+-rw-r--r--   0        0        0      869 2024-03-24 20:20:27.989890 nixos_compose-0.5.6/nixos_compose/flavour.py
+-rw-r--r--   0        0        0     1606 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/__init__.py
+-rw-r--r--   0        0        0     9876 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/docker.py
+-rw-r--r--   0        0        0     8030 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/grid5000.py
+-rwxr-xr-x   0        0        0     1799 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/nspawn/machine-dir.sh
+-rwxr-xr-x   0        0        0     8836 2024-01-11 17:28:25.806006 nixos_compose-0.5.6/nixos_compose/flavours/nspawn/nxc-net.sh
+-rw-r--r--   0        0        0    11435 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/nspawn.py
+-rw-r--r--   0        0        0     7158 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/flavours/vm.py
+-rw-r--r--   0        0        0      602 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/g5k.py
+-rw-r--r--   0        0        0     2187 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/httpd.py
+-rw-r--r--   0        0        0     4273 2024-03-24 20:20:27.990890 nixos_compose-0.5.6/nixos_compose/nxc_execo.py
+-rw-r--r--   0        0        0     3747 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/platform.py
+-rw-r--r--   0        0        0     4033 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/setup.py
+-rw-r--r--   0        0        0      953 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/state.py
+-rw-r--r--   0        0        0        0 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/tools/__init__.py
+-rwxr-xr-x   0        0        0      248 2024-01-11 17:28:25.807006 nixos_compose-0.5.6/nixos_compose/tools/g5k_set_pub_key_sleep.sh
+-rwxr-xr-x   0        0        0     5009 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/tools/kataract.py
+-rw-r--r--   0        0        0     5916 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/tools/nested_deployment.py
+-rw-r--r--   0        0        0     2372 2024-01-11 17:28:25.808006 nixos_compose-0.5.6/nixos_compose/utils.py
+-rw-r--r--   0        0        0     1064 2024-04-24 17:51:32.404552 nixos_compose-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 nixos_compose-0.5.6/PKG-INFO
```

### Comparing `nixos_compose-0.5.5/LICENSE` & `nixos_compose-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/basic/flake.nix` & `nixos_compose-0.5.6/examples/webserver/flake.nix`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
-  description = "nixos-compose - basic setup";
+  description = "nixos-compose - basic webserver setup";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/basic-nur/flake.nix` & `nixos_compose-0.5.6/examples/basic-nur/flake.nix`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - basic setup with external NUR repo";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     NUR.url = "github:nix-community/NUR";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
     #inputs.alice.url = "path:/home/some_path/nur-alice";
   };
 
   outputs = { self, nixpkgs, NUR, nxc }:
     let
```

### Comparing `nixos_compose-0.5.5/examples/execo/execo_script.py` & `nixos_compose-0.5.6/examples/execo/execo_script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,94 @@
 from nixos_compose.nxc_execo import get_oar_job_nodes_nxc, build_nxc_execo
 
-from execo import Process, SshProcess, Remote
-from execo_g5k import oardel, oarsub, OarSubmission, get_oar_job_nodes
-from execo_engine import Engine, logger, ParamSweeper, sweep
+from execo import Remote  # ,Process, SshProcess
+from execo_g5k import oardel, oarsub, OarSubmission  # , get_oar_job_nodes
+from execo_engine import Engine  # , logger, ParamSweeper, sweep
 
-import sys
+# import sys
 import os
 
 
 class MyEngine(Engine):
     def __init__(self):
         super(MyEngine, self).__init__()
         parser = self.args_parser
-        parser.add_argument('--nxc_build_file', help='Path to the NXC deploy file')
-        parser.add_argument('--build', action='store_true', help='Either to build the composition')
-        parser.add_argument('--nxc_folder', default=f"{os.getcwd()}", help='Path to the nxc folder')
+        parser.add_argument("--nxc_build_file", help="Path to the NXC deploy file")
+        parser.add_argument(
+            "--build", action="store_true", help="Either to build the composition"
+        )
+        parser.add_argument(
+            "--nxc_folder", default=f"{os.getcwd()}", help="Path to the nxc folder"
+        )
         self.nodes = {}
         self.oar_job_id = -1
 
     def init(self):
         nb_nodes = 2
         site = "grenoble"
         cluster = "dahu"
 
         nxc_build_file = None
         if self.args.build:
-            (nxc_build_file, _time, _size) = build_nxc_execo(self.args.nxc_folder, site, cluster, walltime=15*60, extra_job_type=["day"])
+            (nxc_build_file, _time, _size) = build_nxc_execo(
+                self.args.nxc_folder,
+                site,
+                cluster,
+                walltime=15 * 60,
+                extra_job_type=["day"],
+            )
         elif self.args.nxc_build_file is not None:
             nxc_build_file = self.args.nxc_build_file
         else:
             raise Exception("No compose info file ...")
 
         print(nxc_build_file)
-        oar_job = reserve_nodes(nb_nodes, site, cluster, walltime=15*60)
+        oar_job = reserve_nodes(nb_nodes, site, cluster, walltime=15 * 60)
         self.oar_job_id, site = oar_job[0]
         roles_quantities = {"foo": ["foo", "bar"]}
-        self.nodes = get_oar_job_nodes_nxc(self.oar_job_id, site, compose_info_file=nxc_build_file, roles_quantities=roles_quantities)
+        self.nodes = get_oar_job_nodes_nxc(
+            self.oar_job_id,
+            site,
+            compose_info_file=nxc_build_file,
+            roles_quantities=roles_quantities,
+        )
         print(self.nodes)
 
     def run(self):
-        my_command = "echo \"Hello from $(whoami) at $(hostname) ($(ip -4 addr | grep \"/20\" | awk '{print $2;}'))\" > /tmp/hello"
-        hello_remote = Remote(my_command, self.nodes["foo"], connection_params={'user': 'root'})
+        my_command = 'echo "Hello from $(whoami) at $(hostname) ($(ip -4 addr | grep "/20" | awk \'{print $2;}\'))" > /tmp/hello'
+        hello_remote = Remote(
+            my_command, self.nodes["foo"], connection_params={"user": "root"}
+        )
         hello_remote.run()
 
         my_command2 = "cat /tmp/hello"
-        cat_remote = Remote(my_command2, self.nodes["foo"], connection_params={'user': 'root'})
+        cat_remote = Remote(
+            my_command2, self.nodes["foo"], connection_params={"user": "root"}
+        )
         cat_remote.run()
         for process in cat_remote.processes:
             print(process.stdout)
 
+
 def reserve_nodes(nb_nodes, site, cluster, walltime=3600):
-    jobs = oarsub([(OarSubmission("{{cluster='{}'}}/nodes={}".format(cluster, nb_nodes), walltime, job_type=["allow_classic_ssh", "day"]), site)])
+    jobs = oarsub(
+        [
+            (
+                OarSubmission(
+                    "{{cluster='{}'}}/nodes={}".format(cluster, nb_nodes),
+                    walltime,
+                    job_type=["allow_classic_ssh", "day"],
+                ),
+                site,
+            )
+        ]
+    )
     return jobs
 
+
 if __name__ == "__main__":
     ENGINE = MyEngine()
     try:
         ENGINE.start()
     except Exception as ex:
         print(f"Failing with error {ex}")
         oardel([(ENGINE.oar_job_id, None)])
```

### Comparing `nixos_compose-0.5.5/examples/execo/flake.nix` & `nixos_compose-0.5.6/examples/execo/flake.nix`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - basic setup";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
       pkgs = nixpkgs.legacyPackages.${system};
```

### Comparing `nixos_compose-0.5.5/examples/flake.lock` & `nixos_compose-0.5.6/examples/flake.lock`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/kernel/flake.nix` & `nixos_compose-0.5.6/examples/kernel/flake.nix`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - simple mutiple compositions";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/kernel/linux_ipanema_5_4.nix` & `nixos_compose-0.5.6/examples/kernel/linux_ipanema_5_4.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/multi-compositions/flake.nix` & `nixos_compose-0.5.6/examples/multi-compositions/flake.nix`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - simple mutiple compositions";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/nbp-mpi/composition.nix` & `nixos_compose-0.5.6/examples/nbp-mpi/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/nbp-mpi/flake.nix` & `nixos_compose-0.5.6/examples/nbp-mpi/flake.nix`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - ";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
     nxc.inputs.nixpkgs.follows = "nixpkgs";
     NUR.url = "github:nix-community/NUR";
     kapack.url = "github:oar-team/nur-kapack?ref=regale";
     kapack.inputs.nixpkgs.follows = "nixpkgs";
   };
```

### Comparing `nixos_compose-0.5.5/examples/nix_flake_templates.nix` & `nixos_compose-0.5.6/examples/nix_flake_templates.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/nixos-cluster/composition.nix` & `nixos_compose-0.5.6/examples/nixos-cluster/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/nixos-cluster/flake.nix` & `nixos_compose-0.5.6/examples/nixos-cluster/flake.nix`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - basic setup";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
       myOverlay = final: prev: {
```

### Comparing `nixos_compose-0.5.5/examples/nixos-cluster/ssh-keys.nix` & `nixos_compose-0.5.6/examples/nixos-cluster/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/scripts/flake.nix` & `nixos_compose-0.5.6/examples/scripts/flake.nix`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - scripts setup";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/setup/flake.nix` & `nixos_compose-0.5.6/examples/setup/flake.nix`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - setup feature";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/setup/setup.toml` & `nixos_compose-0.5.6/examples/setup/setup.toml`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/shared-directories-users/composition.nix` & `nixos_compose-0.5.6/examples/shared-directories-users/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/examples/shared-directories-users/flake.nix` & `nixos_compose-0.5.6/examples/shared-directories-users/flake.nix`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - ";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
     nxc.inputs.nixpkgs.follows = "nixpkgs";
     NUR.url = "github:nix-community/NUR";
     kapack.url = "github:oar-team/nur-kapack?ref=regale";
     kapack.inputs.nixpkgs.follows = "nixpkgs";
   };
```

### Comparing `nixos_compose-0.5.5/examples/spark/flake.nix` & `nixos_compose-0.5.6/examples/basic/flake.nix`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
   description = "nixos-compose - basic setup";
 
   inputs = {
-    nixpkgs.url = "github:NixOS/nixpkgs/22.05";
+    nixpkgs.url = "github:NixOS/nixpkgs/23.05";
     nxc.url = "git+https://gitlab.inria.fr/nixos-compose/nixos-compose.git";
   };
 
   outputs = { self, nixpkgs, nxc }:
     let
       system = "x86_64-linux";
     in {
```

### Comparing `nixos_compose-0.5.5/examples/webserver/composition.nix` & `nixos_compose-0.5.6/examples/webserver/composition.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/all-in-one.nix` & `nixos_compose-0.5.6/nix/all-in-one.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/compose.nix` & `nixos_compose-0.5.6/nix/compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/docker/generate_docker_compose.nix` & `nixos_compose-0.5.6/nix/flavours/docker/generate_docker_compose.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/docker/generate_image.nix` & `nixos_compose-0.5.6/nix/flavours/docker/generate_image.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/docker/nxc-shared-dirs-docker.nix` & `nixos_compose-0.5.6/nix/flavours/docker/nxc-shared-dirs-docker.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/docker/systemd.nix` & `nixos_compose-0.5.6/nix/flavours/docker/systemd.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/g5k-nfs-store.nix` & `nixos_compose-0.5.6/nix/flavours/g5k-nfs-store.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/base-hardware.nix` & `nixos_compose-0.5.6/nix/flavours/shared/base-hardware.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/base-vm.nix` & `nixos_compose-0.5.6/nix/flavours/shared/base-vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/common.nix` & `nixos_compose-0.5.6/nix/flavours/shared/common.nix`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   boot.kernelModules = [ "kvm-intel" ];
 
   users.users.root.password = "nixos";
 
   networking.firewall.enable = false;
 
   services.sshd.enable = true;
-  systemd.services.sshd.wantedBy = mkForce [ "multi-user.target" ];
+
   networking.hostName = mkDefault "";
 
   services.getty.autologinUser = mkDefault "root";
 
   security.polkit.enable = false; # to reduce initrd
   services.udisks2.enable = false; # to reduce initrd
 
@@ -140,13 +140,11 @@
       '';
     } else "Disable_for_space_saving";
   };
 
   # misc
   key = "no-manual";
 
-  environment.noXlibs = mkDefault true;
-
   documentation.enable = mkDefault false;
 
   documentation.nixos.enable = mkDefault false;
 }
```

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/g5k-common.nix` & `nixos_compose-0.5.6/nix/flavours/shared/g5k-common.nix`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ./nxc.nix
     ./g5k-ssh-host-keys.nix
     ./nxc-shared-dirs-nfs.nix
   ];
 
   boot.initrd.availableKernelModules =
     [ "ahci" "ehci_pci" "megaraid_sas" "sd_mod" ];
+
   boot.kernelModules = [ "kvm-intel" ];
 
   # Kadeploy tests some ports' accessibility to follow deployment steps
   networking.firewall.enable = false;
   boot.supportedFilesystems = [ "nfs" ];
   nxc.wait-online.enable = true;
```

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/g5k-ssh-host-keys.nix` & `nixos_compose-0.5.6/nix/flavours/shared/g5k-ssh-host-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/installation-device.nix` & `nixos_compose-0.5.6/nix/flavours/shared/installation-device.nix`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     # We run sshd by default. Login via root is only possible after adding a
     # password via "passwd" or by adding a ssh key to /home/nixos/.ssh/authorized_keys.
     # The latter one is particular useful if keys are manually added to
     # installation device for head-less systems i.e. arm boards by manually
     # mounting the storage in a different system.
     services.openssh = {
       enable = true;
-      permitRootLogin = "yes";
+      settings.PermitRootLogin = "yes";
+      startWhenNeeded = false;
     };
 
     # Enable wpa_supplicant, but don't start it by default.
     #networking.wireless.enable = mkDefault true;
     #systemd.services.wpa_supplicant.wantedBy = mkOverride 50 [];
 
     # Tell the Nix evaluator to garbage collect more aggressively.
```

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/netboot.nix` & `nixos_compose-0.5.6/nix/flavours/shared/netboot.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/nxc-shared-dirs-nfs.nix` & `nixos_compose-0.5.6/nix/flavours/shared/nxc-shared-dirs-nfs.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/nxc.nix` & `nixos_compose-0.5.6/nix/flavours/shared/nxc.nix`

 * *Files 2% similar despite different names*

```diff
@@ -116,24 +116,24 @@
         sleep .2
         done
         '';
       };
     })
     (mkIf cfg.baseBootCommands.enable {
       boot.postBootCommands = ''
-       for o in $(cat /proc/cmdline); do
+        for o in $(cat /proc/cmdline); do
           case $o in
                ip=*)
                    set -- $(IFS==; echo $o)
                    set -- $(IFS=:; echo $2)
                    ip_addr="$1"
                    ${pkgs.iproute2}/bin/ip addr add $1/24 dev eth1
                    ;;
            esac
-       done
+        done
 
         ln -s /run/current-system/sw/bin/bash /bin/bash
         compositionName=""
         if [[ -f /etc/nxc-composition ]]; then
           compositionName=$(cat /etc/nxc-composition)
         fi
         echo "composition name: $compositionName"
@@ -184,24 +184,26 @@
         fi
 
         if [[ -f "$nix_path_registration"-"$compositionName"-"$role" ]]; then
           nix_path_registration="$nix_path_registration"-"$compositionName"-"$role"
         fi
 
         echo "nix-store: load db $nix_path_registration"
-        ${config.nix.package}/bin/nix-store --load-db < $nix_path_registration
+        #${config.nix.package}/bin/nix-store --load-db < $nix_path_registration
 
         #echo "inetutils"
         #echo ${pkgs.inetutils}/bin
         #exec /bin/bash
 
         # nixos-rebuild also requires a "system" profile and an
         # /etc/NIXOS tag.
         touch /etc/NIXOS
-        ${config.nix.package}/bin/nix-env -p /nix/var/nix/profiles/system --set /run/current-system
+        # TODO can we remove it ?
+        #${config.nix.package}/bin/nix-env -p /nix/var/nix/profiles/system --set /run/current-system
+
         ${
           if cfg.sharedDirsBootCommands != "" then
             cfg.sharedDirsBootCommands
           else
             ""
         }
         ${
```

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/ssh-keys.nix` & `nixos_compose-0.5.6/nix/flavours/shared/ssh-keys.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/stage-1-cmds.nix` & `nixos_compose-0.5.6/nix/flavours/shared/stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/shared/vm-stage-1-cmds.nix` & `nixos_compose-0.5.6/nix/flavours/shared/vm-stage-1-cmds.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours/vm.nix` & `nixos_compose-0.5.6/nix/flavours/vm.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/flavours.json` & `nixos_compose-0.5.6/nix/flavours.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'nspawn'": "OrderedDict([('description', 'Systemd-nspawn'), ('image', OrderedDict()), ('name', "*

 * *             "'nspawn')])"}*

```diff
@@ -24,14 +24,19 @@
         "description": "Flavour for Grid'5000 platform",
         "image": {
             "distribution": "all-in-one",
             "type": "ramdisk"
         },
         "name": "g5k-ramdisk"
     },
+    "nspawn": {
+        "description": "Systemd-nspawn",
+        "image": {},
+        "name": "nspawn"
+    },
     "vm": {
         "description": "vm ",
         "image": {
             "distribution": "all-in-one"
         },
         "name": "vm"
     },
```

### Comparing `nixos_compose-0.5.5/nix/generate_one_composition_info.nix` & `nixos_compose-0.5.6/nix/generate_one_composition_info.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/helpers.nix` & `nixos_compose-0.5.6/nix/helpers.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/make-system-tarball.nix` & `nixos_compose-0.5.6/nix/make-system-tarball.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/make-system-tarball.sh` & `nixos_compose-0.5.6/nix/make-system-tarball.sh`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/multiple_compositions.nix` & `nixos_compose-0.5.6/nix/multiple_compositions.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/nur.nix` & `nixos_compose-0.5.6/nix/nur.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nix/one_composition.nix` & `nixos_compose-0.5.6/nix/one_composition.nix`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 { nixpkgs, system, setup, nur, flavour, helpers, composition
 , composition_name ? "composition", overlays, extraConfigurations }:
 let
   multiple_compositions = import ./multiple_compositions.nix;
   generate_docker_compose =
     import ./flavours/docker/generate_docker_compose.nix;
+  generate_nspawn_compose =
+    import ./flavours/nspawn/generate_nspawn_compose.nix;
   commonArguments = {
     inherit nixpkgs system overlays setup nur helpers extraConfigurations;
     flavour = flavour;
   };
   argumentsModule = commonArguments // {
     extraConfigurations = extraConfigurations ++ [ flavour.module ];
   };
   argumentsFlavourMulti = commonArguments // {
     inherit flavour;
     compositions = { ${composition_name} = composition; };
   };
 in if flavour.name == "docker" then
   generate_docker_compose argumentsModule composition
+else if flavour.name == "nspawn" then
+  generate_nspawn_compose argumentsModule composition
 else
   multiple_compositions argumentsFlavourMulti
```

### Comparing `nixos_compose-0.5.5/nix/setup.nix` & `nixos_compose-0.5.6/nix/setup.nix`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/actions.py` & `nixos_compose-0.5.6/nixos_compose/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,38 +99,47 @@
 
 
 def read_deployment_info(ctx, deployment_file=None):
     ctx.deployment_filename = get_deployment_file(ctx, deployment_file)
     with open(ctx.deployment_filename, "r") as f:
         deployment_info = json.load(f)
     ctx.deployment_info = deployment_info
+    if "composition" in deployment_info:
+        composition_name = deployment_info["composition"]
+        if not ctx.composition_name:
+            ctx.composition_name = composition_name
+        elif ctx.composition_name != composition_name:
+            ctx.wlog(
+                "Composition from built ({ctx.composition_name}) is different from deployment ({composition_name})"
+            )
     return
 
 
 def read_deployment_info_str(ctx, deployment_file=None):
     ctx.deployment_filename = get_deployment_file(ctx, deployment_file)
     with open(ctx.deployment_filename, "r") as f:
         deployment_info_str = f.read()
     return deployment_info_str
 
 
 def read_test_script(ctx, compose_info_or_str):
+    if not compose_info_or_str:
+        return None
     if isinstance(compose_info_or_str, str):
         filename = compose_info_or_str
     elif "test_script" in compose_info_or_str:
         filename = compose_info_or_str["test_script"]
     else:
         return None
     with open(realpath_from_store(ctx, filename), "r") as f:
         test_script = f.read()
         return test_script
 
 
 def read_compose_info(ctx):
-
     if not op.isfile(ctx.compose_info_file):
         raise click.ClickException(f"{ctx.compose_info_filename} does not exist")
     with open(ctx.compose_info_file, "r") as f:
         compose_info = json.load(f)
 
     if "compositions_info" in compose_info:
         ctx.compositions_info = compose_info
@@ -209,30 +218,36 @@
             }
             i = i + 1
 
     return deployment, ips
 
 
 def health_check_roles_distribution(ctx, roles_info, roles_distribution_in, ips=None):
-
     roles_distribution = {}
+    # if isinstance(roles_info, list):
+    #     roles = roles_info
+    # else:
+    #     roles = roles_info.keys()
     for role in roles_info.keys():
         if role in roles_distribution_in:
             roles_distribution[role] = roles_distribution_in[role]
         elif (
             "roles_distribution" in ctx.compose_info
             and role in ctx.compose_info["roles_distribution"]
         ):
             hosts = ctx.compose_info["roles_distribution"][role]
-            if type(hosts) != list:
-                try:
-                    quantity = int(hosts)
-                    hosts = [f"{role}{i}" for i in range(1, quantity + 1)]
-                except ValueError:
-                    pass
+            if isinstance(hosts, int):
+                hosts = [f"{role}{i}" for i in range(1, hosts + 1)]
+            # TODO REMOVE after test
+            # if isinstance(hosts, list):
+            #     try:
+            #         quantity = int(hosts)
+            #         hosts = [f"{role}{i}" for i in range(1, quantity + 1)]
+            #     except ValueError:
+            #         pass
             roles_distribution[role] = hosts
         else:
             roles_distribution[role] = [role]
 
     # TODO
     # - if ips is present and ips number lower than host number
     # - if ips is present and ips number greater than host number
@@ -322,15 +337,19 @@
             exit(1)
         for hostname in roles_distribution[role]:
             try:
                 ip = ips[i]
             except IndexError as e:
                 ctx.elog(f"Not enough nodes are available for the deployment: {e}")
                 exit(1)
-            deployment[ip] = {"role": role, "host": hostname, "init": v["init"]}
+            # TODO Ugly need core refactoring to remove it
+            if hasattr(ctx.flavour, "host_info"):
+                deployment[ip] = ctx.flavour.host_info(role, hostname, v)
+            else:
+                deployment[ip] = {"role": role, "host": hostname, "init": v["init"]}
             i = i + 1
     return deployment
 
 
 def generate_deployment_info(ctx, ssh_pub_key_file=None):
     if not ctx.compose_info:
         read_compose_info(ctx)
@@ -355,14 +374,15 @@
                 "role": v["role"],
                 "host": v["host"],
                 "vm_id": v["vm_id"],
                 "init": v["init"] if "host" in v else v["role"],
             }
             for k, v in deployment.items()
         }
+
     deployment = {
         "ssh_key.pub": sshkey_pub,
         "deployment": deployment,
     }
 
     if "all" in ctx.compose_info:
         deployment["all"] = ctx.compose_info["all"]
@@ -398,15 +418,19 @@
 
     ctx.deployment_filename = op.join(
         deploy_dir, f"{ctx.composition_flavour_prefix}.json"
     )
     with open(ctx.deployment_filename, "w") as outfile:
         outfile.write(json_deployment)
 
+    if "parameters" in ctx.deployment_info:
+        deployment["parameters"] = ctx.deployment_info["parameters"]
+
     ctx.deployment_info = deployment
+
     return
 
 
 def generate_kexec_scripts(ctx, flavour_kernel_params=""):
     if ctx.use_httpd:
         base_url = f"http://{ctx.httpd.ip}:{ctx.httpd.port}"
         deploy_info_src = f"{base_url}/deploy/{ctx.composition_flavour_prefix}.json"
@@ -425,15 +449,15 @@
         kernel_params = ctx.kernel_params
 
     if "all" in ctx.deployment_info:
         kernel_path = realpath_from_store(ctx, ctx.deployment_info["all"]["kernel"])
         initrd_path = realpath_from_store(ctx, ctx.deployment_info["all"]["initrd"])
 
         kexec_args = "-l $KERNEL --initrd=$INITRD "
-        kexec_args += fr'--append="deploy={deploy_info_src} console=tty0 console=ttyS0,115200 {flavour_kernel_params} {kernel_params}"'
+        kexec_args += rf'--append="deploy={deploy_info_src} console=tty0 console=ttyS0,115200 {flavour_kernel_params} {kernel_params}"'
         script_path = op.join(kexec_scripts_path, "kexec.sh")
         with open(script_path, "w") as kexec_script:
             kexec_script.write("#!/usr/bin/env bash\n")
             kexec_script.write(": ${KERNEL:=" + kernel_path + "}\n")
             kexec_script.write(": ${INITRD:=" + initrd_path + "}\n")
             kexec_script.write(f"kexec {kexec_args}\n")
             kexec_script.write("kexec -e\n")
@@ -441,26 +465,25 @@
     else:
         for ip, v in ctx.deployment_info["deployment"].items():
             role = v["role"]
             kernel_path = f"{base_path}/kernel_{role}"
             initrd_path = f"{base_path}/initrd_{role}"
             init_path = v["init"]
             kexec_args = f"-l {kernel_path} --initrd={initrd_path} "
-            kexec_args += fr'--append="init={init_path} deploy={deploy_info_src} console=tty0 console=ttyS0,115200 {flavour_kernel_params} {kernel_params}"'
+            kexec_args += rf'--append="init={init_path} deploy={deploy_info_src} console=tty0 console=ttyS0,115200 {flavour_kernel_params} {kernel_params}"'
             script_path = op.join(kexec_scripts_path, f"kexec_{role}.sh")
             with open(script_path, "w") as kexec_script:
                 kexec_script.write("#!/usr/bin/env bash\n")
                 kexec_script.write(f"kexec {kexec_args}\n")
                 kexec_script.write("kexec -e\n")
 
             os.chmod(script_path, 0o755)
 
 
 def generate_deploy_info_b64(ctx):
-
     deployment_info = {
         k: ctx.deployment_info[k]
         for k in [n for n in ctx.deployment_info.keys() if n != "deployment"]
     }
 
     deployment = {
         k: {"role": v["role"], "host": v["host"] if "host" in v else v["role"]}
@@ -545,15 +568,14 @@
 
 ##
 #  Operation: connect, launch, wait_ssh_port,
 #
 
 
 def launch_ssh_kexec(ctx, ip=None, debug=False):
-
     if ctx.show_spinner:
         ctx.spinner.start("Launching remote kexec(s)")
     else:
         ctx.log("Launching remote kexec(s)")
 
     if "all" in ctx.deployment_info:
         if ctx.push_path:
@@ -690,42 +712,55 @@
             if "vm_id" in v:
                 ip = "127.0.0.1"
                 ssh_port = 22021 + int(v["vm_id"])
             break
     return (ip, ssh_port)
 
 
-def ssh_connect(ctx, user, host, execute=True):
+def ssh_connect(ctx, user, host, execute=True, ssh_key_file=None):
     ip, ssh_port = get_ip_ssh_port(ctx, host)
-    ssh_cmd = f"ssh -o StrictHostKeyChecking=no -o LogLevel=ERROR -l {user} -p {ssh_port} {ip}"
+    ssh_key_option = (
+        ""
+        if ssh_key_file is None
+        else "-o IdentitiesOnly=yes -i " + os.path.realpath(ssh_key_file)
+    )
+
+    ssh_cmd = (
+        f"ssh {ssh_key_option} -o StrictHostKeyChecking=no -o LogLevel=ERROR"
+        f" -l {user} -p {ssh_port} {ip}"
+    )
 
     if execute:
         return_code = subprocess.run(ssh_cmd, shell=True).returncode
 
         if return_code:
             ctx.wlog(f"SSH exit code is not null: {return_code}")
         sys.exit(return_code)
     else:
         return ssh_cmd
 
 
 NB_PANES_2_GEOMETRY = ["1", "1+1", "1+2", "2+2", "2+3", "3+3", "3+4", "4+4"]
 
 
-def connect_tmux(ctx, user, nodes, pane_console, geometry, window_name="nxc"):
+def connect_tmux(
+    ctx, user, nodes, ssh_key_file, pane_console, geometry, window_name="nxc"
+):
     if not nodes:
         deploy = ctx.deployment_info["deployment"]
         node = (list(deploy.keys()))[0]
         try:
             ipaddress.ip_address(node)
             nodes = [v["host"] for v in deploy.values()]
         except ValueError:
             nodes = list(deploy.keys())
 
-    ssh_cmds = [ctx.flavour.ext_connect(user, node, execute=False) for node in nodes]
+    connect_cmds = [
+        ctx.flavour.ext_connect(user, node, False, ssh_key_file) for node in nodes
+    ]
 
     console = 0
     if pane_console:
         console = 1
 
     if not geometry:
         geometry = ""
@@ -752,18 +787,18 @@
     ctx.vlog(f"geometry: {geometry}")
     ctx.vlog(f"splitw: {splitw}")
     ctx.vlog(f"nb_panes: {nb_panes}")
 
     # prepare commands
     base_cmds = ["bash" for i in range(nb_panes)]
 
-    nb_ssh_cmds = len(ssh_cmds)
-    if (nb_ssh_cmds + console) > nb_panes:
-        ssh_cmds = ssh_cmds[: nb_panes - console]
-    cmds = base_cmds[: nb_panes - nb_ssh_cmds] + ssh_cmds
+    nb_connect_cmds = len(connect_cmds)
+    if (nb_connect_cmds + console) > nb_panes:
+        connect_cmds = connect_cmds[: nb_panes - console]
+    cmds = base_cmds[: nb_panes - nb_connect_cmds] + connect_cmds
 
     ctx.vlog(f"cmds: {cmds}")
 
     cmds.reverse()
 
     if "TMUX" not in os.environ:
         cmd = "tmux new -d"
@@ -851,31 +886,39 @@
     nix_cmd += ["--extra-experimental-features", "nix-command flakes"]
     return nix_cmd
 
 
 # get Nix-static
 def install_nix_static(
     ctx,
-    version="2.10.3",
     archi="x86_64",
     local_bin_path=f"{os.environ['HOME']}/.local/bin",
 ):
     if ctx.show_spinner:
         ctx.spinner.start("Installing Nix")
     else:
         ctx.log("Installing Nix...")
 
     if not op.exists(local_bin_path):
         os.makedirs(local_bin_path)
     nix_path = op.join(local_bin_path, "nix")
 
-    urllib.request.urlretrieve(
-        f"https://gitlab.inria.fr/nixos-compose/nix-static/-/raw/main/bin/nix-{version}-{archi}-unknown-linux-musl",
-        nix_path,
-    )
+    remote_nix_filename = ""
+    with urllib.request.urlopen(
+        f"https://gitlab.inria.fr/nixos-compose/nix-static/-/raw/main/bin/nix-{archi}-linux-static"
+    ) as response:
+        remote_nix_filename = response.read().decode("utf-8")
+
+    ctx.log(f"Retrieving... {remote_nix_filename}")
+
+    with urllib.request.urlopen(
+        f"https://gitlab.inria.fr/nixos-compose/nix-static/-/raw/main/bin/{remote_nix_filename}"
+    ) as response:
+        with open(nix_path, "wb") as output_file:
+            shutil.copyfileobj(response, output_file)
 
     os.chmod(nix_path, 0o755)
 
     # create store directory to satisfy autodetection in build phase
     os.makedirs(f"{os.environ['HOME']}/.local/share/nix/root/nix/store")
 
     if ctx.show_spinner:
```

### Comparing `nixos_compose-0.5.5/nixos_compose/cli.py` & `nixos_compose-0.5.6/nixos_compose/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     default=op.abspath("./nxc"),
     help="Changes the folder to operate on.",
 )
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Verbose mode.")
 @click.option("--debug", "-D", is_flag=True, default=False, help="Enable debugging")
 @click.version_option(version=version)
 @pass_context
-def cli(ctx, envdir, verbose, debug):
-    """Generate and manage multi Nixos composition."""
+def nxc(ctx, envdir, verbose, debug):
+    """Generate and manage Nixos-compositions."""
     ctx.envdir = envdir
     if os.path.isfile("nxc.json"):
         if os.path.islink("nxc.json"):
             ctx.nxc_file = op.abspath(os.readlink("nxc.json"))
         else:
             ctx.nxc_file = op.abspath("nxc.json")
         with open(ctx.nxc_file, "r") as f:
@@ -53,9 +53,9 @@
         ctx.envdir = op.dirname(ctx.nxc_file)
 
     ctx.verbose = verbose
     ctx.debug = debug
     # ctx.update() not use
 
 
-def main(args=sys.argv[1:]):
-    cli(args)
+def main():
+    nxc()
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_build.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,24 @@
 @click.option(
     "--nix-flags",
     type=click.STRING,
     help='add nix flags (aka options) to nix build command, --nix-flags "--impure"',
 )
 @click.option("--out-link", "-o", help="path of the symlink to the build result")
 @click.option(
-    "-f", "--flavour", type=click.STRING, help="Use particular flavour (name or path)",
+    "-f",
+    "--flavour",
+    type=click.STRING,
+    help="Use particular flavour (name or path)",
 )
 @click.option(
-    "-F", "--list-flavours", is_flag=True, help="List available flavour",
+    "-F",
+    "--list-flavours",
+    is_flag=True,
+    help="List available flavour",
 )
 # TOREMOVE
 # @click.option(
 #    "--copy-from-store",
 #    "-c",
 #    is_flag=True,
 #    help="Copy artifacts (initrd, kernels, ...) from Nix store to artifact directory",
@@ -46,28 +52,27 @@
     is_flag=True,
     help="Eval build expression and show store entry without building derivation",
 )
 @click.option(
     "-C",
     "--composition-flavour",
     type=click.STRING,
-    help="Use to specify which composition and flavour combinaison to build when muliple compostions are describe at once (see -L options to list them).",
+    help="Use to specify which composition and flavour combination to build when multiple compositions are describe at once (see -L options to list them).",
 )
-# @click.option(
-#    "-c", "--composition", type=click.STRING,
-#    help="Use to specify which composition to built when muliple compostions are describe at once."
-# )
 @click.option(
     "-L",
     "--list-compositions-flavours",
     is_flag=True,
-    help="List available combinaisons of compositions and flavours",
+    help="List available combinations of compositions and flavours",
 )
 @click.option(
-    "-s", "--setup", type=click.STRING, help="Select setup variant",
+    "-s",
+    "--setup",
+    type=click.STRING,
+    help="Select setup variant",
 )
 @click.option(
     "-p",
     "--setup-param",
     type=click.STRING,
     multiple=True,
     help="Override setup parameter",
@@ -99,17 +104,28 @@
     composition_flavour,
     list_compositions_flavours,
     update_flake,
     setup,
     setup_param,
     monitor,
 ):
-    """Build multi Nixos composition.
-    Typically it performs the kind of following command:
-      nix build
+    """
+    Builds the composition.
+
+    It generates a `build` folder which stores symlinks to the closure associated to a composition. The file name of the symlink follows this structure  `[composition-name]::[flavour]`
+
+    ## Examples
+
+    - `nxc build -t vm`
+
+        Build the `vm` flavor of your composition.
+
+    - `nxc build -C oar::g5k-nfs-store`
+
+        Build the `oar` composition with the `g5k-nfs-store` flavor.
     """
 
     def determine_flavour(ctx):
         if "default_flavour" in ctx.nxc and ctx.nxc["default_flavour"]:
             flavour = ctx.nxc["default_flavour"]
         else:
             platform_detection(ctx)
@@ -171,19 +187,14 @@
 
     if list_flavours:
         ctx.log("Flavours List:")
         for k in flavours:
             click.echo(f"{k: <18}: {description_flavours[k]['description']}")
         sys.exit(0)
 
-    # if flavour:
-    #    if flavour not in flavours and not op.isfile(flavour):
-    #        ctx.elog(f'"{flavour}" is neither a supported flavour nor flavour_path')
-    # w        sys.exit(1)
-
     if not composition_file:
         composition_file = ctx.nxc["composition"]
 
     if list_compositions_flavours:
         cmd = nix_cmd_base + ["flake", "show", "--json"]
         raw_compositions_flavours = json.loads(
             subprocess.check_output(cmd, cwd=ctx.envdir).decode()
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_clean.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_connect.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_stop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 import click
-import re
-from ..context import pass_context  # , on_started, on_finished
-from ..actions import read_deployment_info, connect_tmux
+import os
+import os.path as op
+import glob
+
+from ..context import pass_context
+from ..actions import read_deployment_info
 from ..flavours import get_flavour_by_name
 
 
-@click.command("connect")
-@click.option("-l", "--user", default="root")
+@click.command("stop")
 @click.option(
-    "-g",
-    "--geometry",
-    help='Tmux geometry, 2 splitting indications are supported: +/*, examples: "1+3+2" (3 adjacent panes respectively horizontally splited by 1,3 and 2), "2*3" (2 adjacent panes horizontally splitted by 3)',
+    "-f",
+    "--flavour",
+    type=click.STRING,
+    help="specify flavour",
 )
 @click.option(
     "-d",
     "--deployment-file",
-    help="Deployment file, take the latest created in deploy directory by default",
+    type=click.STRING,
+    help="specify deployment",
 )
-@click.option(
-    "-f",
-    "--flavour",
-    help="flavour, by default it's extracted from deployment file name",
-)
-@click.option("-pc", "--pane-console", is_flag=True, help="Add a pane console")
-@click.argument("host", nargs=-1)
 @pass_context
-# TODO @on_finished(lambda ctx: ctx.state.dump())
-# TODO @on_started(lambda ctx: ctx.assert_valid_env())
-def cli(ctx, user, host, geometry, pane_console, deployment_file, flavour):
-    """Connect to host."""
-    read_deployment_info(ctx, deployment_file)
+def cli(ctx, flavour, deployment_file):
+    """Stop Nixos composition."""
+    ctx.log("Stopping")
+
+    flavour_name = flavour
 
-    # determine flavour name
-    if not flavour:
-        match = re.match(r"^.*::(.+)\..*$", ctx.deployment_filename)
-        if match:
-            flavour = match.group(1)
+    deploy_path = op.join(ctx.envdir, "deploy")
+
+    if not deployment_file:
+        if flavour_name:
+            search_path = f"{deploy_path}/*::{flavour_name}.json"
         else:
-            raise click.ClickException(
-                "Cannot determined flavour, one must by provided (option fix deployment file name or use --flavour option"
-            )
-
-    ctx.flavour = get_flavour_by_name(flavour)(ctx)
-
-    if not host or len(host) > 1:
-        # TODO  add wait_ssh
-        connect_tmux(ctx, user, host, pane_console, geometry, "nxc")
+            search_path = f"{deploy_path}/*"
+
+        deploy_paths = glob.glob(search_path)
+        if not deploy_paths:
+            raise click.ClickException("Failed to find last deployment file")
+
+        last_deploy_path = max(
+            deploy_paths,
+            key=lambda x: os.stat(x, follow_symlinks=False).st_ctime,
+        )
+
+        deployment_file = last_deploy_path
+        ctx.log("Use last deployment file:")
+        ctx.glog(deployment_file)
+
+        # ctx.composition_flavour_prefix = op.basename(last_deploy_path)
+
+    splitted_filename = deployment_file.split("::")
+
+    if len(splitted_filename) != 2:
+        raise click.ClickException("Sorry, filename is malformed")
+
+    splitted_last = splitted_filename[-1].split(".")
+    if splitted_last[-1] != "json":
+        raise click.ClickException("Sorry, filename is malformed")
+
+    if flavour_name:
+        assert flavour_name == splitted_last[0]
     else:
-        ctx.flavour.ext_connect(user, host[0])
+        flavour_name = splitted_last[0]
+
+    ctx.flavour = get_flavour_by_name(flavour_name)(ctx)
+
+    read_deployment_info(ctx, deployment_file)
 
-        # if "docker-compose-file" in ctx.deployment_info:
-        #    connect_docker(ctx, user, host[0])
-        # else:
-        #    connect(ctx, user, host[0])
+    ctx.flavour.cleanup()
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_driver.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,38 @@
 )
 @click.option(
     "-f",
     "--flavour",
     help="flavour, by default it's extracted from deployment file name",
 )
 @click.option(
-    "-t", "--test-script", is_flag=True, help="execute the 'embedded' testscript",
+    "-t",
+    "--test-script",
+    is_flag=True,
+    help="execute the 'embedded' testScript",
 )
 @click.argument("test-script-file", required=False)
 @pass_context
 # TODO @on_finished(lambda ctx: ctx.state.dump())
 # TODO @on_started(lambda ctx: ctx.assert_valid_env())
 def cli(ctx, user, deployment_file, flavour, test_script_file, test_script):
-    """Start driver to intearct with deployed environment."""
+    """
+    Run the driver to execute the given script to interact with the deployed environment.
+    The script is a python script similar to nixos-test script. See the [NixOS manual on nixos-tests](https://nixos.org/manual/nixos/unstable/#sec-writing-nixos-tests) for more details.
+
+    ```admonish warning
+    Be aware that unlike Nixos-test that only support virtual machines, `nxc` supports many flavors and VM specific features are not supported.
+    ```
+
+    ## Examples
+
+    - `nxc driver -t`
+
+       Run the script defined in the composition
+    """
     read_deployment_info(ctx, deployment_file)
 
     # determine flavour name
     if not flavour:
         match = re.match(r"^.*::(.+)\..*$", ctx.deployment_filename)
         if match:
             flavour = match.group(1)
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_helper.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 import sys
 import socket
 from ..context import pass_context
 from ..g5k import key_sleep_script, g5k_get_seed_store
 from ..actions import install_nix_static, get_ip_ssh_port
+from ..tools.nested_deployment import main as nested
 
 
 def print_helper(ctx, options):
     option = options[0]
     if (option == "g5k_script") or (option == "g5k-script"):
         click.echo(key_sleep_script)
     elif option == "install-nix":
@@ -32,14 +33,17 @@
             fqdn = socket.getfqdn(ip)
             print(f"{fqdn}")
     elif option == "g5k-get-seed-store":
         if len(options) > 1:
             g5k_get_seed_store(ctx, options[1])
         else:
             g5k_get_seed_store(ctx)
+    elif option == "nested":
+        nested(options[1:])
+
     else:
         ctx.elog(f"Helper: {option} does not exist")
         sys.exit(1)
 
 
 def print_helper_list(helper_options):
     print("g5k-script: print path to g5k_key_sleep_script Grid'5000 script")
@@ -47,29 +51,33 @@
     print(
         "g5k-get-seed-store: get an initial store default url: http://public.grenoble.grid5000.fr/~orichard/seed-nix-store.tgz"
     )
     print("ip <composition_hostname>: print hostname's ip address")
     print(
         "ip_ssh_port <composition_hostname>: print hostname's ip address and ssh port"
     )
-    print("fqdn <composition_hostname>: print hostname's fully qualified domain name ")
+    print("fqdn <composition_hostname>: print hostname's fully qualified domain name")
+    print(
+        "nested [options]: various file generation for nested deployement (-h for options details"
+    )
 
 
 @click.command("helper")
 @click.option(
     "-l",
     "--list",
     # "--list-helpers",
     is_flag=True,
     help="List of available helpers",
 )
 @pass_context
 @click.argument("options", nargs=-1)
 def cli(ctx, options, list):
     """Specific and contextual helper information (e.g. g5k_script path for Grid'5000)
-    Warning: Experimental command, may be removed in the future or change without backward compatibility care."""
+    Warning: Experimental command, may be removed in the future or change without backward compatibility care.
+    """
 
     if options:
         print_helper(ctx, options)
 
     if list:
         print_helper_list(ctx)
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_init.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,25 @@
 )
 @click.option(
     "--list-flavours-json",
     is_flag=True,
     help="List description of flavours, in json format",
 )
 @click.option(
-    "-F", "--list-flavours", is_flag=True, help="List available flavour",
+    "-F",
+    "--list-flavours",
+    is_flag=True,
+    help="List available flavour",
 )
 @click.option(
-    "-t", "--template", default="basic", help="Use a template", show_default=True,
+    "-t",
+    "--template",
+    default="basic",
+    help="Use a template",
+    show_default=True,
 )
 @click.option(
     "--use-local-templates",
     is_flag=True,
     default=False,
     help="Either use the local templates or not",
 )
```

### Comparing `nixos_compose-0.5.5/nixos_compose/commands/cmd_start.py` & `nixos_compose-0.5.6/nixos_compose/commands/cmd_start.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,63 +5,118 @@
 
 import os.path as op
 
 import sys
 import glob
 import pyinotify
 import asyncio
+import ast
+import json
 
 import ptpython.repl
 
 from ..context import pass_context, on_finished, on_started
 from ..flavours import get_flavour_by_name
 
 from ..actions import (
+    read_deployment_info,
     read_test_script,
     read_hosts,
     translate_hosts2ip,
     push_on_machines,
     realpath_from_store,
     get_fs_type,
 )
 
 from ..driver.driver import Driver
 from ..httpd import HTTPDaemon
 from ..setup import apply_setup
 
-machines_file_towait = ""
+machine_file_towait = ""
 notifier = None
 
 
 class EventHandler(pyinotify.ProcessEvent):
     def process_IN_CREATE(self, event):
-        if event.pathname == machines_file_towait:
+        if event.pathname == machine_file_towait:
             notifier.loop.stop()
 
 
+def start(ctx, interactive, execute_test_script, port, machine_file=None):
+    if (  # TODO rework (ask flavour ?)
+        ctx.ip_addresses
+        and (ctx.flavour.name != "vm-ramdisk")
+        and (ctx.flavour.name != "vm")
+    ) or ctx.flavour.name == "nspawn":
+        if ctx.use_httpd:
+            ctx.vlog("Launch: httpd to distribute deployment.json")
+            ctx.httpd = HTTPDaemon(ctx=ctx, port=port)
+
+        if hasattr(ctx.flavour, "generate_kexec_scripts"):
+            ctx.flavour.generate_kexec_scripts()
+
+        if ctx.push_path:
+            push_on_machines(ctx)
+
+        if ctx.use_httpd:
+            ctx.httpd.start(directory=ctx.envdir)
+
+        if not interactive:
+            ctx.flavour.launch(machine_file=machine_file)
+            sys.exit(0)
+
+    test_script = read_test_script(ctx, ctx.compose_info)
+
+    if not interactive and not execute_test_script:
+        test_script = "start_all()"
+
+    with Driver(
+        # args.start_scripts, args.vlans, args.testscript.read_text(), args.keep_vm_state
+        ctx,
+        [],
+        [],
+        test_script,
+        False,
+    ) as driver:
+        if interactive:
+            ptpython.repl.embed(driver.test_symbols(), {})
+        elif execute_test_script:
+            tic = time.time()
+            driver.run_tests()
+            toc = time.time()
+            ctx.glog(f"test script finished in {(toc-tic):.2f}s")
+        else:
+            ctx.glog("just start ???")
+            driver.test_script()
+    if ctx.use_httpd:
+        ctx.httpd.stop()
+
+    ctx.glog("Started")
+
+
 # TODO define scope of dry_run, must you dry_run deployment file creation ?
 # Also how to address driver part
 # def dry_run_print(ctx, launch_cmd):
 #     ctx.log("Dry-run:")
 #     ctx.log("   launch command:              {launch_cmd}")
 @click.command("start")
 @click.option(
     "-I",
     "--interactive",
     is_flag=True,
     help="drop into a python repl with driver functions",
 )
 @click.option(
     "-m",
-    "--machines-file",
+    "--machine-file",
     type=click.Path(resolve_path=True),
     help="file that contains remote machines names to (duplicates are considered as one).",
 )
 @click.option(
-    "-W", "--wait-machine-file", is_flag=True, help="wait machnes-file creation"
+    "-W", "--wait-machine-file", is_flag=True, help="wait machine-file creation"
 )
 @click.option(
     "-s",
     "--ssh",
     type=click.STRING,
     default="ssh -l root ",
     help="specify particular ssh command",
@@ -70,15 +125,14 @@
     "-S",
     "--sudo",
     type=click.STRING,
     default="sudo",
     help="specify particular sudo command",
 )
 @click.option(
-    "-p",
     "--push-path",
     help="remote path where to push image, kernel and kexec_script on machines (use to re-kexec)",
 )
 @click.option(
     "--reuse",
     is_flag=True,
     help="supposed a previous succeded start (w/ root access via ssh)",
@@ -98,21 +152,29 @@
     "-c",
     "-C",
     "--composition",
     type=click.STRING,
     help="specify composition, can specify flavour e.g. composition::flavour",
 )
 @click.option(
-    "-f", "--flavour", type=click.STRING, help="specify flavour",
+    "-f",
+    "--flavour",
+    type=click.STRING,
+    help="specify flavour",
 )
 @click.option(
-    "-t", "--test-script", is_flag=True, help="execute testscript",
+    "-t",
+    "--test-script",
+    is_flag=True,
+    help="execute testscript",
 )
 @click.option(
-    "--file-test-script", type=click.STRING, help="alternative testscript",
+    "--file-test-script",
+    type=click.STRING,
+    help="alternative testscript",
 )
 @click.option(
     "-w",
     "--sigwait",
     is_flag=True,
     help="wait any signal to exit after a start only action (not testscript execution or interactive use",
 )
@@ -136,26 +198,59 @@
 )
 @click.option(
     "--compose-info",
     type=click.Path(resolve_path=True),
     help="specific compose info file",
 )
 @click.option(
-    "-s", "--setup", type=click.STRING, help="Select setup variant",
+    "-i",
+    "--identity-file",
+    type=click.STRING,
+    help="path to the ssh public key to use to connect to the deployments",
+)
+@click.option(
+    "-s",
+    "--setup",
+    type=click.STRING,
+    help="Select setup variant",
+)
+@click.option(
+    "-p",
+    "--parameter",
+    type=click.STRING,
+    multiple=True,
+    help="Parameter added to deployment file (for contextualization phase)",
+)
+@click.option(
+    "-P",
+    "--parameter-file",
+    type=click.STRING,
+    help="Json file contains parameters added to deployment file (for contextualization phase)",
+)
+@click.option(
+    "-d",
+    "--deployment-file",
+    type=click.STRING,
+    help="Deployement json file use for the deployment (skip generation) Warning parametrization not supported (upto now)",
+)
+@click.option(
+    "--ip-range",
+    type=click.STRING,
+    default="",
+    help="IP range (for now only usable with nspawn flavour)",
 )
-# @click.option(
 #     "--dry-run", is_flag=True, help="Show what this command would do without doing it"
 # )
 @pass_context
 @on_finished(lambda ctx: ctx.show_elapsed_time())
-@on_started(lambda ctx: ctx.assert_valid_env())
+@on_started(lambda ctx: ctx.warning_valid_env())
 def cli(
     ctx,
     interactive,
-    machines_file,
+    machine_file,
     wait_machine_file,
     ssh,
     sudo,
     push_path,
     reuse,
     composition,
     flavour,
@@ -164,18 +259,45 @@
     test_script,
     file_test_script,
     sigwait,
     kernel_params,
     role_distribution,
     roles_distribution_file,
     compose_info,
+    identity_file,
     setup,
+    parameter,
+    parameter_file,
+    ip_range,
+    deployment_file
     # dry_run,
 ):
-    """Start Nixos Composition."""
+    """
+    Starts a set of nodes using the previous build.
+
+    `ROLE_DISTRIBUTION_FILE` is and optional YAML file describing how many instances of each role are expected.
+
+    ## Examples
+
+    - `nxc start`
+
+       Start the last built composition.
+
+    - `nxc start role-distrib.yaml`
+
+        With the file `role-distrib.yaml` written as this:
+
+        ```yaml
+        nfsServerNode: 1
+        nfsClientNode: 2
+        ```
+
+        Instantiates two nodes with the role `nfsClientNode` and one only with the role `nfsServerNode`. Of course, these roles have to be described beforehand in a `composition.nix` file.
+
+    """
     flavour_name = flavour
     if test_script:
         execute_test_script = True
         test_script = None
     else:
         execute_test_script = False
 
@@ -188,85 +310,130 @@
 
     ctx.ssh = ssh
     ctx.sudo = sudo
     ctx.push_path = push_path
     ctx.interactive = interactive
     ctx.execute_test_script = execute_test_script
     ctx.sigwait = sigwait
+    ctx.ip_range = ip_range
+
+    if deployment_file:
+        if not flavour:
+            ctx.elog("Option --flavour is required with --deployment-file option !")
+            sys.exit(2)
+        else:
+            ctx.flavour = get_flavour_by_name(flavour_name)(ctx)
+            read_deployment_info(ctx, deployment_file)
+
+    if deployment_file and (role_distribution or roles_distribution_file):
+        ctx.wlog(
+            "--role-distribution and --roles-distribution-file are ignored with --deployment-file option !"
+        )
+
     ctx.set_roles_distribution(role_distribution, roles_distribution_file)
 
-    # kernel_params can by setted through setup
+    # kernel_params can by set through setup
     if setup or op.exists(op.join(ctx.envdir, "setup.toml")):
         _, _, _, _, kernel_params = apply_setup(
-            ctx, setup, None, None, None, None, None, kernel_params,
+            ctx,
+            setup,
+            None,
+            None,
+            None,
+            None,
+            None,
+            kernel_params,
         )
     ctx.kernel_params = kernel_params
 
     if remote_deployment_info:
         ctx.use_httpd = True
 
+    if parameter_file:
+        with open(parameter_file, "r") as f:
+            try:
+                ctx.deployment_info["parameters"] = json.load(f)
+            except ValueError:
+                raise click.ClickException(
+                    f"Failed to parse parameters json file: {parameter_file}"
+                )
+
+    if parameter:
+        if "parameters" not in ctx.deployment_info:
+            ctx.deployment_info["parameters"] = {}
+        for p in parameter:
+            try:
+                (k, v) = p.split("=", 1)
+                v = ast.literal_eval(v)
+            except ValueError:
+                raise click.ClickException(f"Fail to parse parameter: {p}")
+            ctx.deployment_info["parameters"][k] = v
+
+    if deployment_file:
+        start(ctx, interactive, execute_test_script, port)
+        sys.exit(0)
+
     build_path = op.join(ctx.envdir, "build")
 
     if not compose_info and not op.exists(build_path):
         raise click.ClickException(
             "You need build composition first, with nxc build command"
         )
 
     # Handle cases where machines list must be provided
     machines = []
-    if machines_file and not op.isfile(machines_file) and not wait_machine_file:
-        raise click.ClickException(f"{machines_file} file does not exist")
+    if machine_file and not op.isfile(machine_file) and not wait_machine_file:
+        raise click.ClickException(f"{machine_file} file does not exist")
 
-    if push_path and not machines_file:
-        raise click.ClickException("machines_file must be provide to use push_path")
+    if push_path and not machine_file:
+        raise click.ClickException("machine_file must be provide to use push_path")
 
     if wait_machine_file:
-        if not machines_file:
+        if not machine_file:
             raise click.ClickException(
-                "You need to provide --machines-file option with --wait"
+                "You need to provide --machine-file option with --wait"
             )
 
-        if not op.isfile(machines_file):
-            # ctx.log(f"Waiting {machines_file} file creation")
+        if not op.isfile(machine_file):
+            # ctx.log(f"Waiting {machine_file} file creation")
             # TODO: add quiet option
             if ctx.show_spinner:
-                ctx.spinner.start(f"Waiting for {machines_file} creation")
+                ctx.spinner.start(f"Waiting for {machine_file} creation")
 
-            if "nfs" == get_fs_type(machines_file):
-                while not op.isfile(machines_file):
+            if "nfs" == get_fs_type(machine_file):
+                while not op.isfile(machine_file):
                     time.sleep(0.1)
             else:
                 wm = pyinotify.WatchManager()  # Watch Manager
                 loop = asyncio.get_event_loop()
 
                 global notifier
                 notifier = pyinotify.AsyncioNotifier(
                     wm, loop, default_proc_fun=EventHandler()
                 )
 
-                global machines_file_towait
-                machines_file_towait = machines_file
+                global machine_file_towait
+                machine_file_towait = machine_file
 
                 # TODO race condition remains possible ....
-                wm.add_watch(op.dirname(machines_file), pyinotify.CREATE)
+                wm.add_watch(op.dirname(machine_file), pyinotify.CREATE)
                 loop.run_forever()
                 notifier.stop()
 
             if ctx.show_spinner:
-                ctx.spinner.succeed(f"{machines_file} file created")
+                ctx.spinner.succeed(f"{machine_file} file created")
             else:
-                ctx.log(f"{machines_file} file created")
+                ctx.log(f"{machine_file} file created")
 
     # Determine composition and flavour name
     # First case composition is given not flavour name
     if composition and (flavour_name is None):
         splitted_composition = composition.split("::")
         len_splitted_composition = len(splitted_composition)
         if len_splitted_composition == 2:
-
             composition_name, flavour_name = splitted_composition
             composition_all_in_one_file = op.join(ctx.envdir, f"build/::{flavour_name}")
 
             if not op.lexists(composition_all_in_one_file):
                 build_path = op.join(ctx.envdir, f"build/{composition}")
                 if not op.lexists(build_path):
                     raise click.ClickException(
@@ -291,15 +458,16 @@
             search_path = f"{build_path}/*"
 
         build_paths = glob.glob(search_path)
         if not build_paths:
             raise click.ClickException("Failed to find last build")
 
         last_build_path = max(
-            build_paths, key=lambda x: os.stat(x, follow_symlinks=False).st_ctime,
+            build_paths,
+            key=lambda x: os.stat(x, follow_symlinks=False).st_ctime,
         )
 
         ctx.log("Use last build:")
         ctx.glog(last_build_path)
 
         build_path = last_build_path
         ctx.composition_flavour_prefix = op.basename(last_build_path)
@@ -334,69 +502,20 @@
         if reuse:
             (ssh, sudo, push_path) = ctx.platform.subsequent_start_values
         else:
             (ssh, sudo, push_path) = ctx.platform.first_start_values
         if ctx.push_path is None:
             ctx.push_path = push_path
 
-    if machines_file:
-        machines = read_hosts(machines_file)
+    if machine_file:
+        machines = read_hosts(machine_file)
         if not machines:
-            ctx.elog(f"Machine file '{machines_file}' is empty")
+            ctx.elog(f"Machine file '{machine_file}' is empty")
             sys.exit(1)
 
     if machines:
         translate_hosts2ip(ctx, machines)
         print(ctx.ip_addresses, ctx.host2ip_address)
 
-    ctx.flavour.generate_deployment_info()
-
-    if (
-        ctx.ip_addresses
-        and (ctx.flavour.name != "vm-ramdisk")
-        and (ctx.flavour.name != "vm")
-    ):
-        if ctx.use_httpd:
-            ctx.vlog("Launch: httpd to distribute deployment.json")
-            ctx.httpd = HTTPDaemon(ctx=ctx, port=port)
-
-
-        if hasattr(ctx.flavour, "generate_kexec_scripts"):
-            ctx.flavour.generate_kexec_scripts()
-
-        if ctx.push_path:
-            push_on_machines(ctx)
-
-        if ctx.use_httpd:
-            ctx.httpd.start(directory=ctx.envdir)
-
-        if not interactive:
-            ctx.flavour.launch(machines_file)
-            sys.exit(0)
-
-    test_script = read_test_script(ctx, ctx.compose_info)
-
-    if not interactive and not execute_test_script:
-        test_script = "start_all()"
-
-    with Driver(
-        # args.start_scripts, args.vlans, args.testscript.read_text(), args.keep_vm_state
-        ctx,
-        [],
-        [],
-        test_script,
-        False,
-    ) as driver:
-        if interactive:
-            ptpython.repl.embed(driver.test_symbols(), {})
-        elif execute_test_script:
-            tic = time.time()
-            driver.run_tests()
-            toc = time.time()
-            ctx.glog(f"test script finished in {(toc-tic):.2f}s")
-        else:
-            ctx.glog("just start ???")
-            driver.test_script()
-    if ctx.use_httpd:
-        ctx.httpd.stop()
+    ctx.flavour.generate_deployment_info(identity_file)
 
-    ctx.glog("Started")
+    start(ctx, interactive, execute_test_script, port, machine_file)
```

### Comparing `nixos_compose-0.5.5/nixos_compose/context.py` & `nixos_compose-0.5.6/nixos_compose/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.composition_name = None
         self.composition_flavour_prefix = None  # REMOVE _prefix ???
         self.compose_info_file = None  # change to compositions_file ?
         self.compose_info = None  # change to compositioin of merge w/ compositionS ?
         self.multiple_compositions = False
         self.compositions_info = None  # Rename to compositions_flavour ????
         self.deployment_filename: str = ""
-        self.deployment_info = None  # change to deployment ?
+        self.deployment_info = {}  # change to deployment ?
         self.deployment_info_b64 = ""  # change to depolyment_b64 ?
         self.ip_addresses = []
         self.host2ip_address = {}
         self.ssh = ""
         self.sudo = ""
         self.push_path = None
         self.interactive = False
@@ -89,15 +89,17 @@
         ]
 
         self.roles_distribution = {}
         self.setup = None
         self.sigwait = None
         self.kernel_params = None
         self.all_started: bool = False
-        self.no_start: bool = False  # use w/ driver CLI command which must not start machines
+        self.no_start: bool = (
+            False  # use w/ driver CLI command which must not start machines
+        )
         self.external_connect: bool = False
         self.vde_tap: bool = False  # use to add tap interface which allow external IP
         # access either done by port forwarding on local
         # interface
         self.spinner = LazySpinner()
         self.show_spinner = True
 
@@ -124,14 +126,20 @@
         if not os.path.isdir(self.envdir):
             raise click.ClickException(
                 "Missing nixos composition environment directory."
                 " Run `nxc init` to create"
                 " a new composition environment "
             )
 
+    def warning_valid_env(self):
+        if not os.path.isdir(self.envdir):
+            click.ClickException(
+                "Warning: missing nixos composition environment directory."
+            )
+
     def log(self, msg, *args, **kwargs):
         """Logs a message to stdout."""
         if args:
             msg %= args
         kwargs.setdefault("file", sys.stdout)
         click.echo(msg, **kwargs)
```

### Comparing `nixos_compose-0.5.5/nixos_compose/driver/__init__.py` & `nixos_compose-0.5.6/nixos_compose/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/driver/driver.py` & `nixos_compose-0.5.6/nixos_compose/driver/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,28 @@
     ):
         self.ctx = ctx
         self.tests = tests
 
         tmp_dir = Path(os.environ.get("TMPDIR", tempfile.gettempdir()))
         tmp_dir.mkdir(mode=0o700, exist_ok=True)
 
-        # if hasattr(ctx.flavour, "vlan"):
-        #    self.vlans = [ctx.flavour.vlan()]
+        # if hasattr(ctx.flavour, "create_vlan"):
+        #    self.vlans = [ctx.flavour.create_vlan()]
 
         ctx.flavour.driver_initialize(tmp_dir)
 
         # if hasattr(ctx.flavour, "machines") and ctx.flavour.machines:
         if ctx.flavour.machines:
             self.machines = ctx.flavour.machines
         else:
             rootlog.warning("No machine defined during driver init")
 
-        if hasattr(ctx.flavour, "vlan") and not ctx.no_start:
-            self.vlans = [ctx.flavour.vlan()]
+        # TODO move
+        if hasattr(ctx.flavour, "create_vlan") and not ctx.no_start:
+            self.vlans = [ctx.flavour.create_vlan()]
 
         # def cmd(scripts: List[str]) -> Iterator[NixStartScript]:
         #     for s in scripts:
         #         yield NixStartScript(s)
 
         # self.machines = [
         #     Machine(
@@ -127,15 +128,20 @@
             + ",\n    "
             + ", ".join(list(general_symbols.keys()))
         )
         return {**general_symbols, **machine_symbols}  # , **vlan_symbols}
 
     def test_script(self) -> None:
         """Run the test script"""
-        with rootlog.nested("run the test script"):
+        if self.ctx.execute_test_script:
+            message = "run the test script"
+        else:
+            message = "run start command in"
+
+        with rootlog.nested(message):
             symbols = self.test_symbols()  # call eagerly
             exec(self.tests, symbols, None)
 
     def run_tests(self) -> None:
         """Run the test script (for non-interactive test runs)"""
         self.test_script()
         # TODO: Collect coverage data
```

### Comparing `nixos_compose-0.5.5/nixos_compose/driver/logger.py` & `nixos_compose-0.5.6/nixos_compose/driver/logger.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/driver/machine.py` & `nixos_compose-0.5.6/nixos_compose/driver/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,19 @@
         # TODO: qemu script already catpures this env variable, legacy?
         qemu_opts += " " + os.environ.get("QEMU_OPTS", "")
 
         self.qemu_opts = qemu_opts
 
         return f"{self._cmd}"
 
-    def build_environment(self, state_dir: Path, shared_dir: Path,) -> dict:
+    def build_environment(
+        self,
+        state_dir: Path,
+        shared_dir: Path,
+    ) -> dict:
         # We make a copy to not update the current environment
         kernel_params = ""
         if self.flavour.ctx.kernel_params:
             kernel_params = self.flavour.ctx.kernel_params
         env = dict(os.environ)
         env.update(
             {
@@ -720,15 +724,18 @@
             s.bind(str(path))
             s.listen(1)
             return s
 
         monitor_socket = create_socket(clear(self.monitor_path))
         shell_socket = create_socket(clear(self.shell_path))
         self.process = self.start_command.run(
-            self.state_dir, self.shared_dir, self.monitor_path, self.shell_path,
+            self.state_dir,
+            self.shared_dir,
+            self.monitor_path,
+            self.shell_path,
         )
 
         try:
             self.monitor, _ = monitor_socket.accept()
         except socket.timeout:
             self.ctx.elog("Time out reached on monitor socket accept (qemu)")
             if self.process.poll():
@@ -856,15 +863,14 @@
 
     def unblock(self) -> None:
         """Make the machine reachable."""
         self.send_monitor_command("set_link virtio-net-pci.1 on")
 
     @use_flavour_method_if_any
     def release(self) -> None:
-
         if self.pid is None:
             return
 
         rootlog.info(f"kill machine (pid {self.pid})")
 
         assert self.process
         assert self.shell
@@ -874,25 +880,29 @@
         self.process.terminate()
         self.shell.close()
         self.monitor.close()
         self.serial_thread.join()
 
     def start_process_shell(self, args):
         # command examples:
-        # ['docker-compose', '-f', '/home/auguste/work/tests/21-22/nxc-test/nxc/deploy/docker_compose/docker-compose.json', 'exec', '-T', ']
-
+        # ['docker-compose', '-f', 'nxc/artifact/composition/docker/docker-compose.json', 'exec', '-T', ']
         # ['ssh', '-t', '-o', 'StrictHostKeyChecking=no', '-l', 'root', '10.0.2.16']
         self.process_shell = subprocess.Popen(
-            args, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+            args,
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
         )
 
     def execute_process_shell(
-        self, command: str, check_return: bool = True, timeout: Optional[int] = 900,
+        self,
+        command: str,
+        check_return: bool = True,
+        timeout: Optional[int] = 900,
     ) -> Tuple[int, str]:
-
         self.connect()
 
         process_shell = self.process_shell
 
         try:
             (stdout, _stderr) = process_shell.communicate(
                 command.encode(), timeout=timeout
```

### Comparing `nixos_compose-0.5.5/nixos_compose/driver/vlan.py` & `nixos_compose-0.5.6/nixos_compose/driver/vlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from typing import Optional
 import io
 import os
 import pty
 import sys
 import shutil
 import subprocess
 
@@ -14,25 +15,26 @@
     number handles. The network's lifetime equals the object's lifetime.
     """
 
     nr: int
     socket_dir: Path
 
     process: subprocess.Popen
-    slirpvde_process: subprocess.Popen
+    slirpvde_process: Optional[subprocess.Popen]
     pid: int
     fd: io.TextIOBase
 
     def __repr__(self) -> str:
         return f"<Vlan Nr. {self.nr}>"
 
     def __init__(self, nr: int, tmp_dir: Path, ctx):
         self.ctx = ctx
         self.nr = nr
         self.socket_dir = tmp_dir / f"vde{self.nr}.ctl"
+        self.slirpvde_process = None
 
         # TODO: don't side-effect environment here
         os.environ[f"QEMU_VDE_SOCKET_{self.nr}"] = str(self.socket_dir)
 
         rootlog.info("start vlan")
         pty_master, pty_slave = pty.openpty()
 
@@ -45,26 +47,24 @@
         if ctx.vde_tap:
             rootlog.info(
                 f"starting VDE switch for network {self.nr}, with tap0 (sudo required)"
             )
             subprocess.call("sudo true", shell=True)
             vde_cmd = ["sudo"] + vde_cmd + ["-tap", "tap0"]
 
-        group_users = "users"
-        if ctx.platform and ctx.platform.group_users:
-            group_users = ctx.platform.group_users
         vde_cmd = vde_cmd + [
             "-s",
             self.socket_dir,
             "-mod",
             "0770",
-            "-group",
-            group_users,
         ]
 
+        if ctx.platform and ctx.platform.group_users:
+            vde_cmd = vde_cmd + ["-group", ctx.platform.group_users]
+
         self.process = subprocess.Popen(
             vde_cmd,
             stdin=pty_slave,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=False,
         )
@@ -101,9 +101,9 @@
 
         rootlog.info(f"running vlan (pid {self.pid})")
 
     def __del__(self) -> None:
         rootlog.info(f"kill vlan (pid {self.pid})")
         self.fd.close()
         self.process.terminate()
-        if self.slirpvde_process:
+        if self.slirpvde_process is not None:
             self.slirpvde_process.terminate()
```

### Comparing `nixos_compose-0.5.5/nixos_compose/flavour.py` & `nixos_compose-0.5.6/nixos_compose/flavour.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,13 @@
         for _ in range(round):
             if mode == "all" and self.check(state) == len(self.machines):
                 return True
             elif mode == "any" and self.check(state) > 0:
                 return
             time.sleep(period)
         return False
+
+    def generate_deployment_info(self, ssh_pub_key_file=None):
+        pass
+
+    def ext_connect(self, user, node, execute=True, ssh_key_file=None):
+        pass
```

### Comparing `nixos_compose-0.5.5/nixos_compose/flavours/__init__.py` & `nixos_compose-0.5.6/nixos_compose/flavours/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
    :copyright: Copyright 2006-2021 by the Pygments team, see AUTHORS.
     :license: BSD, see LICENSE for details.
 """
 
 #: Maps flavour names to 'submodule::classname'.
 FLAVOUR_MAP = {
     "docker": "docker::DockerFlavour",
+    "nspawn": "nspawn::NspawnFlavour",
     "vm": "vm::VmFlavour",
     "vm-ramdisk": "vm::VmRamdiskFlavour",
     "g5k-nfs-store": "grid5000::G5kNfsStoreFlavour",
     "g5k-ramdisk": "grid5000::G5kRamdiskFlavour",
     "g5k-image": "grid5000::G5KImageFlavour",
 }
 
 
 class ClassNotFound(ValueError):
     """Raised if one of the lookup functions didn't find a matching class."""
 
 
 def get_flavour_by_name(name):
-
     if name in FLAVOUR_MAP:
         mod, cls = FLAVOUR_MAP[name].split("::")
 
     try:
         mod = __import__("nixos_compose.flavours." + mod, None, None, [cls])
     except ImportError:
         raise ClassNotFound(f"Could not find flavour module {mod}")
```

### Comparing `nixos_compose-0.5.5/nixos_compose/flavours/docker.py` & `nixos_compose-0.5.6/nixos_compose/flavours/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     base_docker_compose, prefix_store = realpath_from_store(
         ctx, ctx.compose_info["docker-compose-file"], include_prefix_store=True
     )
     docker_compose_content = {"services": {}}
     nodes_info = {}
 
     with open(base_docker_compose) as dc_file:
-
         dc_json = json.load(dc_file)
         if prefix_store:
             set_prefix_store_volumes(dc_json, prefix_store)
 
         roles_distribution = {}
         for role in ctx.compose_info["roles"]:
             if role in ctx.roles_distribution:
@@ -103,20 +102,20 @@
                         docker_compose_content["services"][hostname] = config
                         nodes_info[hostname] = role
             else:
                 raise Exception("Unvalid type for specifying the roles of the nodes")
         dc_json.pop("services")
         docker_compose_content = docker_compose_content | dc_json
 
-    deploy_dir = op.join(ctx.envdir, "deploy", "docker_compose")
-    if not op.exists(deploy_dir):
-        create = click.style("   create", fg="green")
-        ctx.log("   " + create + "  " + deploy_dir)
-        os.mkdir(deploy_dir)
-    docker_compose_path = op.join(deploy_dir, "docker-compose.json")
+    artifact_dir = op.join(
+        ctx.envdir, f"artifact/{ctx.composition_name}/{ctx.flavour.name}"
+    )
+    os.makedirs(artifact_dir, mode=0o700, exist_ok=True)
+
+    docker_compose_path = op.join(artifact_dir, "docker-compose.json")
 
     with open(docker_compose_path, "w") as outfile:
         outfile.write(json.dumps(docker_compose_content))
     return docker_compose_path, nodes_info
 
 
 def generate_deployment_info_docker(ctx):
@@ -126,66 +125,67 @@
     deploy_dir = op.join(ctx.envdir, "deploy")
     if not op.exists(deploy_dir):
         create = click.style("   create", fg="green")
         ctx.log("   " + create + "  " + deploy_dir)
         os.mkdir(deploy_dir)
 
     docker_compose_path, nodes_info = generate_docker_compose_file(ctx)
-    deployment = {
-        # "nodes": ctx.compose_info["nodes"],
-        "nodes": list(nodes_info.keys()),
-        # "deployment": {n: {"role": n} for n in ctx.compose_info["nodes"]},
-        "deployment": {
-            node_name: {"role": role_name}
-            for (node_name, role_name) in nodes_info.items()
-        },
-        "docker-compose-file": docker_compose_path,
+
+    deployment_info = ctx.deployment_info
+
+    # "nodes": ctx.compose_info["nodes"],
+    deployment_info["nodes"] = list(nodes_info.keys())
+    # "deployment": {n: {"role": n} for n in ctx.compose_info["nodes"]},
+    deployment_info["deployment"] = {
+        node_name: {"role": role_name} for (node_name, role_name) in nodes_info.items()
     }
+    deployment_info["docker-compose-file"] = docker_compose_path
 
     if "test_script" in ctx.compose_info:
-        deployment["test_script"] = ctx.compose_info["test_script"]
+        deployment_info["test_script"] = ctx.compose_info["test_script"]
 
     if "all" in ctx.compose_info:
-        deployment["all"] = ctx.compose_info["all"]
-
-    json_deployment = json.dumps(deployment, indent=2)
+        deployment_info["all"] = ctx.compose_info["all"]
 
+    # TODO move to action.py and factorize w/ geenerate_deployment_info
     with open(
         op.join(deploy_dir, f"{ctx.composition_flavour_prefix}.json"), "w"
     ) as outfile:
-        outfile.write(json_deployment)
+        outfile.write(json.dumps(deployment_info, indent=2))
 
-    ctx.deployment_info = deployment
     return docker_compose_path
 
 
 class DockerFlavour(Flavour):
-
     docker_compose_file = None
 
     def __init__(self, ctx):
         super().__init__(ctx)
 
         self.name = "docker"
         self.description = ""
         # TOR self.docker_processes = {}
 
-    def generate_deployment_info(self):
+    def generate_deployment_info(self, ssh_pub_key_file=None):
         self.docker_compose_file = generate_deployment_info_docker(self.ctx)
 
     def driver_initialize(self, tmp_dir):
-
         assert self.ctx.deployment_info
         if not self.docker_compose_file:
             self.docker_compose_file = self.ctx.deployment_info["docker-compose-file"]
 
         nodes_names = self.ctx.deployment_info["nodes"]
         for name in nodes_names:
             self.machines.append(
-                Machine(self.ctx, tmp_dir=tmp_dir, start_command="", name=name,)
+                Machine(
+                    self.ctx,
+                    tmp_dir=tmp_dir,
+                    start_command="",
+                    name=name,
+                )
             )
 
     def check(self, state="running"):
         check_process = subprocess.check_output(
             [
                 "docker-compose",
                 "-f",
@@ -239,15 +239,14 @@
     def execute(
         self,
         machine,
         command: str,
         check_return: bool = True,
         timeout: Optional[int] = 900,
     ) -> Tuple[int, str]:
-
         return machine.execute_process_shell(command, check_return, timeout)
 
     def restart(self, machine):
         machine.restart_process_shell()
 
     def cleanup(self):
         # TODO handle stdout/stderr
@@ -263,15 +262,15 @@
             ]
         )
 
     def shell_interact(self, machine) -> None:
         self.connect(machine)
         self.ext_connect("root", machine.name)
 
-    def ext_connect(self, user, node, execute=True):
+    def ext_connect(self, user, node, execute=True, ssh_key_file=None):
         if not self.docker_compose_file:
             self.docker_compose_file = self.ctx.deployment_info["docker-compose-file"]
 
         cmd = f"docker-compose -f {self.docker_compose_file} exec -u {user} {node} bash"
         print(f"ext_connect {cmd}")
         if execute:
             return_code = subprocess.run(cmd, shell=True).returncode
```

### Comparing `nixos_compose-0.5.5/nixos_compose/flavours/grid5000.py` & `nixos_compose-0.5.6/nixos_compose/flavours/grid5000.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         kernel_params: $kernel_params
       filesystem: ext4
       partition_type: 131
       multipart: false
 """
 
 
-def generate_kadeploy_envfile(ctx, deploy=None, kernel_params="", kaenv_path=None, deploy_image_path=None):
+def generate_kadeploy_envfile(
+    ctx, deploy=None, kernel_params="", kaenv_path=None, deploy_image_path=None
+):
     if not ctx.compose_info:
         read_compose_info(ctx)
 
     base_path = op.join(
         ctx.envdir, f"artifact/{ctx.composition_name}/{ctx.flavour.name}"
     )
     os.makedirs(base_path, mode=0o700, exist_ok=True)
@@ -79,31 +81,33 @@
         additional_kernel_params = ctx.kernel_params
     with open(kaenv_path, "w") as kaenv_file:
         t = Template(KADEPOY_ENV_DESC)
         kaenv = t.substitute(
             image_name="NixOS",
             author=user,
             system=KADEPOY_ARCH[system],
-            file_image_url=f"local://{deploy_image_path}" if deploy_image_path else f"http://public.{g5k_site}.grid5000.fr/~{user}/nixos.tar.xz",
+            file_image_url=f"local://{deploy_image_path}"
+            if deploy_image_path
+            else f"http://public.{g5k_site}.grid5000.fr/~{user}/nixos.tar.xz",
             kernel_params=f"boot.shell_on_fail console=tty0 console=ttyS0,115200 deploy={deploy} {additional_kernel_params} {kernel_params}",
         )
         kaenv_file.write(kaenv)
 
 
 class G5kKexecBasedFlavour(Flavour):
     def __init__(self, ctx):
         super().__init__(ctx)
 
-    def generate_deployment_info(self):
-        generate_deployment_info(self.ctx)
+    def generate_deployment_info(self, ssh_pub_key_file=None):
+        generate_deployment_info(self.ctx, ssh_pub_key_file)
 
     def generate_kexec_scripts(self):
         generate_kexec_scripts(self.ctx)
 
-    def launch(self):
+    def launch(self, machine_file=None):
         launch_ssh_kexec(self.ctx)
         time.sleep(10)
         wait_ssh_ports(self.ctx)
 
     def driver_initialize(self, tmp_dir):
         self.tmp_dir = tmp_dir
         ctx = self.ctx
@@ -141,16 +145,16 @@
                     "StrictHostKeyChecking=no",
                     "-l",
                     "root",
                     machine.ip,
                 ]
             )
 
-    def ext_connect(self, user, node, execute=True):
-        return ssh_connect(self.ctx, user, node, execute)
+    def ext_connect(self, user, node, execute=True, ssh_key_file=None):
+        return ssh_connect(self.ctx, user, node, execute, ssh_key_file)
 
 
 class G5kNfsStoreFlavour(G5kKexecBasedFlavour):
     def __init__(self, ctx):
         super().__init__(ctx)
 
         self.name = "g5k-nfs-store"
@@ -183,50 +187,50 @@
 
 class G5KImageFlavour(Flavour):
     def __init__(self, ctx):
         super().__init__(ctx)
 
         self.name = "g5k-image"
 
-    def generate_deployment_info(self):
-        generate_deployment_info(self.ctx)
+    def generate_deployment_info(self, ssh_pub_key_file=None):
+        generate_deployment_info(self.ctx, ssh_pub_key_file)
 
     def launch(self, machine_file=None, kaenv_path=None, deploy_image_path=None):
-        generate_kadeploy_envfile(self.ctx, kaenv_path=kaenv_path, deploy_image_path=deploy_image_path)
+        generate_kadeploy_envfile(
+            self.ctx, kaenv_path=kaenv_path, deploy_image_path=deploy_image_path
+        )
         image_path = realpath_from_store(
             self.ctx, self.ctx.deployment_info["all"]["image"]
         )
         if deploy_image_path is None:
             user = os.environ["USER"]
             deploy_image_path = f"~{user}/public/nixos.tar.xz"
-            
-        cmd_copy_image = f'cp {image_path} {deploy_image_path} && chmod 644 {deploy_image_path}'
+
+        cmd_copy_image = (
+            f"cp {image_path} {deploy_image_path} && chmod 644 {deploy_image_path}"
+        )
         if machine_file or click.confirm(
-            f'Do you want to copy image to {deploy_image_path} ?'
+            f"Do you want to copy image to {deploy_image_path} ?"
         ):
             try:
                 subprocess.call(cmd_copy_image, shell=True)
             except Exception as ex:
                 raise click.ClickException(f"Failed to copy image: {ex}")
         else:
             print(f"You can copy image with: {cmd_copy_image}")
         base_path = op.join(
             self.ctx.envdir,
             f"artifact/{self.ctx.composition_name}/{self.ctx.flavour.name}",
         )
         if kaenv_path is None:
-            kaenv_path = op.join(base_path, "nixos.yaml") 
+            kaenv_path = op.join(base_path, "nixos.yaml")
         if machine_file:
-            cmd_kadeploy = (
-                f'kadeploy3 -a {kaenv_path} -f {machine_file}'
-            )
+            cmd_kadeploy = f"kadeploy3 -a {kaenv_path} -f {machine_file}"
         else:
-            cmd_kadeploy = (
-                f'kadeploy3 -a {kaenv_path} -f $OAR_NODEFILE'
-            )
+            cmd_kadeploy = f"kadeploy3 -a {kaenv_path} -f $OAR_NODEFILE"
 
         if machine_file or click.confirm(
             "Do you want to kadeploy nixos.tar.xz image on nodes from $OAR_NODEFILE"
         ):
             try:
                 subprocess.call(cmd_kadeploy, shell=True)
             except Exception as ex:
@@ -247,9 +251,9 @@
                     "StrictHostKeyChecking=no",
                     "-l",
                     "root",
                     machine.ip,
                 ]
             )
 
-    def ext_connect(self, user, node, execute=True):
-        return ssh_connect(self.ctx, user, node, execute)
+    def ext_connect(self, user, node, execute=True, ssh_key_file=None):
+        return ssh_connect(self.ctx, user, node, execute, ssh_key_file)
```

### Comparing `nixos_compose-0.5.5/nixos_compose/flavours/vm.py` & `nixos_compose-0.5.6/nixos_compose/flavours/vm.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     vlan = None
 
     def __init__(self, ctx):
         super().__init__(ctx)
         ctx.external_connect = True  # to force use of ssh on foo.execute(command)
         platform_detection(ctx)
 
-    def generate_deployment_info(self):
-        generate_deployment_info(self.ctx)
+    def generate_deployment_info(self, ssh_pub_key_file=None):
+        generate_deployment_info(self.ctx, ssh_pub_key_file)
 
     def create_machines(self):
         ctx = self.ctx
         deployment_nodes = ctx.deployment_info["deployment"]
         qemu_script = realpath_from_store(
             ctx, ctx.deployment_info["all"]["qemu_script"]
         )
@@ -144,15 +144,15 @@
                 "DEPLOY"
             ] = f"deploy={self.ctx.deployment_filename[len(self.ctx.envdir)+1:]}"
         else:
             rootlog.nested(f'Variable environment DEPLOY: {os.environ["DEPLOY"]}')
 
         self.create_machines()
 
-    def vlan(self):
+    def create_vlan(self):
         self.vlan = VLan(0, self.tmp_dir, ctx=self.ctx)
         return self.vlan
 
     def start_process_shell(self, machine):
         machine.start_process_shell(
             [
                 "ssh",
@@ -186,16 +186,16 @@
         kill_proc_tree(machine.pid, include_parent=False)
 
         machine.process.terminate()
         machine.shell.close()
         machine.monitor.close()
         machine.serial_thread.join()
 
-    def ext_connect(self, user, node, execute=True):
-        return ssh_connect(self.ctx, user, node, execute)
+    def ext_connect(self, user, node, execute=True, ssh_key_file=None):
+        return ssh_connect(self.ctx, user, node, execute, ssh_key_file)
 
 
 class VmFlavour(VmBasedFlavour):
     def __init__(self, ctx):
         super().__init__(ctx)
         self.name = "vm"
         self.image = {"distribution": "all-in-one"}
```

### Comparing `nixos_compose-0.5.5/nixos_compose/g5k.py` & `nixos_compose-0.5.6/nixos_compose/g5k.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/httpd.py` & `nixos_compose-0.5.6/nixos_compose/httpd.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/nxc_execo.py` & `nixos_compose-0.5.6/nixos_compose/nxc_execo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-import execo
-import execo_g5k
-import execo_engine
-from execo import Process, Host, Remote, SshProcess, Report
-from execo_g5k import get_oar_job_nodes, oarsub, oardel, OarSubmission, wait_oar_job_start
-from execo_engine import Engine
+# import execo
+# import execo_g5k
+# import execo_engine
+# from execo import Process, Host, Remote, SshProcess, Report
+from execo import Host
+from execo_g5k import get_oar_job_nodes
+
+#     get_oar_job_nodes,
+#     oarsub,
+#     oardel,
+#     OarSubmission,
+#     wait_oar_job_start,
+# )
+# from execo_engine import Engine
 import os
 import os.path as op
-import time
-import logging
+
+# import time
+# import logging
 import tempfile
 from .context import Context
 from .actions import realpath_from_store, translate_hosts2ip
 from .flavours.grid5000 import G5kRamdiskFlavour, G5KImageFlavour, G5kNfsStoreFlavour
-from .g5k import key_sleep_script
+
+# from .g5k import key_sleep_script
 from .httpd import HTTPDaemon
 
 
 def get_envdir(ctx):
     if os.path.isfile("nxc.json"):
         if os.path.islink("nxc.json"):
             ctx.nxc_file = os.readlink("nxc.json")
@@ -25,21 +35,24 @@
         with open(ctx.nxc_file, "r") as f:
             ctx.load_nxc(f)
 
         ctx.envdir = op.dirname(ctx.nxc_file)
     else:
         raise Exception("Cannot find `nxc.json`")
 
-def get_oar_job_nodes_nxc(oar_job_id,
-                          site,
-                          compose_info_file=None,
-                          flavour_name="g5k-ramdisk",
-                          composition_name="composition",
-                          roles_quantities={},
-                          port=0):
+
+def get_oar_job_nodes_nxc(
+    oar_job_id,
+    site,
+    compose_info_file=None,
+    flavour_name="g5k-ramdisk",
+    composition_name="composition",
+    roles_quantities={},
+    port=0,
+):
     """
     Brother of the "get_oar_job_nodes" function from execo
     but does the mapping with roles from NXC
     """
     ctx = Context()
     # TODO: kaberk
     ctx.composition_name = composition_name
@@ -49,15 +62,17 @@
     ctx.envdir = None
     get_envdir(ctx)
 
     if compose_info_file:
         ctx.compose_info_file = compose_info_file
     else:
         build_folder = op.join(ctx.envdir, "build")
-        simlink_build = op.join(build_folder, f"{ctx.composition_name}::{ctx.flavour_name}")
+        simlink_build = op.join(
+            build_folder, f"{ctx.composition_name}::{ctx.flavour_name}"
+        )
         ctx.compose_info_file = realpath_from_store(ctx, simlink_build)
 
     # print(f"compose info file: {ctx.compose_info_file}")
 
     g5k_nodes = get_oar_job_nodes(oar_job_id, site)
     print(f"G5K nodes: {g5k_nodes}")
     machines = [node.address for node in g5k_nodes]
@@ -77,15 +92,14 @@
         raise Exception(f"'{flavour_name}' is not an available flavour")
     # ?!
     flavour.ctx.flavour = flavour
 
     print("generating deploy info")
     flavour.generate_deployment_info()
 
-    flavour.ctx.mode = {"name": "ssh", "vm": False, "shell": "ssh"}
     # flavour.ctx.ssh = f"OAR_JOB_ID={oar_job_id} oarsh"
     flavour.ctx.ssh = "ssh"
     flavour.ctx.sudo = "sudo-g5k"
 
     flavour.ctx.log("Deploying")
     if hasattr(flavour, "generate_kexec_scripts"):
         flavour.generate_kexec_scripts()
@@ -96,18 +110,22 @@
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tmp_kaenv = tempfile.NamedTemporaryFile(delete=False)
         temp_dir = tempfile.TemporaryDirectory()
         try:
             machines_str = "\n".join(machine for machine in machines)
             # for machine in machines:
             #     machines_str += f"{machine}\n"
-            tmp.write(machines_str.encode('utf-8'))
+            tmp.write(machines_str.encode("utf-8"))
             tmp.flush()
             nxc_image_path = op.join(temp_dir.name, "nixos.tar.xz")
-            flavour.launch(machine_file=tmp.name, kaenv_path=tmp_kaenv.name, deploy_image_path=nxc_image_path)
+            flavour.launch(
+                machine_file=tmp.name,
+                kaenv_path=tmp_kaenv.name,
+                deploy_image_path=nxc_image_path,
+            )
         finally:
             tmp.close()
             os.unlink(tmp.name)
             tmp_kaenv.close()
             os.unlink(tmp_kaenv.name)
             temp_dir.cleanup()
```

### Comparing `nixos_compose-0.5.5/nixos_compose/platform.py` & `nixos_compose-0.5.6/nixos_compose/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         self.subsequent_start_values = ("ssh -l root", "sudo", "/")
         self.oar_job_id = None
         self.oar_job = None
         self.group_users = "g5k-users"
         self.nix_store = nix_store_location(ctx)
 
     def retrieve_machines(self, ctx):
-
         oar_job = None
         oar_job_id_str = None
         # oar_job_id_prev_str = None
         halo = False
 
         # if "oar_job_id" in ctx.state:
         #    oar_job_id_prev_str = str(ctx.state["oar_job_id"])
```

### Comparing `nixos_compose-0.5.5/nixos_compose/setup.py` & `nixos_compose-0.5.6/nixos_compose/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     composition_file,
     composition_flavour,
     flavour,
     setup_param,
     kernel_params,
     filename="setup.toml",
 ):
-
     update_setup_file = False
 
     setup_file = op.join(ctx.envdir, filename)
     if not op.exists(setup_file):
         return (nix_flags, composition_file)
 
     # test if setup.toml is inside flake.nix and is not commented
```

### Comparing `nixos_compose-0.5.5/nixos_compose/state.py` & `nixos_compose-0.5.6/nixos_compose/state.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/nixos_compose/tools/kataract.py` & `nixos_compose-0.5.6/nixos_compose/tools/kataract.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         user = f"{user}@"
     tasks_cmd = [f"{scp} {file_input} {user}{h}:{file_output}" for h in hosts]
     # print(tasks_cmd)
     return tasks_cmd
 
 
 def exec_kataract_tasks(tasks_cmd, elog=elog, vlog=vlog):
-
     asyncio.set_event_loop(asyncio.new_event_loop())
     loop = asyncio.get_event_loop()
 
     tasks = [run(task_cmd) for task_cmd in tasks_cmd]
 
     finished, unfinished = loop.run_until_complete(asyncio.wait(tasks, timeout=60))
```

### Comparing `nixos_compose-0.5.5/nixos_compose/utils.py` & `nixos_compose-0.5.6/nixos_compose/utils.py`

 * *Files identical despite different names*

### Comparing `nixos_compose-0.5.5/pyproject.toml` & `nixos_compose-0.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nixos-compose"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["Olivier Richard <olivier.richard@imag.fr>"]
 license = "MIT"
 include = [
      { path = 'examples', format = 'wheel' },
      { path = 'nix', format = 'wheel' },
      #{ path = 'tools', format = 'wheel' }
```

### Comparing `nixos_compose-0.5.5/PKG-INFO` & `nixos_compose-0.5.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nixos-compose
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 License: MIT
 Author: Olivier Richard
 Author-email: olivier.richard@imag.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: execo (>=2.6.8,<3.0.0)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: pexpect (>=4.8.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: ptpython (>=3.0.7,<4.0.0)
```

