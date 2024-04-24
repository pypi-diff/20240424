# Comparing `tmp/jddbusdebugger-3.0.tar.gz` & `tmp/jddbusdebugger-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jddbusdebugger-3.0.tar", last modified: Sun Apr 21 15:11:43 2024, max compression
+gzip compressed data, was "jddbusdebugger-3.1.tar", last modified: Wed Apr 24 17:40:11 2024, max compression
```

## Comparing `jddbusdebugger-3.0.tar` & `jddbusdebugger-3.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2870 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/BuildBackend.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    35087 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)      243 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/MANIFEST.in
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4936 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3792 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/README.md
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/
--rw-r--r--   0 jakob     (1000) jakob     (1000)       60 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Constants.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1828 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Environment.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1622 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Functions.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)   125260 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/Icon.png
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1446 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)       26 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/__main__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/core/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      299 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/Languages.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3416 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/MacroManager.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1501 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/Settings.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/core/__init__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.305544 jddbusdebugger-3.0/jdDBusDebugger/data/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      176 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/data/changelog.html
--rw-r--r--   0 jakob     (1000) jakob     (1000)       39 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/data/translators.json
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.308877 jddbusdebugger-3.0/jdDBusDebugger/gui/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1777 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/AboutDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    22871 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/CentralWidget.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2262 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/ConnectDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1499 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/EmitSignalDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1489 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/GenerateScriptDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    10948 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/MainWindow.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6124 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/ManageMacrosDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    10541 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/MonitorWindow.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3074 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/SettingsDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      939 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/WelcomeDialog.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.312210 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2798 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArgumentInput.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3443 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArrayInput.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      865 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BrowseButton.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1859 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BytearrayInput.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5770 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/DictInput.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4679 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/InputHandler.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2512 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5103 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/StructInput.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1509 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/VariantEdit.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/__init__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.312210 jddbusdebugger-3.0/jdDBusDebugger/translations/
--rw-r--r--   0 jakob     (1000) jakob     (1000)    46119 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts
--rw-r--r--   0 jakob     (1000) jakob     (1000)    46050 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.315544 jddbusdebugger-3.0/jdDBusDebugger/types/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1991 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Connection.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     7053 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/DBusType.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4171 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/DBusValue.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      460 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/EnumHelper.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1687 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Interface.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2583 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Macro.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1294 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Method.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2111 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Property.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3129 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Service.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)      553 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/Signal.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/__init__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.315544 jddbusdebugger-3.0/jdDBusDebugger/types/actions/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      567 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/ActionBase.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2732 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/CallAction.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1709 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/EmitAction.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2906 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/PropertyAction.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1602 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/SignalAction.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)        0 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/types/actions/__init__.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/jdDBusDebugger/ui/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3982 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/AboutDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3888 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/CentralWidget.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2634 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/ConnectDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2450 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/EmitSignalDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2223 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/GenerateScriptDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5662 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/MainWindow.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1780 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/ManageMacrosDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5102 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/MonitorWindow.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3062 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/SettingsDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)     3253 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/ui/WelcomeDialog.ui
--rw-r--r--   0 jakob     (1000) jakob     (1000)        4 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/jdDBusDebugger/version.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/jdDBusDebugger.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4936 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     2611 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       51 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/entry_points.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       19 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       15 2024-04-21 15:11:43.000000 jddbusdebugger-3.0/jdDBusDebugger.egg-info/top_level.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1410 2024-04-21 13:02:28.000000 jddbusdebugger-3.0/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2024-04-21 15:11:43.318877 jddbusdebugger-3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35087 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4936 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3792 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.891229 jddbusdebugger-3.1/jdDBusDebugger/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/Constants.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/Functions.py
+-rw-r--r--   0 root         (0) root         (0)   125260 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/Icon.png
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.891229 jddbusdebugger-3.1/jdDBusDebugger/core/
+-rw-r--r--   0 root         (0) root         (0)      299 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/core/Languages.py
+-rw-r--r--   0 root         (0) root         (0)     3416 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/core/MacroManager.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/core/Settings.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.891229 jddbusdebugger-3.1/jdDBusDebugger/data/
+-rw-r--r--   0 root         (0) root         (0)      375 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/data/changelog.html
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/data/translators.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.895229 jddbusdebugger-3.1/jdDBusDebugger/gui/
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)    22871 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/CentralWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/ConnectDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/EmitSignalDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/GenerateScriptDialog.py
+-rw-r--r--   0 root         (0) root         (0)    10948 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)     6124 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/ManageMacrosDialog.py
+-rw-r--r--   0 root         (0) root         (0)    11455 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/MonitorWindow.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/WelcomeDialog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.895229 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/ArgumentInput.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/ArrayInput.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/BrowseButton.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/BytearrayInput.py
+-rw-r--r--   0 root         (0) root         (0)     5770 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/DictInput.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/InputHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py
+-rw-r--r--   0 root         (0) root         (0)     5103 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/StructInput.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/VariantEdit.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.895229 jddbusdebugger-3.1/jdDBusDebugger/translations/
+-rw-r--r--   0 root         (0) root         (0)    46385 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_de.ts
+-rw-r--r--   0 root         (0) root         (0)    46316 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_nl.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.895229 jddbusdebugger-3.1/jdDBusDebugger/types/
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Connection.py
+-rw-r--r--   0 root         (0) root         (0)     7053 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/DBusType.py
+-rw-r--r--   0 root         (0) root         (0)     4171 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/DBusValue.py
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/EnumHelper.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Interface.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Macro.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Method.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Property.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Service.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/Signal.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/jdDBusDebugger/types/actions/
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/ActionBase.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/CallAction.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/EmitAction.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/PropertyAction.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/SignalAction.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/types/actions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/jdDBusDebugger/ui/
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     3888 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/CentralWidget.ui
+-rw-r--r--   0 root         (0) root         (0)     2634 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/ConnectDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/EmitSignalDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/GenerateScriptDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5662 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/ManageMacrosDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     5102 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/MonitorWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/ui/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/jdDBusDebugger/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/jdDBusDebugger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4936 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 17:40:11.000000 jddbusdebugger-3.1/jdDBusDebugger.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1410 2024-04-24 17:39:33.000000 jddbusdebugger-3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 17:40:11.899229 jddbusdebugger-3.1/setup.cfg
```

### Comparing `jddbusdebugger-3.0/BuildBackend.py` & `jddbusdebugger-3.1/BuildBackend.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/LICENSE` & `jddbusdebugger-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/PKG-INFO` & `jddbusdebugger-3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdDBusDebugger
-Version: 3.0
+Version: 3.1
 Summary: An advanced D-Bus Debugger
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDBusDebugger
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDBusDebugger/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdDBusDebugger
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `jddbusdebugger-3.0/README.md` & `jddbusdebugger-3.1/README.md`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/Environment.py` & `jddbusdebugger-3.1/jdDBusDebugger/Environment.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/Functions.py` & `jddbusdebugger-3.1/jdDBusDebugger/Functions.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/Icon.png` & `jddbusdebugger-3.1/jdDBusDebugger/Icon.png`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/__init__.py` & `jddbusdebugger-3.1/jdDBusDebugger/__init__.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/core/MacroManager.py` & `jddbusdebugger-3.1/jdDBusDebugger/core/MacroManager.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/core/Settings.py` & `jddbusdebugger-3.1/jdDBusDebugger/core/Settings.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/AboutDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/CentralWidget.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/CentralWidget.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/ConnectDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/ConnectDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/EmitSignalDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/EmitSignalDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/GenerateScriptDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/GenerateScriptDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/MainWindow.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/ManageMacrosDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/ManageMacrosDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/MonitorWindow.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/MonitorWindow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from PyQt6.QtGui import QCloseEvent, QStandardItemModel, QStandardItem, QIcon
 from PyQt6.QtCore import QObject, QThread, QCoreApplication, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QStyle, QApplication, QMessageBox
-from PyQt6.QtGui import QCloseEvent, QStandardItemModel, QStandardItem, QIcon
-from PyQt6.QtDBus import QDBusMessage
 from ..ui_compiled.MonitorWindow import Ui_MonitorWindow
+from PyQt6.QtDBus import QDBusMessage
 from typing import TYPE_CHECKING
 import jeepney.io.blocking
 import dataclasses
 import jeepney
 import copy
+import sys
 
 
 if TYPE_CHECKING:
     from ..types.Connection import Connection
     from .MainWindow import MainWindow
 
 
@@ -76,16 +77,19 @@
         row.append(QStandardItem(self._body))
 
         return row
 
 
 class MonitorWorker(QObject):
     new_message = pyqtSignal(_Message)
+    error_message = pyqtSignal(str)
 
     def setup(self, connection: "Connection") -> str | None:
+        self._parent_connection = connection
+
         match connection.connection_type:
             case "session":
                 self._connection = jeepney.io.blocking.open_dbus_connection(bus="SESSION")
             case "system":
                 self._connection = jeepney.io.blocking.open_dbus_connection(bus="SYSTEM")
             case "custom":
                 self._connection = jeepney.io.blocking.open_dbus_connection(bus=connection.connection.name())
@@ -107,16 +111,30 @@
         self._message_filter = message_filter
 
     def close_thread(self) -> None:
         self._exit = True
 
     def run(self) -> None:
         self._exit = False
+
         while True:
-            msg = _Message(self._connection.receive())
+            if self._exit:
+                return
+
+            try:
+                msg = _Message(self._connection.receive())
+            except ConnectionResetError:
+                error_message = self.setup(self._parent_connection)
+                if error_message is not None:
+                    self.error_message.emit(error_message)
+                    return
+                continue
+            except Exception as ex:
+                print(ex, file=sys.stderr)
+                continue
 
             if self._exit:
                 return
 
             if msg.check_message_filter(self._message_filter):
                 self.new_message.emit(msg)
 
@@ -191,14 +209,22 @@
     def _update_message_filter(self) -> None:
         self._worker.set_message_filter(self._get_message_filter())
 
     def _new_message(self, msg: _Message) -> None:
         self._model.appendRow(msg.get_row())
         self.table_view.scrollToBottom()
 
+    def _error_message(self, error_message: str) -> None:
+        QMessageBox.critical(
+            self,
+            QCoreApplication.translate("MonitorWindow", "Error"),
+            QCoreApplication.translate("MonitorWindow", "Lost monitor session") + "<br><br>" + error_message,
+        )
+        self.close()
+
     def _start(self) -> None:
         self._thread = QThread()
         self._worker = MonitorWorker()
 
         self._worker.moveToThread(self._thread)
         self._worker.set_message_filter(self._get_message_filter())
 
@@ -223,14 +249,15 @@
             )
             return
 
         self._worker.set_message_filter(self._get_message_filter())
 
         self._thread.started.connect(self._worker.run)
         self._worker.new_message.connect(self._new_message)
+        self._worker.error_message.connect(self._error_message)
 
         self._thread.start()
 
         match connection.connection_type:
             case "session":
                 self.setWindowTitle(QCoreApplication.translate("MonitorWindow", "Monitor Session"))
             case "system":
```

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/SettingsDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/WelcomeDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArgumentInput.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/ArgumentInput.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/ArrayInput.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/ArrayInput.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BrowseButton.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/BrowseButton.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/BytearrayInput.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/BytearrayInput.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/DictInput.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/DictInput.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/InputHandler.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/InputHandler.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/SingleValueInputDialog.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/StructInput.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/StructInput.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/gui/types_input/VariantEdit.py` & `jddbusdebugger-3.1/jdDBusDebugger/gui/types_input/VariantEdit.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts` & `jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_de.ts`

 * *Files 0% similar despite different names*

#### Comparing `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_de.ts` & `jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_de.ts`

```diff
@@ -112,14 +112,63 @@
       <source>File</source>
       <translation>Datei</translation>
     </message>
   </context>
   <context>
     <name>CentralWidget</name>
     <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Services</source>
