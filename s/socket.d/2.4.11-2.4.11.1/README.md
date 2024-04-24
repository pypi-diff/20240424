# Comparing `tmp/socket.d-2.4.11.tar.gz` & `tmp/socket.d-2.4.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.11.tar", last modified: Tue Apr 23 02:53:54 2024, max compression
+gzip compressed data, was "socket.d-2.4.11.1.tar", last modified: Wed Apr 24 04:51:51 2024, max compression
```

## Comparing `socket.d-2.4.11.tar` & `socket.d-2.4.11.1.tar`

### file list

```diff
@@ -1,153 +1,158 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.160510 socket.d-2.4.11/
--rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-23 02:53:54.159715 socket.d-2.4.11/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.11/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-23 02:53:54.160696 socket.d-2.4.11/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-23 02:26:11.000000 socket.d-2.4.11/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.158442 socket.d-2.4.11/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     5025 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.009590 socket.d-2.4.11/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-23 02:26:11.000000 socket.d-2.4.11/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.013870 socket.d-2.4.11/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.017166 socket.d-2.4.11/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2690 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.018444 socket.d-2.4.11/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.019139 socket.d-2.4.11/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.031843 socket.d-2.4.11/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3607 2024-04-18 09:13:43.000000 socket.d-2.4.11/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6520 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.051133 socket.d-2.4.11/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2482 2024-04-18 09:13:43.000000 socket.d-2.4.11/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-22 15:28:49.000000 socket.d-2.4.11/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-22 17:01:30.000000 socket.d-2.4.11/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 00:58:23.000000 socket.d-2.4.11/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.056171 socket.d-2.4.11/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-22 15:48:56.000000 socket.d-2.4.11/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-22 15:21:21.000000 socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-22 16:12:25.000000 socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-22 16:02:45.000000 socket.d-2.4.11/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.062763 socket.d-2.4.11/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-18 13:46:31.000000 socket.d-2.4.11/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.065816 socket.d-2.4.11/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.075247 socket.d-2.4.11/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     7305 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-20 12:58:36.000000 socket.d-2.4.11/socketd/transport/core/impl/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)     7943 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.092011 socket.d-2.4.11/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-22 14:42:26.000000 socket.d-2.4.11/socketd/transport/core/listener/RouteSelector.py
--rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-22 17:36:14.000000 socket.d-2.4.11/socketd/transport/core/listener/RouteSelectorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-22 17:02:26.000000 socket.d-2.4.11/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.099231 socket.d-2.4.11/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-20 10:08:08.000000 socket.d-2.4.11/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 02:50:04.000000 socket.d-2.4.11/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-20 10:46:19.000000 socket.d-2.4.11/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.105740 socket.d-2.4.11/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/stream/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.108488 socket.d-2.4.11/socketd/transport/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-19 01:32:01.000000 socket.d-2.4.11/socketd/transport/utils/AsyncUtils.py
--rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.109486 socket.d-2.4.11/socketd/transport/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.110376 socket.d-2.4.11/socketd/transport/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.112834 socket.d-2.4.11/socketd/utils/
--rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 02:24:24.000000 socket.d-2.4.11/socketd/utils/RunUtils.py
--rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-19 01:32:01.000000 socket.d-2.4.11/socketd/utils/StrUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 02:48:51.000000 socket.d-2.4.11/socketd/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.134703 socket.d-2.4.11/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4143 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6597 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.150803 socket.d-2.4.11/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3639 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2099 2024-04-22 09:42:19.000000 socket.d-2.4.11/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.156817 socket.d-2.4.11/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4297 2024-04-23 02:24:50.000000 socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.761115 socket.d-2.4.11.1/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-24 04:51:51.759890 socket.d-2.4.11.1/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.11.1/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-24 04:51:51.761554 socket.d-2.4.11.1/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-24 04:51:33.000000 socket.d-2.4.11.1/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.759267 socket.d-2.4.11.1/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     5224 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-24 04:51:51.000000 socket.d-2.4.11.1/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.697716 socket.d-2.4.11.1/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     2710 2024-04-24 03:29:26.000000 socket.d-2.4.11.1/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.700051 socket.d-2.4.11.1/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.702740 socket.d-2.4.11.1/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.704008 socket.d-2.4.11.1/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.704770 socket.d-2.4.11.1/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.711466 socket.d-2.4.11.1/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3609 2024-04-24 03:26:45.000000 socket.d-2.4.11.1/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6514 2024-04-24 03:33:21.000000 socket.d-2.4.11.1/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.11.1/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.721237 socket.d-2.4.11.1/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-24 03:33:21.000000 socket.d-2.4.11.1/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-24 03:33:21.000000 socket.d-2.4.11.1/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-24 04:28:16.000000 socket.d-2.4.11.1/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.723541 socket.d-2.4.11.1/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.726427 socket.d-2.4.11.1/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.730195 socket.d-2.4.11.1/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-24 03:33:21.000000 socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.735185 socket.d-2.4.11.1/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     7305 2024-04-24 03:34:35.000000 socket.d-2.4.11.1/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/impl/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)     7937 2024-04-24 03:33:21.000000 socket.d-2.4.11.1/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4625 2024-04-24 04:28:16.000000 socket.d-2.4.11.1/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.737684 socket.d-2.4.11.1/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/RouteSelector.py
+-rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/RouteSelectorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.739392 socket.d-2.4.11.1/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.741972 socket.d-2.4.11.1/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-24 04:17:01.000000 socket.d-2.4.11.1/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-24 03:00:26.000000 socket.d-2.4.11.1/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-24 03:32:44.000000 socket.d-2.4.11.1/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1068 2024-04-24 03:34:35.000000 socket.d-2.4.11.1/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.744704 socket.d-2.4.11.1/socketd/transport/stream/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     1862 2024-04-24 04:31:14.000000 socket.d-2.4.11.1/socketd/transport/stream/impl/RequestStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      734 2024-04-24 02:55:55.000000 socket.d-2.4.11.1/socketd/transport/stream/impl/SendStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     2391 2024-04-24 03:25:43.000000 socket.d-2.4.11.1/socketd/transport/stream/impl/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1279 2024-04-24 04:31:37.000000 socket.d-2.4.11.1/socketd/transport/stream/impl/SubscribeStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 01:56:25.000000 socket.d-2.4.11.1/socketd/transport/stream/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.746605 socket.d-2.4.11.1/socketd/transport/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/transport/utils/AsyncUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-24 04:13:24.000000 socket.d-2.4.11.1/socketd/transport/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.747241 socket.d-2.4.11.1/socketd/transport/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.747736 socket.d-2.4.11.1/socketd/transport/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd/transport/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.748719 socket.d-2.4.11.1/socketd/utils/
+-rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/utils/RunUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/utils/StrUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.752513 socket.d-2.4.11.1/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4143 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6597 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.756150 socket.d-2.4.11.1/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3639 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2099 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 04:51:51.758681 socket.d-2.4.11.1/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4297 2024-04-23 03:01:10.000000 socket.d-2.4.11.1/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.11.1/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.11/PKG-INFO` & `socket.d-2.4.11.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.11
+Version: 2.4.11.1
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.11/README.md` & `socket.d-2.4.11.1/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/setup.py` & `socket.d-2.4.11.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.11',
+    version='2.4.11.1',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru',
         'websockets'
