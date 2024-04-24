# Comparing `tmp/dimples-0.5.5.tar.gz` & `tmp/dimples-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.5.5.tar", last modified: Tue Apr 23 09:11:37 2024, max compression
+gzip compressed data, was "dist/dimples-0.5.6.tar", last modified: Wed Apr 24 06:49:33 2024, max compression
```

## Comparing `dimples-0.5.5.tar` & `dimples-0.5.6.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-23 09:11:37.000000 dimples-0.5.5/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.5/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.5/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.5/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.5/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2023-12-05 04:21:35.000000 dimples-0.5.5/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.5/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.5/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.5/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.5/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.5/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.5/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.5/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.5/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.5/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.5/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.5/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.5/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.5/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.5/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.5/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6624 2024-04-23 08:44:53.000000 dimples-0.5.5/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8578 2024-03-07 09:39:13.000000 dimples-0.5.5/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.5/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.5/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.5/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5560 2024-04-23 08:43:31.000000 dimples-0.5.5/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.5/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.5/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.5/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.5/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.5/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.5/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.5/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.5/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.5/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.5/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.5/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.5/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.5/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.5.5/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.5/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-16 06:12:16.000000 dimples-0.5.5/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.5/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.5/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.5/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.5/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.5/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.5/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.5/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.5/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.5/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.5/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4531 2023-10-13 16:11:34.000000 dimples-0.5.5/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.5/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.5/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    11821 2024-04-23 08:42:23.000000 dimples-0.5.5/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.5/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.5/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.5/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2023-11-08 09:04:27.000000 dimples-0.5.5/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.5/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     3819 2023-09-05 04:47:59.000000 dimples-0.5.5/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.5/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.5/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.5/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.5/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.5/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.5/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.5/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.5/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.5/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.5/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.5/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.5/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.5/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.5/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.5/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.5/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.5/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.5/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.5/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.5/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.5/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.5/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.5/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.5/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.5/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.5/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.5/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    14595 2024-04-23 08:44:08.000000 dimples-0.5.5/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.5/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.5/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.5/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.5/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.5/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.5/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.5/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.5/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.5/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.5/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.5/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.5/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.5/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.5/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.5/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7346 2024-02-18 04:20:32.000000 dimples-0.5.5/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.5/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.5/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.5/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.5/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.5/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.5/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13438 2024-04-23 08:43:17.000000 dimples-0.5.5/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4454 2024-02-17 18:19:10.000000 dimples-0.5.5/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-16 07:12:40.000000 dimples-0.5.5/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    15437 2024-04-16 06:41:33.000000 dimples-0.5.5/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5476 2024-04-23 08:44:27.000000 dimples-0.5.5/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9843 2024-03-13 14:34:33.000000 dimples-0.5.5/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.5/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.5/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3832 2024-04-22 16:08:14.000000 dimples-0.5.5/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.5/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.5/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4710 2024-04-23 08:43:02.000000 dimples-0.5.5/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6355 2024-04-23 08:38:51.000000 dimples-0.5.5/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-29 14:16:57.000000 dimples-0.5.5/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.5/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:11:37.000000 dimples-0.5.5/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-23 08:45:20.000000 dimples-0.5.5/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-24 06:49:33.000000 dimples-0.5.6/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.6/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.6/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.6/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.6/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2024-04-24 03:33:53.000000 dimples-0.5.6/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.6/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.6/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.6/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.6/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.6/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.6/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.6/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.6/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.6/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.6/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.6/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.6/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.6/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.6/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.6/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6624 2024-04-23 08:44:53.000000 dimples-0.5.6/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8638 2024-04-23 09:37:33.000000 dimples-0.5.6/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.6/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.6/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.6/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5560 2024-04-23 08:43:31.000000 dimples-0.5.6/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.6/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.6/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.6/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.6/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.6/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.6/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.6/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.6/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.6/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.6/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.6/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.6/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.6/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7937 2024-04-23 09:37:33.000000 dimples-0.5.6/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.6/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-24 03:34:20.000000 dimples-0.5.6/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.6/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.6/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.6/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.6/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.6/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.6/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.6/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.6/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.6/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.6/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4561 2024-04-23 09:37:33.000000 dimples-0.5.6/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.6/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.6/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    11821 2024-04-24 03:33:28.000000 dimples-0.5.6/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.6/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.6/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8771 2024-04-23 09:39:58.000000 dimples-0.5.6/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.6/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6444 2024-04-24 03:34:40.000000 dimples-0.5.6/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.6/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     4207 2024-04-24 03:37:25.000000 dimples-0.5.6/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.6/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.6/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.6/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.6/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.6/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.6/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.6/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.6/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.6/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.6/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.6/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.6/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.6/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.6/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.6/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.6/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.6/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.6/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.6/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.6/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.6/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.6/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.6/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.6/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.6/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.6/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.6/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    14595 2024-04-24 03:35:02.000000 dimples-0.5.6/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.6/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.6/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.6/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.6/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.6/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.6/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.6/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.6/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.6/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.6/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.6/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.6/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.6/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.6/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.6/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7406 2024-04-24 04:11:06.000000 dimples-0.5.6/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.6/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.6/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.6/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.6/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.6/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.6/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    17173 2024-04-24 06:39:02.000000 dimples-0.5.6/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4454 2024-04-23 10:00:05.000000 dimples-0.5.6/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-24 03:35:15.000000 dimples-0.5.6/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    13850 2024-04-24 05:59:48.000000 dimples-0.5.6/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5476 2024-04-23 08:44:27.000000 dimples-0.5.6/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9843 2024-04-24 03:38:06.000000 dimples-0.5.6/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.6/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.6/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3832 2024-04-22 16:08:14.000000 dimples-0.5.6/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.6/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.6/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4710 2024-04-23 08:43:02.000000 dimples-0.5.6/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6355 2024-04-23 08:38:51.000000 dimples-0.5.6/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6696 2024-04-23 09:37:33.000000 dimples-0.5.6/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.6/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.6/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-24 06:49:33.000000 dimples-0.5.6/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-24 06:49:33.000000 dimples-0.5.6/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-24 06:37:50.000000 dimples-0.5.6/setup.py
```

### Comparing `dimples-0.5.5/PKG-INFO` & `dimples-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.5
+Version: 0.5.6
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.5/README.md` & `dimples-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/__init__.py` & `dimples-0.5.6/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/__init__.py` & `dimples-0.5.6/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/archivist.py` & `dimples-0.5.6/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/checkpoint.py` & `dimples-0.5.6/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/__init__.py` & `dimples-0.5.6/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/commands.py` & `dimples-0.5.6/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/creator.py` & `dimples-0.5.6/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/group.py` & `dimples-0.5.6/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_expel.py` & `dimples-0.5.6/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_invite.py` & `dimples-0.5.6/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_join.py` & `dimples-0.5.6/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_query.py` & `dimples-0.5.6/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_quit.py` & `dimples-0.5.6/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_reset.py` & `dimples-0.5.6/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/grp_resign.py` & `dimples-0.5.6/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/cpu/handshake.py` & `dimples-0.5.6/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/facebook.py` & `dimples-0.5.6/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/messenger.py` & `dimples-0.5.6/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/network/__init__.py` & `dimples-0.5.6/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/network/session.py` & `dimples-0.5.6/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/network/state.py` & `dimples-0.5.6/dimples/client/network/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,34 +132,38 @@
     def name(self) -> str:
         return self.__name
 
     @property
     def enter_time(self) -> float:
         return self.__time
 
