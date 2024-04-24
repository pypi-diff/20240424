# Comparing `tmp/dimples-0.5.3.tar.gz` & `tmp/dimples-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.5.3.tar", last modified: Tue Apr 16 07:18:12 2024, max compression
+gzip compressed data, was "dist/dimples-0.5.5.tar", last modified: Tue Apr 23 09:11:37 2024, max compression
```

## Comparing `dimples-0.5.3.tar` & `dimples-0.5.5.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-16 07:18:12.000000 dimples-0.5.3/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.3/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.3/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.3/dimples/client/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.3/dimples/client/archivist.py
--rw-r--r--   0 moky       (501) staff       (20)     3862 2023-12-05 04:21:35.000000 dimples-0.5.3/dimples/client/checkpoint.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.3/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.3/dimples/client/cpu/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.3/dimples/client/cpu/creator.py
--rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.3/dimples/client/cpu/group.py
--rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.3/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.3/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.3/dimples/client/cpu/grp_join.py
--rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.3/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.3/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.3/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.3/dimples/client/cpu/grp_resign.py
--rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.3/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.3/dimples/client/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.3/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.3/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6632 2024-03-07 09:27:13.000000 dimples-0.5.3/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8578 2024-03-07 09:39:13.000000 dimples-0.5.3/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.3/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.3/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.3/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5494 2024-03-06 17:56:47.000000 dimples-0.5.3/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.3/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.3/dimples/common/anonymous.py
--rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.3/dimples/common/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.3/dimples/common/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/compat/
--rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.3/dimples/common/compat/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.3/dimples/common/compat/btc.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.3/dimples/common/compat/compatible.py
--rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.3/dimples/common/compat/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.3/dimples/common/compat/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.3/dimples/common/compat/network.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.3/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.3/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.3/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.5.3/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.3/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-16 06:12:16.000000 dimples-0.5.3/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.3/dimples/common/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.3/dimples/common/processer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.3/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.3/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.3/dimples/common/protocol/block.py
--rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.3/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.3/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.3/dimples/common/protocol/mute.py
--rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.3/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.3/dimples/common/register.py
--rw-r--r--   0 moky       (501) staff       (20)     4531 2023-10-13 16:11:34.000000 dimples-0.5.3/dimples/common/session.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.3/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.3/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)    11821 2024-03-13 10:54:50.000000 dimples-0.5.3/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.3/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.3/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.3/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     6444 2023-11-08 09:04:27.000000 dimples-0.5.3/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.3/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     3819 2023-09-05 04:47:59.000000 dimples-0.5.3/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.3/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.3/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.3/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.3/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.3/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.3/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.3/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.3/dimples/database/dos/group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.3/dimples/database/dos/group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.3/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.3/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.3/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.3/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.3/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.3/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.3/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.3/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.3/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.3/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.3/dimples/database/t_group_history.py
--rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.3/dimples/database/t_group_keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.3/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.3/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.3/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.3/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.3/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.3/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    14571 2024-03-02 09:28:05.000000 dimples-0.5.3/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.3/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.3/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/group/
--rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.3/dimples/group/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.3/dimples/group/admin.py
--rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.3/dimples/group/builder.py
--rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.3/dimples/group/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.3/dimples/group/emitter.py
--rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.3/dimples/group/helper.py
--rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.3/dimples/group/manager.py
--rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.3/dimples/group/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.3/dimples/register/base.py
--rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.3/dimples/register/ext.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.3/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.3/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.3/dimples/server/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7346 2024-02-18 04:20:32.000000 dimples-0.5.3/dimples/server/archivist.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.3/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.3/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.3/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.3/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.3/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.3/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13467 2024-03-01 07:38:11.000000 dimples-0.5.3/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)     4454 2024-02-17 18:19:10.000000 dimples-0.5.3/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-16 07:12:40.000000 dimples-0.5.3/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)    15437 2024-04-16 06:41:33.000000 dimples-0.5.3/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5502 2024-03-01 07:47:10.000000 dimples-0.5.3/dimples/server/push.py
--rw-r--r--   0 moky       (501) staff       (20)     9843 2024-03-13 14:34:33.000000 dimples-0.5.3/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/server/session_center.py
--rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.3/dimples/server/trace.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.3/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3832 2023-12-05 08:43:48.000000 dimples-0.5.3/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.3/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.3/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     4692 2023-12-23 05:16:03.000000 dimples-0.5.3/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6324 2024-03-03 09:21:57.000000 dimples-0.5.3/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-29 14:16:57.000000 dimples-0.5.3/dimples/utils/config.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.3/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.3/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-16 07:18:12.000000 dimples-0.5.3/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-16 07:18:11.000000 dimples-0.5.3/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-16 07:18:12.000000 dimples-0.5.3/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-16 07:09:58.000000 dimples-0.5.3/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-23 09:11:37.000000 dimples-0.5.5/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.5.5/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     8913 2024-04-11 15:45:18.000000 dimples-0.5.5/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1977 2023-12-05 04:36:14.000000 dimples-0.5.5/dimples/client/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10796 2023-12-05 08:35:38.000000 dimples-0.5.5/dimples/client/archivist.py
+-rw-r--r--   0 moky       (501) staff       (20)     3862 2023-12-05 04:21:35.000000 dimples-0.5.5/dimples/client/checkpoint.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2287 2023-10-29 13:43:35.000000 dimples-0.5.5/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     1946 2023-10-29 13:45:31.000000 dimples-0.5.5/dimples/client/cpu/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     4803 2023-10-29 13:43:46.000000 dimples-0.5.5/dimples/client/cpu/creator.py
+-rw-r--r--   0 moky       (501) staff       (20)     8885 2024-03-06 18:05:23.000000 dimples-0.5.5/dimples/client/cpu/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     2167 2023-10-14 07:50:57.000000 dimples-0.5.5/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     5889 2023-10-19 02:32:49.000000 dimples-0.5.5/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3962 2023-10-19 02:35:10.000000 dimples-0.5.5/dimples/client/cpu/grp_join.py
+-rw-r--r--   0 moky       (501) staff       (20)     4141 2023-12-05 04:35:16.000000 dimples-0.5.5/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     4352 2023-10-19 02:33:14.000000 dimples-0.5.5/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     5669 2023-10-29 13:35:51.000000 dimples-0.5.5/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     4050 2023-10-19 02:35:32.000000 dimples-0.5.5/dimples/client/cpu/grp_resign.py
+-rw-r--r--   0 moky       (501) staff       (20)     5166 2023-10-13 09:48:02.000000 dimples-0.5.5/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     6196 2023-12-05 04:11:38.000000 dimples-0.5.5/dimples/client/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8331 2024-03-17 08:54:03.000000 dimples-0.5.5/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.5.5/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6624 2024-04-23 08:44:53.000000 dimples-0.5.5/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8578 2024-03-07 09:39:13.000000 dimples-0.5.5/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9501 2024-03-06 17:49:03.000000 dimples-0.5.5/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     9140 2023-12-24 14:13:08.000000 dimples-0.5.5/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6021 2024-04-11 15:43:51.000000 dimples-0.5.5/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5560 2024-04-23 08:43:31.000000 dimples-0.5.5/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2652 2024-04-11 16:03:38.000000 dimples-0.5.5/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3520 2023-10-19 02:46:00.000000 dimples-0.5.5/dimples/common/anonymous.py
+-rw-r--r--   0 moky       (501) staff       (20)     5771 2023-10-13 10:02:36.000000 dimples-0.5.5/dimples/common/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     7382 2023-12-05 08:37:45.000000 dimples-0.5.5/dimples/common/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/compat/
+-rw-r--r--   0 moky       (501) staff       (20)     2751 2023-10-13 16:15:07.000000 dimples-0.5.5/dimples/common/compat/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3806 2023-10-15 03:29:15.000000 dimples-0.5.5/dimples/common/compat/btc.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-15 03:31:01.000000 dimples-0.5.5/dimples/common/compat/compatible.py
+-rw-r--r--   0 moky       (501) staff       (20)     2572 2023-10-13 10:09:19.000000 dimples-0.5.5/dimples/common/compat/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6277 2023-10-17 15:21:36.000000 dimples-0.5.5/dimples/common/compat/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     6192 2023-10-13 10:09:24.000000 dimples-0.5.5/dimples/common/compat/network.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2146 2023-10-15 04:04:22.000000 dimples-0.5.5/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7454 2023-10-29 10:52:28.000000 dimples-0.5.5/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2697 2023-10-15 04:03:21.000000 dimples-0.5.5/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.5.5/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8297 2023-12-05 04:13:00.000000 dimples-0.5.5/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     8860 2024-04-16 06:12:16.000000 dimples-0.5.5/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     8480 2024-04-16 06:08:27.000000 dimples-0.5.5/dimples/common/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     2965 2024-04-11 15:41:49.000000 dimples-0.5.5/dimples/common/processer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2695 2023-10-29 10:59:58.000000 dimples-0.5.5/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3426 2023-10-13 12:48:25.000000 dimples-0.5.5/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     2611 2023-10-29 11:52:51.000000 dimples-0.5.5/dimples/common/protocol/block.py
+-rw-r--r--   0 moky       (501) staff       (20)     5211 2023-10-13 12:47:14.000000 dimples-0.5.5/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4897 2023-12-03 07:02:16.000000 dimples-0.5.5/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2023-10-29 11:53:00.000000 dimples-0.5.5/dimples/common/protocol/mute.py
+-rw-r--r--   0 moky       (501) staff       (20)     2620 2023-10-13 12:45:16.000000 dimples-0.5.5/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     6286 2023-10-18 17:01:36.000000 dimples-0.5.5/dimples/common/register.py
+-rw-r--r--   0 moky       (501) staff       (20)     4531 2023-10-13 16:11:34.000000 dimples-0.5.5/dimples/common/session.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.5.5/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10672 2024-03-13 10:42:57.000000 dimples-0.5.5/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)    11821 2024-04-23 08:42:23.000000 dimples-0.5.5/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10758 2024-03-06 16:34:07.000000 dimples-0.5.5/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7968 2024-03-06 16:34:02.000000 dimples-0.5.5/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8968 2024-03-06 18:07:41.000000 dimples-0.5.5/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     6444 2023-11-08 09:04:27.000000 dimples-0.5.5/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.5.5/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     3819 2023-09-05 04:47:59.000000 dimples-0.5.5/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     7820 2024-03-06 16:54:07.000000 dimples-0.5.5/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2812 2023-10-15 04:57:38.000000 dimples-0.5.5/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7771 2023-10-29 12:57:30.000000 dimples-0.5.5/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1949 2023-10-14 04:19:29.000000 dimples-0.5.5/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4996 2023-10-15 05:40:53.000000 dimples-0.5.5/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     6298 2023-10-29 15:53:53.000000 dimples-0.5.5/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5179 2023-10-15 05:14:45.000000 dimples-0.5.5/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5947 2023-10-15 05:30:27.000000 dimples-0.5.5/dimples/database/dos/group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     2773 2023-10-15 05:43:45.000000 dimples-0.5.5/dimples/database/dos/group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     3085 2023-10-15 05:43:56.000000 dimples-0.5.5/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2630 2023-10-15 05:44:04.000000 dimples-0.5.5/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5523 2023-10-15 05:44:19.000000 dimples-0.5.5/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     7920 2023-10-15 05:44:30.000000 dimples-0.5.5/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     2909 2023-10-15 05:44:37.000000 dimples-0.5.5/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3652 2023-08-21 05:21:20.000000 dimples-0.5.5/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.5.5/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     3116 2023-10-14 04:45:57.000000 dimples-0.5.5/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     4105 2023-10-29 12:54:59.000000 dimples-0.5.5/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     6451 2023-10-14 04:47:41.000000 dimples-0.5.5/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     5703 2023-10-14 12:54:46.000000 dimples-0.5.5/dimples/database/t_group_history.py
+-rw-r--r--   0 moky       (501) staff       (20)     4241 2023-10-14 04:48:13.000000 dimples-0.5.5/dimples/database/t_group_keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4192 2023-12-20 09:34:49.000000 dimples-0.5.5/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     4383 2023-10-14 04:48:54.000000 dimples-0.5.5/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3720 2023-10-14 04:49:08.000000 dimples-0.5.5/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5849 2023-10-14 04:49:32.000000 dimples-0.5.5/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6591 2023-10-14 04:49:49.000000 dimples-0.5.5/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     3506 2023-10-14 04:50:25.000000 dimples-0.5.5/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    14595 2024-04-23 08:44:08.000000 dimples-0.5.5/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     6019 2023-12-05 08:47:31.000000 dimples-0.5.5/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2728 2023-12-05 08:14:04.000000 dimples-0.5.5/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/group/
+-rw-r--r--   0 moky       (501) staff       (20)     1874 2023-10-18 14:55:15.000000 dimples-0.5.5/dimples/group/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6123 2023-10-29 13:04:28.000000 dimples-0.5.5/dimples/group/admin.py
+-rw-r--r--   0 moky       (501) staff       (20)     7083 2023-10-29 14:45:28.000000 dimples-0.5.5/dimples/group/builder.py
+-rw-r--r--   0 moky       (501) staff       (20)     7017 2023-12-05 09:07:02.000000 dimples-0.5.5/dimples/group/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)    12170 2024-04-16 07:10:33.000000 dimples-0.5.5/dimples/group/emitter.py
+-rw-r--r--   0 moky       (501) staff       (20)     5167 2023-12-05 06:47:41.000000 dimples-0.5.5/dimples/group/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)    16233 2024-03-06 18:13:16.000000 dimples-0.5.5/dimples/group/manager.py
+-rw-r--r--   0 moky       (501) staff       (20)     5054 2023-10-18 08:14:29.000000 dimples-0.5.5/dimples/group/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10539 2023-10-29 13:30:09.000000 dimples-0.5.5/dimples/register/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     8152 2023-10-15 03:24:30.000000 dimples-0.5.5/dimples/register/ext.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3832 2023-10-15 03:24:14.000000 dimples-0.5.5/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     4115 2023-10-15 03:16:54.000000 dimples-0.5.5/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2448 2024-02-17 14:40:02.000000 dimples-0.5.5/dimples/server/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7346 2024-02-18 04:20:32.000000 dimples-0.5.5/dimples/server/archivist.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1779 2023-07-05 16:57:44.000000 dimples-0.5.5/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2723 2023-10-17 15:27:50.000000 dimples-0.5.5/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4811 2024-03-06 18:13:38.000000 dimples-0.5.5/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2024-04-11 16:23:39.000000 dimples-0.5.5/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4222 2024-04-11 16:23:49.000000 dimples-0.5.5/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     3533 2023-12-21 13:30:57.000000 dimples-0.5.5/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13438 2024-04-23 08:43:17.000000 dimples-0.5.5/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)     4454 2024-02-17 18:19:10.000000 dimples-0.5.5/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6548 2024-04-16 07:12:40.000000 dimples-0.5.5/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)    15437 2024-04-16 06:41:33.000000 dimples-0.5.5/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5476 2024-04-23 08:44:27.000000 dimples-0.5.5/dimples/server/push.py
+-rw-r--r--   0 moky       (501) staff       (20)     9843 2024-03-13 14:34:33.000000 dimples-0.5.5/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/server/session_center.py
+-rw-r--r--   0 moky       (501) staff       (20)    10121 2023-12-05 04:21:35.000000 dimples-0.5.5/dimples/server/trace.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.5.5/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3832 2024-04-22 16:08:14.000000 dimples-0.5.5/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7381 2024-02-17 14:40:46.000000 dimples-0.5.5/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3708 2023-12-05 08:15:24.000000 dimples-0.5.5/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     4710 2024-04-23 08:43:02.000000 dimples-0.5.5/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6355 2024-04-23 08:38:51.000000 dimples-0.5.5/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     6666 2023-10-29 14:16:57.000000 dimples-0.5.5/dimples/utils/config.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2761 2023-10-13 09:39:33.000000 dimples-0.5.5/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.5.5/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3982 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      104 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2024-04-23 09:11:37.000000 dimples-0.5.5/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:11:37.000000 dimples-0.5.5/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1671 2024-04-23 08:45:20.000000 dimples-0.5.5/setup.py
```

### Comparing `dimples-0.5.3/PKG-INFO` & `dimples-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.3
+Version: 0.5.5
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.3/README.md` & `dimples-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/__init__.py` & `dimples-0.5.5/dimples/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/__init__.py` & `dimples-0.5.5/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/archivist.py` & `dimples-0.5.5/dimples/client/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/checkpoint.py` & `dimples-0.5.5/dimples/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/__init__.py` & `dimples-0.5.5/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/commands.py` & `dimples-0.5.5/dimples/client/cpu/commands.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/creator.py` & `dimples-0.5.5/dimples/client/cpu/creator.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/group.py` & `dimples-0.5.5/dimples/client/cpu/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_expel.py` & `dimples-0.5.5/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_invite.py` & `dimples-0.5.5/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_join.py` & `dimples-0.5.5/dimples/client/cpu/grp_join.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_query.py` & `dimples-0.5.5/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_quit.py` & `dimples-0.5.5/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_reset.py` & `dimples-0.5.5/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/grp_resign.py` & `dimples-0.5.5/dimples/client/cpu/grp_resign.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/cpu/handshake.py` & `dimples-0.5.5/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/facebook.py` & `dimples-0.5.5/dimples/client/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/messenger.py` & `dimples-0.5.5/dimples/client/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/network/__init__.py` & `dimples-0.5.5/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/network/session.py` & `dimples-0.5.5/dimples/client/network/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 """
 
 import traceback
 from typing import Optional, List
 
 from dimsdk import Station
 
-from startrek.fsm import Daemon
 from startrek.fsm import Delegate as StateDelegate
 from startrek import Docker, DockerStatus
 from startrek import Arrival
 
+from ...utils import Daemon
 from ...common import SessionDBI
 from ...conn import BaseSession
 from ...conn import MTPStreamArrival
 
 from .state import StateMachine, SessionState
 
 
@@ -80,15 +80,15 @@
         super().__init__(remote=(station.host, station.port), sock=None, database=database)
         self.__station = station
         # session key
         self.__key: Optional[str] = None
         # state machine
         self.__fsm = StateMachine(session=self)
         # background thread to drive gate & hub processing
-        self.__daemon = Daemon(target=self.run)
+        self.__daemon = Daemon(target=self)
 
     @property
     def station(self) -> Station:
         return self.__station
 
     @property
     def key(self) -> Optional[str]:
```

### Comparing `dimples-0.5.3/dimples/client/network/state.py` & `dimples-0.5.5/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/network/transition.py` & `dimples-0.5.5/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/packer.py` & `dimples-0.5.5/dimples/client/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/processor.py` & `dimples-0.5.5/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/client/terminal.py` & `dimples-0.5.5/dimples/client/terminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,19 @@
 """
     Terminal
     ~~~~~~~~
 
     Client
 """
 
-import threading
 import time
 
 from dimples import EntityType
 
-from ..utils import Runner, Logging
+from ..utils import Runner, Daemon, Logging
 from ..utils import StateDelegate
 
 from .network import ClientSession
 from .network import StateMachine, SessionState
 from .network.state import StateOrder
 
 from .messenger import ClientMessenger
@@ -55,14 +54,15 @@
 class Terminal(Runner, DeviceMixin, Logging, StateDelegate):
 
     def __init__(self, messenger: ClientMessenger):
         super().__init__(interval=60)
         self.__messenger = messenger
         # default online time
         self.__last_time = time.time()
+        self.__daemon = Daemon(target=self)
 
     @property
     def messenger(self) -> ClientMessenger:
         return self.__messenger
 
     @property
     def session(self) -> ClientSession:
@@ -70,16 +70,20 @@
 
     @property  # Override
     def running(self) -> bool:
         if super().running:
             return self.session.running
 
     def start(self):
-        thread = threading.Thread(target=self.run, daemon=True)
-        thread.start()
+        self.__daemon.start()
+
+    # Override
+    def stop(self):
+        self.__daemon.stop()
+        super().stop()
 
     # Override
     def setup(self):
         super().setup()
         self.session.start(delegate=self)
 
     # Override
```

### Comparing `dimples-0.5.3/dimples/common/__init__.py` & `dimples-0.5.5/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/anonymous.py` & `dimples-0.5.5/dimples/common/anonymous.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/ans.py` & `dimples-0.5.5/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/archivist.py` & `dimples-0.5.5/dimples/common/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/__init__.py` & `dimples-0.5.5/dimples/common/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/btc.py` & `dimples-0.5.5/dimples/common/compat/btc.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/compatible.py` & `dimples-0.5.5/dimples/common/compat/compatible.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/entity.py` & `dimples-0.5.5/dimples/common/compat/entity.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/meta.py` & `dimples-0.5.5/dimples/common/compat/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/compat/network.py` & `dimples-0.5.5/dimples/common/compat/network.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/dbi/__init__.py` & `dimples-0.5.5/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/dbi/account.py` & `dimples-0.5.5/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/dbi/message.py` & `dimples-0.5.5/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/dbi/session.py` & `dimples-0.5.5/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/facebook.py` & `dimples-0.5.5/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/messenger.py` & `dimples-0.5.5/dimples/common/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/packer.py` & `dimples-0.5.5/dimples/common/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/processer.py` & `dimples-0.5.5/dimples/common/processer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/__init__.py` & `dimples-0.5.5/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/ans.py` & `dimples-0.5.5/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/block.py` & `dimples-0.5.5/dimples/common/protocol/block.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/handshake.py` & `dimples-0.5.5/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/login.py` & `dimples-0.5.5/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/mute.py` & `dimples-0.5.5/dimples/common/protocol/mute.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/protocol/report.py` & `dimples-0.5.5/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/register.py` & `dimples-0.5.5/dimples/common/register.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/common/session.py` & `dimples-0.5.5/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/__init__.py` & `dimples-0.5.5/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/gate.py` & `dimples-0.5.5/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/gatekeeper.py` & `dimples-0.5.5/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/mars.py` & `dimples-0.5.5/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/mtp.py` & `dimples-0.5.5/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/protocol/__init__.py` & `dimples-0.5.5/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/protocol/mars.py` & `dimples-0.5.5/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/protocol/ws.py` & `dimples-0.5.5/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/queue.py` & `dimples-0.5.5/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/seeker.py` & `dimples-0.5.5/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/session.py` & `dimples-0.5.5/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/conn/ws.py` & `dimples-0.5.5/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/__init__.py` & `dimples-0.5.5/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/account.py` & `dimples-0.5.5/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/__init__.py` & `dimples-0.5.5/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/base.py` & `dimples-0.5.5/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/document.py` & `dimples-0.5.5/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/group.py` & `dimples-0.5.5/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/group_history.py` & `dimples-0.5.5/dimples/database/dos/group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/group_keys.py` & `dimples-0.5.5/dimples/database/dos/group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/login.py` & `dimples-0.5.5/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/meta.py` & `dimples-0.5.5/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/private.py` & `dimples-0.5.5/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/station.py` & `dimples-0.5.5/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/dos/user.py` & `dimples-0.5.5/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/message.py` & `dimples-0.5.5/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/session.py` & `dimples-0.5.5/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_cipherkey.py` & `dimples-0.5.5/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_document.py` & `dimples-0.5.5/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_group.py` & `dimples-0.5.5/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_group_history.py` & `dimples-0.5.5/dimples/database/t_group_history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_group_keys.py` & `dimples-0.5.5/dimples/database/t_group_keys.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_login.py` & `dimples-0.5.5/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_message.py` & `dimples-0.5.5/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_meta.py` & `dimples-0.5.5/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_private.py` & `dimples-0.5.5/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_station.py` & `dimples-0.5.5/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/database/t_user.py` & `dimples-0.5.5/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/edge/__init__.py` & `dimples-0.5.5/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/edge/octopus.py` & `dimples-0.5.5/dimples/edge/octopus.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from dimsdk import ContentType
 from dimsdk import EntityType, ID
 from dimsdk import ReliableMessage
 from dimsdk import Station
 
 from ..utils import Log, Logging
-from ..utils import Runner
+from ..utils import Runner, Daemon
 from ..utils import get_msg_sig
 from ..common import ProviderInfo
 from ..common import MessageDBI, SessionDBI
 from ..common import HandshakeCommand
 
 from ..client import ClientSession
 from ..client import ClientFacebook
@@ -63,14 +63,15 @@
     def __init__(self, shared: GlobalVariable, local_host: str = '127.0.0.1', local_port: int = 9394):
         super().__init__(interval=60)
         self.__shared = shared
         self.__inner = self.create_inner_terminal(host=local_host, port=local_port)
         self.__outers: Set[Terminal] = set()
         self.__outer_map = weakref.WeakValueDictionary()
         self.__outer_lock = threading.Lock()
+        self.__daemon = Daemon(target=self, daemonic=False)
 
     @property
     def shared(self) -> GlobalVariable:
         return self.__shared
 
     @property
     def database(self) -> SessionDBI:
@@ -125,16 +126,15 @@
                     return None
             # create new terminal
             terminal = self.create_outer_terminal(host=host, port=port)
             self.__outers.add(terminal)
             return terminal
 
     def start(self):
-        thread = threading.Thread(target=self.run)
-        thread.start()
+        self.__daemon.start()
 
     # Override
     def stop(self):
         super().stop()
         inner = self.__inner
         if inner is not None:
             inner.stop()
```

### Comparing `dimples-0.5.3/dimples/edge/shared.py` & `dimples-0.5.5/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/edge/start.py` & `dimples-0.5.5/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/__init__.py` & `dimples-0.5.5/dimples/group/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/admin.py` & `dimples-0.5.5/dimples/group/admin.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/builder.py` & `dimples-0.5.5/dimples/group/builder.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/delegate.py` & `dimples-0.5.5/dimples/group/delegate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/emitter.py` & `dimples-0.5.5/dimples/group/emitter.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/helper.py` & `dimples-0.5.5/dimples/group/helper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/manager.py` & `dimples-0.5.5/dimples/group/manager.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/group/packer.py` & `dimples-0.5.5/dimples/group/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/register/__init__.py` & `dimples-0.5.5/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/register/base.py` & `dimples-0.5.5/dimples/register/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/register/ext.py` & `dimples-0.5.5/dimples/register/ext.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/register/run.py` & `dimples-0.5.5/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/register/shared.py` & `dimples-0.5.5/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/__init__.py` & `dimples-0.5.5/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/archivist.py` & `dimples-0.5.5/dimples/server/archivist.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/__init__.py` & `dimples-0.5.5/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/ans.py` & `dimples-0.5.5/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/document.py` & `dimples-0.5.5/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/handshake.py` & `dimples-0.5.5/dimples/server/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/login.py` & `dimples-0.5.5/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/cpu/report.py` & `dimples-0.5.5/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/dispatcher.py` & `dimples-0.5.5/dimples/server/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,19 @@
     A dispatcher to decide which way to deliver message.
 """
 
 import threading
 from abc import ABC, abstractmethod
 from typing import Optional, List
 