```

### Comparing `socket.d-2.4.11/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.11.1/socket.d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.11
+Version: 2.4.11.1
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.11/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.11.1/socket.d.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -89,19 +89,23 @@
 socketd/transport/server/ServerBase.py
 socketd/transport/server/ServerConfig.py
 socketd/transport/server/ServerProvider.py
 socketd/transport/server/__init__.py
 socketd/transport/stream/RequestStream.py
 socketd/transport/stream/SendStream.py
 socketd/transport/stream/Stream.py
-socketd/transport/stream/StreamBase.py
 socketd/transport/stream/StreamManger.py
 socketd/transport/stream/StreamMangerDefault.py
 socketd/transport/stream/SubscribeStream.py
 socketd/transport/stream/__init__.py
+socketd/transport/stream/impl/RequestStreamImpl.py
+socketd/transport/stream/impl/SendStreamImpl.py
+socketd/transport/stream/impl/StreamBase.py
+socketd/transport/stream/impl/SubscribeStreamImpl.py
+socketd/transport/stream/impl/__init__.py
 socketd/transport/utils/AsyncUtils.py
 socketd/transport/utils/CompletableFuture.py
 socketd/transport/utils/__init__.py
 socketd/transport/utils/async_api/AtomicRefer.py
 socketd/transport/utils/async_api/__init__.py
 socketd/transport/utils/sync_api/AtomicRefer.py
 socketd/transport/utils/sync_api/__init__.py