+      <translation>Services</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Search</source>
+      <translation>Suche</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Name</source>
+      <translation>Name</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Activatable</source>
+      <translation>Aktivierbar</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>PID</source>
+      <translation>PID</translation>
+    </message>
+    <message>
+      <location filename="../gui/CentralWidget.py" line="296"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Refresh</source>
+      <translation>Neu laden</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Objects</source>
+      <translation>Objekte</translation>
+    </message>
+    <message>
+      <location filename="../gui/CentralWidget.py" line="349"/>
+      <location filename="../gui/CentralWidget.py" line="305"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Add object path</source>
+      <translation>Objektpfad hinzufügen</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
       <location filename="../gui/CentralWidget.py" line="42"/>
       <source>Call</source>
       <translation>Aufrufen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="73"/>
       <source>Get value</source>
@@ -173,28 +222,14 @@
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="285"/>
       <source>Copy</source>
       <translation>Kopieren</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="296"/>
-      <source>Refresh</source>
-      <translation>Neu laden</translation>
-    </message>
-    <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="349"/>
-      <location filename="../gui/CentralWidget.py" line="305"/>
-      <source>Add object path</source>
-      <translation>Objektpfad hinzufügen</translation>
-    </message>
-    <message>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>If this service has a object path that is not found trough introspection, you cann add it here</source>
       <translation>Wenn der Service einen Objektpfad besitzt, der nciht gefunden wurde, kannst du ihn hier hinzufügen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>Path not loaded</source>
