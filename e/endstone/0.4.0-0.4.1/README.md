# Comparing `tmp/endstone-0.4.0.tar.gz` & `tmp/endstone-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endstone-0.4.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "endstone-0.4.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `endstone-0.4.0.tar` & `endstone-0.4.1.tar`

### file list

```diff
@@ -1,281 +1,291 @@
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 endstone-0.4.0/.clang-format
--rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 endstone-0.4.0/.clang-tidy
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 endstone-0.4.0/.dockerignore
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 endstone-0.4.0/.git_archival.txt
--rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/conan_profiles/linux
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/conan_profiles/windows
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/linux.yml
--rw-r--r--   0        0        0     5258 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/wheel.yml
--rw-r--r--   0        0        0     1167 2022-11-09 12:37:21.000000 endstone-0.4.0/.github/workflows/windows.yml
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 endstone-0.4.0/.gitignore
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 endstone-0.4.0/.readthedocs.yaml
--rw-r--r--   0        0        0     4674 2022-11-09 12:37:21.000000 endstone-0.4.0/CMakeLists.txt
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 endstone-0.4.0/Dockerfile
--rw-r--r--   0        0        0    11356 2022-11-09 12:37:21.000000 endstone-0.4.0/LICENSE
--rw-r--r--   0        0        0     8645 2022-11-09 12:37:21.000000 endstone-0.4.0/README.md
--rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 endstone-0.4.0/codecov.yml
--rw-r--r--   0        0        0     6535 2022-11-09 12:37:21.000000 endstone-0.4.0/conanfile.py
--rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 endstone-0.4.0/docker-compose.yml
--rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 endstone-0.4.0/docs/index.md
--rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 endstone-0.4.0/docs/requirements.txt
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/automatic_id.h
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/bedrock.h
--rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/bedrock_log.h
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command.h
--rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_context.h
--rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_flag.h
--rw-r--r--   0        0        0     4945 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_origin.h
--rw-r--r--   0        0        0     1996 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_output.h
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_permission_level.h
--rw-r--r--   0        0        0    12075 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_registry.h
--rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_utils.h
--rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/command_version.h
--rw-r--r--   0        0        0     1596 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/command/minecraft_commands.h
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/common.h
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/core.h
--rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/details.h
--rw-r--r--   0        0        0     5062 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/forward.h
--rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/i18n.h
--rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/mce.h
--rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/memory.h
--rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/minecraft.h
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/network_identifier.h
--rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/certificate.h
--rw-r--r--   0        0        0     2132 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/game/available_commands_packet.h
--rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/game/text_packet.h
--rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/minecraft_packets.h
--rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/packet.h
--rw-r--r--   0        0        0      822 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/packet_sender.h
--rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/protocol/sub_client_id.h
--rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/raknet/socket2.h
--rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/network/raknet/types.h
--rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/level/server_level.h
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/level/server_player.h
--rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/network/server_network_handler.h
--rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/server/server_instance.h
--rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/threading.h
--rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/type_id.h
--rw-r--r--   0        0        0    12542 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor.h
--rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_initialization_method.h
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_runtime_id.h
--rw-r--r--   0        0        0      740 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/actor_unique_id.h
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/abilities_component.h
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/actor_owner_component.h
--rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/actor_unique_id_component.h
--rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/runtime_id_component.h
--rw-r--r--   0        0        0     1160 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/components/user_entity_identifier_component.h
--rw-r--r--   0        0        0     3163 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/mob/mob.h
--rw-r--r--   0        0        0      973 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/permissions_handler.h
--rw-r--r--   0        0        0     5687 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/player.h
--rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/player/player_permission_level.h
--rw-r--r--   0        0        0     2624 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/registry/entity_context.h
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/actor/registry/entity_registry.h
--rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension.h
--rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension_height_range.h
--rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/dimension_interface.h
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/dimension/vanilla_dimensions.h
--rw-r--r--   0        0        0     3703 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/actor_event.h
--rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/block_event.h
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/coordinator_result.h
--rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_coordinator.h
--rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_ref.h
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/event_result.h
--rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/gameplay_handler.h
--rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/item_event.h
--rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/level_event.h
--rw-r--r--   0        0        0     5082 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/player_event.h
--rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/event/server_event.h
--rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level.h
--rw-r--r--   0        0        0    28182 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level_interface.h
--rw-r--r--   0        0        0      735 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/level_listener.h
--rw-r--r--   0        0        0      905 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/level/storage/saved_data.h
--rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 endstone-0.4.0/include/bedrock/world/math/vec3.h
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/actor/actor.h
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/actor/human.h
--rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/color_format.h
--rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command.h
--rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_executor.h
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_map.h
--rw-r--r--   0        0        0     2055 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/command_sender.h
--rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/command/plugin_command.h
--rw-r--r--   0        0        0     2238 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/actor/actor.h
--rw-r--r--   0        0        0     2160 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/actor/human.h
--rw-r--r--   0        0        0     2431 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/cast.h
--rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/bedrock_command.h
--rw-r--r--   0        0        0     1652 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_adapter.h
--rw-r--r--   0        0        0     2923 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_lexer.h
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_map.h
--rw-r--r--   0        0        0     1751 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_sender.h
--rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/command_usage_parser.h
--rw-r--r--   0        0        0      951 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/debug_command.h
--rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/plugins_command.h
--rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/defaults/version_command.h
--rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/endstone_command.h
--rw-r--r--   0        0        0     1094 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/command/server_command_sender.h
--rw-r--r--   0        0        0     5808 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/hook.h
--rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/level.h
--rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/logger_factory.h
--rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/os.h
--rw-r--r--   0        0        0     1502 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/permissions/default_permissions.h
--rw-r--r--   0        0        0     2513 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/permissions/permissible_base.h
--rw-r--r--   0        0        0     2417 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/player.h
--rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/cpp_plugin_loader.h
--rw-r--r--   0        0        0     5357 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/plugin_description_builder.h
--rw-r--r--   0        0        0     3882 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/plugin_manager.h
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/plugin/python_plugin_loader.h
--rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/pybind_type_caster.h
--rw-r--r--   0        0        0     2766 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/server.h
--rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/signal_handler.h
--rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/level_formatter.h
--rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/log_sink.h
--rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/spdlog_adapter.h
--rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/spdlog/text_formatter.h
--rw-r--r--   0        0        0     2947 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/detail/virtual_table.h
--rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/dimension.h
--rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/endstone.h
--rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_event.h
--rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_remove_event.h
--rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/actor/actor_spawn_event.h
--rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event.h
--rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event_handler.h
--rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/event_priority.h
--rw-r--r--   0        0        0     3747 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/handler_list.h
--rw-r--r--   0        0        0     1768 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_chat_event.h
--rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_event.h
--rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_join_event.h
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/player/player_quit_event.h
--rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/plugin_disable_event.h
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/plugin_enable_event.h
--rw-r--r--   0        0        0     2246 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_command_event.h
--rw-r--r--   0        0        0     5526 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_list_ping_event.h
--rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/server/server_load_event.h
--rw-r--r--   0        0        0     1527 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/thunder_change_event.h
--rw-r--r--   0        0        0     1531 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/weather_change_event.h
--rw-r--r--   0        0        0     1152 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/event/weather/weather_event.h
--rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/game_mode.h
--rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/level.h
--rw-r--r--   0        0        0     3495 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/logger.h
--rw-r--r--   0        0        0     4267 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permissible.h
--rw-r--r--   0        0        0     5770 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission.h
--rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_attachment.h
--rw-r--r--   0        0        0     2204 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_attachment_info.h
--rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/permissions/permission_default.h
--rw-r--r--   0        0        0     1707 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/player.h
--rw-r--r--   0        0        0     7348 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin.h
--rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_description.h
--rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_load_order.h
--rw-r--r--   0        0        0     3062 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_loader.h
--rw-r--r--   0        0        0     8500 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/plugin/plugin_manager.h
--rw-r--r--   0        0        0     3596 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/server.h
--rw-r--r--   0        0        0     4223 2022-11-09 12:37:21.000000 endstone-0.4.0/include/endstone/util/uuid.h
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 endstone-0.4.0/python/.gitignore
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/__init__.py
--rw-r--r--   0        0        0     3110 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/__init__.py
--rw-r--r--   0        0        0    10393 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/base.py
--rw-r--r--   0        0        0     2178 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/linux.py
--rw-r--r--   0        0        0     7266 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/bootstrap/windows.py
--rw-r--r--   0        0        0    37546 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/endstone_python.pyi
--rw-r--r--   0        0        0     4090 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/plugin_loader.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/_internal/version.py
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/actor.py
--rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/command.py
--rw-r--r--   0        0        0     1084 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/event.py
--rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/permissions.py
--rw-r--r--   0        0        0     5200 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/plugin.py
--rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 endstone-0.4.0/python/src/endstone/util.py
--rw-r--r--   0        0        0     1630 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_color_format.py
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_imports.py
--rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 endstone-0.4.0/python/tests/test_plugin_description.py
--rw-r--r--   0        0        0     2562 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/actor/actor.cpp
--rw-r--r--   0        0        0     2687 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/actor/human.cpp
--rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/bedrock_command.cpp
--rw-r--r--   0        0        0     5046 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_adapter.cpp
--rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_lexer.cpp
--rw-r--r--   0        0        0     9109 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_map.cpp
--rw-r--r--   0        0        0     2179 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_sender.cpp
--rw-r--r--   0        0        0     4793 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/command_usage_parser.cpp
--rw-r--r--   0        0        0     1845 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/debug_command.cpp
--rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/plugins_command.cpp
--rw-r--r--   0        0        0     3846 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/defaults/version_command.cpp
--rw-r--r--   0        0        0     1325 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/command/server_command_sender.cpp
--rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/event/server/server_list_ping_event.cpp
--rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/level.cpp
--rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/logger_factory.cpp
--rw-r--r--   0        0        0     2750 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/permissions/default_permissions.cpp
--rw-r--r--   0        0        0     6405 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/permissions/permissible_base.cpp
--rw-r--r--   0        0        0     4513 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/player.cpp
--rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/plugin/cpp_plugin_loader.cpp
--rw-r--r--   0        0        0    11062 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/plugin/plugin_manager.cpp
--rw-r--r--   0        0        0     5425 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/server.cpp
--rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/level_formatter.cpp
--rw-r--r--   0        0        0     3601 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/log_sink.cpp
--rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/spdlog_adapter.cpp
--rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_core/spdlog/text_formatter.cpp
--rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/actor.cpp
--rw-r--r--   0        0        0     4917 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/command.cpp
--rw-r--r--   0        0        0    11142 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/endstone_python.cpp
--rw-r--r--   0        0        0     8623 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/event.cpp
--rw-r--r--   0        0        0     8641 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/permissions.cpp
--rw-r--r--   0        0        0    16268 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/plugin.cpp
--rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_python/util.cpp
--rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/bedrock_log.cpp
--rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command.cpp
--rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_output.cpp
--rw-r--r--   0        0        0     4960 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_registry.cpp
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/command_utils.cpp
--rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/command/minecraft_commands.cpp
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/common.cpp
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/i18n.cpp
--rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/minecraft.cpp
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/protocol/minecraft_packets.cpp
--rw-r--r--   0        0        0     3401 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/socket2.cpp
--rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/types.cpp
--rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_level.cpp
--rw-r--r--   0        0        0     1462 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_player.cpp
--rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/network/server_network_handler.cpp
--rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/server/server_instance.cpp
--rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/threading.cpp
--rw-r--r--   0        0        0     2907 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/actor.cpp
--rw-r--r--   0        0        0     2074 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/player/player.cpp
--rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/dimension/dimension.cpp
--rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/dimension/vanilla_dimensions.cpp
--rw-r--r--   0        0        0     7382 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/event_coordinator.cpp
--rw-r--r--   0        0        0     3196 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/gameplay_handler.cpp
--rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/hook.cpp
--rw-r--r--   0        0        0     4343 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/hook.cpp
--rw-r--r--   0        0        0     2660 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/os.cpp
--rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/linux/signal_handler.cpp
--rw-r--r--   0        0        0     3759 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/magic.cpp
--rw-r--r--   0        0        0     2491 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/main.cpp
--rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/plugin/python_plugin_loader.cpp
--rw-r--r--   0        0        0     4776 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/hook.cpp
--rw-r--r--   0        0        0     2661 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/os.cpp
--rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 endstone-0.4.0/src/endstone_runtime/windows/signal_handler.cpp
--rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/command/test_command_lexer.cpp
--rw-r--r--   0        0        0     8575 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/command/test_command_usage_parser.cpp
--rw-r--r--   0        0        0     3696 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/plugin/test_cpp_plugin_loader.cpp
--rw-r--r--   0        0        0     1750 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/plugin/test_plugin.cpp
--rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 endstone-0.4.0/tests/test_logger_factory.cpp
--rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/.gitignore
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/conandata.yml
--rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/conanfile.py
--rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch
--rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/CMakeLists.txt
--rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/conanfile.py
--rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test.c
--rw-r--r--   0        0        0     2249 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_noasm.c
--rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_masm.asm
--rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S
--rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_masm.asm
--rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/suffix.list
--rw-r--r--   0        0        0    20695 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/test_main.c
--rw-r--r--   0        0        0    10659 2022-11-09 12:37:21.000000 endstone-0.4.0/third_party/funchook/test_package/x86_test.S
--rw-r--r--   0        0        0    22834 2022-11-09 12:37:21.000000 endstone-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 endstone-0.4.1/.clang-format
+-rw-r--r--   0        0        0     4248 2022-11-09 12:37:21.000000 endstone-0.4.1/.clang-tidy
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 endstone-0.4.1/.dockerignore
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 endstone-0.4.1/.git_archival.txt
+-rw-r--r--   0        0        0      219 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/conan_profiles/linux
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/conan_profiles/windows
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2251 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/workflows/linux.yml
+-rw-r--r--   0        0        0     5258 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0     1167 2022-11-09 12:37:21.000000 endstone-0.4.1/.github/workflows/windows.yml
+-rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 endstone-0.4.1/.gitignore
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 endstone-0.4.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     4737 2022-11-09 12:37:21.000000 endstone-0.4.1/CMakeLists.txt
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 endstone-0.4.1/Dockerfile
+-rw-r--r--   0        0        0    11356 2022-11-09 12:37:21.000000 endstone-0.4.1/LICENSE
+-rw-r--r--   0        0        0     8711 2022-11-09 12:37:21.000000 endstone-0.4.1/README.md
+-rw-r--r--   0        0        0       88 2022-11-09 12:37:21.000000 endstone-0.4.1/codecov.yml
+-rw-r--r--   0        0        0     6232 2022-11-09 12:37:21.000000 endstone-0.4.1/conanfile.py
+-rw-r--r--   0        0        0      315 2022-11-09 12:37:21.000000 endstone-0.4.1/docker-compose.yml
+-rw-r--r--   0        0        0      491 2022-11-09 12:37:21.000000 endstone-0.4.1/docs/index.md
+-rw-r--r--   0        0        0       16 2022-11-09 12:37:21.000000 endstone-0.4.1/docs/requirements.txt
+-rw-r--r--   0        0        0      943 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/automatic_id.h
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/bedrock.h
+-rw-r--r--   0        0        0     1777 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/bedrock_log.h
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command.h
+-rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_context.h
+-rw-r--r--   0        0        0     2106 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_flag.h
+-rw-r--r--   0        0        0     4945 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_origin.h
+-rw-r--r--   0        0        0     1996 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_output.h
+-rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_permission_level.h
+-rw-r--r--   0        0        0    12075 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_registry.h
+-rw-r--r--   0        0        0      836 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_utils.h
+-rw-r--r--   0        0        0      715 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/command_version.h
+-rw-r--r--   0        0        0     1596 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/command/minecraft_commands.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/common.h
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/core.h
+-rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/details.h
+-rw-r--r--   0        0        0     5281 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/forward.h
+-rw-r--r--   0        0        0     3892 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/i18n.h
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/mce.h
+-rw-r--r--   0        0        0     1303 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/memory.h
+-rw-r--r--   0        0        0      814 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/minecraft.h
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/network_identifier.h
+-rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/certificate.h
+-rw-r--r--   0        0        0     2132 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/game/available_commands_packet.h
+-rw-r--r--   0        0        0     1495 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/game/text_packet.h
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/minecraft_packets.h
+-rw-r--r--   0        0        0     1001 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/packet.h
+-rw-r--r--   0        0        0      822 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/packet_sender.h
+-rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/protocol/sub_client_id.h
+-rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/raknet/socket2.h
+-rw-r--r--   0        0        0     1126 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/network/raknet/types.h
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/server/command/say_command.h
+-rw-r--r--   0        0        0      987 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/server/level/server_level.h
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/server/level/server_player.h
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/server/network/server_network_handler.h
+-rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/server/server_instance.h
+-rw-r--r--   0        0        0      998 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/threading.h
+-rw-r--r--   0        0        0      941 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/type_id.h
+-rw-r--r--   0        0        0    12514 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/actor.h
+-rw-r--r--   0        0        0      843 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/actor_initialization_method.h
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/actor_runtime_id.h
+-rw-r--r--   0        0        0      740 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/actor_unique_id.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/abilities_component.h
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/actor_owner_component.h
+-rw-r--r--   0        0        0      759 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/actor_unique_id_component.h
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/flag_component.h
+-rw-r--r--   0        0        0      756 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/runtime_id_component.h
+-rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/components/user_entity_identifier_component.h
+-rw-r--r--   0        0        0     3102 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/mob/mob.h
+-rw-r--r--   0        0        0      973 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/player/permissions_handler.h
+-rw-r--r--   0        0        0     5687 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/player/player.h
+-rw-r--r--   0        0        0      773 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/player/player_permission_level.h
+-rw-r--r--   0        0        0     2776 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/registry/entity_context.h
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/actor/registry/entity_registry.h
+-rw-r--r--   0        0        0     1801 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/dimension/dimension.h
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/dimension/dimension_height_range.h
+-rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/dimension/dimension_interface.h
+-rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/dimension/vanilla_dimensions.h
+-rw-r--r--   0        0        0     3703 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/actor_event.h
+-rw-r--r--   0        0        0     2655 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/block_event.h
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/coordinator_result.h
+-rw-r--r--   0        0        0     2642 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/event_coordinator.h
+-rw-r--r--   0        0        0      729 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/event_ref.h
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/event_result.h
+-rw-r--r--   0        0        0     1324 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/gameplay_handler.h
+-rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/item_event.h
+-rw-r--r--   0        0        0     2313 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/level_event.h
+-rw-r--r--   0        0        0     5082 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/player_event.h
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/event/server_event.h
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/level.h
+-rw-r--r--   0        0        0    27305 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/level_interface.h
+-rw-r--r--   0        0        0      735 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/level_listener.h
+-rw-r--r--   0        0        0      905 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/level/storage/saved_data.h
+-rw-r--r--   0        0        0      725 2022-11-09 12:37:21.000000 endstone-0.4.1/include/bedrock/world/math/vec3.h
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/actor/actor.h
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/actor/human.h
+-rw-r--r--   0        0        0     2863 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/color_format.h
+-rw-r--r--   0        0        0     7632 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/command/command.h
+-rw-r--r--   0        0        0     1419 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/command/command_executor.h
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/command/command_map.h
+-rw-r--r--   0        0        0     2180 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/command/command_sender.h
+-rw-r--r--   0        0        0     2767 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/command/plugin_command.h
+-rw-r--r--   0        0        0     2254 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/actor/actor.h
+-rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/actor/human.h
+-rw-r--r--   0        0        0     2431 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/cast.h
+-rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/bedrock_command.h
+-rw-r--r--   0        0        0     1654 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/command_adapter.h
+-rw-r--r--   0        0        0     2923 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/command_lexer.h
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/command_map.h
+-rw-r--r--   0        0        0     1494 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/command_usage_parser.h
+-rw-r--r--   0        0        0     1104 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/console_command_sender.h
+-rw-r--r--   0        0        0     1018 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/defaults/plugins_command.h
+-rw-r--r--   0        0        0     1162 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/defaults/version_command.h
+-rw-r--r--   0        0        0      842 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/endstone_command.h
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/command/server_command_sender.h
+-rw-r--r--   0        0        0     5808 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/hook.h
+-rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/level.h
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/logger_factory.h
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/os.h
+-rw-r--r--   0        0        0     1568 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/permissions/default_permissions.h
+-rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/permissions/permissible_base.h
+-rw-r--r--   0        0        0     2441 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/player.h
+-rw-r--r--   0        0        0     1226 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/plugin/cpp_plugin_loader.h
+-rw-r--r--   0        0        0     5357 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/plugin/plugin_description_builder.h
+-rw-r--r--   0        0        0     3882 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/plugin/plugin_manager.h
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/plugin/python_plugin_loader.h
+-rw-r--r--   0        0        0     3035 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/pybind_type_caster.h
+-rw-r--r--   0        0        0     1401 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/scheduler/scheduler.h
+-rw-r--r--   0        0        0     1942 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/scheduler/task.h
+-rw-r--r--   0        0        0     2934 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/server.h
+-rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/signal_handler.h
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/spdlog/level_formatter.h
+-rw-r--r--   0        0        0     3184 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/spdlog/log_sink.h
+-rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/spdlog/spdlog_adapter.h
+-rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/spdlog/text_formatter.h
+-rw-r--r--   0        0        0     2947 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/detail/virtual_table.h
+-rw-r--r--   0        0        0      785 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/dimension.h
+-rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/endstone.h
+-rw-r--r--   0        0        0     1195 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/actor/actor_event.h
+-rw-r--r--   0        0        0     1429 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/actor/actor_remove_event.h
+-rw-r--r--   0        0        0     1329 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/actor/actor_spawn_event.h
+-rw-r--r--   0        0        0     3097 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/event.h
+-rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/event_handler.h
+-rw-r--r--   0        0        0     1716 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/event_priority.h
+-rw-r--r--   0        0        0     3747 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/handler_list.h
+-rw-r--r--   0        0        0     1768 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/player/player_chat_event.h
+-rw-r--r--   0        0        0     1802 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/player/player_command_event.h
+-rw-r--r--   0        0        0     1157 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/player/player_event.h
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/player/player_join_event.h
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/player/player_quit_event.h
+-rw-r--r--   0        0        0     2331 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/broadcast_message_event.h
+-rw-r--r--   0        0        0     1413 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/plugin_disable_event.h
+-rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/plugin_enable_event.h
+-rw-r--r--   0        0        0     2250 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/server_command_event.h
+-rw-r--r--   0        0        0     5526 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/server_list_ping_event.h
+-rw-r--r--   0        0        0     1352 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/server/server_load_event.h
+-rw-r--r--   0        0        0     1527 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/weather/thunder_change_event.h
+-rw-r--r--   0        0        0     1531 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/weather/weather_change_event.h
+-rw-r--r--   0        0        0     1152 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/event/weather/weather_event.h
+-rw-r--r--   0        0        0     1363 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/game_mode.h
+-rw-r--r--   0        0        0     1543 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/level.h
+-rw-r--r--   0        0        0     3495 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/logger.h
+-rw-r--r--   0        0        0     4365 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/permissions/permissible.h
+-rw-r--r--   0        0        0     5770 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/permissions/permission.h
+-rw-r--r--   0        0        0     4597 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/permissions/permission_attachment.h
+-rw-r--r--   0        0        0     2204 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/permissions/permission_attachment_info.h
+-rw-r--r--   0        0        0      796 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/permissions/permission_default.h
+-rw-r--r--   0        0        0     1707 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/player.h
+-rw-r--r--   0        0        0     7348 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/plugin/plugin.h
+-rw-r--r--   0        0        0     7486 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/plugin/plugin_description.h
+-rw-r--r--   0        0        0     1042 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/plugin/plugin_load_order.h
+-rw-r--r--   0        0        0     3062 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/plugin/plugin_loader.h
+-rw-r--r--   0        0        0     8500 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/plugin/plugin_manager.h
+-rw-r--r--   0        0        0     3083 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/scheduler/scheduler.h
+-rw-r--r--   0        0        0     1604 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/scheduler/task.h
+-rw-r--r--   0        0        0     4379 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/server.h
+-rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 endstone-0.4.1/include/endstone/util/uuid.h
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 endstone-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 endstone-0.4.1/python/.gitignore
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/__init__.py
+-rw-r--r--   0        0        0     3110 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/bootstrap/__init__.py
+-rw-r--r--   0        0        0    10393 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/bootstrap/base.py
+-rw-r--r--   0        0        0     2178 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/bootstrap/linux.py
+-rw-r--r--   0        0        0     7266 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/bootstrap/windows.py
+-rw-r--r--   0        0        0    38316 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/endstone_python.pyi
+-rw-r--r--   0        0        0     4090 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/plugin_loader.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/_internal/version.py
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/actor.py
+-rw-r--r--   0        0        0      146 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/command.py
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/event.py
+-rw-r--r--   0        0        0      277 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/permissions.py
+-rw-r--r--   0        0        0     5200 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/plugin.py
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 endstone-0.4.1/python/src/endstone/util.py
+-rw-r--r--   0        0        0     1630 2022-11-09 12:37:21.000000 endstone-0.4.1/python/tests/test_color_format.py
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 endstone-0.4.1/python/tests/test_imports.py
+-rw-r--r--   0        0        0     2315 2022-11-09 12:37:21.000000 endstone-0.4.1/python/tests/test_plugin_description.py
+-rw-r--r--   0        0        0     2986 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/actor/actor.cpp
+-rw-r--r--   0        0        0     2687 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/actor/human.cpp
+-rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/bedrock_command.cpp
+-rw-r--r--   0        0        0     5046 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/command_adapter.cpp
+-rw-r--r--   0        0        0     3153 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/command_lexer.cpp
+-rw-r--r--   0        0        0     8932 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/command_map.cpp
+-rw-r--r--   0        0        0     4793 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/command_usage_parser.cpp
+-rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/console_command_sender.cpp
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/defaults/plugins_command.cpp
+-rw-r--r--   0        0        0     3846 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/defaults/version_command.cpp
+-rw-r--r--   0        0        0     2214 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/command/server_command_sender.cpp
+-rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/event/server/server_list_ping_event.cpp
+-rw-r--r--   0        0        0     2086 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/level.cpp
+-rw-r--r--   0        0        0     1514 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/logger_factory.cpp
+-rw-r--r--   0        0        0     3174 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/permissions/default_permissions.cpp
+-rw-r--r--   0        0        0     6823 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/permissions/permissible_base.cpp
+-rw-r--r--   0        0        0     4618 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/player.cpp
+-rw-r--r--   0        0        0     4796 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/plugin/cpp_plugin_loader.cpp
+-rw-r--r--   0        0        0    11064 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/plugin/plugin_manager.cpp
+-rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/scheduler/scheduler.cpp
+-rw-r--r--   0        0        0     1944 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/scheduler/task.cpp
+-rw-r--r--   0        0        0     6294 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/server.cpp
+-rw-r--r--   0        0        0     1553 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/spdlog/level_formatter.cpp
+-rw-r--r--   0        0        0     3601 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/spdlog/log_sink.cpp
+-rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/spdlog/spdlog_adapter.cpp
+-rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_core/spdlog/text_formatter.cpp
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/actor.cpp
+-rw-r--r--   0        0        0     4917 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/command.cpp
+-rw-r--r--   0        0        0    11142 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/endstone_python.cpp
+-rw-r--r--   0        0        0     9681 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/event.cpp
+-rw-r--r--   0        0        0     8641 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/permissions.cpp
+-rw-r--r--   0        0        0    16268 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/plugin.cpp
+-rw-r--r--   0        0        0      803 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_python/util.cpp
+-rw-r--r--   0        0        0     2402 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/bedrock_log.cpp
+-rw-r--r--   0        0        0      889 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/command/command.cpp
+-rw-r--r--   0        0        0     1542 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/command/command_output.cpp
+-rw-r--r--   0        0        0     4960 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/command/command_registry.cpp
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/command/command_utils.cpp
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/command/minecraft_commands.cpp
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/common.cpp
+-rw-r--r--   0        0        0      780 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/i18n.cpp
+-rw-r--r--   0        0        0      876 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/minecraft.cpp
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/network/protocol/minecraft_packets.cpp
+-rw-r--r--   0        0        0     3401 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/network/raknet/socket2.cpp
+-rw-r--r--   0        0        0     1086 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/network/raknet/types.cpp
+-rw-r--r--   0        0        0     1313 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/server/command/say_command.cpp
+-rw-r--r--   0        0        0     1377 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/server/level/server_level.cpp
+-rw-r--r--   0        0        0     1550 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/server/level/server_player.cpp
+-rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/server/network/server_network_handler.cpp
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/server/server_instance.cpp
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/threading.cpp
+-rw-r--r--   0        0        0     3063 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/actor/actor.cpp
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/actor/player/player.cpp
+-rw-r--r--   0        0        0      760 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/level/dimension/dimension.cpp
+-rw-r--r--   0        0        0      977 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/level/dimension/vanilla_dimensions.cpp
+-rw-r--r--   0        0        0     7438 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/level/event/event_coordinator.cpp
+-rw-r--r--   0        0        0     3196 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/bedrock/world/level/event/gameplay_handler.cpp
+-rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/hook.cpp
+-rw-r--r--   0        0        0     4343 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/linux/hook.cpp
+-rw-r--r--   0        0        0     2660 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/linux/os.cpp
+-rw-r--r--   0        0        0     1734 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/linux/signal_handler.cpp
+-rw-r--r--   0        0        0     3759 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/magic.cpp
+-rw-r--r--   0        0        0     2491 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/main.cpp
+-rw-r--r--   0        0        0     2088 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/plugin/python_plugin_loader.cpp
+-rw-r--r--   0        0        0     4776 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/windows/hook.cpp
+-rw-r--r--   0        0        0     2661 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/windows/os.cpp
+-rw-r--r--   0        0        0     1696 2022-11-09 12:37:21.000000 endstone-0.4.1/src/endstone_runtime/windows/signal_handler.cpp
+-rw-r--r--   0        0        0     4234 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/command/test_command_lexer.cpp
+-rw-r--r--   0        0        0     8575 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/command/test_command_usage_parser.cpp
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/plugin/test_cpp_plugin_loader.cpp
+-rw-r--r--   0        0        0     1750 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/plugin/test_plugin.cpp
+-rw-r--r--   0        0        0     1781 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/test_logger_factory.cpp
+-rw-r--r--   0        0        0     1237 2022-11-09 12:37:21.000000 endstone-0.4.1/tests/util/test_uuid.cpp
+-rw-r--r--   0        0        0     1621 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/.gitignore
+-rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/conandata.yml
+-rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/conanfile.py
+-rw-r--r--   0        0        0     2134 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch
+-rw-r--r--   0        0        0     1506 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/CMakeLists.txt
+-rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/conanfile.py
+-rw-r--r--   0        0        0      477 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test.c
+-rw-r--r--   0        0        0     2249 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_noasm.c
+-rw-r--r--   0        0        0     1060 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_64_masm.asm
+-rw-r--r--   0        0        0     2634 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_gas.S
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_masm.asm
+-rw-r--r--   0        0        0     4092 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/suffix.list
+-rw-r--r--   0        0        0    20695 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/test_main.c
+-rw-r--r--   0        0        0    10659 2022-11-09 12:37:21.000000 endstone-0.4.1/third_party/funchook/test_package/x86_test.S
+-rw-r--r--   0        0        0    22900 2022-11-09 12:37:21.000000 endstone-0.4.1/PKG-INFO
```

