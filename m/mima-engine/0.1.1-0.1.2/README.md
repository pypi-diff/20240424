# Comparing `tmp/mima_engine-0.1.1.tar.gz` & `tmp/mima_engine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mima_engine-0.1.1.tar", last modified: Mon Apr 22 18:10:08 2024, max compression
+gzip compressed data, was "mima_engine-0.1.2.tar", last modified: Wed Apr 24 19:02:22 2024, max compression
```

## Comparing `mima_engine-0.1.1.tar` & `mima_engine-0.1.2.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.416019 mima_engine-0.1.1/
--rw-r--r--   0 stephan   (1000) stephan   (1000)      431 2024-04-22 18:10:08.416019 mima_engine-0.1.1/PKG-INFO
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       45 2024-01-11 18:26:25.000000 mima_engine-0.1.1/README.md
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      571 2024-04-22 18:10:04.000000 mima_engine-0.1.1/pyproject.toml
--rw-r--r--   0 stephan   (1000) stephan   (1000)       38 2024-04-22 18:10:08.416019 mima_engine-0.1.1/setup.cfg
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.369352 mima_engine-0.1.1/src/
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.369352 mima_engine-0.1.1/src/mima/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       22 2024-04-22 18:05:27.000000 mima_engine-0.1.1/src/mima/__init__.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.372686 mima_engine-0.1.1/src/mima/backend/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        1 2024-01-17 19:15:04.000000 mima_engine-0.1.1/src/mima/backend/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    12247 2024-04-07 18:39:52.000000 mima_engine-0.1.1/src/mima/backend/pygame_assets.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2320 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/backend/pygame_audio.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    11747 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/backend/pygame_backend.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    16248 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/backend/pygame_events.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6872 2024-04-13 12:54:08.000000 mima_engine-0.1.1/src/mima/collision.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5988 2024-04-11 18:23:32.000000 mima_engine-0.1.1/src/mima/engine.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.376019 mima_engine-0.1.1/src/mima/maps/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1178 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/template.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      639 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tile.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      106 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tile_animation.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      152 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tile_info.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1592 2024-01-17 19:14:33.000000 mima_engine-0.1.1/src/mima/maps/tile_layer.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.379352 mima_engine-0.1.1/src/mima/maps/tiled/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tiled/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1572 2024-01-17 19:14:33.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_layer.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2966 2024-03-17 07:04:12.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_map.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2782 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_object.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      588 2024-03-12 18:51:52.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_objectgroup.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1498 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_template.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3172 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_tile.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1428 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tiled/tiled_tileset.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5026 2024-03-17 07:03:23.000000 mima_engine-0.1.1/src/mima/maps/tilemap.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      819 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tileset.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      136 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/maps/tileset_info.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5021 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/maps/transition_map.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.382686 mima_engine-0.1.1/src/mima/objects/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/objects/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6640 2024-04-13 08:50:14.000000 mima_engine-0.1.1/src/mima/objects/animated_sprite.py
--rw-r--r--   0 stephan   (1000) stephan   (1000)      650 2024-04-10 18:40:00.000000 mima_engine-0.1.1/src/mima/objects/attribute_effect.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3705 2024-04-13 09:14:51.000000 mima_engine-0.1.1/src/mima/objects/attributes.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    11101 2024-04-13 09:45:59.000000 mima_engine-0.1.1/src/mima/objects/creature.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5715 2024-04-13 12:54:40.000000 mima_engine-0.1.1/src/mima/objects/dynamic.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.386019 mima_engine-0.1.1/src/mima/objects/effects/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-03-12 19:17:49.000000 mima_engine-0.1.1/src/mima/objects/effects/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1266 2024-03-19 19:53:24.000000 mima_engine-0.1.1/src/mima/objects/effects/colorize_screen.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3739 2024-04-10 17:23:54.000000 mima_engine-0.1.1/src/mima/objects/effects/light.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1228 2024-03-24 17:58:18.000000 mima_engine-0.1.1/src/mima/objects/effects/walking_on_grass.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1335 2024-03-24 17:58:18.000000 mima_engine-0.1.1/src/mima/objects/effects/walking_on_water.py
--rw-r--r--   0 stephan   (1000) stephan   (1000)     4124 2024-04-11 18:13:27.000000 mima_engine-0.1.1/src/mima/objects/loader.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2506 2024-04-13 09:17:56.000000 mima_engine-0.1.1/src/mima/objects/projectile.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3711 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/objects/sprite.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.389352 mima_engine-0.1.1/src/mima/objects/world/
--rw-r--r--   0 stephan   (1000) stephan   (1000)        0 2024-03-12 19:01:22.000000 mima_engine-0.1.1/src/mima/objects/world/__init__.py
--rw-r--r--   0 stephan   (1000) stephan   (1000)     1948 2024-04-11 18:38:07.000000 mima_engine-0.1.1/src/mima/objects/world/color_gate.py
--rw-r--r--   0 stephan   (1000) stephan   (1000)     3207 2024-04-11 18:36:03.000000 mima_engine-0.1.1/src/mima/objects/world/color_switch.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6001 2024-03-24 18:10:52.000000 mima_engine-0.1.1/src/mima/objects/world/container.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3358 2024-03-24 18:09:43.000000 mima_engine-0.1.1/src/mima/objects/world/floor_switch.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5626 2024-03-24 18:11:06.000000 mima_engine-0.1.1/src/mima/objects/world/gate.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3896 2024-03-24 18:09:57.000000 mima_engine-0.1.1/src/mima/objects/world/light_source.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5048 2024-03-24 18:10:04.000000 mima_engine-0.1.1/src/mima/objects/world/logic_gate.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    10944 2024-03-24 18:10:12.000000 mima_engine-0.1.1/src/mima/objects/world/movable.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5423 2024-03-24 18:10:18.000000 mima_engine-0.1.1/src/mima/objects/world/oneway.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3058 2024-03-30 07:22:27.000000 mima_engine-0.1.1/src/mima/objects/world/pickup.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5559 2024-04-11 17:56:24.000000 mima_engine-0.1.1/src/mima/objects/world/switch.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    10336 2024-03-12 19:20:01.000000 mima_engine-0.1.1/src/mima/objects/world/teleport.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2531 2024-04-11 08:04:19.000000 mima_engine-0.1.1/src/mima/scene_engine.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.392686 mima_engine-0.1.1/src/mima/scripts/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       75 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/scripts/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      434 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/scripts/command.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.402685 mima_engine-0.1.1/src/mima/scripts/commands/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-13 21:38:10.000000 mima_engine-0.1.1/src/mima/scripts/commands/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      387 2024-01-12 14:30:20.000000 mima_engine-0.1.1/src/mima/scripts/commands/add_quest.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      449 2024-03-19 19:04:43.000000 mima_engine-0.1.1/src/mima/scripts/commands/change_map.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      207 2024-03-28 21:24:53.000000 mima_engine-0.1.1/src/mima/scripts/commands/close_dialog.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      561 2024-03-24 18:06:10.000000 mima_engine-0.1.1/src/mima/scripts/commands/give_item.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1805 2024-03-24 18:06:27.000000 mima_engine-0.1.1/src/mima/scripts/commands/give_resource.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     4756 2024-03-30 10:52:29.000000 mima_engine-0.1.1/src/mima/scripts/commands/move_map.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1420 2024-01-12 14:30:20.000000 mima_engine-0.1.1/src/mima/scripts/commands/move_to.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1683 2024-03-24 18:08:35.000000 mima_engine-0.1.1/src/mima/scripts/commands/oneway_move.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1489 2024-03-12 19:06:23.000000 mima_engine-0.1.1/src/mima/scripts/commands/parallel.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      348 2024-03-28 17:00:25.000000 mima_engine-0.1.1/src/mima/scripts/commands/play_sound.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1648 2024-03-29 16:15:32.000000 mima_engine-0.1.1/src/mima/scripts/commands/present_item.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      359 2024-03-30 12:05:05.000000 mima_engine-0.1.1/src/mima/scripts/commands/progress_quest.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      219 2024-04-09 18:28:36.000000 mima_engine-0.1.1/src/mima/scripts/commands/quit_game.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      392 2024-04-13 09:58:11.000000 mima_engine-0.1.1/src/mima/scripts/commands/save_game.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1729 2024-03-12 19:19:06.000000 mima_engine-0.1.1/src/mima/scripts/commands/screen_fade.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1548 2024-03-12 19:06:02.000000 mima_engine-0.1.1/src/mima/scripts/commands/serial.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      567 2024-03-12 19:05:10.000000 mima_engine-0.1.1/src/mima/scripts/commands/set_facing_direction.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      434 2024-04-07 18:14:07.000000 mima_engine-0.1.1/src/mima/scripts/commands/set_spawn_map.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1382 2024-03-28 21:25:28.000000 mima_engine-0.1.1/src/mima/scripts/commands/show_choices.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      278 2024-03-24 18:07:05.000000 mima_engine-0.1.1/src/mima/scripts/commands/show_dialog.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      573 2024-03-28 21:25:52.000000 mima_engine-0.1.1/src/mima/scripts/commands/take_coins.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1177 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/scripts/script_processor.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.402685 mima_engine-0.1.1/src/mima/states/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/states/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5013 2024-04-13 18:33:25.000000 mima_engine-0.1.1/src/mima/states/game_state.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2365 2024-04-07 18:14:58.000000 mima_engine-0.1.1/src/mima/states/quest.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.409352 mima_engine-0.1.1/src/mima/types/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       89 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/alignment.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       96 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/blend.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      584 2024-01-16 19:24:19.000000 mima_engine-0.1.1/src/mima/types/damage.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1116 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/direction.py
--rw-r--r--   0 stephan   (1000) stephan   (1000)       86 2024-04-11 18:23:57.000000 mima_engine-0.1.1/src/mima/types/gate_color.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      308 2024-03-30 11:40:10.000000 mima_engine-0.1.1/src/mima/types/graphic_state.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      183 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/keys.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      233 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/mode.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      159 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/nature.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      377 2024-04-11 18:35:29.000000 mima_engine-0.1.1/src/mima/types/object.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       80 2024-03-24 09:25:11.000000 mima_engine-0.1.1/src/mima/types/start.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      130 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/types/terrain.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       87 2024-03-23 16:51:26.000000 mima_engine-0.1.1/src/mima/types/weapon_slot.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.409352 mima_engine-0.1.1/src/mima/usables/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/usables/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      883 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/usables/item.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1269 2024-04-11 07:07:45.000000 mima_engine-0.1.1/src/mima/usables/weapon.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.412685 mima_engine-0.1.1/src/mima/util/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       42 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/util/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1268 2024-03-24 09:28:33.000000 mima_engine-0.1.1/src/mima/util/colors.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1233 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/util/constants.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      524 2024-01-17 19:38:40.000000 mima_engine-0.1.1/src/mima/util/functions.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      759 2024-01-17 19:14:33.000000 mima_engine-0.1.1/src/mima/util/input_defaults.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1197 2024-01-14 08:28:14.000000 mima_engine-0.1.1/src/mima/util/logging.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)      107 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/util/property.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3975 2024-01-17 19:15:05.000000 mima_engine-0.1.1/src/mima/util/runtime_config.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.416019 mima_engine-0.1.1/src/mima/view/
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.1/src/mima/view/__init__.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1779 2024-04-13 08:39:54.000000 mima_engine-0.1.1/src/mima/view/camera.py
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)    12118 2024-04-13 09:05:24.000000 mima_engine-0.1.1/src/mima/view/scene.py
-drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-22 18:10:08.416019 mima_engine-0.1.1/src/mima_engine.egg-info/
--rw-r--r--   0 stephan   (1000) stephan   (1000)      431 2024-04-22 18:10:08.000000 mima_engine-0.1.1/src/mima_engine.egg-info/PKG-INFO
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3781 2024-04-22 18:10:08.000000 mima_engine-0.1.1/src/mima_engine.egg-info/SOURCES.txt
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        1 2024-04-22 18:10:08.000000 mima_engine-0.1.1/src/mima_engine.egg-info/dependency_links.txt
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)       20 2024-04-22 18:10:08.000000 mima_engine-0.1.1/src/mima_engine.egg-info/requires.txt
--rwxr-xr-x   0 stephan   (1000) stephan   (1000)        5 2024-04-22 18:10:08.000000 mima_engine-0.1.1/src/mima_engine.egg-info/top_level.txt
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.097364 mima_engine-0.1.2/
+-rw-r--r--   0 stephan   (1000) stephan   (1000)      431 2024-04-24 19:02:22.097364 mima_engine-0.1.2/PKG-INFO
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       45 2024-01-11 18:26:25.000000 mima_engine-0.1.2/README.md
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      571 2024-04-22 18:10:04.000000 mima_engine-0.1.2/pyproject.toml
+-rw-r--r--   0 stephan   (1000) stephan   (1000)       38 2024-04-24 19:02:22.097364 mima_engine-0.1.2/setup.cfg
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.084030 mima_engine-0.1.2/src/
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.084030 mima_engine-0.1.2/src/mima/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       22 2024-04-24 19:01:23.000000 mima_engine-0.1.2/src/mima/__init__.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.084030 mima_engine-0.1.2/src/mima/backend/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        1 2024-01-17 19:15:04.000000 mima_engine-0.1.2/src/mima/backend/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    11793 2024-04-24 18:41:56.000000 mima_engine-0.1.2/src/mima/backend/pygame_assets.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2320 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/backend/pygame_audio.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    11747 2024-01-17 19:15:05.000000 mima_engine-0.1.2/src/mima/backend/pygame_backend.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    16248 2024-01-17 19:15:05.000000 mima_engine-0.1.2/src/mima/backend/pygame_events.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6872 2024-04-13 12:54:08.000000 mima_engine-0.1.2/src/mima/collision.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6106 2024-04-24 18:06:05.000000 mima_engine-0.1.2/src/mima/engine.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.087364 mima_engine-0.1.2/src/mima/maps/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1178 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/template.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      639 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tile.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      106 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tile_animation.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      152 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tile_info.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1592 2024-01-17 19:14:33.000000 mima_engine-0.1.2/src/mima/maps/tile_layer.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.087364 mima_engine-0.1.2/src/mima/maps/tiled/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tiled/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1572 2024-01-17 19:14:33.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_layer.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2966 2024-03-17 07:04:12.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_map.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2782 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_object.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      588 2024-03-12 18:51:52.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_objectgroup.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1498 2024-01-17 19:15:05.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_template.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3172 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_tile.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1428 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tiled/tiled_tileset.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5026 2024-03-17 07:03:23.000000 mima_engine-0.1.2/src/mima/maps/tilemap.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      819 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tileset.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      136 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/maps/tileset_info.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5021 2024-01-17 19:15:05.000000 mima_engine-0.1.2/src/mima/maps/transition_map.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.087364 mima_engine-0.1.2/src/mima/objects/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/objects/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6640 2024-04-13 08:50:14.000000 mima_engine-0.1.2/src/mima/objects/animated_sprite.py
+-rw-r--r--   0 stephan   (1000) stephan   (1000)      650 2024-04-10 18:40:00.000000 mima_engine-0.1.2/src/mima/objects/attribute_effect.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3705 2024-04-13 09:14:51.000000 mima_engine-0.1.2/src/mima/objects/attributes.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    11101 2024-04-13 09:45:59.000000 mima_engine-0.1.2/src/mima/objects/creature.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5715 2024-04-13 12:54:40.000000 mima_engine-0.1.2/src/mima/objects/dynamic.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.087364 mima_engine-0.1.2/src/mima/objects/effects/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-03-12 19:17:49.000000 mima_engine-0.1.2/src/mima/objects/effects/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1266 2024-03-19 19:53:24.000000 mima_engine-0.1.2/src/mima/objects/effects/colorize_screen.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3739 2024-04-10 17:23:54.000000 mima_engine-0.1.2/src/mima/objects/effects/light.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1228 2024-03-24 17:58:18.000000 mima_engine-0.1.2/src/mima/objects/effects/walking_on_grass.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1335 2024-03-24 17:58:18.000000 mima_engine-0.1.2/src/mima/objects/effects/walking_on_water.py
+-rw-r--r--   0 stephan   (1000) stephan   (1000)     4124 2024-04-11 18:13:27.000000 mima_engine-0.1.2/src/mima/objects/loader.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2506 2024-04-13 09:17:56.000000 mima_engine-0.1.2/src/mima/objects/projectile.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3711 2024-01-17 19:15:05.000000 mima_engine-0.1.2/src/mima/objects/sprite.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.090697 mima_engine-0.1.2/src/mima/objects/world/
+-rw-r--r--   0 stephan   (1000) stephan   (1000)        0 2024-03-12 19:01:22.000000 mima_engine-0.1.2/src/mima/objects/world/__init__.py
+-rw-r--r--   0 stephan   (1000) stephan   (1000)     1948 2024-04-11 18:38:07.000000 mima_engine-0.1.2/src/mima/objects/world/color_gate.py
+-rw-r--r--   0 stephan   (1000) stephan   (1000)     3207 2024-04-11 18:36:03.000000 mima_engine-0.1.2/src/mima/objects/world/color_switch.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     6001 2024-03-24 18:10:52.000000 mima_engine-0.1.2/src/mima/objects/world/container.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3358 2024-03-24 18:09:43.000000 mima_engine-0.1.2/src/mima/objects/world/floor_switch.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5626 2024-03-24 18:11:06.000000 mima_engine-0.1.2/src/mima/objects/world/gate.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3896 2024-03-24 18:09:57.000000 mima_engine-0.1.2/src/mima/objects/world/light_source.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5048 2024-03-24 18:10:04.000000 mima_engine-0.1.2/src/mima/objects/world/logic_gate.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    10944 2024-03-24 18:10:12.000000 mima_engine-0.1.2/src/mima/objects/world/movable.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5423 2024-03-24 18:10:18.000000 mima_engine-0.1.2/src/mima/objects/world/oneway.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3058 2024-03-30 07:22:27.000000 mima_engine-0.1.2/src/mima/objects/world/pickup.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5559 2024-04-11 17:56:24.000000 mima_engine-0.1.2/src/mima/objects/world/switch.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    10336 2024-03-12 19:20:01.000000 mima_engine-0.1.2/src/mima/objects/world/teleport.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2678 2024-04-24 18:20:28.000000 mima_engine-0.1.2/src/mima/scene_engine.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.090697 mima_engine-0.1.2/src/mima/scripts/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       75 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/scripts/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      434 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/scripts/command.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.094030 mima_engine-0.1.2/src/mima/scripts/commands/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-13 21:38:10.000000 mima_engine-0.1.2/src/mima/scripts/commands/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      387 2024-01-12 14:30:20.000000 mima_engine-0.1.2/src/mima/scripts/commands/add_quest.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      449 2024-03-19 19:04:43.000000 mima_engine-0.1.2/src/mima/scripts/commands/change_map.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      207 2024-03-28 21:24:53.000000 mima_engine-0.1.2/src/mima/scripts/commands/close_dialog.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      561 2024-03-24 18:06:10.000000 mima_engine-0.1.2/src/mima/scripts/commands/give_item.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1805 2024-03-24 18:06:27.000000 mima_engine-0.1.2/src/mima/scripts/commands/give_resource.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     4756 2024-03-30 10:52:29.000000 mima_engine-0.1.2/src/mima/scripts/commands/move_map.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1420 2024-01-12 14:30:20.000000 mima_engine-0.1.2/src/mima/scripts/commands/move_to.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1683 2024-03-24 18:08:35.000000 mima_engine-0.1.2/src/mima/scripts/commands/oneway_move.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1489 2024-03-12 19:06:23.000000 mima_engine-0.1.2/src/mima/scripts/commands/parallel.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      348 2024-03-28 17:00:25.000000 mima_engine-0.1.2/src/mima/scripts/commands/play_sound.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1648 2024-03-29 16:15:32.000000 mima_engine-0.1.2/src/mima/scripts/commands/present_item.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      359 2024-03-30 12:05:05.000000 mima_engine-0.1.2/src/mima/scripts/commands/progress_quest.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      219 2024-04-09 18:28:36.000000 mima_engine-0.1.2/src/mima/scripts/commands/quit_game.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      392 2024-04-13 09:58:11.000000 mima_engine-0.1.2/src/mima/scripts/commands/save_game.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1729 2024-03-12 19:19:06.000000 mima_engine-0.1.2/src/mima/scripts/commands/screen_fade.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1548 2024-03-12 19:06:02.000000 mima_engine-0.1.2/src/mima/scripts/commands/serial.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      567 2024-03-12 19:05:10.000000 mima_engine-0.1.2/src/mima/scripts/commands/set_facing_direction.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      434 2024-04-07 18:14:07.000000 mima_engine-0.1.2/src/mima/scripts/commands/set_spawn_map.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1382 2024-03-28 21:25:28.000000 mima_engine-0.1.2/src/mima/scripts/commands/show_choices.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      278 2024-03-24 18:07:05.000000 mima_engine-0.1.2/src/mima/scripts/commands/show_dialog.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      573 2024-03-28 21:25:52.000000 mima_engine-0.1.2/src/mima/scripts/commands/take_coins.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1177 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/scripts/script_processor.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.094030 mima_engine-0.1.2/src/mima/states/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/states/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     5013 2024-04-13 18:33:25.000000 mima_engine-0.1.2/src/mima/states/game_state.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     2365 2024-04-07 18:14:58.000000 mima_engine-0.1.2/src/mima/states/quest.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.094030 mima_engine-0.1.2/src/mima/types/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       89 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/alignment.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       96 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/blend.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      584 2024-01-16 19:24:19.000000 mima_engine-0.1.2/src/mima/types/damage.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1116 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/direction.py
+-rw-r--r--   0 stephan   (1000) stephan   (1000)       86 2024-04-11 18:23:57.000000 mima_engine-0.1.2/src/mima/types/gate_color.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      308 2024-03-30 11:40:10.000000 mima_engine-0.1.2/src/mima/types/graphic_state.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      183 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/keys.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      233 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/mode.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      159 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/nature.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      377 2024-04-11 18:35:29.000000 mima_engine-0.1.2/src/mima/types/object.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       80 2024-03-24 09:25:11.000000 mima_engine-0.1.2/src/mima/types/start.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      130 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/types/terrain.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       87 2024-03-23 16:51:26.000000 mima_engine-0.1.2/src/mima/types/weapon_slot.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.094030 mima_engine-0.1.2/src/mima/usables/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/usables/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      883 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/usables/item.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1269 2024-04-11 07:07:45.000000 mima_engine-0.1.2/src/mima/usables/weapon.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.097364 mima_engine-0.1.2/src/mima/util/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       42 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/util/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1268 2024-03-24 09:28:33.000000 mima_engine-0.1.2/src/mima/util/colors.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1233 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/util/constants.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      524 2024-01-17 19:38:40.000000 mima_engine-0.1.2/src/mima/util/functions.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      759 2024-01-17 19:14:33.000000 mima_engine-0.1.2/src/mima/util/input_defaults.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1197 2024-01-14 08:28:14.000000 mima_engine-0.1.2/src/mima/util/logging.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)      107 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/util/property.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3803 2024-04-24 18:41:43.000000 mima_engine-0.1.2/src/mima/util/runtime_config.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.097364 mima_engine-0.1.2/src/mima/view/
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-01-11 18:26:25.000000 mima_engine-0.1.2/src/mima/view/__init__.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     1779 2024-04-13 08:39:54.000000 mima_engine-0.1.2/src/mima/view/camera.py
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)    12118 2024-04-13 09:05:24.000000 mima_engine-0.1.2/src/mima/view/scene.py
+drwxr-xr-x   0 stephan   (1000) stephan   (1000)        0 2024-04-24 19:02:22.097364 mima_engine-0.1.2/src/mima_engine.egg-info/
+-rw-r--r--   0 stephan   (1000) stephan   (1000)      431 2024-04-24 19:02:22.000000 mima_engine-0.1.2/src/mima_engine.egg-info/PKG-INFO
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)     3781 2024-04-24 19:02:22.000000 mima_engine-0.1.2/src/mima_engine.egg-info/SOURCES.txt
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        1 2024-04-24 19:02:22.000000 mima_engine-0.1.2/src/mima_engine.egg-info/dependency_links.txt
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)       20 2024-04-24 19:02:22.000000 mima_engine-0.1.2/src/mima_engine.egg-info/requires.txt
+-rwxr-xr-x   0 stephan   (1000) stephan   (1000)        5 2024-04-24 19:02:22.000000 mima_engine-0.1.2/src/mima_engine.egg-info/top_level.txt
```

### Comparing `mima_engine-0.1.1/pyproject.toml` & `mima_engine-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/backend/pygame_assets.py` & `mima_engine-0.1.2/src/mima/backend/pygame_assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 import csv
 import logging
 import os
 from typing import TYPE_CHECKING, Dict, Optional
 
 import pygame
 
