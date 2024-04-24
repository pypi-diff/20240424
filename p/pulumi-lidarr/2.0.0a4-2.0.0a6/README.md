# Comparing `tmp/pulumi_lidarr-2.0.0a4.tar.gz` & `tmp/pulumi_lidarr-2.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_lidarr-2.0.0a4.tar", last modified: Mon Apr 22 23:19:44 2024, max compression
+gzip compressed data, was "pulumi_lidarr-2.0.0a6.tar", last modified: Tue Apr 23 20:59:27 2024, max compression
```

## Comparing `pulumi_lidarr-2.0.0a4.tar` & `pulumi_lidarr-2.0.0a6.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.508735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.508735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/get_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/get_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.508735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.512735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (127)    84761 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/download_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36251 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/flood.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24033 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_download_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_download_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_remote_path_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_remote_path_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/hadouken.py
--rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/nzbvortex.py
--rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    40680 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/remote_path_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/torrent_blackhole.py
--rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/torrent_download_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/transmission.py
--rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/usenet_blackhole.py
--rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/usenet_download_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    36637 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/utorrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/vuze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.516734 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_import_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/headphones.py
--rw-r--r--   0 runner    (1001) docker     (127)    56058 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/import_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lastfm_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lastfm_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    34565 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lidarr_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    28610 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/music_brainz.py
--rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32483 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_albums.py
--rw-r--r--   0 runner    (1001) docker     (127)    32539 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_playlists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.520735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/filelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    32303 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_indexers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/headphones.py
--rw-r--r--   0 runner    (1001) docker     (127)    61747 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (127)    25484 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/newznab.py
--rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/redacted.py
--rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torrent_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)    26692 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torznab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.520735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_media_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_root_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_root_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)    47165 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/media_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/root_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.520735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/kodi.py
--rw-r--r--   0 runner    (1001) docker     (127)    23491 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15631 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/roksbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/wdtv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.528735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44934 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/apprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    48258 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/email.py
--rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/emby.py
--rw-r--r--   0 runner    (1001) docker     (127)    44622 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/get_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)    34932 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/gotify.py
--rw-r--r--   0 runner    (1001) docker     (127)    32164 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    43228 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/kodi.py
--rw-r--r--   0 runner    (1001) docker     (127)    35819 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (127)    28297 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/notifiarr.py
--rw-r--r--   0 runner    (1001) docker     (127)   162903 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    43633 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/ntfy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28889 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/prowl.py
--rw-r--r--   0 runner    (1001) docker     (127)    38562 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (127)    41609 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/pushover.py
--rw-r--r--   0 runner    (1001) docker     (127)    36342 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    43017 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    33882 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/simplepush.py
--rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    39066 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/subsonic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/synology_indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41015 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/delay_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_release_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_release_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_custom_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_delay_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_delay_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_metadata_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_primary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_primary_album_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_secondary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_secondary_album_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31419 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/quality_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/release_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/get_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/get_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    26639 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/host.py
--rw-r--r--   0 runner    (1001) docker     (127)    23157 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/get_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:19:44.508735 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 23:19:44.532735 pulumi_lidarr-2.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-22 23:19:44.000000 pulumi_lidarr-2.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.113970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.113970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/get_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/get_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.117970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.121970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10804 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34406 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84761 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/download_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36251 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/flood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24033 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_download_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_download_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_remote_path_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_remote_path_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/hadouken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28900 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/nzbvortex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40680 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/remote_path_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38316 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/torrent_blackhole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28199 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/torrent_download_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/usenet_blackhole.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/usenet_download_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36637 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/utorrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/vuze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.121970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15913 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_import_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/headphones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56058 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/import_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30318 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lastfm_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30396 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lastfm_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34565 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lidarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28610 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/music_brainz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32483 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_albums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32539 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_playlists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.125970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32303 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17698 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_indexers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/headphones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61747 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18621 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25484 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/redacted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21527 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torrent_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26692 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torznab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.125970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_media_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_root_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_root_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47165 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/media_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/root_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.125970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/kodi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23491 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15631 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/roksbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/wdtv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.133970 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44934 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/apprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37628 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48258 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44670 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/emby.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44622 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/get_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34932 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32164 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43228 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/kodi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35819 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28297 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/notifiarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162903 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43633 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/ntfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28889 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38562 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41609 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36342 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43017 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33882 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/simplepush.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39066 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/subsonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21947 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/synology_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36166 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42644 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41015 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/delay_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_release_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_release_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_custom_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_delay_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_delay_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_metadata_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_primary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_primary_album_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_secondary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_secondary_album_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31419 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/quality_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20734 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/release_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15277 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17897 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/get_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26639 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23157 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/get_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:59:27.113970 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 20:59:27.000000 pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:59:27.137971 pulumi_lidarr-2.0.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-23 20:59:26.000000 pulumi_lidarr-2.0.0a6/setup.py
```

### Comparing `pulumi_lidarr-2.0.0a4/PKG-INFO` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: pulumi_lidarr
-Version: 2.0.0a4
+Name: pulumi-lidarr
+Version: 2.0.0a6
 Summary: A Pulumi package for creating and managing Lidarr resources
 Home-page: https://github.com/MaienM/pulumi-lidarr
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-lidarr
 Keywords: pulumi lidarr category/utility
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Lidarr Resource Provider
 
 The Lidarr Resource Provider lets you manage [lidarr](https://www.pulumi.com/registry/packages/lidarr/) resources.
 
@@ -55,9 +54,7 @@
 ```bash
 dotnet add package MaienM.Lidarr
 ```
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/lidarr/api-docs/).
-
-
```