```

### Comparing `socket.d-2.4.11/socketd/SocketD.py` & `socket.d-2.4.11.1/socketd/SocketD.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,73 +20,19 @@
 def protocol_version() -> str:
     return "1.0"
 
 
 client_factory_map: Dict[str, ClientProvider] = {}
 server_factory_map: Dict[str, ServerProvider] = {}
 
-def create_server(schemaOrConfig: str | ServerConfig) -> Server:
-    Asserts.assert_null("schemaOrConfig", schemaOrConfig)
-    config:ServerConfig
-
-    if isinstance(schemaOrConfig, str):
-        config = ServerConfig(schemaOrConfig)
-    else:
-        config = schemaOrConfig
-
-    server = create_server_or_null(config)
-
-    if server is None:
-        raise RuntimeError(f"No socketd server providers were found: {config.get_schema()}")
-    else:
-        return server
-
-def create_server_or_null(config: ServerConfig) -> Server:
-    factory = server_factory_map.get(config.get_schema())
-
-    if factory is None:
-        return None
-    else:
-        return factory.create_server(config)
-
-
-def create_client(urlOrConfig: str | ClientConfig) -> Client:
-    Asserts.assert_null("urlOrConfig", urlOrConfig)
-    config:ClientConfig
-
-    if isinstance(urlOrConfig, str):
-        config = ClientConfig(urlOrConfig)
-    else:
-        config = urlOrConfig
-
-    client = create_client_or_null(config)
-
-    if client is None:
-        raise RuntimeError(f"No socketd client providers were found: {config.get_schema()}")
-    else:
-        return client
-
-def create_client_or_null(config: ClientConfig) -> Client:
-    Asserts.assert_null("config", config)
-
-    factory = client_factory_map.get(config.get_schema())
-    if factory is None:
-        return None
-    else:
-        return factory.create_client(config)
-
-
-def create_cluster_client(*urls):
-    return ClusterClient(*urls)
-
-
 def load_factories(factories: list[ClientProvider | ServerProvider], factory_map: Dict[str, object]) -> None:
     for factory in factories:
         for schema in factory.schema():
             factory_map[schema] = factory
+
 def create_server(schemaOrConfig: str | ServerConfig) -> Server:
     Asserts.assert_null("schemaOrConfig", schemaOrConfig)
     config:ServerConfig
 
     if isinstance(schemaOrConfig, str):
         config = ServerConfig(schemaOrConfig)
     else:
@@ -120,24 +66,24 @@
     client = create_client_or_null(config)
 
     if client is None:
         raise RuntimeError(f"No socketd client providers were found: {config.get_schema()}")
     else:
         return client
 
-def create_client_or_null(config: ClientConfig) -> Client:
+def create_client_or_null(config: ClientConfig) -> Client | None:
     Asserts.assert_null("config", config)
 
     factory = client_factory_map.get(config.get_schema())
     if factory is None:
         return None
     else:
         return factory.create_client(config)
 
 