### Comparing `endstone-0.4.0/.clang-format` & `endstone-0.4.1/.clang-format`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.clang-tidy` & `endstone-0.4.1/.clang-tidy`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.github/workflows/coverage.yml` & `endstone-0.4.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.github/workflows/docker.yml` & `endstone-0.4.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.github/workflows/linux.yml` & `endstone-0.4.1/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.github/workflows/wheel.yml` & `endstone-0.4.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/.github/workflows/windows.yml` & `endstone-0.4.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/CMakeLists.txt` & `endstone-0.4.1/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,29 @@
 find_package(Python COMPONENTS Interpreter Development REQUIRED)
 find_package(pybind11 CONFIG REQUIRED)
 find_package(spdlog CONFIG REQUIRED)
 find_package(funchook CONFIG REQUIRED)
 find_package(magic_enum CONFIG REQUIRED)
 find_package(EnTT CONFIG REQUIRED)
 find_package(cpptrace CONFIG REQUIRED)
+find_package(Microsoft.GSL CONFIG REQUIRED)
 if (UNIX)
     find_package(libelf CONFIG REQUIRED)
 endif ()
 
 find_package(GTest CONFIG REQUIRED)
 
 
 # =================
 # endstone::headers
 # =================
 add_library(endstone_headers INTERFACE)
 add_library(endstone::headers ALIAS endstone_headers)
 target_include_directories(endstone_headers INTERFACE include)
