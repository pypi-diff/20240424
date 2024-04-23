# Comparing `tmp/cs2_battle_bot_api_client-0.0.8.tar.gz` & `tmp/cs2_battle_bot_api_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs2_battle_bot_api_client-0.0.8.tar", max compression
+gzip compressed data, was "cs2_battle_bot_api_client-0.0.9.tar", max compression
```

## Comparing `cs2_battle_bot_api_client-0.0.8.tar` & `cs2_battle_bot_api_client-0.0.9.tar`

### file list

```diff
@@ -1,125 +1,125 @@
--rw-r--r--   0        0        0     5128 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/README.md
--rw-r--r--   0        0        0      161 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/__init__.py
--rw-r--r--   0        0        0       45 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/__init__.py
--rw-r--r--   0        0        0     3645 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py
--rw-r--r--   0        0        0     2212 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py
--rw-r--r--   0        0        0     3927 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py
--rw-r--r--   0        0        0     3973 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py
--rw-r--r--   0        0        0     3359 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py
--rw-r--r--   0        0        0     3846 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/__init__.py
--rw-r--r--   0        0        0     3994 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py
--rw-r--r--   0        0        0     3606 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_create.py
--rw-r--r--   0        0        0     2265 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py
--rw-r--r--   0        0        0     3841 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_list.py
--rw-r--r--   0        0        0     3928 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py
--rw-r--r--   0        0        0     3381 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py
--rw-r--r--   0        0        0     3814 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/__init__.py
--rw-r--r--   0        0        0     3460 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_create.py
--rw-r--r--   0        0        0     2203 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_destroy.py
--rw-r--r--   0        0        0     3813 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_list.py
--rw-r--r--   0        0        0     3771 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_partial_update.py
--rw-r--r--   0        0        0     3246 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_retrieve.py
--rw-r--r--   0        0        0     3661 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/__init__.py
--rw-r--r--   0        0        0     3985 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_ban_create.py
--rw-r--r--   0        0        0     3293 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py
--rw-r--r--   0        0        0     3360 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py
--rw-r--r--   0        0        0     3602 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_destroy.py
--rw-r--r--   0        0        0     3859 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_join_create.py
--rw-r--r--   0        0        0     3842 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_list.py
--rw-r--r--   0        0        0     3713 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_load_create.py
--rw-r--r--   0        0        0     3821 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_partial_update.py
--rw-r--r--   0        0        0     4010 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_pick_create.py
--rw-r--r--   0        0        0     3437 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py
--rw-r--r--   0        0        0     3717 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py
--rw-r--r--   0        0        0     3274 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_retrieve.py
--rw-r--r--   0        0        0     3716 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py
--rw-r--r--   0        0        0     3707 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_update.py
--rw-r--r--   0        0        0     3509 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/__init__.py
--rw-r--r--   0        0        0     3528 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_destroy.py
--rw-r--r--   0        0        0     3855 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_list.py
--rw-r--r--   0        0        0     3845 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_partial_update.py
--rw-r--r--   0        0        0     3287 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_retrieve.py
--rw-r--r--   0        0        0     3729 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/schema/__init__.py
--rw-r--r--   0        0        0     4900 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/schema/schema_retrieve.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/__init__.py
--rw-r--r--   0        0        0     3528 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_create.py
--rw-r--r--   0        0        0     2206 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_destroy.py
--rw-r--r--   0        0        0     3292 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py
--rw-r--r--   0        0        0     4834 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_list.py
--rw-r--r--   0        0        0     3845 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_partial_update.py
--rw-r--r--   0        0        0     3287 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_retrieve.py
--rw-r--r--   0        0        0     3729 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/__init__.py
--rw-r--r--   0        0        0     3599 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py
--rw-r--r--   0        0        0     2210 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py
--rw-r--r--   0        0        0     3899 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py
--rw-r--r--   0        0        0     3923 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py
--rw-r--r--   0        0        0     3331 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py
--rw-r--r--   0        0        0     3800 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py
--rw-r--r--   0        0        0        0 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/__init__.py
--rw-r--r--   0        0        0     3482 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_create.py
--rw-r--r--   0        0        0     2204 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_destroy.py
--rw-r--r--   0        0        0     3827 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_list.py
--rw-r--r--   0        0        0     3795 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_partial_update.py
--rw-r--r--   0        0        0     3259 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_retrieve.py
--rw-r--r--   0        0        0     3683 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_update.py
--rw-r--r--   0        0        0    12417 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/client.py
--rw-r--r--   0        0        0      546 2024-04-18 13:48:59.069451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/errors.py
--rw-r--r--   0        0        0     2987 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_guild.py
--rw-r--r--   0        0        0     1663 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_guild_member.py
--rw-r--r--   0        0        0     4900 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_match.py
--rw-r--r--   0        0        0     1208 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_match_cvars.py
--rw-r--r--   0        0        0     2312 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/discord_user.py
--rw-r--r--   0        0        0     4937 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/guild.py
--rw-r--r--   0        0        0     2192 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/map_.py
--rw-r--r--   0        0        0     2454 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/map_ban.py
--rw-r--r--   0        0        0      237 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/map_sides_enum.py
--rw-r--r--   0        0        0     9921 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match.py
--rw-r--r--   0        0        0     1743 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_ban_map.py
--rw-r--r--   0        0        0     2287 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_ban_map_result.py
--rw-r--r--   0        0        0     4379 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config.py
--rw-r--r--   0        0        0     1208 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_cvars.py
--rw-r--r--   0        0        0     1211 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_team_1.py
--rw-r--r--   0        0        0     1211 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_team_2.py
--rw-r--r--   0        0        0     2507 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_map_selected.py
--rw-r--r--   0        0        0     1748 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_pick_map.py
--rw-r--r--   0        0        0     2312 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_pick_map_result.py
--rw-r--r--   0        0        0     1550 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_player_join.py
--rw-r--r--   0        0        0      166 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_type_enum.py
--rw-r--r--   0        0        0     3629 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_discord_user_list.py
--rw-r--r--   0        0        0     3552 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_guild_list.py
--rw-r--r--   0        0        0     3530 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_map_list.py
--rw-r--r--   0        0        0     3552 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_match_list.py
--rw-r--r--   0        0        0     3564 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_player_list.py
--rw-r--r--   0        0        0     3564 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_server_list.py
--rw-r--r--   0        0        0     3605 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_steam_user_list.py
--rw-r--r--   0        0        0     3540 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_team_list.py
--rw-r--r--   0        0        0     3336 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_discord_user.py
--rw-r--r--   0        0        0     6184 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_guild.py
--rw-r--r--   0        0        0     3205 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_map.py
--rw-r--r--   0        0        0    13243 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_match.py
--rw-r--r--   0        0        0     3385 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_player.py
--rw-r--r--   0        0        0     4068 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_server.py
--rw-r--r--   0        0        0     5851 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_steam_user.py
--rw-r--r--   0        0        0     4483 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_team.py
--rw-r--r--   0        0        0     2354 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/player.py
--rw-r--r--   0        0        0     1605 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/schema_retrieve_lang.py
--rw-r--r--   0        0        0     1256 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py
--rw-r--r--   0        0        0     3745 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/server.py
--rw-r--r--   0        0        0      207 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/status_enum.py
--rw-r--r--   0        0        0     4952 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/steam_user.py
--rw-r--r--   0        0        0     3374 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/team.py
--rw-r--r--   0        0        0      161 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/type_enum.py
--rw-r--r--   0        0        0       25 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/types.py
--rw-r--r--   0        0        0      577 2024-04-18 13:48:59.073451 cs2_battle_bot_api_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 cs2_battle_bot_api_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5128 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/README.md
+-rw-r--r--   0        0        0      161 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py
+-rw-r--r--   0        0        0     2212 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py
+-rw-r--r--   0        0        0     3927 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py
+-rw-r--r--   0        0        0     3973 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py
+-rw-r--r--   0        0        0     3359 2024-04-18 15:01:37.568539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py
+-rw-r--r--   0        0        0     3846 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/__init__.py
+-rw-r--r--   0        0        0     3994 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py
+-rw-r--r--   0        0        0     3606 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_create.py
+-rw-r--r--   0        0        0     2265 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py
+-rw-r--r--   0        0        0     3841 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_list.py
+-rw-r--r--   0        0        0     3928 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py
+-rw-r--r--   0        0        0     3381 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py
+-rw-r--r--   0        0        0     3814 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/__init__.py
+-rw-r--r--   0        0        0     3460 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_create.py
+-rw-r--r--   0        0        0     2203 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_destroy.py
+-rw-r--r--   0        0        0     3813 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_list.py
+-rw-r--r--   0        0        0     3771 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_partial_update.py
+-rw-r--r--   0        0        0     3246 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_retrieve.py
+-rw-r--r--   0        0        0     3661 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/__init__.py
+-rw-r--r--   0        0        0     3985 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_ban_create.py
+-rw-r--r--   0        0        0     3293 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py
+-rw-r--r--   0        0        0     3360 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py
+-rw-r--r--   0        0        0     3607 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_destroy.py
+-rw-r--r--   0        0        0     3859 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_join_create.py
+-rw-r--r--   0        0        0     3842 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_list.py
+-rw-r--r--   0        0        0     3713 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_load_create.py
+-rw-r--r--   0        0        0     3821 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_partial_update.py
+-rw-r--r--   0        0        0     4010 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_pick_create.py
+-rw-r--r--   0        0        0     3437 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py
+-rw-r--r--   0        0        0     3717 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py
+-rw-r--r--   0        0        0     3274 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_retrieve.py
+-rw-r--r--   0        0        0     3716 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py
+-rw-r--r--   0        0        0     3707 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_update.py
+-rw-r--r--   0        0        0     3509 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_destroy.py
+-rw-r--r--   0        0        0     3855 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_list.py
+-rw-r--r--   0        0        0     3845 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_partial_update.py
+-rw-r--r--   0        0        0     3287 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_retrieve.py
+-rw-r--r--   0        0        0     3729 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/schema/__init__.py
+-rw-r--r--   0        0        0     4900 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/schema/schema_retrieve.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/__init__.py
+-rw-r--r--   0        0        0     3528 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_create.py
+-rw-r--r--   0        0        0     2206 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_destroy.py
+-rw-r--r--   0        0        0     3292 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py
+-rw-r--r--   0        0        0     4834 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_list.py
+-rw-r--r--   0        0        0     3845 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_partial_update.py
+-rw-r--r--   0        0        0     3287 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_retrieve.py
+-rw-r--r--   0        0        0     3729 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/__init__.py
+-rw-r--r--   0        0        0     3599 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py
+-rw-r--r--   0        0        0     2210 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py
+-rw-r--r--   0        0        0     3899 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py
+-rw-r--r--   0        0        0     3923 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py
+-rw-r--r--   0        0        0     3331 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py
+-rw-r--r--   0        0        0     3800 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/__init__.py
+-rw-r--r--   0        0        0     3482 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_create.py
+-rw-r--r--   0        0        0     2204 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_destroy.py
+-rw-r--r--   0        0        0     3827 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_list.py
+-rw-r--r--   0        0        0     3795 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_partial_update.py
+-rw-r--r--   0        0        0     3259 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_retrieve.py
+-rw-r--r--   0        0        0     3683 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_update.py
+-rw-r--r--   0        0        0    12417 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/client.py
+-rw-r--r--   0        0        0      546 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/errors.py
+-rw-r--r--   0        0        0     2987 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2723 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_guild.py
+-rw-r--r--   0        0        0     1663 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_guild_member.py
+-rw-r--r--   0        0        0     4900 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_match.py
+-rw-r--r--   0        0        0     1208 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_match_cvars.py
+-rw-r--r--   0        0        0     2312 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/discord_user.py
+-rw-r--r--   0        0        0     4937 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/guild.py
+-rw-r--r--   0        0        0     2192 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/map_.py
+-rw-r--r--   0        0        0     2454 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/map_ban.py
+-rw-r--r--   0        0        0      237 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/map_sides_enum.py
+-rw-r--r--   0        0        0    10408 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match.py
+-rw-r--r--   0        0        0     1743 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_ban_map.py
+-rw-r--r--   0        0        0     2287 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_ban_map_result.py
+-rw-r--r--   0        0        0     4379 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config.py
+-rw-r--r--   0        0        0     1208 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_cvars.py
+-rw-r--r--   0        0        0     1211 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_team_1.py
+-rw-r--r--   0        0        0     1211 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_team_2.py
+-rw-r--r--   0        0        0     2507 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_map_selected.py
+-rw-r--r--   0        0        0     1748 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_pick_map.py
+-rw-r--r--   0        0        0     2312 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_pick_map_result.py
+-rw-r--r--   0        0        0     1550 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_player_join.py
+-rw-r--r--   0        0        0      166 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_type_enum.py
+-rw-r--r--   0        0        0     3629 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_discord_user_list.py
+-rw-r--r--   0        0        0     3552 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_guild_list.py
+-rw-r--r--   0        0        0     3530 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_map_list.py
+-rw-r--r--   0        0        0     3552 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_match_list.py
+-rw-r--r--   0        0        0     3564 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_player_list.py
+-rw-r--r--   0        0        0     3564 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_server_list.py
+-rw-r--r--   0        0        0     3605 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_steam_user_list.py
+-rw-r--r--   0        0        0     3540 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_team_list.py
+-rw-r--r--   0        0        0     3336 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_discord_user.py
+-rw-r--r--   0        0        0     6184 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_guild.py
+-rw-r--r--   0        0        0     3205 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_map.py
+-rw-r--r--   0        0        0    13358 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_match.py
+-rw-r--r--   0        0        0     4297 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_player.py
+-rw-r--r--   0        0        0     4068 2024-04-18 15:01:37.572538 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_server.py
+-rw-r--r--   0        0        0     5851 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_steam_user.py
+-rw-r--r--   0        0        0     4360 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_team.py
+-rw-r--r--   0        0        0     2686 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/player.py
+-rw-r--r--   0        0        0     1605 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/schema_retrieve_lang.py
+-rw-r--r--   0        0        0     1256 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py
+-rw-r--r--   0        0        0     3745 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/server.py
+-rw-r--r--   0        0        0      207 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/status_enum.py
+-rw-r--r--   0        0        0     4952 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/steam_user.py
+-rw-r--r--   0        0        0     2876 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/team.py
+-rw-r--r--   0        0        0      161 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/type_enum.py
+-rw-r--r--   0        0        0       25 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/py.typed
+-rw-r--r--   0        0        0      985 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/types.py
+-rw-r--r--   0        0        0      577 2024-04-18 15:01:37.576539 cs2_battle_bot_api_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5747 1970-01-01 00:00:00.000000 cs2_battle_bot_api_client-0.0.9/PKG-INFO
```

### Comparing `cs2_battle_bot_api_client-0.0.8/README.md` & `cs2_battle_bot_api_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/discord_users/discord_users_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_add_member_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/guilds/guilds_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/guilds/guilds_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/maps/maps_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/maps/maps_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_ban_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_ban_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_bans_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_config_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Match]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Match.from_dict(response.json())
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = Match.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Match]:
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_join_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_join_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_load_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_load_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_pick_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_pick_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_picks_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_recreate_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_shuffle_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/matches/matches_webhook_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/players/players_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/players/players_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/schema/schema_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/schema/schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_join_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/servers/servers_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/servers/servers_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/steam_users/steam_users_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_create.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_create.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_destroy.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_destroy.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_partial_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_partial_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_retrieve.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_retrieve.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/api/teams/teams_update.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/api/teams/teams_update.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/client.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/client.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/errors.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/__init__.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_guild.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_guild.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_guild_member.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_guild_member.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_match.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_match.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/create_match_cvars.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/create_match_cvars.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/discord_user.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/discord_user.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/guild.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/guild.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/map_.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/map_.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/map_ban.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/map_ban.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 @_attrs_define
 class Match:
     """
     Attributes:
         id (int):
         team1 (Team):
         team2 (Team):
-        winner_team (Team):
         maps (List['Map']):
         map_bans (List['MapBan']):
         map_picks (List['MatchMapSelected']):
         connect_command (str):
         load_match_command (str):
         server (Server):
         guild (Guild):
@@ -48,21 +47,21 @@
         num_maps (Union[Unset, int]):
         maplist (Union[Unset, Any]):
         map_sides (Union[Unset, Any]):
         clinch_series (Union[Unset, bool]):
         cvars (Union[Unset, Any]):
         players_per_team (Union[Unset, int]):
         message_id (Union[None, Unset, str]):
+        winner_team (Union[None, Unset, str]):
         author (Union[None, Unset, str]):
     """
 
     id: int
     team1: "Team"
     team2: "Team"