+    # Override
     def __str__(self) -> str:
         return self.__name
 
+    # Override
     def __repr__(self) -> str:
         return self.__name
 
+    # Override
     def __eq__(self, other) -> bool:
         if isinstance(other, SessionState):
             if self is other:
                 return True
             return self.index == other.index
         elif isinstance(other, StateOrder):
             return self.index == other.value
         elif isinstance(other, int):
             return self.index == other
         elif isinstance(other, str):
             return self.__name == other
         else:
             return False
 
+    # Override
     def __ne__(self, other) -> bool:
         if isinstance(other, SessionState):
             if self is other:
                 return False
             return self.index != other.index
         elif isinstance(other, StateOrder):
             return self.index != other.value
```

### Comparing `dimples-0.5.5/dimples/client/network/transition.py` & `dimples-0.5.6/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/packer.py` & `dimples-0.5.6/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/processor.py` & `dimples-0.5.6/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/client/terminal.py` & `dimples-0.5.6/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/__init__.py` & `dimples-0.5.6/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/anonymous.py` & `dimples-0.5.6/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/ans.py` & `dimples-0.5.6/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/archivist.py` & `dimples-0.5.6/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/__init__.py` & `dimples-0.5.6/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/btc.py` & `dimples-0.5.6/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/compatible.py` & `dimples-0.5.6/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/entity.py` & `dimples-0.5.6/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/meta.py` & `dimples-0.5.6/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/compat/network.py` & `dimples-0.5.6/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/dbi/__init__.py` & `dimples-0.5.6/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/dbi/account.py` & `dimples-0.5.6/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/dbi/message.py` & `dimples-0.5.6/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/dbi/session.py` & `dimples-0.5.6/dimples/common/dbi/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,20 @@
     GSP = Identifier(identifier='gsp@everywhere', name='gsp', address=EVERYWHERE)
 
     def __init__(self, identifier: ID, chosen: int):
         super().__init__()
         self.identifier = identifier
         self.chosen = chosen
 
