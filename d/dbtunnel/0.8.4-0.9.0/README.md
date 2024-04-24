# Comparing `tmp/dbtunnel-0.8.4.tar.gz` & `tmp/dbtunnel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtunnel-0.8.4.tar", last modified: Wed Jan 24 19:44:24 2024, max compression
+gzip compressed data, was "dbtunnel-0.9.0.tar", last modified: Thu Jan 25 16:47:16 2024, max compression
```

## Comparing `dbtunnel-0.8.4.tar` & `dbtunnel-0.9.0.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.960257 dbtunnel-0.8.4/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     6964 2023-12-12 19:21:39.000000 dbtunnel-0.8.4/.gitignore
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)    11356 2023-12-01 13:25:22.000000 dbtunnel-0.8.4/LICENSE
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      388 2023-12-01 13:55:08.000000 dbtunnel-0.8.4/Makefile
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     5994 2024-01-24 19:44:24.959914 dbtunnel-0.8.4/PKG-INFO
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3857 2024-01-24 19:11:53.000000 dbtunnel-0.8.4/README.md
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.943141 dbtunnel-0.8.4/dbtunnel/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2036 2024-01-17 19:02:23.000000 dbtunnel-0.8.4/dbtunnel/__init__.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1900 2023-11-30 17:09:02.000000 dbtunnel-0.8.4/dbtunnel/bokeh.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     5430 2024-01-24 19:13:33.000000 dbtunnel-0.8.4/dbtunnel/chainlit.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2470 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/code_server.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2069 2023-11-30 20:14:42.000000 dbtunnel-0.8.4/dbtunnel/dash.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1607 2023-11-29 18:30:29.000000 dbtunnel-0.8.4/dbtunnel/fastapi.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1609 2023-12-01 15:13:42.000000 dbtunnel-0.8.4/dbtunnel/flask.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1641 2023-11-29 18:30:29.000000 dbtunnel-0.8.4/dbtunnel/gradio.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2087 2023-12-14 14:23:30.000000 dbtunnel-0.8.4/dbtunnel/ngrok.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1715 2023-11-29 20:03:10.000000 dbtunnel-0.8.4/dbtunnel/nicegui.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1809 2023-12-01 17:26:39.000000 dbtunnel-0.8.4/dbtunnel/solara.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2564 2023-12-06 16:49:28.000000 dbtunnel-0.8.4/dbtunnel/stable_diffusion_ui.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2226 2023-12-14 13:56:00.000000 dbtunnel-0.8.4/dbtunnel/streamlit.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     7970 2024-01-24 18:10:26.000000 dbtunnel-0.8.4/dbtunnel/tunnels.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2143 2024-01-24 19:35:01.000000 dbtunnel-0.8.4/dbtunnel/utils.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.945413 dbtunnel-0.8.4/dbtunnel/vendor/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1074 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/LICENSE
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/__init__.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.947814 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)       22 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/__init__.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1435 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/__main__.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/base.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3616 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/config.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      971 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/context.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.948499 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/__init__.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3810 2024-01-24 19:13:33.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/http.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4213 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/websocket.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/py.typed
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1342 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/simple_proxy.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.949079 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/utils/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/utils/__init__.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      324 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/utils/streams.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.944750 dbtunnel-0.8.4/dbtunnel.egg-info/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     5994 2024-01-24 19:44:24.000000 dbtunnel-0.8.4/dbtunnel.egg-info/PKG-INFO
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1881 2024-01-24 19:44:24.000000 dbtunnel-0.8.4/dbtunnel.egg-info/SOURCES.txt
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        1 2024-01-24 19:44:24.000000 dbtunnel-0.8.4/dbtunnel.egg-info/dependency_links.txt
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      441 2024-01-24 19:44:24.000000 dbtunnel-0.8.4/dbtunnel.egg-info/requires.txt
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        9 2024-01-24 19:44:24.000000 dbtunnel-0.8.4/dbtunnel.egg-info/top_level.txt
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.934826 dbtunnel-0.8.4/examples/
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.949726 dbtunnel-0.8.4/examples/bokeh/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      328 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/bokeh/bokeh-example.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3362 2023-11-29 20:51:30.000000 dbtunnel-0.8.4/examples/bokeh/bokeh_sample.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.951938 dbtunnel-0.8.4/examples/chainlit/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      372 2024-01-24 18:15:31.000000 dbtunnel-0.8.4/examples/chainlit/chainlit-basic-example.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      501 2024-01-24 19:42:02.000000 dbtunnel-0.8.4/examples/chainlit/chainlit-foundation-model.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      496 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/examples/chainlit/chainlit-ngrok.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      236 2023-12-12 19:21:39.000000 dbtunnel-0.8.4/examples/chainlit/chainlit_example.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4826 2024-01-24 19:11:47.000000 dbtunnel-0.8.4/examples/chainlit/chainlit_foundation_model.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.952422 dbtunnel-0.8.4/examples/code-server/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      425 2024-01-17 19:02:01.000000 dbtunnel-0.8.4/examples/code-server/code-server-example.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.952832 dbtunnel-0.8.4/examples/dash/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      876 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/dash/dask-example.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.953239 dbtunnel-0.8.4/examples/fastapi/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      724 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/fastapi/fastapi.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.953534 dbtunnel-0.8.4/examples/flask/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      357 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/flask/flask-app.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.954553 dbtunnel-0.8.4/examples/gradio/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2648 2023-12-14 13:56:00.000000 dbtunnel-0.8.4/examples/gradio/gradio-chat-bricks-foundational-models-demo.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3784 2023-12-01 22:27:05.000000 dbtunnel-0.8.4/examples/gradio/gradio-chat-mistral7b-demo.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      965 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/gradio/gradio-demo.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.955006 dbtunnel-0.8.4/examples/nicegui/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      855 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/nicegui/nicegui-example.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.955803 dbtunnel-0.8.4/examples/solara/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4456 2023-12-01 16:49:35.000000 dbtunnel-0.8.4/examples/solara/scatter.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      324 2023-12-01 17:51:51.000000 dbtunnel-0.8.4/examples/solara/solara-example.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.956190 dbtunnel-0.8.4/examples/stable-diffusion-webui/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      215 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/stable-diffusion-webui/stable-diffusion-example.py
-drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 19:44:24.957567 dbtunnel-0.8.4/examples/streamlit/
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      341 2024-01-17 19:02:06.000000 dbtunnel-0.8.4/examples/streamlit/streamlit-example-driver.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      900 2024-01-17 19:02:06.000000 dbtunnel-0.8.4/examples/streamlit/streamlit-example-ngrok.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1061 2023-12-01 15:10:10.000000 dbtunnel-0.8.4/examples/streamlit/streamlit_example.py
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)       38 2024-01-24 19:44:24.960324 dbtunnel-0.8.4/setup.cfg
--rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2419 2024-01-24 17:43:56.000000 dbtunnel-0.8.4/setup.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.456245 dbtunnel-0.9.0/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     6964 2023-12-12 19:21:39.000000 dbtunnel-0.9.0/.gitignore
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)    11356 2023-12-01 13:25:22.000000 dbtunnel-0.9.0/LICENSE
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      388 2023-12-01 13:55:08.000000 dbtunnel-0.9.0/Makefile
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     7226 2024-01-25 16:47:16.455870 dbtunnel-0.9.0/PKG-INFO
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4982 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/README.md
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.439756 dbtunnel-0.9.0/dbtunnel/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2488 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/dbtunnel/__init__.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1900 2023-11-30 17:09:02.000000 dbtunnel-0.9.0/dbtunnel/bokeh.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     5348 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/dbtunnel/chainlit.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2470 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/code_server.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2069 2023-11-30 20:14:42.000000 dbtunnel-0.9.0/dbtunnel/dash.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1607 2023-11-29 18:30:29.000000 dbtunnel-0.9.0/dbtunnel/fastapi.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1609 2023-12-01 15:13:42.000000 dbtunnel-0.9.0/dbtunnel/flask.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1641 2023-11-29 18:30:29.000000 dbtunnel-0.9.0/dbtunnel/gradio.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2087 2023-12-14 14:23:30.000000 dbtunnel-0.9.0/dbtunnel/ngrok.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1715 2023-11-29 20:03:10.000000 dbtunnel-0.9.0/dbtunnel/nicegui.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1392 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/dbtunnel/shiny.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1809 2023-12-01 17:26:39.000000 dbtunnel-0.9.0/dbtunnel/solara.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2564 2023-12-06 16:49:28.000000 dbtunnel-0.9.0/dbtunnel/stable_diffusion_ui.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2226 2023-12-14 13:56:00.000000 dbtunnel-0.9.0/dbtunnel/streamlit.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     8327 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/dbtunnel/tunnels.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2143 2024-01-24 19:35:01.000000 dbtunnel-0.9.0/dbtunnel/utils.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.441720 dbtunnel-0.9.0/dbtunnel/vendor/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1074 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/LICENSE
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/__init__.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.443563 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)       22 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/__init__.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1435 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/__main__.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/base.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3616 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/config.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      971 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/context.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.444514 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/__init__.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3810 2024-01-24 19:13:33.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/http.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4213 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/websocket.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/py.typed
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1342 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/simple_proxy.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.444959 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/utils/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/utils/__init__.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      324 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/utils/streams.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.441272 dbtunnel-0.9.0/dbtunnel.egg-info/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     7226 2024-01-25 16:47:16.000000 dbtunnel-0.9.0/dbtunnel.egg-info/PKG-INFO
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1957 2024-01-25 16:47:16.000000 dbtunnel-0.9.0/dbtunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        1 2024-01-25 16:47:16.000000 dbtunnel-0.9.0/dbtunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      469 2024-01-25 16:47:16.000000 dbtunnel-0.9.0/dbtunnel.egg-info/requires.txt
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)        9 2024-01-25 16:47:16.000000 dbtunnel-0.9.0/dbtunnel.egg-info/top_level.txt
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.433067 dbtunnel-0.9.0/examples/
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.445474 dbtunnel-0.9.0/examples/bokeh/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      328 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/bokeh/bokeh-example.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3362 2023-11-29 20:51:30.000000 dbtunnel-0.9.0/examples/bokeh/bokeh_sample.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.447621 dbtunnel-0.9.0/examples/chainlit/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      372 2024-01-24 18:15:31.000000 dbtunnel-0.9.0/examples/chainlit/chainlit-basic-example.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      786 2024-01-24 19:58:54.000000 dbtunnel-0.9.0/examples/chainlit/chainlit-foundation-model-rag-example.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      496 2024-01-24 17:43:56.000000 dbtunnel-0.9.0/examples/chainlit/chainlit-ngrok.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      236 2023-12-12 19:21:39.000000 dbtunnel-0.9.0/examples/chainlit/chainlit_example.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     5039 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/examples/chainlit/chainlit_foundation_model.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.447884 dbtunnel-0.9.0/examples/code-server/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      425 2024-01-17 19:02:01.000000 dbtunnel-0.9.0/examples/code-server/code-server-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.448238 dbtunnel-0.9.0/examples/dash/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      876 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/dash/dask-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.448846 dbtunnel-0.9.0/examples/fastapi/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      724 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/fastapi/fastapi.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.449262 dbtunnel-0.9.0/examples/flask/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      357 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/flask/flask-app.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.450279 dbtunnel-0.9.0/examples/gradio/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2648 2023-12-14 13:56:00.000000 dbtunnel-0.9.0/examples/gradio/gradio-chat-bricks-foundational-models-demo.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     3784 2023-12-01 22:27:05.000000 dbtunnel-0.9.0/examples/gradio/gradio-chat-mistral7b-demo.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      965 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/gradio/gradio-demo.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.450546 dbtunnel-0.9.0/examples/nicegui/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      855 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/nicegui/nicegui-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.451068 dbtunnel-0.9.0/examples/shiny-python/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      760 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/examples/shiny-python/shiny-python-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.451728 dbtunnel-0.9.0/examples/solara/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     4456 2023-12-01 16:49:35.000000 dbtunnel-0.9.0/examples/solara/scatter.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      324 2023-12-01 17:51:51.000000 dbtunnel-0.9.0/examples/solara/solara-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.452082 dbtunnel-0.9.0/examples/stable-diffusion-webui/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      215 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/stable-diffusion-webui/stable-diffusion-example.py
+drwxr-xr-x   0 sri.tikkireddy   (502) staff       (20)        0 2024-01-25 16:47:16.453401 dbtunnel-0.9.0/examples/streamlit/
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      341 2024-01-17 19:02:06.000000 dbtunnel-0.9.0/examples/streamlit/streamlit-example-driver.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)      900 2024-01-17 19:02:06.000000 dbtunnel-0.9.0/examples/streamlit/streamlit-example-ngrok.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     1061 2023-12-01 15:10:10.000000 dbtunnel-0.9.0/examples/streamlit/streamlit_example.py
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)       38 2024-01-25 16:47:16.456359 dbtunnel-0.9.0/setup.cfg
+-rw-r--r--   0 sri.tikkireddy   (502) staff       (20)     2498 2024-01-25 16:47:10.000000 dbtunnel-0.9.0/setup.py
```

### Comparing `dbtunnel-0.8.4/.gitignore` & `dbtunnel-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/LICENSE` & `dbtunnel-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/PKG-INFO` & `dbtunnel-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtunnel
-Version: 0.8.4
+Version: 0.9.0
 Summary: Run app and get cluster proxy url for it in databricks clusters
 Home-page: https://github.com/stikkireddy/dbtunnel
 Author: Sri Tikkireddy
 Author-email: sri.tikkireddy@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,14 +50,17 @@
 Requires-Dist: chainlit; extra == "chainlit"
 Requires-Dist: nest_asyncio; extra == "chainlit"
 Requires-Dist: uvicorn; extra == "chainlit"
 Provides-Extra: asgiproxy
 Requires-Dist: aiohttp; extra == "asgiproxy"
 Requires-Dist: starlette; extra == "asgiproxy"
 Requires-Dist: websockets; extra == "asgiproxy"