-def create_cluster_client(*urls):
+def create_cluster_client(*urls) -> Client:
     return ClusterClient(*urls)
 
 
 # Initialize the client and server factory maps
 load_factories([WsAioProvider(), TcpAioProvider()], server_factory_map)
 load_factories([WsAioProvider(), TcpAioProvider()], client_factory_map)
```

### Comparing `socket.d-2.4.11/socketd/broker/BrokerListener.py` & `socket.d-2.4.11.1/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.11.1/socketd/broker/BrokerListenerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/cluster/ClusterClient.py` & `socket.d-2.4.11.1/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.11.1/socketd/cluster/ClusterClientSession.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,28 +41,28 @@
             if session.is_closing():
                 return True
         return False
 
     def session_id(self) -> str:
         return self.__sessionId
 
-    async def send(self, event: str, content: Entity) -> SendStream:
+    def send(self, event: str, content: Entity) -> SendStream:
         sender = self.get_session_any(None)
 
-        return await sender.send(event, content)
+        return sender.send(event, content)
 
-    async def send_and_request(self, event: str, content: Entity, timeout: int) -> RequestStream:
+    def send_and_request(self, event: str, content: Entity, timeout: int) -> RequestStream:
         sender = self.get_session_any(None)
 
-        return await sender.send_and_request(event, content, timeout)
+        return sender.send_and_request(event, content, timeout)
 
-    async def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0) -> SubscribeStream:
+    def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0) -> SubscribeStream:
         sender = self.get_session_any(None)
 
-        return await sender.send_and_subscribe(event, content, timeout)
+        return sender.send_and_subscribe(event, content, timeout)
 
     async def preclose(self):
         for session in self.__sessionSet:
             try:
                 await session.preclose()
             except RuntimeError as e:
                 pass
```

### Comparing `socket.d-2.4.11/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.11.1/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/exception/SocketDExecption.py` & `socket.d-2.4.11.1/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/client/Client.py` & `socket.d-2.4.11.1/socketd/transport/client/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 
     # 监听
     @abstractmethod
     def listen(self, listener: Listener) -> Client: ...
 
     # 打开会话
     @abstractmethod
-    def open(self) -> Session | Future: ...
+    async def open(self) -> Session: ...
 
     # 打开会话或出异常（即要求第一次是连接成功的）
     @abstractmethod
-    def open_or_throw(self) -> Session | Future: ...
+    async def open_or_throw(self) -> Session: ...
 
 
 class ClientInternal(Client):
     @abstractmethod
     def get_connect_handler(self) -> ClientConnectHandler: ...
 
     @abstractmethod
```

### Comparing `socket.d-2.4.11/socketd/transport/client/ClientBase.py` & `socket.d-2.4.11.1/socketd/transport/client/ClientBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,16 @@
                 await clientChannel.close(code=Constants.CLOSE2008_OPEN_FAIL)
                 raise SocketDException(f"Socket.D client Connection failed {e}")
             else:
                 log.info(f"Socket.D client Connection failed: link={self.get_config().get_link_url()}")
 
         return clientChannel.get_session()
 
-    def open(self) -> Awaitable[Session]:
-        return self._open_do(False)
+    async def open(self) -> Session:
+        return await self._open_do(False)
 
-    def open_or_throw(self) -> Awaitable[Session]:
-        return self._open_do(True)
+    async def open_or_throw(self) -> Session:
+        return await self._open_do(True)
 
     @abstractmethod
     def create_connector(self):
         ...
```

### Comparing `socket.d-2.4.11/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.11.1/socketd/transport/client/ClientChannel.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from socketd.exception.SocketDExecption import SocketDException, SocketDChannelException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.impl.SessionDefault import SessionDefault
-from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
 from socketd.transport.core.impl.ChannelBase import ChannelBase
 from socketd.transport.client.ClientConnector import ClientConnector
 
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandlerDefault
 from socketd.transport.utils.sync_api.AtomicRefer import AtomicRefer