+    # Override
     def __str__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s ID="%s" chosen=%d />' % (clazz, self.identifier, self.chosen)
 
+    # Override
     def __repr__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s ID="%s" chosen=%d />' % (clazz, self.identifier, self.chosen)
 
     @classmethod
     def convert(cls, array: List[Dict[str, Any]]):  # -> List[ProviderInfo]:
         gf = ProviderFactoryManager.general_factory
@@ -90,19 +92,21 @@
             identifier = Station.ANY  # 'station@anywhere'
         self.identifier = identifier
         self.host = host
         self.port = port
         self.provider = provider
         self.chosen = chosen
 
+    # Override
     def __str__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s host="%s" port=%d ID="%s" SP="%s" chosen=%d />' % (clazz, self.host, self.port, self.identifier,
                                                                        self.provider, self.chosen)
 
+    # Override
     def __repr__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s host="%s" port=%d ID="%s" SP="%s" chosen=%d />' % (clazz, self.host, self.port, self.identifier,
                                                                        self.provider, self.chosen)
 
     @classmethod
     def convert(cls, array: List[Dict[str, Any]]):  # -> List[StationInfo]:
```

### Comparing `dimples-0.5.5/dimples/common/facebook.py` & `dimples-0.5.6/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/messenger.py` & `dimples-0.5.6/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/packer.py` & `dimples-0.5.6/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/processer.py` & `dimples-0.5.6/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/__init__.py` & `dimples-0.5.6/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/ans.py` & `dimples-0.5.6/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/block.py` & `dimples-0.5.6/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/handshake.py` & `dimples-0.5.6/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/login.py` & `dimples-0.5.6/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/mute.py` & `dimples-0.5.6/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/protocol/report.py` & `dimples-0.5.6/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/register.py` & `dimples-0.5.6/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/common/session.py` & `dimples-0.5.6/dimples/common/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,18 +110,20 @@
         raise NotImplemented
 
     @abstractmethod
     def set_active(self, active: bool, when: DateTime = None) -> bool:
         """ Update active flag and return True on changed """
         raise NotImplemented
 
+    # Override
     def __str__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
 
+    # Override
     def __repr__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s:%s %s|%s active=%s />' % (clazz, self.key, self.remote_address, self.identifier, self.active)
 
     def queue_message_package(self, msg: ReliableMessage, data: bytes, priority: int = 0) -> bool:
         """
         Pack message into a waiting queue
```

### Comparing `dimples-0.5.5/dimples/conn/__init__.py` & `dimples-0.5.6/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/gate.py` & `dimples-0.5.6/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/gatekeeper.py` & `dimples-0.5.6/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/mars.py` & `dimples-0.5.6/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/mtp.py` & `dimples-0.5.6/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/protocol/__init__.py` & `dimples-0.5.6/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/protocol/mars.py` & `dimples-0.5.6/dimples/conn/protocol/mars.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,20 @@
         self.__data = data
         self.__version = version
         self.__cmd = cmd
         self.__seq = seq
         self.__options = options
         self.__body_length = body_len
 
+    # Override
     def __str__(self) -> str:
         cname = self.__class__.__name__
         return '<%s: %d| cmd=%d, seq=%d, body_len=%d />' % (cname, self.version, self.cmd, self.seq, self.body_length)
 
+    # Override
     def __repr__(self) -> str:
         cname = self.__class__.__name__
         return '<%s: %d| cmd=%d, seq=%d, body_len=%d />' % (cname, self.version, self.cmd, self.seq, self.body_length)
 
     @property
     def data(self) -> bytes:
         return self.__data
@@ -194,19 +196,21 @@
         :return:
         """
         super(NetMsg, self).__init__()
         self.__data = data
         self.__head = head
         self.__body = body
 
