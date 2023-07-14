# Comparing `tmp/nope_py-1.7.8rc2.tar.gz` & `tmp/nope_py-1.7.8rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nope_py-1.7.8rc2.tar", last modified: Fri Jul 14 22:08:16 2023, max compression
+gzip compressed data, was "nope_py-1.7.8rc3.tar", last modified: Fri Jul 14 22:27:18 2023, max compression
```

## Comparing `nope_py-1.7.8rc2.tar` & `nope_py-1.7.8rc3.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/
--rw-r--r--   0 martin    (1000) martin    (1001)     1062 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1001)     7557 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.793771 nope_py-1.7.8rc2/nope/
--rw-r--r--   0 martin    (1000) martin    (1001)      525 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.793771 nope_py-1.7.8rc2/nope/cli/
--rw-r--r--   0 martin    (1000) martin    (1001)      458 2023-07-14 16:52:13.000000 nope_py-1.7.8rc2/nope/cli/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      121 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/cli/__main__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2309 2023-07-14 17:45:33.000000 nope_py-1.7.8rc2/nope/cli/logo.py
--rw-r--r--   0 martin    (1000) martin    (1001)      729 2023-07-14 16:54:17.000000 nope_py-1.7.8rc2/nope/cli/main.py
--rw-r--r--   0 martin    (1000) martin    (1001)     9578 2023-07-14 22:06:47.000000 nope_py-1.7.8rc2/nope/cli/run.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4203 2023-07-14 22:06:14.000000 nope_py-1.7.8rc2/nope/cli/scan.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.793771 nope_py-1.7.8rc2/nope/communication/
--rw-r--r--   0 martin    (1000) martin    (1001)      158 2023-07-14 21:32:17.000000 nope_py-1.7.8rc2/nope/communication/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1111 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/abstractBridgePlugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1633 2023-07-14 21:36:02.000000 nope_py-1.7.8rc2/nope/communication/addLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)     5498 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/bridge.py
--rw-r--r--   0 martin    (1000) martin    (1001)      450 2023-07-14 21:36:59.000000 nope_py-1.7.8rc2/nope/communication/getLayer.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/communication/layers/
--rw-r--r--   0 martin    (1000) martin    (1001)     2522 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/layers/EventCommunicationInterface.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/layers/IoSocketClientLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)      196 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/layers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      872 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/communication/layers/abstractLayer.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6122 2023-07-14 17:51:17.000000 nope_py-1.7.8rc2/nope/communication/layers/mqttLayer.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/decorators/
--rw-r--r--   0 martin    (1000) martin    (1001)       82 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/decorators/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1285 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/decorators/classes.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/demo/
--rw-r--r--   0 martin    (1000) martin    (1001)       93 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/demo/instances/
--rw-r--r--   0 martin    (1000) martin    (1001)     1474 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/instances/DecoratedHelloWorld.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1461 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/instances/HelloWorld.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1212 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/instances/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/demo/plugins/
--rw-r--r--   0 martin    (1000) martin    (1001)      936 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/plugins/00-load-hello.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2514 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/plugins/01-dynamic.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2933 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/plugins/02-multiple.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3176 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/plugins/03-different-items.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1224 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/demo/plugins/04-fix.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/
--rw-r--r--   0 martin    (1000) martin    (1001)      355 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/baseServices/
--rw-r--r--   0 martin    (1000) martin    (1001)      909 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/baseServices/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2676 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/baseServices/connectivy.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/connectivityManager/
--rw-r--r--   0 martin    (1000) martin    (1001)       57 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/connectivityManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    12628 2023-07-14 16:31:06.000000 nope_py-1.7.8rc2/nope/dispatcher/connectivityManager/connectivityManager.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/core/
--rw-r--r--   0 martin    (1000) martin    (1001)      110 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/core/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4897 2023-07-14 17:45:31.000000 nope_py-1.7.8rc2/nope/dispatcher/core/nopeCore.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2103 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/getDispatcher.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/instanceManager/
--rw-r--r--   0 martin    (1000) martin    (1001)      106 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/instanceManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/instanceManager/assignmentChecker.py
--rw-r--r--   0 martin    (1000) martin    (1001)    38653 2023-07-14 21:08:55.000000 nope_py-1.7.8rc2/nope/dispatcher/instanceManager/instanceManager.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4289 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/nopeDispatcher.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/dispatcher/rpcManager/
--rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/rpcManager/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    23952 2023-07-14 17:45:32.000000 nope_py-1.7.8rc2/nope/dispatcher/rpcManager/rpcManager.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3200 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/dispatcher/rpcManager/selectors.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/eventEmitter/
--rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/eventEmitter/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6492 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/eventEmitter/nopeEventEmitter.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.797105 nope_py-1.7.8rc2/nope/helpers/
--rw-r--r--   0 martin    (1000) martin    (1001)     2457 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    15786 2023-07-14 18:38:50.000000 nope_py-1.7.8rc2/nope/helpers/asyncHelpers.py
--rw-r--r--   0 martin    (1000) martin    (1001)    12082 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/dictMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      695 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/dispatcherPathes.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4025 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/dottedDict.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4035 2023-07-14 17:45:29.000000 nope_py-1.7.8rc2/nope/helpers/emitter.py
--rw-r--r--   0 martin    (1000) martin    (1001)      805 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/files.py
--rw-r--r--   0 martin    (1000) martin    (1001)    11974 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/hashable.py
--rw-r--r--   0 martin    (1000) martin    (1001)      767 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/idMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      591 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/importing.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2732 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/jsonMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2316 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/listMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)    14217 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/objectMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     5206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/path.py
--rw-r--r--   0 martin    (1000) martin    (1001)    10488 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/pathMatchingMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)      610 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/prints.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1459 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/runtime.py
--rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/setMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     4807 2023-07-14 17:45:30.000000 nope_py-1.7.8rc2/nope/helpers/stringMethods.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1894 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/timers.py
--rw-r--r--   0 martin    (1000) martin    (1001)      119 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/helpers/timestamp.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/loader/
--rw-r--r--   0 martin    (1000) martin    (1001)      234 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/loader/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/loader/getPackageLoader.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2709 2023-07-14 21:44:22.000000 nope_py-1.7.8rc2/nope/loader/loadPackages.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6379 2023-07-14 16:41:06.000000 nope_py-1.7.8rc2/nope/loader/nopePackkageLoader.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/logger/
--rw-r--r--   0 martin    (1000) martin    (1001)       99 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/logger/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2436 2023-07-14 16:46:17.000000 nope_py-1.7.8rc2/nope/logger/logger.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/merging/
--rw-r--r--   0 martin    (1000) martin    (1001)       53 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/merging/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2293 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/merging/mergeData.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/modules/
--rw-r--r--   0 martin    (1000) martin    (1001)      206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/modules/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)    17745 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/modules/baseModule.py
--rw-r--r--   0 martin    (1000) martin    (1001)     7614 2023-07-14 17:59:08.000000 nope_py-1.7.8rc2/nope/modules/genericModule.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/observable/
--rw-r--r--   0 martin    (1000) martin    (1001)      151 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/observable/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3003 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/observable/nopeObservable.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/plugins/
--rw-r--r--   0 martin    (1000) martin    (1001)      125 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/plugins/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     6051 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/plugins/ack_messages.py
--rw-r--r--   0 martin    (1000) martin    (1001)      919 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/plugins/hello.py
--rw-r--r--   0 martin    (1000) martin    (1001)    21800 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/plugins/plugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)    16129 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/plugins/rpc_with_callbacks.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/pubSub/
--rw-r--r--   0 martin    (1000) martin    (1001)       94 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/pubSub/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3718 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/pubSub/nopeDataPubSubSystem.py
--rw-r--r--   0 martin    (1000) martin    (1001)    25149 2023-07-14 18:38:53.000000 nope_py-1.7.8rc2/nope/pubSub/nopePubSubSystem.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope/types/
--rw-r--r--   0 martin    (1000) martin    (1001)     3358 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/nope/types/__init__.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/nope_py.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1001)     3118 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1001)        1 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1001)       46 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/entry_points.txt
--rw-r--r--   0 martin    (1000) martin    (1001)       49 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1001)        5 2023-07-14 22:08:16.000000 nope_py-1.7.8rc2/nope_py.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1001)      103 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1001)     2520 2023-07-14 22:07:22.000000 nope_py-1.7.8rc2/setup.py
-drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:08:16.800438 nope_py-1.7.8rc2/test/
--rw-r--r--   0 martin    (1000) martin    (1001)     1427 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2053 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_communicator.py
--rw-r--r--   0 martin    (1000) martin    (1001)     2960 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_plugin.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1545 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_plugin_bridge.py
--rw-r--r--   0 martin    (1000) martin    (1001)     1396 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_plugin_rpc_callbacks.py
--rw-r--r--   0 martin    (1000) martin    (1001)      644 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_pub_sub.py
--rw-r--r--   0 martin    (1000) martin    (1001)     3128 2023-07-14 13:43:25.000000 nope_py-1.7.8rc2/test/test_rpc_manager.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/
+-rw-r--r--   0 martin    (1000) martin    (1001)     1062 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1001)     7557 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/
+-rw-r--r--   0 martin    (1000) martin    (1001)      525 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/cli/
+-rw-r--r--   0 martin    (1000) martin    (1001)      458 2023-07-14 16:52:13.000000 nope_py-1.7.8rc3/nope/cli/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      121 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/cli/__main__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2309 2023-07-14 17:45:33.000000 nope_py-1.7.8rc3/nope/cli/logo.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      729 2023-07-14 16:54:17.000000 nope_py-1.7.8rc3/nope/cli/main.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     9578 2023-07-14 22:06:47.000000 nope_py-1.7.8rc3/nope/cli/run.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4669 2023-07-14 22:26:41.000000 nope_py-1.7.8rc3/nope/cli/scan.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/communication/
+-rw-r--r--   0 martin    (1000) martin    (1001)      158 2023-07-14 21:32:17.000000 nope_py-1.7.8rc3/nope/communication/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1111 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/abstractBridgePlugin.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1633 2023-07-14 21:36:02.000000 nope_py-1.7.8rc3/nope/communication/addLayer.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     5498 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/bridge.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      450 2023-07-14 21:36:59.000000 nope_py-1.7.8rc3/nope/communication/getLayer.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/communication/layers/
+-rw-r--r--   0 martin    (1000) martin    (1001)     2522 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/EventCommunicationInterface.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/IoSocketClientLayer.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      196 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      872 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/communication/layers/abstractLayer.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     6122 2023-07-14 17:51:17.000000 nope_py-1.7.8rc3/nope/communication/layers/mqttLayer.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/decorators/
+-rw-r--r--   0 martin    (1000) martin    (1001)       82 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/decorators/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1285 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/decorators/classes.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/
+-rw-r--r--   0 martin    (1000) martin    (1001)       93 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/instances/
+-rw-r--r--   0 martin    (1000) martin    (1001)     1474 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/DecoratedHelloWorld.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1461 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/HelloWorld.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1212 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/instances/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/demo/plugins/
+-rw-r--r--   0 martin    (1000) martin    (1001)      936 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/00-load-hello.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2514 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/01-dynamic.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2933 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/02-multiple.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     3176 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/03-different-items.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1224 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/demo/plugins/04-fix.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/
+-rw-r--r--   0 martin    (1000) martin    (1001)      355 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/baseServices/
+-rw-r--r--   0 martin    (1000) martin    (1001)      909 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/baseServices/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2676 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/baseServices/connectivy.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/
+-rw-r--r--   0 martin    (1000) martin    (1001)       57 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    12628 2023-07-14 16:31:06.000000 nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/connectivityManager.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/core/
+-rw-r--r--   0 martin    (1000) martin    (1001)      110 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/core/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4897 2023-07-14 17:45:31.000000 nope_py-1.7.8rc3/nope/dispatcher/core/nopeCore.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2103 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/getDispatcher.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/
+-rw-r--r--   0 martin    (1000) martin    (1001)      106 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      896 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/assignmentChecker.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    38653 2023-07-14 21:08:55.000000 nope_py-1.7.8rc3/nope/dispatcher/instanceManager/instanceManager.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4289 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/nopeDispatcher.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/
+-rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    23952 2023-07-14 17:45:32.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/rpcManager.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     3200 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/dispatcher/rpcManager/selectors.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.236158 nope_py-1.7.8rc3/nope/eventEmitter/
+-rw-r--r--   0 martin    (1000) martin    (1001)       79 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/eventEmitter/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     6492 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/eventEmitter/nopeEventEmitter.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/helpers/
+-rw-r--r--   0 martin    (1000) martin    (1001)     2457 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    15786 2023-07-14 18:38:50.000000 nope_py-1.7.8rc3/nope/helpers/asyncHelpers.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    12082 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dictMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      695 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dispatcherPathes.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4025 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/dottedDict.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4035 2023-07-14 17:45:29.000000 nope_py-1.7.8rc3/nope/helpers/emitter.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      805 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/files.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    11974 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/hashable.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      767 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/idMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      591 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/importing.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2732 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/jsonMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2316 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/listMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    14217 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/objectMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     5206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/path.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    10488 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/pathMatchingMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      610 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/prints.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1459 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/runtime.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/setMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     4807 2023-07-14 17:45:30.000000 nope_py-1.7.8rc3/nope/helpers/stringMethods.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1894 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/timers.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      119 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/helpers/timestamp.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/loader/
+-rw-r--r--   0 martin    (1000) martin    (1001)      234 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/loader/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      748 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/loader/getPackageLoader.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2709 2023-07-14 21:44:22.000000 nope_py-1.7.8rc3/nope/loader/loadPackages.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     6379 2023-07-14 16:41:06.000000 nope_py-1.7.8rc3/nope/loader/nopePackkageLoader.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/logger/
+-rw-r--r--   0 martin    (1000) martin    (1001)       99 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/logger/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2436 2023-07-14 16:46:17.000000 nope_py-1.7.8rc3/nope/logger/logger.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/merging/
+-rw-r--r--   0 martin    (1000) martin    (1001)       53 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/merging/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2293 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/merging/mergeData.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/modules/
+-rw-r--r--   0 martin    (1000) martin    (1001)      206 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/modules/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    17745 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/modules/baseModule.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     7614 2023-07-14 17:59:08.000000 nope_py-1.7.8rc3/nope/modules/genericModule.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/observable/
+-rw-r--r--   0 martin    (1000) martin    (1001)      151 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/observable/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     3003 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/observable/nopeObservable.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/plugins/
+-rw-r--r--   0 martin    (1000) martin    (1001)      125 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     6051 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/ack_messages.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      919 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/hello.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    21800 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/plugin.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    16129 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/plugins/rpc_with_callbacks.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/pubSub/
+-rw-r--r--   0 martin    (1000) martin    (1001)       94 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/pubSub/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     3718 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/pubSub/nopeDataPubSubSystem.py
+-rw-r--r--   0 martin    (1000) martin    (1001)    25149 2023-07-14 18:38:53.000000 nope_py-1.7.8rc3/nope/pubSub/nopePubSubSystem.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope/types/
+-rw-r--r--   0 martin    (1000) martin    (1001)     3358 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/nope/types/__init__.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/nope_py.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1001)     8141 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1001)     3118 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1001)        1 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1001)       46 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/entry_points.txt
+-rw-r--r--   0 martin    (1000) martin    (1001)       49 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1001)        5 2023-07-14 22:27:18.000000 nope_py-1.7.8rc3/nope_py.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1001)      103 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1001)     2520 2023-07-14 22:27:13.000000 nope_py-1.7.8rc3/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1001)        0 2023-07-14 22:27:18.239491 nope_py-1.7.8rc3/test/
+-rw-r--r--   0 martin    (1000) martin    (1001)     1427 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2053 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_communicator.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     2960 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1545 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin_bridge.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     1396 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_plugin_rpc_callbacks.py
+-rw-r--r--   0 martin    (1000) martin    (1001)      644 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_pub_sub.py
+-rw-r--r--   0 martin    (1000) martin    (1001)     3128 2023-07-14 13:43:25.000000 nope_py-1.7.8rc3/test/test_rpc_manager.py
```

### Comparing `nope_py-1.7.8rc2/LICENSE` & `nope_py-1.7.8rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/PKG-INFO` & `nope_py-1.7.8rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope_py
-Version: 1.7.8rc2
+Version: 1.7.8rc3
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.7.8rc2/README.md` & `nope_py-1.7.8rc3/README.md`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/__init__.py` & `nope_py-1.7.8rc3/nope/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/cli/logo.py` & `nope_py-1.7.8rc3/nope/cli/logo.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/cli/main.py` & `nope_py-1.7.8rc3/nope/cli/main.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/cli/run.py` & `nope_py-1.7.8rc3/nope/cli/run.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/cli/scan.py` & `nope_py-1.7.8rc3/nope/cli/scan.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,21 +23,28 @@
     Returns:
         _type_: _description_
     """
 
     packages = []
 
     for root, directories, files in os.walk(path):
+        if "/venv/" in root:
+            continue
+
         for name in files:
             if name == "__init__.py":
                 # Determine the Path to the File.
                 pathToFile = os.path.join(root, name)
 
                 if absolute:
                     pathToFile = os.path.abspath(os.path.join(root, name))
+                else:
+                    pathToFile = os.path.relpath(pathToFile)
+
+                LOGGER.info(f"Checking file: '{pathToFile}'")
 
                 try:
                     # Dynamically load the File.
                     module = dynamicImport(
                         name, pathToFile)
 
                     # Add the Path:
@@ -48,23 +55,28 @@
                         dumps(
                             description,
                             parse_functions=False))
 
                     # Add it to the packages
                     packages.append(description)
                 except ModuleNotFoundError as E:
+                    LOGGER.error(f"Failed to load file. '{pathToFile}'")
                     LOGGER.error(formatException(E))
+                    pass
                 except ImportError as e:
                     if e.msg == "attempted relative import with no known parent package":
                         pass
                     else:
-                        print("Failed to load", pathToFile)
-                        print(formatException(e))
-                except AttributeError as E:
+                        pass
+                        LOGGER.error(f"Failed to load file. '{pathToFile}'")
+                        LOGGER.error(formatException(e))
+                except AttributeError as E:                    
+                    LOGGER.error(f"Failed to load file. '{pathToFile}'")
                     LOGGER.error(formatException(E))
+                    pass
                 except Exception as e:
                     LOGGER.error(f"Failed to load '{pathToFile}'")
                     LOGGER.error(formatException(e))
                     pass
 
     return packages
```