-    winner_team: "Team"
     maps: List["Map"]
     map_bans: List["MapBan"]
     map_picks: List["MatchMapSelected"]
     connect_command: str
     load_match_command: str
     server: "Server"
     guild: "Guild"
@@ -73,26 +72,25 @@
     num_maps: Union[Unset, int] = UNSET
     maplist: Union[Unset, Any] = UNSET
     map_sides: Union[Unset, Any] = UNSET
     clinch_series: Union[Unset, bool] = UNSET
     cvars: Union[Unset, Any] = UNSET
     players_per_team: Union[Unset, int] = UNSET
     message_id: Union[None, Unset, str] = UNSET
+    winner_team: Union[None, Unset, str] = UNSET
     author: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         team1 = self.team1.to_dict()
 
         team2 = self.team2.to_dict()
 
-        winner_team = self.winner_team.to_dict()
-
         maps = []
         for maps_item_data in self.maps:
             maps_item = maps_item_data.to_dict()
             maps.append(maps_item)
 
         map_bans = []
         for map_bans_item_data in self.map_bans:
@@ -138,28 +136,33 @@
 
         message_id: Union[None, Unset, str]
         if isinstance(self.message_id, Unset):
             message_id = UNSET
         else:
             message_id = self.message_id
 
+        winner_team: Union[None, Unset, str]
+        if isinstance(self.winner_team, Unset):
+            winner_team = UNSET
+        else:
+            winner_team = self.winner_team
+
         author: Union[None, Unset, str]
         if isinstance(self.author, Unset):
             author = UNSET
         else:
             author = self.author
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
                 "team1": team1,
                 "team2": team2,
