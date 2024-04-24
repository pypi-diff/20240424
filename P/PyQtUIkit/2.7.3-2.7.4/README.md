# Comparing `tmp/PyQtUIkit-2.7.3.tar.gz` & `tmp/PyQtUIkit-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.7.3.tar", last modified: Thu Apr 18 11:52:01 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.7.4.tar", last modified: Wed Apr 24 09:33:41 2024, max compression
```

## Comparing `PyQtUIkit-2.7.3.tar` & `PyQtUIkit-2.7.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.871001 PyQtUIkit-2.7.3/
--rw-rw-rw-   0        0        0     1090 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-18 11:52:01.871001 PyQtUIkit-2.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.839747 PyQtUIkit-2.7.3/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3896 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/_icons.py
--rw-rw-rw-   0        0        0     3342 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/_translate.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.839747 PyQtUIkit-2.7.3/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.839747 PyQtUIkit-2.7.3/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     5248 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.855375 PyQtUIkit-2.7.3/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.855375 PyQtUIkit-2.7.3/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     3908 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  2340473 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1830 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/locale.py
--rw-rw-rw-   0        0        0     1470 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.871001 PyQtUIkit-2.7.3/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1654 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3304 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     7885 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2739 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0    11298 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8328 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2542 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/form.py
--rw-rw-rw-   0        0        0     2280 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     1578 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1171 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     5174 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/layout.py
--rw-rw-rw-   0        0        0     1697 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1758 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     4253 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     4948 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/menu_bar.py
--rw-rw-rw-   0        0        0     7084 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2647 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     4021 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1486 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/separator.py
--rw-rw-rw-   0        0        0     7515 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    13972 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2370 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16743 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/PyQtUIkit/widgets/tree_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:52:01.839747 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2576 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 11:52:01.000000 PyQtUIkit-2.7.3/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:52:01.871001 PyQtUIkit-2.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1474 2024-04-18 11:51:06.000000 PyQtUIkit-2.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.634496 PyQtUIkit-2.7.4/
+-rw-rw-rw-   0        0        0     1090 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3896 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/_icons.py
+-rw-rw-rw-   0        0        0     3342 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     5248 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.603240 PyQtUIkit-2.7.4/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     3908 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  2340473 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1830 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/locale.py
+-rw-rw-rw-   0        0        0     1470 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.618862 PyQtUIkit-2.7.4/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1670 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3304 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     7885 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2794 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0    11413 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8328 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5876 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2542 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/form.py
+-rw-rw-rw-   0        0        0     2280 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     1578 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1171 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     5272 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/layout.py
+-rw-rw-rw-   0        0        0     1697 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3671 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1758 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     4253 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     4948 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu_bar.py
+-rw-rw-rw-   0        0        0     7084 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2647 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     4021 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1486 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/separator.py
+-rw-rw-rw-   0        0        0     7515 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    14062 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1295 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     4538 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    17878 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/PyQtUIkit/widgets/tree_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:33:41.587642 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2576 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 09:33:41.000000 PyQtUIkit-2.7.4/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:33:41.634496 PyQtUIkit-2.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2024-04-24 09:33:07.000000 PyQtUIkit-2.7.4/setup.py
```

### Comparing `PyQtUIkit-2.7.3/LICENSE` & `PyQtUIkit-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PKG-INFO` & `PyQtUIkit-2.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.3
+Version: 2.7.4
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/_icons.py` & `PyQtUIkit-2.7.4/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/_translate.py` & `PyQtUIkit-2.7.4/PyQtUIkit/_translate.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.7.4/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.7.4/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/core/font.py` & `PyQtUIkit-2.7.4/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.7.4/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.7.4/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.7.4/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/builtin_themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PyQtUIkit.core.font import KitFont
 from PyQtUIkit.themes.theme import KitTheme, KitPalette
 
 basic_theme = KitTheme({
-    'Transparent': KitPalette('#00FFFFFF', '#30FFFFFF', '#60FFFFFF', '#222222'),
+    'Transparent': KitPalette('#00000000', '#30000000', '#60000000', '#222222'),
 
     'Main': KitPalette('#FFFFFF', '#DFE1E5', '#CFDEFC', '#222222'),
     'Bg': KitPalette('#ECF5F9', '#CBCDCF', '#5283C9', '#222222'),
     'Menu': KitPalette('#C4CBCF', '#9DA3A6', '#3B81F0', '#222222'),
     'Border': KitPalette('#BFC0C2', '#A6A7A8', '#52AFDE', '#222222'),
     'Success': KitPalette('#B3D635', '#D0FA3E', '#41D431', '#222222', '#2A8018'),
     'Warning': KitPalette('#E3C920', '#CFB71D', '#C7891E', '#222222', '#AB8618'),
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/locale.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/locale.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.7.4/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 from PyQtUIkit.widgets.progress_bar import KitProgressBar
 from PyQtUIkit.widgets.tree_widget import KitTreeWidget, KitTreeWidgetItem
 from PyQtUIkit.widgets.menu import KitMenu
 from PyQtUIkit.widgets.group import KitHGroup, KitVGroup
 from PyQtUIkit.widgets.navigation import KitNavigation
 from PyQtUIkit.widgets.radio import KitVRadio, KitHRadio
 from PyQtUIkit.widgets.tabs import KitTabLayout
-from PyQtUIkit.widgets.text_edit import KitTextEdit
+from PyQtUIkit.widgets.text_edit import KitTextEdit, KitTextBrowser
 from PyQtUIkit.widgets.form import KitForm
 from PyQtUIkit.widgets.dialog import KitDialog, KitFormDialog
 from PyQtUIkit.widgets.application import KitApplication, KitAsyncApplication
 from PyQtUIkit.widgets.separator import KitHSeparator, KitVSeparator
 from PyQtUIkit.widgets.menu_bar import KitMenuBar
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/checkbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         self.__button.setChecked(self.__state)
         self.stateChanged.emit(self.__state)
 
     def isChecked(self):
         return self.__state
 
     def setChecked(self, state):
+        if state == self.__state:
+            return
         self.__state = bool(state)
         self.__on_state_changed()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__button._set_tm(tm)
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/combo_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,18 @@
             item = KitComboBoxItem(item, value)
         item.selected.connect(self._on_item_selected)
         self.__widgets.append(item)
         self.__menu.add_item(item)
         if len(self.__widgets) == 1:
             self.setCurrentIndex(0)
 
+    def addItems(self, items: [KitComboBoxItem | str]):
+        for el in items:
+            self.addItem(el)
+
     def deleteItem(self, index):
         self.__widgets.pop(index)
         self.__menu.delete_item(index)
         if index == self.__current:
             self.__current = min(self.__current, len(self.__widgets) - 1)
             if not self.__widgets:
                 self.__current = None
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/flow_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     def _set_tm(self, tm):
         super()._set_tm(tm)
         for el in self.__widgets:
             if hasattr(el, '_set_tm'):
                 el._set_tm(tm)
 
     def _apply_theme(self):
+        if not self._tm or not self._tm.active:
+            return
         for el in self.__widgets:
             if hasattr(el, '_apply_theme'):
                 el._apply_theme()
         self.setStyleSheet(f"""
         QWidget {{
             background-color: {self.main_palette.main};
             border: {self.border}px solid {self.border_palette.main};
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/form.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/form.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/layout.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
     def setSpacing(self, spacing):
         self.__layout.setSpacing(spacing)
 
     def getSpacing(self):
         return self.__layout.spacing()
 
+    def setDirection(self, a0: QHBoxLayout.Direction):
+        self.__layout.setDirection(a0)
+
     def setContentsMargins(self, left: int, top: int, right: int, bottom: int) -> None:
         self.__layout.setContentsMargins(left, top, right, bottom)
 
     def getContentsMargins(self):
         return self.__layout.contentsMargins()
 
     def _set_margins(self, margins):
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/list_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from PyQt6.QtGui import QColor
 from PyQt6.QtWidgets import QListWidget, QListWidgetItem
 
-from PyQtUIkit.core.properties import IntProperty, IconProperty
+from PyQtUIkit.core.properties import IntProperty, IconProperty, EnumProperty, KitFont,FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitListWidget(QListWidget, _KitWidget):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    font = FontProperty('font')
 
     def __init__(self):
         super().__init__()
         self.__widgets = []
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
@@ -29,23 +31,25 @@
         super().insertItem(row, item)
         if isinstance(item, KitListWidgetItem):
             item._set_tm(self._tm)
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
+        self.setFont(self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QListWidget {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main};
     border: {self.border}px solid {self.border_palette.main};
     border-radius: {self.radius}px;
 }}
 QListWidget::item {{
     border-radius: 6px;
+    min-height: 24px;
 }}
 QListWidget::item:hover {{
     background-color: {self.main_palette.hover};
 }}
 QListWidget::item:selected {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.selected};
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/menu_bar.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/menu_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/separator.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tab_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,18 @@
         self.__tabs.insert(index, tab)
         self.__layout.update_tabs()
         tab.show()
         if self.__current is None:
             self.__current = tab
             tab._set_checked(True)
 
+    def clear(self):
+        self.__tabs.clear()
+        self.__layout.update_tabs()
+
     def _scroll_left(self):
         self.__scroll_area.scroll(-50)
 
     def _scroll_right(self):
         self.__scroll_area.scroll(50)
 
     def _close_requested(self, tab):
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tabs.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,19 @@
         else:
             widget.hide()
 
     def addWidget(self, widget: QWidget, *args):
         self.insertWidget(len(self._widgets), widget)
 
     def setCurrent(self, index):
-        if self.__current is not None:
+        if self.__current is not None and self.__current < len(self._widgets):
             self._widgets[self.__current].hide()
         self.__current = index
         self._widgets[self.__current].show()
 
     def connect(self, widget: KitTabBar | KitNavigation | KitVRadio | KitHRadio):
         if self.__connected_widget is not None:
             raise Exception("can connect only one widget")
         self.__connected_widget = widget
         widget.currentChanged.connect(self.setCurrent)
-        self.setCurrent(widget.currentIndex())
+        if widget.currentTab():
+            self.setCurrent(widget.currentIndex())
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/text_edit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt6.QtWidgets import QTextEdit
+from PyQt6.QtWidgets import QTextEdit, QTextBrowser
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, PaletteProperty, EnumProperty, FontProperty, TextProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitTextEdit(QTextEdit, _KitWidget):
@@ -72,7 +72,81 @@
 }}
 """)
 
     def _apply_lang(self):
         if not self._tm:
             return
         self.setPlaceholderText(self.placeholder_text)
+
+
+class KitTextBrowser(QTextBrowser, _KitWidget):
+    main_palette = PaletteProperty('main_palette', 'Main')
+    border = IntProperty('border', 1)
+    radius = IntProperty('radius', 4)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
+    placeholder_text = TextProperty('placeholder_text')
+
+    def __init__(self):
+        super().__init__()
+
+    def _apply_theme(self):
+        if not self._tm or not self._tm.active:
+            return
+        self.setFont(self.font.get(self.font_size))
+        self.setStyleSheet(f"""
+QTextBrowser {{
+    color: {self.main_palette.text};
+    background-color: {self.main_palette.main};
+    border: {self.border}px solid {self.border_palette.main};
+    border-radius: {self.radius}px;
+}}
+QTextBrowser QScrollBar:vertical {{
+    background: {self.main_palette.main};
+    border-top-right-radius: 5px;
+    border-bottom-right-radius: 5px;
+    width: 12px;
+    margin: 0px;
+}}
+QTextBrowser QScrollBar:horizontal {{
+    background: {self.main_palette.main};
+    border-bottom-left-radius: 5px;
+    border-bottom-right-radius: 5px;
+    height: 12px;
+    margin: 0px;
+}}
+QTextBrowser QScrollBar::handle::horizontal {{
+    background-color: {self.border_palette.main};
+    margin: 6px 2px 2px 2px;
+    border-radius: 2px;
+    min-width: 20px;
+}}
+QTextBrowser QScrollBar::handle::horizontal:hover {{
+    margin: 2px;
+    border-radius: 4px;
+}}
+QTextBrowser QScrollBar::handle::vertical {{
+    background-color: {self.border_palette.main};
+    margin: 2px 2px 2px 6px;
+    border-radius: 2px;
+    min-height: 20px;
+}}
+QTextBrowser QScrollBar::handle::vertical:hover {{
+    margin: 2px;
+    border-radius: 4px;
+}}
+QTextBrowser QScrollBar::sub-page, QScrollBar::add-page {{
+    background: none;
+}}
+QTextBrowser QScrollBar::sub-line, QScrollBar::add-line {{
+    background: none;
+    height: 0px;
+    subcontrol-position: left;
+    subcontrol-origin: margin;
+}}
+""")
+
+    def _apply_lang(self):
+        if not self._tm:
+            return
+        self.setPlaceholderText(self.placeholder_text)
+
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.7.4/PyQtUIkit/widgets/tree_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint
 
 from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, StringProperty, IconProperty, BoolProperty, EnumProperty, \
-    PaletteProperty, FontProperty
+    PaletteProperty, FontProperty, MethodsProperty
 from PyQtUIkit.widgets.dialog import KitDialog
 from PyQtUIkit.widgets.layout import KitVBoxLayout, KitHBoxLayout
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.button import KitLayoutButton, KitIconButton
 from PyQtUIkit.widgets.checkbox import KitCheckBox
@@ -33,18 +33,17 @@
         self._main_palette = 'Main'
         self._text_palette = 'Main'
         self.__level = 0
         self._height = 24
         self.__selected = False
         self.__expanded = False
         self.__children: list[KitTreeWidgetItem] = []
+        self.__children_checked = 0
         self.__root: KitTreeWidget = None
         self.__parent: KitTreeWidgetItem = None
-        self._icon1 = None
-        self._icon2 = None
         self.__never_expanded = True
         self.__move_widget = None
         self.__last_pos = None
 
         self.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self.__button = KitLayoutButton()
@@ -53,29 +52,33 @@
         self.__button.mousePressEvent = self._on_clicked
         self.__button.mouseMoveEvent = self._on_move
         self.__button.mouseReleaseEvent = self._on_released
         self.__button.mouseDoubleClickEvent = self._on_double_clicked
         self.addWidget(self.__button)
 
         self.__arrow_right = KitIconButton('line-chevron-forward')
-        self.__arrow_right.setFixedSize(20, 20)
+        self.__arrow_right.main_palette = 'Transparent'
+        self.__arrow_right.size = 16
+        self.__arrow_right.radius = 8
         self.__arrow_right.border = 0
         self.__arrow_right.hide()
         self.__arrow_right.clicked.connect(self.expand)
         self.__button.addWidget(self.__arrow_right)
 
         self.__arrow_down = KitIconButton('line-chevron-down')
-        self.__arrow_down.setFixedSize(20, 20)
+        self.__arrow_down.main_palette = 'Transparent'
+        self.__arrow_down.size = 16
+        self.__arrow_down.radius = 8
         self.__arrow_down.border = 0
         self.__arrow_down.hide()
         self.__arrow_down.clicked.connect(self.collapse)
         self.__button.addWidget(self.__arrow_down)
 
         self.__checkbox = KitCheckBox()
-        self.__checkbox.on_state_edited = self.stateEdited.emit
+        self.__checkbox.on_state_edited = self._on_state_edited
         self.__button.addWidget(self.__checkbox)
 
         self.__icon_widget = KitIconWidget()
         self.__button.addWidget(self.__icon_widget)
 
         self.__label = KitLabel(self._name)
         self.__button.addWidget(self.__label)
@@ -99,26 +102,29 @@
     def insertItem(self, index, item: 'KitTreeWidgetItem'):
         item._set_level(self.__level + 1)
         item._set_root(self.__root, self)
         item._set_tm(self._tm)
 
         self.__children.insert(index, item)
         self.__layout.insertWidget(index, item)
+        if item.state:
+            self.__children_checked += 1
 
         self.__arrow_down.setHidden(not self.__expanded)
         self.__arrow_right.setHidden(self.__expanded)
         self._update_padding()
 
     def childrenCount(self):
         return len(self.__children)
 
     def child(self, index):
         return self.__children[index]
 
     def clear(self):
+        self.__children_checked = 0
         for _ in range(self.count()):
             self.__layout.clear()
         for el in self.__children:
             if el.selected():
                 self.__root._set_current(None)
         self.__children.clear()
 
@@ -171,14 +177,32 @@
     def _select(self, multi=False):
         self.__selected = True
         self._apply_selected_theme()
         if multi:
             for el in self.__children:
                 el._select(True)
 
+    def _on_state_edited(self, state):
+        for el in self.__children:
+            el._parent_state_edited(state)
+        self.__children_checked = self.childrenCount() if state else 0
+        self.__parent._child_state_changed(state)
+        self.stateEdited.emit(state)
+
+    def _parent_state_edited(self, state: bool):
+        self.state = state
+        for el in self.__children:
+            el._parent_state_edited(state)
+
+    def _child_state_changed(self, state: bool):
+        self.__children_checked += 1 if state else -1
+        self.setChecked(self.__children_checked == self.childrenCount())
+        if self.__parent:
+            self.__parent._child_state_changed(self.__children_checked == self.childrenCount())
+
     def _on_move(self, a0):
         KitLayoutButton.mouseMoveEvent(self.__button, a0)
         if self.__last_pos is None:
             return
         if not self.__root.movable:
             return 
         if self.__move_widget is None:
@@ -217,15 +241,14 @@
                                          (0 if self.__children or self.always_expandable else 25), 0, 0, 0)
 
     def _hide_button(self):
         self.__button.hide()
 
     def _set_tm(self, tm):
         super()._set_tm(tm)
-        self.__icon_widget._set_tm(tm)
         for el in self.__children:
             el._set_tm(tm)
 
     def _set_root(self, root, parent):
         self.__root = root
         self.__parent = parent
         for el in self.__children:
@@ -239,32 +262,34 @@
             for i, el in enumerate(self.__children):
                 res, h = el._find_by_pos(pos - QPoint(0, height))
                 if res:
                     return res, 0
                 height += h
         return None, height
 
-    @property
-    def checked(self):
+    def isChecked(self):
         return self.checkable and self.__checkbox.state
 
     def setChecked(self, state):
         self.__checkbox.state = state
 
+    state = MethodsProperty(isChecked, setChecked)
+
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.__checkbox.setHidden(not self.checkable)
         for el in self.__children:
             el._height = self._height
             el.main_palette = self._main_palette
             el.text_palette = self._text_palette
         self.__button.setFixedHeight(self._height)
         self.__icon_widget.setFixedSize(self._height - 4, self._height - 4)
         self.__icon_widget._icon = self._icon
+        self.__icon_widget.setHidden(not self._icon)
 
         if self.__children or self.always_expandable:
             self.__arrow_down.setHidden(not self.__expanded)
             self.__arrow_right.setHidden(self.__expanded)
         else:
             self.__arrow_down.setHidden(True)
             self.__arrow_right.setHidden(True)
@@ -450,14 +475,17 @@
             self.__shift = False
         elif a0.key() == Qt.Key.Key_Control:
             self.__control = False
 
     def clear(self):
         self.__tree.clear()
 
+    def items(self):
+        return self.__tree.children()
+
     def _set_tm(self, tm):
         super()._set_tm(tm)
         self.__tree._set_tm(tm)
 
     def _apply_theme(self):
         self.__tree.main_palette = self._main_palette
         self.__tree._main_palette = self._main_palette
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.7.4/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.7.3
+Version: 2.7.4
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.7.3/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.7.4/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.7.3/setup.py` & `PyQtUIkit-2.7.4/setup.py`

 * *Files identical despite different names*

