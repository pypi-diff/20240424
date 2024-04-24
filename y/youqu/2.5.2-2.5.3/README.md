# Comparing `tmp/youqu-2.5.2.tar.gz` & `tmp/youqu-2.5.3.tar.gz`

## Comparing `youqu-2.5.2.tar` & `youqu-2.5.3.tar`

### file list

```diff
@@ -1,216 +1,221 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/CURRENT
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/_env_base.sh
--rw-r--r--   0        0        0    41623 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/conftest.py
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/env.sh
--rwxr-xr-x   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/env_dev.sh
--rw-r--r--   0        0        0    24243 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/manage.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/pylint.sh
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/ruff.toml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/__init__.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/remote.ini
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/__init__.py
--rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26357 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/calculate.py
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/desktop.py
--rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/filectl.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/filter_image.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14861 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/mouse_key.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/read_csv.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/requestx.py
--rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/singleton.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/startapp.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30165 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/git/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/git/check.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    12110 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/remotectl/base.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/remotectl/remote_ctl.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/remotectl/remote_dogtail_ctl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0    22070 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/pycharm.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 youqu-2.5.2/pyproject.toml
--rw-r--r--   0        0        0    14550 2020-02-02 00:00:00.000000 youqu-2.5.2/youqu/README.md
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 youqu-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/CURRENT
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/_env_base.sh
+-rw-r--r--   0        0        0    43113 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/conftest.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/docs_env.sh
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/env.sh
+-rwxr-xr-x   0        0        0     3090 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/env_dev.sh
+-rw-r--r--   0        0        0    24445 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/manage.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/playbook.toml
+-rw-r--r--   0        0        0    68097 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pnpm-lock.yaml
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pylint.sh
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pytest.ini
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/ruff.toml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/__init__.py
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26357 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/calculate.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/filter_image.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14861 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/read_csv.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/singleton.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    19630 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0    21433 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/opencv_rpc_server.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/pycharm.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/vnc.sh
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/README.md
+-rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 youqu-2.5.3/PKG-INFO
```

### Comparing `youqu-2.5.2/youqu/_env_base.sh` & `youqu-2.5.3/youqu/_env_base.sh`

 * *Files 4% similar despite different names*

```diff
@@ -15,35 +15,45 @@
             ;;
         ?)
             echo "there is unrecognized parameter."
             exit 1
             ;;
     esac
 done
+
+debian_platform=false
+yq=apt
+if command -v apt &> /dev/null; then
+    debian_platform=true
+    yq=apt
+else
+    yq=yum
+fi
+
 DISPLAY_SERVER=$(cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1 | cut -d "=" -f2)
 PYTHON_VERSION=$(python3 -c "import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')")
 flag_feel="\n**** (・_・) ****\n"
 whitelist="/usr/share/deepin-elf-verify/whitelist"
 pypi_mirror="https://pypi.tuna.tsinghua.edu.cn/simple"
-echo "${PASSWORD}" | sudo -S su  > /dev/null 2>&1
+echo "${PASSWORD}" | sudo -S su
 
+if [ ! -f "$HOME/.Xauthority" ]; then
+        touch $HOME/.Xauthority
+fi
 
 check_status(){
     if [ $? = 0 ]; then
         echo -e "$1\t安装成功 √"
     else
         echo -e "$1\t安装失败 ×"
-        echo "PASSWORD: ${PASSWORD}"
-        echo "如果密码与实际不符，请使用 -p 选项传入参数：bash env.sh -p xxx，或修改setting/globalconfig.ini中的PASSWORD配置项"
         cat /tmp/env.log
     fi
 }
 
 wayland_env(){
-    echo -e "${flag_feel}安装 Wayland 上键鼠工具\n"
     deb_array=(g++ build-essential cmake qt5-default qt5-qmake libqt5gui5 libqt5core5a)
     for deb in ${deb_array[*]}
     do
         sudo apt install -y ${deb} > /tmp/env.log 2>&1
         check_status ${deb}
         apt policy ${deb} > /tmp/_yqdebversion.txt 2>&1
         cat /tmp/_yqdebversion.txt | grep "已安装"
@@ -80,18 +90,14 @@
     wayland_cmd_path="/usr/local/bin/wayland_autotool"
     result=`sudo cat ${whitelist} | grep ${wayland_cmd_path}`
     if [ -z "$result" ]; then
         sudo sed -i '$a\'"${wayland_cmd_path}"'' ${whitelist} || echo "白名单${whitelist}写入失败"
         sudo systemctl restart deepin-elf-verify.service || true
     fi
 
-    if [ ! -f "$HOME/.Xauthority" ]; then
-        touch $HOME/.Xauthority
-    fi
-
     nohup wayland_autotool > /dev/null 2>&1 &
 }
 
 system_env(){
     echo "${PASSWORD}" | sudo -S su  > /dev/null 2>&1
     sudo sed -i "s/#PubkeyAuthentication yes/PubkeyAuthentication yes/g" /etc/ssh/sshd_config > /dev/null 2>&1
     sudo sed -i "s/#   StrictHostKeyChecking ask/   StrictHostKeyChecking no/g" /etc/ssh/ssh_config  > /dev/null 2>&1
@@ -109,24 +115,24 @@
 
     gsettings set org.gnome.desktop.interface toolkit-accessibility true  > /dev/null 2>&1
     sudo systemctl enable ssh  > /dev/null 2>&1
     sudo systemctl start ssh  > /dev/null 2>&1
 }
 
 init_pip(){
+    sudo pip3 config set global.index-url ${pypi_mirror} > /tmp/env.log 2>&1
     sudo pip3 install -U pip > /tmp/env.log 2>&1
     sudo pip3 cache purge > /tmp/env.log 2>&1
     sudo pip3 config set global.timeout 10000 > /tmp/env.log 2>&1
-    sudo pip3 config set global.index-url ${pypi_mirror} > /tmp/env.log 2>&1
 }
 
 install_py_deb(){
     rm -rf ${1}*
     apt download ${1} > /tmp/env.log 2>&1
     if [ $? != 0 ]; then
         cat /tmp/env.log
-        exit 520
+        exit 120
     fi
     dpkg -x ${1}*.deb ${1}
     cp -r ./${1}/usr/lib/python3/dist-packages/* ${2}/lib/python${PYTHON_VERSION}/site-packages/
     rm -rf ${1}*
 }
```

### Comparing `youqu-2.5.2/youqu/conftest.py` & `youqu-2.5.3/youqu/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0301,R0912,C0413,R0914,W0212,R1702,R0915
 # pylint: disable=C0114,W0621,C0411,C0412,R1706,E0401
+import re
 import sys
 from os import environ
 
 from setting.globalconfig import GlobalConfig
 
 environ["DISPLAY"] = ":0"
 environ["PIPENV_VERBOSITY"] = "-1"
-environ["XAUTHORITY"] = f"/home/{GlobalConfig.USERNAME}/.Xauthority"
+environ["XAUTHORITY"] = f"{GlobalConfig.HOME}/.Xauthority"
 
 from setting.globalconfig import SystemPath
 
 for i in SystemPath:
     if i.value not in sys.path:
         sys.path.append(i.value)
 
@@ -140,14 +141,15 @@
         default=False,
         help="出现错误时立即显示",
     )
     parser.addoption("--repeat", action="store", default=1, type=int, help="用例重复执行的次数")
     parser.addoption("--export_csv_file", action="store", default="", help="导出csv文件")
     parser.addoption("--line", action="store", default="", help="业务线(CI)")
     parser.addoption("--app_name", action="store", default="", help="执行的应用名称")
+    parser.addoption("--slaves", action="store", default="", help="远程测试机")
     parser.addoption(
         "--autostart", action="store", default="", help="重启类场景开启letmego执行方案"
     )
 
 
 def pytest_cmdline_main(config):
     """pytest_cmdline_main"""
@@ -639,26 +641,27 @@
     """pytest_runtest_makereport"""
     out = yield
     report = out.get_result()
     if report.when == "setup":
         for mark in item.own_markers:
             if mark.name == "parametrize":
                 continue
-            if mark.args[0] == FixedCsvTitle.case_level.value:
-                try:
-                    allure.dynamic.severity(LabelType[mark.name].value)
-                except KeyError:
-                    allure.dynamic.severity(LabelType.L3.value)
-            elif mark.args[0] == FixedCsvTitle.pms_case_id.value:
-                # if mark.name:
-                testcase_url = f"https://pms.uniontech.com/testcase-view-{mark.name}.html"
-                allure.dynamic.testcase(testcase_url)
-                logger.info(testcase_url)
-            else:
-                allure.dynamic.tag(mark.name)
+            if mark.args:
+                if mark.args[0] == FixedCsvTitle.case_level.value:
+                    try:
+                        allure.dynamic.severity(LabelType[mark.name].value)
+                    except KeyError:
+                        allure.dynamic.severity(LabelType.L3.value)
+                elif mark.args[0] == FixedCsvTitle.pms_case_id.value:
+                    # if mark.name:
+                    testcase_url = f"https://pms.uniontech.com/testcase-view-{mark.name}.html"
+                    allure.dynamic.testcase(testcase_url)
+                    logger.info(testcase_url)
+                else:
+                    allure.dynamic.tag(mark.name)
     if report.when == "call":
         logger.info(f"运行结果: {str(report.outcome).upper()}")
         if write_json(item.session):
             # 只要是需要数据回填（无论是自动还是手动）,都需要写json结果.
             write_case_result(item, report)
 
         if item.config.option.autostart:
@@ -969,25 +972,70 @@
         for file in files:
             if file.endswith(".csv") and file != "case_list.csv":
                 csv_path_dict[splitext(file)[0]] = f"{root}/{file}"
     return csv_path_dict, no_youqu_mark
 
 
 @pytest.fixture(scope='session')
-def page():
+def native_page():
     from playwright.sync_api import sync_playwright
     driver = sync_playwright().start()
-    browser = driver.chromium.launch(headless=False)
+    browser = driver.chromium.launch(
+        headless=False,
+        args=[
+            '--start-maximized',
+        ],
+    )
     context = browser.new_context(
         ignore_https_errors=True,
-        viewport={
-            "width": 1920,
-            "height": 1080,
-        },
+        no_viewport=True,
     )
     _page = context.new_page()
-
     yield _page
-
     context.close()
     browser.close()
     driver.stop()
+
+
+@pytest.fixture(scope='session')
+def page():
+    from playwright.sync_api import sync_playwright
+    driver = sync_playwright().start()
+    browser = driver.chromium.launch_persistent_context(
+        user_data_dir=GlobalConfig.USER_DATE_DIR,
+        executable_path=GlobalConfig.EXECUTABLE_PATH,
+        ignore_https_errors=True,
+        no_viewport=True,
+        slow_mo=500,
+        headless=False,
+        bypass_csp=True,
+        args=[
+            '--disable-blink-features=AutomationControlled',
+            '--start-maximized',
+        ],
+
+    )
+    _page = browser.pages[0]
+    yield _page
+    browser.close()
+    driver.stop()
+
+
+@pytest.fixture(scope="session")
+def slaves(pytestconfig):
+    _slaves = pytestconfig.getoption("slaves") or GlobalConfig.SLAVES
+    s = []
+    if _slaves:
+        for slave in _slaves.split("/"):
+            slave_info = re.findall(r"^(.+?)@(\d+\.\d+\.\d+\.\d+):{0,1}(.*?)$", slave)
+            if slave_info:
+                user, ip, password = slave_info[0]
+                s.append(
+                    {
+                        "user": user,
+                        "ip": ip,
+                        "password": password or GlobalConfig.PASSWORD,
+                    }
+                )
+    if not s:
+        raise EnvironmentError("No slaves found")
+    return s
```

### Comparing `youqu-2.5.2/youqu/env.sh` & `youqu-2.5.3/youqu/env.sh`

 * *Files 4% similar despite different names*

```diff
@@ -35,43 +35,41 @@
         deb_array=(
             python3-pip
             sshpass
             openjdk-8-jdk
         )
     fi
 
-    echo -e "${flag_feel}安装 deb 包\n"
     for deb in ${deb_array[*]}
     do
         sudo apt install -y ${deb} > /tmp/env.log 2>&1
         check_status ${deb}
     done
 
     if [ "${DISPLAY_SERVER}" = "wayland" ]; then
         wayland_env
     fi
 }
 env
 
-echo -e "${flag_feel}安装 pip 包\n"
 init_pip
 
 sudo pip3 install pipenv > /tmp/env.log 2>&1
 if [ $? = 0 ]; then
     echo -e "pipenv\t安装成功 √"
 else
     echo -e "pipenv\t安装失败 ×"
     cat /tmp/env.log
-    exit 520
+    exit 120
 fi
 cd ${ROOT_DIR}/
 pipenv --python ${PYTHON_VERSION} > /tmp/env.log 2>&1
 if [ $? != 0 ]; then
     echo -e "AT环境创建失败"
-    exit 521
+    exit 121
 fi
 python_virtualenv_path=$(pipenv --venv)
 whitelist_path=`echo "${python_virtualenv_path}" | sed "s/\/home\/$USER\//\//"`
 result=`sudo cat ${whitelist} | grep ${whitelist_path}`
 if [ -z "$result" ]; then
     sudo sed -i '$a\'"${whitelist_path}"'' ${whitelist}
     sudo sed -i '$a\'"${python_virtualenv_path}"'' ${whitelist}
@@ -152,14 +150,20 @@
 cd ${ROOT_DIR}/src/utils/
 webui=$(python3 sub_webui.py)
 if [ "${webui}" != "" ]; then
     pipenv run pip install playwright -i ${pypi_mirror}
     pipenv run playwright install chromium
 fi
 
+cd ${ROOT_DIR}/src/utils/
+remote=$(python3 sub_remote.py)
+if [ "${remote}" != "" ]; then
+    pipenv run pip install zerorpc -i ${pypi_mirror}
+fi
+
 pipenv run pip install -U auto_uos --extra-index-url ${pypi_mirror} -i http://10.20.52.221:8081 --trusted-host=10.20.52.221 \
 > /tmp/env.log 2>&1
 check_status auto_uos
 pip_show=$(pipenv run pip show auto_uos | grep Location)
 public_location=$(echo "${pip_show}" | cut -d ":" -f2 | python3 -c "s=input();print(s.strip())")
 sudo rm -rf ${ROOT_DIR}/public
 sudo cp -r ${public_location}/auto_uos ${ROOT_DIR}/public