-# from ...maps.object_loader import ObjectLoader
 from ..maps.tiled.tiled_map import TiledMap
 from ..maps.tiled.tiled_template import TiledTemplate
 from ..maps.tiled.tiled_tileset import TiledTileset
-from ..util.colors import (
-    WHITE,
-)  # GB_DARK,; GB_LIGHT,; GB_MEDIUM_DARK,; GB_MEDIUM_LIGHT,; TEXT_COLOR,
+from ..util.colors import WHITE
 
-# from .game.tilemap import Tilemap
 if TYPE_CHECKING:
     from ..util import RuntimeConfig
 
 LOG = logging.getLogger(__name__)
 
 
 class PygameAssets:
@@ -28,15 +24,14 @@
         self._sprites: Dict[str, pygame.Surface] = {}
         self._tilesets: Dict[str, TiledTileset] = {}
         self._templates: Dict[str, TiledTemplate] = {}
         self._maps: Dict[str, TiledMap] = {}
         self._music: Dict[str, str] = {}
         self._sound: Dict[str, str] = {}
         self._csvs: Dict[str, str] = {}
-        # self._items: Dict[str, Item] = {}
         self._assets_to_load: Dict[str, str] = {}
         self._assets_to_preload: Dict[str, str] = {}
         self._paths: Dict[str, str] = {}
         self.data_path = ""
         self._preprocess_asset_file(init_file)
 
     def _preprocess_asset_file(self, init_file: str):