-                "winner_team": winner_team,
                 "maps": maps,
                 "map_bans": map_bans,
                 "map_picks": map_picks,
                 "connect_command": connect_command,
                 "load_match_command": load_match_command,
                 "server": server,
                 "guild": guild,
@@ -181,14 +184,16 @@
             field_dict["clinch_series"] = clinch_series
         if cvars is not UNSET:
             field_dict["cvars"] = cvars
         if players_per_team is not UNSET:
             field_dict["players_per_team"] = players_per_team
         if message_id is not UNSET:
             field_dict["message_id"] = message_id
+        if winner_team is not UNSET:
+            field_dict["winner_team"] = winner_team
         if author is not UNSET:
             field_dict["author"] = author
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -202,16 +207,14 @@
         d = src_dict.copy()
         id = d.pop("id")
 
         team1 = Team.from_dict(d.pop("team1"))
 
         team2 = Team.from_dict(d.pop("team2"))
 
-        winner_team = Team.from_dict(d.pop("winner_team"))
-
         maps = []
         _maps = d.pop("maps")
         for maps_item_data in _maps:
             maps_item = Map.from_dict(maps_item_data)
 
             maps.append(maps_item)
 
@@ -272,28 +275,36 @@
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
 
         message_id = _parse_message_id(d.pop("message_id", UNSET))
 