+    # Override
     def __str__(self) -> str:
         mod = self.__module__
         cname = self.__class__.__name__
         return '<%s body_len=%d>%s</%s module="%s">' % (cname, self.body_length, self.head, cname, mod)
 
+    # Override
     def __repr__(self) -> str:
         mod = self.__module__
         cname = self.__class__.__name__
         return '<%s body_len=%d>%s</%s module="%s">' % (cname, self.body_length, self.head, cname, mod)
 
     @property
     def data(self) -> bytes:
```

### Comparing `dimples-0.5.5/dimples/conn/protocol/ws.py` & `dimples-0.5.6/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/queue.py` & `dimples-0.5.6/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/seeker.py` & `dimples-0.5.6/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/conn/session.py` & `dimples-0.5.6/dimples/conn/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,24 @@
 
     def __init__(self, remote: Tuple[str, int], sock: Optional[socket.socket], database: SessionDBI):
         super().__init__(remote=remote, sock=sock)
         self.__database = database
         self.__identifier: Optional[ID] = None
         self.__messenger: Optional[weakref.ReferenceType] = None
 
+    # Override
+    def __str__(self) -> str:
+        cname = self.__class__.__name__
+        return '<%s id="%s" remote="%s" key="%s" />' % (cname, self.identifier, self.remote_address, self.key)
+
+    # Override
+    def __repr__(self):
+        cname = self.__class__.__name__
+        return '<%s id="%s" remote="%s" key="%s" />' % (cname, self.identifier, self.remote_address, self.key)
+
     @property  # Override
     def database(self) -> SessionDBI:
         return self.__database
 
     @property  # Override
     def identifier(self) -> Optional[ID]:
         return self.__identifier
```

### Comparing `dimples-0.5.5/dimples/conn/ws.py` & `dimples-0.5.6/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/__init__.py` & `dimples-0.5.6/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/account.py` & `dimples-0.5.6/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/__init__.py` & `dimples-0.5.6/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/base.py` & `dimples-0.5.6/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/document.py` & `dimples-0.5.6/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/group.py` & `dimples-0.5.6/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/group_history.py` & `dimples-0.5.6/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/group_keys.py` & `dimples-0.5.6/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/login.py` & `dimples-0.5.6/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/meta.py` & `dimples-0.5.6/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/private.py` & `dimples-0.5.6/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/station.py` & `dimples-0.5.6/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/dos/user.py` & `dimples-0.5.6/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/message.py` & `dimples-0.5.6/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/session.py` & `dimples-0.5.6/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_cipherkey.py` & `dimples-0.5.6/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_document.py` & `dimples-0.5.6/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_group.py` & `dimples-0.5.6/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_group_history.py` & `dimples-0.5.6/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_group_keys.py` & `dimples-0.5.6/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_login.py` & `dimples-0.5.6/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_message.py` & `dimples-0.5.6/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_meta.py` & `dimples-0.5.6/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_private.py` & `dimples-0.5.6/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_station.py` & `dimples-0.5.6/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/database/t_user.py` & `dimples-0.5.6/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/edge/__init__.py` & `dimples-0.5.6/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/edge/octopus.py` & `dimples-0.5.6/dimples/edge/octopus.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/edge/shared.py` & `dimples-0.5.6/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/edge/start.py` & `dimples-0.5.6/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/__init__.py` & `dimples-0.5.6/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/admin.py` & `dimples-0.5.6/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/builder.py` & `dimples-0.5.6/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/delegate.py` & `dimples-0.5.6/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/emitter.py` & `dimples-0.5.6/dimples/group/emitter.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/helper.py` & `dimples-0.5.6/dimples/group/helper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/manager.py` & `dimples-0.5.6/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/group/packer.py` & `dimples-0.5.6/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/register/__init__.py` & `dimples-0.5.6/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/register/base.py` & `dimples-0.5.6/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/register/ext.py` & `dimples-0.5.6/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/register/run.py` & `dimples-0.5.6/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/register/shared.py` & `dimples-0.5.6/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/__init__.py` & `dimples-0.5.6/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/archivist.py` & `dimples-0.5.6/dimples/server/archivist.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from dimsdk import Station
 
 from ..common import AccountDBI
 from ..common import CommonArchivist
 from ..common import CommonFacebook, CommonMessenger
 from ..common import StationInfo
 