@@ -322,24 +317,22 @@
         return self._csvs[name]
 
     def _load_sprite_from_disk(self, filename: str) -> pygame.Surface:
         if "color" in filename:
             return pygame.image.load(filename).convert_alpha()
         else:
             image = pygame.image.load(filename).convert_alpha()
-            # var = pygame.PixelArray(image)
-            # # var.replace((0, 0, 0, 0), (255, 0, 0, 255))
-            # if "font" in filename:
-            #     var.replace(WHITE.getRGB(), TEXT_COLOR.getRGBA())
-
-            # var.replace(GB_DARK.getRGBA(), self.rtc.colors["gb_dark"].getRGBA())
-            # var.replace(
-            #     GB_MEDIUM_DARK.getRGBA(),
-            #     self.rtc.colors["gb_medium_dark"].getRGBA(),
-            # )
-            # var.replace(
-            #     GB_MEDIUM_LIGHT.getRGBA(),
-            #     self.rtc.colors["gb_medium_light"].getRGBA(),
-            # )
-            # var.replace(GB_LIGHT.getRGBA(), self.rtc.colors["gb_light"].getRGBA())
-            # del var
+            var = pygame.PixelArray(image)
+
+            new_colors = {
+                name: color
+                for name, color in self.rtc.colors.items()
+                if f"{name}_default" in self.rtc.colors
+            }
+            for name, new_color in new_colors.items():
+                var.replace(
+                    self.rtc.colors[f"{name}_default"].getRGBA(),
+                    new_color.getRGBA(),
+                )
+
+            del var
             return image