@@ -281,52 +316,52 @@
       <translation>Service {{service}} wurde nicht gefunden</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="499"/>
       <source>Interface {{interface}} was not found on {{path}}</source>
       <translation>Interface {{interface}} wurde auf {{path}} nicht gefunden</translation>
     </message>
+  </context>
+  <context>
+    <name>ConnectDialog</name>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Services</source>
-      <translation>Services</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Connect</source>
+      <translation>Verbinde</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Search</source>
-      <translation>Suche</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>You can connect here with your custom D-Bus address</source>
+      <translation>Du kannst dich hier mit einer eigenen D-Bus Adresse verbinden</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Name</source>
-      <translation>Name</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Name:</source>
+      <translation>Name:</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Activatable</source>
-      <translation>Aktivierbar</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Address:</source>
+      <translation>Adresse:</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>PID</source>
-      <translation>PID</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Auto connect on startup</source>
+      <translation>Beim Starten automatisch verbinden</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Objects</source>
-      <translation>Objekte</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>OK</source>
+      <translation>OK</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Clear</source>
-      <translation>Löschen</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Cancel</source>
+      <translation>Abbrechen</translation>
     </message>
-  </context>
-  <context>
-    <name>ConnectDialog</name>
     <message>
       <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>Name not set</source>
       <translation>Name nicht angegeben</translation>
     </message>
     <message>
       <location filename="../gui/ConnectDialog.py" line="34"/>
@@ -349,49 +384,14 @@
       <translation>Ungültige Adresse</translation>
     </message>
     <message>
       <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Could not connect to {{address}}</source>
       <translation>Konnte keine Verbindung mit {{address}} herstellen</translation>
     </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Connect</source>
-      <translation>Verbinde</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>You can connect here with your custom D-Bus address</source>
-      <translation>Du kannst dich hier mit einer eigenen D-Bus Adresse verbinden</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Name:</source>
-      <translation>Name:</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Address:</source>
-      <translation>Adresse:</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Auto connect on startup</source>
-      <translation>Beim Starten automatisch verbinden</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>OK</source>
-      <translation>OK</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Cancel</source>
-      <translation>Abbrechen</translation>
-    </message>
   </context>
   <context>
     <name>DictInput</name>
     <message>
       <location filename="../gui/types_input/DictInput.py" line="29"/>
       <source>Add</source>
       <translation>Hinzufügen</translation>
@@ -554,75 +554,14 @@
       <source>Dutch</source>
       <translation>Niederländisch</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../gui/MainWindow.py" line="95"/>
