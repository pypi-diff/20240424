# Comparing `tmp/sbin-1.0.1.tar.gz` & `tmp/sbin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbin-1.0.1.tar", max compression
+gzip compressed data, was "sbin-1.1.0.tar", max compression
```

## Comparing `sbin-1.0.1.tar` & `sbin-1.1.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1069 2022-09-01 19:17:31.002476 sbin-1.0.1/LICENSE
--rw-r--r--   0        0        0     1178 2022-11-02 16:49:07.027442 sbin-1.0.1/README.md
--rw-r--r--   0        0        0        0 2022-09-06 21:19:19.528859 sbin-1.0.1/bin/__init__.py
--rw-r--r--   0        0        0      765 2022-10-23 17:19:59.121539 sbin-1.0.1/bin/bin.py
--rw-r--r--   0        0        0        0 2022-09-22 01:28:44.998725 sbin-1.0.1/bin/bin_file/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-22 01:14:21.269990 sbin-1.0.1/bin/bin_file/bin_file_loader.py
--rw-r--r--   0        0        0      326 2022-09-22 01:28:44.999953 sbin-1.0.1/bin/bin_file/bin_file_resolver.py
--rw-r--r--   0        0        0        0 2022-10-18 02:20:16.831457 sbin-1.0.1/bin/bin_file/dtos/__init__.py
--rw-r--r--   0        0        0      610 2024-03-22 00:50:10.122484 sbin-1.0.1/bin/bin_file/dtos/base_bin_file_dto.py
--rw-r--r--   0        0        0     9888 2024-03-22 01:14:21.270385 sbin-1.0.1/bin/bin_file/dtos/bin_file_dto.py
--rw-r--r--   0        0        0     1448 2022-10-22 21:43:35.855691 sbin-1.0.1/bin/bin_file/dtos/bin_file_mapper.py
--rw-r--r--   0        0        0      234 2022-10-10 03:49:42.842428 sbin-1.0.1/bin/bin_file/errors.py
--rw-r--r--   0        0        0     1779 2024-03-22 01:14:21.270713 sbin-1.0.1/bin/bin_file/init_command.py
--rw-r--r--   0        0        0        0 2022-09-10 18:49:43.443509 sbin-1.0.1/bin/commands/__init__.py
--rw-r--r--   0        0        0     1023 2022-11-03 03:28:30.109329 sbin-1.0.1/bin/commands/command.py
--rw-r--r--   0        0        0     3067 2024-03-22 01:14:21.271120 sbin-1.0.1/bin/commands/command_help.py
--rw-r--r--   0        0        0      779 2022-10-14 21:47:15.787742 sbin-1.0.1/bin/commands/errors.py
--rw-r--r--   0        0        0        0 2022-10-22 21:58:51.166687 sbin-1.0.1/bin/commands/internal/__init__.py
--rw-r--r--   0        0        0      627 2022-10-29 20:44:28.695838 sbin-1.0.1/bin/commands/internal/apply_env_command.py
--rw-r--r--   0        0        0     1344 2022-10-23 17:19:59.122226 sbin-1.0.1/bin/commands/internal/factory.py
--rw-r--r--   0        0        0      587 2022-10-22 21:58:51.167258 sbin-1.0.1/bin/commands/internal/help_only_command.py
--rw-r--r--   0        0        0     1804 2024-03-22 00:50:10.123112 sbin-1.0.1/bin/commands/internal/log_title_command.py
--rw-r--r--   0        0        0      567 2022-10-22 21:58:51.167956 sbin-1.0.1/bin/commands/internal/mute_logs_command.py
--rw-r--r--   0        0        0      561 2022-10-22 21:58:51.168197 sbin-1.0.1/bin/commands/internal/noop_command.py
--rw-r--r--   0        0        0      571 2022-10-22 21:58:51.168453 sbin-1.0.1/bin/commands/internal/unmute_logs_command.py
--rw-r--r--   0        0        0      682 2022-10-22 21:58:51.168716 sbin-1.0.1/bin/commands/internal/with_setup_command.py
--rw-r--r--   0        0        0        0 2022-10-22 21:51:18.183468 sbin-1.0.1/bin/custom_commands/__init__.py
--rw-r--r--   0        0        0     1116 2024-03-22 01:14:21.271468 sbin-1.0.1/bin/custom_commands/basic_command.py
--rw-r--r--   0        0        0     1971 2024-03-22 00:50:10.126259 sbin-1.0.1/bin/custom_commands/command_tree.py
--rw-r--r--   0        0        0      256 2022-10-22 21:51:18.184303 sbin-1.0.1/bin/custom_commands/dtos/__init__.py
--rw-r--r--   0        0        0      217 2022-10-22 21:51:18.184510 sbin-1.0.1/bin/custom_commands/dtos/base_custom_command_dto.py
--rw-r--r--   0        0        0     3486 2024-03-22 00:50:10.124688 sbin-1.0.1/bin/custom_commands/dtos/command_tree_dto.py
--rw-r--r--   0        0        0      659 2024-03-22 00:50:10.122709 sbin-1.0.1/bin/custom_commands/dtos/custom_commands_mapper.py
--rw-r--r--   0        0        0      579 2022-10-22 21:51:18.185265 sbin-1.0.1/bin/custom_commands/dtos/str_custom_command_dto.py
--rw-r--r--   0        0        0        0 2022-10-29 19:47:58.643745 sbin-1.0.1/bin/env/__init__.py
--rw-r--r--   0        0        0     1574 2024-03-22 00:50:10.124493 sbin-1.0.1/bin/env/ejson_env_provider.py
--rw-r--r--   0        0        0     1316 2024-03-22 01:14:21.271813 sbin-1.0.1/bin/env/env.py
--rw-r--r--   0        0        0     1036 2022-10-29 19:47:58.644544 sbin-1.0.1/bin/env/env_provider.py
--rw-r--r--   0        0        0      569 2022-10-29 19:47:58.644773 sbin-1.0.1/bin/env/env_providers.py
--rw-r--r--   0        0        0      108 2022-10-29 20:44:28.696874 sbin-1.0.1/bin/env/errors.py
--rw-r--r--   0        0        0     1236 2022-10-29 19:47:58.645008 sbin-1.0.1/bin/env/log_env_command.py
--rw-r--r--   0        0        0     2771 2024-03-22 00:50:10.124933 sbin-1.0.1/bin/error_handler.py
--rw-r--r--   0        0        0     1574 2024-03-22 00:50:10.122323 sbin-1.0.1/bin/main.py
--rw-r--r--   0        0        0        0 2022-09-17 20:12:34.944472 sbin-1.0.1/bin/models/__init__.py
--rw-r--r--   0        0        0      508 2024-03-22 01:22:52.108572 sbin-1.0.1/bin/models/bin_base_model.py
--rw-r--r--   0        0        0      916 2022-11-01 01:20:00.070402 sbin-1.0.1/bin/models/sem_ver_spec.py
--rw-r--r--   0        0        0      719 2022-11-02 17:35:06.612268 sbin-1.0.1/bin/models/str_command.py
--rw-r--r--   0        0        0        0 2022-09-17 15:05:40.066825 sbin-1.0.1/bin/process/__init__.py
--rw-r--r--   0        0        0      220 2022-11-02 00:37:59.195290 sbin-1.0.1/bin/process/emoji.py
--rw-r--r--   0        0        0      124 2022-10-06 14:16:07.963680 sbin-1.0.1/bin/process/helpable.py
--rw-r--r--   0        0        0        0 2022-10-20 16:48:15.443020 sbin-1.0.1/bin/process/io/__init__.py
--rw-r--r--   0        0        0      707 2022-10-20 16:48:15.443346 sbin-1.0.1/bin/process/io/console_io.py
--rw-r--r--   0        0        0      439 2022-10-20 16:48:15.443578 sbin-1.0.1/bin/process/io/io.py
--rw-r--r--   0        0        0      340 2022-10-20 16:48:15.443828 sbin-1.0.1/bin/process/io/mute_io.py
--rw-r--r--   0        0        0     2513 2024-03-22 01:14:21.272158 sbin-1.0.1/bin/process/process.py
--rw-r--r--   0        0        0      274 2022-09-17 15:05:40.067634 sbin-1.0.1/bin/process/process_result.py
--rw-r--r--   0        0        0        0 2022-09-09 18:19:23.466612 sbin-1.0.1/bin/requirements/__init__.py
--rw-r--r--   0        0        0      348 2022-09-18 17:05:56.574363 sbin-1.0.1/bin/requirements/dtos/__init__.py
--rw-r--r--   0        0        0      184 2022-09-17 20:12:34.945759 sbin-1.0.1/bin/requirements/dtos/base_requirement_dto.py
--rw-r--r--   0        0        0      655 2022-09-17 20:12:34.945990 sbin-1.0.1/bin/requirements/dtos/python_requirement_dto.py
--rw-r--r--   0        0        0      381 2022-10-11 22:35:07.274551 sbin-1.0.1/bin/requirements/dtos/requirements_command_mapper.py
--rw-r--r--   0        0        0      664 2024-03-22 00:50:10.121358 sbin-1.0.1/bin/requirements/dtos/sem_ver_requirement_dto.py
--rw-r--r--   0        0        0      575 2022-09-17 20:12:34.946453 sbin-1.0.1/bin/requirements/dtos/shell_requirement_dto.py
--rw-r--r--   0        0        0      343 2022-09-17 15:05:40.067971 sbin-1.0.1/bin/requirements/requirement.py
--rw-r--r--   0        0        0     1865 2024-03-22 00:50:10.123238 sbin-1.0.1/bin/requirements/requirements_command.py
--rw-r--r--   0        0        0      907 2022-10-21 01:40:07.814478 sbin-1.0.1/bin/requirements/sem_ver_requirement.py
--rw-r--r--   0        0        0      591 2022-11-02 19:27:25.649862 sbin-1.0.1/bin/requirements/shell_requirement.py
--rw-r--r--   0        0        0        0 2022-09-13 22:17:57.860791 sbin-1.0.1/bin/up/__init__.py
--rw-r--r--   0        0        0      952 2024-03-22 00:50:10.123677 sbin-1.0.1/bin/up/conditional_up_subcommand.py
--rw-r--r--   0        0        0      419 2022-10-12 13:43:27.700922 sbin-1.0.1/bin/up/down_command.py
--rw-r--r--   0        0        0      245 2022-10-06 14:16:07.965026 sbin-1.0.1/bin/up/dtos/__init__.py
--rw-r--r--   0        0        0      317 2022-10-06 14:16:07.965342 sbin-1.0.1/bin/up/dtos/base_up_subcommand_dto.py
--rw-r--r--   0        0        0     2085 2024-03-22 01:14:21.272507 sbin-1.0.1/bin/up/dtos/conditional_up_subcommand_dto.py
--rw-r--r--   0        0        0      648 2022-10-06 14:16:07.965991 sbin-1.0.1/bin/up/dtos/str_up_subcommand_dto.py
--rw-r--r--   0        0        0      664 2022-10-12 13:43:27.701243 sbin-1.0.1/bin/up/dtos/up_command_mapper.py
--rw-r--r--   0        0        0      444 2022-09-17 20:12:34.949662 sbin-1.0.1/bin/up/simple_up_subcommand.py
--rw-r--r--   0        0        0     2234 2024-03-22 00:50:10.126124 sbin-1.0.1/bin/up/up_command.py
--rw-r--r--   0        0        0      962 2024-03-22 00:50:10.124707 sbin-1.0.1/bin/up/up_subcommand.py
--rw-r--r--   0        0        0        0 2022-11-03 03:24:45.772721 sbin-1.0.1/bin/version/__init__.py
--rw-r--r--   0        0        0     1160 2024-03-22 00:50:10.125438 sbin-1.0.1/bin/version/version_command.py
--rw-r--r--   0        0        0        0 2022-09-10 18:49:43.447449 sbin-1.0.1/bin/virtualenv/__init__.py
--rw-r--r--   0        0        0     1733 2024-03-22 00:50:10.121818 sbin-1.0.1/bin/virtualenv/activate_venv_command.py
--rw-r--r--   0        0        0     1604 2022-11-02 00:37:59.195647 sbin-1.0.1/bin/virtualenv/create_venv_command.py
--rw-r--r--   0        0        0       81 2022-09-18 17:05:56.575534 sbin-1.0.1/bin/virtualenv/dtos/__init__.py
--rw-r--r--   0        0        0     1117 2022-10-22 21:51:18.185638 sbin-1.0.1/bin/virtualenv/dtos/venv_command_mapper.py
--rw-r--r--   0        0        0      470 2024-03-22 01:14:21.272856 sbin-1.0.1/bin/virtualenv/dtos/venv_dto.py
--rw-r--r--   0        0        0     1620 2022-11-02 00:37:59.195972 sbin-1.0.1/bin/virtualenv/remove_venv_command.py
--rw-r--r--   0        0        0      235 2022-10-21 19:48:33.748346 sbin-1.0.1/bin/virtualenv/venv.py
--rw-r--r--   0        0        0     1145 2024-03-22 01:25:40.268362 sbin-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 sbin-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-09-01 19:17:31.002476 sbin-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1178 2022-11-02 16:49:07.027442 sbin-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-09-06 21:19:19.528859 sbin-1.1.0/bin/__init__.py
+-rw-r--r--   0        0        0      765 2022-10-23 17:19:59.121539 sbin-1.1.0/bin/bin.py
+-rw-r--r--   0        0        0        0 2022-09-22 01:28:44.998725 sbin-1.1.0/bin/bin_file/__init__.py
+-rw-r--r--   0        0        0     2558 2024-03-22 01:14:21.269990 sbin-1.1.0/bin/bin_file/bin_file_loader.py
+-rw-r--r--   0        0        0      326 2022-09-22 01:28:44.999953 sbin-1.1.0/bin/bin_file/bin_file_resolver.py
+-rw-r--r--   0        0        0        0 2022-10-18 02:20:16.831457 sbin-1.1.0/bin/bin_file/dtos/__init__.py
+-rw-r--r--   0        0        0      610 2024-03-22 00:50:10.122484 sbin-1.1.0/bin/bin_file/dtos/base_bin_file_dto.py
+-rw-r--r--   0        0        0     9810 2024-04-24 18:16:00.214300 sbin-1.1.0/bin/bin_file/dtos/bin_file_dto.py
+-rw-r--r--   0        0        0     1448 2022-10-22 21:43:35.855691 sbin-1.1.0/bin/bin_file/dtos/bin_file_mapper.py
+-rw-r--r--   0        0        0      234 2022-10-10 03:49:42.842428 sbin-1.1.0/bin/bin_file/errors.py
+-rw-r--r--   0        0        0     1779 2024-03-22 01:14:21.270713 sbin-1.1.0/bin/bin_file/init_command.py
+-rw-r--r--   0        0        0        0 2022-09-10 18:49:43.443509 sbin-1.1.0/bin/commands/__init__.py
+-rw-r--r--   0        0        0     1023 2022-11-03 03:28:30.109329 sbin-1.1.0/bin/commands/command.py
+-rw-r--r--   0        0        0     3067 2024-03-22 01:14:21.271120 sbin-1.1.0/bin/commands/command_help.py
+-rw-r--r--   0        0        0      779 2022-10-14 21:47:15.787742 sbin-1.1.0/bin/commands/errors.py
+-rw-r--r--   0        0        0        0 2022-10-22 21:58:51.166687 sbin-1.1.0/bin/commands/internal/__init__.py
+-rw-r--r--   0        0        0      627 2022-10-29 20:44:28.695838 sbin-1.1.0/bin/commands/internal/apply_env_command.py
+-rw-r--r--   0        0        0     1344 2022-10-23 17:19:59.122226 sbin-1.1.0/bin/commands/internal/factory.py
+-rw-r--r--   0        0        0      587 2022-10-22 21:58:51.167258 sbin-1.1.0/bin/commands/internal/help_only_command.py
+-rw-r--r--   0        0        0     1804 2024-03-22 00:50:10.123112 sbin-1.1.0/bin/commands/internal/log_title_command.py
+-rw-r--r--   0        0        0      567 2022-10-22 21:58:51.167956 sbin-1.1.0/bin/commands/internal/mute_logs_command.py
+-rw-r--r--   0        0        0      561 2022-10-22 21:58:51.168197 sbin-1.1.0/bin/commands/internal/noop_command.py
+-rw-r--r--   0        0        0      571 2022-10-22 21:58:51.168453 sbin-1.1.0/bin/commands/internal/unmute_logs_command.py
+-rw-r--r--   0        0        0      682 2022-10-22 21:58:51.168716 sbin-1.1.0/bin/commands/internal/with_setup_command.py
+-rw-r--r--   0        0        0        0 2022-10-22 21:51:18.183468 sbin-1.1.0/bin/custom_commands/__init__.py
+-rw-r--r--   0        0        0     1116 2024-03-22 01:14:21.271468 sbin-1.1.0/bin/custom_commands/basic_command.py
+-rw-r--r--   0        0        0     1971 2024-03-22 00:50:10.126259 sbin-1.1.0/bin/custom_commands/command_tree.py
+-rw-r--r--   0        0        0      256 2022-10-22 21:51:18.184303 sbin-1.1.0/bin/custom_commands/dtos/__init__.py
+-rw-r--r--   0        0        0      217 2022-10-22 21:51:18.184510 sbin-1.1.0/bin/custom_commands/dtos/base_custom_command_dto.py
+-rw-r--r--   0        0        0     4694 2024-04-24 18:16:00.214737 sbin-1.1.0/bin/custom_commands/dtos/command_tree_dto.py
+-rw-r--r--   0        0        0      659 2024-03-22 00:50:10.122709 sbin-1.1.0/bin/custom_commands/dtos/custom_commands_mapper.py
+-rw-r--r--   0        0        0      579 2022-10-22 21:51:18.185265 sbin-1.1.0/bin/custom_commands/dtos/str_custom_command_dto.py
+-rw-r--r--   0        0        0        0 2022-10-29 19:47:58.643745 sbin-1.1.0/bin/env/__init__.py
+-rw-r--r--   0        0        0     1574 2024-03-22 00:50:10.124493 sbin-1.1.0/bin/env/ejson_env_provider.py
+-rw-r--r--   0        0        0     1316 2024-03-22 01:14:21.271813 sbin-1.1.0/bin/env/env.py
+-rw-r--r--   0        0        0     1036 2022-10-29 19:47:58.644544 sbin-1.1.0/bin/env/env_provider.py
+-rw-r--r--   0        0        0      569 2022-10-29 19:47:58.644773 sbin-1.1.0/bin/env/env_providers.py
+-rw-r--r--   0        0        0      108 2022-10-29 20:44:28.696874 sbin-1.1.0/bin/env/errors.py
+-rw-r--r--   0        0        0     1236 2022-10-29 19:47:58.645008 sbin-1.1.0/bin/env/log_env_command.py
+-rw-r--r--   0        0        0     2771 2024-03-22 00:50:10.124933 sbin-1.1.0/bin/error_handler.py
+-rw-r--r--   0        0        0     1574 2024-03-22 00:50:10.122323 sbin-1.1.0/bin/main.py
+-rw-r--r--   0        0        0        0 2022-09-17 20:12:34.944472 sbin-1.1.0/bin/models/__init__.py
+-rw-r--r--   0        0        0      508 2024-03-22 01:22:52.108572 sbin-1.1.0/bin/models/bin_base_model.py
+-rw-r--r--   0        0        0      916 2022-11-01 01:20:00.070402 sbin-1.1.0/bin/models/sem_ver_spec.py
+-rw-r--r--   0        0        0      719 2022-11-02 17:35:06.612268 sbin-1.1.0/bin/models/str_command.py
+-rw-r--r--   0        0        0        0 2022-09-17 15:05:40.066825 sbin-1.1.0/bin/process/__init__.py
+-rw-r--r--   0        0        0      220 2022-11-02 00:37:59.195290 sbin-1.1.0/bin/process/emoji.py
+-rw-r--r--   0        0        0      124 2022-10-06 14:16:07.963680 sbin-1.1.0/bin/process/helpable.py
+-rw-r--r--   0        0        0        0 2022-10-20 16:48:15.443020 sbin-1.1.0/bin/process/io/__init__.py
+-rw-r--r--   0        0        0      707 2022-10-20 16:48:15.443346 sbin-1.1.0/bin/process/io/console_io.py
+-rw-r--r--   0        0        0      439 2022-10-20 16:48:15.443578 sbin-1.1.0/bin/process/io/io.py
+-rw-r--r--   0        0        0      340 2022-10-20 16:48:15.443828 sbin-1.1.0/bin/process/io/mute_io.py
+-rw-r--r--   0        0        0     2513 2024-03-22 01:14:21.272158 sbin-1.1.0/bin/process/process.py
+-rw-r--r--   0        0        0      274 2022-09-17 15:05:40.067634 sbin-1.1.0/bin/process/process_result.py
+-rw-r--r--   0        0        0        0 2022-09-09 18:19:23.466612 sbin-1.1.0/bin/requirements/__init__.py
+-rw-r--r--   0        0        0      348 2022-09-18 17:05:56.574363 sbin-1.1.0/bin/requirements/dtos/__init__.py
+-rw-r--r--   0        0        0      184 2022-09-17 20:12:34.945759 sbin-1.1.0/bin/requirements/dtos/base_requirement_dto.py
+-rw-r--r--   0        0        0      655 2022-09-17 20:12:34.945990 sbin-1.1.0/bin/requirements/dtos/python_requirement_dto.py
+-rw-r--r--   0        0        0      381 2022-10-11 22:35:07.274551 sbin-1.1.0/bin/requirements/dtos/requirements_command_mapper.py
+-rw-r--r--   0        0        0      664 2024-03-22 00:50:10.121358 sbin-1.1.0/bin/requirements/dtos/sem_ver_requirement_dto.py
+-rw-r--r--   0        0        0      575 2022-09-17 20:12:34.946453 sbin-1.1.0/bin/requirements/dtos/shell_requirement_dto.py
+-rw-r--r--   0        0        0      343 2022-09-17 15:05:40.067971 sbin-1.1.0/bin/requirements/requirement.py
+-rw-r--r--   0        0        0     1865 2024-03-22 00:50:10.123238 sbin-1.1.0/bin/requirements/requirements_command.py
+-rw-r--r--   0        0        0      907 2022-10-21 01:40:07.814478 sbin-1.1.0/bin/requirements/sem_ver_requirement.py
+-rw-r--r--   0        0        0      591 2022-11-02 19:27:25.649862 sbin-1.1.0/bin/requirements/shell_requirement.py
+-rw-r--r--   0        0        0        0 2022-09-13 22:17:57.860791 sbin-1.1.0/bin/up/__init__.py
+-rw-r--r--   0        0        0      952 2024-03-22 00:50:10.123677 sbin-1.1.0/bin/up/conditional_up_subcommand.py
+-rw-r--r--   0        0        0      419 2022-10-12 13:43:27.700922 sbin-1.1.0/bin/up/down_command.py
+-rw-r--r--   0        0        0      245 2022-10-06 14:16:07.965026 sbin-1.1.0/bin/up/dtos/__init__.py
+-rw-r--r--   0        0        0      317 2022-10-06 14:16:07.965342 sbin-1.1.0/bin/up/dtos/base_up_subcommand_dto.py
+-rw-r--r--   0        0        0     2085 2024-03-22 01:14:21.272507 sbin-1.1.0/bin/up/dtos/conditional_up_subcommand_dto.py
+-rw-r--r--   0        0        0      648 2022-10-06 14:16:07.965991 sbin-1.1.0/bin/up/dtos/str_up_subcommand_dto.py
+-rw-r--r--   0        0        0      664 2022-10-12 13:43:27.701243 sbin-1.1.0/bin/up/dtos/up_command_mapper.py
+-rw-r--r--   0        0        0      606 2024-04-24 18:16:00.215081 sbin-1.1.0/bin/up/simple_up_subcommand.py
+-rw-r--r--   0        0        0     2234 2024-03-22 00:50:10.126124 sbin-1.1.0/bin/up/up_command.py
+-rw-r--r--   0        0        0      962 2024-03-22 00:50:10.124707 sbin-1.1.0/bin/up/up_subcommand.py
+-rw-r--r--   0        0        0        0 2022-11-03 03:24:45.772721 sbin-1.1.0/bin/version/__init__.py
+-rw-r--r--   0        0        0     1160 2024-03-22 00:50:10.125438 sbin-1.1.0/bin/version/version_command.py
+-rw-r--r--   0        0        0        0 2022-09-10 18:49:43.447449 sbin-1.1.0/bin/virtualenv/__init__.py
+-rw-r--r--   0        0        0     1733 2024-03-22 00:50:10.121818 sbin-1.1.0/bin/virtualenv/activate_venv_command.py
+-rw-r--r--   0        0        0     1604 2022-11-02 00:37:59.195647 sbin-1.1.0/bin/virtualenv/create_venv_command.py
+-rw-r--r--   0        0        0       81 2022-09-18 17:05:56.575534 sbin-1.1.0/bin/virtualenv/dtos/__init__.py
+-rw-r--r--   0        0        0     1117 2022-10-22 21:51:18.185638 sbin-1.1.0/bin/virtualenv/dtos/venv_command_mapper.py
+-rw-r--r--   0        0        0      470 2024-03-22 01:14:21.272856 sbin-1.1.0/bin/virtualenv/dtos/venv_dto.py
+-rw-r--r--   0        0        0     1620 2022-11-02 00:37:59.195972 sbin-1.1.0/bin/virtualenv/remove_venv_command.py
+-rw-r--r--   0        0        0      235 2022-10-21 19:48:33.748346 sbin-1.1.0/bin/virtualenv/venv.py
+-rw-r--r--   0        0        0     1145 2024-04-24 18:17:34.084867 sbin-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 sbin-1.1.0/PKG-INFO
```

### Comparing `sbin-1.0.1/LICENSE` & `sbin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/README.md` & `sbin-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/bin.py` & `sbin-1.1.0/bin/bin.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/bin_file/bin_file_loader.py` & `sbin-1.1.0/bin/bin_file/bin_file_loader.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/bin_file/dtos/base_bin_file_dto.py` & `sbin-1.1.0/bin/bin_file/dtos/base_bin_file_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/bin_file/dtos/bin_file_dto.py` & `sbin-1.1.0/bin/bin_file/dtos/bin_file_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,14 @@
     req: RequirementDto
 
 
 class _UpValidationDto(BinBaseModel):
     up: UpSubcommandDto
 
 