```

### Comparing `socket.d-2.4.11/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.11.1/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/client/ClientSession.py` & `socket.d-2.4.11.1/socketd/transport/client/ClientSession.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,28 +17,25 @@
         ...
 
     @abc.abstractmethod
     def session_id(self) -> str:
         ...
 
     @abc.abstractmethod
-    async def send(self, event: str, content: Entity) -> SendStream:
+    def send(self, event: str, content: Entity) -> SendStream:
         ...
 
     @abc.abstractmethod
-    async def send_and_request(self, event: str, content: Entity, timeout: int = 0) -> RequestStream:
+    def send_and_request(self, event: str, content: Entity, timeout: int = 0) -> RequestStream:
         ...
 
     @abc.abstractmethod
-    async def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0) -> SubscribeStream:
+    def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0) -> SubscribeStream:
         ...
 
-    async def close_starting(self):
-        self.preclose()
-
     @abc.abstractmethod
     async def preclose(self):
         ...
 
     @abc.abstractmethod
     async def close(self):
         ...
```

### Comparing `socket.d-2.4.11/socketd/transport/core/Asserts.py` & `socket.d-2.4.11.1/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Channel.py` & `socket.d-2.4.11.1/socketd/transport/core/Channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Session import Session
 from socketd.transport.core.Config import Config
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.Message import Message
 from abc import abstractmethod, ABC
 
-from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
 
 
 class Channel(ABC):
     @abstractmethod
     def get_attachment(self, name: str) -> Any:
         ...
```

### Comparing `socket.d-2.4.11/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.11.1/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.11.1/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.11.1/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Codec.py` & `socket.d-2.4.11.1/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Config.py` & `socket.d-2.4.11.1/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Costants.py` & `socket.d-2.4.11.1/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Entity.py` & `socket.d-2.4.11.1/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.11.1/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Flags.py` & `socket.d-2.4.11.1/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.11.1/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.11.1/socketd/transport/core/FragmentHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Callable
 
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.Message import MessageInternal
-from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
 from socketd.transport.core import Channel
 
 
 class FragmentHandler(ABC):
     """
     数据分片处理
     """
```

### Comparing `socket.d-2.4.11/socketd/transport/core/Frames.py` & `socket.d-2.4.11.1/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Message.py` & `socket.d-2.4.11.1/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Processor.py` & `socket.d-2.4.11.1/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/Session.py` & `socket.d-2.4.11.1/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.11.1/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.11.1/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.11.1/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/codec/CodecDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.11.1/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.11.1/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.11.1/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.Message import Message, MessageInternal
 from socketd.transport.core.entity.EntityDefault import EntityDefault
 from socketd.transport.core.FragmentAggregator import FragmentAggregator
 from socketd.transport.core.fragment.FragmentAggregatorDefault import FragmentAggregatorDefault
 from socketd.transport.core.FragmentHandler import FragmentHandler
-from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
 
 
 class FragmentHandlerBase(FragmentHandler, ABC):
 
     async def split_fragment(self, channel: Channel, stream: StreamInternal, message: MessageInternal, consumer: Callable):
         if message.data_size() > channel.get_config().get_fragment_size():
             fragment_total = message.data_size()  # channel.get_config().fragment_size