```

### Comparing `mima_engine-0.1.1/src/mima/backend/pygame_audio.py` & `mima_engine-0.1.2/src/mima/backend/pygame_audio.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/backend/pygame_backend.py` & `mima_engine-0.1.2/src/mima/backend/pygame_backend.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/backend/pygame_events.py` & `mima_engine-0.1.2/src/mima/backend/pygame_events.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/collision.py` & `mima_engine-0.1.2/src/mima/collision.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/engine.py` & `mima_engine-0.1.2/src/mima/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,35 @@
 from .maps.tilemap import Tilemap
 from .objects.animated_sprite import AnimatedSprite
 from .objects.creature import Creature
 from .objects.dynamic import Dynamic
 from .objects.sprite import Sprite
 from .scripts import Command, ScriptProcessor
 from .states.quest import Quest
-from .types.mode import Mode
 from .types.gate_color import GateColor
+from .types.mode import Mode
 from .usables.item import Item
 from .util import RuntimeConfig
 from .util.logging import install_trace_logger
 from .view.camera import Camera
 from .view.scene import Scene
 
 LOG = logging.getLogger(__name__)
 
 
 class MimaEngine(ABC):
     def __init__(
-        self, init_file: str, platform: str = "PC", caption: str = "MimaEngine"
+        self,
+        init_file: str,
+        config_path: str,
+        default_config: Dict[str, Any],
+        platform: str = "PC",
+        caption: str = "MimaEngine",
     ):