-      <source>Session</source>
-      <translation>Sitzung</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="98"/>
-      <source>Could not connect to session bus</source>
-      <translation>Konnte nicht zum Sitzungsbus verbinden</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="98"/>
-      <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger konnte sich nicht mit dem Sitzungsbus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="103"/>
-      <source>System</source>
-      <translation>System</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="106"/>
-      <source>Could not connect to system bus</source>
-      <translation>Konnte nicht zum Systembus verbinden</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="106"/>
-      <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger konnte sich nicht mit dem Systembus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="206"/>
-      <location filename="../gui/MainWindow.py" line="112"/>
-      <source>Name exists</source>
-      <translation>Name existiert</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="112"/>
-      <source>Could not connect to {{connection}}</source>
-      <translation>Konnte nicht zu {{connection}} verbinden</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="169"/>
-      <source>You have no macros saved</source>
-      <translation>DU hast keine Makros gespeichert</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="200"/>
-      <source>Enter Name</source>
-      <translation>Namen eingeben</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="200"/>
-      <source>Please enter a name for your macro</source>
-      <translation>Bitte gib einen Namen für dein Makro ein</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="206"/>
-      <source>There is already a macro with this name</source>
-      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
-    </message>
-    <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
       <translation>Datei</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
@@ -720,18 +659,114 @@
       <translation>Signal senden</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Monitor</source>
       <translation>Beobachten</translation>
     </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="95"/>
+      <source>Session</source>
+      <translation>Sitzung</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="98"/>
+      <source>Could not connect to session bus</source>
+      <translation>Konnte nicht zum Sitzungsbus verbinden</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="98"/>
+      <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
+      <translation>jdDBusDebugger konnte sich nicht mit dem Sitzungsbus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="103"/>
+      <source>System</source>
+      <translation>System</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="106"/>
+      <source>Could not connect to system bus</source>
+      <translation>Konnte nicht zum Systembus verbinden</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="106"/>
+      <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
+      <translation>jdDBusDebugger konnte sich nicht mit dem Systembus verbinden. Wenn du jdDBusDebugger in einer Sandboxumgebung ausführst stelle sicher, dass es die notwendigen Berechtigungen hat.</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
+      <source>Name exists</source>
+      <translation>Name existiert</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="112"/>
+      <source>Could not connect to {{connection}}</source>
+      <translation>Konnte nicht zu {{connection}} verbinden</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="169"/>
+      <source>You have no macros saved</source>
+      <translation>DU hast keine Makros gespeichert</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="200"/>
+      <source>Enter Name</source>
+      <translation>Namen eingeben</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="200"/>
+      <source>Please enter a name for your macro</source>
+      <translation>Bitte gib einen Namen für dein Makro ein</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <source>There is already a macro with this name</source>
+      <translation>Es existiert bereits ein Makro mit diesem Namen</translation>
+    </message>
   </context>
   <context>
     <name>ManageMacrosDialog</name>
     <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Manage Macros</source>
+      <translation>Makros verwalten</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Rename</source>
+      <translation>Umbennen</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Delete</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>View Script</source>
+      <translation>Skript ansehen</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Export</source>
+      <translation>Exportieren</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Import</source>
+      <translation>Importieren</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>OK</source>
+      <translation>OK</translation>
+    </message>
+    <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Enter name</source>
       <translation>Name eingeben</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
@@ -793,233 +828,184 @@
       <translation>Das Makro konnte nicht importiert werden. Stelle sicher, dass du die korrekte Datei benutzt.</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <source>Please enter a name for the macro</source>
       <translation>Bitte gib einen Namen für das Makro ein</translation>
     </message>
+  </context>
+  <context>
+    <name>MonitorWindow</name>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Manage Macros</source>
-      <translation>Makros verwalten</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Filter</source>
+      <translation>Filter</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Rename</source>
-      <translation>Umbennen</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Destination:</source>
+      <translation>Empfänger:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Delete</source>
-      <translation>Löschen</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Path:</source>
+      <translation>Pfad:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>View Script</source>
-      <translation>Skript ansehen</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Sender:</source>
+      <translation>Sender:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Export</source>
-      <translation>Exportieren</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Member:</source>
+      <translation>Mitglied:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Import</source>
-      <translation>Importieren</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Interface:</source>
+      <translation>Schnitstelle:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>OK</source>
-      <translation>OK</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Signature:</source>
+      <translation>Signatur:</translation>
     </message>
-  </context>
-  <context>
-    <name>MonitorWindow</name>
     <message>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="63"/>
+      <source>Type:</source>
+      <translation>Typ:</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="64"/>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
       <source>Method call</source>
       <comment>Message type</comment>
       <translation>Methodenaufruf</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="66"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="65"/>
       <source>Method return</source>
       <comment>Message type</comment>
       <translation>Methodenrückgabe</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="68"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="67"/>
       <source>Error</source>
       <comment>Message type</comment>
       <translation>Fehler</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="70"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="69"/>
       <source>Signal</source>
       <comment>Message type</comment>
       <translation>Signal</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="71"/>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>OK</source>
+      <translation>OK</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="72"/>
       <source>Unknown</source>
       <comment>Message type</comment>
       <translation>Unbekannt</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="137"/>
+      <location filename="../gui/MonitorWindow.py" line="155"/>
       <source>Type</source>
       <comment>Table Header</comment>
       <translation>Typ</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="138"/>
+      <location filename="../gui/MonitorWindow.py" line="156"/>
       <source>Sender</source>
       <comment>Table Header</comment>
       <translation>Sender</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="139"/>
+      <location filename="../gui/MonitorWindow.py" line="157"/>
       <source>Destination</source>
       <comment>Table Header</comment>
       <translation>Empfänger</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="140"/>
+      <location filename="../gui/MonitorWindow.py" line="158"/>
       <source>Path</source>
       <comment>Table Header</comment>
       <translation>Pfad</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="141"/>