```

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from socketd.transport.core import Entity
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.ChannelSupporter import ChannelSupporter
 from socketd.transport.core.Message import MessageInternal, Message
 from socketd.transport.core.entity.MessageBuilder import MessageBuilder
 from socketd.transport.core.impl.LogConfig import log
-from socketd.transport.stream.Stream import Stream
-from socketd.transport.stream.StreamManger import StreamManger, StreamInternal
+from socketd.transport.stream.Stream import Stream, StreamInternal
+from socketd.transport.stream.StreamManger import StreamManger
 from socketd.transport.core.impl.ChannelBase import ChannelBase
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Session import Session
 from socketd.transport.core.impl.SessionDefault import SessionDefault
 from socketd.transport.core.Frame import Frame
```

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from socketd.transport.core.Processor import Processor
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.listener.SimpleListener import SimpleListener
-from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
 from socketd.utils.RunUtils import RunUtils
 
 
 class ProcessorDefault(Processor, ABC):
 
     def __init__(self):
         self.listener = SimpleListener()
```

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/impl/SessionDefault.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 from socketd.transport.stream.RequestStream import RequestStream
 from socketd.transport.stream.SendStream import SendStream
 
 from socketd.transport.stream.SubscribeStream import SubscribeStream
 
 from loguru import logger
 
+from socketd.transport.stream.impl.RequestStreamImpl import RequestStreamImpl
+from socketd.transport.stream.impl.SendStreamImpl import SendStreamImpl
+from socketd.transport.stream.impl.SubscribeStreamImpl import SubscribeStreamImpl
+from socketd.utils.RunUtils import RunUtils
+
 
 class SessionDefault(SessionBase):
 
     def __init__(self, channel: Channel):
         super().__init__(channel)
         self.__path_new = None
 
@@ -37,35 +42,35 @@
 
     def handshake(self) -> HandshakeDefault:
         return self._channel.get_handshake()
 
     async def send_ping(self):
         await self._channel.send_ping()
 
-    async def send(self, topic: str, content: Entity) -> SendStream:
+    def send(self, topic: str, content: Entity) -> SendStream:
         message = MessageBuilder().sid(self.generate_id()).event(topic).entity(content).build()
 
-        stream: SendStream = SendStream(message.sid())
-        await self._channel.send(Frame(Flags.Message, message), stream)
+        stream: SendStream = SendStreamImpl(message.sid())
+        RunUtils.taskTry(self._channel.send(Frame(Flags.Message, message), stream))
         return stream
 
-    async def send_and_request(self, event: str, content: Entity,
+    def send_and_request(self, event: str, content: Entity,
                                timeout: int = 100) -> RequestStream:
 
         if timeout < 100:
             timeout = self._channel.get_config().get_request_timeout() / 1000
         message = MessageBuilder().sid(self.generate_id()).event(event).entity(content).build()
-        stream = RequestStream(message.sid(), timeout)
-        await self._channel.send(Frame(Flags.Request, message), stream)
+        stream:RequestStream = RequestStreamImpl(message.sid(), timeout)
+        RunUtils.taskTry(self._channel.send(Frame(Flags.Request, message), stream))
         return stream
 
-    async def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0):
+    def send_and_subscribe(self, event: str, content: Entity, timeout: int = 0):
         message = MessageBuilder().sid(self.generate_id()).event(event).entity(content).build()
-        stream = SubscribeStream(message.sid(), timeout)
-        await self._channel.send(Frame(Flags.Subscribe, message), stream)
+        stream:SubscribeStream = SubscribeStreamImpl(message.sid(), timeout)
+        RunUtils.taskTry(self._channel.send(Frame(Flags.Subscribe, message), stream))
         return stream
 
     async def reply(self, from_msg: Message, content: Entity):
         message = MessageBuilder().sid(from_msg.sid()).event(from_msg.event()).entity(content).build()
 
         await self._channel.send(Frame(Flags.Reply, message), None)
```

### Comparing `socket.d-2.4.11/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.11.1/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.11.1/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/listener/PipelineListener.py` & `socket.d-2.4.11.1/socketd/transport/core/listener/PipelineListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/core/listener/RouteSelectorDefault.py` & `socket.d-2.4.11.1/socketd/transport/core/listener/RouteSelectorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/server/Server.py` & `socket.d-2.4.11.1/socketd/transport/server/Server.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/server/ServerBase.py` & `socket.d-2.4.11.1/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.11.1/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.11.1/socketd/transport/stream/impl/RequestStreamImpl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 import asyncio
 from typing import Callable