### Comparing `pulumi_lidarr-2.0.0a4/README.md` & `pulumi_lidarr-2.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/_utilities.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/artist.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/artist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/get_artist.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/get_artist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/get_artists.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/get_artists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/artists/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/artists/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/config/vars.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/aria2.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/aria2.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/deluge.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/deluge.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/download_client.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/download_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/flood.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/flood.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_download_client.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_download_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_download_clients.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_download_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_remote_path_mapping.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_remote_path_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/get_remote_path_mappings.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/get_remote_path_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/hadouken.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/hadouken.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/nzbget.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/nzbget.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/nzbvortex.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/nzbvortex.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/pneumatic.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/pneumatic.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/qbittorrent.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/remote_path_mapping.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/remote_path_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/rtorrent.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/rtorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/sabnzbd.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/torrent_blackhole.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/torrent_blackhole.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/torrent_download_station.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/torrent_download_station.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/transmission.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/transmission.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/usenet_blackhole.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/usenet_blackhole.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/usenet_download_station.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/usenet_download_station.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/utorrent.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/utorrent.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/downloadclients/vuze.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/downloadclients/vuze.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/exclusion.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_exclusion.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_exclusions.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_exclusions.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_import_list.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_import_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/get_import_lists.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/get_import_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/headphones.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/headphones.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/import_list.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/import_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lastfm_tag.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lastfm_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lastfm_user.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lastfm_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lidarr.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lidarr.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/lidarr_list.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/lidarr_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/music_brainz.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/music_brainz.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_albums.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_albums.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_artists.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_artists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/importlists/spotify_playlists.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/importlists/spotify_playlists.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/filelist.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/filelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/gazelle.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/gazelle.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_indexer.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/get_indexers.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/get_indexers.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/headphones.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/headphones.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/indexer.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/iptorrents.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/iptorrents.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/newznab.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/newznab.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/nyaa.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/nyaa.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/redacted.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/redacted.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torrent_rss.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torrent_rss.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torrentleech.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torrentleech.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/indexers/torznab.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/indexers/torznab.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_media_management.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_media_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_naming.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_naming.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_root_folder.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_root_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/get_root_folders.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/get_root_folders.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/media_management.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/media_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/naming.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/naming.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/mediamanagement/root_folder.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/mediamanagement/root_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_config.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_consumers.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_consumers.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/get_metadata.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/get_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/kodi.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/kodi.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/metadata.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/roksbox.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/roksbox.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/metadata/wdtv.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/metadata/wdtv.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/apprise.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/custom_script.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/custom_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/discord.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/discord.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/email.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/email.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/emby.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/emby.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/get_notification.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/get_notifications.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/get_notifications.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/gotify.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/gotify.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/join.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/join.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/kodi.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/kodi.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/mailgun.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/mailgun.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/notifiarr.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/notifiarr.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/notification.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/ntfy.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/ntfy.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/plex.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/plex.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/prowl.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/prowl.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/pushbullet.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/pushbullet.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/pushover.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/pushover.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/sendgrid.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/sendgrid.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/signal.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/signal.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/simplepush.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/simplepush.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/slack.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/subsonic.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/subsonic.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/synology_indexer.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/synology_indexer.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/telegram.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/telegram.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/twitter.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/twitter.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/notifications/webhook.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/notifications/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/__init__.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/_inputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/custom_format.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/custom_format.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/delay_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/delay_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_release_group.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_release_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_release_title.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_release_title.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_condition_size.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_condition_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_custom_format.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_custom_format.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_custom_formats.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_custom_formats.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_delay_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_delay_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_delay_profiles.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_delay_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_metadata_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_metadata_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_metadata_profiles.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_metadata_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_primary_album_type.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_primary_album_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_primary_album_types.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_primary_album_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_definition.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_definitions.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_definitions.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_quality_profiles.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_quality_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_profiles.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_status.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_release_statuses.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_release_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_secondary_album_type.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_secondary_album_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/get_secondary_album_types.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/get_secondary_album_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/metadata_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/metadata_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/quality_definition.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/quality_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/quality_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/quality_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/profiles/release_profile.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/profiles/release_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/provider.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/_inputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/get_host.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/get_status.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/get_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/host.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/host.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/system/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/system/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/get_tag.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/get_tags.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/get_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/outputs.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr/tags/tag.py` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/PKG-INFO` & `pulumi_lidarr-2.0.0a6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: pulumi-lidarr
-Version: 2.0.0a4
+Name: pulumi_lidarr
+Version: 2.0.0a6
 Summary: A Pulumi package for creating and managing Lidarr resources
 Home-page: https://github.com/MaienM/pulumi-lidarr
 License: Apache-2.0
 Project-URL: Repository, https://github.com/MaienM/pulumi-lidarr
 Keywords: pulumi lidarr category/utility
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Lidarr Resource Provider
 
 The Lidarr Resource Provider lets you manage [lidarr](https://www.pulumi.com/registry/packages/lidarr/) resources.
 
@@ -55,9 +54,7 @@
 ```bash
 dotnet add package MaienM.Lidarr
 ```
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/lidarr/api-docs/).
-
-
```

### Comparing `pulumi_lidarr-2.0.0a4/pulumi_lidarr.egg-info/SOURCES.txt` & `pulumi_lidarr-2.0.0a6/pulumi_lidarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_lidarr-2.0.0a4/setup.py` & `pulumi_lidarr-2.0.0a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.0.0a4"
+VERSION = "2.0.0a6"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "lidarr Pulumi Package - Development Version"
```