+      <location filename="../gui/MonitorWindow.py" line="159"/>
       <source>Interface</source>
       <comment>Table Header</comment>
       <translation>Schnittstelle</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="142"/>
+      <location filename="../gui/MonitorWindow.py" line="160"/>
       <source>Member</source>
       <comment>Table Header</comment>
       <translation>Mitglied</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="143"/>
+      <location filename="../gui/MonitorWindow.py" line="161"/>
       <source>Signature</source>
       <comment>Table Header</comment>
       <translation>Signatur</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="144"/>
+      <location filename="../gui/MonitorWindow.py" line="162"/>
       <source>Body</source>
       <comment>Table Header</comment>
       <translation>Inhalt</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="221"/>
+      <location filename="../gui/MonitorWindow.py" line="247"/>
+      <location filename="../gui/MonitorWindow.py" line="219"/>
       <source>Error</source>
       <translation>Fehler</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="222"/>
+      <location filename="../gui/MonitorWindow.py" line="220"/>
+      <source>Lost monitor session</source>
+      <translation>Monitorsitzung verloren</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="248"/>
       <source>Could not start monitor session</source>
       <translation>Monitorsitzung konnte nicht gestartet werden</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="235"/>
+      <location filename="../gui/MonitorWindow.py" line="262"/>
       <source>Monitor Session</source>
       <translation>Beobachte Sitzung</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="237"/>
+      <location filename="../gui/MonitorWindow.py" line="264"/>
       <source>Monitor System</source>
       <translation>Beobachte System</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="239"/>
+      <location filename="../gui/MonitorWindow.py" line="266"/>
       <source>Monitor {{name}}</source>
       <translation>Beobachte {{name}}</translation>
     </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Filter</source>
-      <translation>Filter</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Destination:</source>
-      <translation>Empfänger:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Path:</source>
-      <translation>Pfad:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Sender:</source>
-      <translation>Sender:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Member:</source>
-      <translation>Mitglied:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Interface:</source>
-      <translation>Schnitstelle:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Signature:</source>
-      <translation>Signatur:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Type:</source>
-      <translation>Typ:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Clear</source>
-      <translation>Löschen</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>OK</source>
-      <translation>OK</translation>
-    </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="30"/>
-      <source>Use system language</source>
-      <translation>Benutze Systemsprache</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="32"/>
-      <source>Add object path to list</source>
-      <translation>Füge Objektpfad zur Liste hinzu</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="33"/>
-      <source>Ask the User</source>
-      <translation>Frage den Benutzer</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="34"/>
-      <source>Do nothing</source>
-      <translation>Nichtstun</translation>
-    </message>
-    <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
       <translation>Einstellungen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
@@ -1051,14 +1037,34 @@
       <translation>OK</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
       <translation>Abbrechen</translation>
     </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="30"/>
+      <source>Use system language</source>
+      <translation>Benutze Systemsprache</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="32"/>
+      <source>Add object path to list</source>
+      <translation>Füge Objektpfad zur Liste hinzu</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="33"/>
+      <source>Ask the User</source>
+      <translation>Frage den Benutzer</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="34"/>
+      <source>Do nothing</source>
+      <translation>Nichtstun</translation>
+    </message>
   </context>
   <context>
     <name>SingleValueInputDialog</name>
     <message>
       <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
       <source>OK</source>
       <translation>OK</translation>
```

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts` & `jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_nl.ts`

 * *Files 0% similar despite different names*

#### Comparing `jddbusdebugger-3.0/jdDBusDebugger/translations/jdDBusDebugger_nl.ts` & `jddbusdebugger-3.1/jdDBusDebugger/translations/jdDBusDebugger_nl.ts`