```

### Comparing `youqu-2.5.2/youqu/env_dev.sh` & `youqu-2.5.3/youqu/env_dev.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
 source ./_env_base.sh
 
 env(){
-    sudo apt update
+
+    if [ ${debian_platform} == true ]; then
+        sudo apt update
+    fi
 
     deb_array=(
         python3-pip
         sshpass
         scrot
         python3-tk
         python3-pyatspi
-        openjdk-8-jdk
+        openjdk-11-jdk-headless
         python3-opencv
     )
 
     # 裁剪基础环境
     cd ${ROOT_DIR}/src/utils
     BASICENV=$(python3 sub_env_cut.py)
     if [ "${BASICENV}" = "BASICENV" ]; then
         ENV_CUT_FLAG="cut"
         deb_array=(
             python3-pip
             sshpass
-            openjdk-8-jdk
+            openjdk-11-jdk-headless
         )
     fi
 
-    echo -e "${flag_feel}安装 deb 包\n"
+    if [ ${debian_platform} == false ]; then
+        deb_array[${#deb_array[@]}]=java-11-openjdk-headless
+        deb_array[${#deb_array[@]}]=python3-tkinter
+        deb_array[${#deb_array[@]}]=xdotool
+    fi
+
     for deb in ${deb_array[*]}
     do
-        sudo apt install -y ${deb} > /tmp/env.log 2>&1
+        sudo ${yq} install -y ${deb} > /tmp/env.log 2>&1
         check_status ${deb}
     done
 
     cd ${ROOT_DIR}/src/utils/
     sub_py_debs=$(python3 sub_deb.py)
     for spd in ${sub_py_debs[*]}
     do
-        sudo apt install -y ${spd} > /tmp/env.log 2>&1
+        sudo ${yq} install -y ${spd} > /tmp/env.log 2>&1
         check_status ${spd}
     done
 
     # wayland
     if [ "${DISPLAY_SERVER}" = "wayland" ]; then
         wayland_env
     fi
 }
 env
 
-echo -e "${flag_feel}安装 pip 包\n"
 init_pip
 
 pip_array=(
     pyscreeze==0.1.28
     PyAutoGUI==0.9.53
     pytest==6.2.5
     pytest-rerunfailures==10.2
@@ -99,14 +106,20 @@
 cd ${ROOT_DIR}/src/utils/
 webui=$(python3 sub_webui.py)
 if [ "${webui}" != "" ]; then
     sudo pip3 install playwright -i ${pypi_mirror}
     playwright install chromium
 fi
 
+cd ${ROOT_DIR}/src/utils/
+remote=$(python3 sub_remote.py)
+if [ "${remote}" != "" ]; then
+    sudo pip3 install zerorpc -i ${pypi_mirror}
+fi
+
 sudo pip3 install -U auto_uos --extra-index-url ${pypi_mirror} -i http://10.20.52.221:8081 --trusted-host=10.20.52.221 \
 > /tmp/env.log 2>&1
 check_status auto_uos
 pip_show=$(pip3 show auto_uos | grep Location)
 public_location=$(echo "${pip_show}" | cut -d ":" -f2 | python3 -c "s=input();print(s.strip())")
 sudo rm -rf ${ROOT_DIR}/public
 sudo cp -r ${public_location}/auto_uos ${ROOT_DIR}/public
```

### Comparing `youqu-2.5.2/youqu/manage.py` & `youqu-2.5.3/youqu/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from argparse import ArgumentParser
 
 from setting.globalconfig import GlobalConfig
 from setting.globalconfig import SystemPath
 
 os.environ["DISPLAY"] = ":0"
 os.environ["PIPENV_VERBOSITY"] = "-1"
-os.environ["XAUTHORITY"] = f"/home/{GlobalConfig.USERNAME}/.Xauthority"
+os.environ["XAUTHORITY"] = f"{GlobalConfig.HOME}/.Xauthority"
 
 for i in SystemPath:
     if i.value in sys.path:
         continue
     sys.path.append(i.value)
 
 from funnylog import logger
@@ -84,14 +84,15 @@
             send2task=None,
             url=None,
             startdate=None,
             enddate=None,
             git_user=None,
             git_password=None,
             depth=None,
+            slaves=None
     ):
         self.default_app = app
         self.default_keywords = keywords
         self.default_tags = tags
         self.default_rerun = rerun
         self.default_record_failed_case = record_failed_case
         self.default_clean = clean
@@ -135,14 +136,15 @@
         self.default_send2task = send2task
         self.default_url = url
         self.default_startdate = startdate
         self.default_enddate = enddate
         self.default_git_user = git_user
         self.default_git_password = git_password
         self.default_depth = depth
+        self.default_slaves = slaves
         from src.depends.cfonts import say
 
         say(GlobalConfig.PROJECT_NAME)
         version_font = "slick"
         say(GlobalConfig.current_tag, font=version_font, space=False)
         say(f"Code: \033[0;32m{GlobalConfig.GITHUB_URL}\033[0m", font="console", space=False)
         say(f"Docs: \033[0;32m{GlobalConfig.DOCS_URL}\033[0m", font="console", space=False)
@@ -318,14 +320,15 @@
             help="测试过程中立即显示报错",
         )
         sub_parser_run.add_argument("--repeat", default="", help="指定用例执行次数")
         sub_parser_run.add_argument("--project_name", default="", help="工程名称（写入json文件）")
         sub_parser_run.add_argument("--build_location", default="", help="构建地区（写入json文件）")
         sub_parser_run.add_argument("--line", default="", help="执行的业务线（写入json文件）")
         sub_parser_run.add_argument("--autostart", default="", help="重启类场景开启letmego执行方案")
+        sub_parser_run.add_argument("--slaves", default="", help="远程测试机")
         args = parser.parse_args()
         from src.rtk._base import Args
 
         local_kwargs = {
             Args.app_name.value: args.app or self.default_app,
             Args.keywords.value: args.keywords or self.default_keywords,
             Args.tags.value: args.tags or self.default_tags,
@@ -354,14 +357,15 @@
             Args.lastfailed.value: args.lastfailed or self.default_lastfailed,
             Args.duringfail.value: args.duringfail or self.default_duringfail,
             Args.repeat.value: args.repeat or self.default_repeat,
             Args.project_name.value: args.project_name or self.default_project_name,
             Args.build_location.value: args.build_location or self.default_build_location,
             Args.line.value: args.line or self.default_line,
             Args.autostart.value: args.autostart or self.default_autostart,
+            Args.slaves.value: args.slaves or self.default_slaves,
         }
         if local_kwargs.get(Args.autostart.value) or GlobalConfig.AUTOSTART:
             import letmego
 
             letmego.conf.setting.PASSWORD = GlobalConfig.PASSWORD
             letmego.register_autostart_service(
                 user=GlobalConfig.USERNAME,
```

### Comparing `youqu-2.5.2/youqu/pylint.sh` & `youqu-2.5.3/youqu/pylint.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/ruff.toml` & `youqu-2.5.3/youqu/ruff.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/startproject.py` & `youqu-2.5.3/youqu/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/setting/globalconfig.ini` & `youqu-2.5.3/youqu/setting/globalconfig.ini`

 * *Files 27% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 ;1.关闭录屏：RECORD_FAILED_CASE > RERUN
 ;2.每条用例都录屏：RECORD_FAILED_CASE = 0
 RECORD_FAILED_CASE = 1
 
 ;yes 每条用例执行之后进行环境清理
 CLEAN_ALL = yes
 
-;检查测试机分辨率, 比如：1920x1080
+;检查测试机分辨率, 比如：1920x1080, 多个分辨率检查用英文逗号连接。
 ;no: 表示不做分辨率校验
-RESOLUTION = 1920x1080
+RESOLUTION = 1920x1080, 1080x1920, 3840x1080
 
 ;不跳过用例，csv文件里面标记了 skip-xxx的用例不跳过
 NOSKIP = no
 
 ;ignore fixed
 ;no，只要标记了fixed的用例，即使标记了skip-，也会执行；
 ;yes，fixed不生效，仅通过skip跳过用例；
@@ -141,14 +141,70 @@
 
 ;图像识别的总超时
 OPENCV_TIMEOUT = 5
 
 ;图像识别的最大次数
 OPENCV_MAX_MATCH_NUMBER = 100
 
+;=============================== SLAVE CONFIG ===================================
+;附属的测试机，用例步骤中与其他机器进行交互
+;        ┌─ slave ${user}@${ip}:${password}
+; master ┼─ slave mikigo@192.168.8.11:admin123
+;        └─ slave ${user}@${ip}
+;如果${password}和前面配置项PASSWORD一样，可以不传：${user}@${ip}
+;多个机器之间用斜线分割：${user}@${ip}:${password}/${user}@${ip}
+SLAVES =
+
+;=============================== Web UI CONFIG ===================================
+;为Web UI自动化测试提供一个fixture对象：page，它默认使用系统自带的浏览器进行测试。
+;框架还提供一个fixture对象：native_page，它使用最新的chromium浏览器进行测试。
+;以下配置项默认值为系统自带的浏览器的配置，如果是其他第三方的浏览器可以指定浏览器对应的路径。
+; def test_xxx_001(page):
+;     page.goto("www.baidu.com")
+;
+; def test_xxx_001(native_page):
+;     native_page.goto("www.baidu.com")
+
+;指定浏览器启动的用户数据缓存目录
+USER_DATE_DIR = {{HOME}}/.config/browser
+
+;指定浏览器可执行文件路径
+EXECUTABLE_PATH = /usr/bin/browser
+
+;=============================== REMOTE CONFIG ===================================
+[remote]
+;发送代码到测试机（不含report目录）
+SEND_CODE = yes
+
+;搭建测试环境
+;如果为yes，不管send_code是否为yes都会发送代码到测试机。
+BUILD_ENV = no
+
+;测试机密码
+CLIENT_PASSWORD = 1
+
+;yes表示所有测试机并行跑，执行相同的测试用例。
+;no表示测试机分布式执行，服务端会根据收集到的测试用例自动分配给各个测试机执行。
+PARALLEL = yes
+
+;清理 report 目录
+CLEAN_SERVER_REPORT_DIR = no
+CLEAN_CLIENT_REPORT_DIR = yes
+
+;测试机轮询次数
+SCAN = 300
+
+;远程执行测试机
+;              ┌─ client ${user}@${ip}:${password}
+; youqu-server ┼─ client mikigo@192.168.8.11:admin123
+;              └─ client ${user}@${ip}
+;如果${password}和前面配置项CLIENT_PASSWORD一样，可以不传：${user}@${ip}
+;多个机器之间用斜线分割：${user}@${ip}:${password}/${user}@${ip}
+CLIENTS =
+
 ;=============================== REPORT CONFIG ===================================
 [report]
 ;测试报告的title
 REPORT_TITLE = YouQu Report
 
 ;测试报告的name
 REPORT_NAME = YouQu Report
```

### Comparing `youqu-2.5.2/youqu/setting/globalconfig.py` & `youqu-2.5.3/youqu/setting/globalconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 from configparser import RawConfigParser  # 解决读取log报错
 from enum import Enum
 from enum import unique
 from getpass import getuser
 from os import popen
+from os import getenv
 from os.path import abspath
 from os.path import dirname
 from os.path import join
 from platform import machine
 from time import strftime
+import pathlib
 
 
 # pylint: disable=C0116,C0103,C0103,C0115,R0903
 
 
 class GetCfg:
     """Gets the value in the configuration file"""
@@ -63,14 +63,18 @@
     # apps path
     APPS_PATH = join(ROOT_DIR, DirName.APPS)
     # setting path
     SETTING_PATH = join(ROOT_DIR, DirName.SETTING)
     # Default does not exist
     REPORT_PATH = join(ROOT_DIR, DirName.REPORT)
 
+    # username
+    USERNAME = getuser()
+    HOME = str(pathlib.Path.home())
+
     # ====================== GLOBAL CONFIG INI ======================
     # Get config file object
     GLOBAL_CONFIG_FILE_PATH = join(SETTING_PATH, "globalconfig.ini")
     # [run]
     run_cfg = GetCfg(GLOBAL_CONFIG_FILE_PATH, "run")
     APP_NAME = run_cfg.get("APP_NAME", default="")
     KEYWORDS = run_cfg.get("KEYWORDS", default="")
@@ -110,14 +114,29 @@
     OPENCV_SERVER_HOST = run_cfg.get("OPENCV_SERVER_HOST", default="localhost")
     OPENCV_PORT = run_cfg.get("OPENCV_PORT", default="8889")
     OPENCV_NETWORK_RETRY = run_cfg.get("OPENCV_NETWORK_RETRY", default=1)
     OPENCV_PAUSE = run_cfg.get("OPENCV_PAUSE", default=1)
     OPENCV_TIMEOUT = run_cfg.get("OPENCV_TIMEOUT", default=5)
     OPENCV_MAX_MATCH_NUMBER = run_cfg.get("OPENCV_MAX_MATCH_NUMBER", default=100)
 
+    SLAVES = run_cfg.get("SLAVES", default="")
+    USER_DATE_DIR = run_cfg.get("USER_DATE_DIR", default="").replace("{{HOME}}", HOME)
+    EXECUTABLE_PATH = run_cfg.get("EXECUTABLE_PATH", default="")
+
+    # [remote]
+    remote_cfg = GetCfg(GLOBAL_CONFIG_FILE_PATH, "remote")
+    SEND_CODE = remote_cfg.get_bool("SEND_CODE", default=True)
+    BUILD_ENV = remote_cfg.get_bool("BUILD_ENV", default=False)
+    CLIENT_PASSWORD = remote_cfg.get("CLIENT_PASSWORD", default="1")
+    PARALLEL = remote_cfg.get_bool("PARALLEL", default=True)
+    CLEAN_SERVER_REPORT_DIR = remote_cfg.get_bool("CLEAN_SERVER_REPORT_DIR", default=False)
+    CLEAN_CLIENT_REPORT_DIR = remote_cfg.get_bool("CLEAN_CLIENT_REPORT_DIR", default=True)
+    SCAN = remote_cfg.get("SCAN", default="300")
+    CLIENTS = remote_cfg.get("CLIENTS", default="")
+
     # [report]
     report_cfg = GetCfg(GLOBAL_CONFIG_FILE_PATH, "report")
     REPORT_TITLE = report_cfg.get("REPORT_TITLE", default="YouQu Report")
     REPORT_NAME = report_cfg.get("REPORT_NAME", default="YouQu Report")
     REPORT_LANGUAGE = report_cfg.get("REPORT_LANGUAGE", default="zh")
     REPORT_FORMAT = report_cfg.get("REPORT_FORMAT", default="allure, xml, json")
     ALLURE_REPORT_PATH = join(
@@ -178,23 +197,21 @@
     GIT_PASSWORD = log_cli.get("GIT_PASSWORD", default="")
     BRANCH = log_cli.get("BRANCH", default="")
     DEPTH = log_cli.get("DEPTH", default="")
     START_DATE = log_cli.get("STAR_TDATE", default="")
     END_DATE = log_cli.get("END_DATE", default="")
 
     # ====================== 动态获取变量 ======================
-    # username
-    USERNAME = getuser()
+    version_cfg = GetCfg("/etc/os-version", "Version")
+    VERSION = (version_cfg.get("EditionName[zh_CN]") or "") + (
+            version_cfg.get("MinorVersion") or ""
+    )
     # IP
-    OS_VERSION = GetCfg("/etc/os-version", "Version")
     HOST_IP = str(popen("hostname -I |awk '{print $1}'").read()).strip("\n").strip()
     PRODUCT_INFO = popen("cat /etc/product-info").read()
-    VERSION = (OS_VERSION.get("EditionName[zh_CN]") or "") + (
-            OS_VERSION.get("MinorVersion") or ""
-    )
     # machine type
     # e.g. x86_64
     SYS_ARCH = machine()
     LANGUAGE_INI = GetCfg(join(SETTING_PATH, "template/language.ini"), "language")
 
     current_tag = GetCfg(f"{ROOT_DIR}/CURRENT", "current").get("tag")
 
@@ -213,31 +230,34 @@
     TIME_STRING = strftime("%Y%m%d%H%M%S")
 
     slp_cfg = GetCfg(f"{SETTING_PATH}/sleepx.ini", "sleepx")
 
     # 显示服务器
     # 直接读环境变量XDG_SESSION_TYPE会有问题，采用读文件的方式获取
     DISPLAY_SERVER = (
-        popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
-        .read()
-        .split("=")[-1]
-        .strip("\n")
-    )
+                         popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
+                         .read()
+                         .split("=")[-1]
+                         .strip("\n")
+                     ) or ("x11" if popen("ps -ef | grep -v grep | grep kwin_x11").read() else "wayland")
 
     class DisplayServer:
         wayland = "wayland"
         x11 = "x11"
 
+    if DISPLAY_SERVER not in (DisplayServer.x11, DisplayServer.wayland):
+        raise EnvironmentError(f"DISPLAY_SERVER: {DISPLAY_SERVER} why?")
+
     IS_X11 = DISPLAY_SERVER == DisplayServer.x11
     IS_WAYLAND = DISPLAY_SERVER == DisplayServer.wayland
 
     top_cmd = "top -b -d 3 -w 512"
 
-    GITHUB_URL = "https://github.com/linuxdeepin/deepin-autotest-framework"
-    DOCS_URL = "https://linuxdeepin.github.io/deepin-autotest-framework"
+    GITHUB_URL = "https://github.com/linuxdeepin/youqu"
+    DOCS_URL = "https://linuxdeepin.github.io/youqu"
     PyPI_URL = "https://pypi.org/project/youqu"
 
     LETMEGO_DEBUG = True
     DTK_DISPLAY = False
 
 
 GlobalConfig = _GlobalConfig()
```

### Comparing `youqu-2.5.2/youqu/setting/pylintrc.cfg` & `youqu-2.5.3/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/setting/skipif.py` & `youqu-2.5.3/youqu/setting/skipif.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,31 +45,39 @@
     使用 sudo dmidecode -s system-product-name 查看机器的cpu型号
     剔除中横线和&符号，比如：KLVV-W5821，标签记录为 KLVVW5821
     skipif_cpu_name-KLVVW5821
     """
     _skip_key = args.split("&")
     for key in _skip_key:
         if (
-            os.popen(
-                f"echo '{GlobalConfig.PASSWORD}'| "
-                "sudo -S dmidecode -s system-product-name | awk '{print $NF}'"
-            )
-            .read()
-            .strip("\n")
-            .replace("-", "")
-            .replace("&", "")
-            == key
+                os.popen(
+                    f"echo '{GlobalConfig.PASSWORD}'| "
+                    "sudo -S dmidecode -s system-product-name | awk '{print $NF}'"
+                )
+                        .read()
+                        .split("\n")[0]
+                        .replace("-", "")
+                        .replace("&", "")
+                == key
         ):
             return True
     return False
 
 
 def skipif_os_version(args: str):
     """
     系统版本跳过
     skipif_os_version-1060
     """
     _skip_key = args.split("&")
     for key in _skip_key:
-        if key == GlobalConfig.OS_VERSION.get("MinorVersion"):
+        if key == GlobalConfig.version_cfg.get("MinorVersion"):
             return True
     return False
+
+
+if __name__ == '__main__':
+    a = os.popen(
+        f"echo '{GlobalConfig.PASSWORD}'| "
+        "sudo -S dmidecode -s system-product-name | awk '{print $NF}'"
+    ).read().split("\n")[0]
+    print(a)
```

### Comparing `youqu-2.5.2/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.5.3/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.5.3/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.5.3/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/__init__.py` & `youqu-2.5.3/youqu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/assert_common.py` & `youqu-2.5.3/youqu/src/assert_common.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/button_center.py` & `youqu-2.5.3/youqu/src/button_center.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/calculate.py` & `youqu-2.5.3/youqu/src/calculate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/cmdctl.py` & `youqu-2.5.3/youqu/src/cmdctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,26 +65,29 @@
             data = ex.__str__()
             exitcode = -1
         if data[-1:] == "\n":
             data = data[:-1]
         return exitcode, data
 
     @classmethod
-    def sudo_run_cmd(cls, command, interrupt=True, timeout=25, out_debug_flag=True, command_log=True):
-        cls.run_cmd(
-            f"echo '{conf.PASSWORD}' | sudo -S {command}",
+    def sudo_run_cmd(cls, command, interrupt=False, timeout=25, out_debug_flag=True,
+                     command_log=True, password=None):
+        if password is None:
+            password = conf.PASSWORD
+        return cls.run_cmd(
+            f"echo '{password}' | sudo -S {command}",
             interrupt=interrupt,
             timeout=timeout,
             out_debug_flag=out_debug_flag,
             command_log=command_log
         )
 
     @classmethod
     def run_cmd(
-            cls, command, interrupt=True, timeout=25, out_debug_flag=True, command_log=True
+            cls, command, interrupt=False, timeout=25, out_debug_flag=True, command_log=True
     ):
         """
          执行shell命令
         :param command: shell 命令
         :param interrupt: 命令异常时是否中断
         :param timeout: 命令执行超时
         :param out_debug_flag: 命令返回信息输出日志
```

### Comparing `youqu-2.5.2/youqu/src/csvctl.py` & `youqu-2.5.3/youqu/src/csvctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/custom_exception.py` & `youqu-2.5.3/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/dbus_utils.py` & `youqu-2.5.3/youqu/src/dbus_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/desktop.py` & `youqu-2.5.3/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/dogtail_utils.py` & `youqu-2.5.3/youqu/src/dogtail_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114,C0103
 import re
+from typing import Union
 
 from setting.globalconfig import GlobalConfig
-from src  import logger
+from src import logger
 from src.cmdctl import CmdCtl
 from src.custom_exception import ElementNotFound
 from src.custom_exception import ApplicationStartError
 
 try:
     from src.depends.dogtail.tree import SearchError
     from src.depends.dogtail.tree import root
     from src.depends.dogtail.tree import predicate
     from src.depends.dogtail.tree import config
+    from src.depends.dogtail.tree import Node
 
     config.childrenLimit = 1000
     # config.logDebugToStdOut = False
     config.logDebugToFile = False
     config.searchCutoffCount = 2
     GlobalConfig.NO_DOGTAIL = False
 except ModuleNotFoundError:
@@ -57,15 +59,15 @@
 
         except SearchError:
             if check_start:
                 search_app = CmdCtl.run_cmd(f"ps -ef | grep {self.name}")
                 logger.error(search_app)
                 raise ApplicationStartError(self.name) from SearchError
 
-    def app_element(self, *args, **kwargs):
+    def app_element(self, *args, **kwargs) -> Node:
         """
          获取app元素的对象
         :return: 元素的对象
         """
         try:
             element = self.obj.child(*args, **kwargs, retry=False)
             logger.debug(f"{args, kwargs} 获取元素对象 <{element}>")
@@ -164,15 +166,14 @@
         else:
             element = element.findChildren(
                 predicate.GenericPredicate(name), recursive=recursive
             )
         return node, element
 
     def __trace(self, element, result, expr):
-        """trace"""
         if expr.startswith("//"):
             name = expr[2:]
             node, element = self.__evalx(name, element, recursive=True)
         elif expr.startswith("/"):
             name = expr[1:]
             node, element = self.__evalx(name, element, recursive=False)
         else:
@@ -184,15 +185,15 @@
                     self.__trace(i, result, next_node)
             else:
                 result += element
         except SearchError:
             raise ElementNotFound(expr) from SearchError
         return result
 
-    def find_elements_by_attr(self, expr):
+    def find_elements_by_attr(self, expr) -> Union[list, bool]:
         """
          通过层级获取元素
         :param expr: 元素定位 $/xx.xxx//xxx,  $根节点  /当前子节点， //递归查找子节点
         :return: 元素对象
         """
         logger.debug(f"查找元素 expr={expr}")
         if expr == "$":
@@ -201,18 +202,18 @@
             return False
         if not expr.endswith("/") or expr.endswith(r"\/"):
             expr = expr + "/"
         result = self.__trace(self.obj, [], expr[1:])
         logger.debug(f"元素 {result}")
         return result
 
-    def find_element_by_attr(self, expr, index=0):
+    def find_element_by_attr(self, expr, index=0) -> Node:
         """
          查找界面元素
-        :param expr: 匹配格式
+        :param expr: 匹配格式 元素定位 $/xxx//xxx,  $根节点  /当前子节点， //递归查找子节点
         :param index: 匹配结果索引
         :return: 元素对象
         """
         elements = self.find_elements_by_attr(expr)
         if not elements:
             raise ElementNotFound(expr)
         try:
```

### Comparing `youqu-2.5.2/youqu/src/filectl.py` & `youqu-2.5.3/youqu/src/filectl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/filter_image.py` & `youqu-2.5.3/youqu/src/filter_image.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/image_utils.py` & `youqu-2.5.3/youqu/src/image_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/mouse_key.py` & `youqu-2.5.3/youqu/src/mouse_key.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/ocr_utils.py` & `youqu-2.5.3/youqu/src/ocr_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pinyin.py` & `youqu-2.5.3/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/read_csv.py` & `youqu-2.5.3/youqu/src/read_csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/recording_screen.py` & `youqu-2.5.3/youqu/src/recording_screen.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/requestx.py` & `youqu-2.5.3/youqu/src/requestx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/shortcut.py` & `youqu-2.5.3/youqu/src/shortcut.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/singleton.py` & `youqu-2.5.3/youqu/src/singleton.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+#!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114,C0203
+
 import weakref
 import threading
 
 
 class Singleton(type):
     """底层单例模式封装"""
```

### Comparing `youqu-2.5.2/youqu/src/sleepx.py` & `youqu-2.5.3/youqu/src/sleepx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/startapp.py` & `youqu-2.5.3/youqu/src/startapp.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/startproject.py` & `youqu-2.5.3/youqu/src/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/video_utils.py` & `youqu-2.5.3/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/wayland_wininfo.py` & `youqu-2.5.3/youqu/src/wayland_wininfo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/ydotool.py` & `youqu-2.5.3/youqu/src/ydotool.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/cli.py` & `youqu-2.5.3/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/colors.py` & `youqu-2.5.3/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/consts.py` & `youqu-2.5.3/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/core.py` & `youqu-2.5.3/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.5.3/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/colorama/ansi.py` & `youqu-2.5.3/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.5.3/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/colorama/initialise.py` & `youqu-2.5.3/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/colorama/win32.py` & `youqu-2.5.3/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/colorama/winterm.py` & `youqu-2.5.3/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/COPYING` & `youqu-2.5.3/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/__init__.py` & `youqu-2.5.3/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/config.py` & `youqu-2.5.3/youqu/src/depends/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/distro.py` & `youqu-2.5.3/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/dump.py` & `youqu-2.5.3/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/errors.py` & `youqu-2.5.3/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/i18n.py` & `youqu-2.5.3/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/logging.py` & `youqu-2.5.3/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/path.py` & `youqu-2.5.3/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/predicate.py` & `youqu-2.5.3/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/procedural.py` & `youqu-2.5.3/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.5.3/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.5.3/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/sessions.py` & `youqu-2.5.3/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/tc.py` & `youqu-2.5.3/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/tree.py` & `youqu-2.5.3/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/utils.py` & `youqu-2.5.3/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/version.py` & `youqu-2.5.3/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.5.3/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.5.3/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.5.3/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.5.3/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.5.3/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.5.3/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/sniff` & `youqu-2.5.3/youqu/src/depends/sniff/sniff`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # 在某些机型上可能出现环境变量未加载的问题，这里强制将其注册到环境变量中；
 sys_path.append(dn(dn(dn(dn(abspath(__file__))))))
 
 from setting.globalconfig import GlobalConfig
 
 if GlobalConfig.IS_WAYLAND:
-    environ["XAUTHORITY"] = f"/home/{GlobalConfig.USERNAME}/.Xauthority"
+    environ["XAUTHORITY"] = f"{GlobalConfig.HOME}/.Xauthority"
 
 from src.depends.dogtail.config import config
 
 if config.checkForA11y:
     from src.depends.dogtail.utils import checkForA11yInteractively
 
     checkForA11yInteractively()
```

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/sniff.ui` & `youqu-2.5.3/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.5.3/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.5.3/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.5.3/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.5.3/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/LICENSE` & `youqu-2.5.3/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/git/clone.py` & `youqu-2.5.3/youqu/src/git/clone.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/git/code_statistics.py` & `youqu-2.5.3/youqu/src/git/code_statistics.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/git/commit.py` & `youqu-2.5.3/youqu/src/git/commit.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/plugins/allure_report_extend.py` & `youqu-2.5.3/youqu/src/plugins/allure_report_extend.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/plugins/emoji_hooks.py` & `youqu-2.5.3/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pms/_base.py` & `youqu-2.5.3/youqu/src/pms/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pms/csv2pms.py` & `youqu-2.5.3/youqu/src/pms/csv2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pms/pms2csv.py` & `youqu-2.5.3/youqu/src/pms/pms2csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,25 +84,25 @@
             case = cases.get(i)
             case_id = case.get("id")
             case_level = case.get("pri")
             case_type = self.pms_mark.get(case.get("type"))
             case_from = case.get("caseSource")
             device_type = case.get("deviceType")
             online_obj = case.get("lineCD")
-            if case_type:
-                res_data[case_id] = {
-                    "case_level": f"L{case_level}",
-                    "case_type": case_type,
-                    "case_from": "BUG" if case_from == "是" else "",
-                    "device_type": device_type.split("(")[0]
-                    if device_type and device_type != "null"
-                    else "",
-                    "online_obj": "CICD" if online_obj == "是" else "",
-                    "skip_reason": "skip-下线CD" if online_obj == "否" else None
-                }
+            # if case_type:
+            res_data[case_id] = {
+                "case_level": f"L{case_level}",
+                "case_type": case_type,
+                "case_from": "BUG" if case_from == "是" else "",
+                "device_type": device_type.split("(")[0]
+                if device_type and device_type != "null"
+                else "",
+                "online_obj": "CICD" if online_obj == "是" else "",
+                "skip_reason": "skip-下线CD" if online_obj == "否" else None
+            }
         if not res_data:
             logger.error(f"未从pms获取到数据, {self.config_error_log}")
             raise ValueError
         return res_data
 
     def read_csv(self):
         """读取本地csv文件数据"""
```

### Comparing `youqu-2.5.2/youqu/src/pms/send2pms.py` & `youqu-2.5.3/youqu/src/pms/send2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pms/suite.py` & `youqu-2.5.3/youqu/src/pms/suite.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/pms/task.py` & `youqu-2.5.3/youqu/src/pms/task.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/rtk/_base.py` & `youqu-2.5.3/youqu/src/rtk/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     send2task = "send2task"
     url = "url"
     startdate = "startdate"
     enddate = "enddate"
     user = "user"
     password = "password"
     depth = "depth"
+    slaves = "slaves"
 
 
 def  transform_app_name(app_name):
     """转换 app_name"""
     if not app_name:
         return None
     if "-" in app_name:
```

### Comparing `youqu-2.5.2/youqu/src/rtk/local_runner.py` & `youqu-2.5.3/youqu/src/rtk/local_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,21 @@
             repeat=None,
             project_name=None,
             build_location=None,
             line=None,
             collection_only=None,
             autostart=None,
             export_csv_file=None,
+            slaves=None,
             **kwargs,
     ):
         logger("INFO")
         try:
             github_tags = RequestX().open_url(
-                f"https://api.github.com/repos/linuxdeepin/deepin-autotest-framework/tags",
+                f"https://api.github.com/repos/linuxdeepin/youqu/tags",
                 timeout=1
             )
             latest_tag = json.loads(github_tags)[0].get("name")
             if GlobalConfig.current_tag != latest_tag:
                 print(f"YouQu最新版本为: {latest_tag}，当前使用版本为: {GlobalConfig.current_tag}")
                 print(f"建议使用：sudo pip3 install youqu=={latest_tag} 升级版本")
         except Exception:
@@ -131,22 +132,27 @@
             Args.pms_info_file.value: pms_info_file,
             Args.autostart.value: autostart or GlobalConfig.AUTOSTART,
         }
         self.lastfailed = lastfailed
         self.project_name = project_name
         self.build_location = build_location
         self.line = line
+        self.slaves = slaves
         self.collection_only = collection_only
         self.export_csv_file = export_csv_file or GlobalConfig.EXPORT_CSV_FILE
 
         if not (self.default.get(Args.debug.value) or self.collection_only):
             screen = Tk()
             x = screen.winfo_screenwidth()
             y = screen.winfo_screenheight()
-            if self.default.get(Args.resolution.value) not in (f"{x}x{y}", "no"):
+            rls = [i.strip() for i in self.default.get(Args.resolution.value).split(",")]
+            for rl in rls:
+                if rl in (f"{x}x{y}", "no"):
+                    break
+            else:
                 raise ValueError(f"当前分辨率为：{x}x{y},您配置的分辨率为：{GlobalConfig.RESOLUTION}")
 
     @property
     def export_default(self):
         return self.default
 
     @staticmethod
@@ -282,14 +288,16 @@
         if default.get(Args.autostart.value):
             GlobalConfig.LETMEGO_DEBUG = False
             cmd.extend(["--autostart", default.get(Args.autostart.value)])
         if default.get(Args.repeat.value):
             cmd.extend(["--repeat", default.get(Args.repeat.value)])
         if self.line:
             cmd.extend(["--line", self.line])
+        if self.slaves:
+            cmd.extend(["--slaves", self.slaves])
 
         report_formats = default.get(Args.report_formats.value)
         if report_formats:
             report_formats = [i.strip() for i in report_formats.split(",")]
             # allure
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) and (
                     GlobalConfig.ReportFormat.JSON not in report_formats
```

### Comparing `youqu-2.5.2/youqu/src/rtk/remote_runner.py` & `youqu-2.5.3/youqu/src/rtk/remote_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 setting.report_name = GlobalConfig.REPORT_NAME
 setting.report_language = GlobalConfig.REPORT_LANGUAGE
 
 from src.cmdctl import CmdCtl
 from src import logger
 from src.rtk._base import Args
 from src.rtk._base import transform_app_name
+from setting import conf
 
 
 class RemoteRunner:
     """
     远程执行器：控制多台测试机远程执行用例。
     在 setting/remote.ini 里面配置要执行的测试机信息。
     """
@@ -52,61 +53,47 @@
             self,
             remote_kwargs: dict = None,
             local_kwargs: dict = None,
     ):
         self.remote_kwargs = remote_kwargs
         self.local_kwargs = local_kwargs
         logger("INFO")
-        conf = ConfigParser()
-        conf.read(f"{GlobalConfig.SETTING_PATH}/remote.ini")
-        self.parallel = conf.getboolean("remote", "PARALLEL")
-        self.clean_server_report_dir = conf.getboolean(
-            "remote", "CLEAN_SERVER_REPORT_DIR"
-        )
-        self.clean_client_report_dir = conf.getboolean(
-            "remote", "CLEAN_CLIENT_REPORT_DIR"
-        )
-        self.send_code = conf.getboolean("remote", "SEND_CODE")
-        self.scan = conf.getint("remote", "SCAN")
-        self.client_env = conf.getboolean("remote", "BUILD_ENV")
-        self.client_password = conf.get("remote", "CLIENT_PASSWORD")
+        self.parallel = conf.PARALLEL
+        self.clean_server_report_dir = conf.CLEAN_SERVER_REPORT_DIR
+        self.clean_client_report_dir = conf.CLEAN_CLIENT_REPORT_DIR
+        self.send_code = conf.SEND_CODE
+        self.scan = int(conf.SCAN)
+        self.client_env = conf.BUILD_ENV
+        self.client_password = conf.CLIENT_PASSWORD
 
         self._default = {
             Args.client_password.value: remote_kwargs.get("client_password") or self.client_password,
         }
 
-        self.ini_client_dict = {
-            op: [
-                conf.get(op, "user"),
-                conf.get(op, "ip"),
-                conf.get(op, "password", fallback=self._default.get(Args.client_password.value)),
-            ]
-            for op in filter(lambda x: "client" in x, conf.sections())
-        }
-
-        cli_client_dict = {}
-        if remote_kwargs.get("clients"):
-            clients = remote_kwargs.get("clients").split("/")
+        client_dict = {}
+        _client = remote_kwargs.get("clients") or conf.CLIENTS
+        if _client:
+            clients = _client.split("/")
             for index, client in enumerate(clients):
                 client_info = re.findall(r"^(.+?)@(\d+\.\d+\.\d+\.\d+):{0,1}(.*?)$", client)
                 if client_info:
                     _c = list(client_info[0])
                     if _c[2] == "":
                         _c[2] = self._default.get(Args.client_password.value)
-                    cli_client_dict[f"client{index + 1}"] = _c
+                    client_dict[f"client{index + 1}"] = _c
 
-        if not cli_client_dict and not self.ini_client_dict:
+        else:
             raise ValueError(
-                "未获取到测试机信息,请检查 setting/remote.ini 中 CLIENT LIST 是否配置，"
+                "未获取到测试机信息,请检查 setting/globalconfig.ini 中 CLIENT LIST 是否配置，"
                 "或通过命令行 remote -c user@ip:password 传入。"
             )
 
         self.default = {
             Args.app_name.value: transform_app_name(local_kwargs.get("app_name") or GlobalConfig.APP_NAME),
-            Args.clients.value: cli_client_dict or self.ini_client_dict,
+            Args.clients.value: client_dict,
             Args.send_code.value: remote_kwargs.get("send_code") or self.send_code,
             Args.build_env.value: remote_kwargs.get("build_env") or self.client_env,
             Args.parallel.value: remote_kwargs.get("parallel") or self.parallel,
         }
         # 客户端地址
         if "/home/" not in GlobalConfig.ROOT_DIR:
             raise EnvironmentError
```

### Comparing `youqu-2.5.2/youqu/src/utils/check_python_source.py` & `youqu-2.5.3/youqu/src/utils/check_python_source.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/utils/opencv_rpc_server.py` & `youqu-2.5.3/youqu/src/utils/opencv_rpc_server.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/utils/pycharm.sh` & `youqu-2.5.3/youqu/src/utils/pycharm.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/utils/sslclone.sh` & `youqu-2.5.3/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/utils/sub_deb.py` & `youqu-2.5.3/youqu/src/utils/sub_deb.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/src/utils/vnc.sh` & `youqu-2.5.3/youqu/src/utils/vnc.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.2/youqu/README.md` & `youqu-2.5.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,137 @@
+Metadata-Version: 2.1
+Name: youqu
+Version: 2.5.3
+Summary: youqu
+Project-URL: Source, https://github.com/linuxdeepin/youqu
+Project-URL: Documentation, https://linuxdeepin.github.io/youqu
+Author-email: mikigo <huangmingqiang@uniontech.com>
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 <p align="center">
-  <a href="https://linuxdeepin.github.io/deepin-autotest-framework/">
+  <a href="https://linuxdeepin.github.io/youqu/">
     <img src="./docs/logo.png" width="520" alt="YouQu">
   </a>
 </p>
-
 <p align="center">
-    <em>有趣，一个使用简单且功能强大的自动化测试基础框架。</em>
+    <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
-[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/pulls)
-[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/discussions)
+
+
+[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
+[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
 
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
 ![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-![Static Badge](https://img.shields.io/badge/Linux-Platform?style=flat&label=Platform&color=%23F79431)
-![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=flat&logo=MaterialForMkDocs&logoColor=white&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
 
-[![Hits](https://hits.sh/github.com/linuxdeepin/deepin-autotest-framework.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/deepin-autotest-framework)
-[![Hits](https://hits.sh/linuxdeepin.github.io/deepin-autotest-framework.svg?style=flat&label=YouQu_Hits&color=blue)](https://linuxdeepin.github.io/deepin-autotest-framework)
-[![Hits](https://hits.sh/youqu.uniontech.com.svg?style=flat&label=YouQu内网_Hits&color=blue)](http://youqu.uniontech.com/)
-[![Hits](https://hits.sh/pypi.org/project/youqu.svg?style=flat&label=PyPI_Hits&color=blue)](https://pypi.org/project/youqu/)
+[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
-**文档**: <a href="https://linuxdeepin.github.io/deepin-autotest-framework" target="_blank">https://linuxdeepin.github.io/deepin-autotest-framework</a>
+<a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
-**源码**: <a href="https://github.com/linuxdeepin/deepin-autotest-framework" target="_blank">https://github.com/linuxdeepin/deepin-autotest-framework</a>
+<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a> | <a href="https://deepin-community.gitee.io/youqu/" target="_blank">在线文档（国内加速）</a>
 
 ---
 
-有趣（YouQu）是深度科技开源的一个用于 `Deepin/UOS` 操作系统（Linux）的自动化测试框架，采用结构分层的设计理念，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
-
-### 爱上 “有趣” 的 18 个理由
+YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
 
-1. 核心库提供了统一的接口，编写方法时只需要导入一个包就可以使用到核心库提供的所有功能；
-2. 公共库封装了很多常用模块的相关方法，比如：任务栏的操作、桌面的操作、右键菜单的操作等等；
-3. 除了常用的属性定位、图像识别以外，我们还提供基于 `UI` 的元素定位方案，其使用简单且高效，效果一定能惊讶到你；
-4. 对属性定位的方法进行了二次封装，将编写属性定位的方法变得简单而优雅；
-5. 对图像识别定位技术进行功能升级，除了支持单个坐标返回，还支持同一界面下多个相同元素返回多个坐标的功能；
-6. 提供用例标签化管理、批量跳过和批量条件跳过的功能，你想不到一个 `csv` 文件原来能干这么多事情；
-7. 提供了功能强大的执行器入口，让你可以方便的在本地执行任何用例集的用例，其丰富的自定义配置项，满足你对执行器所有的幻想；
-8. 提供远程执行的功能，可以控制多台机器并行跑，或者分布式跑，这种付费功能现在免费给你用；
-9. 提供自动输出日志的功能，你再也不用为每个方法单独写输出日志的代码，一切我们给你搞定了，日志输出不仅内容丰富，颜值也绝对在线，我们还自己设计了一款终端输出主题叫《五彩斑斓的黑》；
-10. 提供一键部署自动化测试环境的功能，让你再也不用为环境部署而烦恼；
-11. 提供自动生成多种报告的功能，你想输出什么报告形式都行，而且我们在报告中还加入了失败录屏和失败截图的功能；
-12. 对断言进行了二次封装，提供更友好化的错误提示，让定位问题精准高效；
-13. 不仅支持单条用例超时控制，而且还支持动态控制用例批量执行的总时间，确保 `CI` 环境下能顺畅运行；
-14. 支持本地文件测试套执行、`PMS` 测试套执行、标签化执行方案，满足你各种场景下的执行需求；
-15. 支持基于深度学习的 `OCR` 功能，可定位可断言，中文识别的天花板；
-16. 完美兼容 `Wayland`  和 `X11`，真正做到一套代码，随处执行；
-17. 支持多种方式的数据回填功能，其中异步回填的方案，完美解决了数据回填的耗时问题；
-18. 支持重启交互场景用例的执行，使用方法优雅简洁；
+## YouQu（有趣）能做什么
 
-------------------------
+- [x] Linux 桌面应用 UI 自动化测试
+- [x] Linux 桌面应用 DBus/Gsettings 接口自动化测试
+- [x] 命令行自动化测试
+- [x] HTTP 接口自动化测试
+- [x] Web UI 自动化测试
+- [ ] Linux 桌面应用性能自动化测试
+
+<details>
+	<summary style="color: #FF9933">点击查看爱上 “有趣（YouQu）” 的 N 个理由</summary>
+	<ul>
+        <li>无处不在的代码补全，让编写自动化测试用例成为一种享受；</li>
+        <li>核心库提供了统一的接口，编写方法时只需要导入一个包就可以使用到核心库提供的所有功能；</li>
+        <li>除了常用的属性定位、图像识别以外，我们还提供基于 UI 的元素定位方案，其使用简单且高效，效果一定能惊讶到你；</li>
+        <li>对属性定位的方法进行了二次封装，将编写属性定位的方法变得简单而优雅；</li>
+        <li>对图像识别定位技术进行功能升级，除了支持单个坐标返回，还支持同一界面下多个相同元素返回多个坐标的功能；</li>
+        <li>提供用例标签化管理、批量跳过和批量条件跳过的功能，你想不到一个 csv 文件原来能干这么多事情；</li>
+        <li>提供了功能强大的执行器入口，让你可以方便的在本地执行任何用例集的用例，其丰富的自定义配置项，满足你对执行器所有的幻想；</li>
+        <li>提供远程执行的功能，可以控制多台机器并行跑，或者分布式跑，这种付费功能现在免费给你用；</li>
+        <li>提供自动输出日志的功能，你再也不用为每个方法单独写输出日志的代码，一切我们给你搞定了，日志输出不仅内容丰富，颜值也绝对在线，我们还自己设计了一款终端输出主题叫《五彩斑斓的黑》；</li>
+        <li>提供一键部署自动化测试环境的功能，让你再也不用为环境部署而烦恼；</li>
+        <li>提供自动生成多种报告的功能，你想输出什么报告形式都行，而且我们在报告中还加入了失败录屏和失败截图的功能；</li>
+        <li>对断言进行了二次封装，提供更友好化的错误提示，让定位问题精准高效；</li>
+        <li>不仅支持单条用例超时控制，而且还支持动态控制用例批量执行的总时间，确保 CI 环境下能顺畅运行；</li>
+        <li>支持本地文件测试套执行、PMS 测试套执行、标签化执行方案，满足你各种场景下的执行需求；</li>
+        <li>支持基于深度学习的 OCR 功能，可定位可断言，中文识别的天花板；</li>
+        <li>完美兼容 Wayland  和 X11，真正做到一套代码，随处执行；</li>
+        <li>支持多种方式的数据回填功能，其中异步回填的方案，完美解决了数据回填的耗时问题；</li>
+        <li>支持重启交互场景用例的执行，使用方法优雅简洁；</li>
+    </ul>
+</details>
 
-统信公司内网还可以访问【[内网文档](http://youqu.uniontech.com/)】，文档内容一样，访问速度更快哦~~
-
-## 安装使用
+## 安装
 
 从 PyPI 安装:
 
-<div class="termy">
 
-```console
+```shell
 $ sudo pip3 install youqu
----> 100%
 ```
 
-</div>
-
 创建项目:
 
-<div class="termy">
-
-```console
+```shell
 $ youqu-startproject my_project
----> 100%
-The project: [my_project],has been created by youqu-x.x.x
 ```
 
-</div>
-
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
 安装依赖:
 
-<div class="termy">
-
-```console
-// 如果你的测试机密码不是 `1` ，那你需要在全局配置文件 `globalconfig.ini` 里面将 `PASSWORD` 配置项修改为当前测试机的密码。
+```shell
 $ cd my_project
-$ bash env.sh
----> 100%
-```
 
-</div>
+# 使用的默认密码是 1 ，您可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项
+$ bash env.sh
 
--------------------------------
+# 也可以使用 -p 选项传入密码
+$ bash env.sh -p ${my_password}
+```
 
-**【APP工程】**
+## 创建工程
 
 如果您已经有一个可用的 `APP` 工程，将应用库放到基础框架下 `apps` 目录下，像这样：
 
-```shell hl_lines="3"
+```shell
 my_project
 ├── apps
 │   ├── autotest_deepin_music  # 应用库
 ...
 ```
 
 如果您还没有 `APP` 工程，建议使用框架提供的脚手架功能创建一个全新的 `APP` 工程。
 
-## 创建工程
-
-创建一个 APP 工程：
-
-<div class="termy">
+**创建一个 APP 工程**
 
-```console
+```shell
 $ youqu manage.py startapp autotest_deepin_some
----> 100%
 ```
 
-</div>
-
 这样在 `apps` 目录下会创建一个子项目工程 `autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 apps
 └── autotest_deepin_some
     ├── case
     │   ├── assert_res
@@ -170,118 +167,57 @@
 
 ### 1. 工作空间
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
 ### 2. 本地执行
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run
 ```
 
-</div>
-
 #### 2.1. 命令行参数
 
 通过命令行参数配置参数，使用 `-h` 或 `--help` 可以查看所有支持的命令行参数：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run -h
 ```
 
-</div>
-
 在一些 CI 环境下使用命令行参数会更加方便：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags "xxx"
 ```
 
-</div>
-
-更多参数请查看【[命令行参数](https://linuxdeepin.github.io/deepin-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
+更多参数请查看【[命令行参数](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
 
 #### 2.2. 配置文件
 
 通过配置文件配置参数
 
 在配置文件 `setting/globalconfig.ini` 里面支持配置对执行的一些参数进行配置，配置完成之后，直接在命令行执行 `manage.py` 就好了。
 
-详细配置项请查看【[配置项](https://linuxdeepin.github.io/deepin-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
+详细配置项请查看【[配置项](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
 
 ### 3. 远程执行
 
 远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同；
 
 使用 `remote` 命令：
 
-<div class="termy">
-
-```console
-$ youqu manage.py remote
-```
-
-</div>
 
-#### 3.1. 远程多机器分布式异步执行
-
-![](https://pic.imgdb.cn/item/64f6d3c0661c6c8e549f8ca5.png)
-
-多机器分布式异步执行就是由本地 YouQu 作为服务端，控制远程 N 台机器执行相同的用例，执行完之后所有测试机的测试结果会返回给服务端 report 目录下；
-
-远程执行同样通过配置文件 `setting/globalconfig.ini` 进行用例相关配置；
-
-需要重点说一下远程执行时的测试机信息配置，在配置文件 `setting/remote.ini`  里面配置测试机的用户名、IP、密码。
-
-```ini
-;=============================== CLIENT LIST =====================================
-; 测试机配置列表
-;[client{number}]     ;测试机别名，有多少台测试机就写多少个 client，别名必须包含 client 字符，且不能重复。
-;user =               ;测试机 user
-;ip =                 ;测试机 ip
-;password = 1         ;测试机的密码, 可以不配置此项，默认取 CLIENT_PASSWORD 的值；
-                      ;如果你所有测试机密码都相同，那么只需要配置 CLIENT_PASSWORD 就可以了
-;=================================================================================
-
-[client1]
-user = uos
-ip = 10.8.15.xx
-
-[client2]
-user = uos
-ip = 10.8.15.xx
-
-[client3]
-user = uos
-ip = 10.8.11.xx
-```
-
-有多少台机器就像这样参考上面的格式写就行了。
-
-然后在命令行：
-
-<div class="termy">
-
-```console
+```shell
 $ youqu manage.py remote
 ```
 
-</div>
-
-这样运行是从配置文件去读取相关配置。
-
-如果你不想通过配置文件，你仍然通过命令行参数进行传参，
-
-以下为 `python3 manage.py remote` 提供的一些参数选项：
+以下为 `remote` 提供的一些参数选项：
 
 ```coffeescript
   -h, --help            show this help message and exit
   -c CLIENTS, --clients CLIENTS
                         远程机器的user@ip:password,多个机器用'/'连接,如果password不传入,默认取sett
                         ing/remote.ini中CLIENT_PASSWORD的值,比如: uos@10.8.13.xx:1
                         或 uos@10.8.13.xx
@@ -290,86 +226,55 @@
   -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
                         测试机密码（全局）
   -y PARALLEL, --parallel PARALLEL
                         yes:表示所有测试机并行跑，执行相同的测试用例;no:表示测试机分布式执行，服务端会根据收集到的测试用例自
                         动分配给各个测试机执行。
 ```
 
-==除了这些特有参数以外，它同样支持本地执行的所有参数；==
+除了这些特有参数以外，它同样支持本地执行的所有参数；
 
 在命令行这样运行：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py remote -a apps/autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx"
 ```
 
-</div>
-
 所有用例执行完之后会在 `report` 目录下回收各个测试机执行的测试报告。
 
 注意：如果远程机器没有搭建自动化测试环境，记得加上参数 `-e` ：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py remote -a ... -e
 ```
 
-</div>
-
 执行前确保远程机器已经开启了 ssh 服务，否则会提示无法连接，如果没有开启，请手动开启：
 
-<div class="termy">
 
-```console
+```shell
 $ sudo systemctl restart ssh
 $ sudo systemctl enable ssh
 ```
 
-</div>
-
 配置文件其他相关配置项详细说明，请查看配置文件中的注释内容。
 
-#### 3.2. 远程多机器分布式异步负载均衡执行
-
-多机器分布式异步负载均衡执行也是用本地作为服务端控制远程机器执行，但远程机器执行的用例不同，而是所有远程机器执行的用例之和，为你想要执行的用例集；
-
-似乎有点难以理解，我用大白话举例描述下：
-
-服务端想要执行 10 条用例，现在远程机器有 5 台，然后服务端就先拿着第 1 条用例给远程 1 号机执行，拿第 2 条用例给远程 2 号机执行...，如此循环直到所有用例执行完，这就是负载均衡执行。
-
-![](https://pic.imgdb.cn/item/64f6d694661c6c8e54a1025b.png)
-
-使用方法和前面一样，只是需要增加一个参数 `--parallel`：
-
-<div class="termy">
-
-```console
-$ youqu manage.py remote -a ... --parallel no
-```
-
-</div>
-
-## 贡献者
-
-[贡献文档](https://github.com/linuxdeepin/deepin-autotest-framework/blob/master/CONTRIBUTING.md) 
+## 贡献
 
---8<-- "docs/contributors.html"
+[贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
 
 
 ## 开源许可证
 
-有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/deepin-autotest-framework/blob/master/LICENSE) 下发布。
+有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
 
 ------------
 
 [__Github Star History__]()
 
-[![Stargazers over time](https://starchart.cc/linuxdeepin/deepin-autotest-framework.svg)](https://starchart.cc/linuxdeepin/deepin-autotest-framework)
+[![Stargazers over time](https://starchart.cc/linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu)
 
 
 
 [__Gitee Info__]()
 
-[![deepin-community/deepin-autotest-framework](https://gitee.com/deepin-community/deepin-autotest-framework/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/deepin-autotest-framework)
+[![deepin-community/youqu](https://gitee.com/deepin-community/youqu/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/youqu)
```

#### html2text {}

```diff
@@ -1,100 +1,81 @@
+Metadata-Version: 2.1 Name: youqu Version: 2.5.3 Summary: youqu Project-URL:
+Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
+//linuxdeepin.github.io/youqu Author-email: mikigo
+uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
+License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
+Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
-  ?æ???è?¶?£?ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
-[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/deepin-
-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-
-autotest-framework/issues) [![GitHub pull requests](https://img.shields.io/
-github/issues-pr/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https:
-//github.com/linuxdeepin/deepin-autotest-framework/pulls) [![GitHub
-Discussions](https://img.shields.io/github/discussions/linuxdeepin/deepin-
-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-
-autotest-framework/discussions) [![PyPI](https://img.shields.io/pypi/v/
+YYoouuQQuu?ï?¼??æ???è?¶?£?ï?¼??ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
+[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![GitHub
+pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls) [![GitHub
+Discussions](https://img.shields.io/github/discussions/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions) [!
+[PyPI](https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
 (https://pypi.org/project/youqu/) ![PyPI - License](https://img.shields.io/
 pypi/l/youqu?color=%23F79431) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
 badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-![Static Badge](https://img.shields.io/badge/Linux-
-Platform?style=flat&label=Platform&color=%23F79431) ![Built with Material for
-MkDocs](https://img.shields.io/badge/Material_for_MkDocs-
-526CFE?style=flat&logo=MaterialForMkDocs&logoColor=white&color=%23F79431) [!
-[Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
+[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
 project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
 (https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
 youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
-linuxdeepin/deepin-autotest-
-framework.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/
-linuxdeepin/deepin-autotest-framework) [![Hits](https://hits.sh/
-linuxdeepin.github.io/deepin-autotest-
-framework.svg?style=flat&label=YouQu_Hits&color=blue)](https://
-linuxdeepin.github.io/deepin-autotest-framework) [![Hits](https://hits.sh/
-youqu.uniontech.com.svg?style=flat&label=YouQuåç½_Hits&color=blue)](http://
-youqu.uniontech.com/) [![Hits](https://hits.sh/pypi.org/project/
-youqu.svg?style=flat&label=PyPI_Hits&color=blue)](https://pypi.org/project/
-youqu/) --- **ææ¡£**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_d_e_e_p_i_n_-_a_u_t_o_t_e_s_t_-_f_r_a_m_e_w_o_r_k
-**æºç **: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_d_e_e_p_i_n_-_a_u_t_o_t_e_s_t_-_f_r_a_m_e_w_o_r_k --
-- æè¶£ï¼YouQuï¼æ¯æ·±åº¦ç§æå¼æºçä¸ä¸ªç¨äº `Deepin/UOS`
-æä½ç³»ç»ï¼Linuxï¼çèªå¨åæµè¯æ¡æ¶ï¼éç¨ç»æåå±çè®¾è®¡çå¿µï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
-X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ### ç±ä¸
-âæè¶£â ç 18 ä¸ªçç± 1.
-æ ¸å¿åºæä¾äºç»ä¸çæ¥å£ï¼ç¼åæ¹æ³æ¶åªéè¦å¯¼å¥ä¸ä¸ªåå°±å¯ä»¥ä½¿ç¨å°æ ¸å¿åºæä¾çææåè½ï¼
-2.
-å¬å±åºå°è£äºå¾å¤å¸¸ç¨æ¨¡åçç¸å³æ¹æ³ï¼æ¯å¦ï¼ä»»å¡æ çæä½ãæ¡é¢çæä½ãå³é®èåçæä½ç­ç­ï¼
-3. é¤äºå¸¸ç¨çå±æ§å®ä½ãå¾åè¯å«ä»¥å¤ï¼æä»¬è¿æä¾åºäº
-`UI`
-çåç´ å®ä½æ¹æ¡ï¼å¶ä½¿ç¨ç®åä¸é«æï¼ææä¸å®è½æè®¶å°ä½ ï¼
-4.
-å¯¹å±æ§å®ä½çæ¹æ³è¿è¡äºäºæ¬¡å°è£ï¼å°ç¼åå±æ§å®ä½çæ¹æ³åå¾ç®åèä¼éï¼
-5.
-å¯¹å¾åè¯å«å®ä½ææ¯è¿è¡åè½åçº§ï¼é¤äºæ¯æåä¸ªåæ è¿åï¼è¿æ¯æåä¸çé¢ä¸å¤ä¸ªç¸ååç´ è¿åå¤ä¸ªåæ çåè½ï¼
-6.
-æä¾ç¨ä¾æ ç­¾åç®¡çãæ¹éè·³è¿åæ¹éæ¡ä»¶è·³è¿çåè½ï¼ä½ æ³ä¸å°ä¸ä¸ª
-`csv` æä»¶åæ¥è½å¹²è¿ä¹å¤äºæï¼ 7.
-æä¾äºåè½å¼ºå¤§çæ§è¡å¨å¥å£ï¼è®©ä½ å¯ä»¥æ¹ä¾¿çå¨æ¬å°æ§è¡ä»»ä½ç¨ä¾éçç¨ä¾ï¼å¶ä¸°å¯çèªå®ä¹éç½®é¡¹ï¼æ»¡è¶³ä½ å¯¹æ§è¡å¨ææçå¹»æ³ï¼
-8.
-æä¾è¿ç¨æ§è¡çåè½ï¼å¯ä»¥æ§å¶å¤å°æºå¨å¹¶è¡è·ï¼æèåå¸å¼è·ï¼è¿ç§ä»è´¹åè½ç°å¨åè´¹ç»ä½ ç¨ï¼
-9.
-æä¾èªå¨è¾åºæ¥å¿çåè½ï¼ä½ åä¹ä¸ç¨ä¸ºæ¯ä¸ªæ¹æ³åç¬åè¾åºæ¥å¿çä»£ç ï¼ä¸åæä»¬ç»ä½ æå®äºï¼æ¥å¿è¾åºä¸ä»åå®¹ä¸°å¯ï¼é¢å¼ä¹ç»å¯¹å¨çº¿ï¼æä»¬è¿èªå·±è®¾è®¡äºä¸æ¬¾ç»ç«¯è¾åºä¸»é¢å«ãäºå½©ææçé»ãï¼
-10.
-æä¾ä¸é®é¨ç½²èªå¨åæµè¯ç¯å¢çåè½ï¼è®©ä½ åä¹ä¸ç¨ä¸ºç¯å¢é¨ç½²èç¦æ¼ï¼
-11.
-æä¾èªå¨çæå¤ç§æ¥åçåè½ï¼ä½ æ³è¾åºä»ä¹æ¥åå½¢å¼é½è¡ï¼èä¸æä»¬å¨æ¥åä¸­è¿å å¥äºå¤±è´¥å½å±åå¤±è´¥æªå¾çåè½ï¼
-12.
-å¯¹æ­è¨è¿è¡äºäºæ¬¡å°è£ï¼æä¾æ´åå¥½åçéè¯¯æç¤ºï¼è®©å®ä½é®é¢ç²¾åé«æï¼
-13.
-ä¸ä»æ¯æåæ¡ç¨ä¾è¶æ¶æ§å¶ï¼èä¸è¿æ¯æå¨ææ§å¶ç¨ä¾æ¹éæ§è¡çæ»æ¶é´ï¼ç¡®ä¿
-`CI` ç¯å¢ä¸è½é¡ºçè¿è¡ï¼ 14. æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ã`PMS`
-æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
-15. æ¯æåºäºæ·±åº¦å­¦ä¹ ç `OCR`
-åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼ 16. å®ç¾å¼å®¹
-`Wayland` å `X11`ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼ 17.
-æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
-18. æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼ -----
-------------------- ç»ä¿¡å¬å¸åç½è¿å¯ä»¥è®¿é®ã[åç½ææ¡£](http://
-youqu.uniontech.com/)ãï¼ææ¡£åå®¹ä¸æ ·ï¼è®¿é®éåº¦æ´å¿«å¦~~ ##
-å®è£ä½¿ç¨ ä» PyPI å®è£:
-```console $ sudo pip3 install youqu ---> 100% ```
-åå»ºé¡¹ç®:
-```console $ youqu-startproject my_project ---> 100% The project:
-[my_project],has been created by youqu-x.x.x ```
-å¦æ `youqu-startproject`
+linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
+github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ |
+_å__¨_ç_º_¿_æ___æ_¡_£_ï_¼__å__½_å___å__ _é___ï_¼_ --
+- YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
+æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
+X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ##
+YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] Linux æ¡é¢åºç¨ UI èªå¨åæµè¯ - [x]
+Linux æ¡é¢åºç¨ DBus/Gsettings æ¥å£èªå¨åæµè¯ - [x]
+å½ä»¤è¡èªå¨åæµè¯ - [x] HTTP æ¥å£èªå¨åæµè¯ - [x] Web UI
+èªå¨åæµè¯ - [ ] Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯
+ç¹å»æ¥çç±ä¸ âæè¶£ï¼YouQuï¼â ç N ä¸ªçç±
+    * æ å¤ä¸å¨çä»£ç è¡¥å¨ï¼è®©ç¼åèªå¨åæµè¯ç¨ä¾æä¸ºä¸ç§äº«åï¼
+    * æ ¸å¿åºæä¾äºç»ä¸çæ¥å£ï¼ç¼åæ¹æ³æ¶åªéè¦å¯¼å¥ä¸ä¸ªåå°±å¯ä»¥ä½¿ç¨å°æ ¸å¿åºæä¾çææåè½ï¼
+    * é¤äºå¸¸ç¨çå±æ§å®ä½ãå¾åè¯å«ä»¥å¤ï¼æä»¬è¿æä¾åºäº
+      UI
+      çåç´ å®ä½æ¹æ¡ï¼å¶ä½¿ç¨ç®åä¸é«æï¼ææä¸å®è½æè®¶å°ä½ ï¼
+    * å¯¹å±æ§å®ä½çæ¹æ³è¿è¡äºäºæ¬¡å°è£ï¼å°ç¼åå±æ§å®ä½çæ¹æ³åå¾ç®åèä¼éï¼
+    * å¯¹å¾åè¯å«å®ä½ææ¯è¿è¡åè½åçº§ï¼é¤äºæ¯æåä¸ªåæ è¿åï¼è¿æ¯æåä¸çé¢ä¸å¤ä¸ªç¸ååç´ è¿åå¤ä¸ªåæ çåè½ï¼
+    * æä¾ç¨ä¾æ ç­¾åç®¡çãæ¹éè·³è¿åæ¹éæ¡ä»¶è·³è¿çåè½ï¼ä½ æ³ä¸å°ä¸ä¸ª
+      csv æä»¶åæ¥è½å¹²è¿ä¹å¤äºæï¼
+    * æä¾äºåè½å¼ºå¤§çæ§è¡å¨å¥å£ï¼è®©ä½ å¯ä»¥æ¹ä¾¿çå¨æ¬å°æ§è¡ä»»ä½ç¨ä¾éçç¨ä¾ï¼å¶ä¸°å¯çèªå®ä¹éç½®é¡¹ï¼æ»¡è¶³ä½ å¯¹æ§è¡å¨ææçå¹»æ³ï¼
+    * æä¾è¿ç¨æ§è¡çåè½ï¼å¯ä»¥æ§å¶å¤å°æºå¨å¹¶è¡è·ï¼æèåå¸å¼è·ï¼è¿ç§ä»è´¹åè½ç°å¨åè´¹ç»ä½ ç¨ï¼
+    * æä¾èªå¨è¾åºæ¥å¿çåè½ï¼ä½ åä¹ä¸ç¨ä¸ºæ¯ä¸ªæ¹æ³åç¬åè¾åºæ¥å¿çä»£ç ï¼ä¸åæä»¬ç»ä½ æå®äºï¼æ¥å¿è¾åºä¸ä»åå®¹ä¸°å¯ï¼é¢å¼ä¹ç»å¯¹å¨çº¿ï¼æä»¬è¿èªå·±è®¾è®¡äºä¸æ¬¾ç»ç«¯è¾åºä¸»é¢å«ãäºå½©ææçé»ãï¼
+    * æä¾ä¸é®é¨ç½²èªå¨åæµè¯ç¯å¢çåè½ï¼è®©ä½ åä¹ä¸ç¨ä¸ºç¯å¢é¨ç½²èç¦æ¼ï¼
+    * æä¾èªå¨çæå¤ç§æ¥åçåè½ï¼ä½ æ³è¾åºä»ä¹æ¥åå½¢å¼é½è¡ï¼èä¸æä»¬å¨æ¥åä¸­è¿å å¥äºå¤±è´¥å½å±åå¤±è´¥æªå¾çåè½ï¼
+    * å¯¹æ­è¨è¿è¡äºäºæ¬¡å°è£ï¼æä¾æ´åå¥½åçéè¯¯æç¤ºï¼è®©å®ä½é®é¢ç²¾åé«æï¼
+    * ä¸ä»æ¯æåæ¡ç¨ä¾è¶æ¶æ§å¶ï¼èä¸è¿æ¯æå¨ææ§å¶ç¨ä¾æ¹éæ§è¡çæ»æ¶é´ï¼ç¡®ä¿
+      CI ç¯å¢ä¸è½é¡ºçè¿è¡ï¼
+    * æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ãPMS
+      æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
+    * æ¯æåºäºæ·±åº¦å­¦ä¹ ç OCR
+      åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼
+    * å®ç¾å¼å®¹ Wayland å X11ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼
+    * æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
+    * æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼
+## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` åå»ºé¡¹ç®:
+```shell $ youqu-startproject my_project ``` å¦æ `youqu-startproject`
 åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ å®è£ä¾èµ:
-```console // å¦æä½ çæµè¯æºå¯ç ä¸æ¯ `1`
-ï¼é£ä½ éè¦å¨å¨å±éç½®æä»¶ `globalconfig.ini` éé¢å° `PASSWORD`
-éç½®é¡¹ä¿®æ¹ä¸ºå½åæµè¯æºçå¯ç ã $ cd my_project $ bash env.sh ---
-> 100% ```
-------------------------------- **ãAPPå·¥ç¨ã**
-å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
+```shell $ cd my_project # ä½¿ç¨çé»è®¤å¯ç æ¯ 1
+ï¼æ¨å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/globalconfig.ini éé¢ç PASSWORD
+éç½®é¡¹ $ bash env.sh # ä¹å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç  $ bash env.sh -
+p ${my_password} ``` ## åå»ºå·¥ç¨ å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
 å·¥ç¨ï¼å°åºç¨åºæ¾å°åºç¡æ¡æ¶ä¸ `apps` ç®å½ä¸ï¼åè¿æ ·ï¼
-```shell hl_lines="3" my_project âââ apps â âââ
-autotest_deepin_music # åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
+```shell my_project âââ apps â âââ autotest_deepin_music #
+åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
 å·¥ç¨ï¼å»ºè®®ä½¿ç¨æ¡æ¶æä¾çèææ¶åè½åå»ºä¸ä¸ªå¨æ°ç `APP`
-å·¥ç¨ã ## åå»ºå·¥ç¨ åå»ºä¸ä¸ª APP å·¥ç¨ï¼
-```console $ youqu manage.py startapp autotest_deepin_some ---> 100% ```
-è¿æ ·å¨ `apps` ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
+å·¥ç¨ã **åå»ºä¸ä¸ª APP å·¥ç¨** ```shell $ youqu manage.py startapp
+autotest_deepin_some ``` è¿æ ·å¨ `apps`
+ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
 `autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
 ```shell apps âââ autotest_deepin_some Â Â  âââ case Â Â  âÂ Â 
 âââ assert_res Â Â  âÂ Â  âÂ Â  âââ readme Â Â  âÂ Â 
 âââ base_case.py Â Â  âÂ Â  âââ __init__.py Â Â  âââ
 config.ini Â Â  âââ config.py Â Â  âââ conftest.py Â Â  âââ
 control Â Â  âââ deepin_some_assert.py Â Â  âââ deepin_some.csv
 Â Â  âââ __init__.py Â Â  âââ widget Â Â  âââ base_widget.py
@@ -103,98 +84,55 @@
 âââ other_widget.py Â Â  âââ pic_res Â Â  âÂ Â  âââ readme
 Â Â  âââ ui.ini ``` `autotest_deepin_some`
 æ¯ä½ çå·¥ç¨åç§°ï¼æ¯å¦ï¼`autotest_deepin_music` ï¼
 å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã è¿è¡ ------- ### 1.
 å·¥ä½ç©ºé´ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
-### 2. æ¬å°æ§è¡
-```console $ youqu manage.py run ```
-#### 2.1. å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ
-`--help` å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼
-```console $ youqu manage.py run -h ```
-å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
-```console $ youqu manage.py run --app apps/autotest_deepin_music --keywords
-"xxx" --tags "xxx" ```
-æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://linuxdeepin.github.io/deepin-
-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
+### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
+å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ `--help`
+å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼ ```shell $ youqu manage.py run -
+h ``` å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $
+youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags
+"xxx" ``` æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://
+linuxdeepin.github.io/youqu/
+%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
 %E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)ã #### 2.2. éç½®æä»¶
 éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ `setting/globalconfig.ini`
 éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ï¼éç½®å®æä¹åï¼ç´æ¥å¨å½ä»¤è¡æ§è¡
 `manage.py` å°±å¥½äºã è¯¦ç»éç½®é¡¹è¯·æ¥çã[éç½®é¡¹](https://
-linuxdeepin.github.io/deepin-autotest-framework/
+linuxdeepin.github.io/youqu/
 %E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
 %E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)ã ### 3. è¿ç¨æ§è¡
 è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åï¼
-ä½¿ç¨ `remote` å½ä»¤ï¼
-```console $ youqu manage.py remote ```
-#### 3.1. è¿ç¨å¤æºå¨åå¸å¼å¼æ­¥æ§è¡ ![](https://pic.imgdb.cn/item/
-64f6d3c0661c6c8e549f8ca5.png) å¤æºå¨åå¸å¼å¼æ­¥æ§è¡å°±æ¯ç±æ¬å°
-YouQu ä½ä¸ºæå¡ç«¯ï¼æ§å¶è¿ç¨ N
-å°æºå¨æ§è¡ç¸åçç¨ä¾ï¼æ§è¡å®ä¹åæææµè¯æºçæµè¯ç»æä¼è¿åç»æå¡ç«¯
-report ç®å½ä¸ï¼ è¿ç¨æ§è¡åæ ·éè¿éç½®æä»¶ `setting/
-globalconfig.ini` è¿è¡ç¨ä¾ç¸å³éç½®ï¼
-éè¦éç¹è¯´ä¸ä¸è¿ç¨æ§è¡æ¶çæµè¯æºä¿¡æ¯éç½®ï¼å¨éç½®æä»¶
-`setting/remote.ini` éé¢éç½®æµè¯æºçç¨æ·åãIPãå¯ç ã ```ini
-;=============================== CLIENT LIST
-===================================== ; æµè¯æºéç½®åè¡¨ ;[client{number}]
-;æµè¯æºå«åï¼æå¤å°å°æµè¯æºå°±åå¤å°ä¸ª
-clientï¼å«åå¿é¡»åå« client å­ç¬¦ï¼ä¸ä¸è½éå¤ã ;user =
-;æµè¯æº user ;ip = ;æµè¯æº ip ;password = 1 ;æµè¯æºçå¯ç ,
-å¯ä»¥ä¸éç½®æ­¤é¡¹ï¼é»è®¤å CLIENT_PASSWORD çå¼ï¼
-;å¦æä½ æææµè¯æºå¯ç é½ç¸åï¼é£ä¹åªéè¦éç½®
-CLIENT_PASSWORD å°±å¯ä»¥äº
-;=================================================================================
-[client1] user = uos ip = 10.8.15.xx [client2] user = uos ip = 10.8.15.xx
-[client3] user = uos ip = 10.8.11.xx ```
-æå¤å°å°æºå¨å°±åè¿æ ·åèä¸é¢çæ ¼å¼åå°±è¡äºã
-ç¶åå¨å½ä»¤è¡ï¼
-```console $ youqu manage.py remote ```
-è¿æ ·è¿è¡æ¯ä»éç½®æä»¶å»è¯»åç¸å³éç½®ã
-å¦æä½ ä¸æ³éè¿éç½®æä»¶ï¼ä½ ä»ç¶éè¿å½ä»¤è¡åæ°è¿è¡ä¼ åï¼
-ä»¥ä¸ä¸º `python3 manage.py remote` æä¾çä¸äºåæ°éé¡¹ï¼
-```coffeescript -h, --help show this help message and exit -c CLIENTS, --
-clients CLIENTS è¿ç¨æºå¨çuser@ip:password,å¤ä¸ªæºå¨ç¨'/
-'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ä»¥ä¸ä¸º
+`remote` æä¾çä¸äºåæ°éé¡¹ï¼ ```coffeescript -h, --help show this
+help message and exit -c CLIENTS, --clients CLIENTS è¿ç¨æºå¨çuser@ip:
+password,å¤ä¸ªæºå¨ç¨'/'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
 remote.iniä¸­CLIENT_PASSWORDçå¼,æ¯å¦: uos@10.8.13.xx:1 æ uos@10.8.13.xx
 -s, --send_code åéä»£ç å°æµè¯æºï¼ä¸å«reportç®å½ï¼ -e, --
 build_env
 æ­å»ºæµè¯ç¯å¢,å¦æä¸ºyesï¼ä¸ç®¡send_codeæ¯å¦ä¸ºyesé½ä¼åéä»£ç å°æµè¯æº.
 -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
 æµè¯æºå¯ç ï¼å¨å±ï¼ -y PARALLEL, --parallel PARALLEL yes:
 è¡¨ç¤ºæææµè¯æºå¹¶è¡è·ï¼æ§è¡ç¸åçæµè¯ç¨ä¾;no:
 è¡¨ç¤ºæµè¯æºåå¸å¼æ§è¡ï¼æå¡ç«¯ä¼æ ¹æ®æ¶éå°çæµè¯ç¨ä¾èª
 å¨åéç»åä¸ªæµè¯æºæ§è¡ã ```
-==é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼==
-å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼
-```console $ youqu manage.py remote -a apps/autotest_deepin_music -
-c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
+é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼
+å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼ ```shell $ youqu manage.py remote -a apps/
+autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
 ææç¨ä¾æ§è¡å®ä¹åä¼å¨ `report`
 ç®å½ä¸åæ¶åä¸ªæµè¯æºæ§è¡çæµè¯æ¥åã
 æ³¨æï¼å¦æè¿ç¨æºå¨æ²¡ææ­å»ºèªå¨åæµè¯ç¯å¢ï¼è®°å¾å ä¸åæ°
-`-e` ï¼
-```console $ youqu manage.py remote -a ... -e ```
+`-e` ï¼ ```shell $ youqu manage.py remote -a ... -e ```
 æ§è¡åç¡®ä¿è¿ç¨æºå¨å·²ç»å¼å¯äº ssh
 æå¡ï¼å¦åä¼æç¤ºæ æ³è¿æ¥ï¼å¦ææ²¡æå¼å¯ï¼è¯·æå¨å¼å¯ï¼
-```console $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
+```shell $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
 éç½®æä»¶å¶ä»ç¸å³éç½®é¡¹è¯¦ç»è¯´æï¼è¯·æ¥çéç½®æä»¶ä¸­çæ³¨éåå®¹ã
-#### 3.2. è¿ç¨å¤æºå¨åå¸å¼å¼æ­¥è´è½½åè¡¡æ§è¡
-å¤æºå¨åå¸å¼å¼æ­¥è´è½½åè¡¡æ§è¡ä¹æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼ä½è¿ç¨æºå¨æ§è¡çç¨ä¾ä¸åï¼èæ¯ææè¿ç¨æºå¨æ§è¡çç¨ä¾ä¹åï¼ä¸ºä½ æ³è¦æ§è¡çç¨ä¾éï¼
-ä¼¼ä¹æç¹é¾ä»¥çè§£ï¼æç¨å¤§ç½è¯ä¸¾ä¾æè¿°ä¸ï¼
-æå¡ç«¯æ³è¦æ§è¡ 10 æ¡ç¨ä¾ï¼ç°å¨è¿ç¨æºå¨æ 5
-å°ï¼ç¶åæå¡ç«¯å°±åæ¿çç¬¬ 1 æ¡ç¨ä¾ç»è¿ç¨ 1
-å·æºæ§è¡ï¼æ¿ç¬¬ 2 æ¡ç¨ä¾ç»è¿ç¨ 2
-å·æºæ§è¡...ï¼å¦æ­¤å¾ªç¯ç´å°ææç¨ä¾æ§è¡å®ï¼è¿å°±æ¯è´è½½åè¡¡æ§è¡ã
-![](https://pic.imgdb.cn/item/64f6d694661c6c8e54a1025b.png)
-ä½¿ç¨æ¹æ³ååé¢ä¸æ ·ï¼åªæ¯éè¦å¢å ä¸ä¸ªåæ° `--parallel`ï¼
-```console $ youqu manage.py remote -a ... --parallel no ```
-## è´¡ç®è [è´¡ç®ææ¡£](https://github.com/linuxdeepin/deepin-autotest-
-framework/blob/master/CONTRIBUTING.md) --8<-- "docs/contributors.html" ##
-å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://github.com/linuxdeepin/
-deepin-autotest-framework/blob/master/LICENSE) ä¸åå¸ã ------------
+## è´¡ç® [è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
+CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://
+github.com/linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã ------------
 [__Github Star History__]() [![Stargazers over time](https://starchart.cc/
-linuxdeepin/deepin-autotest-framework.svg)](https://starchart.cc/linuxdeepin/
-deepin-autotest-framework) [__Gitee Info__]() [![deepin-community/deepin-
-autotest-framework](https://gitee.com/deepin-community/deepin-autotest-
-framework/widgets/
-widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://
-gitee.com/deepin-community/deepin-autotest-framework)
+linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu) [__Gitee
+Info__]() [![deepin-community/youqu](https://gitee.com/deepin-community/youqu/
+widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)]
+(https://gitee.com/deepin-community/youqu)
```

### Comparing `youqu-2.5.2/PKG-INFO` & `youqu-2.5.3/youqu/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,153 +1,124 @@
-Metadata-Version: 2.1
-Name: youqu
-Version: 2.5.2
-Summary: deepin-autotest-framework
-Project-URL: Source, https://github.com/linuxdeepin/deepin-autotest-framework
-Project-URL: Documentation, https://linuxdeepin.github.io/deepin-autotest-framework
-Author-email: mikigo <huangmingqiang@uniontech.com>
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 <p align="center">
-  <a href="https://linuxdeepin.github.io/deepin-autotest-framework/">
+  <a href="https://linuxdeepin.github.io/youqu/">
     <img src="./docs/logo.png" width="520" alt="YouQu">
   </a>
 </p>
-
 <p align="center">
-    <em>有趣，一个使用简单且功能强大的自动化测试基础框架。</em>
+    <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
-[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/pulls)
-[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-autotest-framework/discussions)
+
+
+[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
+[![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
 
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
 ![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-![Static Badge](https://img.shields.io/badge/Linux-Platform?style=flat&label=Platform&color=%23F79431)
-![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=flat&logo=MaterialForMkDocs&logoColor=white&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
 
-[![Hits](https://hits.sh/github.com/linuxdeepin/deepin-autotest-framework.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/deepin-autotest-framework)
-[![Hits](https://hits.sh/linuxdeepin.github.io/deepin-autotest-framework.svg?style=flat&label=YouQu_Hits&color=blue)](https://linuxdeepin.github.io/deepin-autotest-framework)
-[![Hits](https://hits.sh/youqu.uniontech.com.svg?style=flat&label=YouQu内网_Hits&color=blue)](http://youqu.uniontech.com/)
-[![Hits](https://hits.sh/pypi.org/project/youqu.svg?style=flat&label=PyPI_Hits&color=blue)](https://pypi.org/project/youqu/)
+[![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
-**文档**: <a href="https://linuxdeepin.github.io/deepin-autotest-framework" target="_blank">https://linuxdeepin.github.io/deepin-autotest-framework</a>
+<a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
-**源码**: <a href="https://github.com/linuxdeepin/deepin-autotest-framework" target="_blank">https://github.com/linuxdeepin/deepin-autotest-framework</a>
+<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a> | <a href="https://deepin-community.gitee.io/youqu/" target="_blank">在线文档（国内加速）</a>
 
 ---
 
-有趣（YouQu）是深度科技开源的一个用于 `Deepin/UOS` 操作系统（Linux）的自动化测试框架，采用结构分层的设计理念，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
-
-### 爱上 “有趣” 的 18 个理由
+YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
 
-1. 核心库提供了统一的接口，编写方法时只需要导入一个包就可以使用到核心库提供的所有功能；
-2. 公共库封装了很多常用模块的相关方法，比如：任务栏的操作、桌面的操作、右键菜单的操作等等；
-3. 除了常用的属性定位、图像识别以外，我们还提供基于 `UI` 的元素定位方案，其使用简单且高效，效果一定能惊讶到你；
-4. 对属性定位的方法进行了二次封装，将编写属性定位的方法变得简单而优雅；
-5. 对图像识别定位技术进行功能升级，除了支持单个坐标返回，还支持同一界面下多个相同元素返回多个坐标的功能；
-6. 提供用例标签化管理、批量跳过和批量条件跳过的功能，你想不到一个 `csv` 文件原来能干这么多事情；
-7. 提供了功能强大的执行器入口，让你可以方便的在本地执行任何用例集的用例，其丰富的自定义配置项，满足你对执行器所有的幻想；
-8. 提供远程执行的功能，可以控制多台机器并行跑，或者分布式跑，这种付费功能现在免费给你用；
-9. 提供自动输出日志的功能，你再也不用为每个方法单独写输出日志的代码，一切我们给你搞定了，日志输出不仅内容丰富，颜值也绝对在线，我们还自己设计了一款终端输出主题叫《五彩斑斓的黑》；
-10. 提供一键部署自动化测试环境的功能，让你再也不用为环境部署而烦恼；
-11. 提供自动生成多种报告的功能，你想输出什么报告形式都行，而且我们在报告中还加入了失败录屏和失败截图的功能；
-12. 对断言进行了二次封装，提供更友好化的错误提示，让定位问题精准高效；
-13. 不仅支持单条用例超时控制，而且还支持动态控制用例批量执行的总时间，确保 `CI` 环境下能顺畅运行；
-14. 支持本地文件测试套执行、`PMS` 测试套执行、标签化执行方案，满足你各种场景下的执行需求；
-15. 支持基于深度学习的 `OCR` 功能，可定位可断言，中文识别的天花板；
-16. 完美兼容 `Wayland`  和 `X11`，真正做到一套代码，随处执行；
-17. 支持多种方式的数据回填功能，其中异步回填的方案，完美解决了数据回填的耗时问题；
-18. 支持重启交互场景用例的执行，使用方法优雅简洁；
+## YouQu（有趣）能做什么
 
-------------------------
+- [x] Linux 桌面应用 UI 自动化测试
+- [x] Linux 桌面应用 DBus/Gsettings 接口自动化测试
+- [x] 命令行自动化测试
+- [x] HTTP 接口自动化测试
+- [x] Web UI 自动化测试
+- [ ] Linux 桌面应用性能自动化测试
+
+<details>
+	<summary style="color: #FF9933">点击查看爱上 “有趣（YouQu）” 的 N 个理由</summary>
+	<ul>
+        <li>无处不在的代码补全，让编写自动化测试用例成为一种享受；</li>
+        <li>核心库提供了统一的接口，编写方法时只需要导入一个包就可以使用到核心库提供的所有功能；</li>
+        <li>除了常用的属性定位、图像识别以外，我们还提供基于 UI 的元素定位方案，其使用简单且高效，效果一定能惊讶到你；</li>
+        <li>对属性定位的方法进行了二次封装，将编写属性定位的方法变得简单而优雅；</li>
+        <li>对图像识别定位技术进行功能升级，除了支持单个坐标返回，还支持同一界面下多个相同元素返回多个坐标的功能；</li>
+        <li>提供用例标签化管理、批量跳过和批量条件跳过的功能，你想不到一个 csv 文件原来能干这么多事情；</li>
+        <li>提供了功能强大的执行器入口，让你可以方便的在本地执行任何用例集的用例，其丰富的自定义配置项，满足你对执行器所有的幻想；</li>
+        <li>提供远程执行的功能，可以控制多台机器并行跑，或者分布式跑，这种付费功能现在免费给你用；</li>
+        <li>提供自动输出日志的功能，你再也不用为每个方法单独写输出日志的代码，一切我们给你搞定了，日志输出不仅内容丰富，颜值也绝对在线，我们还自己设计了一款终端输出主题叫《五彩斑斓的黑》；</li>
+        <li>提供一键部署自动化测试环境的功能，让你再也不用为环境部署而烦恼；</li>
+        <li>提供自动生成多种报告的功能，你想输出什么报告形式都行，而且我们在报告中还加入了失败录屏和失败截图的功能；</li>
+        <li>对断言进行了二次封装，提供更友好化的错误提示，让定位问题精准高效；</li>
+        <li>不仅支持单条用例超时控制，而且还支持动态控制用例批量执行的总时间，确保 CI 环境下能顺畅运行；</li>
+        <li>支持本地文件测试套执行、PMS 测试套执行、标签化执行方案，满足你各种场景下的执行需求；</li>
+        <li>支持基于深度学习的 OCR 功能，可定位可断言，中文识别的天花板；</li>
+        <li>完美兼容 Wayland  和 X11，真正做到一套代码，随处执行；</li>
+        <li>支持多种方式的数据回填功能，其中异步回填的方案，完美解决了数据回填的耗时问题；</li>
+        <li>支持重启交互场景用例的执行，使用方法优雅简洁；</li>
+    </ul>
+</details>
 
-统信公司内网还可以访问【[内网文档](http://youqu.uniontech.com/)】，文档内容一样，访问速度更快哦~~
-
-## 安装使用
+## 安装
 
 从 PyPI 安装:
 
-<div class="termy">
 
-```console
+```shell
 $ sudo pip3 install youqu
----> 100%
 ```
 
-</div>
-
 创建项目:
 
-<div class="termy">
-
-```console
+```shell
 $ youqu-startproject my_project
----> 100%
-The project: [my_project],has been created by youqu-x.x.x
 ```
 
-</div>
-
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
 安装依赖:
 
-<div class="termy">
-
-```console
-// 如果你的测试机密码不是 `1` ，那你需要在全局配置文件 `globalconfig.ini` 里面将 `PASSWORD` 配置项修改为当前测试机的密码。
+```shell
 $ cd my_project
-$ bash env.sh
----> 100%
-```
 
-</div>
+# 使用的默认密码是 1 ，您可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项
+$ bash env.sh
 
--------------------------------
+# 也可以使用 -p 选项传入密码
+$ bash env.sh -p ${my_password}
+```
 
-**【APP工程】**
+## 创建工程
 
 如果您已经有一个可用的 `APP` 工程，将应用库放到基础框架下 `apps` 目录下，像这样：
 
-```shell hl_lines="3"
+```shell
 my_project
 ├── apps
 │   ├── autotest_deepin_music  # 应用库
 ...
 ```
 
 如果您还没有 `APP` 工程，建议使用框架提供的脚手架功能创建一个全新的 `APP` 工程。
 
-## 创建工程
-
-创建一个 APP 工程：
-
-<div class="termy">
+**创建一个 APP 工程**
 
-```console
+```shell
 $ youqu manage.py startapp autotest_deepin_some
----> 100%
 ```
 
-</div>
-
 这样在 `apps` 目录下会创建一个子项目工程 `autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
 apps
 └── autotest_deepin_some
     ├── case
     │   ├── assert_res
@@ -183,118 +154,57 @@
 
 ### 1. 工作空间
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
 ### 2. 本地执行
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run
 ```
 
-</div>
-
 #### 2.1. 命令行参数
 
 通过命令行参数配置参数，使用 `-h` 或 `--help` 可以查看所有支持的命令行参数：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run -h
 ```
 
-</div>
-
 在一些 CI 环境下使用命令行参数会更加方便：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags "xxx"
 ```
 
-</div>
-
-更多参数请查看【[命令行参数](https://linuxdeepin.github.io/deepin-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
+更多参数请查看【[命令行参数](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
 
 #### 2.2. 配置文件
 
 通过配置文件配置参数
 
 在配置文件 `setting/globalconfig.ini` 里面支持配置对执行的一些参数进行配置，配置完成之后，直接在命令行执行 `manage.py` 就好了。
 
-详细配置项请查看【[配置项](https://linuxdeepin.github.io/deepin-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
+详细配置项请查看【[配置项](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
 
 ### 3. 远程执行
 
 远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同；
 
 使用 `remote` 命令：
 
-<div class="termy">
-
-```console
-$ youqu manage.py remote
-```
-
-</div>
 
-#### 3.1. 远程多机器分布式异步执行
-
-![](https://pic.imgdb.cn/item/64f6d3c0661c6c8e549f8ca5.png)
-
-多机器分布式异步执行就是由本地 YouQu 作为服务端，控制远程 N 台机器执行相同的用例，执行完之后所有测试机的测试结果会返回给服务端 report 目录下；
-
-远程执行同样通过配置文件 `setting/globalconfig.ini` 进行用例相关配置；
-
-需要重点说一下远程执行时的测试机信息配置，在配置文件 `setting/remote.ini`  里面配置测试机的用户名、IP、密码。
-
-```ini
-;=============================== CLIENT LIST =====================================
-; 测试机配置列表
-;[client{number}]     ;测试机别名，有多少台测试机就写多少个 client，别名必须包含 client 字符，且不能重复。
-;user =               ;测试机 user
-;ip =                 ;测试机 ip
-;password = 1         ;测试机的密码, 可以不配置此项，默认取 CLIENT_PASSWORD 的值；
-                      ;如果你所有测试机密码都相同，那么只需要配置 CLIENT_PASSWORD 就可以了
-;=================================================================================
-
-[client1]
-user = uos
-ip = 10.8.15.xx
-
-[client2]
-user = uos
-ip = 10.8.15.xx
-
-[client3]
-user = uos
-ip = 10.8.11.xx
-```
-
-有多少台机器就像这样参考上面的格式写就行了。
-
-然后在命令行：
-
-<div class="termy">
-
-```console
+```shell
 $ youqu manage.py remote
 ```
 
-</div>
-
-这样运行是从配置文件去读取相关配置。
-
-如果你不想通过配置文件，你仍然通过命令行参数进行传参，
-
-以下为 `python3 manage.py remote` 提供的一些参数选项：
+以下为 `remote` 提供的一些参数选项：
 
 ```coffeescript
   -h, --help            show this help message and exit
   -c CLIENTS, --clients CLIENTS
                         远程机器的user@ip:password,多个机器用'/'连接,如果password不传入,默认取sett
                         ing/remote.ini中CLIENT_PASSWORD的值,比如: uos@10.8.13.xx:1
                         或 uos@10.8.13.xx
@@ -303,86 +213,55 @@
   -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
                         测试机密码（全局）
   -y PARALLEL, --parallel PARALLEL
                         yes:表示所有测试机并行跑，执行相同的测试用例;no:表示测试机分布式执行，服务端会根据收集到的测试用例自
                         动分配给各个测试机执行。
 ```
 
-==除了这些特有参数以外，它同样支持本地执行的所有参数；==
+除了这些特有参数以外，它同样支持本地执行的所有参数；
 
 在命令行这样运行：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py remote -a apps/autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx"
 ```
 
-</div>
-
 所有用例执行完之后会在 `report` 目录下回收各个测试机执行的测试报告。
 
 注意：如果远程机器没有搭建自动化测试环境，记得加上参数 `-e` ：
 
-<div class="termy">
 
-```console
+```shell
 $ youqu manage.py remote -a ... -e
 ```
 
-</div>
-
 执行前确保远程机器已经开启了 ssh 服务，否则会提示无法连接，如果没有开启，请手动开启：
 
-<div class="termy">
 
-```console
+```shell
 $ sudo systemctl restart ssh
 $ sudo systemctl enable ssh
 ```
 
-</div>
-
 配置文件其他相关配置项详细说明，请查看配置文件中的注释内容。
 
-#### 3.2. 远程多机器分布式异步负载均衡执行
-
-多机器分布式异步负载均衡执行也是用本地作为服务端控制远程机器执行，但远程机器执行的用例不同，而是所有远程机器执行的用例之和，为你想要执行的用例集；
-
-似乎有点难以理解，我用大白话举例描述下：
-
-服务端想要执行 10 条用例，现在远程机器有 5 台，然后服务端就先拿着第 1 条用例给远程 1 号机执行，拿第 2 条用例给远程 2 号机执行...，如此循环直到所有用例执行完，这就是负载均衡执行。
-
-![](https://pic.imgdb.cn/item/64f6d694661c6c8e54a1025b.png)
-
-使用方法和前面一样，只是需要增加一个参数 `--parallel`：
-
-<div class="termy">
-
-```console
-$ youqu manage.py remote -a ... --parallel no
-```
-
-</div>
-
-## 贡献者
-
-[贡献文档](https://github.com/linuxdeepin/deepin-autotest-framework/blob/master/CONTRIBUTING.md) 
+## 贡献
 
---8<-- "docs/contributors.html"
+[贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
 
 
 ## 开源许可证
 
-有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/deepin-autotest-framework/blob/master/LICENSE) 下发布。
+有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
 
 ------------
 
 [__Github Star History__]()
 
-[![Stargazers over time](https://starchart.cc/linuxdeepin/deepin-autotest-framework.svg)](https://starchart.cc/linuxdeepin/deepin-autotest-framework)
+[![Stargazers over time](https://starchart.cc/linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu)
 
 
 
 [__Gitee Info__]()
 
-[![deepin-community/deepin-autotest-framework](https://gitee.com/deepin-community/deepin-autotest-framework/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/deepin-autotest-framework)
+[![deepin-community/youqu](https://gitee.com/deepin-community/youqu/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/youqu)
```

#### html2text {}

```diff
@@ -1,108 +1,74 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.5.2 Summary: deepin-autotest-
-framework Project-URL: Source, https://github.com/linuxdeepin/deepin-autotest-
-framework Project-URL: Documentation, https://linuxdeepin.github.io/deepin-
-autotest-framework Author-email: mikigo
-uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
-License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
-  ?æ???è?¶?£?ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
-[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/deepin-
-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-
-autotest-framework/issues) [![GitHub pull requests](https://img.shields.io/
-github/issues-pr/linuxdeepin/deepin-autotest-framework?color=%23F79431)](https:
-//github.com/linuxdeepin/deepin-autotest-framework/pulls) [![GitHub
-Discussions](https://img.shields.io/github/discussions/linuxdeepin/deepin-
-autotest-framework?color=%23F79431)](https://github.com/linuxdeepin/deepin-
-autotest-framework/discussions) [![PyPI](https://img.shields.io/pypi/v/
+YYoouuQQuu?ï?¼??æ???è?¶?£?ï?¼??ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
+[![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![GitHub
+pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls) [![GitHub
+Discussions](https://img.shields.io/github/discussions/linuxdeepin/
+youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions) [!
+[PyPI](https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
 (https://pypi.org/project/youqu/) ![PyPI - License](https://img.shields.io/
 pypi/l/youqu?color=%23F79431) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
 badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
-![Static Badge](https://img.shields.io/badge/Linux-
-Platform?style=flat&label=Platform&color=%23F79431) ![Built with Material for
-MkDocs](https://img.shields.io/badge/Material_for_MkDocs-
-526CFE?style=flat&logo=MaterialForMkDocs&logoColor=white&color=%23F79431) [!
-[Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
+[![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
 project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
 (https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
 youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
-linuxdeepin/deepin-autotest-
-framework.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/
-linuxdeepin/deepin-autotest-framework) [![Hits](https://hits.sh/
-linuxdeepin.github.io/deepin-autotest-
-framework.svg?style=flat&label=YouQu_Hits&color=blue)](https://
-linuxdeepin.github.io/deepin-autotest-framework) [![Hits](https://hits.sh/
-youqu.uniontech.com.svg?style=flat&label=YouQuåç½_Hits&color=blue)](http://
-youqu.uniontech.com/) [![Hits](https://hits.sh/pypi.org/project/
-youqu.svg?style=flat&label=PyPI_Hits&color=blue)](https://pypi.org/project/
-youqu/) --- **ææ¡£**: _h_t_t_p_s_:_/_/_l_i_n_u_x_d_e_e_p_i_n_._g_i_t_h_u_b_._i_o_/_d_e_e_p_i_n_-_a_u_t_o_t_e_s_t_-_f_r_a_m_e_w_o_r_k
-**æºç **: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_l_i_n_u_x_d_e_e_p_i_n_/_d_e_e_p_i_n_-_a_u_t_o_t_e_s_t_-_f_r_a_m_e_w_o_r_k --
-- æè¶£ï¼YouQuï¼æ¯æ·±åº¦ç§æå¼æºçä¸ä¸ªç¨äº `Deepin/UOS`
-æä½ç³»ç»ï¼Linuxï¼çèªå¨åæµè¯æ¡æ¶ï¼éç¨ç»æåå±çè®¾è®¡çå¿µï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
-X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ### ç±ä¸
-âæè¶£â ç 18 ä¸ªçç± 1.
-æ ¸å¿åºæä¾äºç»ä¸çæ¥å£ï¼ç¼åæ¹æ³æ¶åªéè¦å¯¼å¥ä¸ä¸ªåå°±å¯ä»¥ä½¿ç¨å°æ ¸å¿åºæä¾çææåè½ï¼
-2.
-å¬å±åºå°è£äºå¾å¤å¸¸ç¨æ¨¡åçç¸å³æ¹æ³ï¼æ¯å¦ï¼ä»»å¡æ çæä½ãæ¡é¢çæä½ãå³é®èåçæä½ç­ç­ï¼
-3. é¤äºå¸¸ç¨çå±æ§å®ä½ãå¾åè¯å«ä»¥å¤ï¼æä»¬è¿æä¾åºäº
-`UI`
-çåç´ å®ä½æ¹æ¡ï¼å¶ä½¿ç¨ç®åä¸é«æï¼ææä¸å®è½æè®¶å°ä½ ï¼
-4.
-å¯¹å±æ§å®ä½çæ¹æ³è¿è¡äºäºæ¬¡å°è£ï¼å°ç¼åå±æ§å®ä½çæ¹æ³åå¾ç®åèä¼éï¼
-5.
-å¯¹å¾åè¯å«å®ä½ææ¯è¿è¡åè½åçº§ï¼é¤äºæ¯æåä¸ªåæ è¿åï¼è¿æ¯æåä¸çé¢ä¸å¤ä¸ªç¸ååç´ è¿åå¤ä¸ªåæ çåè½ï¼
-6.
-æä¾ç¨ä¾æ ç­¾åç®¡çãæ¹éè·³è¿åæ¹éæ¡ä»¶è·³è¿çåè½ï¼ä½ æ³ä¸å°ä¸ä¸ª
-`csv` æä»¶åæ¥è½å¹²è¿ä¹å¤äºæï¼ 7.
-æä¾äºåè½å¼ºå¤§çæ§è¡å¨å¥å£ï¼è®©ä½ å¯ä»¥æ¹ä¾¿çå¨æ¬å°æ§è¡ä»»ä½ç¨ä¾éçç¨ä¾ï¼å¶ä¸°å¯çèªå®ä¹éç½®é¡¹ï¼æ»¡è¶³ä½ å¯¹æ§è¡å¨ææçå¹»æ³ï¼
-8.
-æä¾è¿ç¨æ§è¡çåè½ï¼å¯ä»¥æ§å¶å¤å°æºå¨å¹¶è¡è·ï¼æèåå¸å¼è·ï¼è¿ç§ä»è´¹åè½ç°å¨åè´¹ç»ä½ ç¨ï¼
-9.
-æä¾èªå¨è¾åºæ¥å¿çåè½ï¼ä½ åä¹ä¸ç¨ä¸ºæ¯ä¸ªæ¹æ³åç¬åè¾åºæ¥å¿çä»£ç ï¼ä¸åæä»¬ç»ä½ æå®äºï¼æ¥å¿è¾åºä¸ä»åå®¹ä¸°å¯ï¼é¢å¼ä¹ç»å¯¹å¨çº¿ï¼æä»¬è¿èªå·±è®¾è®¡äºä¸æ¬¾ç»ç«¯è¾åºä¸»é¢å«ãäºå½©ææçé»ãï¼
-10.
-æä¾ä¸é®é¨ç½²èªå¨åæµè¯ç¯å¢çåè½ï¼è®©ä½ åä¹ä¸ç¨ä¸ºç¯å¢é¨ç½²èç¦æ¼ï¼
-11.
-æä¾èªå¨çæå¤ç§æ¥åçåè½ï¼ä½ æ³è¾åºä»ä¹æ¥åå½¢å¼é½è¡ï¼èä¸æä»¬å¨æ¥åä¸­è¿å å¥äºå¤±è´¥å½å±åå¤±è´¥æªå¾çåè½ï¼
-12.
-å¯¹æ­è¨è¿è¡äºäºæ¬¡å°è£ï¼æä¾æ´åå¥½åçéè¯¯æç¤ºï¼è®©å®ä½é®é¢ç²¾åé«æï¼
-13.
-ä¸ä»æ¯æåæ¡ç¨ä¾è¶æ¶æ§å¶ï¼èä¸è¿æ¯æå¨ææ§å¶ç¨ä¾æ¹éæ§è¡çæ»æ¶é´ï¼ç¡®ä¿
-`CI` ç¯å¢ä¸è½é¡ºçè¿è¡ï¼ 14. æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ã`PMS`
-æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
-15. æ¯æåºäºæ·±åº¦å­¦ä¹ ç `OCR`
-åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼ 16. å®ç¾å¼å®¹
-`Wayland` å `X11`ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼ 17.
-æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
-18. æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼ -----
-------------------- ç»ä¿¡å¬å¸åç½è¿å¯ä»¥è®¿é®ã[åç½ææ¡£](http://
-youqu.uniontech.com/)ãï¼ææ¡£åå®¹ä¸æ ·ï¼è®¿é®éåº¦æ´å¿«å¦~~ ##
-å®è£ä½¿ç¨ ä» PyPI å®è£:
-```console $ sudo pip3 install youqu ---> 100% ```
-åå»ºé¡¹ç®:
-```console $ youqu-startproject my_project ---> 100% The project:
-[my_project],has been created by youqu-x.x.x ```
-å¦æ `youqu-startproject`
+linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
+github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ |
+_å__¨_ç_º_¿_æ___æ_¡_£_ï_¼__å__½_å___å__ _é___ï_¼_ --
+- YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
+æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
+X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ##
+YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] Linux æ¡é¢åºç¨ UI èªå¨åæµè¯ - [x]
+Linux æ¡é¢åºç¨ DBus/Gsettings æ¥å£èªå¨åæµè¯ - [x]
+å½ä»¤è¡èªå¨åæµè¯ - [x] HTTP æ¥å£èªå¨åæµè¯ - [x] Web UI
+èªå¨åæµè¯ - [ ] Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯
+ç¹å»æ¥çç±ä¸ âæè¶£ï¼YouQuï¼â ç N ä¸ªçç±
+    * æ å¤ä¸å¨çä»£ç è¡¥å¨ï¼è®©ç¼åèªå¨åæµè¯ç¨ä¾æä¸ºä¸ç§äº«åï¼
+    * æ ¸å¿åºæä¾äºç»ä¸çæ¥å£ï¼ç¼åæ¹æ³æ¶åªéè¦å¯¼å¥ä¸ä¸ªåå°±å¯ä»¥ä½¿ç¨å°æ ¸å¿åºæä¾çææåè½ï¼
+    * é¤äºå¸¸ç¨çå±æ§å®ä½ãå¾åè¯å«ä»¥å¤ï¼æä»¬è¿æä¾åºäº
+      UI
+      çåç´ å®ä½æ¹æ¡ï¼å¶ä½¿ç¨ç®åä¸é«æï¼ææä¸å®è½æè®¶å°ä½ ï¼
+    * å¯¹å±æ§å®ä½çæ¹æ³è¿è¡äºäºæ¬¡å°è£ï¼å°ç¼åå±æ§å®ä½çæ¹æ³åå¾ç®åèä¼éï¼
+    * å¯¹å¾åè¯å«å®ä½ææ¯è¿è¡åè½åçº§ï¼é¤äºæ¯æåä¸ªåæ è¿åï¼è¿æ¯æåä¸çé¢ä¸å¤ä¸ªç¸ååç´ è¿åå¤ä¸ªåæ çåè½ï¼
+    * æä¾ç¨ä¾æ ç­¾åç®¡çãæ¹éè·³è¿åæ¹éæ¡ä»¶è·³è¿çåè½ï¼ä½ æ³ä¸å°ä¸ä¸ª
+      csv æä»¶åæ¥è½å¹²è¿ä¹å¤äºæï¼
+    * æä¾äºåè½å¼ºå¤§çæ§è¡å¨å¥å£ï¼è®©ä½ å¯ä»¥æ¹ä¾¿çå¨æ¬å°æ§è¡ä»»ä½ç¨ä¾éçç¨ä¾ï¼å¶ä¸°å¯çèªå®ä¹éç½®é¡¹ï¼æ»¡è¶³ä½ å¯¹æ§è¡å¨ææçå¹»æ³ï¼
+    * æä¾è¿ç¨æ§è¡çåè½ï¼å¯ä»¥æ§å¶å¤å°æºå¨å¹¶è¡è·ï¼æèåå¸å¼è·ï¼è¿ç§ä»è´¹åè½ç°å¨åè´¹ç»ä½ ç¨ï¼
+    * æä¾èªå¨è¾åºæ¥å¿çåè½ï¼ä½ åä¹ä¸ç¨ä¸ºæ¯ä¸ªæ¹æ³åç¬åè¾åºæ¥å¿çä»£ç ï¼ä¸åæä»¬ç»ä½ æå®äºï¼æ¥å¿è¾åºä¸ä»åå®¹ä¸°å¯ï¼é¢å¼ä¹ç»å¯¹å¨çº¿ï¼æä»¬è¿èªå·±è®¾è®¡äºä¸æ¬¾ç»ç«¯è¾åºä¸»é¢å«ãäºå½©ææçé»ãï¼
+    * æä¾ä¸é®é¨ç½²èªå¨åæµè¯ç¯å¢çåè½ï¼è®©ä½ åä¹ä¸ç¨ä¸ºç¯å¢é¨ç½²èç¦æ¼ï¼
+    * æä¾èªå¨çæå¤ç§æ¥åçåè½ï¼ä½ æ³è¾åºä»ä¹æ¥åå½¢å¼é½è¡ï¼èä¸æä»¬å¨æ¥åä¸­è¿å å¥äºå¤±è´¥å½å±åå¤±è´¥æªå¾çåè½ï¼
+    * å¯¹æ­è¨è¿è¡äºäºæ¬¡å°è£ï¼æä¾æ´åå¥½åçéè¯¯æç¤ºï¼è®©å®ä½é®é¢ç²¾åé«æï¼
+    * ä¸ä»æ¯æåæ¡ç¨ä¾è¶æ¶æ§å¶ï¼èä¸è¿æ¯æå¨ææ§å¶ç¨ä¾æ¹éæ§è¡çæ»æ¶é´ï¼ç¡®ä¿
+      CI ç¯å¢ä¸è½é¡ºçè¿è¡ï¼
+    * æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ãPMS
+      æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
+    * æ¯æåºäºæ·±åº¦å­¦ä¹ ç OCR
+      åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼
+    * å®ç¾å¼å®¹ Wayland å X11ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼
+    * æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
+    * æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼
+## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` åå»ºé¡¹ç®:
+```shell $ youqu-startproject my_project ``` å¦æ `youqu-startproject`
 åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ å®è£ä¾èµ:
-```console // å¦æä½ çæµè¯æºå¯ç ä¸æ¯ `1`
-ï¼é£ä½ éè¦å¨å¨å±éç½®æä»¶ `globalconfig.ini` éé¢å° `PASSWORD`
-éç½®é¡¹ä¿®æ¹ä¸ºå½åæµè¯æºçå¯ç ã $ cd my_project $ bash env.sh ---
-> 100% ```
-------------------------------- **ãAPPå·¥ç¨ã**
-å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
+```shell $ cd my_project # ä½¿ç¨çé»è®¤å¯ç æ¯ 1
+ï¼æ¨å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/globalconfig.ini éé¢ç PASSWORD
+éç½®é¡¹ $ bash env.sh # ä¹å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç  $ bash env.sh -
+p ${my_password} ``` ## åå»ºå·¥ç¨ å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
 å·¥ç¨ï¼å°åºç¨åºæ¾å°åºç¡æ¡æ¶ä¸ `apps` ç®å½ä¸ï¼åè¿æ ·ï¼
-```shell hl_lines="3" my_project âââ apps â âââ
-autotest_deepin_music # åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
+```shell my_project âââ apps â âââ autotest_deepin_music #
+åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
 å·¥ç¨ï¼å»ºè®®ä½¿ç¨æ¡æ¶æä¾çèææ¶åè½åå»ºä¸ä¸ªå¨æ°ç `APP`
-å·¥ç¨ã ## åå»ºå·¥ç¨ åå»ºä¸ä¸ª APP å·¥ç¨ï¼
-```console $ youqu manage.py startapp autotest_deepin_some ---> 100% ```
-è¿æ ·å¨ `apps` ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
+å·¥ç¨ã **åå»ºä¸ä¸ª APP å·¥ç¨** ```shell $ youqu manage.py startapp
+autotest_deepin_some ``` è¿æ ·å¨ `apps`
+ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
 `autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
 ```shell apps âââ autotest_deepin_some Â Â  âââ case Â Â  âÂ Â 
 âââ assert_res Â Â  âÂ Â  âÂ Â  âââ readme Â Â  âÂ Â 
 âââ base_case.py Â Â  âÂ Â  âââ __init__.py Â Â  âââ
 config.ini Â Â  âââ config.py Â Â  âââ conftest.py Â Â  âââ
 control Â Â  âââ deepin_some_assert.py Â Â  âââ deepin_some.csv
 Â Â  âââ __init__.py Â Â  âââ widget Â Â  âââ base_widget.py
@@ -111,98 +77,55 @@
 âââ other_widget.py Â Â  âââ pic_res Â Â  âÂ Â  âââ readme
 Â Â  âââ ui.ini ``` `autotest_deepin_some`
 æ¯ä½ çå·¥ç¨åç§°ï¼æ¯å¦ï¼`autotest_deepin_music` ï¼
 å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
 é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã è¿è¡ ------- ### 1.
 å·¥ä½ç©ºé´ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
-### 2. æ¬å°æ§è¡
-```console $ youqu manage.py run ```
-#### 2.1. å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ
-`--help` å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼
-```console $ youqu manage.py run -h ```
-å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
-```console $ youqu manage.py run --app apps/autotest_deepin_music --keywords
-"xxx" --tags "xxx" ```
-æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://linuxdeepin.github.io/deepin-
-autotest-framework/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
+### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
+å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ `--help`
+å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼ ```shell $ youqu manage.py run -
+h ``` å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $
+youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags
+"xxx" ``` æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://
+linuxdeepin.github.io/youqu/
+%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
 %E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)ã #### 2.2. éç½®æä»¶
 éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ `setting/globalconfig.ini`
 éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ï¼éç½®å®æä¹åï¼ç´æ¥å¨å½ä»¤è¡æ§è¡
 `manage.py` å°±å¥½äºã è¯¦ç»éç½®é¡¹è¯·æ¥çã[éç½®é¡¹](https://
-linuxdeepin.github.io/deepin-autotest-framework/
+linuxdeepin.github.io/youqu/
 %E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
 %E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)ã ### 3. è¿ç¨æ§è¡
 è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åï¼
-ä½¿ç¨ `remote` å½ä»¤ï¼
-```console $ youqu manage.py remote ```
-#### 3.1. è¿ç¨å¤æºå¨åå¸å¼å¼æ­¥æ§è¡ ![](https://pic.imgdb.cn/item/
-64f6d3c0661c6c8e549f8ca5.png) å¤æºå¨åå¸å¼å¼æ­¥æ§è¡å°±æ¯ç±æ¬å°
-YouQu ä½ä¸ºæå¡ç«¯ï¼æ§å¶è¿ç¨ N
-å°æºå¨æ§è¡ç¸åçç¨ä¾ï¼æ§è¡å®ä¹åæææµè¯æºçæµè¯ç»æä¼è¿åç»æå¡ç«¯
-report ç®å½ä¸ï¼ è¿ç¨æ§è¡åæ ·éè¿éç½®æä»¶ `setting/
-globalconfig.ini` è¿è¡ç¨ä¾ç¸å³éç½®ï¼
-éè¦éç¹è¯´ä¸ä¸è¿ç¨æ§è¡æ¶çæµè¯æºä¿¡æ¯éç½®ï¼å¨éç½®æä»¶
-`setting/remote.ini` éé¢éç½®æµè¯æºçç¨æ·åãIPãå¯ç ã ```ini
-;=============================== CLIENT LIST
-===================================== ; æµè¯æºéç½®åè¡¨ ;[client{number}]
-;æµè¯æºå«åï¼æå¤å°å°æµè¯æºå°±åå¤å°ä¸ª
-clientï¼å«åå¿é¡»åå« client å­ç¬¦ï¼ä¸ä¸è½éå¤ã ;user =
-;æµè¯æº user ;ip = ;æµè¯æº ip ;password = 1 ;æµè¯æºçå¯ç ,
-å¯ä»¥ä¸éç½®æ­¤é¡¹ï¼é»è®¤å CLIENT_PASSWORD çå¼ï¼
-;å¦æä½ æææµè¯æºå¯ç é½ç¸åï¼é£ä¹åªéè¦éç½®
-CLIENT_PASSWORD å°±å¯ä»¥äº
-;=================================================================================
-[client1] user = uos ip = 10.8.15.xx [client2] user = uos ip = 10.8.15.xx
-[client3] user = uos ip = 10.8.11.xx ```
-æå¤å°å°æºå¨å°±åè¿æ ·åèä¸é¢çæ ¼å¼åå°±è¡äºã
-ç¶åå¨å½ä»¤è¡ï¼
-```console $ youqu manage.py remote ```
-è¿æ ·è¿è¡æ¯ä»éç½®æä»¶å»è¯»åç¸å³éç½®ã
-å¦æä½ ä¸æ³éè¿éç½®æä»¶ï¼ä½ ä»ç¶éè¿å½ä»¤è¡åæ°è¿è¡ä¼ åï¼
-ä»¥ä¸ä¸º `python3 manage.py remote` æä¾çä¸äºåæ°éé¡¹ï¼
-```coffeescript -h, --help show this help message and exit -c CLIENTS, --
-clients CLIENTS è¿ç¨æºå¨çuser@ip:password,å¤ä¸ªæºå¨ç¨'/
-'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ä»¥ä¸ä¸º
+`remote` æä¾çä¸äºåæ°éé¡¹ï¼ ```coffeescript -h, --help show this
+help message and exit -c CLIENTS, --clients CLIENTS è¿ç¨æºå¨çuser@ip:
+password,å¤ä¸ªæºå¨ç¨'/'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
 remote.iniä¸­CLIENT_PASSWORDçå¼,æ¯å¦: uos@10.8.13.xx:1 æ uos@10.8.13.xx
 -s, --send_code åéä»£ç å°æµè¯æºï¼ä¸å«reportç®å½ï¼ -e, --
 build_env
 æ­å»ºæµè¯ç¯å¢,å¦æä¸ºyesï¼ä¸ç®¡send_codeæ¯å¦ä¸ºyesé½ä¼åéä»£ç å°æµè¯æº.
 -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
 æµè¯æºå¯ç ï¼å¨å±ï¼ -y PARALLEL, --parallel PARALLEL yes:
 è¡¨ç¤ºæææµè¯æºå¹¶è¡è·ï¼æ§è¡ç¸åçæµè¯ç¨ä¾;no:
 è¡¨ç¤ºæµè¯æºåå¸å¼æ§è¡ï¼æå¡ç«¯ä¼æ ¹æ®æ¶éå°çæµè¯ç¨ä¾èª
 å¨åéç»åä¸ªæµè¯æºæ§è¡ã ```
-==é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼==
-å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼
-```console $ youqu manage.py remote -a apps/autotest_deepin_music -
-c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
+é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼
+å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼ ```shell $ youqu manage.py remote -a apps/
+autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
 ææç¨ä¾æ§è¡å®ä¹åä¼å¨ `report`
 ç®å½ä¸åæ¶åä¸ªæµè¯æºæ§è¡çæµè¯æ¥åã
 æ³¨æï¼å¦æè¿ç¨æºå¨æ²¡ææ­å»ºèªå¨åæµè¯ç¯å¢ï¼è®°å¾å ä¸åæ°
-`-e` ï¼
-```console $ youqu manage.py remote -a ... -e ```
+`-e` ï¼ ```shell $ youqu manage.py remote -a ... -e ```
 æ§è¡åç¡®ä¿è¿ç¨æºå¨å·²ç»å¼å¯äº ssh
 æå¡ï¼å¦åä¼æç¤ºæ æ³è¿æ¥ï¼å¦ææ²¡æå¼å¯ï¼è¯·æå¨å¼å¯ï¼
-```console $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
+```shell $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
 éç½®æä»¶å¶ä»ç¸å³éç½®é¡¹è¯¦ç»è¯´æï¼è¯·æ¥çéç½®æä»¶ä¸­çæ³¨éåå®¹ã
-#### 3.2. è¿ç¨å¤æºå¨åå¸å¼å¼æ­¥è´è½½åè¡¡æ§è¡
-å¤æºå¨åå¸å¼å¼æ­¥è´è½½åè¡¡æ§è¡ä¹æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼ä½è¿ç¨æºå¨æ§è¡çç¨ä¾ä¸åï¼èæ¯ææè¿ç¨æºå¨æ§è¡çç¨ä¾ä¹åï¼ä¸ºä½ æ³è¦æ§è¡çç¨ä¾éï¼
-ä¼¼ä¹æç¹é¾ä»¥çè§£ï¼æç¨å¤§ç½è¯ä¸¾ä¾æè¿°ä¸ï¼
-æå¡ç«¯æ³è¦æ§è¡ 10 æ¡ç¨ä¾ï¼ç°å¨è¿ç¨æºå¨æ 5
-å°ï¼ç¶åæå¡ç«¯å°±åæ¿çç¬¬ 1 æ¡ç¨ä¾ç»è¿ç¨ 1
-å·æºæ§è¡ï¼æ¿ç¬¬ 2 æ¡ç¨ä¾ç»è¿ç¨ 2
-å·æºæ§è¡...ï¼å¦æ­¤å¾ªç¯ç´å°ææç¨ä¾æ§è¡å®ï¼è¿å°±æ¯è´è½½åè¡¡æ§è¡ã
-![](https://pic.imgdb.cn/item/64f6d694661c6c8e54a1025b.png)
-ä½¿ç¨æ¹æ³ååé¢ä¸æ ·ï¼åªæ¯éè¦å¢å ä¸ä¸ªåæ° `--parallel`ï¼
-```console $ youqu manage.py remote -a ... --parallel no ```
-## è´¡ç®è [è´¡ç®ææ¡£](https://github.com/linuxdeepin/deepin-autotest-
-framework/blob/master/CONTRIBUTING.md) --8<-- "docs/contributors.html" ##
-å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://github.com/linuxdeepin/
-deepin-autotest-framework/blob/master/LICENSE) ä¸åå¸ã ------------
+## è´¡ç® [è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
+CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://
+github.com/linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã ------------
 [__Github Star History__]() [![Stargazers over time](https://starchart.cc/
-linuxdeepin/deepin-autotest-framework.svg)](https://starchart.cc/linuxdeepin/
-deepin-autotest-framework) [__Gitee Info__]() [![deepin-community/deepin-
-autotest-framework](https://gitee.com/deepin-community/deepin-autotest-
-framework/widgets/
-widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://
-gitee.com/deepin-community/deepin-autotest-framework)
+linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu) [__Gitee
+Info__]() [![deepin-community/youqu](https://gitee.com/deepin-community/youqu/
+widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)]
+(https://gitee.com/deepin-community/youqu)
```

