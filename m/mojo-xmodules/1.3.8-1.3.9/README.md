# Comparing `tmp/mojo_xmodules-1.3.8.tar.gz` & `tmp/mojo_xmodules-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_xmodules-1.3.8.tar", max compression
+gzip compressed data, was "mojo_xmodules-1.3.9.tar", max compression
```

## Comparing `mojo_xmodules-1.3.8.tar` & `mojo_xmodules-1.3.9.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:53:41.926735 mojo_xmodules-1.3.8/LICENSE.txt
--rw-r--r--   0        0        0      358 2024-01-26 02:53:41.926853 mojo_xmodules-1.3.8/README.rst
--rw-r--r--   0        0        0      976 2024-02-21 07:54:08.297780 mojo_xmodules-1.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928303 mojo_xmodules-1.3.8/source/packages/mojo/xmods/__init__.py
--rw-r--r--   0        0        0     7574 2024-01-26 02:53:41.928404 mojo_xmodules-1.3.8/source/packages/mojo/xmods/aspects.py
--rw-r--r--   0        0        0     1766 2024-02-10 20:07:06.396699 mojo_xmodules-1.3.8/source/packages/mojo/xmods/autoclean.py
--rw-r--r--   0        0        0     1181 2024-01-26 02:53:41.928472 mojo_xmodules-1.3.8/source/packages/mojo/xmods/compression.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928533 mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/__init__.py
--rw-r--r--   0        0        0      697 2024-01-26 02:53:41.928632 mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/enumerations.py
--rw-r--r--   0        0        0    11832 2024-01-26 02:53:41.928743 mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/eventedvariable.py
--rw-r--r--   0        0        0     8066 2024-01-26 02:53:41.928835 mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/eventedvariablesink.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928893 mojo_xmodules-1.3.8/source/packages/mojo/xmods/extension/__init__.py
--rw-r--r--   0        0        0     5304 2024-01-26 02:53:41.928973 mojo_xmodules-1.3.8/source/packages/mojo/xmods/extension/dynamic.py
--rw-r--r--   0        0        0     4468 2024-01-26 02:53:41.929060 mojo_xmodules-1.3.8/source/packages/mojo/xmods/fspath.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.929201 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/__init__.py
--rw-r--r--   0        0        0      767 2024-01-26 02:53:41.929303 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/basecoupling.py
--rw-r--r--   0        0        0     7894 2024-01-26 02:53:41.929392 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/integrationcoupling.py
--rw-r--r--   0        0        0     8164 2024-01-26 02:53:41.929494 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/scopecoupling.py
--rw-r--r--   0        0        0      555 2024-01-26 02:53:41.929558 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/validatorcoupling.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.929613 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/decorators/__init__.py
--rw-r--r--   0        0        0     8059 2024-01-26 02:53:41.929701 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/decorators/factory.py
--rw-r--r--   0        0        0     2661 2024-01-26 02:53:41.929774 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/decorators/injection.py
--rw-r--r--   0        0        0     5415 2024-01-26 02:53:41.929873 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectablegroup.py
--rw-r--r--   0        0        0     4409 2024-01-26 02:53:41.929953 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectableref.py
--rw-r--r--   0        0        0    13108 2024-02-12 14:25:06.390782 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectionregistry.py
--rw-r--r--   0        0        0      683 2024-01-26 02:53:41.930119 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/integrationsource.py
--rw-r--r--   0        0        0     2992 2024-01-26 02:53:41.930186 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/origination.py
--rw-r--r--   0        0        0     3144 2024-01-26 02:53:41.930256 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/parameterorigin.py
--rw-r--r--   0        0        0      409 2024-01-26 02:53:41.930332 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resourcelifespan.py
--rw-r--r--   0        0        0     6894 2024-01-26 02:53:41.930420 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resources.py
--rw-r--r--   0        0        0    20883 2024-01-26 02:53:41.930552 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resourcescope.py
--rw-r--r--   0        0        0      630 2024-01-26 02:53:41.930632 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resourcesource.py
--rw-r--r--   0        0        0      736 2024-01-26 02:53:41.930693 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/scopesource.py
--rw-r--r--   0        0        0     1575 2024-01-26 02:53:41.930762 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/sourcebase.py
--rw-r--r--   0        0        0      894 2024-01-26 02:53:41.930827 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/unknownsource.py
--rw-r--r--   0        0        0     2332 2024-01-26 02:53:41.930881 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/validatororigin.py
--rw-r--r--   0        0        0      583 2024-01-26 02:53:41.930979 mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/validatorsource.py
--rw-r--r--   0        0        0     1010 2024-01-26 02:53:41.931041 mojo_xmodules-1.3.8/source/packages/mojo/xmods/jsos.py
--rw-r--r--   0        0        0     7344 2024-01-26 02:53:41.931095 mojo_xmodules-1.3.8/source/packages/mojo/xmods/markers.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.931156 mojo_xmodules-1.3.8/source/packages/mojo/xmods/modeling/__init__.py
--rw-r--r--   0        0        0      928 2024-01-26 02:53:41.931235 mojo_xmodules-1.3.8/source/packages/mojo/xmods/modeling/extensionproperty.py
--rw-r--r--   0        0        0    19240 2024-01-26 02:53:41.931344 mojo_xmodules-1.3.8/source/packages/mojo/xmods/verification.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.931440 mojo_xmodules-1.3.8/source/packages/mojo/xmods/wrappers/__init__.py
--rw-r--r--   0        0        0     6322 2024-01-26 02:53:41.931619 mojo_xmodules-1.3.8/source/packages/mojo/xmods/wrappers/fsdict.py
--rw-r--r--   0        0        0     1395 2024-01-26 02:53:41.931709 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xclick.py
--rw-r--r--   0        0        0     1689 2024-01-26 02:53:41.931781 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xconvert.py
--rwxr-xr-x   0        0        0     2433 2024-01-26 02:53:41.931854 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xdatetime.py
--rw-r--r--   0        0        0     5114 2024-02-20 01:05:27.582170 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xdebugger.py
--rw-r--r--   0        0        0     6695 2024-01-26 02:53:41.932119 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xfeature.py
--rw-r--r--   0        0        0     5683 2024-01-26 02:53:41.932225 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xformatting.py
--rw-r--r--   0        0        0     2220 2024-01-26 02:53:41.932315 mojo_xmodules-1.3.8/source/packages/mojo/xmods/ximport.py
--rw-r--r--   0        0        0     2301 2024-01-26 02:53:41.932404 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xinspect.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.932471 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/__init__.py
--rw-r--r--   0        0        0    11503 2024-02-13 20:23:35.730674 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/foundations.py
--rw-r--r--   0        0        0      829 2024-02-10 20:40:13.978195 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/levels.py
--rw-r--r--   0        0        0    10490 2024-01-26 02:53:41.932834 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/scopemonitoring.py
--rw-r--r--   0        0        0        0 2024-01-26 02:53:41.932896 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xmultiprocessing/__init__.py
--rw-r--r--   0        0        0     3137 2024-01-26 02:53:41.932998 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xmultiprocessing/pipedprocess.py
--rw-r--r--   0        0        0     1535 2024-01-26 02:53:41.933069 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xpython.py
--rw-r--r--   0        0        0     1342 2024-02-21 07:55:47.668708 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xserialize.py
--rw-r--r--   0        0        0      544 2024-01-26 02:53:41.933177 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/__init__.py
--rw-r--r--   0        0        0     1632 2024-01-26 02:53:41.933251 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/lockscopes.py
--rw-r--r--   0        0        0     3275 2024-01-26 02:53:41.933335 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looper.py
--rw-r--r--   0        0        0     4914 2024-01-26 02:53:41.933406 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looperpool.py
--rw-r--r--   0        0        0     3550 2024-01-26 02:53:41.933475 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looperqueue.py
--rw-r--r--   0        0        0     5780 2024-01-26 02:53:41.933558 mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/readwritelock.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 mojo_xmodules-1.3.8/setup.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 mojo_xmodules-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:53:41.926735 mojo_xmodules-1.3.9/LICENSE.txt
+-rw-r--r--   0        0        0      358 2024-01-26 02:53:41.926853 mojo_xmodules-1.3.9/README.rst
+-rw-r--r--   0        0        0      976 2024-02-21 13:18:51.354804 mojo_xmodules-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928303 mojo_xmodules-1.3.9/source/packages/mojo/xmods/__init__.py
+-rw-r--r--   0        0        0     7574 2024-01-26 02:53:41.928404 mojo_xmodules-1.3.9/source/packages/mojo/xmods/aspects.py
+-rw-r--r--   0        0        0     1766 2024-02-10 20:07:06.396699 mojo_xmodules-1.3.9/source/packages/mojo/xmods/autoclean.py
+-rw-r--r--   0        0        0     1181 2024-01-26 02:53:41.928472 mojo_xmodules-1.3.9/source/packages/mojo/xmods/compression.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928533 mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/__init__.py
+-rw-r--r--   0        0        0      697 2024-01-26 02:53:41.928632 mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/enumerations.py
+-rw-r--r--   0        0        0    11832 2024-01-26 02:53:41.928743 mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/eventedvariable.py
+-rw-r--r--   0        0        0     8066 2024-01-26 02:53:41.928835 mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/eventedvariablesink.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.928893 mojo_xmodules-1.3.9/source/packages/mojo/xmods/extension/__init__.py
+-rw-r--r--   0        0        0     5304 2024-01-26 02:53:41.928973 mojo_xmodules-1.3.9/source/packages/mojo/xmods/extension/dynamic.py
+-rw-r--r--   0        0        0     4468 2024-01-26 02:53:41.929060 mojo_xmodules-1.3.9/source/packages/mojo/xmods/fspath.py
+-rw-r--r--   0        0        0     2439 2024-02-21 13:21:19.472031 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/constraints.py
+-rw-r--r--   0        0        0     3250 2024-02-21 13:23:59.247877 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/constraintscatalog.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.929201 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/__init__.py
+-rw-r--r--   0        0        0      767 2024-01-26 02:53:41.929303 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/basecoupling.py
+-rw-r--r--   0        0        0     7894 2024-01-26 02:53:41.929392 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/integrationcoupling.py
+-rw-r--r--   0        0        0     8164 2024-01-26 02:53:41.929494 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/scopecoupling.py
+-rw-r--r--   0        0        0      555 2024-01-26 02:53:41.929558 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/validatorcoupling.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.929613 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/decorators/__init__.py
+-rw-r--r--   0        0        0     8059 2024-01-26 02:53:41.929701 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/decorators/factory.py
+-rw-r--r--   0        0        0     2661 2024-01-26 02:53:41.929774 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/decorators/injection.py
+-rw-r--r--   0        0        0     5415 2024-01-26 02:53:41.929873 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectablegroup.py
+-rw-r--r--   0        0        0     4409 2024-01-26 02:53:41.929953 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectableref.py
+-rw-r--r--   0        0        0    13108 2024-02-12 14:25:06.390782 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectionregistry.py
+-rw-r--r--   0        0        0      683 2024-01-26 02:53:41.930119 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/integrationsource.py
+-rw-r--r--   0        0        0     2992 2024-01-26 02:53:41.930186 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/origination.py
+-rw-r--r--   0        0        0     3144 2024-01-26 02:53:41.930256 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/parameterorigin.py
+-rw-r--r--   0        0        0      409 2024-01-26 02:53:41.930332 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resourcelifespan.py
+-rw-r--r--   0        0        0     6894 2024-01-26 02:53:41.930420 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resources.py
+-rw-r--r--   0        0        0    20883 2024-01-26 02:53:41.930552 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resourcescope.py
+-rw-r--r--   0        0        0      630 2024-01-26 02:53:41.930632 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resourcesource.py
+-rw-r--r--   0        0        0      736 2024-01-26 02:53:41.930693 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/scopesource.py
+-rw-r--r--   0        0        0     1575 2024-01-26 02:53:41.930762 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/sourcebase.py
+-rw-r--r--   0        0        0      894 2024-01-26 02:53:41.930827 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/unknownsource.py
+-rw-r--r--   0        0        0     2332 2024-01-26 02:53:41.930881 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/validatororigin.py
+-rw-r--r--   0        0        0      583 2024-01-26 02:53:41.930979 mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/validatorsource.py
+-rw-r--r--   0        0        0     1010 2024-01-26 02:53:41.931041 mojo_xmodules-1.3.9/source/packages/mojo/xmods/jsos.py
+-rw-r--r--   0        0        0     7344 2024-01-26 02:53:41.931095 mojo_xmodules-1.3.9/source/packages/mojo/xmods/markers.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.931156 mojo_xmodules-1.3.9/source/packages/mojo/xmods/modeling/__init__.py
+-rw-r--r--   0        0        0      928 2024-01-26 02:53:41.931235 mojo_xmodules-1.3.9/source/packages/mojo/xmods/modeling/extensionproperty.py
+-rw-r--r--   0        0        0    19240 2024-01-26 02:53:41.931344 mojo_xmodules-1.3.9/source/packages/mojo/xmods/verification.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.931440 mojo_xmodules-1.3.9/source/packages/mojo/xmods/wrappers/__init__.py
+-rw-r--r--   0        0        0     6322 2024-01-26 02:53:41.931619 mojo_xmodules-1.3.9/source/packages/mojo/xmods/wrappers/fsdict.py
+-rw-r--r--   0        0        0     1395 2024-01-26 02:53:41.931709 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xclick.py
+-rw-r--r--   0        0        0     1689 2024-01-26 02:53:41.931781 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xconvert.py
+-rwxr-xr-x   0        0        0     2433 2024-01-26 02:53:41.931854 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xdatetime.py
+-rw-r--r--   0        0        0     5114 2024-02-20 01:05:27.582170 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xdebugger.py
+-rw-r--r--   0        0        0     6695 2024-01-26 02:53:41.932119 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xfeature.py
+-rw-r--r--   0        0        0     5683 2024-01-26 02:53:41.932225 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xformatting.py
+-rw-r--r--   0        0        0     2220 2024-01-26 02:53:41.932315 mojo_xmodules-1.3.9/source/packages/mojo/xmods/ximport.py
+-rw-r--r--   0        0        0     2301 2024-01-26 02:53:41.932404 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xinspect.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.932471 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/__init__.py
+-rw-r--r--   0        0        0    11503 2024-02-13 20:23:35.730674 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/foundations.py
+-rw-r--r--   0        0        0      829 2024-02-10 20:40:13.978195 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/levels.py
+-rw-r--r--   0        0        0    10490 2024-01-26 02:53:41.932834 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/scopemonitoring.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:41.932896 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xmultiprocessing/__init__.py
+-rw-r--r--   0        0        0     3137 2024-01-26 02:53:41.932998 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xmultiprocessing/pipedprocess.py
+-rw-r--r--   0        0        0     1535 2024-01-26 02:53:41.933069 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xpython.py
+-rw-r--r--   0        0        0     1342 2024-02-21 07:55:47.668708 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xserialize.py
+-rw-r--r--   0        0        0      544 2024-01-26 02:53:41.933177 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/__init__.py
+-rw-r--r--   0        0        0     1632 2024-01-26 02:53:41.933251 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/lockscopes.py
+-rw-r--r--   0        0        0     3275 2024-01-26 02:53:41.933335 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looper.py
+-rw-r--r--   0        0        0     4914 2024-01-26 02:53:41.933406 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looperpool.py
+-rw-r--r--   0        0        0     3550 2024-01-26 02:53:41.933475 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looperqueue.py
+-rw-r--r--   0        0        0     5780 2024-01-26 02:53:41.933558 mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/readwritelock.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 mojo_xmodules-1.3.9/setup.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 mojo_xmodules-1.3.9/PKG-INFO
```

### Comparing `mojo_xmodules-1.3.8/LICENSE.txt` & `mojo_xmodules-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/pyproject.toml` & `mojo_xmodules-1.3.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-xmodules"
 description = "Automation Mojo X-Modules"