+
 from socketd.exception.SocketDExecption import SocketDTimeoutException, SocketDException
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Entity import Reply
-from socketd.transport.stream.StreamBase import StreamBase
+from socketd.transport.core.Message import MessageInternal
+from socketd.transport.stream.RequestStream import RequestStream
+from socketd.transport.stream.impl.StreamBase import StreamBase
 from socketd.transport.utils.CompletableFuture import CompletableFuture
 
 
-class RequestStream(StreamBase):
-
+class RequestStreamImpl(StreamBase, RequestStream):
     def __init__(self, sid: str, timeout: int):
         super().__init__(sid, Constants.DEMANDS_SINGLE, timeout)
-        self._future: CompletableFuture = CompletableFuture()
+        self.__future: CompletableFuture = CompletableFuture()
 
     def is_done(self):
-        return self._future.done()
+        return self.__future.done()
 
     def __await__(self):
         try:
-            return self._future.get(self.timeout())
+            return self.__future.get(self.timeout() / 1000.0)
         except asyncio.TimeoutError as _e:
-            raise SocketDTimeoutException(f"Request reply timeout>{self.timeout()}  sid={self.get_sid()}")
+            raise SocketDTimeoutException(f"Request reply timeout>{self.timeout()}  sid={self.sid()}")
         except Exception as _e:
-            raise SocketDException(f"Request failed, sid= sid={self.get_sid()} {str(_e)}")
+            raise SocketDException(f"Request failed, sid= sid={self.sid()} {str(_e)}")
 
-    async def await_result(self):
-        if self._future.done():
-            return self._future.get_result()
+    async def get(self) -> Reply:
+        if self.__future.done():
+            return self.__future.get_result()
         return await self.__await__()
 
-    async def on_reply(self, message: Reply):
-        return await self._future.set_result(message)
+    async def on_reply(self, reply: MessageInternal):
+        return await self.__future.set_result(reply)
 
-    def then_reply(self, onReply: Callable[[Reply], None]):
-        self._future.then_callback(onReply)
+    def then_reply(self, onReply: Callable[[MessageInternal], None]) -> RequestStream:
+        self.__future.then_callback(onReply)
+        return self
+
+    def then_error(self, onError: Callable[[Exception], None]) -> RequestStream:
+        super().then_error_do(onError)
+        return self
+
+    def then_progress(self, onProgress: Callable[[bool, int, int], None]) -> RequestStream:
+        super().then_progress_do(onProgress)
+        return self
```

### Comparing `socket.d-2.4.11/socketd/transport/stream/StreamBase.py` & `socket.d-2.4.11.1/socketd/transport/stream/impl/StreamBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 import asyncio
 from abc import ABC
 from typing import Callable, Optional
 
 from socketd.exception.SocketDExecption import SocketDTimeoutException
-from socketd.transport.stream.StreamManger import StreamInternal, StreamManger
+from socketd.transport.core.Message import MessageInternal
+from socketd.transport.stream.Stream import StreamInternal
+from socketd.transport.stream.StreamManger import StreamManger
 from socketd.transport.utils.CompletableFuture import CompletableFuture
 
 
 class StreamBase(StreamInternal, ABC):
     """流接收器基类"""
 
     def __init__(self, sid: str, demands: int, timeout: int):
-        self.__onError: Callable[[Exception], None] = None
         self.__sid = sid
         self.__timeout = timeout
         self.__demands = demands
+
+        self.__onError: Callable[[Exception], None] = None
         self.__doOnError: Callable[[Exception], None] = None
         self.__doOnProgress: Callable[[bool, int, int], None] = None
+
         self.__insuranceFuture: Optional[asyncio.Future] = None
 