-from startrek.fsm import Daemon
-
 from dimsdk import EntityType, ID
 from dimsdk import Content, ReceiptCommand
 from dimsdk import ReliableMessage
 
-from ..utils import Singleton, Logging, Runner
+from ..utils import Singleton, Logging, Runner, Daemon
 from ..common import CommonFacebook
 from ..common import MessageDBI, SessionDBI
 from ..common import ReliableMessageDBI
 from ..common import LoginCommand
 
 from .session_center import SessionCenter
 from .push import PushCenter
@@ -207,15 +205,15 @@
 
     def __init__(self, database: MessageDBI):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__database = database
         # roaming (user id => station id)
         self.__queue: List[RoamingInfo] = []
         self.__lock = threading.Lock()
-        self.__daemon = Daemon(target=self.run)
+        self.__daemon = Daemon(target=self)
 
     @property
     def database(self) -> Optional[MessageDBI]:
         return self.__database
 
     def __append(self, info: RoamingInfo):
         with self.__lock:
```

### Comparing `dimples-0.5.3/dimples/server/messenger.py` & `dimples-0.5.5/dimples/server/messenger.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/packer.py` & `dimples-0.5.5/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/processor.py` & `dimples-0.5.5/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/push.py` & `dimples-0.5.5/dimples/server/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 """
 
 import threading
 import time
 from abc import ABC, abstractmethod
 from typing import Optional, List, Dict
 
-from startrek.fsm import Daemon
 from dimsdk import ID, ReliableMessage
 
-from ..utils import Singleton, Logging, Runner
+from ..utils import Runner, Daemon
+from ..utils import Singleton, Logging
 
 
 class MessageQueue(Logging):
 
     def __init__(self):
         super().__init__()
         self.__messages: Optional[List[ReliableMessage]] = None
@@ -121,17 +121,16 @@
 
     def __init__(self):
         super().__init__(interval=Runner.INTERVAL_SLOW)
         self.__queue = MessageQueue()
         self.__keeper = BadgeKeeper()
         self.__service: Optional[PushService] = None
         # background thread
-        daemon = Daemon(target=self.run)
-        daemon.start()
-        self.__daemon = daemon
+        self.__daemon = Daemon(target=self)
+        self.__daemon.start()
 
     @property
     def service(self) -> Optional[PushService]:
         return self.__service
 
     @service.setter
     def service(self, pusher: PushService):
```

### Comparing `dimples-0.5.3/dimples/server/session.py` & `dimples-0.5.5/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/session_center.py` & `dimples-0.5.5/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/server/trace.py` & `dimples-0.5.5/dimples/server/trace.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/station/__init__.py` & `dimples-0.5.5/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/station/handler.py` & `dimples-0.5.5/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/station/shared.py` & `dimples-0.5.5/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/station/start.py` & `dimples-0.5.5/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/utils/__init__.py` & `dimples-0.5.5/dimples/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from dimsdk import Converter
 from dimsdk import DateTime
 from dimsdk import ReliableMessage
 from dimsdk import DocumentHelper
 
 from dimplugins.crypto.aes import random_bytes
 
-from startrek.fsm import Runnable, Runner
+from startrek.fsm import Runnable, Runner, Daemon
 from startrek.fsm import Delegate as StateDelegate
 from startrek.net.channel import get_remote_address, get_local_address
 
 
 from .singleton import Singleton
 from .log import Log, Logging
 from .dos import Path, File, TextFile, JSONFile
@@ -118,15 +118,15 @@
     'utf8_encode', 'utf8_decode',
     'json_encode', 'json_decode',
 
     'random_bytes',
 
     'Converter',
 
-    'Runnable', 'Runner',
+    'Runnable', 'Runner', 'Daemon',
     'StateDelegate',
 
     'get_remote_address', 'get_local_address',
 
 
     'Singleton',
     'Log', 'Logging',
```

### Comparing `dimples-0.5.3/dimples/utils/cache.py` & `dimples-0.5.5/dimples/utils/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ~~~~~~~~~~~~~~~
 
 """
 
 import time
 from typing import TypeVar, Generic, Optional, Dict, Set, Tuple
 