### Comparing `nope_py-1.7.8rc2/nope/communication/abstractBridgePlugin.py` & `nope_py-1.7.8rc3/nope/communication/abstractBridgePlugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/addLayer.py` & `nope_py-1.7.8rc3/nope/communication/addLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/bridge.py` & `nope_py-1.7.8rc3/nope/communication/bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/layers/EventCommunicationInterface.py` & `nope_py-1.7.8rc3/nope/communication/layers/EventCommunicationInterface.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/layers/IoSocketClientLayer.py` & `nope_py-1.7.8rc3/nope/communication/layers/IoSocketClientLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/layers/abstractLayer.py` & `nope_py-1.7.8rc3/nope/communication/layers/abstractLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/communication/layers/mqttLayer.py` & `nope_py-1.7.8rc3/nope/communication/layers/mqttLayer.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/decorators/classes.py` & `nope_py-1.7.8rc3/nope/decorators/classes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/instances/DecoratedHelloWorld.py` & `nope_py-1.7.8rc3/nope/demo/instances/DecoratedHelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/instances/HelloWorld.py` & `nope_py-1.7.8rc3/nope/demo/instances/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/instances/__init__.py` & `nope_py-1.7.8rc3/nope/demo/instances/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/plugins/00-load-hello.py` & `nope_py-1.7.8rc3/nope/demo/plugins/00-load-hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/plugins/01-dynamic.py` & `nope_py-1.7.8rc3/nope/demo/plugins/01-dynamic.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/plugins/02-multiple.py` & `nope_py-1.7.8rc3/nope/demo/plugins/02-multiple.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/plugins/03-different-items.py` & `nope_py-1.7.8rc3/nope/demo/plugins/03-different-items.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/demo/plugins/04-fix.py` & `nope_py-1.7.8rc3/nope/demo/plugins/04-fix.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/baseServices/__init__.py` & `nope_py-1.7.8rc3/nope/dispatcher/baseServices/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/baseServices/connectivy.py` & `nope_py-1.7.8rc3/nope/dispatcher/baseServices/connectivy.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/connectivityManager/connectivityManager.py` & `nope_py-1.7.8rc3/nope/dispatcher/connectivityManager/connectivityManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/core/nopeCore.py` & `nope_py-1.7.8rc3/nope/dispatcher/core/nopeCore.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/getDispatcher.py` & `nope_py-1.7.8rc3/nope/dispatcher/getDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/instanceManager/assignmentChecker.py` & `nope_py-1.7.8rc3/nope/dispatcher/instanceManager/assignmentChecker.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/instanceManager/instanceManager.py` & `nope_py-1.7.8rc3/nope/dispatcher/instanceManager/instanceManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/nopeDispatcher.py` & `nope_py-1.7.8rc3/nope/dispatcher/nopeDispatcher.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/rpcManager/rpcManager.py` & `nope_py-1.7.8rc3/nope/dispatcher/rpcManager/rpcManager.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/dispatcher/rpcManager/selectors.py` & `nope_py-1.7.8rc3/nope/dispatcher/rpcManager/selectors.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/eventEmitter/nopeEventEmitter.py` & `nope_py-1.7.8rc3/nope/eventEmitter/nopeEventEmitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/__init__.py` & `nope_py-1.7.8rc3/nope/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/asyncHelpers.py` & `nope_py-1.7.8rc3/nope/helpers/asyncHelpers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/dictMethods.py` & `nope_py-1.7.8rc3/nope/helpers/dictMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/dispatcherPathes.py` & `nope_py-1.7.8rc3/nope/helpers/dispatcherPathes.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/dottedDict.py` & `nope_py-1.7.8rc3/nope/helpers/dottedDict.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/emitter.py` & `nope_py-1.7.8rc3/nope/helpers/emitter.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/files.py` & `nope_py-1.7.8rc3/nope/helpers/files.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/hashable.py` & `nope_py-1.7.8rc3/nope/helpers/hashable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/idMethods.py` & `nope_py-1.7.8rc3/nope/helpers/idMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/importing.py` & `nope_py-1.7.8rc3/nope/helpers/importing.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/jsonMethods.py` & `nope_py-1.7.8rc3/nope/helpers/jsonMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/listMethods.py` & `nope_py-1.7.8rc3/nope/helpers/listMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/objectMethods.py` & `nope_py-1.7.8rc3/nope/helpers/objectMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/path.py` & `nope_py-1.7.8rc3/nope/helpers/path.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/pathMatchingMethods.py` & `nope_py-1.7.8rc3/nope/helpers/pathMatchingMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/prints.py` & `nope_py-1.7.8rc3/nope/helpers/prints.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/runtime.py` & `nope_py-1.7.8rc3/nope/helpers/runtime.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/setMethods.py` & `nope_py-1.7.8rc3/nope/helpers/setMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/stringMethods.py` & `nope_py-1.7.8rc3/nope/helpers/stringMethods.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/helpers/timers.py` & `nope_py-1.7.8rc3/nope/helpers/timers.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/loader/getPackageLoader.py` & `nope_py-1.7.8rc3/nope/loader/getPackageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/loader/loadPackages.py` & `nope_py-1.7.8rc3/nope/loader/loadPackages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/loader/nopePackkageLoader.py` & `nope_py-1.7.8rc3/nope/loader/nopePackkageLoader.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/logger/logger.py` & `nope_py-1.7.8rc3/nope/logger/logger.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/merging/mergeData.py` & `nope_py-1.7.8rc3/nope/merging/mergeData.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/modules/baseModule.py` & `nope_py-1.7.8rc3/nope/modules/baseModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/modules/genericModule.py` & `nope_py-1.7.8rc3/nope/modules/genericModule.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/observable/nopeObservable.py` & `nope_py-1.7.8rc3/nope/observable/nopeObservable.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/plugins/ack_messages.py` & `nope_py-1.7.8rc3/nope/plugins/ack_messages.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/plugins/hello.py` & `nope_py-1.7.8rc3/nope/plugins/hello.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/plugins/plugin.py` & `nope_py-1.7.8rc3/nope/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/plugins/rpc_with_callbacks.py` & `nope_py-1.7.8rc3/nope/plugins/rpc_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/pubSub/nopeDataPubSubSystem.py` & `nope_py-1.7.8rc3/nope/pubSub/nopeDataPubSubSystem.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/pubSub/nopePubSubSystem.py` & `nope_py-1.7.8rc3/nope/pubSub/nopePubSubSystem.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope/types/__init__.py` & `nope_py-1.7.8rc3/nope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/nope_py.egg-info/PKG-INFO` & `nope_py-1.7.8rc3/nope_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nope-py
-Version: 1.7.8rc2
+Version: 1.7.8rc3
 Summary: NOPE-Lib represents the No Programming Environment Library for python.
 Home-page: https://github.com/ZeMA-gGmbH/NoPE-PY.git
 Author: Martin Karkowski
 Author-email: m.karkowski@zema.de
 Maintainer: Martin Karkowski
 Maintainer-email: m.karkowski@zema.de
 Classifier: Operating System :: OS Independent