+        def _parse_winner_team(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        winner_team = _parse_winner_team(d.pop("winner_team", UNSET))
+
         def _parse_author(data: object) -> Union[None, Unset, str]:
             if data is None:
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
 
         author = _parse_author(d.pop("author", UNSET))
 
         match = cls(
             id=id,
             team1=team1,
             team2=team2,
-            winner_team=winner_team,
             maps=maps,
             map_bans=map_bans,
             map_picks=map_picks,
             connect_command=connect_command,
             load_match_command=load_match_command,
             server=server,
             guild=guild,
@@ -304,14 +315,15 @@
             num_maps=num_maps,
             maplist=maplist,
             map_sides=map_sides,
             clinch_series=clinch_series,
             cvars=cvars,
             players_per_team=players_per_team,
             message_id=message_id,
+            winner_team=winner_team,
             author=author,
         )
 
         match.additional_properties = d
         return match
 
     @property
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_ban_map.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_ban_map.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_ban_map_result.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_ban_map_result.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_cvars.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_cvars.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_team_1.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_team_1.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_config_team_2.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_config_team_2.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_map_selected.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_map_selected.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_pick_map.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_pick_map.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_pick_map_result.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_pick_map_result.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/match_player_join.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/match_player_join.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_discord_user_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_discord_user_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_guild_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_guild_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_map_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_map_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_match_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_match_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_player_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_player_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_server_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_server_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_steam_user_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_steam_user_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/paginated_team_list.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/paginated_team_list.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_discord_user.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_discord_user.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_guild.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_guild.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_map.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_map.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_match.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 @_attrs_define
 class PatchedMatch:
     """
     Attributes:
         id (Union[Unset, int]):
         team1 (Union[Unset, Team]):
         team2 (Union[Unset, Team]):
-        winner_team (Union[Unset, Team]):
         maps (Union[Unset, List['Map']]):
         map_bans (Union[Unset, List['MapBan']]):
         map_picks (Union[Unset, List['MatchMapSelected']]):
         connect_command (Union[Unset, str]):
         load_match_command (Union[Unset, str]):
         server (Union[Unset, Server]):
         guild (Union[Unset, Guild]):
@@ -48,21 +47,21 @@
         map_sides (Union[Unset, Any]):
         clinch_series (Union[Unset, bool]):
         cvars (Union[Unset, Any]):
         players_per_team (Union[Unset, int]):
         message_id (Union[None, Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
+        winner_team (Union[None, Unset, str]):
         author (Union[None, Unset, str]):
     """
 
     id: Union[Unset, int] = UNSET
     team1: Union[Unset, "Team"] = UNSET
     team2: Union[Unset, "Team"] = UNSET
-    winner_team: Union[Unset, "Team"] = UNSET
     maps: Union[Unset, List["Map"]] = UNSET
     map_bans: Union[Unset, List["MapBan"]] = UNSET
     map_picks: Union[Unset, List["MatchMapSelected"]] = UNSET
     connect_command: Union[Unset, str] = UNSET
     load_match_command: Union[Unset, str] = UNSET
     server: Union[Unset, "Server"] = UNSET
     guild: Union[Unset, "Guild"] = UNSET
@@ -73,32 +72,29 @@
     map_sides: Union[Unset, Any] = UNSET
     clinch_series: Union[Unset, bool] = UNSET
     cvars: Union[Unset, Any] = UNSET
     players_per_team: Union[Unset, int] = UNSET
     message_id: Union[None, Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
+    winner_team: Union[None, Unset, str] = UNSET
     author: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         team1: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.team1, Unset):
             team1 = self.team1.to_dict()
 
         team2: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.team2, Unset):
             team2 = self.team2.to_dict()
 