-target_link_libraries(endstone_headers INTERFACE fmt::fmt EnTT::EnTT)
+target_link_libraries(endstone_headers INTERFACE fmt::fmt)
 
 include(GNUInstallDirs)
 install(DIRECTORY include/ DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
 
 
 # ================
 # endstone::python
@@ -61,15 +62,15 @@
 
 # ==============
 # endstone::core
 # ==============
 file(GLOB_RECURSE ENDSTONE_CORE_SOURCE_FILES CONFIGURE_DEPENDS "src/endstone_core/*.cpp")
 add_library(endstone_core ${ENDSTONE_CORE_SOURCE_FILES})
 add_library(endstone::core ALIAS endstone_core)
-target_link_libraries(endstone_core PUBLIC endstone::headers spdlog::spdlog magic_enum::magic_enum)
+target_link_libraries(endstone_core PUBLIC endstone::headers spdlog::spdlog magic_enum::magic_enum EnTT::EnTT Microsoft.GSL::GSL)
 if (UNIX)
     target_link_libraries(endstone_core PUBLIC ${CMAKE_DL_LIBS})
 endif ()
 target_compile_definitions(endstone_core PUBLIC ENDSTONE_VERSION="${ENDSTONE_VERSION}")
 
 include(GNUInstallDirs)
 install(TARGETS endstone_core
```

### Comparing `endstone-0.4.0/Dockerfile` & `endstone-0.4.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/LICENSE` & `endstone-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/README.md` & `endstone-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 </p>
 
 [![Windows](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml)
 [![Linux](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml)
 [![Wheel](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml)
 [![Docker](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml)
 [![Documentation](https://img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/)
-[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
+[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.80%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
 [![PyPI - Version](https://img.shields.io/pypi/v/endstone)](https://pypi.org/project/endstone)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
 [![Python](https://img.shields.io/badge/Python-3-blue?logo=python&logoColor=white)](https://www.python.org/)
 [![GitHub License](https://img.shields.io/github/license/endstonemc/endstone)](LICENSE)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8877402fc70b40f5a8c4b325d890e3f7?logo=codacy)](https://app.codacy.com/gh/EndstoneMC/endstone/dashboard)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -78,30 +78,33 @@
 ```shell
 pip install endstone
 endstone
 ```
 
 ### 🐳 Docker
 
-To try Endstone from a Docker image, use the following command:
+To try Endstone from the latest Docker image, use the following command:
 
 ```shell
 docker pull endstone/endstone
 docker run --rm -it -p 19132:19132/udp endstone/endstone
 ```
 
-or
+This will pull the latest Endstone image and run it interactively in your terminal.
+
+### 🕋 Docker Compose
+
+You can also use Docker Compose to run Endstone in a production environment.
 
 ```shell
-docker pull ghcr.io/endstonemc/endstone
-docker run --rm -it -p 19132:19132/udp ghcr.io/endstonemc/endstone
+docker compose build
+docker compose up -d
+docker attach endstone
 ```
 
-This will pull the latest Endstone image and run it interactively in your terminal.
-
 ### 🔨 Build locally from Source
 
 For advanced users, you may build Endstone locally from the source.
 
 **Please note that building from source requires toolchains to be installed on your system.**
 
 |                                  | Windows                       | Linux    |
@@ -150,15 +153,15 @@
 - [Python Example Plugin](https://github.com/EndstoneMC/python-plugin-template)
 
 | Milestone                                | Duration   | Core | C++ API | Python API | Since  |
 |------------------------------------------|------------|------|---------|------------|--------|
 | **🔌 Plugin Loader**                     | 1-2 months | ✅    | ✅       | ✅          | v0.1.0 |
 | **⌨️ Command System**                    | 2-3 months | ✅    | ✅       | ✅          | v0.2.0 |
 | **🔐 Permission System**                 | 2-3 months | ✅    | ✅       | ✅          | v0.3.0 |
-| **🎈 Event System**                      | 2-3 months | 🚧   | ✅       | ✅          |        |
+| **🎈 Event System**                      | 2-3 months | ✅    | ✅       | ✅          | v0.4.0 |
 | **🛠 Minecraft Core Features**           | 4-5 months | ⏳    | ⏳       | ⏳          |        |
 | **🖼 GUI & Inventory System**            | 3-4 months | ⏳    | ⏳       | ⏳          |        |
 | **🌟 Advanced Features & Refinements**   | 4-6 months | ⏳    | ⏳       | ⏳          |        |
 | **🧪 Beta Testing & Community Feedback** | 3 months   | ⏳    | ⏳       | ⏳          |        |
 | **🚀 Official Release & Support**        | -          | ⏳    | ⏳       | ⏳          |        |
 
 Here's a legend to guide you:
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/
 actions/workflows/linux.yml) [![Wheel](https://github.com/EndstoneMC/endstone/
 actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/
 actions/workflows/wheel.yml) [![Docker](https://github.com/EndstoneMC/endstone/
     actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/
        endstone/actions/workflows/docker.yml) [![Documentation](https://
   img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/) [!
-   [Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20
+   [Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.80%20
       (Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/
   360001186971-Release-Changelogs) [![PyPI - Version](https://img.shields.io/
    pypi/v/endstone)](https://pypi.org/project/endstone) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
                [![Python](https://img.shields.io/badge/Python-3-
 blue?logo=python&logoColor=white)](https://www.python.org/) [![GitHub License]
 (https://img.shields.io/github/license/endstonemc/endstone)](LICENSE) [![Codacy
@@ -48,58 +48,59 @@
 of-contents) Before getting started, verify that you are using one of the
 following compatible operating systems: - Windows 10 version 10.0.15063 or
 later - Windows Server 2016 or later - Debian 11 or later - Ubuntu 20.04 or
 later Please also ensure you have **Python 3.9 or higher** installed on your
 system. There are several ways to install Endstone: ### ð PyPi Endstone can
 be installed directly from PyPi using pip. Open your terminal and execute the
 following command to install and start the Endstone server: ```shell pip
-install endstone endstone ``` ### ð³ Docker To try Endstone from a Docker
-image, use the following command: ```shell docker pull endstone/endstone docker
-run --rm -it -p 19132:19132/udp endstone/endstone ``` or ```shell docker pull
-ghcr.io/endstonemc/endstone docker run --rm -it -p 19132:19132/udp ghcr.io/
-endstonemc/endstone ``` This will pull the latest Endstone image and run it
-interactively in your terminal. ### ð¨ Build locally from Source For advanced
-users, you may build Endstone locally from the source. **Please note that
-building from source requires toolchains to be installed on your system.** | |
-Windows | Linux | |----------------------------------|-------------------------
-------|----------| | Build System | CMake | CMake | | Generator | Ninja | Ninja
-| | C/C++ Compiler **(Recommended)** | MSVC 193 (Visual Studio 2022) | Clang 15
-| | C/C++ Compiler (Minimum) | MSVC 191 (Visual Studio 2017) | Clang 5 | |
-Standard Library | MSVC STL | libc++ | Click to toggle the detailed
-instructions First, clone the repository: ```shell git clone https://
-github.com/EndstoneMC/endstone.git cd endstone ``` The Endstone project uses
-Conan as the package manager. The next step will involve the installation of
-conan and dependencies. ```shell pip install conan conan export third_party/
-funchook --version 1.1.3 conan install . --build=missing -s compiler.cppstd=17
--c tools.cmake.cmaketoolchain:generator=Ninja ``` Finally, you can build the
-wheel and install it on your local machine: ```shell pip install . endstone ```
-## ð Plugins [ð](#-table-of-contents) Currently, the Endstone project is
-under active development, and we invite you to review our roadmap. While you
-wait, why not take a sneaky peek of our example plugins which illustrate the
-friendliness of the plugin API. If you have previous experience with Bukkit,
-you should find the API particularly intuitive to work with: - [C++ Example
-Plugin](https://github.com/EndstoneMC/cpp-plugin-template) - [Python Example
-Plugin](https://github.com/EndstoneMC/python-plugin-template) | Milestone |
-Duration | Core | C++ API | Python API | Since | |-----------------------------
--------------|------------|------|---------|------------|--------| | **ð
-Plugin Loader** | 1-2 months | â | â | â | v0.1.0 | | **â¨ï¸ Command
-System** | 2-3 months | â | â | â | v0.2.0 | | **ð Permission System**
-| 2-3 months | â | â | â | v0.3.0 | | **ð Event System** | 2-3 months
-| ð§ | â | â | | | **ð  Minecraft Core Features** | 4-5 months | â³ |
-â³ | â³ | | | **ð¼ GUI & Inventory System** | 3-4 months | â³ | â³ | â³
-| | | **ð Advanced Features & Refinements** | 4-6 months | â³ | â³ | â³ |
-| | **ð§ª Beta Testing & Community Feedback** | 3 months | â³ | â³ | â³ | |
-| **ð Official Release & Support** | - | â³ | â³ | â³ | | Here's a legend
-to guide you: - â: Task is completed. Woohoo! ð - ð§: Task is under way.
-We're on it! ðª - â³: Task is up next. Exciting things are coming! ð  ##
-ð Contributing [ð](#-table-of-contents) We warmly welcome contributions
-to the Endstone project! If you're enthusiastic about enhancing Bedrock
-Dedicated Servers with Python and C++ and have ideas on how to improve
-Endstone, here are a few ways you can contribute: ### Reporting Bugs If you
-encounter any bugs while using Endstone, please open an [issue](https://
-github.com/EndstoneMC/endstone/issues) in our GitHub repository. Ensure to
-include a detailed description of the bug and steps to reproduce it. ###
-Submitting a Pull Request We appreciate code contributions. If you've fixed a
-bug or implemented a new feature, please submit a pull request! Please ensure
-your code follows our coding standards and include tests where possible. ##
-ð« License [ð](#-table-of-contents) The Endstone project is licensed under
-the [Apache-2.0 license](LICENSE).
+install endstone endstone ``` ### ð³ Docker To try Endstone from the latest
+Docker image, use the following command: ```shell docker pull endstone/endstone
+docker run --rm -it -p 19132:19132/udp endstone/endstone ``` This will pull the
+latest Endstone image and run it interactively in your terminal. ### ð
+Docker Compose You can also use Docker Compose to run Endstone in a production
+environment. ```shell docker compose build docker compose up -d docker attach
+endstone ``` ### ð¨ Build locally from Source For advanced users, you may
+build Endstone locally from the source. **Please note that building from source
+requires toolchains to be installed on your system.** | | Windows | Linux | |--
+--------------------------------|-------------------------------|----------| |
+Build System | CMake | CMake | | Generator | Ninja | Ninja | | C/C++ Compiler
+**(Recommended)** | MSVC 193 (Visual Studio 2022) | Clang 15 | | C/C++ Compiler
+(Minimum) | MSVC 191 (Visual Studio 2017) | Clang 5 | | Standard Library | MSVC
+STL | libc++ | Click to toggle the detailed instructions First, clone the
+repository: ```shell git clone https://github.com/EndstoneMC/endstone.git cd
+endstone ``` The Endstone project uses Conan as the package manager. The next
+step will involve the installation of conan and dependencies. ```shell pip
+install conan conan export third_party/funchook --version 1.1.3 conan install .
+--build=missing -s compiler.cppstd=17 -c tools.cmake.cmaketoolchain:
+generator=Ninja ``` Finally, you can build the wheel and install it on your
+local machine: ```shell pip install . endstone ``` ## ð Plugins [ð](#-
+table-of-contents) Currently, the Endstone project is under active development,
+and we invite you to review our roadmap. While you wait, why not take a sneaky
+peek of our example plugins which illustrate the friendliness of the plugin
+API. If you have previous experience with Bukkit, you should find the API
+particularly intuitive to work with: - [C++ Example Plugin](https://github.com/
+EndstoneMC/cpp-plugin-template) - [Python Example Plugin](https://github.com/
+EndstoneMC/python-plugin-template) | Milestone | Duration | Core | C++ API |
+Python API | Since | |------------------------------------------|------------|-
+-----|---------|------------|--------| | **ð Plugin Loader** | 1-2 months |
+â | â | â | v0.1.0 | | **â¨ï¸ Command System** | 2-3 months | â | â
+| â | v0.2.0 | | **ð Permission System** | 2-3 months | â | â | â |
+v0.3.0 | | **ð Event System** | 2-3 months | â | â | â | v0.4.0 | |
+**ð  Minecraft Core Features** | 4-5 months | â³ | â³ | â³ | | | **ð¼
+GUI & Inventory System** | 3-4 months | â³ | â³ | â³ | | | **ð Advanced
+Features & Refinements** | 4-6 months | â³ | â³ | â³ | | | **ð§ª Beta
+Testing & Community Feedback** | 3 months | â³ | â³ | â³ | | | **ð
+Official Release & Support** | - | â³ | â³ | â³ | | Here's a legend to guide
+you: - â: Task is completed. Woohoo! ð - ð§: Task is under way. We're on
+it! ðª - â³: Task is up next. Exciting things are coming! ð  ## ð
+Contributing [ð](#-table-of-contents) We warmly welcome contributions to the
+Endstone project! If you're enthusiastic about enhancing Bedrock Dedicated
+Servers with Python and C++ and have ideas on how to improve Endstone, here are
+a few ways you can contribute: ### Reporting Bugs If you encounter any bugs
+while using Endstone, please open an [issue](https://github.com/EndstoneMC/
+endstone/issues) in our GitHub repository. Ensure to include a detailed
+description of the bug and steps to reproduce it. ### Submitting a Pull Request
+We appreciate code contributions. If you've fixed a bug or implemented a new
+feature, please submit a pull request! Please ensure your code follows our
+coding standards and include tests where possible. ## ð« License [ð](#-
+table-of-contents) The Endstone project is licensed under the [Apache-2.0
+license](LICENSE).
```

### Comparing `endstone-0.4.0/conanfile.py` & `endstone-0.4.1/conanfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,23 +29,14 @@
         "capstone/*:ppc": False,
         "capstone/*:sparc": False,
         "capstone/*:sysz": False,
         "capstone/*:xcore": False,
         "capstone/*:tms320c64x": False,
         "capstone/*:m680x": False,
         "capstone/*:evm": False,
-        "lief/*:with_frozen": False,
-        "lief/*:with_json": False,
-        "lief/*:with_c_api": False,
-        "lief/*:with_art": False,
-        "lief/*:with_dex": False,
-        "lief/*:with_macho": False,
-        "lief/*:with_oat": False,
-        "lief/*:with_pe": False,
-        "lief/*:with_vdex": False,
     }
 
     exports_sources = "CMakeLists.txt", "src/*", "include/*", "tests/*"
 
     def set_version(self):
         if self.version:
             return
@@ -115,14 +106,15 @@
         self.requires("spdlog/1.12.0")
         self.requires("fmt/[>=10.1.1]", transitive_headers=True, transitive_libs=True)
         self.requires("pybind11/2.11.1")
         self.requires("funchook/1.1.3")
         self.requires("magic_enum/0.9.5")
         self.requires("entt/3.13.0")
         self.requires("cpptrace/0.5.2")
+        self.requires("ms-gsl/4.0.0")
         if self.settings.os == "Linux":
             self.requires("libelf/0.8.13")
 
         self.test_requires("gtest/1.14.0")
 
     def config_options(self):
         if self.settings.os == "Windows":
@@ -152,29 +144,32 @@
         cmake = CMake(self)
         cmake.install()
 
     def package_info(self):
         self.cpp_info.components["headers"].libs = []
         self.cpp_info.components["headers"].libdirs = []
         self.cpp_info.components["headers"].set_property("cmake_target_name", "endstone::headers")
-        self.cpp_info.components["headers"].requires = ["fmt::fmt", "entt::entt"]
+        self.cpp_info.components["headers"].requires = ["fmt::fmt"]
 
         self.cpp_info.components["core"].libs = ["endstone_core"]
         self.cpp_info.components["core"].set_property("cmake_target_name", "endstone::core")
-        self.cpp_info.components["core"].requires = ["spdlog::spdlog"]
-        self.cpp_info.components["core"].defines = ["PYBIND11_USE_SMART_HOLDER_AS_DEFAULT"]
+        self.cpp_info.components["core"].requires = [
+            "spdlog::spdlog",
+            "magic_enum::magic_enum",
+            "entt::entt",
+            "ms-gsl::ms-gsl",
+        ]
         if self.settings.os == "Linux":
             self.cpp_info.components["core"].system_libs.extend(["dl", "stdc++fs"])
 
         self.cpp_info.components["runtime"].libs = ["endstone_runtime"]
         self.cpp_info.components["runtime"].set_property("cmake_target_name", "endstone::runtime")
         self.cpp_info.components["runtime"].requires = [
             "core",
             "funchook::funchook",
-            "magic_enum::magic_enum",
             "pybind11::pybind11",
             "cpptrace::cpptrace",
         ]
         if self.settings.os == "Linux":
             self.cpp_info.components["runtime"].requires.extend(["libelf::libelf"])
         if self.settings.os == "Windows":
             self.cpp_info.components["runtime"].system_libs.extend(["dbghelp"])
```

### Comparing `endstone-0.4.0/include/bedrock/automatic_id.h` & `endstone-0.4.1/include/bedrock/automatic_id.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/bedrock.h` & `endstone-0.4.1/include/bedrock/bedrock.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/bedrock_log.h` & `endstone-0.4.1/include/bedrock/bedrock_log.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command.h` & `endstone-0.4.1/include/bedrock/command/command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_context.h` & `endstone-0.4.1/include/bedrock/command/command_context.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_flag.h` & `endstone-0.4.1/include/bedrock/command/command_flag.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_origin.h` & `endstone-0.4.1/include/bedrock/command/command_origin.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_output.h` & `endstone-0.4.1/include/bedrock/command/command_output.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_permission_level.h` & `endstone-0.4.1/include/bedrock/command/command_permission_level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_registry.h` & `endstone-0.4.1/include/bedrock/command/command_registry.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_utils.h` & `endstone-0.4.1/include/bedrock/command/command_utils.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/command_version.h` & `endstone-0.4.1/include/bedrock/command/command_version.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/command/minecraft_commands.h` & `endstone-0.4.1/include/bedrock/command/minecraft_commands.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/common.h` & `endstone-0.4.1/include/bedrock/common.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/core.h` & `endstone-0.4.1/include/bedrock/core.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/details.h` & `endstone-0.4.1/include/bedrock/details.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/forward.h` & `endstone-0.4.1/include/bedrock/forward.h`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 class FeatureRegistry;
 class FeatureTypeFactory;
 class FrameUpdateContextBase;
 class GameRules;
 class HandSlot;
 class HashedString;
 class HitResult;
+class I18nObserver;
 class IAddActorEntityProxy;
 class IConstBlockSource;
 class IContainerManager;
 class IMinecraftEventing;
 class INpcDialogueData;
 class IUnknownBlockTypeRegistry;
 class InputMode;
@@ -100,23 +101,26 @@
 class JigsawStructureRegistry;
 class LayeredAbilities;
 class LevelChunk;
 class LevelData;
 class LevelSettings;
 class LevelSoundManager;
 class LevelStorage;
+class Localization;
 class LootTables;
 class MapItemSavedData;
 class MaterialTypeHelper;
 class MobEffectInstance;
 class MolangVariableMap;
 class NavigationComponent;
 class NetEventCallback;
 class NewInteractionModel;
 class Options;
+class PackAccessStrategy;
+class PackManifest;
 class Particle;
 class Path;
 class PauseManager;
 class PhotoStorage;
 class PlayerListEntry;
 class PlayerMovementSettings;
 class PortalForcer;
@@ -126,14 +130,16 @@
 class PropertiesSettings;
 class ProjectileFactory;
 class Random;
 class Recipes;
 class RenderParams;
 class ResolvedItemIconInfo;
 class ResolvedTextObject;
+class ResourceLoadManager;
+class ResourcePackManager;
 class SavedDataStorage;
 class Scheduler;
 class Scoreboard;
 class ScreenSetupCleanupHelper;
 class ScreenshotOptions;
 class SearchQuery;
 class SerializedSkin;
@@ -203,7 +209,9 @@
 class StackRefResult;
 template <typename A, typename B, typename C>
 class Factory;
 template <typename A, typename B>
 class TagRegistry;
 template <typename T>
 class IDType;
+template <typename T>
+using optional_ref = T *; // NOLINT(*-identifier-naming)
```

### Comparing `endstone-0.4.0/include/bedrock/i18n.h` & `endstone-0.4.1/include/bedrock/server/command/say_command.h`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
 #include <string>
-#include <vector>
 
 #include "bedrock/bedrock.h"
 
-class I18n {
-public:
-    BEDROCK_API static std::string get(const std::string &message_id, const std::vector<std::string> &params,
-                                       const class Localization *localization);
+class SayCommand {
+private:
+    BEDROCK_API static void _sendMessage(std::string const &, std::string const &,  // NOLINT(*-identifier-naming)
+                                         struct CommandOriginIdentity const &, class Level &);
 };
```

### Comparing `endstone-0.4.0/include/bedrock/mce.h` & `endstone-0.4.1/include/bedrock/network/network_identifier.h`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,11 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include <array>
-#include <cstdint>
-
-namespace mce {
-class UUID {
+class NetworkIdentifier {
 public:
-    std::int64_t msb;  // most significant bits
-    std::int64_t lsb;  // least significant bits
+    char pad[160];  // TODO(fixme): find out the class structure
 };
-
-class Color {
-public:
-    float r;
-    float g;
-    float b;
-    float a;
-};
-
-}  // namespace mce
```

### Comparing `endstone-0.4.0/include/bedrock/memory.h` & `endstone-0.4.1/include/bedrock/memory.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/minecraft.h` & `endstone-0.4.1/include/bedrock/minecraft.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/network_identifier.h` & `endstone-0.4.1/include/bedrock/world/actor/components/actor_unique_id_component.h`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-class NetworkIdentifier {
-public:
-    char pad[160];  // TODO(fixme): find out the class structure
+#include "bedrock/world/actor/actor.h"
+
+struct ActorUniqueIDComponent {
+    ActorUniqueID id;
 };
```

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/certificate.h` & `endstone-0.4.1/include/bedrock/network/protocol/certificate.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/game/available_commands_packet.h` & `endstone-0.4.1/include/bedrock/network/protocol/game/available_commands_packet.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/game/text_packet.h` & `endstone-0.4.1/include/bedrock/network/protocol/game/text_packet.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/minecraft_packets.h` & `endstone-0.4.1/include/bedrock/network/protocol/minecraft_packets.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/packet.h` & `endstone-0.4.1/include/bedrock/network/protocol/packet.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/packet_sender.h` & `endstone-0.4.1/include/bedrock/network/protocol/packet_sender.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/protocol/sub_client_id.h` & `endstone-0.4.1/include/bedrock/network/protocol/sub_client_id.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/raknet/socket2.h` & `endstone-0.4.1/include/bedrock/network/raknet/socket2.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/network/raknet/types.h` & `endstone-0.4.1/include/bedrock/network/raknet/types.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/server/level/server_level.h` & `endstone-0.4.1/include/bedrock/server/level/server_level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/server/level/server_player.h` & `endstone-0.4.1/include/bedrock/server/level/server_player.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/server/network/server_network_handler.h` & `endstone-0.4.1/include/bedrock/server/network/server_network_handler.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/server/server_instance.h` & `endstone-0.4.1/include/bedrock/server/server_instance.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/threading.h` & `endstone-0.4.1/include/bedrock/threading.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/type_id.h` & `endstone-0.4.1/include/bedrock/type_id.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/actor.h` & `endstone-0.4.1/include/bedrock/world/actor/actor.h`

 * *Files 4% similar despite different names*

```diff
@@ -58,22 +58,20 @@
 #ifdef __linux__
     virtual bool hasComponent(HashedString const &) = 0;
 #endif
     virtual ~Actor() = 0;
     virtual void resetUserPos(bool) = 0;
     virtual ActorType getOwnerEntityType() = 0;
     BEDROCK_API virtual void remove();
-    virtual bool isRuntimePredictedMovementEnabled() = 0;
     [[nodiscard]] virtual Vec3 getFiringPos() const = 0;
     [[nodiscard]] virtual float getInterpolatedBodyRot(float) const = 0;
     [[nodiscard]] virtual float getInterpolatedHeadRot(float) const = 0;
     [[nodiscard]] virtual float getInterpolatedBodyYaw(float) const = 0;
     [[nodiscard]] virtual float getYawSpeedInDegreesPerSecond() const = 0;
     [[nodiscard]] virtual Vec3 getInterpolatedRidingOffset(float, int) const = 0;
-    virtual void resetInterpolated() = 0;
     [[nodiscard]] virtual bool isFireImmune() const = 0;
     virtual void blockedByShield(ActorDamageSource const &, Actor &) = 0;
     virtual bool canDisableShield() = 0;
     virtual void teleportTo(Vec3 const &, bool, int, int, bool) = 0;
     virtual Vec3 lerpMotion(Vec3 const &) = 0;
     virtual std::unique_ptr<AddActorBasePacket> tryCreateAddActorPacket() = 0;
     virtual void normalTick() = 0;
@@ -101,16 +99,14 @@
     virtual void setSneaking(bool) = 0;
     [[nodiscard]] virtual bool isBlocking() const = 0;
     [[nodiscard]] virtual bool isDamageBlocked(ActorDamageSource const &) const = 0;
     [[nodiscard]] virtual bool isAlive() const = 0;
     [[nodiscard]] virtual bool isOnFire() const = 0;
     [[nodiscard]] virtual bool isSurfaceMob() const = 0;
     [[nodiscard]] virtual bool isTargetable() const = 0;
-    [[nodiscard]] virtual bool isLocalPlayer() const = 0;
-    [[nodiscard]] virtual bool isPlayer() const = 0;
     virtual bool canAttack(Actor *, bool) const = 0;
     virtual void setTarget(Actor *) = 0;
     virtual bool isValidTarget(Actor *) const = 0;
     virtual bool attack(Actor &, ActorDamageCause const &) = 0;
     virtual void performRangedAttack(Actor &, float) = 0;
     virtual void setOwner(ActorUniqueID) = 0;
     virtual void setSitting(bool) = 0;
@@ -214,27 +210,34 @@
 
 protected:
     virtual void _playStepSound(BlockPos const &, Block const &) = 0;
     virtual void _doAutoAttackOnTouch(Actor &) = 0;
 
 public:
     template <typename Component>
+    [[nodiscard]] bool hasComponent() const
+    {
+        return context_.hasComponent<Component>();
+    }
+
+    template <typename Component>
     Component *tryGetComponent()
     {
         return context_.tryGetComponent<Component>();
     }
 
     template <typename Component>
     Component *tryGetComponent() const
     {
         return context_.tryGetComponent<Component>();
     }
 
     BEDROCK_API void setDimension(WeakRef<Dimension>);
 
+    [[nodiscard]] bool isPlayer() const;
     [[nodiscard]] bool isRemoved() const;
     [[nodiscard]] Dimension &getDimension() const;
     [[nodiscard]] Level &getLevel() const;
     [[nodiscard]] Vec3 const &getPosition() const;
     [[nodiscard]] ActorRuntimeID getRuntimeID() const;
 
     static Actor *tryGetFromEntity(EntityContext const &, bool include_removed);
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/actor_initialization_method.h` & `endstone-0.4.1/include/bedrock/world/actor/actor_initialization_method.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/actor_runtime_id.h` & `endstone-0.4.1/include/bedrock/world/actor/actor_runtime_id.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/actor_unique_id.h` & `endstone-0.4.1/include/bedrock/world/actor/actor_unique_id.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/components/abilities_component.h` & `endstone-0.4.1/include/bedrock/world/actor/components/abilities_component.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/components/actor_owner_component.h` & `endstone-0.4.1/include/bedrock/world/actor/components/actor_owner_component.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/components/actor_unique_id_component.h` & `endstone-0.4.1/include/bedrock/world/actor/components/runtime_id_component.h`

 * *Files 4% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
 #include "bedrock/world/actor/actor.h"
 
-struct ActorUniqueIDComponent {
-    ActorUniqueID id;
+struct RuntimeIDComponent {
+    ActorRuntimeID id;
 };
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/components/runtime_id_component.h` & `endstone-0.4.1/src/endstone_python/util.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#pragma once
+#include <pybind11/pybind11.h>
 
-#include "bedrock/world/actor/actor.h"
+namespace py = pybind11;
 
-struct RuntimeIDComponent {
-    ActorRuntimeID id;
-};
+namespace endstone::detail {
+
+void init_util(py::module &m) {}
+
+}  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/components/user_entity_identifier_component.h` & `endstone-0.4.1/src/endstone_runtime/bedrock/minecraft.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#pragma once
+#include "bedrock/minecraft.h"
 
-#include "bedrock/mce.h"
-#include "bedrock/network/network_identifier.h"
-#include "bedrock/network/protocol/certificate.h"
-#include "bedrock/network/protocol/sub_client_id.h"
+#include "endstone/endstone.h"
 
-class UserEntityIdentifierComponent {
-public:
-    NetworkIdentifier network_id;              // +0
-    SubClientId sub_client_id;                 // +160
-    mce::UUID uuid;                            // +168
-    std::string pfid;                          // +184
-    std::unique_ptr<Certificate> certificate;  // +216
-};
+MinecraftCommands &Minecraft::getCommands()
+{
+    return **reinterpret_cast<MinecraftCommands **>(reinterpret_cast<std::size_t *>(this) + _WIN32_LINUX_(23, 22));
+}
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/mob/mob.h` & `endstone-0.4.1/include/bedrock/world/actor/mob/mob.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 class Mob : public Actor {
 public:
     ~Mob() override = 0;
     virtual void knockback(Actor *, int, float, float, float, float, float) = 0;
     virtual void spawnAnim() = 0;
     virtual void setSprinting(bool) = 0;
-    virtual Puv::Legacy::LevelSoundEvent getHurtSound() = 0;
     virtual Puv::Legacy::LevelSoundEvent getDeathSound() = 0;
     [[nodiscard]] virtual float getSpeed() const = 0;
     virtual void setSpeed(float) = 0;
     virtual void hurtEffects(ActorDamageSource const &, float, bool, bool) = 0;
     virtual void aiStep() = 0;
     virtual void pushActors() = 0;
     virtual bool checkSpawnRules(bool) = 0;
@@ -42,16 +41,16 @@
     virtual int getArmorValue() = 0;
     virtual void hurtArmorSlots(ActorDamageSource const &, int, std::bitset<4>) = 0;
     virtual void setDamagedArmor(ArmorSlot, ItemStack const &) = 0;
     virtual void sendArmorDamage(std::bitset<4>) = 0;
     virtual void sendArmor(std::bitset<4>) = 0;
     [[nodiscard]] virtual std::vector<ItemStack const *> getAllHand() const = 0;
     [[nodiscard]] virtual std::vector<ItemStack const *> getAllEquipment() const = 0;
-    virtual void dropEquipmentOnDeath() = 0;
     virtual void dropEquipmentOnDeath(ActorDamageSource const &, int) = 0;
+    virtual void dropEquipmentOnDeath() = 0;
     virtual void clearVanishEnchantedItemsOnDeath() = 0;
     virtual void sendInventory(bool) = 0;
     [[nodiscard]] virtual float getDamageAfterEnchantReduction(ActorDamageSource const &, float) const = 0;
     virtual bool createAIGoals() = 0;
     virtual void onBorn(Actor &, Actor &) = 0;
     virtual bool setItemSlot(EquipmentSlot, ItemStack const &) = 0;
     virtual void setTransitioningSitting(bool) = 0;
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/player/permissions_handler.h` & `endstone-0.4.1/include/bedrock/world/actor/player/permissions_handler.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/player/player.h` & `endstone-0.4.1/include/bedrock/world/actor/player/player.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/player/player_permission_level.h` & `endstone-0.4.1/include/bedrock/world/actor/player/player_permission_level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/actor/registry/entity_context.h` & `endstone-0.4.1/include/bedrock/world/actor/registry/entity_context.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 class EntityContext {
 public:
     EntityContext(EntityRegistry &registry, EntityId entity_id)
         : registry_(registry), entt_registry_(registry.registry_), entity_id_(entity_id){};
 
     template <typename Component>
+    [[nodiscard]] bool hasComponent() const
+    {
+        return entt_registry_.all_of<Component>(entity_id_);
+    }
+
+    template <typename Component>
     Component *tryGetComponent()
     {
         return entt_registry_.try_get<Component>(entity_id_);
     }
 
     template <typename Component>
     Component *tryGetComponent() const
```

### Comparing `endstone-0.4.0/include/bedrock/world/actor/registry/entity_registry.h` & `endstone-0.4.1/include/bedrock/world/actor/registry/entity_registry.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/dimension/dimension.h` & `endstone-0.4.1/include/bedrock/world/level/dimension/dimension.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/dimension/dimension_height_range.h` & `endstone-0.4.1/include/bedrock/world/level/dimension/dimension_height_range.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/dimension/dimension_interface.h` & `endstone-0.4.1/include/bedrock/world/level/dimension/dimension_interface.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/dimension/vanilla_dimensions.h` & `endstone-0.4.1/include/bedrock/world/level/dimension/vanilla_dimensions.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/actor_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/actor_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/block_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/block_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/coordinator_result.h` & `endstone-0.4.1/include/bedrock/world/level/event/coordinator_result.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/event_coordinator.h` & `endstone-0.4.1/include/bedrock/world/level/event/event_coordinator.h`

 * *Files 20% similar despite different names*

```diff
@@ -25,35 +25,35 @@
 #include "bedrock/world/level/event/item_event.h"
 #include "bedrock/world/level/event/level_event.h"
 #include "bedrock/world/level/event/player_event.h"
 #include "bedrock/world/level/event/server_event.h"
 
 class ActorEventCoordinator {
 public:
-    BEDROCK_API void sendEvent(EventRef<ActorGameplayEvent<void>> const &ref);
-    BEDROCK_API CoordinatorResult sendEvent(EventRef<ActorGameplayEvent<CoordinatorResult>> const &ref);
+    void sendEvent(EventRef<ActorGameplayEvent<void>> const &ref);
+    CoordinatorResult sendEvent(EventRef<ActorGameplayEvent<CoordinatorResult>> const &ref);
 };
 
 class BlockEventCoordinator {
 public:
-    BEDROCK_API void sendEvent(EventRef<BlockGameplayEvent<void>> const &ref);
-    BEDROCK_API CoordinatorResult sendEvent(EventRef<BlockGameplayEvent<CoordinatorResult>> const &ref);
+    void sendEvent(EventRef<BlockGameplayEvent<void>> const &ref);
+    CoordinatorResult sendEvent(EventRef<BlockGameplayEvent<CoordinatorResult>> const &ref);
 };
 class ItemEventCoordinator;
 
 class LevelEventCoordinator {
 public:
-    BEDROCK_API void sendEvent(EventRef<LevelGameplayEvent<void>> const &ref);
+    void sendEvent(EventRef<LevelGameplayEvent<void>> const &ref);
     LevelGameplayHandler &getLevelGameplayHandler();
 };
 
 class PlayerEventCoordinator {
 public:
-    BEDROCK_API void sendEvent(EventRef<PlayerGameplayEvent<void>> const &ref);
-    BEDROCK_API CoordinatorResult sendEvent(EventRef<PlayerGameplayEvent<CoordinatorResult>> const &ref);
+    void sendEvent(EventRef<PlayerGameplayEvent<void>> const &ref);
+    CoordinatorResult sendEvent(EventRef<PlayerGameplayEvent<CoordinatorResult>> const &ref);
 };
 class ServerPlayerEventCoordinator : public PlayerEventCoordinator {};
 class ClientPlayerEventCoordinator : public PlayerEventCoordinator {};
 
 class ServerInstanceEventCoordinator {
 public:
     BEDROCK_API void sendServerInitializeStart(ServerInstance &instance);
```

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/event_ref.h` & `endstone-0.4.1/include/bedrock/world/level/event/event_ref.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/event_result.h` & `endstone-0.4.1/include/bedrock/world/level/event/event_result.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/gameplay_handler.h` & `endstone-0.4.1/include/bedrock/world/level/event/gameplay_handler.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/item_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/item_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/level_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/level_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/player_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/player_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/event/server_event.h` & `endstone-0.4.1/include/bedrock/world/level/event/server_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/level.h` & `endstone-0.4.1/include/bedrock/world/level/level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/level_interface.h` & `endstone-0.4.1/include/bedrock/world/level/level_interface.h`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,18 @@
     virtual OwnerPtr<EntityContext> removeActorAndTakeEntity(WeakEntityRef) = 0;
     virtual OwnerPtr<EntityContext> removeActorFromWorldAndTakeEntity(WeakEntityRef) = 0;
     virtual OwnerPtr<EntityContext> takeEntity(WeakEntityRef, LevelChunk &) = 0;
     [[nodiscard]] virtual StrictEntityContext fetchStrictEntity(ActorUniqueID, bool) const = 0;
     [[nodiscard]] virtual Actor *fetchEntity(ActorUniqueID, bool) const = 0;
     [[nodiscard]] virtual Actor *getRuntimeEntity(ActorRuntimeID, bool) const = 0;
     [[nodiscard]] virtual Mob *getMob(ActorUniqueID) const = 0;
-    [[nodiscard]] virtual Player *getPlayer(ActorUniqueID) const = 0;
-    [[nodiscard]] virtual Player *getPlayer(mce::UUID const &) const = 0;
     [[nodiscard]] virtual Player *getPlayer(std::string const &) const = 0;
+    [[nodiscard]] virtual Player *getPlayer(mce::UUID const &) const = 0;
     [[nodiscard]] virtual Player *getPlayerByXuid(std::string const &) const = 0;
+    [[nodiscard]] virtual Player *getPlayer(ActorUniqueID) const = 0;
     [[nodiscard]] virtual Player *getPlatformPlayer(std::string const &) const = 0;
     [[nodiscard]] virtual Player *getPlayerFromServerId(std::string const &) const = 0;
     [[nodiscard]] virtual Player *getRuntimePlayer(ActorRuntimeID) const = 0;
     virtual int getNumRemotePlayers() = 0;
     [[nodiscard]] virtual Player *getPrimaryLocalPlayer() const = 0;
     virtual IMinecraftEventing &getEventing() = 0;
     [[nodiscard]] virtual mce::Color getPlayerColor(Player const &) const = 0;
@@ -129,38 +129,32 @@
     [[nodiscard]] virtual BiomeManager const &getBiomeManager() const = 0;
     virtual BiomeManager &getBiomeManager() = 0;
     [[nodiscard]] virtual OwnerPtrFactory<Dimension, ILevel &, Scheduler &> const &getDimensionFactory() const = 0;
     virtual OwnerPtrFactory<Dimension, ILevel &, Scheduler &> &getDimensionFactory() = 0;
     [[nodiscard]] virtual Factory<BaseLightTextureImageBuilder, Level &, Scheduler &> const &
     getLightTextureImageBuilderFactory() const = 0;
     virtual Factory<BaseLightTextureImageBuilder, Level &, Scheduler &> &getLightTextureImageBuilderFactory() = 0;
-
     [[nodiscard]] virtual void *getWorldRegistriesProvider() const = 0;
     virtual void *getWorldRegistriesProvider() = 0;
     virtual void addListener(LevelListener &) = 0;
     virtual void removeListener(LevelListener &) = 0;
     virtual void tickEntities() = 0;
     virtual void tickEntitySystems() = 0;
     virtual StackRefResult<PauseManager> getPauseManager() = 0;
     [[nodiscard]] virtual StackRefResult<PauseManager const> getPauseManager() const = 0;
     virtual void onPlayerDeath(Player &, ActorDamageSource const &) = 0;
     virtual void tick() = 0;
-
-private:
-    virtual void directTickEntities(BlockSource &) = 0;
-
-public:
-    virtual bool explode(Explosion &) = 0;
     virtual bool explode(BlockSource &, Actor *, Vec3 const &, float, bool, bool, float, bool) = 0;
+    virtual bool explode(Explosion &) = 0;
     virtual void spawnParticleEffect(std::string const &, Vec3 const &, Dimension *) = 0;
     virtual void denyEffect(BlockSource &, Vec3 const &) = 0;
     virtual void potionSplash(Vec3 const &, mce::Color const &, bool) = 0;
     virtual bool extinguishFire(BlockSource &, BlockPos const &, std::uint8_t, Actor *) = 0;
-    virtual std::unique_ptr<Path> findPath(Actor &, Actor &, NavigationComponent &) = 0;
     virtual std::unique_ptr<Path> findPath(Actor &, int, int, int, NavigationComponent &) = 0;
+    virtual std::unique_ptr<Path> findPath(Actor &, Actor &, NavigationComponent &) = 0;
     virtual void updateSleepingPlayerList() = 0;
     virtual void setSleepStatus(PlayerSleepStatus const &) = 0;
     [[nodiscard]] virtual PlayerSleepStatus getSleepStatus() const = 0;
     [[nodiscard]] virtual int getTime() const = 0;
     virtual void setTime(int) = 0;
     virtual std::uint32_t getSeed() = 0;
     [[nodiscard]] virtual BlockPos const &getSharedSpawnPos() const = 0;
@@ -205,68 +199,58 @@
     virtual void save() = 0;
     virtual void saveLevelData() = 0;
     virtual void saveGameData() = 0;
     virtual std::shared_ptr<void *> requestTimedStorageDeferment() = 0;
     virtual TickingAreasManager &getTickingAreasMgr() = 0;
     virtual void addTickingAreaList(AutomaticID<Dimension, int>, std::shared_ptr<TickingAreaList> const &) = 0;
     virtual void sendServerLegacyParticle(ParticleType, Vec3 const &, Vec3 const &, int) = 0;
-    virtual void playSound(AutomaticID<Dimension, int>, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
-                           ActorDefinitionIdentifier const &, bool, bool) = 0;
-    virtual void playSound(IConstBlockSource const &, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
-                           ActorDefinitionIdentifier const &, bool, bool) = 0;
-    virtual void playSound(std::string const &, Vec3 const &, float, float) = 0;
-    virtual void playSound(Puv::Legacy::LevelSoundEvent, Vec3 const &, float, float) = 0;
     virtual void playSound(Puv::Legacy::LevelSoundEvent, Vec3 const &, int, ActorDefinitionIdentifier const &, bool,
                            bool) = 0;
-    virtual void registerEventCoordinators() = 0;
-    virtual void setRemotePlayerEventCoordinator(std::unique_ptr<PlayerEventCoordinator> &&) = 0;
+    virtual void playSound(Puv::Legacy::LevelSoundEvent, Vec3 const &, float, float) = 0;
+    virtual void playSound(std::string const &, Vec3 const &, float, float) = 0;
+    virtual void playSound(IConstBlockSource const &, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
+                           ActorDefinitionIdentifier const &, bool, bool) = 0;
+    virtual void playSound(AutomaticID<Dimension, int>, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
+                           ActorDefinitionIdentifier const &, bool, bool) = 0;
     virtual PlayerEventCoordinator &getRemotePlayerEventCoordinator() = 0;
-    virtual void setServerPlayerEventCoordinator(std::unique_ptr<ServerPlayerEventCoordinator> &&) = 0;
     virtual ServerPlayerEventCoordinator &getServerPlayerEventCoordinator() = 0;
-    virtual void setClientPlayerEventCoordinator(std::unique_ptr<ClientPlayerEventCoordinator> &&) = 0;
     virtual ClientPlayerEventCoordinator &getClientPlayerEventCoordinator() = 0;
-    virtual void setActorEventCoordinator(std::unique_ptr<ActorEventCoordinator> &&) = 0;
     virtual ActorEventCoordinator &getActorEventCoordinator() = 0;
-    virtual void setBlockEventCoordinator(std::unique_ptr<BlockEventCoordinator> &&) = 0;
     virtual BlockEventCoordinator &getBlockEventCoordinator() = 0;
-    virtual void setItemEventCoordinator(std::unique_ptr<ItemEventCoordinator> &&) = 0;
     virtual ItemEventCoordinator &getItemEventCoordinator() = 0;
-    virtual void setServerNetworkEventCoordinator(std::unique_ptr<ServerNetworkEventCoordinator> &&) = 0;
     virtual ServerNetworkEventCoordinator &getServerNetworkEventCoordinator() = 0;
-    virtual void setScriptingEventCoordinator(std::unique_ptr<ScriptingEventCoordinator> &&) = 0;
     virtual ScriptingEventCoordinator &getScriptingEventCoordinator() = 0;
-    virtual void setScriptDeferredEventCoordinator(std::unique_ptr<ScriptDeferredEventCoordinator> &&) = 0;
     virtual ScriptDeferredEventCoordinator &getScriptDeferredEventCoordinator() = 0;
     virtual LevelEventCoordinator &getLevelEventCoordinator() = 0;
-    virtual void handleLevelEvent(LevelEvent, CompoundTag const &) = 0;
     virtual void handleLevelEvent(LevelEvent, Vec3 const &, int) = 0;
+    virtual void handleLevelEvent(LevelEvent, CompoundTag const &) = 0;
     virtual void handleStopSoundEvent(std::string const &) = 0;
     virtual void handleStopAllSounds() = 0;
-    virtual void broadcastLevelEvent(LevelEvent, CompoundTag const &, UserEntityIdentifierComponent const *) = 0;
     virtual void broadcastLevelEvent(LevelEvent, Vec3 const &, int, UserEntityIdentifierComponent const *) = 0;
-    virtual void broadcastLocalEvent(BlockSource &, LevelEvent, Vec3 const &, Block const &) = 0;
+    virtual void broadcastLevelEvent(LevelEvent, CompoundTag const &, UserEntityIdentifierComponent const *) = 0;
     virtual void broadcastLocalEvent(BlockSource &, LevelEvent, Vec3 const &, int) = 0;
-    virtual void broadcastSoundEvent(Dimension &, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
+    virtual void broadcastLocalEvent(BlockSource &, LevelEvent, Vec3 const &, Block const &) = 0;
+    virtual void broadcastSoundEvent(BlockSource &, Puv::Legacy::LevelSoundEvent, Vec3 const &, Block const &,
                                      ActorDefinitionIdentifier const &, bool, bool) = 0;
     virtual void broadcastSoundEvent(BlockSource &, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
                                      ActorDefinitionIdentifier const &, bool, bool) = 0;
-    virtual void broadcastSoundEvent(BlockSource &, Puv::Legacy::LevelSoundEvent, Vec3 const &, Block const &,
+    virtual void broadcastSoundEvent(Dimension &, Puv::Legacy::LevelSoundEvent, Vec3 const &, int,
                                      ActorDefinitionIdentifier const &, bool, bool) = 0;
     virtual void broadcastActorEvent(Actor &, ActorEvent, int) const = 0;
     virtual void addChunkViewTracker(std::weak_ptr<ChunkViewSource>) = 0;
     virtual void onChunkReload(Bounds const &) = 0;
     virtual void onChunkReloaded(ChunkSource &, LevelChunk &) = 0;
     [[nodiscard]] virtual int getActivePlayerCount() const = 0;
     [[nodiscard]] virtual int getActiveUsersCount() const = 0;
-    virtual void forEachPlayer(std::function<bool(Player const &)>) const = 0;
     virtual void forEachPlayer(std::function<bool(Player &)>) = 0;
-    virtual void forEachUser(std::function<bool(EntityContext const &)>) const = 0;
+    virtual void forEachPlayer(std::function<bool(Player const &)>) const = 0;
     virtual void forEachUser(std::function<bool(EntityContext &)>) = 0;
-    virtual Player *findPlayer(std::function<bool(WeakEntityRef const &)>) const = 0;
+    virtual void forEachUser(std::function<bool(EntityContext const &)>) const = 0;
     virtual Player *findPlayer(std::function<bool(Player const &)>) const = 0;
+    virtual Player *findPlayer(std::function<bool(WeakEntityRef const &)>) const = 0;
     [[nodiscard]] virtual int getUserCount() const = 0;
     [[nodiscard]] virtual int countUsersWithMatchingNetworkId(NetworkIdentifier const &) const = 0;
     [[nodiscard]] virtual std::vector<OwnerPtr<EntityContext>> const &getUsers() const = 0;
     [[nodiscard]] virtual std::vector<OwnerPtr<EntityContext>> const &getEntities() const = 0;
 
 private:
     virtual void onSubChunkLoaded(ChunkSource &, LevelChunk &, std::int16_t, bool) = 0;
@@ -276,16 +260,16 @@
     virtual void onChunkDiscarded(LevelChunk &) = 0;
 
 private:
     virtual void *getLevelChunkMetaDataManager() = 0;
 
 public:
     virtual void queueEntityDestruction(OwnerPtr<EntityContext>) = 0;
-    virtual OwnerPtr<EntityContext> removeEntity(WeakEntityRef) = 0;
     virtual OwnerPtr<EntityContext> removeEntity(Actor &) = 0;
+    virtual OwnerPtr<EntityContext> removeEntity(WeakEntityRef) = 0;
     virtual void forceRemoveEntity(Actor &) = 0;
     virtual void forceRemoveEntityfromWorld(Actor &) = 0;
     virtual void forceFlushRemovedPlayers() = 0;
 
 private:
     virtual void loadFunctionManager() = 0;
 
@@ -302,20 +286,22 @@
     virtual void addTerrainParticleEffect(BlockPos const &, Block const &, Vec3 const &, float, float, float) = 0;
     virtual void addTerrainSlideEffect(BlockPos const &, Block const &, Vec3 const &, float, float, float) = 0;
     virtual void addBreakingItemParticleEffect(Vec3 const &, ParticleType, ResolvedItemIconInfo const &) = 0;
     virtual ActorUniqueID getNewUniqueID() = 0;
     virtual ActorRuntimeID getNextRuntimeID() = 0;
     [[nodiscard]] virtual std::vector<ChunkPos> const &getTickingOffsets() const = 0;
     [[nodiscard]] virtual std::vector<ChunkPos> const &getClientTickingOffsets() const = 0;
+    [[nodiscard]] virtual std::vector<ChunkPos> getSortedPositionsFromClientOffsets(
+        std::vector<ChunkPos> const &) const = 0;
     [[nodiscard]] virtual bool isExporting() const = 0;
     virtual void setIsExporting(bool) = 0;
     virtual SavedDataStorage &getSavedData() = 0;
+    virtual MapItemSavedData *getMapSavedData(ActorUniqueID) = 0;
     virtual MapItemSavedData *getMapSavedData(CompoundTag const &) = 0;
     virtual MapItemSavedData *getMapSavedData(CompoundTag const *) = 0;
-    virtual MapItemSavedData *getMapSavedData(ActorUniqueID) = 0;
     virtual void requestMapInfo(ActorUniqueID, bool) = 0;
     virtual ActorUniqueID expandMapByID(ActorUniqueID, bool) = 0;
     virtual bool copyAndLockMap(ActorUniqueID, ActorUniqueID) = 0;
     virtual MapItemSavedData &createMapSavedData(std::vector<ActorUniqueID> const &, BlockPos const &,
                                                  AutomaticID<Dimension, int>, int) = 0;
     virtual MapItemSavedData &createMapSavedData(ActorUniqueID const &, BlockPos const &, AutomaticID<Dimension, int>,
                                                  int) = 0;
```

### Comparing `endstone-0.4.0/include/bedrock/world/level/level_listener.h` & `endstone-0.4.1/include/bedrock/world/level/level_listener.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/level/storage/saved_data.h` & `endstone-0.4.1/include/bedrock/world/level/storage/saved_data.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/bedrock/world/math/vec3.h` & `endstone-0.4.1/include/bedrock/world/math/vec3.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/actor/actor.h` & `endstone-0.4.1/include/endstone/actor/actor.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/actor/human.h` & `endstone-0.4.1/include/endstone/actor/human.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/color_format.h` & `endstone-0.4.1/include/endstone/color_format.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/command/command.h` & `endstone-0.4.1/include/endstone/command/command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/command/command_executor.h` & `endstone-0.4.1/include/endstone/command/command_executor.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/command/command_map.h` & `endstone-0.4.1/include/endstone/command/command_map.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/command/command_sender.h` & `endstone-0.4.1/include/endstone/command/command_sender.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 class Server;
 class CommandSender : public Permissible {
 public:
     CommandSender() = default;
     ~CommandSender() override = default;
 
+    // Permissible
+    [[nodiscard]] const CommandSender *asCommandSender() const override
+    {
+        return this;
+    }
+
     /**
      * Sends this sender a message
      *
      * @param message Message to be displayed
      */
     virtual void sendMessage(const std::string &message) const = 0;
```

### Comparing `endstone-0.4.0/include/endstone/command/plugin_command.h` & `endstone-0.4.1/include/endstone/command/plugin_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/actor/actor.h` & `endstone-0.4.1/include/endstone/detail/actor/actor.h`

 * *Files 3% similar despite different names*

```diff
@@ -48,11 +48,11 @@
 
     // Actor
     std::uint64_t getRuntimeId() override;
 
 private:
     EndstoneServer &server_;
     ::Actor &actor_;
-    static PermissibleBase mPerm;
+    static PermissibleBase& getPermissibleBase();
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/endstone/detail/actor/human.h` & `endstone-0.4.1/include/endstone/detail/actor/human.h`

 * *Files 1% similar despite different names*

```diff
@@ -42,13 +42,15 @@
     [[nodiscard]] std::unordered_set<PermissionAttachmentInfo *> getEffectivePermissions() const override;
     [[nodiscard]] bool isOp() const override;
     void setOp(bool value) override;
 
     // Actor
     std::uint64_t getRuntimeId() override;
 
+protected:
+    PermissibleBase perm_;
+
 private:
     bool op_;
-    PermissibleBase perm_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/endstone/detail/cast.h` & `endstone-0.4.1/include/endstone/detail/cast.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/bedrock_command.h` & `endstone-0.4.1/include/endstone/detail/command/bedrock_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/command_adapter.h` & `endstone-0.4.1/include/endstone/detail/command/command_adapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #include "bedrock/command/command.h"
 #include "endstone/command/command_sender.h"
 #include "endstone/detail/permissions/permissible_base.h"
 #include "endstone/detail/server.h"
 
 namespace endstone::detail {
 
-class CommandSenderAdapter : public BaseCommandSender {
+class CommandSenderAdapter : public ServerCommandSender {
 public:
     CommandSenderAdapter(const CommandOrigin &origin, CommandOutput &output);
     void sendMessage(const std::string &message) const override;
     void sendErrorMessage(const std::string &message) const override;
     [[nodiscard]] std::string getName() const override;
     [[nodiscard]] bool isOp() const override;
     void setOp(bool value) override;
```

### Comparing `endstone-0.4.0/include/endstone/detail/command/command_lexer.h` & `endstone-0.4.1/include/endstone/detail/command/command_lexer.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/command_map.h` & `endstone-0.4.1/include/endstone/detail/command/command_map.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/command_sender.h` & `endstone-0.4.1/include/endstone/detail/command/server_command_sender.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #pragma once
 
 #include "endstone/command/command_sender.h"
 #include "endstone/detail/permissions/permissible_base.h"
 
 namespace endstone::detail {
 
-class BaseCommandSender : public CommandSender {
+class ServerCommandSender : public CommandSender {
 
 public:
-    BaseCommandSender();
-    explicit BaseCommandSender(PermissibleBase perm);
+    ServerCommandSender();
+    explicit ServerCommandSender(PermissibleBase perm);
     [[nodiscard]] Server &getServer() const override;
     [[nodiscard]] bool isPermissionSet(std::string name) const override;
     [[nodiscard]] bool isPermissionSet(const Permission &perm) const override;
     [[nodiscard]] bool hasPermission(std::string name) const override;
     [[nodiscard]] bool hasPermission(const Permission &perm) const override;
     PermissionAttachment *addAttachment(Plugin &plugin, const std::string &name, bool value) override;
     PermissionAttachment *addAttachment(Plugin &plugin) override;
```

### Comparing `endstone-0.4.0/include/endstone/detail/command/command_usage_parser.h` & `endstone-0.4.1/include/endstone/detail/command/command_usage_parser.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/defaults/debug_command.h` & `endstone-0.4.1/src/endstone_runtime/bedrock/command/command.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#pragma once
+#include "bedrock/command/command.h"
 
-#include "endstone/detail/command/endstone_command.h"
+#include "endstone/detail/hook.h"
 
-namespace endstone::detail {
-class DebugCommand : public EndstoneCommand {
-public:
-    DebugCommand();
-    bool execute(CommandSender &sender, const std::vector<std::string> &args) const override;
-};
-
-}  // namespace endstone::detail
+std::string Command::getCommandName() const
+{
+    std::string result;
+    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&Command::getCommandName, result, this);
+    return result;
+}
```

### Comparing `endstone-0.4.0/include/endstone/detail/command/defaults/plugins_command.h` & `endstone-0.4.1/include/endstone/detail/command/defaults/plugins_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/defaults/version_command.h` & `endstone-0.4.1/include/endstone/detail/command/defaults/version_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/endstone_command.h` & `endstone-0.4.1/include/endstone/detail/command/endstone_command.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/command/server_command_sender.h` & `endstone-0.4.1/include/endstone/detail/command/console_command_sender.h`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #pragma once
 
-#include "command_sender.h"
+#include "server_command_sender.h"
 namespace endstone::detail {
 
-class ServerCommandSender : public BaseCommandSender {
+class ConsoleCommandSender : public ServerCommandSender {
 public:
     void sendMessage(const std::string &message) const override;
     void sendErrorMessage(const std::string &message) const override;
     [[nodiscard]] std::string getName() const override;
     [[nodiscard]] bool isOp() const override;
     void setOp(bool value) override;
 };
```

### Comparing `endstone-0.4.0/include/endstone/detail/hook.h` & `endstone-0.4.1/include/endstone/detail/hook.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/level.h` & `endstone-0.4.1/include/endstone/detail/level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/logger_factory.h` & `endstone-0.4.1/include/endstone/detail/logger_factory.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/os.h` & `endstone-0.4.1/include/endstone/detail/os.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/permissions/default_permissions.h` & `endstone-0.4.1/include/endstone/detail/permissions/default_permissions.h`

 * *Files 4% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 
     static Permission *registerPermission(const std::string &name, Permission *parent = nullptr,
                                           const std::string &desc = "",
                                           PermissionDefault default_value = Permission::DefaultPermission,
                                           const std::unordered_map<std::string, bool> &children = {});
     static void registerCorePermissions();
     static void registerCommandPermissions(Permission *parent);
+    static void registerBroadcastPermissions(Permission *parent);
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/endstone/detail/permissions/permissible_base.h` & `endstone-0.4.1/include/endstone/detail/permissions/permissible_base.h`

 * *Files 7% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 namespace endstone::detail {
 
 /**
  * Base Permissible for use in any Permissible object via proxy or extension
  */
 class PermissibleBase : public Permissible {
 public:
-    explicit PermissibleBase(Permissible *opable) : opable_(opable), parent_(opable ? *opable : *this) {}
+    explicit PermissibleBase(Permissible *opable);
 
     [[nodiscard]] bool isOp() const override;
     void setOp(bool value) override;
     [[nodiscard]] bool isPermissionSet(std::string name) const override;
     [[nodiscard]] bool isPermissionSet(const Permission &perm) const override;
     [[nodiscard]] bool hasPermission(std::string name) const override;
     [[nodiscard]] bool hasPermission(const Permission &perm) const override;
     PermissionAttachment *addAttachment(Plugin &plugin, const std::string &name, bool value) override;
     PermissionAttachment *addAttachment(Plugin &plugin) override;
     bool removeAttachment(PermissionAttachment &attachment) override;
     void recalculatePermissions() override;
     [[nodiscard]] std::unordered_set<PermissionAttachmentInfo *> getEffectivePermissions() const override;
+    [[nodiscard]] const CommandSender *asCommandSender() const override;
+    void clearPermissions();
 
 private:
     void calculateChildPermissions(const std::unordered_map<std::string, bool> &children, bool invert,
                                    PermissionAttachment *attachment);
     [[nodiscard]] static bool hasPermission(PermissionDefault default_value, bool op);
     Permissible *opable_;
     Permissible &parent_;
```

### Comparing `endstone-0.4.0/include/endstone/detail/player.h` & `endstone-0.4.1/include/endstone/detail/player.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,13 +50,15 @@
 
     // Player
     [[nodiscard]] UUID getUniqueId() const override;
     void sendRawMessage(std::string message) const override;
     void sendPopup(std::string message) const override;
     void sendTip(std::string message) const override;
 
+    void disconnect();
+
 private:
     ::Player &player_;
     UUID uuid_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/endstone/detail/plugin/cpp_plugin_loader.h` & `endstone-0.4.1/include/endstone/detail/plugin/cpp_plugin_loader.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/plugin/plugin_description_builder.h` & `endstone-0.4.1/include/endstone/detail/plugin/plugin_description_builder.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/plugin/plugin_manager.h` & `endstone-0.4.1/include/endstone/detail/plugin/plugin_manager.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/plugin/python_plugin_loader.h` & `endstone-0.4.1/include/endstone/detail/plugin/python_plugin_loader.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/pybind_type_caster.h` & `endstone-0.4.1/include/endstone/detail/pybind_type_caster.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/server.h` & `endstone-0.4.1/include/endstone/detail/server.h`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #include <memory>
 #include <string>
 #include <string_view>
 
 #include "bedrock/server/server_instance.h"
 #include "endstone/detail/command/command_map.h"
-#include "endstone/detail/command/server_command_sender.h"
+#include "endstone/detail/command/console_command_sender.h"
 #include "endstone/detail/plugin/plugin_manager.h"
 #include "endstone/level.h"
 #include "endstone/plugin/plugin_manager.h"
 #include "endstone/server.h"
 
 namespace endstone::detail {
 
@@ -33,14 +33,18 @@
     explicit EndstoneServer(ServerInstance &server_instance);
     EndstoneServer(EndstoneServer const &) = delete;
     EndstoneServer(EndstoneServer &&) = delete;
     EndstoneServer &operator=(EndstoneServer const &) = delete;
     EndstoneServer &operator=(EndstoneServer &&) = delete;
     ~EndstoneServer() override = default;
 
+    [[nodiscard]] std::string getName() const override;
+    [[nodiscard]] std::string getVersion() const override;
+    [[nodiscard]] std::string getMinecraftVersion() const override;
+
     [[nodiscard]] Logger &getLogger() const override;
     [[nodiscard]] EndstoneCommandMap &getCommandMap() const;
     [[nodiscard]] MinecraftCommands &getMinecraftCommands();
     [[nodiscard]] PluginManager &getPluginManager() const override;
     [[nodiscard]] PluginCommand *getPluginCommand(std::string name) const override;
     [[nodiscard]] CommandSender &getCommandSender() const override;
 
@@ -50,23 +54,23 @@
 
     std::vector<Level *> getLevels() const override;
     Level *getLevel(std::string name) const override;
     void addLevel(std::unique_ptr<Level> level);
 
     [[nodiscard]] Player *getPlayer(endstone::UUID id) const override;
 
-    [[nodiscard]] std::string getName() const override;
-    [[nodiscard]] std::string getVersion() const override;
-    [[nodiscard]] std::string getMinecraftVersion() const override;
+    void broadcast(const std::string &message, const std::string &permission) const override;
+    void broadcastMessage(const std::string &message) const override;
+
     bool isPrimaryThread() const override;
 
 private:
     void enablePlugin(Plugin &plugin);
     ServerInstance &server_instance_;
     Logger &logger_;
     std::unique_ptr<EndstoneCommandMap> command_map_;
     std::unique_ptr<EndstonePluginManager> plugin_manager_;
-    mutable ServerCommandSender command_sender_;
+    mutable ConsoleCommandSender command_sender_;
     std::unordered_map<std::string, std::unique_ptr<Level>> levels_;
 };
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/include/endstone/detail/signal_handler.h` & `endstone-0.4.1/include/endstone/detail/signal_handler.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/spdlog/level_formatter.h` & `endstone-0.4.1/include/endstone/detail/spdlog/level_formatter.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/spdlog/log_sink.h` & `endstone-0.4.1/include/endstone/detail/spdlog/log_sink.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/spdlog/spdlog_adapter.h` & `endstone-0.4.1/include/endstone/detail/spdlog/spdlog_adapter.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/spdlog/text_formatter.h` & `endstone-0.4.1/include/endstone/detail/spdlog/text_formatter.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/detail/virtual_table.h` & `endstone-0.4.1/include/endstone/detail/virtual_table.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/dimension.h` & `endstone-0.4.1/include/endstone/dimension.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/endstone.h` & `endstone-0.4.1/include/endstone/endstone.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #pragma once
 
 #define ENDSTONE_STRINGIFY(x) #x
 #define ENDSTONE_TOSTRING(x)  ENDSTONE_STRINGIFY(x)
 
 #define ENDSTONE_VERSION_MAJOR 0
 #define ENDSTONE_VERSION_MINOR 4
-#define ENDSTONE_VERSION_PATCH 0
+#define ENDSTONE_VERSION_PATCH 1
 #define ENDSTONE_API_VERSION   ENDSTONE_TOSTRING(ENDSTONE_VERSION_MAJOR) "." ENDSTONE_TOSTRING(ENDSTONE_VERSION_MINOR);
 
 #if !defined(ENDSTONE_EXPORT)
 #if defined(WIN32) || defined(_WIN32)
 #define ENDSTONE_EXPORT __declspec(dllexport)
 #else
 #define ENDSTONE_EXPORT __attribute__((visibility("default")))
```

### Comparing `endstone-0.4.0/include/endstone/event/actor/actor_event.h` & `endstone-0.4.1/include/endstone/event/actor/actor_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/actor/actor_remove_event.h` & `endstone-0.4.1/include/endstone/event/actor/actor_remove_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/actor/actor_spawn_event.h` & `endstone-0.4.1/include/endstone/event/actor/actor_spawn_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/event.h` & `endstone-0.4.1/include/endstone/event/event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/event_handler.h` & `endstone-0.4.1/include/endstone/event/event_handler.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/event_priority.h` & `endstone-0.4.1/include/endstone/event/event_priority.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/handler_list.h` & `endstone-0.4.1/include/endstone/event/handler_list.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/player/player_chat_event.h` & `endstone-0.4.1/include/endstone/event/player/player_chat_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/player/player_event.h` & `endstone-0.4.1/include/endstone/event/player/player_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/player/player_join_event.h` & `endstone-0.4.1/include/endstone/event/player/player_join_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/player/player_quit_event.h` & `endstone-0.4.1/include/endstone/event/player/player_quit_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/server/plugin_disable_event.h` & `endstone-0.4.1/include/endstone/event/server/plugin_disable_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/server/plugin_enable_event.h` & `endstone-0.4.1/include/endstone/event/server/plugin_enable_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/server/server_command_event.h` & `endstone-0.4.1/include/endstone/event/server/server_command_event.h`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 
     [[nodiscard]] bool isCancellable() const override
     {
         return true;
     }
 
     /**
-     * Gets the command that the user is attempting to execute from the console
+     * Gets the command that the server is attempting to execute from the console
      *
-     * @return Command the user is attempting to execute
+     * @return Command the server is attempting to execute
      */
     [[nodiscard]] std::string getCommand() const
     {
         return command_;
     }
 
     /**
```

### Comparing `endstone-0.4.0/include/endstone/event/server/server_list_ping_event.h` & `endstone-0.4.1/include/endstone/event/server/server_list_ping_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/server/server_load_event.h` & `endstone-0.4.1/include/endstone/event/server/server_load_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/weather/thunder_change_event.h` & `endstone-0.4.1/include/endstone/event/weather/thunder_change_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/weather/weather_change_event.h` & `endstone-0.4.1/include/endstone/event/weather/weather_change_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/event/weather/weather_event.h` & `endstone-0.4.1/include/endstone/event/weather/weather_event.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/game_mode.h` & `endstone-0.4.1/include/endstone/game_mode.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/level.h` & `endstone-0.4.1/include/endstone/level.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/logger.h` & `endstone-0.4.1/include/endstone/logger.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/permissions/permissible.h` & `endstone-0.4.1/include/endstone/permissions/permissible.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #include <string>
 #include <unordered_set>
 
 #include "endstone/permissions/permission_attachment_info.h"
 
 namespace endstone {
 
+class CommandSender;
 class Plugin;
 class Permission;
 class PermissionAttachment;
 
 /**
  * Represents an object that may become a server operator and can be assigned permissions.
  */
@@ -114,9 +115,11 @@
 
     /**
      * Gets a set containing all of the permissions currently in effect by this object
      *
      * @return Set of currently effective permissions
      */
     [[nodiscard]] virtual std::unordered_set<PermissionAttachmentInfo *> getEffectivePermissions() const = 0;
+
+    [[nodiscard]] virtual const CommandSender *asCommandSender() const = 0;
 };
 }  // namespace endstone
```

### Comparing `endstone-0.4.0/include/endstone/permissions/permission.h` & `endstone-0.4.1/include/endstone/permissions/permission.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/permissions/permission_attachment.h` & `endstone-0.4.1/include/endstone/permissions/permission_attachment.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/permissions/permission_attachment_info.h` & `endstone-0.4.1/include/endstone/permissions/permission_attachment_info.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/permissions/permission_default.h` & `endstone-0.4.1/include/endstone/permissions/permission_default.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/player.h` & `endstone-0.4.1/include/endstone/player.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/plugin/plugin.h` & `endstone-0.4.1/include/endstone/plugin/plugin.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/plugin/plugin_description.h` & `endstone-0.4.1/include/endstone/plugin/plugin_description.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/plugin/plugin_load_order.h` & `endstone-0.4.1/include/endstone/plugin/plugin_load_order.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/plugin/plugin_loader.h` & `endstone-0.4.1/include/endstone/plugin/plugin_loader.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/plugin/plugin_manager.h` & `endstone-0.4.1/include/endstone/plugin/plugin_manager.h`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/include/endstone/util/uuid.h` & `endstone-0.4.1/include/endstone/util/uuid.h`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,14 @@
 /**
  * Implementation of Universally Unique Identifier (UUID)
  *
  * Adapted from https://github.com/boostorg/uuid/blob/develop/include/boost/uuid/uuid.hpp
  */
 class UUID {
 public:
-    UUID() : data{0} {}
-    UUID(std::int64_t msb, std::int64_t lsb)
-    {
-        bits.most_significant = msb;
-        bits.least_significant = lsb;
-    }
-
     std::uint8_t *begin() noexcept
     {
         return data;
     }
 
     [[nodiscard]] const uint8_t *begin() const noexcept
     {
@@ -106,22 +99,15 @@
             if (i == 3 || i == 5 || i == 7 || i == 9) {
                 result.push_back('-');
             }
         }
 
         return result;
     }
-
-    union {
-        std::uint8_t data[16];
-        struct {
-            std::int64_t most_significant;
-            std::int64_t least_significant;
-        } bits;
-    };
+    std::uint8_t data[16];
 };
 static_assert(sizeof(endstone::UUID) == endstone::UUID::size());
 
 inline bool operator==(UUID const &lhs, UUID const &rhs) noexcept
 {
     return memcmp(lhs.data, rhs.data, sizeof(lhs.data)) == 0;
 }
```

### Comparing `endstone-0.4.0/mkdocs.yml` & `endstone-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/pyproject.toml` & `endstone-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/_internal/bootstrap/__init__.py` & `endstone-0.4.1/python/src/endstone/_internal/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/_internal/bootstrap/base.py` & `endstone-0.4.1/python/src/endstone/_internal/bootstrap/base.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/_internal/bootstrap/linux.py` & `endstone-0.4.1/python/src/endstone/_internal/bootstrap/linux.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/_internal/bootstrap/windows.py` & `endstone-0.4.1/python/src/endstone/_internal/bootstrap/windows.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/_internal/endstone_python.pyi` & `endstone-0.4.1/python/src/endstone/_internal/endstone_python.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 from __future__ import annotations
 import typing
 import uuid
-__all__ = ['Actor', 'ActorRemoveEvent', 'ActorSpawnEvent', 'ColorFormat', 'Command', 'CommandExecutor', 'CommandSender', 'Event', 'EventPriority', 'GameMode', 'HumanActor', 'Level', 'Logger', 'Permissible', 'Permission', 'PermissionAttachment', 'PermissionAttachmentInfo', 'PermissionDefault', 'Player', 'PlayerChatEvent', 'PlayerJoinEvent', 'PlayerQuitEvent', 'Plugin', 'PluginCommand', 'PluginDescription', 'PluginDisableEvent', 'PluginEnableEvent', 'PluginLoadOrder', 'PluginLoader', 'PluginManager', 'Server', 'ServerCommandEvent', 'ServerListPingEvent', 'ServerLoadEvent', 'ThunderChangeEvent', 'WeatherChangeEvent']
+__all__ = ['Actor', 'ActorRemoveEvent', 'ActorSpawnEvent', 'BroadcastMessageEvent', 'ColorFormat', 'Command', 'CommandExecutor', 'CommandSender', 'Event', 'EventPriority', 'GameMode', 'HumanActor', 'Level', 'Logger', 'Permissible', 'Permission', 'PermissionAttachment', 'PermissionAttachmentInfo', 'PermissionDefault', 'Player', 'PlayerChatEvent', 'PlayerCommandEvent', 'PlayerJoinEvent', 'PlayerQuitEvent', 'Plugin', 'PluginCommand', 'PluginDescription', 'PluginDisableEvent', 'PluginEnableEvent', 'PluginLoadOrder', 'PluginLoader', 'PluginManager', 'Server', 'ServerCommandEvent', 'ServerListPingEvent', 'ServerLoadEvent', 'ThunderChangeEvent', 'WeatherChangeEvent']
 class Actor(CommandSender):
     pass
 class ActorRemoveEvent(Event):
     @property
     def actor(self) -> Actor:
         """
         Returns the Actor being removed
         """
 class ActorSpawnEvent(Event):
     @property
     def actor(self) -> Actor:
         """
         Returns the Actor being spawned
         """
+class BroadcastMessageEvent(Event):
+    @property
+    def message(self) -> str:
+        """
+        The message to broadcast.
+        """
+    @message.setter
+    def message(self, arg1: str) -> None:
+        ...
+    @property
+    def recipients(self) -> set[CommandSender]:
+        """
+        Gets a set of recipients that this broadcast message will be displayed to.
+        """
 class ColorFormat:
     AQUA: typing.ClassVar[str] = '§b'
     BLACK: typing.ClassVar[str] = '§0'
     BLUE: typing.ClassVar[str] = '§9'
     BOLD: typing.ClassVar[str] = '§l'
     DARK_AQUA: typing.ClassVar[str] = '§3'
     DARK_BLUE: typing.ClassVar[str] = '§1'
@@ -645,15 +659,29 @@
         """
     @message.setter
     def message(self, arg1: str) -> None:
         ...
     @property
     def player(self) -> Player:
         """
-        Returns the Player who joins the server
+        Returns the Player who sends the message
+        """
+class PlayerCommandEvent(Event):
+    @property
+    def command(self) -> str:
+        """
+        The command that the player will send.
+        """
+    @command.setter
+    def command(self, arg1: str) -> None:
+        ...
+    @property
+    def player(self) -> Player:
+        """
+        Returns the Player who sends the command
         """
 class PlayerJoinEvent(Event):
     @property
     def player(self) -> Player:
         """
         Returns the Player who joins the server
         """
```

### Comparing `endstone-0.4.0/python/src/endstone/_internal/plugin_loader.py` & `endstone-0.4.1/python/src/endstone/_internal/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/src/endstone/event.py` & `endstone-0.4.1/python/src/endstone/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from endstone._internal.endstone_python import (
     Event,
     EventPriority,
     ActorRemoveEvent,
     ActorSpawnEvent,
     PlayerChatEvent,
+    PlayerCommandEvent,
     PlayerJoinEvent,
     PlayerQuitEvent,
+    BroadcastMessageEvent,
     PluginEnableEvent,
     PluginDisableEvent,
     ServerCommandEvent,
     ServerListPingEvent,
     ServerLoadEvent,
     ThunderChangeEvent,
     WeatherChangeEvent,
@@ -18,16 +20,18 @@
 __all__ = [
     "event_handler",
     "Event",
     "EventPriority",
     "ActorRemoveEvent",
     "ActorSpawnEvent",
     "PlayerChatEvent",
+    "PlayerCommandEvent",
     "PlayerJoinEvent",
     "PlayerQuitEvent",
+    "BroadcastMessageEvent",
     "PluginEnableEvent",
     "PluginDisableEvent",
     "ServerCommandEvent",
     "ServerListPingEvent",
     "ServerLoadEvent",
     "ThunderChangeEvent",
     "WeatherChangeEvent",
```

### Comparing `endstone-0.4.0/python/src/endstone/plugin.py` & `endstone-0.4.1/python/src/endstone/plugin.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/tests/test_color_format.py` & `endstone-0.4.1/python/tests/test_color_format.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/python/tests/test_plugin_description.py` & `endstone-0.4.1/python/tests/test_plugin_description.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/actor/human.cpp` & `endstone-0.4.1/src/endstone_core/actor/human.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/bedrock_command.cpp` & `endstone-0.4.1/src/endstone_core/command/bedrock_command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/command_adapter.cpp` & `endstone-0.4.1/src/endstone_core/command/command_adapter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/command_lexer.cpp` & `endstone-0.4.1/src/endstone_core/command/command_lexer.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/command_map.cpp` & `endstone-0.4.1/src/endstone_core/command/command_map.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,20 @@
 #include "endstone/detail/command/command_map.h"
 
 #include <algorithm>
 #include <string>
 #include <unordered_map>
 #include <vector>
 
-#include "bedrock/command/command.h"
 #include "bedrock/command/command_registry.h"
 #include "bedrock/i18n.h"
-#include "bedrock/type_id.h"
 #include "endstone/command/plugin_command.h"
 #include "endstone/detail/command/bedrock_command.h"
 #include "endstone/detail/command/command_adapter.h"
 #include "endstone/detail/command/command_usage_parser.h"
-#include "endstone/detail/command/defaults/debug_command.h"
 #include "endstone/detail/command/defaults/plugins_command.h"
 #include "endstone/detail/command/defaults/version_command.h"
 #include "endstone/detail/server.h"
 
 namespace endstone::detail {
 
 EndstoneCommandMap::EndstoneCommandMap(EndstoneServer &server) : server_(server) {}
@@ -61,15 +58,14 @@
     }
 
     return it->second.get();
 }
 
 void EndstoneCommandMap::setDefaultCommands()
 {
-    registerCommand(std::make_unique<DebugCommand>());
     registerCommand(std::make_unique<PluginsCommand>());
     registerCommand(std::make_unique<VersionCommand>());
 }
 
 void EndstoneCommandMap::setMinecraftCommands()
 {
     auto &commands = server_.getMinecraftCommands();
@@ -78,15 +74,15 @@
     std::unordered_map<std::string, std::vector<std::string>> command_aliases;
     for (const auto &[alias, command_name] : registry.aliases) {
         auto it = command_aliases.emplace(command_name, std::vector<std::string>()).first;
         it->second.push_back(alias);
     }
 
     for (const auto &[command_name, signature] : registry.commands) {
-        auto description = I18n::get(signature.description, {}, nullptr);
+        auto description = getI18n().get(signature.description, {}, nullptr);
 
         std::vector<std::string> usages;
         usages.reserve(signature.overloads.size());
         for (const auto &overload : signature.overloads) {
             usages.push_back(registry.describe(signature, overload));
         }
```

### Comparing `endstone-0.4.0/src/endstone_core/command/command_sender.cpp` & `endstone-0.4.1/src/endstone_core/actor/actor.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -8,72 +8,104 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "endstone/detail/command/command_sender.h"
+#include "endstone/detail/actor/actor.h"
 
-#include <utility>
+#include "bedrock/command/command_utils.h"
+#include "bedrock/world/actor/actor.h"
 
-#include <entt/entt.hpp>
+namespace endstone::detail {
 
-#include "endstone/detail/server.h"
+EndstoneActor::EndstoneActor(EndstoneServer &server, ::Actor &actor) : server_(server), actor_(actor)
+{
+    getPermissibleBase();
+}
 
-namespace endstone::detail {
+void EndstoneActor::sendMessage(const std::string &message) const {}
+
+void EndstoneActor::sendErrorMessage(const std::string &message) const {}
+
+Server &EndstoneActor::getServer() const
+{
+    return server_;
+}
+
+std::string EndstoneActor::getName() const
+{
+    return CommandUtils::getActorName(actor_);
+}
 
-BaseCommandSender::BaseCommandSender() : perm_(this) {}
+bool EndstoneActor::isPermissionSet(std::string name) const
+{
+    return getPermissibleBase().isPermissionSet(name);
+}
 
-BaseCommandSender::BaseCommandSender(PermissibleBase perm) : perm_(std::move(perm)) {}
+bool EndstoneActor::isPermissionSet(const Permission &perm) const
+{
+    return getPermissibleBase().isPermissionSet(perm);
+}
+
+bool EndstoneActor::hasPermission(std::string name) const
+{
+    return getPermissibleBase().hasPermission(name);
+}
 
-Server &BaseCommandSender::getServer() const
+bool EndstoneActor::hasPermission(const Permission &perm) const
 {
-    return entt::locator<EndstoneServer>::value();
+    return getPermissibleBase().hasPermission(perm);
 }
 
-bool BaseCommandSender::isPermissionSet(std::string name) const
+PermissionAttachment *EndstoneActor::addAttachment(Plugin &plugin, const std::string &name, bool value)
 {
-    return perm_.isPermissionSet(name);
+    return getPermissibleBase().addAttachment(plugin, name, value);
 }
 
-bool BaseCommandSender::isPermissionSet(const Permission &perm) const
+PermissionAttachment *EndstoneActor::addAttachment(Plugin &plugin)
 {
-    return perm_.isPermissionSet(perm);
+    return getPermissibleBase().addAttachment(plugin);
 }
 
-bool BaseCommandSender::hasPermission(std::string name) const
+bool EndstoneActor::removeAttachment(PermissionAttachment &attachment)
 {
-    return perm_.hasPermission(name);
+    return getPermissibleBase().removeAttachment(attachment);
 }
 
-bool BaseCommandSender::hasPermission(const Permission &perm) const
+void EndstoneActor::recalculatePermissions()
 {
-    return perm_.hasPermission(perm);
+    getPermissibleBase().recalculatePermissions();
 }
 
-PermissionAttachment *BaseCommandSender::addAttachment(Plugin &plugin, const std::string &name, bool value)
+std::unordered_set<PermissionAttachmentInfo *> EndstoneActor::getEffectivePermissions() const
 {
-    return perm_.addAttachment(plugin, name, value);
+    return getPermissibleBase().getEffectivePermissions();
 }
 
-PermissionAttachment *BaseCommandSender::addAttachment(Plugin &plugin)
+bool EndstoneActor::isOp() const
 {
-    return perm_.addAttachment(plugin);
+    return getPermissibleBase().isOp();
 }
 
-bool BaseCommandSender::removeAttachment(PermissionAttachment &attachment)
+void EndstoneActor::setOp(bool value)
 {
-    return perm_.removeAttachment(attachment);
+    getPermissibleBase().setOp(value);
 }
 
-void BaseCommandSender::recalculatePermissions()
+std::uint64_t EndstoneActor::getRuntimeId()
 {
-    perm_.recalculatePermissions();
+    return actor_.getRuntimeID().id;
 }
 
-std::unordered_set<PermissionAttachmentInfo *> BaseCommandSender::getEffectivePermissions() const
+PermissibleBase &EndstoneActor::getPermissibleBase()
 {
-    return perm_.getEffectivePermissions();
+    static std::unique_ptr<PermissibleBase> perm = []() {
+        auto instance = std::make_unique<PermissibleBase>(nullptr);
+        instance->recalculatePermissions();
+        return instance;
+    }();
+    return *perm;
 }
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/command/command_usage_parser.cpp` & `endstone-0.4.1/src/endstone_core/command/command_usage_parser.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/defaults/debug_command.cpp` & `endstone-0.4.1/include/endstone/detail/scheduler/scheduler.h`

 * *Files 21% similar despite different names*

```diff
@@ -8,50 +8,39 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "endstone/detail/command/defaults/debug_command.h"
+#pragma once
 
-#include <sstream>
-#include <string>
-#include <vector>
+#include <atomic>
+#include <queue>
 
-#include <entt/entt.hpp>
-
-#include "endstone/color_format.h"
-#include "endstone/detail/command/command_map.h"
-#include "endstone/detail/server.h"
+#include "endstone/detail/scheduler/task.h"
+#include "endstone/scheduler/scheduler.h"
 
 namespace endstone::detail {
 
-DebugCommand::DebugCommand() : EndstoneCommand("debug")
-{
-    setDescription("Toggle the debug mode");
-    setUsages("/debug <toggle: bool>");
-    setPermissions("endstone.command.debug");
-}
-
-bool DebugCommand::execute(CommandSender &sender, const std::vector<std::string> &args) const
-{
-    auto &server = entt::locator<EndstoneServer>::value();
-    if (&sender != &server.getCommandSender()) {
-        return true;
-    }
-
-    auto enabled = args[0];
-    std::transform(enabled.begin(), enabled.end(), enabled.begin(), [](unsigned char c) { return std::tolower(c); });
-
-    if (enabled == "true") {
-        server.getLogger().setLevel(Logger::Level::Debug);
-        sender.sendMessage("Debug mode is enabled.");
-    }
-    else {
-        server.getLogger().setLevel(Logger::Level::Info);
-        sender.sendMessage("Debug mode is disabled.");
-    }
-    return true;
-}
+class EndstoneScheduler {
+private:
+    struct PendingTaskComparator {
+        bool operator()(const EndstoneTask &lhs, const EndstoneTask &rhs)
+        {
+            if (lhs.getNextRun() != rhs.getNextRun()) {
+                return lhs.getNextRun() > rhs.getNextRun();
+            }
+            return lhs.getCreatedAt() > rhs.getCreatedAt();
+        }
+    };
+
+public:
+protected:
+    TaskId incrementIds();
+
+private:
+    std::atomic<TaskId> ids_{1};
+    std::priority_queue<EndstoneTask, std::vector<EndstoneTask>, PendingTaskComparator> pending_;
+};
 
-};  // namespace endstone::detail
+}  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/command/defaults/plugins_command.cpp` & `endstone-0.4.1/src/endstone_core/command/defaults/plugins_command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/defaults/version_command.cpp` & `endstone-0.4.1/src/endstone_core/command/defaults/version_command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/command/server_command_sender.cpp` & `endstone-0.4.1/src/endstone_core/command/console_command_sender.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,38 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "endstone/detail/command/server_command_sender.h"
-
+#include "endstone/detail/command/console_command_sender.h"
 #include "endstone/detail/server.h"
 
 namespace endstone::detail {
 
-void ServerCommandSender::sendMessage(const std::string &message) const
+void ConsoleCommandSender::sendMessage(const std::string &message) const
 {
     getServer().getLogger().info(message);
 }
 
-void ServerCommandSender::sendErrorMessage(const std::string &message) const
+void ConsoleCommandSender::sendErrorMessage(const std::string &message) const
 {
     getServer().getLogger().error(message);
 }
 
-std::string ServerCommandSender::getName() const
+std::string ConsoleCommandSender::getName() const
 {
     return "Server";
 }
 
-bool ServerCommandSender::isOp() const
+bool ConsoleCommandSender::isOp() const
 {
     return true;
 }
 
-void ServerCommandSender::setOp(bool value)
+void ConsoleCommandSender::setOp(bool value)
 {
     getServer().getLogger().error("Cannot change operator status of server console");
 }
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/event/server/server_list_ping_event.cpp` & `endstone-0.4.1/src/endstone_core/event/server/server_list_ping_event.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/level.cpp` & `endstone-0.4.1/src/endstone_core/level.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/logger_factory.cpp` & `endstone-0.4.1/src/endstone_core/logger_factory.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/permissions/default_permissions.cpp` & `endstone-0.4.1/src/endstone_core/permissions/default_permissions.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -33,28 +33,37 @@
                                                    const std::unordered_map<std::string, bool> &children)
 {
     return registerPermission(std::make_unique<Permission>(name, desc, default_value, children), parent);
 }
 
 void DefaultPermissions::registerCorePermissions()
 {
-    auto *endstone = registerPermission("endstone", nullptr,
-                                        "Gives the user the ability to use all Endstone utilities and commands");
-    registerCommandPermissions(endstone);
-    // TODO(permission): registerBroadcastPermissions (endstone.broadcast)
-    endstone->recalculatePermissibles();
+    auto *root = registerPermission("endstone", nullptr,
+                                    "Gives the user the ability to use all Endstone utilities and commands");
+    registerCommandPermissions(root);
+    registerBroadcastPermissions(root);
+    root->recalculatePermissibles();
 }
 
 void DefaultPermissions::registerCommandPermissions(Permission *parent)
 {
-    auto *command =
-        registerPermission("endstone.command", parent, "Gives the user the ability to use all Endstone command");
-    registerPermission("endstone.command.debug", command, "Allows the user to toggle the debug mode of this server",
-                       PermissionDefault::Operator);
-    registerPermission("endstone.command.plugins", command,
+    auto *root = registerPermission(parent->getName() + ".command", parent,
+                                    "Gives the user the ability to use all Endstone command");
+    registerPermission(root->getName() + ".plugins", root,
                        "Allows the user to view the list of plugins running on this server", PermissionDefault::True);
-    registerPermission("endstone.command.version", command, "Allows the user to view the version of the server",
-                       PermissionDefault::True);
-    command->recalculatePermissibles();
+    registerPermission(root->getName() + ".version", root,  //
+                       "Allows the user to view the version of the server", PermissionDefault::True);
+    root->recalculatePermissibles();
+}
+
+void DefaultPermissions::registerBroadcastPermissions(Permission *parent)
+{
+    auto *root = registerPermission(parent->getName() + ".broadcast", parent,
+                                    "Allows the user to receive all broadcast messages");
+    registerPermission(root->getName() + ".admin", root,  //
+                       "Allows the user to receive administrative broadcasts", PermissionDefault::Operator);
+    registerPermission(root->getName() + ".user", root,  //
+                       "Allows the user to receive user broadcasts", PermissionDefault::True);
+    root->recalculatePermissibles();
 }
 
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/permissions/permissible_base.cpp` & `endstone-0.4.1/src/endstone_core/permissions/permissible_base.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 #include "endstone/detail/server.h"
 #include "endstone/permissions/permission.h"
 #include "endstone/permissions/permission_attachment_info.h"
 
 namespace endstone::detail {
 
+PermissibleBase::PermissibleBase(Permissible *opable) : opable_(opable), parent_(opable ? *opable : *this) {}
+
 bool PermissibleBase::isOp() const
 {
     if (opable_) {
         return opable_->isOp();
     }
     return false;
 }
@@ -129,23 +131,15 @@
 }
 
 void PermissibleBase::recalculatePermissions()
 {
     auto &server = entt::locator<EndstoneServer>::value();
     auto &plugin_manager = server.getPluginManager();
 
-    // Clear permissions
-    for (const auto &[name, perm] : permissions_) {
-        plugin_manager.unsubscribeFromPermission(name, parent_);
-    }
-    plugin_manager.unsubscribeFromDefaultPerms(false, parent_);
-    plugin_manager.unsubscribeFromDefaultPerms(true, parent_);
-    permissions_.clear();
-
-    // Recalculate permissions
+    clearPermissions();
     auto defaults = plugin_manager.getDefaultPermissions(isOp());
     plugin_manager.subscribeToDefaultPerms(isOp(), parent_);
 
     for (auto *perm : defaults) {
         auto name = perm->getName();
         std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
         permissions_.emplace(name, std::make_unique<PermissionAttachmentInfo>(parent_, name, nullptr, true));
@@ -184,8 +178,30 @@
     std::unordered_set<PermissionAttachmentInfo *> result;
     for (const auto &entry : permissions_) {
         result.insert(entry.second.get());
     }
     return result;
 }
 
+const CommandSender *PermissibleBase::asCommandSender() const
+{
+    if (opable_) {
+        return opable_->asCommandSender();
+    }
+    return nullptr;
+}
+
+void PermissibleBase::clearPermissions()
+{
+    auto &server = entt::locator<EndstoneServer>::value();
+    auto &plugin_manager = server.getPluginManager();
+
+    // Clear permissions
+    for (const auto &[name, perm] : permissions_) {
+        plugin_manager.unsubscribeFromPermission(name, parent_);
+    }
+    plugin_manager.unsubscribeFromDefaultPerms(false, parent_);
+    plugin_manager.unsubscribeFromDefaultPerms(true, parent_);
+    permissions_.clear();
+}
+
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/player.cpp` & `endstone-0.4.1/src/endstone_core/player.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 EndstonePlayer::EndstonePlayer(EndstoneServer &server, ::Player &player)
     : EndstoneHumanActor(server, player), player_(player)
 {
     auto *component = player.tryGetComponent<UserEntityIdentifierComponent>();
     if (!component) {
         throw std::runtime_error("UserEntityIdentifierComponent is not valid");
     }
-    uuid_ = {component->uuid.msb, component->uuid.lsb};
+    uuid_ = component->uuid.toEndstone();
 }
 
 void EndstonePlayer::sendMessage(const std::string &message) const
 {
     sendRawMessage(message);
 }
 
@@ -101,14 +101,18 @@
 bool EndstonePlayer::isOp() const
 {
     return player_.getCommandPermissionLevel() != CommandPermissionLevel::Any;
 }
 
 void EndstonePlayer::setOp(bool value)
 {
+    if (value == isOp()) {
+        return;
+    }
+
     player_.setPermissions(value ? CommandPermissionLevel::Any : CommandPermissionLevel::GameDirectors);
 }
 
 std::uint64_t EndstonePlayer::getRuntimeId()
 {
     return EndstoneHumanActor::getRuntimeId();
 }
@@ -141,8 +145,13 @@
     auto packet = MinecraftPackets::createPacket(MinecraftPacketIds::Text);
     std::shared_ptr<TextPacket> text_packet = std::static_pointer_cast<TextPacket>(packet);
     text_packet->type = TextPacketType::Tip;
     text_packet->message = message;
     player_.sendNetworkPacket(*packet);
 }
 
+void EndstonePlayer::disconnect()
+{
+    perm_.clearPermissions();
+}
+
 }  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_core/plugin/cpp_plugin_loader.cpp` & `endstone-0.4.1/src/endstone_core/plugin/cpp_plugin_loader.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/plugin/plugin_manager.cpp` & `endstone-0.4.1/src/endstone_core/plugin/plugin_manager.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     }
 }
 
 void EndstonePluginManager::subscribeToPermission(std::string permission, Permissible &permissible)
 {
     auto &name = permission;
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
-    auto map = perm_subs_.emplace(name, std::unordered_map<Permissible *, bool>()).first->second;
+    auto &map = perm_subs_.emplace(name, std::unordered_map<Permissible *, bool>()).first->second;
     map[&permissible] = true;
 }
 
 void EndstonePluginManager::unsubscribeFromPermission(std::string permission, Permissible &permissible)
 {
     auto &name = permission;
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
@@ -308,15 +308,15 @@
         return subs;
     }
     return {};
 }
 
 void EndstonePluginManager::subscribeToDefaultPerms(bool op, Permissible &permissible)
 {
-    auto map = def_subs_.emplace(op, std::unordered_map<Permissible *, bool>()).first->second;
+    auto &map = def_subs_.emplace(op, std::unordered_map<Permissible *, bool>()).first->second;
     map[&permissible] = true;
 }
 
 void EndstonePluginManager::unsubscribeFromDefaultPerms(bool op, Permissible &permissible)
 {
     auto it = def_subs_.find(op);
     if (it != def_subs_.end()) {
```

### Comparing `endstone-0.4.0/src/endstone_core/server.cpp` & `endstone-0.4.1/src/endstone_core/server.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #include "bedrock/world/actor/player/player.h"
 #include "endstone/command/plugin_command.h"
 #include "endstone/detail/command/command_map.h"
 #include "endstone/detail/level.h"
 #include "endstone/detail/logger_factory.h"
 #include "endstone/detail/permissions/default_permissions.h"
 #include "endstone/detail/plugin/cpp_plugin_loader.h"
+#include "endstone/event/server/broadcast_message_event.h"
 #include "endstone/plugin/plugin.h"
 
 #if !defined(ENDSTONE_VERSION)
 #error ENDSTONE_VERSION is not defined
 #endif
 
 namespace endstone::detail {
@@ -39,14 +40,62 @@
     : server_instance_(server_instance), logger_(LoggerFactory::getLogger("Server"))
 {
     command_map_ = std::make_unique<EndstoneCommandMap>(*this);
     plugin_manager_ = std::make_unique<EndstonePluginManager>(*this);
     plugin_manager_->registerLoader(std::make_unique<CppPluginLoader>(*this));
 }
 
+std::string EndstoneServer::getName() const
+{
+    return "Endstone";
+}
+
+std::string EndstoneServer::getVersion() const
+{
+    return ENDSTONE_VERSION;
+}
+
+std::string EndstoneServer::getMinecraftVersion() const
+{
+    return Common::getGameVersionString();
+}
+
+Logger &EndstoneServer::getLogger() const
+{
+    return logger_;
+}
+
+EndstoneCommandMap &EndstoneServer::getCommandMap() const
+{
+    return *command_map_;
+}
+
+MinecraftCommands &EndstoneServer::getMinecraftCommands()
+{
+    return server_instance_.getMinecraft().getCommands();
+}
+
+PluginManager &EndstoneServer::getPluginManager() const
+{
+    return *plugin_manager_;
+}
+
+PluginCommand *EndstoneServer::getPluginCommand(std::string name) const
+{
+    if (auto *command = command_map_->getCommand(name)) {
+        return command->asPluginCommand();
+    }
+    return nullptr;
+}
+
+CommandSender &EndstoneServer::getCommandSender() const
+{
+    return command_sender_;
+}
+
 void EndstoneServer::loadPlugins()
 {
     auto plugin_dir = fs::current_path() / "plugins";
 
     if (exists(plugin_dir)) {
         plugin_manager_->loadPlugins(plugin_dir.string());
     }
@@ -85,47 +134,14 @@
 }
 
 void EndstoneServer::disablePlugins() const
 {
     plugin_manager_->disablePlugins();
 }
 
-Logger &EndstoneServer::getLogger() const
-{
-    return logger_;
-}
-
-EndstoneCommandMap &EndstoneServer::getCommandMap() const
-{
-    return *command_map_;
-}
-
-MinecraftCommands &EndstoneServer::getMinecraftCommands()
-{
-    return server_instance_.getMinecraft().getCommands();
-}
-
-PluginManager &EndstoneServer::getPluginManager() const
-{
-    return *plugin_manager_;
-}
-
-PluginCommand *EndstoneServer::getPluginCommand(std::string name) const
-{
-    if (auto *command = command_map_->getCommand(name)) {
-        return command->asPluginCommand();
-    }
-    return nullptr;
-}
-
-CommandSender &EndstoneServer::getCommandSender() const
-{
-    return command_sender_;
-}
-
 std::vector<Level *> EndstoneServer::getLevels() const
 {
     std::vector<Level *> levels;
     levels.reserve(levels_.size());
     for (const auto &it : levels_) {
         levels.push_back(it.second.get());
     }
@@ -152,36 +168,48 @@
     std::transform(name.begin(), name.end(), name.begin(), [](unsigned char c) { return std::tolower(c); });
     levels_[name] = std::move(level);
 }
 
 Player *EndstoneServer::getPlayer(endstone::UUID id) const
 {
     for (const auto *level : getLevels()) {
-        auto uuid = mce::UUID{id.bits.most_significant, id.bits.least_significant};
+        auto uuid = mce::UUID::fromEndstone(id);
         auto *player = static_cast<const EndstoneLevel *>(level)->getBedrockLevel().getPlayer(uuid);
         if (player) {
             return &player->getEndstonePlayer();
         }
     }
     return nullptr;
 }
 
-std::string EndstoneServer::getName() const
+void EndstoneServer::broadcast(const std::string &message, const std::string &permission) const
 {
-    return "Endstone";
-}
+    std::unordered_set<const CommandSender *> recipients;
+    for (const auto *permissible : getPluginManager().getPermissionSubscriptions(permission)) {
+        const auto *sender = permissible->asCommandSender();
+        if (sender != nullptr && sender->hasPermission(permission)) {
+            recipients.insert(sender);
+        }
+    }
 
-std::string EndstoneServer::getVersion() const
-{
-    return ENDSTONE_VERSION;
+    BroadcastMessageEvent event{!isPrimaryThread(), message, recipients};
+    getPluginManager().callEvent(event);
+
+    if (event.isCancelled()) {
+        return;
+    }
+
+    for (const auto &recipient : recipients) {
+        recipient->sendMessage(event.getMessage());
+    }
 }
 
-std::string EndstoneServer::getMinecraftVersion() const
+void EndstoneServer::broadcastMessage(const std::string &message) const
 {
-    return Common::getGameVersionString();
+    broadcast(message, "endstone.broadcast.user");
 }
 
 bool EndstoneServer::isPrimaryThread() const
 {
     return Bedrock::Threading::getServerThread().isOnThread();
 }
```

### Comparing `endstone-0.4.0/src/endstone_core/spdlog/level_formatter.cpp` & `endstone-0.4.1/src/endstone_core/spdlog/level_formatter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/spdlog/log_sink.cpp` & `endstone-0.4.1/src/endstone_core/spdlog/log_sink.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/spdlog/spdlog_adapter.cpp` & `endstone-0.4.1/src/endstone_core/spdlog/spdlog_adapter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_core/spdlog/text_formatter.cpp` & `endstone-0.4.1/src/endstone_core/spdlog/text_formatter.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/actor.cpp` & `endstone-0.4.1/src/endstone_python/actor.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/command.cpp` & `endstone-0.4.1/src/endstone_python/command.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/endstone_python.cpp` & `endstone-0.4.1/src/endstone_python/endstone_python.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/event.cpp` & `endstone-0.4.1/src/endstone_python/event.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "endstone/event/event.h"
 
 #include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
 
 #include "endstone/event/actor/actor_remove_event.h"
 #include "endstone/event/actor/actor_spawn_event.h"
 #include "endstone/event/event_priority.h"
 #include "endstone/event/player/player_chat_event.h"
+#include "endstone/event/player/player_command_event.h"
 #include "endstone/event/player/player_join_event.h"
 #include "endstone/event/player/player_quit_event.h"
+#include "endstone/event/server/broadcast_message_event.h"
 #include "endstone/event/server/plugin_disable_event.h"
 #include "endstone/event/server/plugin_enable_event.h"
 #include "endstone/event/server/server_command_event.h"
 #include "endstone/event/server/server_list_ping_event.h"
 #include "endstone/event/server/server_load_event.h"
 #include "endstone/event/weather/thunder_change_event.h"
 #include "endstone/event/weather/weather_change_event.h"
@@ -70,26 +73,39 @@
 
     py::class_<ActorSpawnEvent, Event>(m, "ActorSpawnEvent")
         .def_property_readonly("actor", &ActorSpawnEvent::getActor, py::return_value_policy::reference,
                                "Returns the Actor being spawned");
 
     py::class_<PlayerChatEvent, Event>(m, "PlayerChatEvent")
         .def_property_readonly("player", &PlayerChatEvent::getPlayer, py::return_value_policy::reference,
-                               "Returns the Player who joins the server")
+                               "Returns the Player who sends the message")
         .def_property("message", &PlayerChatEvent::getMessage, &PlayerChatEvent::setMessage,
                       "The message that the player will send.");
 
+    py::class_<PlayerCommandEvent, Event>(m, "PlayerCommandEvent")
+        .def_property_readonly("player", &PlayerCommandEvent::getPlayer, py::return_value_policy::reference,
+                               "Returns the Player who sends the command")
+        .def_property("command", &PlayerCommandEvent::getCommand, &PlayerCommandEvent::setCommand,
+                      "The command that the player will send.");
+
     py::class_<PlayerJoinEvent, Event>(m, "PlayerJoinEvent")
         .def_property_readonly("player", &PlayerJoinEvent::getPlayer, py::return_value_policy::reference,
                                "Returns the Player who joins the server");
 
     py::class_<PlayerQuitEvent, Event>(m, "PlayerQuitEvent")
         .def_property_readonly("player", &PlayerQuitEvent::getPlayer, py::return_value_policy::reference,
                                "Returns the Player who leaves the server");
 
+    py::class_<BroadcastMessageEvent, Event>(m, "BroadcastMessageEvent")
+        .def_property("message", &BroadcastMessageEvent::getMessage, &BroadcastMessageEvent::setMessage,
+                      "The message to broadcast.")
+        .def_property_readonly("recipients", &BroadcastMessageEvent::getRecipients,
+                               py::return_value_policy::reference_internal,
+                               "Gets a set of recipients that this broadcast message will be displayed to.");
+
     py::class_<PluginEnableEvent, Event>(m, "PluginEnableEvent")
         .def_property_readonly("plugin", &PluginEnableEvent::getPlugin, py::return_value_policy::reference);
 
     py::class_<PluginDisableEvent, Event>(m, "PluginDisableEvent")
         .def_property_readonly("plugin", &PluginDisableEvent::getPlugin, py::return_value_policy::reference);
 
     py::class_<ServerCommandEvent, Event>(m, "ServerCommandEvent")
```

### Comparing `endstone-0.4.0/src/endstone_python/permissions.cpp` & `endstone-0.4.1/src/endstone_python/permissions.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/plugin.cpp` & `endstone-0.4.1/src/endstone_python/plugin.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_python/util.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/i18n.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include <pybind11/pybind11.h>
+#include "bedrock/i18n.h"
 
-namespace py = pybind11;
+#include "endstone/detail/hook.h"
 
-namespace endstone::detail {
-
-void init_util(py::module &m) {}
-
-}  // namespace endstone::detail
+I18n &getI18n()
+{
+    return ENDSTONE_HOOK_CALL_ORIGINAL(&getI18n);
+}
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/bedrock_log.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/bedrock_log.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/command/command.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/command/command_utils.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/command/command.h"
+#include "bedrock/command/command_utils.h"
 
 #include "endstone/detail/hook.h"
 
-std::string Command::getCommandName() const
+std::string CommandUtils::getActorName(const Actor &actor)
 {
     std::string result;
-    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&Command::getCommandName, result, this);
+    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&CommandUtils::getActorName, result, actor);
     return result;
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/command/command_output.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/command/command_output.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/command/command_registry.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/command/command_registry.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/command/command_utils.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/threading.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/command/command_utils.h"
+#include "bedrock/threading.h"
 
 #include "endstone/detail/hook.h"
 
-std::string CommandUtils::getActorName(const Actor &actor)
+namespace Bedrock::Threading {
+
+AssignedThread &getServerThread()
 {
-    std::string result;
-    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&CommandUtils::getActorName, result, actor);
-    return result;
+    return ENDSTONE_HOOK_CALL_ORIGINAL(&getServerThread);
 }
+
+}  // namespace Bedrock::Threading
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/command/minecraft_commands.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/server/network/server_network_handler.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -8,45 +8,40 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/command/minecraft_commands.h"
+#include "bedrock/server/network/server_network_handler.h"
 
 #include <entt/entt.hpp>
 
 #include "endstone/detail/hook.h"
 #include "endstone/detail/server.h"
-#include "endstone/event/server/server_command_event.h"
+#include "endstone/event/player/player_chat_event.h"
 
 using endstone::detail::EndstoneServer;
 
-MCRESULT MinecraftCommands::executeCommand(CommandContext &ctx, bool flag) const
+bool ServerNetworkHandler::_loadNewPlayer(ServerPlayer &server_player, bool flag)
 {
-    MCRESULT result;
-    if (ctx.getOrigin().getOriginType() != CommandOriginType::DedicatedServer) {
-#ifdef _WIN32
-        ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&MinecraftCommands::executeCommand, result, this, ctx, flag);
-#else
-        result = ENDSTONE_HOOK_CALL_ORIGINAL(&MinecraftCommands::executeCommand, this, ctx, flag);
-#endif
-        return result;
-    }
+    auto &server = entt::locator<EndstoneServer>::value();
+    auto &endstone_player = server_player.getEndstonePlayer();
+    // TODO(event): call PlayerLoginEvent
+    return ENDSTONE_HOOK_CALL_ORIGINAL(&ServerNetworkHandler::_loadNewPlayer, this, server_player, flag);
+}
 
+void ServerNetworkHandler::_displayGameMessage(const Player &player, ChatEvent &event)
+{
     auto &server = entt::locator<EndstoneServer>::value();
-    endstone::ServerCommandEvent event(server.getCommandSender(), ctx.getCommandLine());
-    server.getPluginManager().callEvent(event);
+    endstone::PlayerChatEvent e{player.getEndstonePlayer(), event.message};
+    server.getPluginManager().callEvent(e);
 
-    if (event.isCancelled()) {
-        result = MCRESULT_CommandsDisabled;
+    if (e.isCancelled()) {
+        return;
     }
-    else {
-#ifdef _WIN32
-        ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&MinecraftCommands::executeCommand, result, this, ctx, flag);
-#else
-        result = ENDSTONE_HOOK_CALL_ORIGINAL(&MinecraftCommands::executeCommand, this, ctx, flag);
-#endif
-    }
-    return result;
+
+    event.message = std::move(e.getMessage());
+    server.getLogger().info("<{}> {}", e.getPlayer().getName(), e.getMessage());
+
+    ENDSTONE_HOOK_CALL_ORIGINAL(&ServerNetworkHandler::_displayGameMessage, this, player, event);
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/common.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/common.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/i18n.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/level/dimension/vanilla_dimensions.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/i18n.h"
+#include "bedrock/world/level/dimension/vanilla_dimensions.h"
 
 #include "endstone/detail/hook.h"
 
-std::string I18n::get(const std::string &message_id, const std::vector<std::string> &params,
-                      const Localization *localization)
+std::string const VanillaDimensions::toString(const AutomaticID<Dimension, int> &dimension_id)
 {
     std::string result;
-    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&I18n::get, result, message_id, params, localization);
+    ENDSTONE_HOOK_CALL_ORIGINAL_RVO(&VanillaDimensions::toString, result, dimension_id);
     return result;
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/minecraft.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/server/server_instance.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/minecraft.h"
+#include "bedrock/server/server_instance.h"
 
 #include "endstone/endstone.h"
 
-MinecraftCommands &Minecraft::getCommands()
+Minecraft &ServerInstance::getMinecraft()
 {
-    return **reinterpret_cast<MinecraftCommands **>(reinterpret_cast<std::size_t *>(this) + _WIN32_LINUX_(23, 22));
+    return **reinterpret_cast<Minecraft **>(reinterpret_cast<std::size_t *>(this) + _WIN32_LINUX_(21, 16));
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/network/protocol/minecraft_packets.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/network/protocol/minecraft_packets.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/socket2.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/network/raknet/socket2.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/network/raknet/types.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/network/raknet/types.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_level.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/server/level/server_level.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/server/level/server_player.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/server/level/server_player.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 
 void ServerPlayer::doInitialSpawn()
 {
     ENDSTONE_HOOK_CALL_ORIGINAL(&ServerPlayer::doInitialSpawn, this);
     auto &server = entt::locator<EndstoneServer>::value();
     endstone::PlayerJoinEvent e{getEndstonePlayer()};
     server.getPluginManager().callEvent(e);
+    getEndstonePlayer().recalculatePermissions();
     sendCommands();
 }
 
 void ServerPlayer::disconnect()
 {
+    getEndstonePlayer().disconnect();
     auto &server = entt::locator<EndstoneServer>::value();
     endstone::PlayerQuitEvent e{getEndstonePlayer()};
     server.getPluginManager().callEvent(e);
     ENDSTONE_HOOK_CALL_ORIGINAL(&ServerPlayer::disconnect, this);
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/server/server_instance.cpp` & `endstone-0.4.1/src/endstone_core/scheduler/scheduler.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/server/server_instance.h"
+#include "endstone/detail/scheduler/scheduler.h"
 
-#include "endstone/endstone.h"
+namespace endstone::detail {
 
-Minecraft &ServerInstance::getMinecraft()
+TaskId EndstoneScheduler::incrementIds()
 {
-    return **reinterpret_cast<Minecraft **>(reinterpret_cast<std::size_t *>(this) + _WIN32_LINUX_(21, 16));
+    if (ids_ >= std::numeric_limits<std::uint32_t>::max()) {
+        ids_ = 1;
+    }
+    return ids_++;
 }
+
+}  // namespace endstone::detail
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/threading.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/server/command/say_command.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
-#include "bedrock/threading.h"
+#include "bedrock/server/command/say_command.h"
 
+#include <entt/entt.hpp>
+
+#include "bedrock/i18n.h"
 #include "endstone/detail/hook.h"
+#include "endstone/detail/server.h"
 
-namespace Bedrock::Threading {
+using endstone::detail::EndstoneServer;
 
-AssignedThread &getServerThread()
+void SayCommand::_sendMessage(const std::string &message, const std::string &sender_name,
+                              const CommandOriginIdentity &origin_identity, Level &level)
 {
-    return ENDSTONE_HOOK_CALL_ORIGINAL(&getServerThread);
+    ENDSTONE_HOOK_CALL_ORIGINAL(&SayCommand::_sendMessage, message, sender_name, origin_identity, level);
+    auto &server = entt::locator<EndstoneServer>::value();
+    server.getLogger().info(getI18n().get("chat.type.announcement", {sender_name, message}, nullptr));
 }
-
-}  // namespace Bedrock::Threading
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/actor.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/actor/actor.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 
 #include "bedrock/world/actor/actor.h"
 
 #include "bedrock/world/actor/components/actor_owner_component.h"
+#include "bedrock/world/actor/components/flag_component.h"
 #include "bedrock/world/actor/components/runtime_id_component.h"
 #include "bedrock/world/actor/player/player.h"
 #include "endstone/detail/actor/actor.h"
 #include "endstone/detail/hook.h"
 #include "endstone/detail/player.h"
 #include "endstone/detail/server.h"
 #include "endstone/event/actor/actor_remove_event.h"
@@ -42,14 +43,19 @@
 
 void Actor::setDimension(WeakRef<Dimension> dimension)
 {
     // TODO(event): call PlayerChangedLevelEvent for player??
     ENDSTONE_HOOK_CALL_ORIGINAL(&Actor::setDimension, this, std::move(dimension));
 }
 
+bool Actor::isPlayer() const
+{
+    return hasComponent<FlagComponent<PlayerComponentFlag>>();
+}
+
 bool Actor::isRemoved() const
 {
     return !isAlive();
 }
 
 Dimension &Actor::getDimension() const
 {
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/world/actor/player/player.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/actor/player/player.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #include "endstone/detail/server.h"
 
 using endstone::detail::EndstoneServer;
 
 void Player::setPermissions(CommandPermissionLevel level)
 {
     ENDSTONE_HOOK_CALL_ORIGINAL(&Player::setPermissions, this, level);
+    getEndstonePlayer().recalculatePermissions();
     sendCommands();
 }
 
 const std::string &Player::getName() const
 {
     return ENDSTONE_HOOK_CALL_ORIGINAL(&Player::getName, this);
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/world/level/dimension/dimension.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/level/dimension/dimension.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/event_coordinator.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/level/event/event_coordinator.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -122,28 +122,29 @@
     };
     std::visit(visitor, ref.reference.event);
     return ENDSTONE_HOOK_CALL_ORIGINAL(fp, this, ref);
 }
 
 void ServerInstanceEventCoordinator::sendServerInitializeStart(ServerInstance &instance)
 {
+    endstone::detail::register_signal_handler();
     auto &server = entt::locator<EndstoneServer>::value_or(instance);
     server.getPluginManager().registerLoader(std::make_unique<PythonPluginLoader>(server));
+    server.getCommandSender().recalculatePermissions();
     server.getLogger().info(ColorFormat::DarkAqua + ColorFormat::Bold +
                                 "This server is running {} version: {} (Minecraft: {})",
                             server.getName(), server.getVersion(), server.getMinecraftVersion());
 
     server.loadPlugins();
     server.enablePlugins(PluginLoadOrder::Startup);
     ENDSTONE_HOOK_CALL_ORIGINAL(&ServerInstanceEventCoordinator::sendServerInitializeStart, this, instance);
 }
 
 void ServerInstanceEventCoordinator::sendServerThreadStarted(ServerInstance &instance)
 {
-    endstone::detail::register_signal_handler();
     auto &server = entt::locator<EndstoneServer>::value();
     server.enablePlugins(PluginLoadOrder::PostWorld);
     ServerLoadEvent event{ServerLoadEvent::LoadType::Startup};
     server.getPluginManager().callEvent(event);
     ENDSTONE_HOOK_CALL_ORIGINAL(&ServerInstanceEventCoordinator::sendServerThreadStarted, this, instance);
 }
```

### Comparing `endstone-0.4.0/src/endstone_runtime/bedrock/world/level/event/gameplay_handler.cpp` & `endstone-0.4.1/src/endstone_runtime/bedrock/world/level/event/gameplay_handler.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/hook.cpp` & `endstone-0.4.1/src/endstone_runtime/hook.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/linux/hook.cpp` & `endstone-0.4.1/src/endstone_runtime/linux/hook.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/linux/os.cpp` & `endstone-0.4.1/src/endstone_runtime/linux/os.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/linux/signal_handler.cpp` & `endstone-0.4.1/src/endstone_runtime/linux/signal_handler.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/magic.cpp` & `endstone-0.4.1/src/endstone_runtime/magic.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/main.cpp` & `endstone-0.4.1/src/endstone_runtime/main.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/plugin/python_plugin_loader.cpp` & `endstone-0.4.1/src/endstone_runtime/plugin/python_plugin_loader.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/windows/hook.cpp` & `endstone-0.4.1/src/endstone_runtime/windows/hook.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/windows/os.cpp` & `endstone-0.4.1/src/endstone_runtime/windows/os.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/src/endstone_runtime/windows/signal_handler.cpp` & `endstone-0.4.1/src/endstone_runtime/windows/signal_handler.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/tests/command/test_command_lexer.cpp` & `endstone-0.4.1/tests/command/test_command_lexer.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/tests/command/test_command_usage_parser.cpp` & `endstone-0.4.1/tests/command/test_command_usage_parser.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/tests/plugin/test_cpp_plugin_loader.cpp` & `endstone-0.4.1/tests/plugin/test_cpp_plugin_loader.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 #include "endstone/detail/plugin/cpp_plugin_loader.h"
 #include "endstone/server.h"
 
 namespace fs = std::filesystem;
 
 class MockServer : public endstone::Server {
 public:
+    MOCK_METHOD(std::string, getName, (), (const, override));
+    MOCK_METHOD(std::string, getVersion, (), (const, override));
+    MOCK_METHOD(std::string, getMinecraftVersion, (), (const, override));
     MOCK_METHOD(endstone::Logger &, getLogger, (), (const, override));
     MOCK_METHOD(endstone::PluginManager &, getPluginManager, (), (const, override));
     MOCK_METHOD(endstone::PluginCommand *, getPluginCommand, (std::string name), (const, override));
     MOCK_METHOD(endstone::CommandSender &, getCommandSender, (), (const, override));
     MOCK_METHOD(std::vector<endstone::Level *>, getLevels, (), (const, override));
     MOCK_METHOD(endstone::Level *, getLevel, (std::string name), (const, override));
     MOCK_METHOD(endstone::Player *, getPlayer, (endstone::UUID id), (const, override));
-    MOCK_METHOD(std::string, getName, (), (const, override));
-    MOCK_METHOD(std::string, getVersion, (), (const, override));
-    MOCK_METHOD(std::string, getMinecraftVersion, (), (const, override));
+    MOCK_METHOD(void, broadcast, (const std::string &, const std::string &), (const, override));
+    MOCK_METHOD(void, broadcastMessage, (const std::string &), (const, override));
     MOCK_METHOD(bool, isPrimaryThread, (), (const, override));
     MockServer()
     {
         ON_CALL(*this, getLogger())
             .WillByDefault(testing::ReturnRef(endstone::detail::LoggerFactory::getLogger("Test")));
     }
 };
```

### Comparing `endstone-0.4.0/tests/plugin/test_plugin.cpp` & `endstone-0.4.1/tests/plugin/test_plugin.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/tests/test_logger_factory.cpp` & `endstone-0.4.1/tests/test_logger_factory.cpp`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/.gitignore` & `endstone-0.4.1/third_party/.gitignore`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/conanfile.py` & `endstone-0.4.1/third_party/funchook/conanfile.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch` & `endstone-0.4.1/third_party/funchook/patches/1.1.3-0001-cmake-use-cci-capstone.patch`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/CMakeLists.txt` & `endstone-0.4.1/third_party/funchook/test_package/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/conanfile.py` & `endstone-0.4.1/third_party/funchook/test_package/conanfile.py`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S` & `endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_aarch64_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S` & `endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_64_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/libfunchook_test_x86_gas.S` & `endstone-0.4.1/third_party/funchook/test_package/libfunchook_test_x86_gas.S`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/suffix.list` & `endstone-0.4.1/third_party/funchook/test_package/suffix.list`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/test_main.c` & `endstone-0.4.1/third_party/funchook/test_package/test_main.c`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/third_party/funchook/test_package/x86_test.S` & `endstone-0.4.1/third_party/funchook/test_package/x86_test.S`

 * *Files identical despite different names*

### Comparing `endstone-0.4.0/PKG-INFO` & `endstone-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endstone
-Version: 0.4.0
+Version: 0.4.1
 Summary: Endstone offers a plugin API for Bedrock Dedicated Servers, supporting both Python and C++.
 Keywords: plugin,python,minecraft,bedrock
 Author-Email: Vincent Wu <magicdroidx@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -242,15 +242,15 @@
 </p>
 
 [![Windows](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/windows.yml)
 [![Linux](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/linux.yml)
 [![Wheel](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/wheel.yml)
 [![Docker](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml/badge.svg)](https://github.com/EndstoneMC/endstone/actions/workflows/docker.yml)
 [![Documentation](https://img.shields.io/readthedocs/endstone)](https://endstone.readthedocs.io/)
-[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.73%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
+[![Minecraft - Version](https://img.shields.io/badge/minecraft-v1.20.80%20(Bedrock)-green)](https://feedback.minecraft.net/hc/en-us/sections/360001186971-Release-Changelogs)
 [![PyPI - Version](https://img.shields.io/pypi/v/endstone)](https://pypi.org/project/endstone)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/endstone)](https://pypi.org/project/endstone)
 [![Python](https://img.shields.io/badge/Python-3-blue?logo=python&logoColor=white)](https://www.python.org/)
 [![GitHub License](https://img.shields.io/github/license/endstonemc/endstone)](LICENSE)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8877402fc70b40f5a8c4b325d890e3f7?logo=codacy)](https://app.codacy.com/gh/EndstoneMC/endstone/dashboard)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -308,30 +308,33 @@
 ```shell
 pip install endstone
 endstone
 ```
 
 ### 🐳 Docker
 
-To try Endstone from a Docker image, use the following command:
+To try Endstone from the latest Docker image, use the following command:
 
 ```shell
 docker pull endstone/endstone
 docker run --rm -it -p 19132:19132/udp endstone/endstone
 ```
 
-or
+This will pull the latest Endstone image and run it interactively in your terminal.
+
+### 🕋 Docker Compose
+
+You can also use Docker Compose to run Endstone in a production environment.
 
 ```shell
-docker pull ghcr.io/endstonemc/endstone
-docker run --rm -it -p 19132:19132/udp ghcr.io/endstonemc/endstone
+docker compose build
+docker compose up -d
+docker attach endstone
 ```
 
-This will pull the latest Endstone image and run it interactively in your terminal.
-
 ### 🔨 Build locally from Source
 
 For advanced users, you may build Endstone locally from the source.
 
 **Please note that building from source requires toolchains to be installed on your system.**
 
 |                                  | Windows                       | Linux    |
@@ -380,15 +383,15 @@
 - [Python Example Plugin](https://github.com/EndstoneMC/python-plugin-template)
 
 | Milestone                                | Duration   | Core | C++ API | Python API | Since  |
 |------------------------------------------|------------|------|---------|------------|--------|
 | **🔌 Plugin Loader**                     | 1-2 months | ✅    | ✅       | ✅          | v0.1.0 |
 | **⌨️ Command System**                    | 2-3 months | ✅    | ✅       | ✅          | v0.2.0 |
 | **🔐 Permission System**                 | 2-3 months | ✅    | ✅       | ✅          | v0.3.0 |
-| **🎈 Event System**                      | 2-3 months | 🚧   | ✅       | ✅          |        |
+| **🎈 Event System**                      | 2-3 months | ✅    | ✅       | ✅          | v0.4.0 |
 | **🛠 Minecraft Core Features**           | 4-5 months | ⏳    | ⏳       | ⏳          |        |
 | **🖼 GUI & Inventory System**            | 3-4 months | ⏳    | ⏳       | ⏳          |        |
 | **🌟 Advanced Features & Refinements**   | 4-6 months | ⏳    | ⏳       | ⏳          |        |
 | **🧪 Beta Testing & Community Feedback** | 3 months   | ⏳    | ⏳       | ⏳          |        |
 | **🚀 Official Release & Support**        | -          | ⏳    | ⏳       | ⏳          |        |
 
 Here's a legend to guide you:
```