-from startrek.fsm import Daemon
+from startrek.fsm import Daemon, Runnable
 from dimsdk import DateTime
 
 from .singleton import Singleton
 
 
 K = TypeVar('K')
 V = TypeVar('V')
@@ -131,33 +131,34 @@
                 # remove expired holders
                 self.__holders.pop(key, None)
                 count += 1
         return count
 
 
 @Singleton
-class CacheManager:
+class CacheManager(Runnable):
 
     def __init__(self):
         self.__pools: Dict[str, CachePool] = {}  # name -> pool
         # thread for cleaning caches
-        self.__daemon = Daemon(target=self.run)
+        self.__daemon = Daemon(target=self)
         self.__running = False
 
     @property
     def running(self) -> bool:
         return self.__running
 
     def start(self):
         self.__running = True
         self.__daemon.start()
 
     def stop(self):
         self.__daemon.stop()
 
+    # Override
     def run(self):
         next_time = 0
         while self.running:
             # try to purge each 5 minutes
             now = DateTime.now()
             if now < next_time:
                 time.sleep(2)
```

### Comparing `dimples-0.5.3/dimples/utils/config.py` & `dimples-0.5.5/dimples/utils/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/utils/dos.py` & `dimples-0.5.5/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/utils/log.py` & `dimples-0.5.5/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples/utils/singleton.py` & `dimples-0.5.5/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/dimples.egg-info/PKG-INFO` & `dimples-0.5.5/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.5.3
+Version: 0.5.5
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.5.3/dimples.egg-info/SOURCES.txt` & `dimples-0.5.5/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.5.3/setup.py` & `dimples-0.5.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.5.3'
+__version__ = '0.5.5'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -54,12 +54,12 @@
         'dimplugins>=1.0.2',
 
         'dimsdk>=1.0.3',
         'dimp>=1.0.3',
         'dkd>=1.0.2',
         'mkm>=1.0.2',
 
-        'startrek>=1.1.2',
-        'tcp>=1.1.2',
-        'udp>=1.1.2',
+        'startrek>=1.2.0',
+        'tcp>=1.2.0',
+        'udp>=1.2.0',
     ]
 )
```