-        winner_team: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.winner_team, Unset):
-            winner_team = self.winner_team.to_dict()
-
         maps: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.maps, Unset):
             maps = []
             for maps_item_data in self.maps:
                 maps_item = maps_item_data.to_dict()
                 maps.append(maps_item)
 
@@ -158,14 +154,20 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
+        winner_team: Union[None, Unset, str]
+        if isinstance(self.winner_team, Unset):
+            winner_team = UNSET
+        else:
+            winner_team = self.winner_team
+
         author: Union[None, Unset, str]
         if isinstance(self.author, Unset):
             author = UNSET
         else:
             author = self.author
 
         field_dict: Dict[str, Any] = {}
@@ -173,16 +175,14 @@
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if team1 is not UNSET:
             field_dict["team1"] = team1
         if team2 is not UNSET:
             field_dict["team2"] = team2
-        if winner_team is not UNSET:
-            field_dict["winner_team"] = winner_team
         if maps is not UNSET:
             field_dict["maps"] = maps
         if map_bans is not UNSET:
             field_dict["map_bans"] = map_bans
         if map_picks is not UNSET:
             field_dict["map_picks"] = map_picks
         if connect_command is not UNSET:
@@ -211,14 +211,16 @@
             field_dict["players_per_team"] = players_per_team
         if message_id is not UNSET:
             field_dict["message_id"] = message_id
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
+        if winner_team is not UNSET:
+            field_dict["winner_team"] = winner_team
         if author is not UNSET:
             field_dict["author"] = author
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -242,21 +244,14 @@
         _team2 = d.pop("team2", UNSET)
         team2: Union[Unset, Team]
         if isinstance(_team2, Unset):
             team2 = UNSET
         else:
             team2 = Team.from_dict(_team2)
 
