# Comparing `tmp/socket.d-2.4.11.2.tar.gz` & `tmp/socket.d-2.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.11.2.tar", last modified: Wed Apr 24 05:12:50 2024, max compression
+gzip compressed data, was "socket.d-2.4.12.tar", last modified: Thu Apr 25 05:57:11 2024, max compression
```

## Comparing `socket.d-2.4.11.2.tar` & `socket.d-2.4.12.tar`

### file list

```diff
@@ -1,158 +1,156 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.111307 socket.d-2.4.11.2/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-24 05:12:50.110352 socket.d-2.4.11.2/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.11.2/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-24 05:12:50.111480 socket.d-2.4.11.2/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-24 05:12:31.000000 socket.d-2.4.11.2/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.109304 socket.d-2.4.11.2/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     5224 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-24 05:12:49.000000 socket.d-2.4.11.2/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.024176 socket.d-2.4.11.2/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     2710 2024-04-24 03:29:26.000000 socket.d-2.4.11.2/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.026576 socket.d-2.4.11.2/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.028369 socket.d-2.4.11.2/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.029340 socket.d-2.4.11.2/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.029706 socket.d-2.4.11.2/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.040679 socket.d-2.4.11.2/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3609 2024-04-24 03:26:45.000000 socket.d-2.4.11.2/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6514 2024-04-24 03:33:21.000000 socket.d-2.4.11.2/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.11.2/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.053548 socket.d-2.4.11.2/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-24 03:33:21.000000 socket.d-2.4.11.2/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-24 03:33:21.000000 socket.d-2.4.11.2/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-24 04:28:16.000000 socket.d-2.4.11.2/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.057907 socket.d-2.4.11.2/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.060495 socket.d-2.4.11.2/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.063139 socket.d-2.4.11.2/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-24 03:33:21.000000 socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.068789 socket.d-2.4.11.2/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     7305 2024-04-24 03:34:35.000000 socket.d-2.4.11.2/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/impl/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)     7937 2024-04-24 03:33:21.000000 socket.d-2.4.11.2/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4625 2024-04-24 04:28:16.000000 socket.d-2.4.11.2/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.077412 socket.d-2.4.11.2/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/RouteSelector.py
--rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/RouteSelectorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.079939 socket.d-2.4.11.2/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.084112 socket.d-2.4.11.2/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)      876 2024-04-24 05:00:55.000000 socket.d-2.4.11.2/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-24 03:00:26.000000 socket.d-2.4.11.2/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-24 03:32:44.000000 socket.d-2.4.11.2/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1068 2024-04-24 03:34:35.000000 socket.d-2.4.11.2/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.086538 socket.d-2.4.11.2/socketd/transport/stream/impl/
--rw-r--r--   0 noear      (501) staff       (20)     1865 2024-04-24 05:01:03.000000 socket.d-2.4.11.2/socketd/transport/stream/impl/RequestStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      734 2024-04-24 02:55:55.000000 socket.d-2.4.11.2/socketd/transport/stream/impl/SendStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     2391 2024-04-24 03:25:43.000000 socket.d-2.4.11.2/socketd/transport/stream/impl/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1279 2024-04-24 04:31:37.000000 socket.d-2.4.11.2/socketd/transport/stream/impl/SubscribeStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 01:56:25.000000 socket.d-2.4.11.2/socketd/transport/stream/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.089213 socket.d-2.4.11.2/socketd/transport/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/transport/utils/AsyncUtils.py
--rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-24 04:13:24.000000 socket.d-2.4.11.2/socketd/transport/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.090806 socket.d-2.4.11.2/socketd/transport/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.092139 socket.d-2.4.11.2/socketd/transport/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd/transport/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.094568 socket.d-2.4.11.2/socketd/utils/
--rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/utils/RunUtils.py
--rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/utils/StrUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.100785 socket.d-2.4.11.2/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4143 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6597 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.103433 socket.d-2.4.11.2/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3639 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2099 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-24 05:12:50.107360 socket.d-2.4.11.2/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4297 2024-04-23 03:01:10.000000 socket.d-2.4.11.2/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.11.2/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.194645 socket.d-2.4.12/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-25 05:57:11.193563 socket.d-2.4.12/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.12/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-25 05:57:11.194954 socket.d-2.4.12/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-25 05:32:39.000000 socket.d-2.4.12/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.192385 socket.d-2.4.12/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     5114 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-25 05:57:11.000000 socket.d-2.4.12/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.111688 socket.d-2.4.12/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     2710 2024-04-25 05:32:39.000000 socket.d-2.4.12/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.112958 socket.d-2.4.12/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.115033 socket.d-2.4.12/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.115813 socket.d-2.4.12/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.116080 socket.d-2.4.12/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.128797 socket.d-2.4.12/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3584 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6490 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.144586 socket.d-2.4.12/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.147704 socket.d-2.4.12/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.151225 socket.d-2.4.12/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.152976 socket.d-2.4.12/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-24 03:33:21.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.156451 socket.d-2.4.12/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     7281 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6565 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     8216 2024-04-25 04:57:58.000000 socket.d-2.4.12/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4625 2024-04-24 04:28:16.000000 socket.d-2.4.12/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.160571 socket.d-2.4.12/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/RouteSelector.py
+-rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/RouteSelectorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.162205 socket.d-2.4.12/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.169510 socket.d-2.4.12/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)      876 2024-04-24 05:00:55.000000 socket.d-2.4.12/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-24 03:00:26.000000 socket.d-2.4.12/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-24 03:32:44.000000 socket.d-2.4.12/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1068 2024-04-24 03:34:35.000000 socket.d-2.4.12/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-24 03:25:43.000000 socket.d-2.4.12/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.174044 socket.d-2.4.12/socketd/transport/stream/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     1855 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/transport/stream/impl/RequestStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      734 2024-04-24 02:55:55.000000 socket.d-2.4.12/socketd/transport/stream/impl/SendStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     2381 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/transport/stream/impl/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1279 2024-04-24 04:31:37.000000 socket.d-2.4.12/socketd/transport/stream/impl/SubscribeStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 01:56:25.000000 socket.d-2.4.12/socketd/transport/stream/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.178882 socket.d-2.4.12/socketd/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/AsyncUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)     1977 2024-04-24 09:22:27.000000 socket.d-2.4.12/socketd/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/RunUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/StrUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.12/socketd/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.179927 socket.d-2.4.12/socketd/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 09:21:46.000000 socket.d-2.4.12/socketd/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.181578 socket.d-2.4.12/socketd/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-24 09:21:55.000000 socket.d-2.4.12/socketd/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.186057 socket.d-2.4.12/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4119 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6563 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.188449 socket.d-2.4.12/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3615 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2085 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-25 05:57:11.191752 socket.d-2.4.12/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     5966 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4283 2024-04-25 04:54:27.000000 socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.12/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.11.2/PKG-INFO` & `socket.d-2.4.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.11.2
+Version: 2.4.12
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.11.2/README.md` & `socket.d-2.4.12/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/setup.py` & `socket.d-2.4.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.11.2',
+    version='2.4.12',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru',
         'websockets'
