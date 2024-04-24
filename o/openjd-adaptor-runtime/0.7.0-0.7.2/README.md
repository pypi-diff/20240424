# Comparing `tmp/openjd_adaptor_runtime-0.7.0.tar.gz` & `tmp/openjd_adaptor_runtime-0.7.2.tar.gz`

## Comparing `openjd_adaptor_runtime-0.7.0.tar` & `openjd_adaptor_runtime-0.7.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/__init__.py
--rw-r--r--   0        0        0    19313 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_entrypoint.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_osname.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_version.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/configuration.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/configuration.schema.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/py.typed
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/__init__.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_named_pipe_server.py
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_runner.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/background_named_pipe_request_handler.py
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/frontend_runner.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/http_server.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/log_buffers.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/model.py
--rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/server_response.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/exceptions.py
--rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/request_handler.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/sockets.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/__init__.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_request_handler.py
--rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_server.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/__init__.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_logging.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_secure_open.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/__init__.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_runner.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_states.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_base_adaptor.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_command_adaptor.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_path_mapping.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_validator.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_versioning.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_adaptor_configuration.schema.json
--rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration.py
--rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration_manager.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/app_handlers/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/app_handlers/_regex_callback_handler.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/__init__.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_actions_queue.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server_response.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_http_request_handler.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_named_pipe_request_handler.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_win_adaptor_server.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_logging.py
--rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_logging_subprocess.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_managed_process.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_stream_logger.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/_version.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/action.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/base_client_interface.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/connection.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/posix_client_interface.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/py.typed
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/win_client_interface.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_config.py
--rw-r--r--   0        0        0    17311 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_helper.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/NOTICE
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/hatch.toml
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    11449 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/__init__.py
+-rw-r--r--   0        0        0    19313 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_entrypoint.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_osname.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_version.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/configuration.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/configuration.schema.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/py.typed
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/__init__.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/backend_named_pipe_server.py
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/backend_runner.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/background_named_pipe_request_handler.py
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/frontend_runner.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/http_server.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/log_buffers.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/model.py
+-rw-r--r--   0        0        0     9493 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/server_response.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/exceptions.py
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/request_handler.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/sockets.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_named_pipe/__init__.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_named_pipe/named_pipe_request_handler.py
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_named_pipe/named_pipe_server.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_utils/__init__.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_utils/_logging.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_utils/_secure_open.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor_runner.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor_states.py
+-rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_base_adaptor.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_command_adaptor.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_path_mapping.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_validator.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_versioning.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/_adaptor_configuration.schema.json
+-rw-r--r--   0        0        0     6342 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/_configuration.py
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/_configuration_manager.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/app_handlers/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/app_handlers/_regex_callback_handler.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/__init__.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_actions_queue.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_adaptor_server.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_adaptor_server_response.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_http_request_handler.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_named_pipe_request_handler.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_win_adaptor_server.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_logging.py
+-rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_logging_subprocess.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_managed_process.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_stream_logger.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/_version.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/action.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/base_client_interface.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/connection.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/posix_client_interface.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/py.typed
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/win_client_interface.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/named_pipe/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/named_pipe/named_pipe_config.py
+-rw-r--r--   0        0        0    17311 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/named_pipe/named_pipe_helper.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/NOTICE
+-rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/hatch.toml
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 openjd_adaptor_runtime-0.7.2/PKG-INFO
```

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_entrypoint.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_entrypoint.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_osname.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_osname.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_named_pipe_server.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/backend_named_pipe_server.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/backend_runner.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/backend_runner.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/background_named_pipe_request_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/background_named_pipe_request_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/frontend_runner.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/frontend_runner.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/http_server.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/http_server.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/log_buffers.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/log_buffers.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/model.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/model.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_background/server_response.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_background/server_response.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/request_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/request_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_http/sockets.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_http/sockets.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_request_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_named_pipe/named_pipe_request_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_named_pipe/named_pipe_server.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_named_pipe/named_pipe_server.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_logging.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_utils/_logging.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/_utils/_secure_open.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/_utils/_secure_open.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/__init__.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_runner.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor_runner.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_adaptor_states.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_adaptor_states.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_base_adaptor.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_base_adaptor.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_command_adaptor.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_command_adaptor.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_path_mapping.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_path_mapping.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_validator.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_validator.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/_versioning.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/_versioning.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/__init__.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/adaptors/configuration/_configuration_manager.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/adaptors/configuration/_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/app_handlers/_regex_callback_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/app_handlers/_regex_callback_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_actions_queue.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_actions_queue.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_adaptor_server.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_adaptor_server_response.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_adaptor_server_response.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_http_request_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_http_request_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_named_pipe_request_handler.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_named_pipe_request_handler.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/application_ipc/_win_adaptor_server.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/application_ipc/_win_adaptor_server.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_logging_subprocess.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_logging_subprocess.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_managed_process.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_managed_process.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime/process/_stream_logger.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime/process/_stream_logger.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/__init__.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/action.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/action.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/base_client_interface.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/base_client_interface.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/connection.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/connection.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/posix_client_interface.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/posix_client_interface.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/win_client_interface.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/win_client_interface.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_config.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/named_pipe/named_pipe_config.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/openjd/adaptor_runtime_client/named_pipe/named_pipe_helper.py` & `openjd_adaptor_runtime-0.7.2/openjd/adaptor_runtime_client/named_pipe/named_pipe_helper.py`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/LICENSE` & `openjd_adaptor_runtime-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/README.md` & `openjd_adaptor_runtime-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/hatch.toml` & `openjd_adaptor_runtime-0.7.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `openjd_adaptor_runtime-0.7.0/pyproject.toml` & `openjd_adaptor_runtime-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,25 @@
   "Programming Language :: Python :: 3.12",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "License :: OSI Approved :: Apache Software License",
   "Intended Audience :: Developers",
 ]
-
 dependencies = [
   "pyyaml ~= 6.0",
   "jsonschema >= 4.17.0, == 4.*",
   "pywin32 == 306; platform_system == 'Windows'",
 ]
 
+[project.urls]
+Homepage = "https://github.com/OpenJobDescription/openjd-adaptor-runtime-for-python"
+Source = "https://github.com/OpenJobDescription/openjd-adaptor-runtime-for-python"
+
+
 [tool.hatch.build]
 artifacts = [
   "*_version.py"
 ]
 only-pacakges = true
 
 [tool.hatch.version]
```

### Comparing `openjd_adaptor_runtime-0.7.0/PKG-INFO` & `openjd_adaptor_runtime-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.3
 Name: openjd-adaptor-runtime
-Version: 0.7.0
+Version: 0.7.2
 Summary: A python library for building adaptors that integrate applications with Open Job Description jobs.
+Project-URL: Homepage, https://github.com/OpenJobDescription/openjd-adaptor-runtime-for-python
+Project-URL: Source, https://github.com/OpenJobDescription/openjd-adaptor-runtime-for-python
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