-        _winner_team = d.pop("winner_team", UNSET)
-        winner_team: Union[Unset, Team]
-        if isinstance(_winner_team, Unset):
-            winner_team = UNSET
-        else:
-            winner_team = Team.from_dict(_winner_team)
-
         maps = []
         _maps = d.pop("maps", UNSET)
         for maps_item_data in _maps or []:
             maps_item = Map.from_dict(maps_item_data)
 
             maps.append(maps_item)
 
@@ -337,28 +332,36 @@
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
+        def _parse_winner_team(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        winner_team = _parse_winner_team(d.pop("winner_team", UNSET))
+
         def _parse_author(data: object) -> Union[None, Unset, str]:
             if data is None:
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
 
         author = _parse_author(d.pop("author", UNSET))
 
         patched_match = cls(
             id=id,
             team1=team1,
             team2=team2,
-            winner_team=winner_team,
             maps=maps,
             map_bans=map_bans,
             map_picks=map_picks,
             connect_command=connect_command,
             load_match_command=load_match_command,
             server=server,
             guild=guild,
@@ -369,14 +372,15 @@
             map_sides=map_sides,
             clinch_series=clinch_series,
             cvars=cvars,
             players_per_team=players_per_team,
             message_id=message_id,
             created_at=created_at,
             updated_at=updated_at,
+            winner_team=winner_team,
             author=author,
         )
 
         patched_match.additional_properties = d
         return patched_match
 
     @property
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_player.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_player.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,119 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
+if TYPE_CHECKING:
+    from ..models.discord_user import DiscordUser
+    from ..models.steam_user import SteamUser
+
+
 T = TypeVar("T", bound="PatchedPlayer")
 
 
 @_attrs_define
 class PatchedPlayer:
     """
     Attributes:
         id (Union[Unset, str]):
+        discord_user (Union[Unset, DiscordUser]):
+        steam_user (Union[Unset, SteamUser]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
-        discord_user (Union[Unset, str]):
-        steam_user (Union[Unset, str]):
     """
 
     id: Union[Unset, str] = UNSET
+    discord_user: Union[Unset, "DiscordUser"] = UNSET
+    steam_user: Union[Unset, "SteamUser"] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    discord_user: Union[Unset, str] = UNSET
-    steam_user: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
+        discord_user: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.discord_user, Unset):
+            discord_user = self.discord_user.to_dict()
+
+        steam_user: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.steam_user, Unset):
+            steam_user = self.steam_user.to_dict()
+
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        discord_user = self.discord_user
-
-        steam_user = self.steam_user
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
-        if created_at is not UNSET:
-            field_dict["created_at"] = created_at
-        if updated_at is not UNSET:
-            field_dict["updated_at"] = updated_at
         if discord_user is not UNSET:
             field_dict["discord_user"] = discord_user
         if steam_user is not UNSET:
             field_dict["steam_user"] = steam_user