+Provides-Extra: shiny
+Requires-Dist: shiny; extra == "shiny"
+Requires-Dist: nest_asyncio; extra == "shiny"
 
 # dbtunnel 
 
 Proxy solution to run elegant Web UIs natively inside databricks notebooks.
 
 **YOU CAN ONLY USE THIS IN DATABRICKS NOTEBOOKS WITH A RUNNING CLUSTER**
 
@@ -73,22 +76,40 @@
 * [x] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
 * [x] stable diffusion webui: [stable-diffusion-example.py](examples%2Fstable-diffusion-webui%2Fstable-diffusion-example.py)
 * [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
 * [x] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
 * [x] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
 * [x] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
 * [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
-* [ ] posit
+* [x] shiny for python: [shiny-python-example.py](examples%2Fshiny-python%2Fshiny-python-example.py)
 * [ ] panel
 * [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
-* [x] chainlit: [chainlit.py](examples%2Fchainlit%2Fchainlit.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
 * [x] code-server on repos [code-server-example.py](examples%2Fcode-server%2Fcode-server-example.py)
 
 Easy way to test out llm chatbots; look in examples/gradio
 
+### File or Directory Support
+
+This is to support decoupling your UI code from your databricks notebooks. 
+Usually will have a script_path argument instead of directly passing your "app" object. This is convenient for 
+shipping your app outside of a notebook.
+
+* [ ] fastapi: [fastapi.py](examples%2Ffastapi%2Ffastapi.py)
+* [ ] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
+* [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
+* [ ] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
+* [ ] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
+* [ ] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
+* [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
+* [ ] shiny for python
+* [ ] panel
+* [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
+
 ### Chatbot Support
 
 **You must use A10 GPU instances or higher**
 
 * [x] Mistral-7b [gradio-chat-mistral7b-demo.py](examples%2Fgradio%2Fgradio-chat-mistral7b-demo.py)
 * [x] Mixtral 8x7B [chainlit-foundation-model.py](examples%2Fchainlit%2Fchainlit-foundation-model.py)
 * [ ] Llama-2-7b
```

### Comparing `dbtunnel-0.8.4/README.md` & `dbtunnel-0.9.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -16,22 +16,40 @@
 * [x] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
 * [x] stable diffusion webui: [stable-diffusion-example.py](examples%2Fstable-diffusion-webui%2Fstable-diffusion-example.py)
 * [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
 * [x] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
 * [x] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
 * [x] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
 * [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
-* [ ] posit
+* [x] shiny for python: [shiny-python-example.py](examples%2Fshiny-python%2Fshiny-python-example.py)
 * [ ] panel
 * [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
-* [x] chainlit: [chainlit.py](examples%2Fchainlit%2Fchainlit.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
 * [x] code-server on repos [code-server-example.py](examples%2Fcode-server%2Fcode-server-example.py)
 
 Easy way to test out llm chatbots; look in examples/gradio
 
+### File or Directory Support
+
+This is to support decoupling your UI code from your databricks notebooks. 
+Usually will have a script_path argument instead of directly passing your "app" object. This is convenient for 
+shipping your app outside of a notebook.
+
+* [ ] fastapi: [fastapi.py](examples%2Ffastapi%2Ffastapi.py)
+* [ ] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
+* [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
+* [ ] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
+* [ ] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
+* [ ] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
+* [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
+* [ ] shiny for python
+* [ ] panel
+* [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
+
 ### Chatbot Support
 
 **You must use A10 GPU instances or higher**
 
 * [x] Mistral-7b [gradio-chat-mistral7b-demo.py](examples%2Fgradio%2Fgradio-chat-mistral7b-demo.py)
 * [x] Mixtral 8x7B [chainlit-foundation-model.py](examples%2Fchainlit%2Fchainlit-foundation-model.py)
 * [ ] Llama-2-7b
```

### Comparing `dbtunnel-0.8.4/dbtunnel/__init__.py` & `dbtunnel-0.9.0/dbtunnel/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+import subprocess
+
 from dbtunnel.bokeh import BokehTunnel
 from dbtunnel.chainlit import ChainlitAppTunnel
 from dbtunnel.code_server import CodeServerTunnel
 from dbtunnel.dash import DashAppTunnel
 from dbtunnel.fastapi import FastApiAppTunnel
 from dbtunnel.flask import FlaskAppTunnel
 from dbtunnel.gradio import GradioAppTunnel
 from dbtunnel.nicegui import NiceGuiAppTunnel
+from dbtunnel.shiny import ShinyPythonAppTunnel
 from dbtunnel.solara import SolaraAppTunnel
 from dbtunnel.stable_diffusion_ui import StableDiffusionUITunnel
 from dbtunnel.streamlit import StreamlitTunnel
 
 
 class AppTunnels:
+    """
+    This class is used to create tunnels to different apps. It is the user facing api should not have breaking changes.
+    """
+
+    @staticmethod
+    def kill_port(port: int):
+        subprocess.run(f"kill -9 $(lsof -t -i:{port})", capture_output=True, shell=True)
 
     @staticmethod
     def fastapi(app, port: int = 8080):
         return FastApiAppTunnel(app, port)
 
     @staticmethod
     def gradio(app, port: int = 8080):
@@ -55,9 +65,13 @@
     def code_server(directory_path: str = None, repo_name: str = None, port: int = 9988):
         return CodeServerTunnel(directory_path, repo_name, port)
 
     @staticmethod
     def chainlit(script_path: str, cwd: str = None, port: int = 8000):
         return ChainlitAppTunnel(script_path, cwd=cwd, port=port)
 
+    @staticmethod
+    def shiny_python(app, port: int = 8080):
+        return ShinyPythonAppTunnel(app, port)
+
 
 dbtunnel = AppTunnels()
```

### Comparing `dbtunnel-0.8.4/dbtunnel/bokeh.py` & `dbtunnel-0.9.0/dbtunnel/bokeh.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/chainlit.py` & `dbtunnel-0.9.0/dbtunnel/chainlit.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,16 @@
         regex_pattern = r'\{path:"\/",element:(\w+)\.jsx\((\w+),\{\}\)\}'
 
         decoded_content = content.decode("utf-8")
         # Find all matches
         # find the default root function
         matches = re.findall(regex_pattern, decoded_content)
         if matches:
-            print(matches)
             jsx_call = matches[0][0]
             func = matches[0][1]  # Assuming there is only one match
-
-            print(f"Found match: {jsx_call}, {func}")
             modified_code = re.sub(r'\{path:"\*",element:.*\.jsx\(.*,\{replace:!0,to:"\/"\}\)\}',
                                    f'{{path:"*",element:{jsx_call}.jsx({func},{{}})}}', decoded_content)
             return modified_code.encode("utf-8")
         else:
             print("No match found.")
             return content
```

### Comparing `dbtunnel-0.8.4/dbtunnel/code_server.py` & `dbtunnel-0.9.0/dbtunnel/code_server.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/dash.py` & `dbtunnel-0.9.0/dbtunnel/dash.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/fastapi.py` & `dbtunnel-0.9.0/dbtunnel/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/flask.py` & `dbtunnel-0.9.0/dbtunnel/flask.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/gradio.py` & `dbtunnel-0.9.0/dbtunnel/gradio.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/ngrok.py` & `dbtunnel-0.9.0/dbtunnel/ngrok.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/nicegui.py` & `dbtunnel-0.9.0/dbtunnel/nicegui.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/solara.py` & `dbtunnel-0.9.0/dbtunnel/solara.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/stable_diffusion_ui.py` & `dbtunnel-0.9.0/dbtunnel/stable_diffusion_ui.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/streamlit.py` & `dbtunnel-0.9.0/dbtunnel/streamlit.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/tunnels.py` & `dbtunnel-0.9.0/dbtunnel/tunnels.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 @dataclass
 class ProxySettings:
     proxy_url: str
     port: str
     url_base_path: str
     url_base_path_no_port: Optional[str] = None
 
+    def get_proxy_url(self, ensure_ends_with_slash=False):
+        """
+        For certain apps that use relative paths like "assets/index-*.js" we need to ensure that the url ends
+        with a slash.
+        """
+        if ensure_ends_with_slash is True:
+            return self.proxy_url.rstrip("/") + "/"
+        return self.proxy_url
+
 
 def get_cloud(context: Dict[str, Any]) -> str:
     # TODO: support gcp
     if context["extraContext"]["api_url"].endswith("azuredatabricks.net"):
         return "azure"
     return "aws"
 
@@ -52,15 +61,15 @@
         url_base_path=url_base_path,
         url_base_path_no_port=url_base_path_no_port
     )
 
 
 Flavor = Literal[
     "gradio", "fastapi", "nicegui", "streamlit", "stable-diffusion-ui", "bokeh", "flask", "dash", "solara",
-    "code-server", "chainlit"]
+    "code-server", "chainlit", "shiny-python"]
 
 
 # from langchain: https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/llms/databricks.py#L86
 def get_repl_context() -> Any:
     """Gets the notebook REPL context if running inside a Databricks notebook.
     Returns None otherwise.
     """
```

### Comparing `dbtunnel-0.8.4/dbtunnel/utils.py` & `dbtunnel-0.9.0/dbtunnel/utils.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/LICENSE` & `dbtunnel-0.9.0/dbtunnel/vendor/LICENSE`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/__main__.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/__main__.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/config.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/config.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/context.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/context.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/http.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/http.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/proxies/websocket.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/proxies/websocket.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel/vendor/asgiproxy/simple_proxy.py` & `dbtunnel-0.9.0/dbtunnel/vendor/asgiproxy/simple_proxy.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/dbtunnel.egg-info/PKG-INFO` & `dbtunnel-0.9.0/dbtunnel.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbtunnel
-Version: 0.8.4
+Version: 0.9.0
 Summary: Run app and get cluster proxy url for it in databricks clusters
 Home-page: https://github.com/stikkireddy/dbtunnel
 Author: Sri Tikkireddy
 Author-email: sri.tikkireddy@databricks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,14 +50,17 @@
 Requires-Dist: chainlit; extra == "chainlit"
 Requires-Dist: nest_asyncio; extra == "chainlit"
 Requires-Dist: uvicorn; extra == "chainlit"
 Provides-Extra: asgiproxy
 Requires-Dist: aiohttp; extra == "asgiproxy"
 Requires-Dist: starlette; extra == "asgiproxy"
 Requires-Dist: websockets; extra == "asgiproxy"
+Provides-Extra: shiny
+Requires-Dist: shiny; extra == "shiny"
+Requires-Dist: nest_asyncio; extra == "shiny"
 
 # dbtunnel 
 
 Proxy solution to run elegant Web UIs natively inside databricks notebooks.
 
 **YOU CAN ONLY USE THIS IN DATABRICKS NOTEBOOKS WITH A RUNNING CLUSTER**
 
@@ -73,22 +76,40 @@
 * [x] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
 * [x] stable diffusion webui: [stable-diffusion-example.py](examples%2Fstable-diffusion-webui%2Fstable-diffusion-example.py)
 * [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
 * [x] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
 * [x] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
 * [x] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
 * [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
-* [ ] posit
+* [x] shiny for python: [shiny-python-example.py](examples%2Fshiny-python%2Fshiny-python-example.py)
 * [ ] panel
 * [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
-* [x] chainlit: [chainlit.py](examples%2Fchainlit%2Fchainlit.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
 * [x] code-server on repos [code-server-example.py](examples%2Fcode-server%2Fcode-server-example.py)
 
 Easy way to test out llm chatbots; look in examples/gradio
 
+### File or Directory Support
+
+This is to support decoupling your UI code from your databricks notebooks. 
+Usually will have a script_path argument instead of directly passing your "app" object. This is convenient for 
+shipping your app outside of a notebook.
+
+* [ ] fastapi: [fastapi.py](examples%2Ffastapi%2Ffastapi.py)
+* [ ] gradio: [gradio-demo.py](examples%2Fgradio%2Fgradio-demo.py)
+* [x] streamlit: [streamlit_example.py](examples%2Fstreamlit%2Fstreamlit_example.py)
+* [ ] nicegui: [nicegui-example.py](examples%2Fnicegui%2Fnicegui-example.py)
+* [ ] flask: [flask-app.py](examples%2Fflask%2Fflask-app.py)
+* [ ] dash: [dask-example.py](examples%2Fdash%2Fdask-example.py)
+* [x] bokeh: [bokeh-example.py](examples%2Fbokeh%2Fbokeh-example.py)
+* [ ] shiny for python
+* [ ] panel
+* [x] solara: [solara-example.py](examples%2Fsolara%2Fsolara-example.py)
+* [x] chainlit: [chainlit-foundation-model-rag-example.py](examples%2Fchainlit%2Fchainlit-foundation-model-rag-example.py)
+
 ### Chatbot Support
 
 **You must use A10 GPU instances or higher**
 
 * [x] Mistral-7b [gradio-chat-mistral7b-demo.py](examples%2Fgradio%2Fgradio-chat-mistral7b-demo.py)
 * [x] Mixtral 8x7B [chainlit-foundation-model.py](examples%2Fchainlit%2Fchainlit-foundation-model.py)
 * [ ] Llama-2-7b
```

### Comparing `dbtunnel-0.8.4/dbtunnel.egg-info/SOURCES.txt` & `dbtunnel-0.9.0/dbtunnel.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dbtunnel/code_server.py
 dbtunnel/dash.py
 dbtunnel/fastapi.py
 dbtunnel/flask.py
 dbtunnel/gradio.py
 dbtunnel/ngrok.py
 dbtunnel/nicegui.py
+dbtunnel/shiny.py
 dbtunnel/solara.py
 dbtunnel/stable_diffusion_ui.py
 dbtunnel/streamlit.py
 dbtunnel/tunnels.py
 dbtunnel/utils.py
 dbtunnel.egg-info/PKG-INFO
 dbtunnel.egg-info/SOURCES.txt
@@ -36,25 +37,26 @@
 dbtunnel/vendor/asgiproxy/proxies/http.py
 dbtunnel/vendor/asgiproxy/proxies/websocket.py
 dbtunnel/vendor/asgiproxy/utils/__init__.py
 dbtunnel/vendor/asgiproxy/utils/streams.py
 examples/bokeh/bokeh-example.py
 examples/bokeh/bokeh_sample.py
 examples/chainlit/chainlit-basic-example.py
-examples/chainlit/chainlit-foundation-model.py
+examples/chainlit/chainlit-foundation-model-rag-example.py
 examples/chainlit/chainlit-ngrok.py
 examples/chainlit/chainlit_example.py
 examples/chainlit/chainlit_foundation_model.py
 examples/code-server/code-server-example.py
 examples/dash/dask-example.py
 examples/fastapi/fastapi.py
 examples/flask/flask-app.py
 examples/gradio/gradio-chat-bricks-foundational-models-demo.py
 examples/gradio/gradio-chat-mistral7b-demo.py
 examples/gradio/gradio-demo.py
 examples/nicegui/nicegui-example.py
+examples/shiny-python/shiny-python-example.py
 examples/solara/scatter.py
 examples/solara/solara-example.py
 examples/stable-diffusion-webui/stable-diffusion-example.py
 examples/streamlit/streamlit-example-driver.py
 examples/streamlit/streamlit-example-ngrok.py
 examples/streamlit/streamlit_example.py
```

### Comparing `dbtunnel-0.8.4/examples/bokeh/bokeh_sample.py` & `dbtunnel-0.9.0/examples/bokeh/bokeh_sample.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/chainlit/chainlit_foundation_model.py` & `dbtunnel-0.9.0/examples/chainlit/chainlit_foundation_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,22 @@
 
 @cl.step
 async def retriever(content: str):
     loop = asyncio.get_event_loop()
     await cl.sleep(0)
     processed_prompt = await loop.run_in_executor(None, rag_prompt.invoke, content)
     return [{"content": msg.content, "role": "user"} for msg in processed_prompt.to_messages()]
-    # return "Response from the tool!"
+
+
+@cl.on_chat_start
+async def on_start():
+    msg = cl.Message(content="Please ask any questions about the book of Frankenstein; Or, The Modern Prometheus by Mary Wollstonecraft Shelley. Example: Who is Frankenstein's monster?")
+
+    await msg.send()
+
 
 @cl.on_message
 async def main(message: cl.Message):
     # Your custom logic goes here...
     response = cl.Message(content="")
     loop = asyncio.get_event_loop()
     await response.send()  # causes loading indicator
```

### Comparing `dbtunnel-0.8.4/examples/dash/dask-example.py` & `dbtunnel-0.9.0/examples/dash/dask-example.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/fastapi/fastapi.py` & `dbtunnel-0.9.0/examples/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/gradio/gradio-chat-bricks-foundational-models-demo.py` & `dbtunnel-0.9.0/examples/gradio/gradio-chat-bricks-foundational-models-demo.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/gradio/gradio-chat-mistral7b-demo.py` & `dbtunnel-0.9.0/examples/gradio/gradio-chat-mistral7b-demo.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/gradio/gradio-demo.py` & `dbtunnel-0.9.0/examples/gradio/gradio-demo.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/nicegui/nicegui-example.py` & `dbtunnel-0.9.0/examples/nicegui/nicegui-example.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/solara/scatter.py` & `dbtunnel-0.9.0/examples/solara/scatter.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/streamlit/streamlit-example-ngrok.py` & `dbtunnel-0.9.0/examples/streamlit/streamlit-example-ngrok.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/examples/streamlit/streamlit_example.py` & `dbtunnel-0.9.0/examples/streamlit/streamlit_example.py`

 * *Files identical despite different names*

### Comparing `dbtunnel-0.8.4/setup.py` & `dbtunnel-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,14 +72,18 @@
             "nest_asyncio",
             "uvicorn",
         ],
         "asgiproxy": [
             "aiohttp",
             "starlette",
             "websockets"
+        ],
+        "shiny": [
+            "shiny",
+            "nest_asyncio",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