-from .dispatcher import Dispatcher
 from .session_center import SessionCenter
 
 
 def get_facebook(archivist: CommonArchivist):
     facebook = archivist.facebook
     if facebook is not None:
         assert isinstance(facebook, CommonFacebook), 'facebook error: %s' % facebook
@@ -58,14 +57,19 @@
 def get_messenger(archivist: CommonArchivist):
     messenger = archivist.messenger
     if messenger is not None:
         assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
     return messenger
 
 
+def get_dispatcher():
+    from .dispatcher import Dispatcher
+    return Dispatcher()
+
+
 class ServerArchivist(CommonArchivist, ABC):
 
     # each respond will be expired after 10 minutes
     RESPOND_EXPIRES = 600.0  # seconds
 
     def __init__(self, database: AccountDBI):
         super().__init__(database=database)
@@ -91,15 +95,15 @@
                 self.__neighbors = neighbors
                 self.__expires = now.timestamp + 128
             return self.__neighbors
 
     @property
     def all_stations(self) -> List[StationInfo]:
         """ get stations from database """
-        dispatcher = Dispatcher()
+        dispatcher = get_dispatcher()
         db = dispatcher.sdb
         # TODO: get chosen provider
         providers = db.all_providers()
         assert len(providers) > 0, 'service provider not found'
         gsp = providers[0].identifier
         return db.all_stations(provider=gsp)
 
@@ -132,15 +136,15 @@
         sid = facebook.current_user.identifier
         env = Envelope.create(sender=sid, receiver=Station.EVERY)
         i_msg = InstantMessage.create(head=env, body=command)
         # pack & deliver message
         s_msg = messenger.encrypt_message(msg=i_msg)
         r_msg = messenger.sign_message(msg=s_msg)
         # dispatch
-        dispatcher = Dispatcher()
+        dispatcher = get_dispatcher()
         neighbors = self.all_neighbors
         # avoid the new recipients redirect it to same targets
         r_msg['recipients'] = ID.revert(neighbors)
         for receiver in neighbors:
             if receiver == sid:
                 self.debug(msg='skip cycled message: %s -> %s' % (sid, receiver))
                 continue
```

### Comparing `dimples-0.5.5/dimples/server/cpu/__init__.py` & `dimples-0.5.6/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/cpu/ans.py` & `dimples-0.5.6/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/cpu/document.py` & `dimples-0.5.6/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/cpu/handshake.py` & `dimples-0.5.6/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/cpu/login.py` & `dimples-0.5.6/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/cpu/report.py` & `dimples-0.5.6/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/dispatcher.py` & `dimples-0.5.6/dimples/server/dispatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,28 +28,30 @@
     ~~~~~~~~~~~~~~~~~~
 
     A dispatcher to decide which way to deliver message.
 """
 
 import threading
 from abc import ABC, abstractmethod
-from typing import Optional, List
+from typing import Optional, Set, List
 
-from dimsdk import EntityType, ID
+from dimsdk import EntityType, ID, EVERYONE
+from dimsdk import Station
 from dimsdk import Content, ReceiptCommand
 from dimsdk import ReliableMessage
 
-from ..utils import Singleton, Logging, Runner, Daemon
+from ..utils import Singleton, Log, Logging, Runner, Daemon
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
 from ..common import ReliableMessageDBI
 from ..common import LoginCommand
 
 from .session_center import SessionCenter
 from .push import PushCenter
+from .archivist import ServerArchivist
 
 
 class MessageDeliver(ABC):
     """ Delegate for deliver message """
 
     @abstractmethod
     def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
@@ -60,15 +62,15 @@
         :param receiver: message destination
         :return: responses
         """
         raise NotImplemented
 
 
 @Singleton
-class Dispatcher(MessageDeliver):
+class Dispatcher(MessageDeliver, Logging):
 
     def __init__(self):
         super().__init__()
         self.__facebook: Optional[CommonFacebook] = None
         self.__mdb: Optional[MessageDBI] = None
         self.__sdb: Optional[SessionDBI] = None
         # actually deliver worker