+        if created_at is not UNSET:
+            field_dict["created_at"] = created_at
+        if updated_at is not UNSET:
+            field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.discord_user import DiscordUser
+        from ..models.steam_user import SteamUser
+
         d = src_dict.copy()
         id = d.pop("id", UNSET)
 
+        _discord_user = d.pop("discord_user", UNSET)
+        discord_user: Union[Unset, DiscordUser]
+        if isinstance(_discord_user, Unset):
+            discord_user = UNSET
+        else:
+            discord_user = DiscordUser.from_dict(_discord_user)
+
+        _steam_user = d.pop("steam_user", UNSET)
+        steam_user: Union[Unset, SteamUser]
+        if isinstance(_steam_user, Unset):
+            steam_user = UNSET
+        else:
+            steam_user = SteamUser.from_dict(_steam_user)
+
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        discord_user = d.pop("discord_user", UNSET)
-
-        steam_user = d.pop("steam_user", UNSET)
-
         patched_player = cls(
             id=id,
-            created_at=created_at,
-            updated_at=updated_at,
             discord_user=discord_user,
             steam_user=steam_user,
+            created_at=created_at,
+            updated_at=updated_at,
         )
 
         patched_player.additional_properties = d
         return patched_player
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_server.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_server.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_steam_user.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_steam_user.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/patched_team.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/patched_team.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
@@ -16,69 +16,67 @@
 
 @_attrs_define
 class PatchedTeam:
     """
     Attributes:
         id (Union[Unset, str]):
         players (Union[Unset, List['Player']]):
+        leader (Union[Unset, Player]):
         name (Union[Unset, str]):
         created_at (Union[Unset, datetime.datetime]):
         updated_at (Union[Unset, datetime.datetime]):
-        leader (Union[None, Unset, str]):
     """
 
     id: Union[Unset, str] = UNSET
     players: Union[Unset, List["Player"]] = UNSET
+    leader: Union[Unset, "Player"] = UNSET
     name: Union[Unset, str] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    leader: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         players: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.players, Unset):
             players = []
             for players_item_data in self.players:
                 players_item = players_item_data.to_dict()
                 players.append(players_item)
 
+        leader: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.leader, Unset):
+            leader = self.leader.to_dict()
+
         name = self.name
 
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        leader: Union[None, Unset, str]
-        if isinstance(self.leader, Unset):
-            leader = UNSET
-        else:
-            leader = self.leader
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if players is not UNSET:
             field_dict["players"] = players
+        if leader is not UNSET:
+            field_dict["leader"] = leader
         if name is not UNSET:
             field_dict["name"] = name
         if created_at is not UNSET:
             field_dict["created_at"] = created_at
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
-        if leader is not UNSET:
-            field_dict["leader"] = leader
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.player import Player
 
@@ -88,14 +86,21 @@
         players = []
         _players = d.pop("players", UNSET)
         for players_item_data in _players or []:
             players_item = Player.from_dict(players_item_data)
 
             players.append(players_item)
 