```

### Comparing `socket.d-2.4.11.2/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.12/socket.d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.11.2
+Version: 2.4.12
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.11.2/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.12/socket.d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 socketd/transport/core/fragment/FragmentHandlerBase.py
 socketd/transport/core/fragment/FragmentHandlerDefault.py
 socketd/transport/core/fragment/FragmentHolder.py
 socketd/transport/core/fragment/__init__.py
 socketd/transport/core/impl/ChannelBase.py
 socketd/transport/core/impl/ChannelDefault.py
 socketd/transport/core/impl/ConfigBase.py
-socketd/transport/core/impl/LogConfig.py
 socketd/transport/core/impl/ProcessorDefault.py
 socketd/transport/core/impl/SessionBase.py
 socketd/transport/core/impl/SessionDefault.py
 socketd/transport/core/impl/__init__.py
 socketd/transport/core/listener/EventListener.py
 socketd/transport/core/listener/PathListener.py
 socketd/transport/core/listener/PipelineListener.py
@@ -98,24 +97,24 @@
 socketd/transport/stream/SubscribeStream.py
 socketd/transport/stream/__init__.py
 socketd/transport/stream/impl/RequestStreamImpl.py
 socketd/transport/stream/impl/SendStreamImpl.py
 socketd/transport/stream/impl/StreamBase.py
 socketd/transport/stream/impl/SubscribeStreamImpl.py
 socketd/transport/stream/impl/__init__.py