@@ -143,15 +145,19 @@
     #   Deliver
     #
 
     # Override
     def deliver_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
         """ Deliver message to destination """
         worker = self.deliver_worker
-        if receiver.type == EntityType.STATION:
+        if receiver.is_group:
+            # broadcast message to neighbor stations
+            # e.g.: 'stations@everywhere', 'everyone@everywhere'
+            return self.__deliver_group_message(msg=msg, receiver=receiver)
+        elif receiver.type == EntityType.STATION:
             # message to other stations
             # station won't roam to other station, so just push for it directly
             responses = worker.redirect_message(msg=msg, neighbor=receiver)
         elif receiver.type == EntityType.BOT:
             # message to a bot
             # save message before trying to push
             self.__save_reliable_message(msg=msg, receiver=receiver)
@@ -177,14 +183,78 @@
             text = 'Message received.'
             res = ReceiptCommand.create(text=text, envelope=msg.envelope)
             return [res]
         else:
             # message delivered
             return responses
 
+    def __deliver_group_message(self, msg: ReliableMessage, receiver: ID) -> List[Content]:
+        if receiver == Station.EVERY or receiver == EVERYONE:
+            # broadcast message to neighbor stations
+            # e.g.: 'stations@everywhere', 'everyone@everywhere'
+            archivist = self.facebook.archivist
+            assert isinstance(archivist, ServerArchivist)
+            candidates = archivist.all_neighbors
+            if len(candidates) == 0:
+                self.warning(msg='failed to get neighbors: %s' % receiver)
+                return []
+            self.info(msg='forward to neighbor stations: %s -> %s' % (receiver, candidates))
+            return self.__broadcast_message(msg=msg, receiver=receiver, neighbors=candidates)
+        else:
+            self.warning(msg='unknown group: %s' % receiver)
+            text = 'Group message not allow for this station'
+            res = ReceiptCommand.create(text=text, envelope=msg.envelope)
+            return [res]
+
+    def __broadcast_message(self, msg: ReliableMessage, receiver: ID, neighbors: Set[ID]) -> List[Content]:
+        #
+        #  0. check recipients
+        #
+        new_recipients = neighbors.copy()
+        old_recipients = msg.get('recipients')
+        if old_recipients is None:
+            all_recipients = []
+        else:
+            all_recipients = ID.convert(old_recipients)
+            # check duplicated
+            self.info(msg='discard recipients: %s, new recipients: %s' % (old_recipients, new_recipients))
+            for item in all_recipients:
+                new_recipients.discard(item)
+            if len(new_recipients) == 0:
+                self.info(msg='new recipients empty: %s => %s' % (receiver, neighbors))
+                return []
+        self.info(msg='append new recipients: %s, %s => %s' % (receiver, new_recipients, all_recipients))
+        for item in new_recipients:
+            all_recipients.append(item)
+        # avoid the new recipients redirect it to same targets
+        msg['recipients'] = ID.revert(all_recipients)
+        #
+        #  1. push to neighbor stations directly
+        #
+        indirect_neighbors = set()
+        for target in new_recipients:
+            if session_push(msg=msg, receiver=target) == 0:
+                indirect_neighbors.add(target)
+        if len(indirect_neighbors) > 0:
+            for item in indirect_neighbors:
+                all_recipients.remove(item)
+            msg['recipients'] = ID.revert(all_recipients)
+        #
+        #  2. push to other neighbor stations via station bridge
+        #
+        worker = self.deliver_worker
+        worker.redirect_message(msg=msg, neighbor=None)
+        #
+        #  OK
+        #
+        text = 'Message forwarded.'
+        cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
+        cmd['recipients'] = ID.revert(new_recipients)
+        return [cmd]
+
     def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         if receiver.type == EntityType.STATION or msg.sender.type == EntityType.STATION:
             # no need to save station message
             return False
         elif msg.receiver.is_broadcast:
             # no need to save broadcast message
             return False
@@ -301,15 +371,15 @@
         if roaming is None:
             # login command not found
             # return None to tell the push center to push notification for it.
             return None
         # 3. redirect message to roaming station
         return self.redirect_message(msg=msg, neighbor=roaming)
 