+        _leader = d.pop("leader", UNSET)
+        leader: Union[Unset, Player]
+        if isinstance(_leader, Unset):
+            leader = UNSET
+        else:
+            leader = Player.from_dict(_leader)
+
         name = d.pop("name", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
@@ -104,30 +109,21 @@
         _updated_at = d.pop("updated_at", UNSET)
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        def _parse_leader(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        leader = _parse_leader(d.pop("leader", UNSET))
-
         patched_team = cls(
             id=id,
             players=players,
+            leader=leader,
             name=name,
             created_at=created_at,
             updated_at=updated_at,
-            leader=leader,
         )
 
         patched_team.additional_properties = d
         return patched_team
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/player.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/player.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,87 @@
 import datetime
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
+if TYPE_CHECKING:
+    from ..models.discord_user import DiscordUser
+    from ..models.steam_user import SteamUser
+
+
 T = TypeVar("T", bound="Player")
 
 
 @_attrs_define
 class Player:
     """
     Attributes:
         id (str):
+        discord_user (DiscordUser):
+        steam_user (SteamUser):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
-        discord_user (str):
-        steam_user (str):
     """
 
     id: str
+    discord_user: "DiscordUser"
+    steam_user: "SteamUser"
     created_at: datetime.datetime
     updated_at: datetime.datetime
-    discord_user: str
-    steam_user: str
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        created_at = self.created_at.isoformat()
+        discord_user = self.discord_user.to_dict()
 
-        updated_at = self.updated_at.isoformat()
+        steam_user = self.steam_user.to_dict()
 
-        discord_user = self.discord_user
+        created_at = self.created_at.isoformat()
 
-        steam_user = self.steam_user
+        updated_at = self.updated_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
-                "created_at": created_at,
-                "updated_at": updated_at,
                 "discord_user": discord_user,
                 "steam_user": steam_user,
+                "created_at": created_at,
+                "updated_at": updated_at,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.discord_user import DiscordUser
+        from ..models.steam_user import SteamUser
+
         d = src_dict.copy()
         id = d.pop("id")
 
-        created_at = isoparse(d.pop("created_at"))
+        discord_user = DiscordUser.from_dict(d.pop("discord_user"))
 
-        updated_at = isoparse(d.pop("updated_at"))
+        steam_user = SteamUser.from_dict(d.pop("steam_user"))
 
-        discord_user = d.pop("discord_user")
+        created_at = isoparse(d.pop("created_at"))
 
-        steam_user = d.pop("steam_user")
+        updated_at = isoparse(d.pop("updated_at"))
 
         player = cls(
             id=id,
-            created_at=created_at,
-            updated_at=updated_at,
             discord_user=discord_user,
             steam_user=steam_user,
+            created_at=created_at,
+            updated_at=updated_at,
         )
 
         player.additional_properties = d
         return player
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/schema_retrieve_lang.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/schema_retrieve_lang.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/schema_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/server.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/server.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/steam_user.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/steam_user.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/models/team.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/models/team.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,69 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
-from ..types import UNSET, Unset
-
 if TYPE_CHECKING:
     from ..models.player import Player
 
 
 T = TypeVar("T", bound="Team")
 
 
 @_attrs_define
 class Team:
     """
     Attributes:
         id (str):
         players (List['Player']):
+        leader (Player):
         name (str):
         created_at (datetime.datetime):
         updated_at (datetime.datetime):
-        leader (Union[None, Unset, str]):
     """
 
     id: str
     players: List["Player"]
+    leader: "Player"
     name: str
     created_at: datetime.datetime
     updated_at: datetime.datetime
-    leader: Union[None, Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         players = []
         for players_item_data in self.players:
             players_item = players_item_data.to_dict()
             players.append(players_item)
 
+        leader = self.leader.to_dict()
+
         name = self.name
 
         created_at = self.created_at.isoformat()
 
         updated_at = self.updated_at.isoformat()
 
-        leader: Union[None, Unset, str]
-        if isinstance(self.leader, Unset):
-            leader = UNSET
-        else:
-            leader = self.leader
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
                 "players": players,
+                "leader": leader,
                 "name": name,
                 "created_at": created_at,
                 "updated_at": updated_at,
             }
         )
-        if leader is not UNSET:
-            field_dict["leader"] = leader
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.player import Player
 
@@ -80,36 +73,29 @@
         players = []
         _players = d.pop("players")
         for players_item_data in _players:
             players_item = Player.from_dict(players_item_data)
 
             players.append(players_item)
 
+        leader = Player.from_dict(d.pop("leader"))
+
         name = d.pop("name")
 
         created_at = isoparse(d.pop("created_at"))
 
         updated_at = isoparse(d.pop("updated_at"))
 
-        def _parse_leader(data: object) -> Union[None, Unset, str]:
-            if data is None:
-                return data
-            if isinstance(data, Unset):
-                return data
-            return cast(Union[None, Unset, str], data)
-
-        leader = _parse_leader(d.pop("leader", UNSET))
-
         team = cls(
             id=id,
             players=players,
+            leader=leader,
             name=name,
             created_at=created_at,
             updated_at=updated_at,
-            leader=leader,
         )
 
         team.additional_properties = d
         return team
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cs2_battle_bot_api_client-0.0.8/cs2_battle_bot_api_client/types.py` & `cs2_battle_bot_api_client-0.0.9/cs2_battle_bot_api_client/types.py`

 * *Files identical despite different names*

### Comparing `cs2_battle_bot_api_client-0.0.8/pyproject.toml` & `cs2_battle_bot_api_client-0.0.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cs2-battle-bot-api-client"
-version = "0.0.8"
+version = "0.0.9"
 description = "A client library for accessing cs2-battle-bot-api"
 authors = []
 readme = "README.md"
 packages = [
     {include = "cs2_battle_bot_api_client"},
 ]
 include = ["CHANGELOG.md", "cs2_battle_bot_api_client/py.typed"]
```

### Comparing `cs2_battle_bot_api_client-0.0.8/PKG-INFO` & `cs2_battle_bot_api_client-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2-battle-bot-api-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client library for accessing cs2-battle-bot-api
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