-version = "1.3.8"
+version = "1.3.9"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/aspects.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/aspects.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/autoclean.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/autoclean.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/compression.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/compression.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/enumerations.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/enumerations.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/eventedvariable.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/eventedvariable.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/eventing/eventedvariablesink.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/eventing/eventedvariablesink.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/extension/dynamic.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/extension/dynamic.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/fspath.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/fspath.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/basecoupling.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/basecoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/integrationcoupling.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/integrationcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/scopecoupling.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/scopecoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/coupling/validatorcoupling.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/coupling/validatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/decorators/factory.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/decorators/factory.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/decorators/injection.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/decorators/injection.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectablegroup.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectablegroup.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectableref.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectableref.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/injectionregistry.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/injectionregistry.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/integrationsource.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/integrationsource.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/origination.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/origination.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/parameterorigin.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/parameterorigin.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resources.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resources.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resourcescope.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resourcescope.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/resourcesource.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/resourcesource.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/scopesource.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/scopesource.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/sourcebase.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/sourcebase.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/unknownsource.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/unknownsource.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/validatororigin.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/validatororigin.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/injection/validatorsource.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/injection/validatorsource.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/jsos.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/jsos.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/markers.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/markers.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/modeling/extensionproperty.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/modeling/extensionproperty.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/verification.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/verification.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/wrappers/fsdict.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/wrappers/fsdict.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xclick.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xclick.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xconvert.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xconvert.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xdatetime.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xdatetime.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xdebugger.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xdebugger.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xfeature.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xfeature.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xformatting.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xformatting.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/ximport.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/ximport.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xinspect.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xinspect.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/foundations.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/foundations.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/levels.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/levels.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xlogging/scopemonitoring.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xlogging/scopemonitoring.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xmultiprocessing/pipedprocess.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xmultiprocessing/pipedprocess.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xpython.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xpython.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xserialize.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xserialize.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/__init__.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/lockscopes.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/lockscopes.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looper.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looper.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looperpool.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looperpool.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/looperqueue.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/looperqueue.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/source/packages/mojo/xmods/xthreading/readwritelock.py` & `mojo_xmodules-1.3.9/source/packages/mojo/xmods/xthreading/readwritelock.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-1.3.8/setup.py` & `mojo_xmodules-1.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'mojo-errors>=1.3.0,<1.4.0',
  'mojo-interfaces>=1.3.1,<1.4.0',
  'mojo-waiting>=1.3.0,<1.4.0',
  'paramiko>=3.1.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'mojo-xmodules',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'Automation Mojo X-Modules',
     'long_description': '\n=========================================\nAutomation Mojo X-Modules (mojo-xmodules)\n=========================================\n\nThis package contains helper modules that extend the function of standard python modules.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`_\n- `Coding Standards <userguide/10-00-coding-standards.rst>`_\n\n\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_xmodules-1.3.8/PKG-INFO` & `mojo_xmodules-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-xmodules
-Version: 1.3.8
+Version: 1.3.9
 Summary: Automation Mojo X-Modules
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python,support
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
```