-    def redirect_message(self, msg: ReliableMessage, neighbor: ID) -> Optional[List[Content]]:
+    def redirect_message(self, msg: ReliableMessage, neighbor: Optional[ID]) -> Optional[List[Content]]:
         """
         Redirect message to neighbor station
 
         :param msg:      network message
         :param neighbor: neighbor station
         :return: responses
         """
@@ -321,47 +391,57 @@
         assert current.type == EntityType.STATION, 'current station ID error: %s' % current
         if neighbor == current:
             self.debug(msg='same destination: %s, msg %s => %s' % (neighbor, msg.sender, msg.receiver))
             # the user is roaming to current station, but it's not online now
             # return None to tell the push center to push notification for it.
             return None
         # 1. try to push message to neighbor station directly
-        if session_push(msg=msg, receiver=neighbor) > 0:
+        if neighbor is not None and session_push(msg=msg, receiver=neighbor) > 0:
             text = 'Message redirected.'
             cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
             cmd['neighbor'] = str(neighbor)
             return [cmd]
         # 2. push message to bridge
         return bridge_message(msg=msg, neighbor=neighbor, bridge=current)
 
 
-def bridge_message(msg: ReliableMessage, neighbor: ID, bridge: ID) -> Optional[List[Content]]:
+def bridge_message(msg: ReliableMessage, neighbor: Optional[ID], bridge: ID) -> List[Content]:
     """
     Redirect message to neighbor station via the station bridge
+    if neighbor is None, try to broadcast
 
     :param msg:      network message
     :param neighbor: roaming station
     :param bridge:   current station
     :return: responses
     """
     # NOTE: the messenger will serialize this message immediately, so
     #       we don't need to clone this dictionary to avoid 'neighbor'
     #       be changed to another value before pushing to the bridge.
     # clone = msg.copy_dictionary()
     # msg = ReliableMessage.parse(msg=clone)
-    msg['neighbor'] = str(neighbor)
-    if session_push(msg=msg, receiver=bridge) > 0:
-        text = 'Message redirected.'
-        cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
-        cmd['neighbor'] = str(neighbor)
-        return [cmd]
+    if neighbor is None:
+        # broadcast to all neighbor stations
+        # except that ones already in msg['recipients']
+        session_push(msg=msg, receiver=bridge)
+        # no need to respond receipt for this broadcast message
+        return []
     else:
+        assert neighbor != bridge, 'cannot bridge cycled message: %s' % neighbor
+        msg['neighbor'] = str(neighbor)
+    # push to the bridge
+    if session_push(msg=msg, receiver=bridge) == 0:
         # station bridge not found
-        # return an empty array to avoid calling push center
+        Log.warning(msg='failed to push message to bridge: %s, drop message: %s -> %s'
+                        % (bridge, msg.sender, msg.receiver))
         return []
+    text = 'Message redirected via station bridge.'
+    cmd = ReceiptCommand.create(text=text, envelope=msg.envelope)
+    cmd['neighbor'] = str(neighbor)
+    return [cmd]
 
 
 def session_push(msg: ReliableMessage, receiver: ID) -> int:
     """ push message via active session(s) of receiver """
     success = 0
     center = SessionCenter()
     active_sessions = center.active_sessions(identifier=receiver)
```

### Comparing `dimples-0.5.5/dimples/server/messenger.py` & `dimples-0.5.6/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/packer.py` & `dimples-0.5.6/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/processor.py` & `dimples-0.5.6/dimples/server/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 from .cpu import ReportCommandProcessor
 from .cpu import AnsCommandProcessor
 
 from .cpu import DocumentCommandProcessor
 
 from .packer import FilterManager
 from .dispatcher import Dispatcher
-from .archivist import ServerArchivist
 
 
 class ServerMessageProcessor(CommonMessageProcessor):
 
     @property
     def messenger(self) -> CommonMessenger:
         transceiver = super().messenger
@@ -191,57 +190,26 @@
             # e.g.: 'archivist@anywhere', 'announcer@anywhere', 'monitor@anywhere', ...
             name = receiver.name
             assert name is not None and name != 'station' and name != 'anyone', 'receiver error: %s' % receiver
             bot = AnsCommandProcessor.ans_id(name=name)
             if bot is None:
                 self.warning(msg='failed to get receiver: %s' % receiver)
                 return False