-socketd/transport/utils/AsyncUtils.py
-socketd/transport/utils/CompletableFuture.py
-socketd/transport/utils/__init__.py
-socketd/transport/utils/async_api/AtomicRefer.py
-socketd/transport/utils/async_api/__init__.py
-socketd/transport/utils/sync_api/AtomicRefer.py
-socketd/transport/utils/sync_api/__init__.py
+socketd/utils/AsyncUtils.py
+socketd/utils/CompletableFuture.py
+socketd/utils/LogConfig.py
 socketd/utils/RunUtils.py
 socketd/utils/StrUtils.py
 socketd/utils/__init__.py
+socketd/utils/async_api/AtomicRefer.py
+socketd/utils/async_api/__init__.py
+socketd/utils/sync_api/AtomicRefer.py
+socketd/utils/sync_api/__init__.py
 socketd_aio_tcp/TCPAIOServer.py
 socketd_aio_tcp/TCPStreamIO.py
 socketd_aio_tcp/TcpAIOChannelAssistant.py
 socketd_aio_tcp/TcpAioClient.py
 socketd_aio_tcp/TcpAioClientConnector.py
 socketd_aio_tcp/TcpAioProvider.py
 socketd_aio_tcp/__init__.py
```

### Comparing `socket.d-2.4.11.2/socketd/SocketD.py` & `socket.d-2.4.12/socketd/SocketD.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from socketd.transport.server.ServerProvider import ServerProvider
 
 from socketd_websocket.WsAioProvider import WsAioProvider
 from socketd_aio_tcp.TcpAioProvider import TcpAioProvider
 
 
 def version() -> str:
-    return "2.4.11"
+    return "2.4.12"
 
 
 def protocol_version() -> str:
     return "1.0"
 
 
 client_factory_map: Dict[str, ClientProvider] = {}
```

### Comparing `socket.d-2.4.11.2/socketd/broker/BrokerListener.py` & `socket.d-2.4.12/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.12/socketd/broker/BrokerListenerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/cluster/ClusterClient.py` & `socket.d-2.4.12/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.12/socketd/cluster/ClusterClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.12/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/exception/SocketDExecption.py` & `socket.d-2.4.12/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/client/Client.py` & `socket.d-2.4.12/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/client/ClientBase.py` & `socket.d-2.4.12/socketd/transport/client/ClientBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABC, abstractmethod
-from typing import Awaitable, Optional
+from typing import Optional
 
 from socketd.exception.SocketDExecption import SocketDException
 from socketd.transport.client.Client import ClientInternal, Client
 from socketd.transport.client.ClientChannel import ClientChannel
 from socketd.transport.client.ClientConfigHandler import ClientConfigHandler
 from socketd.transport.client.ClientConnectHandler import ClientConnectHandler, ClientConnectHandlerDefault
 from socketd.transport.client.ClientConnector import ClientConnector
 from socketd.transport.core.ChannelAssistant import ChannelAssistant
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Session import Session
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandler
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.core.impl.ProcessorDefault import ProcessorDefault
 from socketd.transport.client.ClientConfig import ClientConfig
 
 
 
 class ClientBase(ClientInternal, ABC):
```

### Comparing `socket.d-2.4.11.2/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.12/socketd/transport/client/ClientChannel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from asyncio import Future
 
 from socketd.exception.SocketDExecption import SocketDException, SocketDChannelException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.Costants import Constants
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.core.impl.SessionDefault import SessionDefault
 from socketd.transport.stream.Stream import StreamInternal
 from socketd.transport.core.impl.ChannelBase import ChannelBase
 from socketd.transport.client.ClientConnector import ClientConnector
 
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandlerDefault
-from socketd.transport.utils.sync_api.AtomicRefer import AtomicRefer
+from socketd.utils.sync_api.AtomicRefer import AtomicRefer
 
 
 class ClientChannel(ChannelBase):
     def __init__(self, client: ClientInternal, connector: ClientConnector):
         super().__init__(connector.get_config())
         self.__client = client
         self.__connector: ClientConnector = connector