-        self.rtc = RuntimeConfig()
+        self.rtc = RuntimeConfig(config_path, default_config)
         install_trace_logger()
 
         self.backend: PygameBackend = PygameBackend(
             self.rtc, init_file, platform
         )
 
         self._caption: str = caption
```

### Comparing `mima_engine-0.1.1/src/mima/maps/template.py` & `mima_engine-0.1.2/src/mima/maps/template.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tile.py` & `mima_engine-0.1.2/src/mima/maps/tile.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tile_layer.py` & `mima_engine-0.1.2/src/mima/maps/tile_layer.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_layer.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_layer.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_map.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_map.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_object.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_object.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_objectgroup.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_objectgroup.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_template.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_template.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_tile.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_tile.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tiled/tiled_tileset.py` & `mima_engine-0.1.2/src/mima/maps/tiled/tiled_tileset.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tilemap.py` & `mima_engine-0.1.2/src/mima/maps/tilemap.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/tileset.py` & `mima_engine-0.1.2/src/mima/maps/tileset.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/maps/transition_map.py` & `mima_engine-0.1.2/src/mima/maps/transition_map.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/animated_sprite.py` & `mima_engine-0.1.2/src/mima/objects/animated_sprite.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/attribute_effect.py` & `mima_engine-0.1.2/src/mima/objects/attribute_effect.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/attributes.py` & `mima_engine-0.1.2/src/mima/objects/attributes.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/creature.py` & `mima_engine-0.1.2/src/mima/objects/creature.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/dynamic.py` & `mima_engine-0.1.2/src/mima/objects/dynamic.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/effects/colorize_screen.py` & `mima_engine-0.1.2/src/mima/objects/effects/colorize_screen.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/effects/light.py` & `mima_engine-0.1.2/src/mima/objects/effects/light.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/effects/walking_on_grass.py` & `mima_engine-0.1.2/src/mima/objects/effects/walking_on_grass.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/effects/walking_on_water.py` & `mima_engine-0.1.2/src/mima/objects/effects/walking_on_water.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/loader.py` & `mima_engine-0.1.2/src/mima/objects/loader.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/projectile.py` & `mima_engine-0.1.2/src/mima/objects/projectile.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/sprite.py` & `mima_engine-0.1.2/src/mima/objects/sprite.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/color_gate.py` & `mima_engine-0.1.2/src/mima/objects/world/color_gate.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/color_switch.py` & `mima_engine-0.1.2/src/mima/objects/world/color_switch.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/container.py` & `mima_engine-0.1.2/src/mima/objects/world/container.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/floor_switch.py` & `mima_engine-0.1.2/src/mima/objects/world/floor_switch.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/gate.py` & `mima_engine-0.1.2/src/mima/objects/world/gate.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/light_source.py` & `mima_engine-0.1.2/src/mima/objects/world/light_source.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/logic_gate.py` & `mima_engine-0.1.2/src/mima/objects/world/logic_gate.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/movable.py` & `mima_engine-0.1.2/src/mima/objects/world/movable.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/oneway.py` & `mima_engine-0.1.2/src/mima/objects/world/oneway.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/pickup.py` & `mima_engine-0.1.2/src/mima/objects/world/pickup.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/switch.py` & `mima_engine-0.1.2/src/mima/objects/world/switch.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/objects/world/teleport.py` & `mima_engine-0.1.2/src/mima/objects/world/teleport.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scene_engine.py` & `mima_engine-0.1.2/src/mima/scene_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Dict, List, Optional, Union, Any
 
 from .engine import MimaEngine
 from .states.game_state import GameState
 from .types.keys import Key as K