-            candidates = set()
-            candidates.add(bot)
-            self.info(msg='forward to station bot: %s -> %s' % (name, bot))
-        elif receiver == Station.EVERY or receiver == EVERYONE:
-            # broadcast message to neighbor stations
-            # e.g.: 'stations@everywhere', 'everyone@everywhere'
-            archivist = self.facebook.archivist
-            assert isinstance(archivist, ServerArchivist)
-            candidates = archivist.all_neighbors
-            if len(candidates) == 0:
-                self.warning(msg='failed to get neighbors: %s' % receiver)
+            elif bot == sender:
+                self.warning(msg='skip cycled message: %s -> %s' % (sender, receiver))
                 return False
-            self.info(msg='forward to neighbor stations: %s -> %s' % (receiver, candidates))
-        else:
-            self.warning(msg='unknown receiver: %s' % receiver)
-            return False
-        # check recipients
-        new_recipients = candidates.copy()
-        old_recipients = msg.get('recipients')
-        if old_recipients is None:
-            all_recipients = []
-        else:
-            all_recipients = ID.convert(old_recipients)
-            # check duplicated
-            self.info(msg='discard recipients: %s, new recipients: %s' % (old_recipients, new_recipients))
-            for item in all_recipients:
-                new_recipients.discard(item)
-            if len(new_recipients) == 0:
-                self.info(msg='new recipients empty: %s => %s' % (receiver, candidates))
+            elif bot == station:
+                self.warning(msg='skip current station: %s -> %s' % (sender, receiver))
                 return False
-        self.info(msg='append new recipients: %s, %s => %s' % (receiver, new_recipients, all_recipients))
-        for item in new_recipients:
-            all_recipients.append(item)
-        # avoid the new recipients redirect it to same targets
-        msg['recipients'] = ID.revert(all_recipients)
-        # dispatch
-        dispatcher = Dispatcher()
-        for target in new_recipients:
-            if target == sender or target == station:
-                self.info(msg='skip cycled message: %s -> %s, %s' % (sender, receiver, target))
             else:
-                dispatcher.deliver_message(msg=msg, receiver=target)
-        return True
+                self.info(msg='forward to bot: %s -> %s' % (name, bot))
+                receiver = bot
+        # deliver by dispatcher
+        dispatcher = Dispatcher()
+        dispatcher.deliver_message(msg=msg, receiver=receiver)
 
     def _split_group_message(self, msg: ReliableMessage, station: ID):
         """ redirect group message to assistant """
         sender = msg.sender
         receiver = msg.receiver
         self.error(msg='group message should not send to station: %s, %s -> %s' % (station, sender, receiver))
```

### Comparing `dimples-0.5.5/dimples/server/push.py` & `dimples-0.5.6/dimples/server/push.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/session.py` & `dimples-0.5.6/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/session_center.py` & `dimples-0.5.6/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/server/trace.py` & `dimples-0.5.6/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/station/__init__.py` & `dimples-0.5.6/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/station/handler.py` & `dimples-0.5.6/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/station/shared.py` & `dimples-0.5.6/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/station/start.py` & `dimples-0.5.6/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/utils/__init__.py` & `dimples-0.5.6/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/utils/cache.py` & `dimples-0.5.6/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/utils/config.py` & `dimples-0.5.6/dimples/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,20 @@
         if name is not None:
             self['name'] = name
         if host is not None:
             self['host'] = host
         if port > 0:
             self['port'] = port
 
+    # Override
     def __str__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s host="%s" port=%d name="%s" />' % (clazz, self.host, self.port, self.name)
 
+    # Override
     def __repr__(self) -> str:
         clazz = self.__class__.__name__
         return '<%s host="%s" port=%d name="%s" />' % (clazz, self.host, self.port, self.name)
 
     @property
     def name(self) -> str:
         return self.get('name')
```

### Comparing `dimples-0.5.5/dimples/utils/dos.py` & `dimples-0.5.6/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/utils/log.py` & `dimples-0.5.6/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples/utils/singleton.py` & `dimples-0.5.6/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/dimples.egg-info/PKG-INFO` & `dimples-0.5.6/dimples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.5
+Version: 0.5.6
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.5/dimples.egg-info/SOURCES.txt` & `dimples-0.5.6/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.5.5/setup.py` & `dimples-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.5.5'
+__version__ = '0.5.6'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