-class _CommandsValidationDto(BinBaseModel):
-    commands: CustomCommandsDto
-
-
 class BinFileDto(BinBaseModel, BaseBinFileDto):
     name: Optional[Any]
     description: Optional[Any]
     env: Env = Env({})
     requirements: List[RequirementDto] = []
     venv: Optional[VenvDto] = None
     up: List[UpSubcommandDto] = []
```

### Comparing `sbin-1.0.1/bin/bin_file/dtos/bin_file_mapper.py` & `sbin-1.1.0/bin/bin_file/dtos/bin_file_mapper.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/bin_file/init_command.py` & `sbin-1.1.0/bin/bin_file/init_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/command.py` & `sbin-1.1.0/bin/commands/command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/command_help.py` & `sbin-1.1.0/bin/commands/command_help.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/errors.py` & `sbin-1.1.0/bin/commands/errors.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/apply_env_command.py` & `sbin-1.1.0/bin/commands/internal/apply_env_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/factory.py` & `sbin-1.1.0/bin/commands/internal/factory.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/help_only_command.py` & `sbin-1.1.0/bin/commands/internal/help_only_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/log_title_command.py` & `sbin-1.1.0/bin/commands/internal/log_title_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/mute_logs_command.py` & `sbin-1.1.0/bin/commands/internal/mute_logs_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/noop_command.py` & `sbin-1.1.0/bin/commands/internal/noop_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/unmute_logs_command.py` & `sbin-1.1.0/bin/commands/internal/unmute_logs_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/commands/internal/with_setup_command.py` & `sbin-1.1.0/bin/commands/internal/with_setup_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/custom_commands/basic_command.py` & `sbin-1.1.0/bin/custom_commands/basic_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/custom_commands/command_tree.py` & `sbin-1.1.0/bin/custom_commands/command_tree.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/custom_commands/dtos/custom_commands_mapper.py` & `sbin-1.1.0/bin/custom_commands/dtos/custom_commands_mapper.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/custom_commands/dtos/str_custom_command_dto.py` & `sbin-1.1.0/bin/custom_commands/dtos/str_custom_command_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/env/ejson_env_provider.py` & `sbin-1.1.0/bin/env/ejson_env_provider.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/env/env.py` & `sbin-1.1.0/bin/env/env.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/env/env_provider.py` & `sbin-1.1.0/bin/env/env_provider.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/env/env_providers.py` & `sbin-1.1.0/bin/env/env_providers.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/env/log_env_command.py` & `sbin-1.1.0/bin/env/log_env_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/error_handler.py` & `sbin-1.1.0/bin/error_handler.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/main.py` & `sbin-1.1.0/bin/main.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/models/sem_ver_spec.py` & `sbin-1.1.0/bin/models/sem_ver_spec.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/models/str_command.py` & `sbin-1.1.0/bin/models/str_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/process/io/console_io.py` & `sbin-1.1.0/bin/process/io/console_io.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/process/process.py` & `sbin-1.1.0/bin/process/process.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/dtos/python_requirement_dto.py` & `sbin-1.1.0/bin/requirements/dtos/python_requirement_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/dtos/sem_ver_requirement_dto.py` & `sbin-1.1.0/bin/requirements/dtos/sem_ver_requirement_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/dtos/shell_requirement_dto.py` & `sbin-1.1.0/bin/requirements/dtos/shell_requirement_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/requirements_command.py` & `sbin-1.1.0/bin/requirements/requirements_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/sem_ver_requirement.py` & `sbin-1.1.0/bin/requirements/sem_ver_requirement.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/requirements/shell_requirement.py` & `sbin-1.1.0/bin/requirements/shell_requirement.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/conditional_up_subcommand.py` & `sbin-1.1.0/bin/up/conditional_up_subcommand.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/dtos/conditional_up_subcommand_dto.py` & `sbin-1.1.0/bin/up/dtos/conditional_up_subcommand_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/dtos/str_up_subcommand_dto.py` & `sbin-1.1.0/bin/up/dtos/str_up_subcommand_dto.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/dtos/up_command_mapper.py` & `sbin-1.1.0/bin/up/dtos/up_command_mapper.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/up_command.py` & `sbin-1.1.0/bin/up/up_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/up/up_subcommand.py` & `sbin-1.1.0/bin/up/up_subcommand.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/version/version_command.py` & `sbin-1.1.0/bin/version/version_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/virtualenv/activate_venv_command.py` & `sbin-1.1.0/bin/virtualenv/activate_venv_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/virtualenv/create_venv_command.py` & `sbin-1.1.0/bin/virtualenv/create_venv_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/virtualenv/dtos/venv_command_mapper.py` & `sbin-1.1.0/bin/virtualenv/dtos/venv_command_mapper.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/bin/virtualenv/remove_venv_command.py` & `sbin-1.1.0/bin/virtualenv/remove_venv_command.py`

 * *Files identical despite different names*

### Comparing `sbin-1.0.1/pyproject.toml` & `sbin-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sbin"
-version = "1.0.1"
+version = "1.1.0"
 description = "Makes your repo setup clean"
 authors = ["Mazine Mrini <mazmrini@hotmail.com>"]
 keywords= ["bin"]
 license = "MIT License"
 readme = "README.md"
 homepage="https://gitlab.com/mazmrini/bin"
 repository="https://gitlab.com/mazmrini/bin"
```

### Comparing `sbin-1.0.1/PKG-INFO` & `sbin-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbin
-Version: 1.0.1
+Version: 1.1.0
 Summary: Makes your repo setup clean
 Home-page: https://gitlab.com/mazmrini/bin
 License: MIT
 Keywords: bin
 Author: Mazine Mrini
 Author-email: mazmrini@hotmail.com
 Requires-Python: >=3.8,<3.12
```