```diff
@@ -112,14 +112,63 @@
       <source>File</source>
       <translation>Bestand</translation>
     </message>
   </context>
   <context>
     <name>CentralWidget</name>
     <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Services</source>
+      <translation>Diensten</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Search</source>
+      <translation>Zoeken</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Name</source>
+      <translation>Naam</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Activatable</source>
+      <translation>Activeerbaar</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>PID</source>
+      <translation>PID</translation>
+    </message>
+    <message>
+      <location filename="../gui/CentralWidget.py" line="296"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Refresh</source>
+      <translation>Herladen</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Objects</source>
+      <translation>Objecten</translation>
+    </message>
+    <message>
+      <location filename="../gui/CentralWidget.py" line="349"/>
+      <location filename="../gui/CentralWidget.py" line="305"/>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Add object path</source>
+      <translation>Objectlocatie toevoegen</translation>
+    </message>
+    <message>
+      <location filename="../ui/CentralWidget.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Wissen</translation>
+    </message>
+    <message>
       <location filename="../gui/CentralWidget.py" line="42"/>
       <source>Call</source>
       <translation>Aanroepen</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="73"/>
       <source>Get value</source>
@@ -173,28 +222,14 @@
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="285"/>
       <source>Copy</source>
       <translation>Kopiëren</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="296"/>
-      <source>Refresh</source>
-      <translation>Herladen</translation>
-    </message>
-    <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <location filename="../gui/CentralWidget.py" line="349"/>
-      <location filename="../gui/CentralWidget.py" line="305"/>
-      <source>Add object path</source>
-      <translation>Objectlocatie toevoegen</translation>
-    </message>
-    <message>
       <location filename="../gui/CentralWidget.py" line="305"/>
       <source>If this service has a object path that is not found trough introspection, you cann add it here</source>
       <translation>Als deze dienst beschikt over een objectlocatie die niet door middel van introspectie is aangetroffen, voeg deze dan hier toe</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="316"/>
       <source>Path not loaded</source>
@@ -281,52 +316,52 @@
       <translation>‘{{service}}’ bestaat niet</translation>
     </message>
     <message>
       <location filename="../gui/CentralWidget.py" line="499"/>
       <source>Interface {{interface}} was not found on {{path}}</source>
       <translation>‘{{interface}}’ is niet aangetroffen in {{path}}</translation>
     </message>
+  </context>
+  <context>
+    <name>ConnectDialog</name>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Services</source>
-      <translation>Diensten</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Connect</source>
+      <translation>Verbinden</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Search</source>
-      <translation>Zoeken</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>You can connect here with your custom D-Bus address</source>
+      <translation>Je kunt hier verbinding maken met je eigen D-Bus-adres</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Name</source>
-      <translation>Naam</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Name:</source>
+      <translation>Naam:</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Activatable</source>
-      <translation>Activeerbaar</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Address:</source>
+      <translation>Adres:</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>PID</source>
-      <translation>PID</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Auto connect on startup</source>
+      <translation>Automatisch verbinden na opstarten</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Objects</source>
-      <translation>Objecten</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>OK</source>
+      <translation>Oké</translation>
     </message>
     <message>
-      <location filename="../ui/CentralWidget.ui" line="0"/>
-      <source>Clear</source>
-      <translation>Wissen</translation>
+      <location filename="../ui/ConnectDialog.ui" line="0"/>
+      <source>Cancel</source>
+      <translation>Annuleren</translation>
     </message>
-  </context>
-  <context>
-    <name>ConnectDialog</name>
     <message>
       <location filename="../gui/ConnectDialog.py" line="34"/>
       <source>Name not set</source>
       <translation>Geen naam ingesteld</translation>
     </message>
     <message>
       <location filename="../gui/ConnectDialog.py" line="34"/>
@@ -349,49 +384,14 @@
       <translation>Ongeldig adres</translation>
     </message>
     <message>
       <location filename="../gui/ConnectDialog.py" line="43"/>
       <source>Could not connect to {{address}}</source>
       <translation>Er kan geen verbinding worden gemaakt met {{address}}</translation>
     </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Connect</source>
-      <translation>Verbinden</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>You can connect here with your custom D-Bus address</source>
-      <translation>Je kunt hier verbinding maken met je eigen D-Bus-adres</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Name:</source>
-      <translation>Naam:</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Address:</source>
-      <translation>Adres:</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Auto connect on startup</source>
-      <translation>Automatisch verbinden na opstarten</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>OK</source>
-      <translation>Oké</translation>
-    </message>
-    <message>
-      <location filename="../ui/ConnectDialog.ui" line="0"/>
-      <source>Cancel</source>
-      <translation>Annuleren</translation>
-    </message>
   </context>
   <context>
     <name>DictInput</name>
     <message>
       <location filename="../gui/types_input/DictInput.py" line="29"/>
       <source>Add</source>
       <translation>Toevoegen</translation>
@@ -554,75 +554,14 @@
       <source>Dutch</source>
       <translation>Nederlands</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
-      <location filename="../gui/MainWindow.py" line="95"/>
-      <source>Session</source>
-      <translation>Sessie</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="98"/>
-      <source>Could not connect to session bus</source>
-      <translation>Kan niet verbinden met sessiebus</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="98"/>
-      <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger kan geen verbinding maken met de sessiebus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="103"/>
-      <source>System</source>
-      <translation>Systeem</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="106"/>
-      <source>Could not connect to system bus</source>
-      <translation>Kan niet verbinden met systeembus</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="106"/>
-      <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
-      <translation>jdDBusDebugger kan geen verbinding maken met de systeembus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="206"/>
-      <location filename="../gui/MainWindow.py" line="112"/>
-      <source>Name exists</source>
-      <translation>Deze naam is al in gebruik</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="112"/>
-      <source>Could not connect to {{connection}}</source>
-      <translation>Er kan geen verbinding worden gemaakt met {{connection}}</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="169"/>
-      <source>You have no macros saved</source>
-      <translation>Er zĳn nog geen macro's</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="200"/>
-      <source>Enter Name</source>
-      <translation>Voer een naam in</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="200"/>
-      <source>Please enter a name for your macro</source>
-      <translation>Geef de macro een naam</translation>
-    </message>
-    <message>
-      <location filename="../gui/MainWindow.py" line="206"/>
-      <source>There is already a macro with this name</source>
-      <translation>Er is al een macro met deze naam</translation>
-    </message>
-    <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>File</source>
       <translation>Bestand</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <location filename="../ui/MainWindow.ui" line="0"/>
@@ -720,18 +659,114 @@
       <translation>Signaal uitsturen</translation>
     </message>
     <message>
       <location filename="../ui/MainWindow.ui" line="0"/>
       <source>Monitor</source>
       <translation>Monitoren</translation>
     </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="95"/>
+      <source>Session</source>
+      <translation>Sessie</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="98"/>
+      <source>Could not connect to session bus</source>
+      <translation>Kan niet verbinden met sessiebus</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="98"/>
+      <source>jdDBusDebugger was unable to connect to the session bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
+      <translation>jdDBusDebugger kan geen verbinding maken met de sessiebus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="103"/>
+      <source>System</source>
+      <translation>Systeem</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="106"/>
+      <source>Could not connect to system bus</source>
+      <translation>Kan niet verbinden met systeembus</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="106"/>
+      <source>jdDBusDebugger was unable to connect to the system bus. If you run jdDBusDebugger in a sandboxed environment make sure it has the correct permission.</source>
+      <translation>jdDBusDebugger kan geen verbinding maken met de systeembus. Als je het programma uitvoert in een gesandboxte omgeving, zorg er dan voor dat het juiste recht is toegekend.</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <location filename="../gui/MainWindow.py" line="112"/>
+      <source>Name exists</source>
+      <translation>Deze naam is al in gebruik</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="112"/>
+      <source>Could not connect to {{connection}}</source>
+      <translation>Er kan geen verbinding worden gemaakt met {{connection}}</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="169"/>
+      <source>You have no macros saved</source>
+      <translation>Er zĳn nog geen macro's</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="200"/>
+      <source>Enter Name</source>
+      <translation>Voer een naam in</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="200"/>
+      <source>Please enter a name for your macro</source>
+      <translation>Geef de macro een naam</translation>
+    </message>
+    <message>
+      <location filename="../gui/MainWindow.py" line="206"/>
+      <source>There is already a macro with this name</source>
+      <translation>Er is al een macro met deze naam</translation>
+    </message>
   </context>
   <context>
     <name>ManageMacrosDialog</name>
     <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Manage Macros</source>
+      <translation>Macro's beheren</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Rename</source>
+      <translation>Naam wĳzigen</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Delete</source>
+      <translation>Verwijderen</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>View Script</source>
+      <translation>Script bekĳken</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Export</source>
+      <translation>Exporteren</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>Import</source>
+      <translation>Importeren</translation>
+    </message>
+    <message>
+      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
+      <source>OK</source>
+      <translation>Oké</translation>
+    </message>
+    <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
       <source>Enter name</source>
       <translation>Voer een naam in</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="58"/>
@@ -793,233 +828,184 @@
       <translation>De macro kan niet worden geïmporteerd. Controleer of je het juiste bestand hebt gekozen.</translation>
     </message>
     <message>
       <location filename="../gui/ManageMacrosDialog.py" line="126"/>
       <source>Please enter a name for the macro</source>
       <translation>Geef de macro een naam</translation>
     </message>
+  </context>
+  <context>
+    <name>MonitorWindow</name>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Manage Macros</source>
-      <translation>Macro's beheren</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Filter</source>
+      <translation>Filteren</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Rename</source>
-      <translation>Naam wĳzigen</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Destination:</source>
+      <translation>Bestemming:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Delete</source>
-      <translation>Verwijderen</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Path:</source>
+      <translation>Locatie:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>View Script</source>
-      <translation>Script bekĳken</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Sender:</source>
+      <translation>Afzender:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Export</source>
-      <translation>Exporteren</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Member:</source>
+      <translation>Lid:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>Import</source>
-      <translation>Importeren</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Interface:</source>
+      <translation>Interface:</translation>
     </message>
     <message>
-      <location filename="../ui/ManageMacrosDialog.ui" line="0"/>
-      <source>OK</source>
-      <translation>Oké</translation>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Signature:</source>
+      <translation>Ondertekening:</translation>
     </message>
-  </context>
-  <context>
-    <name>MonitorWindow</name>
     <message>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="63"/>
+      <source>Type:</source>
+      <translation>Type:</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="64"/>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
       <source>Method call</source>
       <comment>Message type</comment>
       <translation>Aanroepmethode</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="66"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="65"/>
       <source>Method return</source>
       <comment>Message type</comment>
       <translation>Terugroepmethode</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="68"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="67"/>
       <source>Error</source>
       <comment>Message type</comment>
       <translation>Foutmelding</translation>
     </message>
     <message>
+      <location filename="../gui/MonitorWindow.py" line="70"/>
       <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <location filename="../gui/MonitorWindow.py" line="69"/>
       <source>Signal</source>
       <comment>Message type</comment>
       <translation>Signaal</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="71"/>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>Clear</source>
+      <translation>Wissen</translation>
+    </message>
+    <message>
+      <location filename="../ui/MonitorWindow.ui" line="0"/>
+      <source>OK</source>
+      <translation>Oké</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="72"/>
       <source>Unknown</source>
       <comment>Message type</comment>
       <translation>Onbekend</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="137"/>
+      <location filename="../gui/MonitorWindow.py" line="155"/>
       <source>Type</source>
       <comment>Table Header</comment>
       <translation>Type</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="138"/>
+      <location filename="../gui/MonitorWindow.py" line="156"/>
       <source>Sender</source>
       <comment>Table Header</comment>
       <translation>Afzender</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="139"/>
+      <location filename="../gui/MonitorWindow.py" line="157"/>
       <source>Destination</source>
       <comment>Table Header</comment>
       <translation>Bestemming</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="140"/>
+      <location filename="../gui/MonitorWindow.py" line="158"/>
       <source>Path</source>
       <comment>Table Header</comment>
       <translation>Locatie</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="141"/>
+      <location filename="../gui/MonitorWindow.py" line="159"/>
       <source>Interface</source>
       <comment>Table Header</comment>
       <translation>Interface</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="142"/>
+      <location filename="../gui/MonitorWindow.py" line="160"/>
       <source>Member</source>
       <comment>Table Header</comment>
       <translation>Lid</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="143"/>
+      <location filename="../gui/MonitorWindow.py" line="161"/>
       <source>Signature</source>
       <comment>Table Header</comment>
       <translation>Ondertekening</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="144"/>
+      <location filename="../gui/MonitorWindow.py" line="162"/>
       <source>Body</source>
       <comment>Table Header</comment>
       <translation>Inhoud</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="221"/>
+      <location filename="../gui/MonitorWindow.py" line="247"/>
+      <location filename="../gui/MonitorWindow.py" line="219"/>
       <source>Error</source>
       <translation>Foutmelding</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="222"/>
+      <location filename="../gui/MonitorWindow.py" line="220"/>
+      <source>Lost monitor session</source>
+      <translation>De sessie is afgebroken</translation>
+    </message>
+    <message>
+      <location filename="../gui/MonitorWindow.py" line="248"/>
       <source>Could not start monitor session</source>
       <translation>De sessie kan niet worden gestart</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="235"/>
+      <location filename="../gui/MonitorWindow.py" line="262"/>
       <source>Monitor Session</source>
       <translation>Sessie monitoren</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="237"/>
+      <location filename="../gui/MonitorWindow.py" line="264"/>
       <source>Monitor System</source>
       <translation>Systeem monitoren</translation>
     </message>
     <message>
-      <location filename="../gui/MonitorWindow.py" line="239"/>
+      <location filename="../gui/MonitorWindow.py" line="266"/>
       <source>Monitor {{name}}</source>
       <translation>{{name}} monitoren</translation>
     </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Filter</source>
-      <translation>Filteren</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Destination:</source>
-      <translation>Bestemming:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Path:</source>
-      <translation>Locatie:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Sender:</source>
-      <translation>Afzender:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Member:</source>
-      <translation>Lid:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Interface:</source>
-      <translation>Interface:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Signature:</source>
-      <translation>Ondertekening:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Type:</source>
-      <translation>Type:</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>Clear</source>
-      <translation>Wissen</translation>
-    </message>
-    <message>
-      <location filename="../ui/MonitorWindow.ui" line="0"/>
-      <source>OK</source>
-      <translation>Oké</translation>
-    </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
-      <location filename="../gui/SettingsDialog.py" line="30"/>
-      <source>Use system language</source>
-      <translation>Systeemtaal</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="32"/>
-      <source>Add object path to list</source>
-      <translation>Objectlocatie toevoegen aan lĳst</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="33"/>
-      <source>Ask the User</source>
-      <translation>Om actie vragen</translation>
-    </message>
-    <message>
-      <location filename="../gui/SettingsDialog.py" line="34"/>
-      <source>Do nothing</source>
-      <translation>Niets doen</translation>
-    </message>
-    <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Settings</source>
       <translation>Instellingen</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Language:</source>
@@ -1051,14 +1037,34 @@
       <translation>Oké</translation>
     </message>
     <message>
       <location filename="../ui/SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
       <translation>Annuleren</translation>
     </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="30"/>
+      <source>Use system language</source>
+      <translation>Systeemtaal</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="32"/>
+      <source>Add object path to list</source>
+      <translation>Objectlocatie toevoegen aan lĳst</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="33"/>
+      <source>Ask the User</source>
+      <translation>Om actie vragen</translation>
+    </message>
+    <message>
+      <location filename="../gui/SettingsDialog.py" line="34"/>
+      <source>Do nothing</source>
+      <translation>Niets doen</translation>
+    </message>
   </context>
   <context>
     <name>SingleValueInputDialog</name>
     <message>
       <location filename="../gui/types_input/SingleValueInputDialog.py" line="22"/>
       <source>OK</source>
       <translation>Oké</translation>
```

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Connection.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Connection.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/DBusType.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/DBusType.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/DBusValue.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/DBusValue.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Interface.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Interface.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Macro.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Macro.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Method.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Method.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Property.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Property.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Service.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Service.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/Signal.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/Signal.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/actions/ActionBase.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/actions/ActionBase.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/actions/CallAction.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/actions/CallAction.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/actions/EmitAction.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/actions/EmitAction.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/actions/PropertyAction.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/actions/PropertyAction.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/types/actions/SignalAction.py` & `jddbusdebugger-3.1/jdDBusDebugger/types/actions/SignalAction.py`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/AboutDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/AboutDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/CentralWidget.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/CentralWidget.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/ConnectDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/ConnectDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/EmitSignalDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/EmitSignalDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/GenerateScriptDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/GenerateScriptDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/MainWindow.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/ManageMacrosDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/ManageMacrosDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/MonitorWindow.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/MonitorWindow.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/SettingsDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger/ui/WelcomeDialog.ui` & `jddbusdebugger-3.1/jdDBusDebugger/ui/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/jdDBusDebugger.egg-info/PKG-INFO` & `jddbusdebugger-3.1/jdDBusDebugger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jdDBusDebugger
-Version: 3.0
+Version: 3.1
 Summary: An advanced D-Bus Debugger
 Author-email: JakobDev <jakobdev@gmx.de>
 License: GPL-3
 Project-URL: Source, https://codeberg.org/JakobDev/jdDBusDebugger
 Project-URL: Issues, https://codeberg.org/JakobDev/jdDBusDebugger/issues
 Project-URL: Translate, https://translate.codeberg.org/projects/jdDBusDebugger
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `jddbusdebugger-3.0/jdDBusDebugger.egg-info/SOURCES.txt` & `jddbusdebugger-3.1/jdDBusDebugger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jddbusdebugger-3.0/pyproject.toml` & `jddbusdebugger-3.1/pyproject.toml`

 * *Files identical despite different names*