```

### Comparing `socket.d-2.4.11.2/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.12/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/client/ClientSession.py` & `socket.d-2.4.12/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Asserts.py` & `socket.d-2.4.12/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Channel.py` & `socket.d-2.4.12/socketd/transport/core/Channel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.12/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.12/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.12/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Codec.py` & `socket.d-2.4.12/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Config.py` & `socket.d-2.4.12/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Costants.py` & `socket.d-2.4.12/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Entity.py` & `socket.d-2.4.12/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.12/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Flags.py` & `socket.d-2.4.12/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.12/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.12/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Frames.py` & `socket.d-2.4.12/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.12/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Message.py` & `socket.d-2.4.12/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Processor.py` & `socket.d-2.4.12/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/Session.py` & `socket.d-2.4.12/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.12/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.12/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.12/socketd/transport/core/codec/CodecDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.12/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.12/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.12/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.12/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.12/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.12/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.12/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.12/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 from socketd.transport.core import Entity
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.ChannelSupporter import ChannelSupporter
 from socketd.transport.core.Message import MessageInternal, Message
 from socketd.transport.core.entity.MessageBuilder import MessageBuilder
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.stream.Stream import Stream, StreamInternal
 from socketd.transport.stream.StreamManger import StreamManger
 from socketd.transport.core.impl.ChannelBase import ChannelBase
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Session import Session
 from socketd.transport.core.impl.SessionDefault import SessionDefault
 from socketd.transport.core.Frame import Frame
-from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.CompletableFuture import CompletableFuture
 from socketd.utils.RunUtils import RunUtils
 
 S = TypeVar("S")
 
 
 class ChannelDefault(ChannelBase, ChannelInternal):
```

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.12/socketd/transport/core/impl/ConfigBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from socketd.transport.core.Config import Config
 from socketd.transport.core.Codec import Codec
 from socketd.transport.core.IdGenerator import IdGenerator, GuidGenerator
 from socketd.transport.core.codec.CodecDefault import CodecDefault
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.fragment.FragmentHandlerDefault import FragmentHandlerDefault
 
-from socketd.transport.core.impl.LogConfig import logger
+from socketd.utils.LogConfig import logger
 from socketd.transport.stream.StreamManger import StreamManger
 from socketd.transport.stream.StreamMangerDefault import StreamMangerDefault
 
 
 class ConfigBase(Config, ABC):
 
     def __init__(self, clientMode: bool):
```

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.12/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Processor import Processor
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Frame import Frame
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.core.listener.SimpleListener import SimpleListener
 from socketd.transport.stream.Stream import StreamInternal
 from socketd.utils.RunUtils import RunUtils
 
 
 class ProcessorDefault(Processor, ABC):
 
@@ -167,17 +167,23 @@
         if channel.is_closed() <= Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
             RunUtils.taskTry(self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION))
 
     async def on_close_internal(self, channel: ChannelInternal, code: int):
         await channel.close(code)
 
     def on_error(self, channel: ChannelInternal, error):
-        RunUtils.taskTry(self.listener.on_error(channel.get_session(), error))
+        RunUtils.taskTry(self.on_error_internal(channel, error))
+
+    async def on_error_internal(self, channel: ChannelInternal, error):
+        try:
+            await RunUtils.waitTry(self.listener.on_error(channel.get_session(), error))
+        except Exception as e:
+            log.warning("{} channel listener onError error", channel.get_config().get_role_name(), e)
 
     def do_close_notice(self, channel: ChannelInternal):