```

### Comparing `nope_py-1.7.8rc2/nope_py.egg-info/SOURCES.txt` & `nope_py-1.7.8rc3/nope_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/setup.py` & `nope_py-1.7.8rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     long_description = open("./README.md").read()
 except BaseException:
     long_description = """NOPE-Python Backend. A Generic Backend for Python"""
 
 if __name__ == "__main__":
     setup(name="nope_py",
-          version="1.7.8rc2",
+          version="1.7.8rc3",
           description="NOPE-Lib represents the No Programming Environment Library for python.",
           long_description=long_description,
           long_description_content_type="text/markdown",
           author="Martin Karkowski",
           author_email="m.karkowski@zema.de",
           maintainer="Martin Karkowski",
           maintainer_email="m.karkowski@zema.de",
```

### Comparing `nope_py-1.7.8rc2/test/test.py` & `nope_py-1.7.8rc3/test/test.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_communicator.py` & `nope_py-1.7.8rc3/test/test_communicator.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_plugin.py` & `nope_py-1.7.8rc3/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_plugin_bridge.py` & `nope_py-1.7.8rc3/test/test_plugin_bridge.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_plugin_rpc_callbacks.py` & `nope_py-1.7.8rc3/test/test_plugin_rpc_callbacks.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_pub_sub.py` & `nope_py-1.7.8rc3/test/test_pub_sub.py`

 * *Files identical despite different names*

### Comparing `nope_py-1.7.8rc2/test/test_rpc_manager.py` & `nope_py-1.7.8rc3/test/test_rpc_manager.py`

 * *Files identical despite different names*