+from .types.mode import Mode
 from .types.nature import Nature
 from .view.scene import Scene
-from .types.mode import Mode
 
 
 class MimaSceneEngine(MimaEngine):
     def __init__(
-        self, init_file: str, platform: str = "PC", caption: str = "MimaEngine"
+        self,
+        init_file: str,
+        config_path: str,
+        default_config: Dict[str, Any],
+        platform: str = "PC",
+        caption: str = "MimaEngine",
     ):
-        super().__init__(init_file, platform, caption)
+        super().__init__(
+            init_file, config_path, default_config, platform, caption
+        )
 
         self.scene_stack: List[str] = []
         self._scenes: Dict[str, Scene] = {}
         self._current_scene: Scene
 
         self.all_games: Dict[str, GameState] = {}
         self.current_game: str = ""
```

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/give_item.py` & `mima_engine-0.1.2/src/mima/scripts/commands/give_item.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/give_resource.py` & `mima_engine-0.1.2/src/mima/scripts/commands/give_resource.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/move_map.py` & `mima_engine-0.1.2/src/mima/scripts/commands/move_map.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/move_to.py` & `mima_engine-0.1.2/src/mima/scripts/commands/move_to.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/oneway_move.py` & `mima_engine-0.1.2/src/mima/scripts/commands/oneway_move.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/parallel.py` & `mima_engine-0.1.2/src/mima/scripts/commands/parallel.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/present_item.py` & `mima_engine-0.1.2/src/mima/scripts/commands/present_item.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/screen_fade.py` & `mima_engine-0.1.2/src/mima/scripts/commands/screen_fade.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/serial.py` & `mima_engine-0.1.2/src/mima/scripts/commands/serial.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/set_facing_direction.py` & `mima_engine-0.1.2/src/mima/scripts/commands/set_facing_direction.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/show_choices.py` & `mima_engine-0.1.2/src/mima/scripts/commands/show_choices.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/commands/take_coins.py` & `mima_engine-0.1.2/src/mima/scripts/commands/take_coins.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/scripts/script_processor.py` & `mima_engine-0.1.2/src/mima/scripts/script_processor.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/states/game_state.py` & `mima_engine-0.1.2/src/mima/states/game_state.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/states/quest.py` & `mima_engine-0.1.2/src/mima/states/quest.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/types/damage.py` & `mima_engine-0.1.2/src/mima/types/damage.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/types/direction.py` & `mima_engine-0.1.2/src/mima/types/direction.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/usables/item.py` & `mima_engine-0.1.2/src/mima/usables/item.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/usables/weapon.py` & `mima_engine-0.1.2/src/mima/usables/weapon.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/colors.py` & `mima_engine-0.1.2/src/mima/util/colors.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/constants.py` & `mima_engine-0.1.2/src/mima/util/constants.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/functions.py` & `mima_engine-0.1.2/src/mima/util/functions.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/input_defaults.py` & `mima_engine-0.1.2/src/mima/util/input_defaults.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/logging.py` & `mima_engine-0.1.2/src/mima/util/logging.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/util/runtime_config.py` & `mima_engine-0.1.2/src/mima/util/runtime_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import configparser
 import os
 from copy import deepcopy
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from ..types.keys import Key as K
 from .colors import Color
 from .functions import strtobool
 
 DEFAULT_CONFIG = {
     "keymap": {
@@ -18,27 +18,30 @@
         "X": "l",
         "Y": "j",
         "L": "o",
         "R": "c",
         "START": "i",
         "SELECT": "t",
     },
-    "colors": {
-        "gb_dark": "42,0,0",
-        "gb_medium_dark": "91,86,95",
-        "gb_medium_light": "186,191,181",
-        "gb_light": "255,255,241",
-    },
-    "flags": {"use_color": "false"},
+    "colors": {},
+    "color_remaps": {},
+    "flags": {},
 }
 
 
 class RuntimeConfig:
-    def __init__(self, config_path: str = ""):
-        self._loaded: Dict[str, Any] = deepcopy(DEFAULT_CONFIG)
+    def __init__(
+        self,
+        config_path: str = "",
+        default_config: Optional[Dict[str, Any]] = None,
+    ):
+        if default_config is None:
+            default_config = DEFAULT_CONFIG
+
+        self._loaded: Dict[str, Any] = deepcopy(default_config)
         self._converted: Dict[str, Any] = {}
 
         if not config_path:
             config_path = os.path.abspath(
                 os.path.join(os.getcwd(), "avenight.ini")
             )
 
@@ -58,42 +61,37 @@
             self._write_config(config)
 
     def _read_config(self, config: configparser.ConfigParser):
         for key, mapping in config["keymap"].items():
             vals = mapping.strip().split(",")
             self._loaded["keymap"][key.upper()] = vals
 
-        self._loaded["colors"]["gb_dark"] = config["colors"]["gb_dark"]
-        self._loaded["colors"]["gb_medium_dark"] = config["colors"][
-            "gb_medium_dark"
-        ]
-        self._loaded["colors"]["gb_medium_light"] = config["colors"][
-            "gb_medium_light"
-        ]
-        self._loaded["colors"]["gb_light"] = config["colors"]["gb_light"]
+        default_colors = {}
+        for color_name, color in self._loaded["colors"].items():
+            default_colors[f"{color_name}_default"] = color
+            self._loaded["colors"][color_name] = config["colors"][color_name]
+        self._loaded["colors"].update(default_colors)
 
-        self._loaded["flags"]["use_color"] = config["flags"]["use_color"]
+        for flag in self._loaded["flags"]:
+            self._loaded["flags"][flag] = config["flags"][flag]
 
     def _write_config(self, config: configparser.ConfigParser):
         config["keymap"] = {}
         config["colors"] = {}
         config["flags"] = {}
         for key, mapping in self._loaded["keymap"].items():
             config["keymap"][key.lower()] = mapping
 
-        config["colors"]["gb_dark"] = self._loaded["colors"]["gb_dark"]
-        config["colors"]["gb_medium_dark"] = self._loaded["colors"][
-            "gb_medium_dark"
-        ]
-        config["colors"]["gb_medium_light"] = self._loaded["colors"][
-            "gb_medium_light"
-        ]
-        config["colors"]["gb_light"] = self._loaded["colors"]["gb_light"]
+        for color_name, color in self._loaded["colors"].items():
+            if color_name.endswith("_default"):
+                continue
+            config["colors"][color_name] = color
 
-        config["flags"]["use_color"] = self._loaded["flags"]["use_color"]
+        for flag_name, flag in self._loaded["flags"]:
+            config["flags"][flag_name] = flag
 
         with open(self._config_path, "w") as cfg_file:
             config.write(cfg_file)
 
     @property
     def keymap(self):
         if "keymap" in self._converted:
@@ -122,12 +120,11 @@
 
     @property
     def flags(self) -> Dict[str, bool]:
         if "flags" in self._converted:
             return self._converted["flags"]
         else:
             self._converted["flags"] = {}
-            self._converted["flags"]["use_color"] = strtobool(
-                self._loaded["flags"]["use_color"]
-            )
+            for flag, value in self._loaded["flags"].items():
+                self._converted["flags"][flag] = strtobool(value)
 
             return self._converted["flags"]
```

### Comparing `mima_engine-0.1.1/src/mima/view/camera.py` & `mima_engine-0.1.2/src/mima/view/camera.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima/view/scene.py` & `mima_engine-0.1.2/src/mima/view/scene.py`

 * *Files identical despite different names*

### Comparing `mima_engine-0.1.1/src/mima_engine.egg-info/SOURCES.txt` & `mima_engine-0.1.2/src/mima_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