-         RunUtils.taskTry(self.do_close_notice_internal(channel))
+        RunUtils.taskTry(self.do_close_notice_internal(channel))
 
     async def do_close_notice_internal(self, channel: ChannelInternal):
         try:
             await RunUtils.waitTry(self.listener.on_close(channel.get_session()))
         except Exception as e:
             self.on_error(channel, e)
```

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.12/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.12/socketd/transport/core/impl/SessionDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.12/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.12/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/listener/PipelineListener.py` & `socket.d-2.4.12/socketd/transport/core/listener/PipelineListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/core/listener/RouteSelectorDefault.py` & `socket.d-2.4.12/socketd/transport/core/listener/RouteSelectorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/server/Server.py` & `socket.d-2.4.12/socketd/transport/server/Server.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/server/ServerBase.py` & `socket.d-2.4.12/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.12/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.12/socketd/transport/stream/RequestStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/SendStream.py` & `socket.d-2.4.12/socketd/transport/stream/SendStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/Stream.py` & `socket.d-2.4.12/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.12/socketd/transport/stream/StreamMangerDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.12/socketd/transport/stream/SubscribeStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/impl/RequestStreamImpl.py` & `socket.d-2.4.12/socketd/transport/stream/impl/RequestStreamImpl.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from socketd.exception.SocketDExecption import SocketDTimeoutException, SocketDException
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Entity import Reply
 from socketd.transport.core.Message import MessageInternal
 from socketd.transport.stream.RequestStream import RequestStream
 from socketd.transport.stream.impl.StreamBase import StreamBase
-from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.CompletableFuture import CompletableFuture
 
 
 class RequestStreamImpl(StreamBase, RequestStream):
     def __init__(self, sid: str, timeout: int):
         super().__init__(sid, Constants.DEMANDS_SINGLE, timeout)
         self.__future: CompletableFuture = CompletableFuture()
```

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/impl/SendStreamImpl.py` & `socket.d-2.4.12/socketd/transport/stream/impl/SendStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/impl/StreamBase.py` & `socket.d-2.4.12/socketd/transport/stream/impl/StreamBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import ABC
 from typing import Callable, Optional
 
 from socketd.exception.SocketDExecption import SocketDTimeoutException
 from socketd.transport.core.Message import MessageInternal
 from socketd.transport.stream.Stream import StreamInternal
 from socketd.transport.stream.StreamManger import StreamManger
-from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.CompletableFuture import CompletableFuture
 
 
 class StreamBase(StreamInternal, ABC):
     """流接收器基类"""
 
     def __init__(self, sid: str, demands: int, timeout: int):
         self.__sid = sid
```

### Comparing `socket.d-2.4.11.2/socketd/transport/stream/impl/SubscribeStreamImpl.py` & `socket.d-2.4.12/socketd/transport/stream/impl/SubscribeStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/utils/AsyncUtils.py` & `socket.d-2.4.12/socketd/utils/AsyncUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/utils/CompletableFuture.py` & `socket.d-2.4.12/socketd/utils/CompletableFuture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import functools
 from threading import Lock
-from typing import Generic, TypeVar, Callable, Union, Coroutine
+from typing import Generic, TypeVar, Callable
 
 from loguru import logger
 
 T = TypeVar('T')
 
 
 class CompletableFuture(Generic[T]):
```

### Comparing `socket.d-2.4.11.2/socketd/transport/utils/async_api/AtomicRefer.py` & `socket.d-2.4.12/socketd/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/transport/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.12/socketd/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd/utils/StrUtils.py` & `socket.d-2.4.12/socketd/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.12/socketd_aio_tcp/TCPAIOServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from socketd.exception.SocketDExecption import SocketDTimeoutException
 from socketd.transport.core.ChannelSupporter import ChannelSupporter
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.server.ServerBase import ServerBase
 from socketd.transport.server.ServerConfig import ServerConfig
 
-from socketd.transport.utils.async_api.AtomicRefer import AtomicRefer
+from socketd.utils.async_api.AtomicRefer import AtomicRefer
 from .TCPStreamIO import TCPStreamIO
 
 from .TcpAIOChannelAssistant import TcpAIOChannelAssistant
 
 
 class TCPAIOServer(ServerBase, ChannelSupporter):