-    def on_error(self, error: Exception):
-        if error:
-            self.__doOnError(error)
+    def sid(self) -> str:
+        return self.__sid
 
     def is_done(self):
         return True
 
-    def then_progress(self, on_progress: Callable[[bool, int, int], None]):
-        pass
-
-    def get_sid(self) -> str:
-        return self.__sid
-
-    def timeout(self):
-        return self.__timeout
-
-    def then_error(self, onError: Callable[[Exception], None]):
+    def then_error_do(self, onError: Callable[[Exception], None]):
         self.__onError = onError
 
+    def then_progress_do(self, onProgress: Callable[[bool, int, int], None]):
+        self.__doOnProgress = onProgress
+
     def demands(self) -> int:
         return self.__demands
 
+    def timeout(self):
+        return self.__timeout
+
+    # 保险开始（避免永久没有回调，造成内存不能释放）
     def insurance_start(self, streamManger: StreamManger, streamTimeout: float) -> None:
         if self.__insuranceFuture:
             return
 
         async def __insuranceFuture():
             await asyncio.sleep(streamTimeout)
             streamManger.remove_stream(self.__sid)
             self.on_error(SocketDTimeoutException(f"The stream response timeout, sid={self.__sid}"))
 
         self.__insuranceFuture = CompletableFuture(__insuranceFuture())
         asyncio.run_coroutine_threadsafe(self.__insuranceFuture.get(streamTimeout), asyncio.get_running_loop())
 
+    # 保险取消
     def insurance_cancel(self) -> None:
         if self.__insuranceFuture:
             self.__insuranceFuture.cancel()
 
+    def on_reply(self, reply:MessageInternal):
+        ...
+
+    def on_error(self, error: Exception):
+        if error:
+            self.__doOnError(error)
+
     def on_progress(self, is_send, val, max_val):
         if self.__doOnProgress:
             self.__doOnProgress(is_send, val, max_val)
+
+
+
```

### Comparing `socket.d-2.4.11/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.11.1/socketd/transport/stream/StreamMangerDefault.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
-from socketd.transport.stream.StreamManger import StreamManger, StreamInternal
+from socketd.transport.stream.Stream import StreamInternal
+from socketd.transport.stream.StreamManger import StreamManger
 
 logger = logging.getLogger(__name__)
 
 
 class StreamMangerDefault(StreamManger):
     def __init__(self, config):
         self.config = config
```

### Comparing `socket.d-2.4.11/socketd/transport/utils/AsyncUtils.py` & `socket.d-2.4.11.1/socketd/transport/utils/AsyncUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/utils/CompletableFuture.py` & `socket.d-2.4.11.1/socketd/transport/utils/CompletableFuture.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             loop = asyncio.get_running_loop()
         if _future and not asyncio.iscoroutine(_future):
             logger.warning("{name}对象不是协程对象", name=_future.__name__)
             return
         self._future: asyncio.Task = loop.create_task(_future) if _future else loop.create_future()
         self._lock = Lock()
 
-    def get(self, timeout):
+    def get(self, timeout:float):
         with self._lock:
             async def _get():
                 await asyncio.wait_for(self._future, timeout)
                 return self._future.result()
         return _get()
 
     def accept(self, result: T):
```

### Comparing `socket.d-2.4.11/socketd/transport/utils/async_api/AtomicRefer.py` & `socket.d-2.4.11.1/socketd/transport/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/transport/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.11.1/socketd/transport/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd/utils/StrUtils.py` & `socket.d-2.4.11.1/socketd/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TCPAIOServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.11.1/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.11.1/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/WsAioClient.py` & `socket.d-2.4.11.1/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.11.1/socketd_websocket/WsAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.11.1/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/WsAioServer.py` & `socket.d-2.4.11.1/socketd_websocket/WsAioServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.11.1/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.11.1/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.11.1/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.11.1/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files identical despite different names*