```

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.12/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.12/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.12/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.12/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from socketd.exception.SocketDExecption import SocketDTimeoutException, SocketDConnectionException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.client.ClientConnectorBase import ClientConnectorBase
 from socketd.transport.client.ClientHandshakeResult import ClientHandshakeResult
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
-from socketd.transport.core.impl.LogConfig import log
-from socketd.transport.utils.AsyncUtils import AsyncUtils
-from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.LogConfig import log
+from socketd.utils.AsyncUtils import AsyncUtils
+from socketd.utils.CompletableFuture import CompletableFuture
 
 from socketd_aio_tcp.TCPStreamIO import TCPStreamIO
 
 
 class TcpAioClientConnector(ClientConnectorBase):
 
     def __init__(self, client: ClientInternal):
```

### Comparing `socket.d-2.4.11.2/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.12/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.12/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/WsAioClient.py` & `socket.d-2.4.12/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.12/socketd_websocket/WsAioClientConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from websockets.client import WebSocketClientProtocol
 
 from socketd.exception.SocketDExecption import SocketDTimeoutException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.client.ClientHandshakeResult import ClientHandshakeResult
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.Costants import Constants
-from socketd.transport.core.impl.LogConfig import log, logger
+from socketd.utils.LogConfig import log, logger
 from socketd.transport.client.ClientConnectorBase import ClientConnectorBase
-from socketd.transport.utils.AsyncUtils import AsyncUtils
+from socketd.utils.AsyncUtils import AsyncUtils
 from socketd_websocket.impl.AIOConnect import AIOConnect
 from socketd_websocket.impl.AIOWebSocketClientImpl import AIOWebSocketClientImpl
 
 
 class WsAioClientConnector(ClientConnectorBase):
     def __init__(self, client: ClientInternal):
         self._top: Optional[asyncio.Future] = None
```

### Comparing `socket.d-2.4.11.2/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.12/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/WsAioServer.py` & `socket.d-2.4.12/socketd_websocket/WsAioServer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from socketd.transport.core.Costants import Constants
 from socketd.transport.server.ServerBase import ServerBase
 from socketd_websocket.WsAioChannelAssistant import WsAioChannelAssistant
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd_websocket.impl.AIOServe import AIOServe
 from socketd_websocket.impl.AIOWebSocketServerImpl import AIOWebSocketServerImpl
 
-from socketd.transport.core.impl.LogConfig import logger, log
+from socketd.utils.LogConfig import logger, log
 
 
 class WsAioServer(ServerBase):
 
     def __init__(self, config: ServerConfig):
         super().__init__(config, WsAioChannelAssistant(config))
         self._server: Optional[Serve] = None
```

### Comparing `socket.d-2.4.11.2/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.12/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.12/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.11.2/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import Optional, Sequence, List
 from loguru import logger
 from websockets.extensions import ClientExtensionFactory
 from websockets.uri import WebSocketURI
 
 from socketd.exception.SocketDExecption import SocketDConnectionException
 from socketd.transport.client.ClientHandshakeResult import ClientHandshakeResult
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
 from websockets import WebSocketClientProtocol, Origin, Subprotocol, HeadersLike, ConnectionClosedOK
 
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.Frame import Frame
-from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.CompletableFuture import CompletableFuture
 from socketd_websocket import WsAioClient
 
 
 class AIOWebSocketClientImpl(WebSocketClientProtocol):
     def __init__(self, client: WsAioClient, message_loop, *args, **kwargs):
         WebSocketClientProtocol.__init__(self, *args, **kwargs)
         self.status_state = Flags.Unknown
```

### Comparing `socket.d-2.4.11.2/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.12/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from websockets import ConnectionClosedOK
 from websockets.frames import Opcode
 from websockets.server import WebSocketServer, WebSocketServerProtocol
 
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.ChannelInternal import ChannelInternal
-from socketd.transport.core.impl.LogConfig import log
+from socketd.utils.LogConfig import log
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.Frame import Frame
 
 
 class AIOWebSocketServerImpl(WebSocketServerProtocol):
```

