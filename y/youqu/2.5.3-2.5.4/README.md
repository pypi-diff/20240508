# Comparing `tmp/youqu-2.5.3.tar.gz` & `tmp/youqu-2.5.4.tar.gz`

## Comparing `youqu-2.5.3.tar` & `youqu-2.5.4.tar`

### file list

```diff
@@ -1,221 +1,228 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/CURRENT
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/_env_base.sh
--rw-r--r--   0        0        0    43113 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/conftest.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/docs_env.sh
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/env.sh
--rwxr-xr-x   0        0        0     3090 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/env_dev.sh
--rw-r--r--   0        0        0    24445 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/manage.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/playbook.toml
--rw-r--r--   0        0        0    68097 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pnpm-lock.yaml
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pylint.sh
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/ruff.toml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/__init__.py
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/__init__.py
--rw-r--r--   0        0        0    18506 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26357 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/calculate.py
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/desktop.py
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/filectl.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/filter_image.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14861 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/mouse_key.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/read_csv.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/requestx.py
--rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/singleton.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/startapp.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/webui.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/check.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_base.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_remote_dogtail_ctl.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/_remote_other_ctl.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/remotectl/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    19630 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0    21433 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/pycharm.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_remote.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.3/pyproject.toml
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 youqu-2.5.3/youqu/README.md
--rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 youqu-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/CURRENT
+-rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/conftest.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/env.sh
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/manage.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/pytest.ini
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/ruff.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/__init__.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/_env_base.sh
+-rwxr-xr-x   0        0        0     3272 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/env_dev.sh
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/env_vir.sh
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/playbook.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/subcmd.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/calculate.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/filter_image.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/read_csv.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/read_toml.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/singleton.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/_cargo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/mng.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/_cargo.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/_cargo.py
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/playbook.py
+-rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/command_complete.sh
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/docs_env.sh
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/opencv_rpc_server.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/pylint.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/vnc.sh
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/README.md
+-rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 youqu-2.5.4/PKG-INFO
```

### Comparing `youqu-2.5.3/youqu/_env_base.sh` & `youqu-2.5.4/youqu/setting/_env_base.sh`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,11 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
 
-tag=$(echo "$(cat ./CURRENT | grep "tag = ")" | cut -d "=" -f2 | python3 -c "s=input();print(s.strip())")
-ROOT_DIR=`pwd`
-
-config_pwd=$(cat ./setting/globalconfig.ini | grep "PASSWORD = ")
-PASSWORD=$(echo "${config_pwd}" | cut -d "=" -f2 | python3 -c "s=input();print(s.strip())")
-while getopts ":p:" opt
-do
-    case $opt in
-        p)
-            PASSWORD=$OPTARG
-            ;;
-        ?)
-            echo "there is unrecognized parameter."
-            exit 1
-            ;;
-    esac
-done
-
-debian_platform=false
-yq=apt
-if command -v apt &> /dev/null; then
-    debian_platform=true
-    yq=apt
-else
-    yq=yum
-fi
-
-DISPLAY_SERVER=$(cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1 | cut -d "=" -f2)
-PYTHON_VERSION=$(python3 -c "import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')")
-flag_feel="\n**** (・_・) ****\n"
-whitelist="/usr/share/deepin-elf-verify/whitelist"
-pypi_mirror="https://pypi.tuna.tsinghua.edu.cn/simple"
-echo "${PASSWORD}" | sudo -S su
-
-if [ ! -f "$HOME/.Xauthority" ]; then
-        touch $HOME/.Xauthority
-fi
-
 check_status(){
     if [ $? = 0 ]; then
         echo -e "$1\t安装成功 √"
     else
         echo -e "$1\t安装失败 ×"
         cat /tmp/env.log
     fi
```

### Comparing `youqu-2.5.3/youqu/conftest.py` & `youqu-2.5.4/youqu/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,50 +69,43 @@
 from src.recording_screen import recording_screen
 
 FLAG_FEEL = "=" * 10
 LN = "\n"
 
 
 class LabelType(Enum):
-    """用例级别对应报告级别"""
-
     L1 = allure.severity_level.BLOCKER
     L2 = allure.severity_level.CRITICAL
     L3 = allure.severity_level.NORMAL
     L4 = allure.severity_level.MINOR
 
 
 def add_mark(item, name: str = "", args: tuple = (), kwargs: dict = None):
-    """add mark"""
     item.own_markers.append(Mark(name=name, args=args, kwargs=kwargs))
 
 
 def write_json(session):
-    """write json"""
     return bool(
         session.config.option.send_pms
         and (session.config.option.task_id or session.config.option.suite_id)
     )
 
 
 def auto_send(session):
-    """auto send"""
     return bool(session.config.option.send_pms and session.config.option.trigger)
 
 
 def async_send(session):
-    """async send"""
     return bool(
         session.config.option.send_pms == ConfStr.ASYNC.value
         and session.config.option.trigger == ConfStr.AUTO.value
     )
 
 
 def finish_send(session):
-    """finish send"""
     return bool(
         session.config.option.send_pms == ConfStr.FINISH.value
         and session.config.option.trigger == ConfStr.AUTO.value
     )
 
 
 def pytest_addoption(parser):
@@ -148,63 +141,44 @@
     parser.addoption("--slaves", action="store", default="", help="远程测试机")
     parser.addoption(
         "--autostart", action="store", default="", help="重启类场景开启letmego执行方案"
     )
 
 
 def pytest_cmdline_main(config):
-    """pytest_cmdline_main"""
     # 初始化log配置，以解决allure报告日志格式问题
     log_info = logger(config.option.log_level)
     config.option.log_level = config.option.log_level
     config.option.log_format = log_info.log_format
     config.option.log_date_format = log_info.date_format
 
 
 def pytest_addhooks(pluginmanager):
     """pytest_addhooks"""
     pluginmanager.add_hookspecs(emoji_hooks)
 
 
 @pytest.mark.trylast
 def pytest_configure(config):
-    """pytest_configure"""
     if hasattr(config, "workerinput"):
         return  # xdist worker
     reporter = config.pluginmanager.getplugin("terminalreporter")
     if config.option.duringfail and reporter:
         custom_reporter = DuringfailingTerminalReporter(reporter)
         config.pluginmanager.unregister(custom_reporter)
         config.pluginmanager.register(custom_reporter)
 
 
 def pytest_sessionstart(session):
-    """pytest_sessionstart"""
-    # if (
-    #         CmdCtl.run_cmd(
-    #             "gsettings get com.deepin.dde.appearance gtk-theme",
-    #             interrupt=False,
-    #             out_debug_flag=False,
-    #             command_log=False,
-    #         ).strip("'")
-    #         != GlobalConfig.SYS_THEME
-    # ):
-    #     CmdCtl.run_cmd(
-    #         f"gsettings set com.deepin.dde.appearance gtk-theme {GlobalConfig.SYS_THEME}",
-    #         interrupt=False,
-    #         out_debug_flag=False,
-    #         command_log=False,
-    #     )
     _display = (
         GlobalConfig.DisplayServer.wayland
         if GlobalConfig.IS_WAYLAND
         else GlobalConfig.DisplayServer.x11
     )
     logger.info(f"当前系统显示协议为 {_display.title()}")
-    # popen("gsettings set com.deepin.dde.dock position bottom")
     session.config.option.start_time = datetime.now()
 
     user = session.config.option.pms_user
     password = session.config.option.pms_password
     task_id = session.config.option.task_id
     suite_id = session.config.option.suite_id
     if write_json(session):
@@ -228,15 +202,14 @@
 
         session.p = Process(target=record_top, args=())
         session.p.start()
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_generate_tests(metafunc):
-    """pytest generate tests"""
     repeat = metafunc.config.option.repeat
     marks = metafunc.definition.get_closest_marker("repeat")
     if marks is not None:
         repeat = int(marks.args[0])
     if repeat > 1:
         metafunc.fixturenames.append("__pytest_repeat_step_number")
 
@@ -248,16 +221,14 @@
             range(repeat),
             indirect=True,
             ids=ids,
         )
 
 
 def pytest_collection_modifyitems(session):
-    """pytest collection modifyitems"""
-
     walk_dir = (
         f"{GlobalConfig.APPS_PATH}/{session.config.option.app_name}"
         if session.config.option.app_name
            and exists(f"{GlobalConfig.APPS_PATH}/{session.config.option.app_name}")
         else GlobalConfig.APPS_PATH
     )
     csv_path_dict, no_youqu_mark = walk_apps(walk_dir)
@@ -473,15 +444,14 @@
                 if mark.args == (FixedCsvTitle.pms_case_id.value,):
                     print(f"case_id: {mark.name}, case_name: {item.name}")
                     break
         print()  # 处理日志换行
 
 
 def pytest_collection_finish(session):
-    """pytest collection finish"""
     session.item_count = len(session.items)
 
     pop_skip_case_from_items = session.items[:]
     is_skiped_case = False
     for item in pop_skip_case_from_items[::-1]:
         for mark in item.own_markers:
             if mark.name == ConfStr.SKIP.value:
@@ -564,15 +534,14 @@
                 "w+",
                 encoding="utf-8",
         ) as _f:
             _f.writelines(execute2)
 
 
 def pytest_runtest_setup(item):
-    """pytest runtest setup"""
     if hasattr(item, "execution_count"):
         letmego.conf.setting.EXECUTION_COUNT = item.execution_count
 
     print()  # 处理首行日志换行的问题
     current_item_count = f"[{item.session.items.index(item) + 1}/{item.session.item_count}] "
     try:
         current_item_percent = "{:.0f}%".format(
@@ -614,35 +583,32 @@
                 send2pms, item.session.case_res_path, item.session.data_send_result_csv
             )
             item.session.all_thread_task.append(task)
 
 
 # pylint: disable=unused-argument
 def pytest_runtest_call(item):
-    """pytest runtest call"""
     logger.info(f"{FLAG_FEEL} case body {FLAG_FEEL}")
 
 
 def pytest_runtest_teardown(item):
-    """pytest runtest teardown"""
     logger.info(f"{FLAG_FEEL} teardown {FLAG_FEEL}")
     sessiontimeout = item.session.sessiontimeout
     if sessiontimeout:
         duration = datetime.now() - item.session.config.option.start_time
         if duration.seconds > int(sessiontimeout):
             # 处理时间秒为 XX分XX秒
             _min, sec = divmod(duration.seconds, 60)
             # 处理时间分为 XX小时xx分xx秒
             hour, _min = divmod(_min, 60)
             raise item.session.Interrupted(f"会话超时（{hour}小时{_min}分{sec}秒）,用例强制终止!")
 
 
 @pytest.hookimpl(hookwrapper=True, tryfirst=True)
 def pytest_runtest_makereport(item, call):
-    """pytest_runtest_makereport"""
     out = yield
     report = out.get_result()
     if report.when == "setup":
         for mark in item.own_markers:
             if mark.name == "parametrize":
                 continue
             if mark.args:
@@ -736,15 +702,14 @@
                         f"{'重跑用例测试成功，删除视频录像' if item.record.get('result') == ConfStr.PASSED.value else ''}"
                     )
     except (AttributeError, KeyError):
         pass
 
 
 def pytest_report_teststatus(report, config):
-    """pytest report teststatus"""
     # 在 setup 和 teardown 阶段处理 error 和 skip
     if report.when in ("setup", "teardown"):
         if report.failed:
             short, verbose = config.hook.pytest_emoji_error(
                 config=config, head_line=report.head_line
             )
             return "error", short, verbose
@@ -769,39 +734,37 @@
                 config=config, head_line=report.head_line
             )
         return report.outcome, short, verbose
     return None
 
 
 def pytest_sessionfinish(session):
-    """pytest session finish"""
     if session.config.option.allure_report_dir:
-        AllureReportExtend.environment_info(session)
-        terminalreporter = session.config.pluginmanager.get_plugin("terminalreporter")
+        tr = session.config.pluginmanager.get_plugin("terminalreporter")
         execute = {}
-        for _, items in terminalreporter.stats.items():
+        for _, items in tr.stats.items():
             for item in items:
-                default_result = {"result": "blocked", "longrepr": "None"}
-                try:
+                if hasattr(item, "outcome"):
+                    default_result = {"result": "blocked", "longrepr": "None"}
                     if item.outcome == ConfStr.PASSED.value:
                         default_result["result"] = "pass"
                     elif item.outcome == ConfStr.SKIPPED.value:
                         default_result["result"] = "skip"
                     elif item.outcome == ConfStr.RERUN.value:
                         continue
                     else:
                         default_result["result"] = "fail"
-                    item_name = item.nodeid.split("[")[0]
+                    default_result["longrepr"] = item.longreprtext
+                    item_name = item.fspath
                     if not execute.get(item_name) or (
                             item.outcome != ConfStr.PASSED.value
                             and execute.get(item_name).get("result") == "pass"
                     ):
                         execute[item_name] = default_result
-                except AttributeError:
-                    pass
+        AllureReportExtend.environment_info(session, execute)
         if execute:
             with open(f"{GlobalConfig.ROOT_DIR}/ci_result.json", "w", encoding="utf-8") as _f:
                 _f.write(dumps(execute, indent=2, ensure_ascii=False))
 
     if session.config.option.pms_user and session.config.option.pms_password:
 
         def send2pms(case_res_path, data_send_result_csv):
@@ -817,15 +780,15 @@
 
         if finish_send(session):
             send2pms(session.case_res_path, session.data_send_result_csv)
 
     if not session.config.option.collectonly and session.config.option.top:
         session.p.terminate()
         system(
-            f"ps -aux | grep '{GlobalConfig.top_cmd}' | "
+            f"ps -ef | grep '{GlobalConfig.top_cmd}' | "
             "cut -c 9-15 | xargs kill -9 > /dev/null 2>&1"
         )
         session.p.close()
 
     if exists(GlobalConfig.TMPDIR):
         # 清理临时模板图片
         CmdCtl.run_cmd(
@@ -971,15 +934,15 @@
             continue
         for file in files:
             if file.endswith(".csv") and file != "case_list.csv":
                 csv_path_dict[splitext(file)[0]] = f"{root}/{file}"
     return csv_path_dict, no_youqu_mark
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope='module')
 def native_page():
     from playwright.sync_api import sync_playwright
     driver = sync_playwright().start()
     browser = driver.chromium.launch(
         headless=False,
         args=[
             '--start-maximized',
@@ -992,15 +955,15 @@
     _page = context.new_page()
     yield _page
     context.close()
     browser.close()
     driver.stop()
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope='module')
 def page():
     from playwright.sync_api import sync_playwright
     driver = sync_playwright().start()
     browser = driver.chromium.launch_persistent_context(
         user_data_dir=GlobalConfig.USER_DATE_DIR,
         executable_path=GlobalConfig.EXECUTABLE_PATH,
         ignore_https_errors=True,
```

### Comparing `youqu-2.5.3/youqu/docs_env.sh` & `youqu-2.5.4/youqu/src/utils/docs_env.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 set -e
+ROOT_DIR=$(dirname "$(dirname "$(pwd)")")
 
+cd ${ROOT_DIR}
 # check path
 docs_path="$( cd "$( dirname "$0")" && pwd)"
 if [[ "${docs_path}" != "${PWD}" ]]; then
     cd "${docs_path}" || exit 1
 fi
 
 node_version=v18.16.1
@@ -17,19 +19,18 @@
 	sudo mv node-${node_version}-linux-x64 /opt/${opt_node_dir}
 	sudo rm -rf /usr/local/bin/npm; sudo ln -s /opt/${opt_node_dir}/bin/npm   /usr/local/bin/npm
 	sudo rm -rf /usr/local/bin/node; sudo ln -s /opt/${opt_node_dir}/bin/node   /usr/local/bin/node
 
 elif ! command -v pnpm  &> /dev/null; then
 	npm config set registry https://registry.npmmirror.com
 	npm install -g pnpm
+	sudo rm -rf /usr/local/bin/pnpm; sudo ln -s /opt/${opt_node_dir}/bin/pnpm /usr/local/bin/pnpm
+  sudo rm -rf /usr/local/bin/pnpx; sudo ln -s /opt/${opt_node_dir}/bin/pnpx /usr/local/bin/pnpx
 fi
 
-sudo rm -rf /usr/local/bin/pnpm; sudo ln -s /opt/${opt_node_dir}/bin/pnpm /usr/local/bin/pnpm
-sudo rm -rf /usr/local/bin/pnpx; sudo ln -s /opt/${opt_node_dir}/bin/pnpx /usr/local/bin/pnpx
-
 pnpm add -D vitepress
 pnpm i vitepress-plugin-comment-with-giscus
 pnpm i vitepress-plugin-back-to-top
 pnpm add -D busuanzi.pure.js
 pnpm add -D markdown-it-mathjax3
 pnpm i @mermaid-js/mermaid-mindmap@9.3.0 mermaid@9.1.0 vitepress-plugin-mermaid@2.0.10
 pnpm i medium-zoom
```

### Comparing `youqu-2.5.3/youqu/env.sh` & `youqu-2.5.4/youqu/setting/env_vir.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
-source ./_env_base.sh
+source ${ROOT_DIR}/setting/_env_base.sh
 echo "
  ██╗   ██╗  ██████╗      ███████╗ ███╗   ██╗ ██╗   ██╗
  ╚██╗ ██╔╝ ██╔═══██╗     ██╔════╝ ████╗  ██║ ██║   ██║
   ╚████╔╝  ██║   ██║     █████╗   ██╔██╗ ██║ ██║   ██║
    ╚██╔╝   ██║▄▄ ██║     ██╔══╝   ██║╚██╗██║ ╚██╗ ██╔╝
     ██║    ╚██████╔╝     ███████╗ ██║ ╚████║  ╚████╔╝
     ╚═╝     ╚══▀▀═╝      ╚══════╝ ╚═╝  ╚═══╝   ╚═══╝
@@ -112,24 +112,26 @@
     pytest-timeout==2.1.0
     allure-pytest==2.9.45
     funnylog
     pdocr-rpc
     image-center
     allure-custom
     letmego
+    tomli
 )
 
 if [ "${ENV_CUT_FLAG}" = "cut" ]; then
     pip_array=(
         pytest==6.2.5
         pytest-rerunfailures==10.2
         pytest-timeout==2.1.0
         allure-pytest==2.9.45
         allure-custom
         funnylog
+        tomli
     )
 fi
 
 for p in ${pip_array[*]}
 do
     pipenv run pip install ${p} -i ${pypi_mirror} > /tmp/env.log 2>&1
     check_status ${p}
@@ -172,10 +174,17 @@
 rm -rf Pipfile
 echo "${python_virtualenv_path}"
 pipenv run pip list
 system_env
 
 echo 'pipenv run python "$@"' | sudo tee /usr/bin/youqu > /dev/null 2>&1
 echo "pipenv shell" | sudo tee /usr/bin/youqu-shell > /dev/null 2>&1
+echo "pipenv --rm" | sudo tee /usr/bin/youqu-shell-rm > /dev/null 2>&1
 sudo chmod +x /usr/bin/youqu
 sudo chmod +x /usr/bin/youqu-shell
+sudo chmod +x /usr/bin/youqu-shell-rm
+
+cp --force ${ROOT_DIR}/src/utils/command_complete.sh ${HOME}/.config/
+echo "source ${HOME}/.config/command_complete.sh" >> $HOME/.bashrc
+source $HOME/.bashrc
+
 cd ${ROOT_DIR};youqu manage.py -h
```

### Comparing `youqu-2.5.3/youqu/env_dev.sh` & `youqu-2.5.4/youqu/setting/env_dev.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
-source ./_env_base.sh
+source ${ROOT_DIR}/setting/_env_base.sh
 
 env(){
 
-    if [ ${debian_platform} == true ]; then
+    if [ "${debian_platform}" = "true" ]; then
         sudo apt update
     fi
 
     deb_array=(
         python3-pip
         sshpass
         scrot
@@ -27,18 +27,19 @@
         deb_array=(
             python3-pip
             sshpass
             openjdk-11-jdk-headless
         )
     fi
 
-    if [ ${debian_platform} == false ]; then
+    if [ "${debian_platform}" = "false" ]; then
         deb_array[${#deb_array[@]}]=java-11-openjdk-headless
         deb_array[${#deb_array[@]}]=python3-tkinter
         deb_array[${#deb_array[@]}]=xdotool
+        deb_array[${#deb_array[@]}]=opencv
     fi
 
     for deb in ${deb_array[*]}
     do
         sudo ${yq} install -y ${deb} > /tmp/env.log 2>&1
         check_status ${deb}
     done
@@ -68,27 +69,33 @@
     pytest-timeout==2.1.0
     allure-pytest==2.9.45
     pdocr-rpc
     allure-custom
     funnylog
     image-center
     letmego
+    tomli
 )
 # 裁剪基础环境
 if [ "${ENV_CUT_FLAG}" = "cut" ]; then
     pip_array=(
         pytest==6.2.5
         pytest-rerunfailures==10.2
         pytest-timeout==2.1.0
         allure-pytest==2.9.45
         allure-custom
         funnylog
+        tomli
     )
 fi
 
+if [ ${debian_platform} == false ]; then
+        pip_array[${#pip_array[@]}]=numpy
+    fi
+
 for p in ${pip_array[*]}
 do
     sudo pip3 install ${p} > /tmp/env.log 2>&1
     check_status ${p}
     pip3 list | grep -v grep | grep ${p}
 done
 echo "${PASSWORD}" | sudo -S su > /dev/null 2>&1
```

### Comparing `youqu-2.5.3/youqu/ruff.toml` & `youqu-2.5.4/youqu/ruff.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/startproject.py` & `youqu-2.5.4/youqu/startproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,12 +34,14 @@
                 os.system(f"rm -rf {root}/{d}")
     conf = ConfigParser()
     try:
         conf.read(f"{root_dir}/CURRENT")
         youqu_version = conf.get("current", "tag")
     except NoSectionError:
         youqu_version = None
-    print(f"The project: [\033[0;32m{project_name}\033[0m],has been created by youqu{f'-{youqu_version}' if youqu_version else ''}")
+    print(
+        f"The project: [\033[0;32m{project_name}\033[0m],has been created by youqu{f'-{youqu_version}' if youqu_version else ''}"
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `youqu-2.5.3/youqu/setting/globalconfig.ini` & `youqu-2.5.4/youqu/setting/globalconfig.ini`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/globalconfig.py` & `youqu-2.5.4/youqu/setting/globalconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 from configparser import RawConfigParser  # 解决读取log报错
 from enum import Enum
 from enum import unique
 from getpass import getuser
 from os import popen
-from os import getenv
 from os.path import abspath
 from os.path import dirname
 from os.path import join
+from os.path import exists
 from platform import machine
 from time import strftime
 import pathlib
 
 
 # pylint: disable=C0116,C0103,C0103,C0115,R0903
 
@@ -197,21 +197,25 @@
     GIT_PASSWORD = log_cli.get("GIT_PASSWORD", default="")
     BRANCH = log_cli.get("BRANCH", default="")
     DEPTH = log_cli.get("DEPTH", default="")
     START_DATE = log_cli.get("STAR_TDATE", default="")
     END_DATE = log_cli.get("END_DATE", default="")
 
     # ====================== 动态获取变量 ======================
-    version_cfg = GetCfg("/etc/os-version", "Version")
-    VERSION = (version_cfg.get("EditionName[zh_CN]") or "") + (
-            version_cfg.get("MinorVersion") or ""
-    )
+    VERSION = ""
+    if exists("/etc/os-version"):
+        version_cfg = GetCfg("/etc/os-version", "Version")
+        VERSION = (version_cfg.get("EditionName[zh_CN]") or "") + (
+                version_cfg.get("MinorVersion") or ""
+        )
     # IP
     HOST_IP = str(popen("hostname -I |awk '{print $1}'").read()).strip("\n").strip()
-    PRODUCT_INFO = popen("cat /etc/product-info").read()
+    PRODUCT_INFO = ""
+    if exists("cat /etc/product-info"):
+        PRODUCT_INFO = popen("cat /etc/product-info").read()
     # machine type
     # e.g. x86_64
     SYS_ARCH = machine()
     LANGUAGE_INI = GetCfg(join(SETTING_PATH, "template/language.ini"), "language")
 
     current_tag = GetCfg(f"{ROOT_DIR}/CURRENT", "current").get("tag")
 
@@ -281,21 +285,20 @@
     REMOVED_INDEX = "removed_index"
     PMS_ID_INDEX = "pms_id_index"
 
 
 @unique
 class FixedCsvTitle(Enum):
     case_id = "脚本ID"
-    pms_case_id = "PMS用例ID"
+    pms_case_id = "*PMS用例ID"
     case_level = "用例级别"
     case_type = "用例类型"
-    device_type = "设备类型"
+    device_type = "*设备类型"
     case_from = "一二级bug自动化"
-    online_obj = "上线对象"
-    test_level = "测试级别"
+    online_obj = "*上线对象"
     skip_reason = "跳过原因"
     fixed = "确认修复"
     removed = "废弃用例"
 
 
 @unique
 class SystemPath(Enum):
```

### Comparing `youqu-2.5.3/youqu/setting/pylintrc.cfg` & `youqu-2.5.4/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/skipif.py` & `youqu-2.5.4/youqu/setting/skipif.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.5.4/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.5.4/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.5.4/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/__init__.py` & `youqu-2.5.4/youqu/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,22 +46,22 @@
     ShortCut,
     Calculate,
     OCR,
 ):
     """src"""
 
     def __init__(
-            self,
-            name=None,
-            description=None,
-            config_path=None,
-            number=-1,
-            check_start=True,
-            ui_name=None,
-            **kwargs,
+        self,
+        name=None,
+        description=None,
+        config_path=None,
+        number=-1,
+        check_start=True,
+        ui_name=None,
+        **kwargs,
     ):
         """dogtail or button center param
         :param kwargs: app_name, desc, number
         """
         self.dog = DogtailUtils(
             name=name,
             description=description,
```

### Comparing `youqu-2.5.3/youqu/src/assert_common.py` & `youqu-2.5.4/youqu/src/assert_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114
 import os
 from time import sleep
 from typing import Union
 
 try:
     import pyscreenshot
 except ModuleNotFoundError:
@@ -25,40 +22,37 @@
 from src.custom_exception import AssertOptionError
 from src.cmdctl import CmdCtl
 from src.button_center import ButtonCenter
 from src import logger, log
 from setting.globalconfig import GlobalConfig
 
 
-# pylint: disable=too-many-public-methods
 @log
 class AssertCommon:
     """
     自定义断言类
     """
 
     @staticmethod
     def assert_image_exist(
-            widget: str,
-            rate: float = None,
-            multiple: bool = False,
-            picture_abspath: str = None,
-            network_retry: int = None,
-            pause: [int, float] = None,
-            timeout: [int, float] = None,
-            match_number: int = None,
+        widget: str,
+        rate: float = None,
+        multiple: bool = False,
+        picture_abspath: str = None,
+        network_retry: int = None,
+        pause: [int, float] = None,
+        timeout: [int, float] = None,
+        match_number: int = None,
     ):
         """
          期望界面存在模板图片
         :param widget: 图片路径 例：apps/autotest_app/assert_res/1.png
         :param rate: 匹配相似度
         """
-        logger.info(
-            f"屏幕上匹配图片< {f'***{widget[-40:]}' if len(widget) >= 40 else widget} >"
-        )
+        logger.info(f"屏幕上匹配图片< {f'***{widget[-40:]}' if len(widget) >= 40 else widget} >")
 
         try:
             ImageUtils.find_image(
                 widget,
                 rate=rate,
                 multiple=multiple,
                 picture_abspath=picture_abspath,
@@ -70,48 +64,46 @@
         except TemplateElementNotFound as exc:
             raise AssertionError(exc) from TemplateElementNotFound
         except Exception as exc:
             raise AssertOptionError(exc) from Exception
 
     @classmethod
     def assert_image_exist_during_time(
-            cls,
-            widget: str,
-            screen_time: Union[float, int],
-            rate: float = None,
-            pause: Union[int, float] = None,
+        cls,
+        widget: str,
+        screen_time: Union[float, int],
+        rate: float = None,
+        pause: Union[int, float] = None,
     ):
         """
         在一段时间内截图多张图片进行识别，其中有一张图片识别成功即返回结果;
         适用于气泡类的断言，比如气泡在1秒内消失，如果用常规的图像识别则有可能无法识别到；
         :param image_path: 要识别的模板图片；
         :param screen_time: 截取屏幕图片的时间，单位秒；
         :param rate: 识别率；
         :param pause: 截取屏幕图片的间隔时间，默认不间隔；
         """
-        logger.info(
-            f"屏幕上匹配图片< {f'***{widget[-40:]}' if len(widget) >= 40 else widget} >"
-        )
+        logger.info(f"屏幕上匹配图片< {f'***{widget[-40:]}' if len(widget) >= 40 else widget} >")
         try:
             ImageUtils.get_during(widget, screen_time, rate, pause)
         except TemplateElementNotFound as exc:
             raise AssertionError(exc) from TemplateElementNotFound
         except Exception as exc:
             raise AssertOptionError(exc) from Exception
 
     @staticmethod
     def assert_image_not_exist(
-            widget: str,
-            rate: float = None,
-            multiple: bool = False,
-            picture_abspath: str = None,
-            network_retry: int = None,
-            pause: [int, float] = None,
-            timeout: [int, float] = None,
-            match_number: int = None,
+        widget: str,
+        rate: float = None,
+        multiple: bool = False,
+        picture_abspath: str = None,
+        network_retry: int = None,
+        pause: [int, float] = None,
+        timeout: [int, float] = None,
+        match_number: int = None,
     ):
         """
          期望界面不存在模板图片
         :param widget: 图片路径 apps/autotest_app/assert_res/1.png
         :param rate: 匹配相似度
         """
         logger.info(
@@ -320,17 +312,15 @@
         config = {"浅色": (248, 248, 248), "深色": (37, 37, 37)}
         exp_color = config[expect]
         # 在data/pic_res这个目录下生成一张临时的图，每次生成会被覆盖
         if GlobalConfig.IS_X11:
             pyscreenshot.grab().save(GlobalConfig.SCREEN_CACHE)
         else:
             GlobalConfig.SCREEN_CACHE = (
-                os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
-                .read()
-                .strip("\n")
+                os.popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen").read().strip("\n")
             )
         color_list = ImageUtils.find_image_color(GlobalConfig.SCREEN_CACHE)
         proportion = round(color_list.count(exp_color) / len(color_list), 2)
         if proportion < 0.6:
             raise AssertionError(
                 f"{expect}主题颜色占屏幕总体颜色占比低于60%，实际占比{proportion * 100}%，初步断言主题失败"
             )
@@ -394,24 +384,24 @@
         :param endwith: 文件后缀， txt，rar 等
         """
         if not FileCtl.find_files(path, endwith=endwith):
             raise AssertionError(f"路径 {path} 下，不存在以 {endwith} 结尾的文件")
 
     @staticmethod
     def assert_ocr_exist(
-            *args,
-            picture_abspath=None,
-            similarity=0.6,
-            return_first=False,
-            lang="ch",
-            network_retry: int = None,
-            pause: [int, float] = None,
-            timeout: [int, float] = None,
-            max_match_number: int = None,
-            mode: str = "all",
+        *args,
+        picture_abspath=None,
+        similarity=0.6,
+        return_first=False,
+        lang="ch",
+        network_retry: int = None,
+        pause: [int, float] = None,
+        timeout: [int, float] = None,
+        max_match_number: int = None,
+        mode: str = "all",
     ):
         """
         断言文案存在
         :param args:
             目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
             如果不传参，返回图片中识别到的所有字符串。
         :param picture_abspath: 要识别的图片路径，如果不传默认截取全屏识别。
@@ -460,23 +450,23 @@
                         f"通过OCR未识别到：{args}中的任意一个",
                         f"{pic if pic else GlobalConfig.SCREEN_CACHE}",
                     )
                 )
 
     @staticmethod
     def assert_ocr_not_exist(
-            *args,
-            picture_abspath=None,
-            similarity=0.6,
-            return_first=False,
-            lang="ch",
-            network_retry: int = None,
-            pause: [int, float] = None,
-            timeout: [int, float] = None,
-            max_match_number: int = None,
+        *args,
+        picture_abspath=None,
+        similarity=0.6,
+        return_first=False,
+        lang="ch",
+        network_retry: int = None,
+        pause: [int, float] = None,
+        timeout: [int, float] = None,
+        max_match_number: int = None,
     ):
         """断言文案不存在"""
         pic = None
         if picture_abspath is not None:
             pic = picture_abspath + ".png"
         res = OCR.ocr(
             *args,
```

### Comparing `youqu-2.5.3/youqu/src/button_center.py` & `youqu-2.5.4/youqu/src/button_center.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114
+
 import re
 from configparser import ConfigParser, NoSectionError
 from time import sleep
 
 import dbus
 
 from setting.globalconfig import GlobalConfig
@@ -19,18 +19,20 @@
 from src.wayland_wininfo import WaylandWindowInfo
 
 
 class ButtonCenter:
     """
     根据应用程序中控件元素的相对坐标，通过配置元素的x、y、w和h来定位元素在屏幕中的位置，并返回用于鼠标和键盘操作的坐标。
     """
-    # pylint: disable=too-many-arguments,too-many-locals,too-many-public-methods
+
     __author__ = "Mikigo <huangmingqiang@uniontech.com>, Litao <litaoa@uniontech.com>"
 
-    def __init__(self, app_name: str, config_path: str, number: int = -1, pause: int = 1, retry: int = 1):
+    def __init__(
+        self, app_name: str, config_path: str, number: int = -1, pause: int = 1, retry: int = 1
+    ):
         """
         :param app_name: 系统应用软件包，例如，dde-file-manager
         :param config_path: ui 定位配置文件路径（绝对路径）
         :param number: 默认为 -1, 即最后一个窗口
             如果你想指定不同的窗口，你可以在实例化对象的时候显式的传入 number，第一个为 0
         """
         self.app_name = app_name
@@ -44,20 +46,24 @@
         """
          窗口信息
         :return:  窗口的基本信息，左上角坐标，窗口宽高等
         """
         if GlobalConfig.IS_X11:
             try:
                 # Get window_operate ID based on package name
-                app_id = CmdCtl.run_cmd(
-                    f"xdotool search --classname --onlyvisible {self.app_name}",
-                    interrupt=False,
-                    out_debug_flag=False,
-                    command_log=False,
-                ).strip().split("\n")
+                app_id = (
+                    CmdCtl.run_cmd(
+                        f"xdotool search --classname --onlyvisible {self.app_name}",
+                        interrupt=False,
+                        out_debug_flag=False,
+                        command_log=False,
+                    )
+                    .strip()
+                    .split("\n")
+                )
                 app_id_list = [int(_id) for _id in app_id if _id]
                 app_id_list.sort()
                 logger.debug(f"app_id_list: {app_id_list}")
                 return CmdCtl.run_cmd(
                     f"xwininfo -id {app_id_list[self.number]}",
                     interrupt=False,
                     out_debug_flag=False,
@@ -109,20 +115,24 @@
                 window_width = re.findall(r"Width.*:\s(\d+)", app_window_info)[0]
                 window_height = re.findall(r"Height.*:\s(\d+)", app_window_info)[0]
                 window_x, window_y = result
             else:
                 self.wwininfo = WaylandWindowInfo()
                 if hasattr(self.wwininfo.library, "GetAllWindowStatesList"):
                     app_window_info = self.window_info()
-                    window_x, window_y, window_width, window_height = app_window_info.get("location")
+                    window_x, window_y, window_width, window_height = app_window_info.get(
+                        "location"
+                    )
                 else:
                     app_window_info = self.window_info()
                     name = app_window_info.get("name")
                     if name != self.app_name:
-                        raise ValueError(f"您想要获取的窗口为：{self.app_name}, 但实际获取的窗口为：{name}")
+                        raise ValueError(
+                            f"您想要获取的窗口为：{self.app_name}, 但实际获取的窗口为：{name}"
+                        )
                     window_x, window_y, window_width, window_height = app_window_info.get("wininfo")
             logger.debug(
                 f"窗口左上角坐标 {window_x, window_y},获取窗口大小 {window_width}*{window_height}"
             )
             return (int(window_x), int(window_y), int(window_width), int(window_height))
         except (IndexError, KeyError) as exc:
             raise GetWindowInformation(f"获取窗口大小错误 {exc}") from exc
@@ -140,15 +150,17 @@
                 if not result:
                     sleep(1)
                     result = re.findall(re_pattern, self.window_info())
                 window_x, window_y = result
             else:
                 self.wwininfo = WaylandWindowInfo()
                 if hasattr(self.wwininfo.library, "GetAllWindowStatesList"):
-                    window_x, window_y, window_width, window_height = app_window_info.get("location")
+                    window_x, window_y, window_width, window_height = app_window_info.get(
+                        "location"
+                    )
                 else:
                     window_x, window_y, window_width, window_height = app_window_info.get("wininfo")
             logger.debug(f"窗口左上角坐标 {window_x, window_y}")
             return int(window_x), int(window_y)
         except (ValueError, KeyError) as exc:
             raise GetWindowInformation(f"获取窗口左上角坐标错误 {exc}") from exc
 
@@ -161,15 +173,17 @@
             app_window_info = self.window_info()
             if GlobalConfig.IS_X11:
                 window_width = re.findall(r"Width.*:\s(\d+)", app_window_info)[0]
                 window_height = re.findall(r"Height.*:\s(\d+)", app_window_info)[0]
             else:
                 self.wwininfo = WaylandWindowInfo()
                 if hasattr(self.wwininfo.library, "GetAllWindowStatesList"):
-                    window_x, window_y, window_width, window_height = app_window_info.get("location")
+                    window_x, window_y, window_width, window_height = app_window_info.get(
+                        "location"
+                    )
                 else:
                     window_x, window_y, window_width, window_height = app_window_info.get("wininfo")
             logger.debug(f"获取窗口大小 {window_width}*{window_height}")
             return int(window_width), int(window_height)
         except (IndexError, KeyError) as exc:
             raise GetWindowInformation(f"获取窗口大小错误 {exc}") from exc
 
@@ -323,34 +337,30 @@
         """
         window_x, window_y = self.window_right_top_position()
         b_x = window_x - button_x - button_w / 2
         b_y = window_y + button_y + button_h / 2
         logger.debug(f"右上角按钮的中心坐标 {b_x, b_y}")
         return b_x, b_y
 
-    def btn_center_by_left_bottom(
-            self, button_x, button_y, button_w, button_h
-    ) -> tuple:
+    def btn_center_by_left_bottom(self, button_x, button_y, button_w, button_h) -> tuple:
         """
          根据左下角的坐标按钮的中心坐标
         :param button_x: 控件左下角相对于窗口左下角的横向距离
         :param button_y: 控件左下角相对于窗口左下角的纵向距离
         :param button_w: 控件宽度
         :param button_h: 控件高度
         :return:  控件的中心坐标 （1, 1）
         """
         window_x, window_y = self.window_left_bottom_position()
         b_x = window_x + button_x + button_w / 2
         b_y = window_y - button_y - button_h / 2
         logger.debug(f"左下角按钮的中心坐标 {b_x, b_y}")
         return b_x, b_y
 
-    def btn_center_by_right_bottom(
-            self, button_x, button_y, button_w, button_h
-    ) -> tuple:
+    def btn_center_by_right_bottom(self, button_x, button_y, button_w, button_h) -> tuple:
         """
          根据右下角的坐标按钮的中心坐标
         :param button_x: 控件右下角相对于窗口右下角的横向距离
         :param button_y: 控件右下角相对于窗口右下角的纵向距离
         :param button_w: 控件宽度
         :param button_h: 控件高度
         :return:  控件的中心坐标 （1, 1）
@@ -418,20 +428,20 @@
         window_x, window_y = self.window_right_bottom_position()
         b_x = window_x - button_x - button_w
         b_y = window_y - button_y - button_h
         logger.debug(f"右下角按钮的截取区域左上角 {b_x, b_y}, 控件长宽 {button_w, button_h}")
         return b_x, b_y, button_w, button_h
 
     def btn_center(
-            self,
-            btn_name,
-            offset_x=None,
-            multiplier_x=None,
-            offset_y=None,
-            multiplier_y=None,
+        self,
+        btn_name,
+        offset_x=None,
+        multiplier_x=None,
+        offset_y=None,
+        multiplier_y=None,
     ) -> tuple:
         """
          获取元素的中心坐标
         :param btn_name: 控件名
         :param offset_x
             正数为右移动
             负数为左移动
@@ -479,34 +489,30 @@
             )
         elif direction == "window_size":
             btn_x, btn_y, button_w, button_y = self.window_location_and_sizes()
             btn_x = btn_x + button_w / 2
             btn_y = btn_y + button_y / 2
         if btn_x and btn_y:
             if offset_x:
-                btn_x = btn_x + int(offset_x) * (
-                    int(multiplier_x) if multiplier_x else 1
-                )
+                btn_x = btn_x + int(offset_x) * (int(multiplier_x) if multiplier_x else 1)
             if offset_y:
-                btn_y = btn_y + int(offset_y) * (
-                    int(multiplier_y) if multiplier_y else 1
-                )
+                btn_y = btn_y + int(offset_y) * (int(multiplier_y) if multiplier_y else 1)
             logger.debug(f"[{btn_name}] 坐标：{str(btn_x)}, {str(btn_y)})")
             return btn_x, btn_y
         raise NoSetReferencePoint(
             f"{direction}, 默认参考点 {default_point + default_boundary_point}"
         )
 
     def btn_size(
-            self,
-            btn_name: str,
-            offset_x: [int, float] = None,
-            multiplier_x: [int, float] = None,
-            offset_y: [int, float] = None,
-            multiplier_y: [int, float] = None,
+        self,
+        btn_name: str,
+        offset_x: [int, float] = None,
+        multiplier_x: [int, float] = None,
+        offset_y: [int, float] = None,
+        multiplier_y: [int, float] = None,
     ) -> tuple:
         """
          获取元素的左上角坐标及长宽
         :param btn_name: 控件名
         :param offset_x
             正数为右移动
             负数为左移动
@@ -528,33 +534,27 @@
         default_boundary_point = (
             "top_center",
             "bottom_center",
             "left_center",
             "right_center",
         )
         if direction in default_point:
-            btn_x, btn_y, button_w, button_y = getattr(self, f"btn_pic_by_{direction}")(
-                *position
-            )
+            btn_x, btn_y, button_w, button_y = getattr(self, f"btn_pic_by_{direction}")(*position)
         elif direction in default_boundary_point:
             window_x, window_y = getattr(self, f"window_{direction}_position")()
             btn_x = window_x + position[0] - (0 if position[0] > 0 else position[2])
             btn_y = window_y + position[1] - (0 if position[1] > 0 else position[3])
             button_w, button_y = position[2], position[3]
         elif direction == "window_size":
             btn_x, btn_y, button_w, button_y = self.window_location_and_sizes()
         if btn_x != "" and btn_y != "":
             if offset_x:
-                btn_x = btn_x + int(offset_x) * (
-                    int(multiplier_x) if multiplier_x else 1
-                )
+                btn_x = btn_x + int(offset_x) * (int(multiplier_x) if multiplier_x else 1)
             if offset_y:
-                btn_y = btn_y + int(offset_y) * (
-                    int(multiplier_y) if multiplier_y else 1
-                )
+                btn_y = btn_y + int(offset_y) * (int(multiplier_y) if multiplier_y else 1)
             logger.debug(
                 f"[{btn_name}] 左上角坐标：{str(btn_x)}, {str(btn_y)}), 长宽 {button_w, button_y}"
             )
             return btn_x, btn_y, button_w, button_y
         raise NoSetReferencePoint(
             f"{direction}, 默认参考点 {default_point + default_boundary_point}"
         )
@@ -627,20 +627,24 @@
     def get_lastest_window_id(self, app_name: str) -> int:
         """
          获取应用的所有窗口编号，并返回编号最大的窗口ID
         :return: 返回最新创建的窗口编号
         """
         if GlobalConfig.IS_X11:
             try:
-                app_id = CmdCtl.run_cmd(
-                    f"xdotool search --classname --onlyvisible {app_name}",
-                    interrupt=False,
-                    out_debug_flag=False,
-                    command_log=False,
-                ).strip().split("\n")
+                app_id = (
+                    CmdCtl.run_cmd(
+                        f"xdotool search --classname --onlyvisible {app_name}",
+                        interrupt=False,
+                        out_debug_flag=False,
+                        command_log=False,
+                    )
+                    .strip()
+                    .split("\n")
+                )
                 app_id_list = [int(_id) for _id in app_id if _id]  # to int
                 app_id_list.sort()
                 return app_id_list[-1]
             except Exception as exc:
                 raise ApplicationStartError(f"{app_name, exc}") from exc
         else:
             info = self.wwininfo.window_info().get(self.app_name)
```

### Comparing `youqu-2.5.3/youqu/src/calculate.py` & `youqu-2.5.4/youqu/src/calculate.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 import math
 from xmlrpc.client import ServerProxy
 
 from setting.globalconfig import GlobalConfig
 
 try:
     import numpy as np
+
     GET_NP_FROM_RPC = False
 except ModuleNotFoundError:
     GET_NP_FROM_RPC = True
 
-from src  import logger
+from src import logger
 
 
 class Calculate:
     """Calculate"""
 
     @staticmethod
     def coordinate_distance(start: tuple, end: tuple):
```

### Comparing `youqu-2.5.3/youqu/src/cmdctl.py` & `youqu-2.5.4/youqu/src/cmdctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from src.custom_exception import ShellExecutionFailed
 from src import logger
 from setting import conf
 
 
 class CmdCtl:
     """命令行工具"""
+
     # pylint: disable=too-many-arguments,too-many-locals,too-many-public-methods
     # clean_env也要用
     GREP_LIST = (
         "grep",
         "pytest",
         "python",
         "asan",
@@ -65,30 +66,35 @@
             data = ex.__str__()
             exitcode = -1
         if data[-1:] == "\n":
             data = data[:-1]
         return exitcode, data
 
     @classmethod
-    def sudo_run_cmd(cls, command, interrupt=False, timeout=25, out_debug_flag=True,
-                     command_log=True, password=None):
+    def sudo_run_cmd(
+        cls,
+        command,
+        interrupt=False,
+        timeout=25,
+        out_debug_flag=True,
+        command_log=True,
+        password=None,
+    ):
         if password is None:
             password = conf.PASSWORD
         return cls.run_cmd(
             f"echo '{password}' | sudo -S {command}",
             interrupt=interrupt,
             timeout=timeout,
             out_debug_flag=out_debug_flag,
-            command_log=command_log
+            command_log=command_log,
         )
 
     @classmethod
-    def run_cmd(
-            cls, command, interrupt=False, timeout=25, out_debug_flag=True, command_log=True
-    ):
+    def run_cmd(cls, command, interrupt=False, timeout=25, out_debug_flag=True, command_log=True):
         """
          执行shell命令
         :param command: shell 命令
         :param interrupt: 命令异常时是否中断
         :param timeout: 命令执行超时
         :param out_debug_flag: 命令返回信息输出日志
         :param command_log: 执行的命令字符串日志
@@ -226,26 +232,23 @@
     @classmethod
     def change_app_to_default_theme(cls, app_name):
         """
          修改app主题跟随系统
         :param app_name: 应用名字
         """
         cls.run_cmd(
-            f"gsettings set com.deepin.dtk:/dtk/deepin/{app_name}/ "
-            "palette-type UnknownType"
+            f"gsettings set com.deepin.dtk:/dtk/deepin/{app_name}/ " "palette-type UnknownType"
         )
 
     @classmethod
     def kill_process(cls, process, grep_list: [list, tuple] = None):
         """
          杀进程
         :param process: 进程名
         """
         # 杀进程要过滤的进程
         if grep_list:
             cls.GREP_LIST = grep_list
         cmd = ""
         for i in cls.GREP_LIST:
             cmd += f"grep -v {i} | "
-        os.system(
-            f"ps -ef | grep {process} | {cmd}cut -c 9-15 | xargs kill -9 > /dev/null 2>&1"
-        )
+        os.system(f"ps -ef | grep {process} | {cmd}cut -c 9-15 | xargs kill -9 > /dev/null 2>&1")
```

### Comparing `youqu-2.5.3/youqu/src/csvctl.py` & `youqu-2.5.4/youqu/src/csvctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,34 @@
 from collections import Counter
 
 from setting.globalconfig import GlobalConfig, FixedCsvTitle
 from src.rtk._base import transform_app_name
 
 
 class CsvControl:
-    """csv control"""
 
     def __init__(self, app_name=None):
         self.walk_dir = (
             f"{GlobalConfig.APPS_PATH}/{transform_app_name(app_name)}"
             if app_name
             else GlobalConfig.APPS_PATH
         )
         self.csv_path_dict, self.py_path_dict = self.scan_csv_and_py()
 
     def scan_csv_and_py(self):
-        """scan csv and case py"""
         csv_path_dict = {}
         py_path_dict = {}
         for root, _, files in os.walk(self.walk_dir):
             py_files = []
             for file in files:
                 if file.endswith(".csv") and file != "case_list.csv":
                     csv_path_dict[os.path.splitext(file)[0]] = f"{root}/{file}"
                 if file.startswith("test_") and file.endswith(".py"):
                     case_name = []
-                    _case_name = re.findall(
-                        r"test_(.*?)_(\d+)_\d+.py|test_(.*?)_(\d+).py", file
-                    )
+                    _case_name = re.findall(r"test_(.*?)_(\d+)_\d+.py|test_(.*?)_(\d+).py", file)
                     if _case_name:
                         _case_name = _case_name[0]
                         if isinstance(_case_name, tuple):
                             for i in _case_name:
                                 if i:
                                     case_name.append(i)
 
@@ -53,15 +49,14 @@
                         py_path_dict[case_name[0]] = py_files
 
         for i in py_path_dict:
             py_path_dict[i] = sorted(py_path_dict[i], key=lambda x: int(x[-1]))
         return csv_path_dict, py_path_dict
 
     def delete_mark_in_csv_if_not_exists_py(self):
-        """delete mark in csv if not exists case py"""
         res = self.scan_csv_and_py()
         if res is None:
             return
         csv_path_dict, py_path_dict = res
         flag = False
         for csv_name in csv_path_dict:
             for case_name in py_path_dict:
@@ -72,15 +67,17 @@
                     taglines = [txt.strip().split(",") for txt in csv_txt_list[1:]]
                     new_taglines = []
                     py_case_paths = py_path_dict.get(case_name)
                     for tag in taglines:
                         try:
                             csv_case_id = f"{int(tag[0]):0>3}"
                         except ValueError as e:
-                            raise ValueError(f"文件：{csv_path} 里面似乎格式有点问题,出现了一个报错：{e}")
+                            raise ValueError(
+                                f"文件：{csv_path} 里面似乎格式有点问题,出现了一个报错：{e}"
+                            )
                         for py_case in py_case_paths:
                             py_case_id = py_case[-1]
                             if csv_case_id == py_case_id:
                                 new_taglines.append(tag)
                                 break
                         else:
                             print(f"{tag} will remove from {csv_path}")
@@ -143,13 +140,13 @@
                 else:
                     for i in csv_taglines:
                         if i[0] == case_id or int(i[0]) == int(case_id):
                             break
                     else:
                         with open(csv_path, "a+", encoding="utf-8") as f:
                             f.write(f"{case_id}{comma_num * ','}" + "\n")
-        print("Complete synchronization of automated test script id to csv file")
+        print("完成自动化用例脚本同步到CSV文件。")
 
 
 if __name__ == "__main__":
     CsvControl().delete_mark_in_csv_if_not_exists_py()
     CsvControl().async_mark_to_csv()
```

### Comparing `youqu-2.5.3/youqu/src/custom_exception.py` & `youqu-2.5.4/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/dbus_utils.py` & `youqu-2.5.4/youqu/src/dbus_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 
 import dbus
 
 
 class DbusUtils:
```

### Comparing `youqu-2.5.3/youqu/src/desktop.py` & `youqu-2.5.4/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/dogtail_utils.py` & `youqu-2.5.4/youqu/src/dogtail_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,34 +32,31 @@
 from src.mouse_key import MouseKey
 
 
 class DogtailUtils(MouseKey):
     """
     通过属性进行元素定位和操作。
     """
+
     # pylint: disable=too-many-arguments,too-many-locals,too-many-public-methods
     __author__ = "Mikigo <huangmingqiang@uniontech.com>, Litao <litaoa@uniontech.com>"
 
-    def __init__(
-            self, name=None, description=None, number=-1, check_start=True, key: dict = None
-    ):
+    def __init__(self, name=None, description=None, number=-1, check_start=True, key: dict = None):
         if GlobalConfig.NO_DOGTAIL:
             raise EnvironmentError("Dogtail 及其相关依赖存在问题,调用相关方法失败~")
         config.logDebugToStdOut = False
         self.name = name
         self.description = description
         try:
             if name:
                 self.obj = root.application(self.name, self.description)
             else:
                 self.obj = root
             if number > 0:
-                self.obj = self.obj.findChildren(
-                    predicate.GenericPredicate(**key)
-                )[number]
+                self.obj = self.obj.findChildren(predicate.GenericPredicate(**key))[number]
 
         except SearchError:
             if check_start:
                 search_app = CmdCtl.run_cmd(f"ps -ef | grep {self.name}")
                 logger.error(search_app)
                 raise ApplicationStartError(self.name) from SearchError
 
@@ -124,19 +121,15 @@
         :param button: 1>left,2>middle,3>right
         :return: None
         """
         logger.debug(
             f"""{"左键" if button == 1 else f"{'右键' if button == 3 else '鼠标中健'}"} 点击元素 {element}"""
         )
         mouse_click = (
-            self.click
-            if button == 1
-            else self.right_click
-            if button == 3
-            else self.middle_click
+            self.click if button == 1 else self.right_click if button == 3 else self.middle_click
         )
         mouse_click(*self.element_center(element))
 
     def element_double_click(self, element):
         """
          元素双击
         :return: None
@@ -160,30 +153,28 @@
         if node:
             name = node.group().replace("\\/", "/")[:-1]
         else:
             return False
         if name == "*":
             element = element.children
         else:
-            element = element.findChildren(
-                predicate.GenericPredicate(name), recursive=recursive
-            )
+            element = element.findChildren(predicate.GenericPredicate(name), recursive=recursive)
         return node, element
 
     def __trace(self, element, result, expr):
         if expr.startswith("//"):
             name = expr[2:]
             node, element = self.__evalx(name, element, recursive=True)
         elif expr.startswith("/"):
             name = expr[1:]
             node, element = self.__evalx(name, element, recursive=False)
         else:
             return False
         try:
-            next_node = name[node.end() - 1:]
+            next_node = name[node.end() - 1 :]
             if next_node != "/":
                 for i in element:
                     self.__trace(i, result, next_node)
             else:
                 result += element
         except SearchError:
             raise ElementNotFound(expr) from SearchError
```

### Comparing `youqu-2.5.3/youqu/src/filectl.py` & `youqu-2.5.4/youqu/src/filectl.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 import os
 from copy import deepcopy
 
 from setting.globalconfig import GlobalConfig
-from src  import logger
+from src import logger
 
 
 class FileCtl:
     """
     Operations on system files and directories.
     Realize the addition, deletion, modification
     and query of documents.
     """
+
     # pylint: disable=too-many-arguments,too-many-branches,too-many-nested-blocks
     __author__ = "Mikigo <huangmingqiang@uniontech.com>, Litao <litaoa@uniontech.com>"
 
     @staticmethod
     def creat_files(path: str, file_name: str = "", file_type: str = "dir"):
         """
          创建文件或文件夹
@@ -77,21 +78,18 @@
                             if include in file:
                                 os.system(
                                     f"echo '{GlobalConfig.PASSWORD}' | "
                                     f"sudo -S rm -rf '{abs_file_path}/{file}'"
                                 )
                 elif not ignores and not includes:
                     os.system(
-                        f"echo '{GlobalConfig.PASSWORD}' | "
-                        f"sudo -S rm -rf {abs_file_path}/*"
+                        f"echo '{GlobalConfig.PASSWORD}' | " f"sudo -S rm -rf {abs_file_path}/*"
                     )
                 else:
-                    logger.info(
-                        "This deletion mode is not supported for the time being!"
-                    )
+                    logger.info("This deletion mode is not supported for the time being!")
             # else:
             #     logger.info(f"There are no files in the directory <{path}!>")
         else:
             logger.error(f"{abs_file_path} is not exsits !")
 
     @staticmethod
     def rename_files(path: str, old_name: str, new_name: str):
@@ -104,17 +102,15 @@
         """
         parent_dir = f"/home/{GlobalConfig.USERNAME}/{path}"
         old_abs_path = f"{parent_dir}/{old_name}"
         new_abs_path = f"{parent_dir}/{new_name}"
         os.system(f"mv {old_abs_path} {new_abs_path}")
 
     @staticmethod
-    def move_files(
-        path: str, file_name: str, new_path: str = None, new_file_name: str = None
-    ):
+    def move_files(path: str, file_name: str, new_path: str = None, new_file_name: str = None):
         """
          移动文件
         :param path: 旧路径
         :param file_name: 旧文件
         :param new_path: 新路径
         :param new_file_name: 新文件
         :return:
@@ -196,36 +192,29 @@
                     f"endwith:{endwith}\nrecursive:{recursive}\n"
                     f"{parent_dir}目录下未找到该查找模式的文件～"
                 )
             return files_list
         logger.error(f"{parent_dir} is not exists!")
         return []
 
-
     @classmethod
     def __check_not_includes(
         cls, not_includes, endwith, file, files_list, include, startwith, abs_path, root
     ):
         """Filter criteria for function 'find_files' parameter 'notincludes'"""
         if not_includes:
             for not_include in not_includes:
                 if not_include in file:
                     continue
-                cls.__check_startwith(
-                    endwith, file, files_list, include, startwith, abs_path, root
-                )
+                cls.__check_startwith(endwith, file, files_list, include, startwith, abs_path, root)
         else:
-            cls.__check_startwith(
-                endwith, file, files_list, include, startwith, abs_path, root
-            )
+            cls.__check_startwith(endwith, file, files_list, include, startwith, abs_path, root)
 
     @classmethod
-    def __check_startwith(
-        cls, endwith, file, files_list, include, startwith, abs_path, root
-    ):
+    def __check_startwith(cls, endwith, file, files_list, include, startwith, abs_path, root):
         """Filter criteria for function 'find_files' parameter 'startwith'"""
         if not startwith:
             cls.__check_endwith(endwith, file, files_list, include, abs_path, root)
         else:
             if file.startswith(startwith):
                 cls.__check_endwith(endwith, file, files_list, include, abs_path, root)
```

### Comparing `youqu-2.5.3/youqu/src/filter_image.py` & `youqu-2.5.4/youqu/src/filter_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,14 @@
     pyscreenshot.grab().save(after_img_path)
     after_img = Image.open(after_img_path)
 
     filter_img = ImageChops.difference(before_img, after_img)
     if filter_img.getbbox() is None:
         print(f"{before_img_path}、{after_img_path}两张图片相同")
         return None
-    res_img = (
-        splitext(GlobalConfig.SCREEN_CACHE)[0] + f'_{strftime("%Y%m%d%H%M%S")}.png'
-    )
+    res_img = splitext(GlobalConfig.SCREEN_CACHE)[0] + f'_{strftime("%Y%m%d%H%M%S")}.png'
     filter_img.save(res_img)
     return res_img
 
 
 if __name__ == "__main__":
     filter_image(MouseKey.right_click)
```

### Comparing `youqu-2.5.3/youqu/src/image_utils.py` & `youqu-2.5.4/youqu/src/image_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/mouse_key.py` & `youqu-2.5.4/youqu/src/mouse_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114
+
 import os
 import sys
 from time import sleep
 
 from src import logger
 from src.cmdctl import CmdCtl
 
 os.environ["DISPLAY"] = ":0"
-# pylint: disable=C0103,R0904,C0411
-# pylint: disable=wrong-import-position
+
 from setting.globalconfig import GlobalConfig
 
 
 class HiddenPrints:
     def __enter__(self):
         self._original_stdout = sys.stdout
-        sys.stdout = open(os.devnull, 'w')
+        sys.stdout = open(os.devnull, "w")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         sys.stdout.close()
         sys.stdout = self._original_stdout
 
 
 with HiddenPrints():
@@ -69,23 +66,14 @@
         :return: 鼠标当前的坐标
         """
         position = pyautogui.position()
         if out_log:
             logger.debug(f"当前鼠标坐标 {position}")
         return position
 
-    # @classmethod
-    # def input_chinese(cls, text, delay_time=300):
-    #     """
-    #     输入中文
-    #     """
-    #     CmdCtl.run_cmd(f"xdotool type --delay {delay_time} '{text}'", timeout=60)
-    #     logger.debug(f"输入文本 {text}")
-    #     sleep(1)
-
     @classmethod
     def move_to(cls, _x, _y, duration=0.4):
         """
          移动到指定位置
         :param _x: x
         :param _y: y
         :param duration:移动的速度
@@ -147,47 +135,41 @@
     def right_click(cls, _x=None, _y=None):
         """
          单击鼠标右键
         :param _x:
         :param _y:
         :return:
         """
-        logger.debug(
-            f"鼠标右键坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}"
-        )
+        logger.debug(f"鼠标右键坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}")
         pyautogui.rightClick(x=_x, y=_y)
         sleep(1)
 
     @classmethod
     def double_click(cls, _x=None, _y=None, interval=0.3):
         """
          双击鼠标左键
         :param _x:
         :param _y:
         :param interval: 两次点击的间隔，默认 0.3s
         :return:
         """
-        logger.debug(
-            f"鼠标左键双击坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}"
-        )
+        logger.debug(f"鼠标左键双击坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}")
         pyautogui.doubleClick(x=_x, y=_y, interval=interval)
         # CmdCtl.run_cmd(f"xdotool mousemove {_x} {_y} click --repeat 2 1")
         sleep(1)
 
     @classmethod
     def triple_click(cls, _x=None, _y=None):
         """
          三击鼠标左键
         :param _x:
         :param _y:
         :return:
         """
-        logger.debug(
-            f"鼠标三连击坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}"
-        )
+        logger.debug(f"鼠标三连击坐标 {(_x, _y) if _x else cls.current_location(out_log=False)}")
         pyautogui.tripleClick(x=_x, y=_y, interval=0.3)
         sleep(1)
 
     @classmethod
     def drag_to(cls, _x, _y, duration=0.4, delay=1):
         """
          拖拽到指定位置(绝对位置)
@@ -206,17 +188,15 @@
         """
          按住鼠标左键,拖拽到指定位置(相对位置)
         :param _x: 拖拽的相对位置x，正数向右，负数向左
         :param _y: 拖拽的相对位置y，正数向下，负数向上
         :return:
         """
         logger.debug(f"鼠标从当前位置拖拽到相对坐标 ({_x, _y})")
-        pyautogui.dragRel(
-            xOffset=int(_x), yOffset=int(_y), duration=0.4, mouseDownUp=True
-        )
+        pyautogui.dragRel(xOffset=int(_x), yOffset=int(_y), duration=0.4, mouseDownUp=True)
         sleep(1)
 
     @classmethod
     def mouse_down(cls, _x=None, _y=None, button=1):
         """
          按住鼠标键不放
         :param _x:
@@ -256,19 +236,20 @@
         else:
             direct = "下"
         logger.debug(f"向<{direct}>滑动滚轮")
         sleep(duration)
 
     @classmethod
     def input_message(
-            cls, message,
+            cls,
+            message,
             delay_time: int = 300,
             interval: [int, float] = 0.2,
             wayland_shift: bool = False,
-            _ydotool: bool = False
+            _ydotool: bool = False,
     ):
         """
          输入字符串
         :param message: 输入的内容
         :param delay_time: 延迟时间
         :param interval:
         :return:
@@ -280,17 +261,15 @@
             for _ch in message:
                 if "\u4e00" <= _ch <= "\u9fff":
                     return True
             return False
 
         if GlobalConfig.IS_X11:
             if check_chinese():
-                CmdCtl.run_cmd(
-                    f"xdotool type --delay {delay_time} '{message}'", timeout=60
-                )
+                CmdCtl.run_cmd(f"xdotool type --delay {delay_time} '{message}'", timeout=60)
             else:
                 pyautogui.typewrite(message=str(message), interval=interval)
         # wayland上
         else:
             if check_chinese():
                 # 复制
                 if os.popen("ps -aux |  grep wayland_autotool | grep -v grep").read():
@@ -309,14 +288,15 @@
                 if wayland_shift:
                     _hk.insert(1, "shift")
                 cls.hot_key(*_hk)
             else:
                 for key in message:
                     if _ydotool:
                         from src import ydotool
+
                         ydotool.press(key)
                     else:
                         pyautogui.press(key, interval=interval)
 
     @classmethod
     def press_key(cls, key: str, interval=0.0, _ydotool: bool = False):
         """
@@ -324,14 +304,15 @@
         :param key: 键盘按键
         :param interval:
         :return:
         """
         logger.debug(f"点击键盘上指定的按键<{key}>, 间隔<{interval}>")
         if _ydotool:
             from src import ydotool
+
             ydotool.press(key)
         else:
             pyautogui.press(key, interval=interval)
 
     @classmethod
     def press_key_down(cls, key: str):
         """
```

### Comparing `youqu-2.5.3/youqu/src/ocr_utils.py` & `youqu-2.5.4/youqu/src/ocr_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=E0401,C0413,R0903,W0707,W0611
 try:
     import cv2 as cv
 
     GET_OPENCV_FORM_RPC = False
```

### Comparing `youqu-2.5.3/youqu/src/pinyin.py` & `youqu-2.5.4/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/read_csv.py` & `youqu-2.5.4/youqu/src/read_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=C0301,W1514,R1721,R1710,W1514,C0103,R1710
 import os
 import csv
 
-from src  import logger
+from src import logger
 
 
 class ReadCsv:
     """
     读取 csv 文件
     """
```

### Comparing `youqu-2.5.3/youqu/src/recording_screen.py` & `youqu-2.5.4/youqu/src/recording_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 import time
 import subprocess as sp
 import os
 import errno
 
 from src.mouse_key import MouseKey
 from setting.globalconfig import GlobalConfig
-from src  import logger
+from src import logger
 from contextlib import contextmanager
 
 
 def recording_screen(name):
     """
      录制视频
     :param name: 视频名称
     :return:
     """
-    record_path = f'{GlobalConfig.ROOT_DIR}/report/record/{time.strftime("%Y-%m-%d", time.localtime())}/'
+    record_path = (
+        f'{GlobalConfig.ROOT_DIR}/report/record/{time.strftime("%Y-%m-%d", time.localtime())}/'
+    )
     if not os.path.exists(record_path):
         os.makedirs(record_path)
     width, height = MouseKey.screen_size()
     cmd, paths = _create_ffmpeg_cmd(
         width,
         height,
         record_path,
@@ -36,18 +38,15 @@
 
     for path in paths:
         with suppress(OSError, errnos=(errno.ENOENT, errno.ENAMETOOLONG)):
             os.remove(path)
         logger.info(f"录屏路径存放  {path}")
 
     with open(os.devnull, "w", encoding="utf-8") as dev_null:
-        with sp.Popen(
-            cmd, stdin=sp.PIPE, stdout=dev_null, stderr=dev_null, close_fds=True
-        ) as proc:
-
+        with sp.Popen(cmd, stdin=sp.PIPE, stdout=dev_null, stderr=dev_null, close_fds=True) as proc:
             time.sleep(0.5)
             if proc.poll() is not None:
                 raise RuntimeError("ffmpeg did not start")
 
             try:
                 yield paths[0]
             finally:
```

### Comparing `youqu-2.5.3/youqu/src/requestx.py` & `youqu-2.5.4/youqu/src/requestx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/shortcut.py` & `youqu-2.5.4/youqu/src/shortcut.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/singleton.py` & `youqu-2.5.4/youqu/src/singleton.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/sleepx.py` & `youqu-2.5.4/youqu/src/sleepx.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 from time import sleep as slp
 from setting.globalconfig import GlobalConfig
-from src  import logger
+from src import logger
 
 
 def sleep(second: [float, int]):
     """
      重写sleep方法
      1、增加等待时间的日志
      2、根据不同CPU架构进行放大
     :param second: 等待时间
     :return:
     """
     sys_arch = GlobalConfig.SYS_ARCH
     multiple = float(GlobalConfig.slp_cfg.get(sys_arch))
     mult_sec = second * multiple
-    logger.debug(
-        f"sleep {second} s [{sys_arch} * {multiple} = {mult_sec}]"
-    )
+    logger.debug(f"sleep {second} s [{sys_arch} * {multiple} = {mult_sec}]")
     slp(mult_sec)
```

### Comparing `youqu-2.5.3/youqu/src/startapp.py` & `youqu-2.5.4/youqu/src/startapp.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from configparser import ConfigParser
 
 from setting.globalconfig import GlobalConfig
 from setting.globalconfig import FixedCsvTitle
 
 
 class StartApp:
-    def __init__(self, app_name:str):
+    def __init__(self, app_name: str):
         self.app_name = app_name.strip("/")
 
     def copy_template_to_apps(self):
         """copy_template_to_apps"""
         app_name_path = f"{GlobalConfig.APPS_PATH}/{self.app_name}"
         if os.path.exists(app_name_path) and os.listdir(app_name_path):
             if input(
@@ -28,17 +28,15 @@
             ) in ("y", "Y"):
                 os.system(f"rm -rf {app_name_path}/*")
             else:
                 exit(0)
         if not os.path.exists(app_name_path):
             os.makedirs(app_name_path)
         os.system(
-            "cp -r "
-            f"{GlobalConfig.SETTING_PATH}/template/app_template/* "
-            f"{app_name_path}/"
+            "cp -r " f"{GlobalConfig.SETTING_PATH}/template/app_template/* " f"{app_name_path}/"
         )
         os.system(
             "cp -r "
             f"{GlobalConfig.SETTING_PATH}/template/app_template/.gitignore-tpl "
             f"{app_name_path}/"
         )
 
@@ -69,38 +67,34 @@
                         if "##" in code:
                             code = code.replace("##", "")
                         if "${APP_NAME}" in code:
                             code = re.sub(r"\${APP_NAME}", self.app_name, code)
                         if "${app_name}" in code:
                             code = re.sub(r"\${app_name}", app_name, code)
                         if "${APP-NAME}" in code:
-                            code = re.sub(
-                                r"\${APP-NAME}", app_name.replace("_", "-"), code
-                            )
+                            code = re.sub(r"\${APP-NAME}", app_name.replace("_", "-"), code)
                         if "${AppName}" in code:
-                            code = re.sub(
-                                r"\${AppName}", app_name.title().replace("_", ""), code
-                            )
+                            code = re.sub(r"\${AppName}", app_name.title().replace("_", ""), code)
                         if "${USER}" in code:
                             code = re.sub(r"\${USER}", GlobalConfig.USERNAME, code)
                         if "${DATE}" in code:
                             code = re.sub(r"\${DATE}", strftime("%Y/%m/%d"), code)
                         if "${TIME}" in code:
                             code = re.sub(r"\${TIME}", strftime("%H:%M:%S"), code)
                         if "${FIXEDCSVTITLE}" in code:
                             code = re.sub(
-                                r"\${FIXEDCSVTITLE}", ",".join([i.value for i in FixedCsvTitle]), code
+                                r"\${FIXEDCSVTITLE}",
+                                ",".join([i.value for i in FixedCsvTitle]),
+                                code,
                             )
                         new_codes.append(code)
                     with open(f"{root}/{file}", "w") as f:
                         f.writelines([i for i in new_codes])
 
                 if file == "control":
                     conf = ConfigParser()
                     conf.read(f"{root}/{file}")
-                    conf.set(
-                        "Depends", "autotest-basic-frame", GlobalConfig.current_tag
-                    )
+                    conf.set("Depends", "autotest-basic-frame", GlobalConfig.current_tag)
                     with open(f"{root}/{file}", "w", encoding="utf-8") as f:
                         conf.write(f)
 
         print(f"{self.app_name} 创建成功,请查看 {GlobalConfig.APPS_PATH}/{self.app_name}")
```

### Comparing `youqu-2.5.3/youqu/src/startproject.py` & `youqu-2.5.4/youqu/src/startproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,12 +34,14 @@
                 os.system(f"rm -rf {root}/{d}")
     conf = ConfigParser()
     try:
         conf.read(f"{root_dir}/CURRENT")
         youqu_version = conf.get("current", "tag")
     except NoSectionError:
         youqu_version = None
-    print(f"The project: [\033[0;32m{project_name}\033[0m],has been created by youqu{f'-{youqu_version}' if youqu_version else ''}")
+    print(
+        f"The project: [\033[0;32m{project_name}\033[0m],has been created by youqu{f'-{youqu_version}' if youqu_version else ''}"
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `youqu-2.5.3/youqu/src/video_utils.py` & `youqu-2.5.4/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/wayland_wininfo.py` & `youqu-2.5.4/youqu/src/wayland_wininfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 
 from platform import machine
 import ctypes
 
 
 class Geometry(ctypes.Structure):
     """sub structure"""
+
     _fields_ = [
         ("x", ctypes.c_int),
         ("y", ctypes.c_int),
         ("width", ctypes.c_int),
         ("height", ctypes.c_int),
     ]
 
 
 class WindowState(ctypes.Structure):
     """window structure"""
+
     _fields_ = [
         ("pid", ctypes.c_int),  # 4
         ("windowId", ctypes.c_int),  # 4
         ("resourceName", ctypes.c_char * 256),  # 256
         ("Geometry", Geometry),  # 16
         ("isMinimized", ctypes.c_bool),  # 4
         ("isFullScreen", ctypes.c_bool),
@@ -53,14 +55,15 @@
         ("alloc", ctypes.c_size_t),
         ("data", ctypes.POINTER(WindowState)),
     ]
 
 
 class WindowStructure(ctypes.Structure):
     """window structure"""
+
     _fields_ = [
         ("pid", ctypes.c_int),
         ("windowId", ctypes.c_int),
         ("resourceName", ctypes.c_char * 256),
         ("Geometry", Geometry),
         ("isMinimized", ctypes.c_bool),
         ("isFullScreen", ctypes.c_bool),
@@ -91,20 +94,15 @@
         ws = self.library.GetWindowState(wid)
         window_info = ws.contents.Geometry
         resourceName = ws.contents.resourceName.decode("utf-8")
         if not resourceName:
             resourceName = os.popen(f"cat /proc/{ws.contents.pid}/cmdline").read().strip("\x00")
         return {
             "name": resourceName,
-            "wininfo": (
-                window_info.x,
-                window_info.y,
-                window_info.width,
-                window_info.height
-            ),
+            "wininfo": (window_info.x, window_info.y, window_info.width, window_info.height),
         }
 
     def window_info(self):
         """窗口信息"""
         self.library.GetAllWindowStatesList.restype = ctypes.c_int
         _e = None
         for _ in range(3):
@@ -118,21 +116,23 @@
         else:
             raise ValueError(_e)
         res = {}
         for i in range(int(range_index)):
             window_info = windows_pointer[i]
             resource_name = window_info.resourceName.decode("utf-8")
             if not resource_name:
-                resource_name = os.popen(f"cat /proc/{window_info.pid}/cmdline").read().strip("\x00")
+                resource_name = (
+                    os.popen(f"cat /proc/{window_info.pid}/cmdline").read().strip("\x00")
+                )
             _info = {
                 "location": (
                     window_info.Geometry.x,
                     window_info.Geometry.y,
                     window_info.Geometry.width,
-                    window_info.Geometry.height
+                    window_info.Geometry.height,
                 ),
                 "pid": window_info.pid,
                 "window_id": window_info.windowId,
                 "uuid": window_info.uuid.decode("utf-8"),
                 "is_minimized": window_info.isMinimized,
                 "is_full_screen": window_info.isFullScreen,
                 "is_active": window_info.isActive,
@@ -143,14 +143,14 @@
                 if isinstance(res.get(resource_name), dict):
                     res[resource_name] = [res.get(resource_name), _info]
                 elif isinstance(res.get(resource_name), list):
                     res[resource_name].append(_info)
         return res
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     wwininfo = WaylandWindowInfo()
     wwininfo.library.InitDtkWmDisplay()
     for i in range(100):
         print(wwininfo.window_info())
         sleep(1)
     wwininfo.library.DestoryDtkWmDisplay()
```

### Comparing `youqu-2.5.3/youqu/src/webui.py` & `youqu-2.5.4/youqu/src/webui.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,33 +17,31 @@
     from playwright.sync_api import PageAssertions
     from playwright.sync_api import APIResponseAssertions
 except ImportError:
     print("Please install playwright")
 
 
 class WebUI:
-
     def __init__(self, page: Page):
         self.page = page
 
     def goto(self, url):
         self.page.goto(url)
 
     def input_text(self, element, text):
         self.page.fill(element, text)
 
     def click_element(self, element):
         self.page.click(element)
 
 
 class WebAssert:
-
     @staticmethod
     def assert_locator(
-            locator: Union[Page, Locator, APIResponse]
+        locator: Union[Page, Locator, APIResponse],
     ) -> Union[PageAssertions, LocatorAssertions, APIResponseAssertions]:
         return _expect(locator)
 
 
 @contextmanager
 def debug_page():
     driver = sync_playwright().start()
@@ -52,16 +50,15 @@
         executable_path=GlobalConfig.EXECUTABLE_PATH,
         ignore_https_errors=True,
         no_viewport=True,
         slow_mo=500,
         headless=False,
         bypass_csp=True,
         args=[
-            '--disable-blink-features=AutomationControlled',
-            '--start-maximized',
+            "--disable-blink-features=AutomationControlled",
+            "--start-maximized",
         ],
-
     )
     _page = browser.pages[0]
     yield _page
     browser.close()
     driver.stop()
```

### Comparing `youqu-2.5.3/youqu/src/ydotool.py` & `youqu-2.5.4/youqu/src/ydotool.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,137 +10,137 @@
 import os
 from time import sleep
 
 from setting import conf
 from src import CmdCtl
 
 KEY_NAMES = {
-    ' ': 57,
-    '\'': 40,
-    '*': 55,
-    '+': 78,
-    ',': 51,
-    '-': 12,
-    '.': 52,
-    '/': 53,
-    '0': 11,
-    '1': 2,
-    '2': 3,
-    '4': 5,
-    '5': 6,
-    '3': 4,
-    '6': 7,
-    '7': 8,
-    '8': 9,
-    '9': 10,
-    ';': 39,
-    '=': 13,
-    '[': 26,
-    '\\': 43,
-    ']': 27,
-    '`': 41,
-    'a': 30,
-    'b': 48,
-    'c': 46,
-    'd': 32,
-    'e': 18,
-    'f': 33,
-    'g': 34,
-    'h': 35,
-    'i': 23,
-    'j': 36,
-    'k': 37,
-    'l': 38,
-    'm': 50,
-    'n': 49,
-    'o': 24,
-    'p': 25,
-    'q': 16,
-    'r': 19,
-    's': 31,
-    't': 20,
-    'u': 22,
-    'v': 47,
-    'w': 17,
-    'x': 45,
-    'y': 21,
-    'z': 44,
-    'add': 78,
-    'alt': 56,
-    'altleft': 56,
-    'altright': 100,
-    'backspace': 14,
-    'capslock': 58,
-    'ctrl': 29,
-    'ctrlleft': 29,
-    'ctrlright': 97,
-    'del': 111,
-    'delete': 111,
-    'down': 108,
-    'end': 107,
-    'enter': 28,
-    'esc': 1,
-    'escape': 1,
-    'f1': 59,
-    'f10': 68,
-    'f11': 87,
-    'f12': 88,
-    'f13': 183,
-    'f14': 184,
-    'f15': 185,
-    'f16': 186,
-    'f17': 187,
-    'f18': 188,
-    'f19': 189,
-    'f2': 60,
-    'f20': 190,
-    'f21': 191,
-    'f22': 192,
-    'f23': 193,
-    'f24': 194,
-    'f3': 61,
-    'f4': 62,
-    'f5': 63,
-    'f6': 64,
-    'f7': 65,
-    'f8': 66,
-    'f9': 67,
-    'home': 172,
-    'insert': 110,
-    'left': 105,
-    'num0': 82,
-    'num1': 79,
-    'num2': 80,
-    'num3': 81,
-    'num4': 75,
-    'num5': 76,
-    'num6': 77,
-    'num7': 71,
-    'num8': 72,
-    'num9': 73,
-    'numlock': 69,
-    'pagedown': 109,
-    'pageup': 104,
-    'pgdn': 109,
-    'pgup': 104,
-    'print': 210,
-    'right': 106,
-    'scrolllock': 70,
-    'printscreen': 210,
-    'shift': 42,
-    'shiftleft': 42,
-    'shiftright': 54,
-    'space': 57,
-    'tab': 15,
-    'up': 103,
-    'volumedown': 114,
-    'volumeup': 115,
-    'win': 125,
-    'winleft': 125,
-    'winright': 126,
+    " ": 57,
+    "'": 40,
+    "*": 55,
+    "+": 78,
+    ",": 51,
+    "-": 12,
+    ".": 52,
+    "/": 53,
+    "0": 11,
+    "1": 2,
+    "2": 3,
+    "4": 5,
+    "5": 6,
+    "3": 4,
+    "6": 7,
+    "7": 8,
+    "8": 9,
+    "9": 10,
+    ";": 39,
+    "=": 13,
+    "[": 26,
+    "\\": 43,
+    "]": 27,
+    "`": 41,
+    "a": 30,
+    "b": 48,
+    "c": 46,
+    "d": 32,
+    "e": 18,
+    "f": 33,
+    "g": 34,
+    "h": 35,
+    "i": 23,
+    "j": 36,
+    "k": 37,
+    "l": 38,
+    "m": 50,
+    "n": 49,
+    "o": 24,
+    "p": 25,
+    "q": 16,
+    "r": 19,
+    "s": 31,
+    "t": 20,
+    "u": 22,
+    "v": 47,
+    "w": 17,
+    "x": 45,
+    "y": 21,
+    "z": 44,
+    "add": 78,
+    "alt": 56,
+    "altleft": 56,
+    "altright": 100,
+    "backspace": 14,
+    "capslock": 58,
+    "ctrl": 29,
+    "ctrlleft": 29,
+    "ctrlright": 97,
+    "del": 111,
+    "delete": 111,
+    "down": 108,
+    "end": 107,
+    "enter": 28,
+    "esc": 1,
+    "escape": 1,
+    "f1": 59,
+    "f10": 68,
+    "f11": 87,
+    "f12": 88,
+    "f13": 183,
+    "f14": 184,
+    "f15": 185,
+    "f16": 186,
+    "f17": 187,
+    "f18": 188,
+    "f19": 189,
+    "f2": 60,
+    "f20": 190,
+    "f21": 191,
+    "f22": 192,
+    "f23": 193,
+    "f24": 194,
+    "f3": 61,
+    "f4": 62,
+    "f5": 63,
+    "f6": 64,
+    "f7": 65,
+    "f8": 66,
+    "f9": 67,
+    "home": 172,
+    "insert": 110,
+    "left": 105,
+    "num0": 82,
+    "num1": 79,
+    "num2": 80,
+    "num3": 81,
+    "num4": 75,
+    "num5": 76,
+    "num6": 77,
+    "num7": 71,
+    "num8": 72,
+    "num9": 73,
+    "numlock": 69,
+    "pagedown": 109,
+    "pageup": 104,
+    "pgdn": 109,
+    "pgup": 104,
+    "print": 210,
+    "right": 106,
+    "scrolllock": 70,
+    "printscreen": 210,
+    "shift": 42,
+    "shiftleft": 42,
+    "shiftright": 54,
+    "space": 57,
+    "tab": 15,
+    "up": 103,
+    "volumedown": 114,
+    "volumeup": 115,
+    "win": 125,
+    "winleft": 125,
+    "winright": 126,
     ")": 11,
     "!": 2,
     "@": 3,
     "#": 4,
     "$": 5,
     "%": 6,
     "^": 7,
@@ -148,72 +148,73 @@
     "(": 10,
     "_": 12,
     "~": 41,
     "{": 26,
     "}": 27,
     "|": 43,
     ":": 39,
-    "\"": 40,
+    '"': 40,
     "<": 51,
     ">": 52,
     "?": 53,
-    'A': 30,
-    'B': 48,
-    'C': 46,
-    'D': 32,
-    'E': 18,
-    'F': 33,
-    'G': 34,
-    'H': 35,
-    'I': 23,
-    'J': 36,
-    'K': 37,
-    'L': 38,
-    'M': 50,
-    'N': 49,
-    'O': 24,
-    'P': 25,
-    'Q': 16,
-    'R': 19,
-    'S': 31,
-    'T': 20,
-    'U': 22,
-    'V': 47,
-    'W': 17,
-    'X': 45,
-    'Y': 21,
-    'Z': 44,
-    '。': 52
+    "A": 30,
+    "B": 48,
+    "C": 46,
+    "D": 32,
+    "E": 18,
+    "F": 33,
+    "G": 34,
+    "H": 35,
+    "I": 23,
+    "J": 36,
+    "K": 37,
+    "L": 38,
+    "M": 50,
+    "N": 49,
+    "O": 24,
+    "P": 25,
+    "Q": 16,
+    "R": 19,
+    "S": 31,
+    "T": 20,
+    "U": 22,
+    "V": 47,
+    "W": 17,
+    "X": 45,
+    "Y": 21,
+    "Z": 44,
+    "。": 52,
 }
 
 
 def context_manager(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         tool_status = os.popen("ps aux | grep ydotoold | grep -v grep").read()
         if not tool_status:
             os.system(
                 f'echo "{conf.PASSWORD}" | sudo -S apt update;'
                 f'echo "{conf.PASSWORD}" | sudo -S apt install -y scdoc;'
                 f"cd {conf.ROOT_DIR}/src/depends/ydotool/;"
-                'mkdir build;'
-                'cd build;'
-                'cmake ..;'
+                "mkdir build;"
+                "cd build;"
+                "cmake ..;"
                 'make -j "$(nproc)";'
                 f'echo "{conf.PASSWORD}" | sudo -S make install'
             )
             sleep(1)
             res = os.popen(
                 f'echo "{conf.PASSWORD}" | sudo -S -b '
                 'ydotoold --socket-path="$HOME/.ydotool_socket" --socket-own="$(id -u):$(id -g)"'
             )
             if "未找到命令" in res:
                 raise EnvironmentError("ydotool not installed")
             sleep(2)
         return func(*args, **kwargs)
+
     return wrapper
 
 
 @context_manager
 def _popen(cmd):
     return CmdCtl.run_cmd(cmd, out_debug_flag=False, command_log=False)
```

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/cli.py` & `youqu-2.5.4/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/colors.py` & `youqu-2.5.4/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/consts.py` & `youqu-2.5.4/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/core.py` & `youqu-2.5.4/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.5.4/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/colorama/ansi.py` & `youqu-2.5.4/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.5.4/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/colorama/initialise.py` & `youqu-2.5.4/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/colorama/win32.py` & `youqu-2.5.4/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/colorama/winterm.py` & `youqu-2.5.4/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/COPYING` & `youqu-2.5.4/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/__init__.py` & `youqu-2.5.4/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/config.py` & `youqu-2.5.4/youqu/src/depends/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/distro.py` & `youqu-2.5.4/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/dump.py` & `youqu-2.5.4/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/errors.py` & `youqu-2.5.4/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/i18n.py` & `youqu-2.5.4/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/logging.py` & `youqu-2.5.4/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/path.py` & `youqu-2.5.4/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/predicate.py` & `youqu-2.5.4/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/procedural.py` & `youqu-2.5.4/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.5.4/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.5.4/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/sessions.py` & `youqu-2.5.4/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/tc.py` & `youqu-2.5.4/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/tree.py` & `youqu-2.5.4/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/utils.py` & `youqu-2.5.4/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/version.py` & `youqu-2.5.4/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.5.4/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.5.4/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.5.4/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.5.4/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.5.4/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.5.4/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/sniff` & `youqu-2.5.4/youqu/src/depends/sniff/sniff`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/sniff.ui` & `youqu-2.5.4/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.5.4/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.5.4/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.5.4/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.5.4/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/LICENSE` & `youqu-2.5.4/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/git/clone.py` & `youqu-2.5.4/youqu/src/git/clone.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,39 +13,44 @@
 
 
 def sslclone(
     url: str = None,
     user: str = None,
     password: str = None,
     branch: str = None,
+    path_to: str = None,
     depth: [str, int] = None,
     **kwargs,
 ):
     branch = branch or conf.BRANCH
     depth = depth or conf.DEPTH
+    if path_to is None:
+        path_to = "apps"
     git_config()
     clone_cmd = (
         f"cd {conf.ROOT_DIR}/src/utils && "
-        f"bash sslclone.sh {conf.APPS_PATH} "
+        f"bash sslclone.sh {conf.ROOT_DIR}/{path_to} "
         f"{url or conf.GIT_URL} "
         f"{user or conf.GTI_USER} {password or conf.GIT_PASSWORD} "
         f"{branch or ''} {depth or ''}"
     )
     print(clone_cmd)
     os.system(clone_cmd)
     # relax
     sleep(2)
 
 
-def clone(url: str = None, branch: str = "", depth: [str, int] = "", **kwargs):
+def clone(url: str = None, branch: str = "", path_to: str = None, depth: [str, int] = "", **kwargs):
     branch = branch or conf.BRANCH
     depth = depth or conf.DEPTH
+    if path_to is None:
+        path_to = "apps"
     git_config()
     clone_cmd = (
-        f"cd {conf.APPS_PATH} && git clone "
+        f"cd {conf.ROOT_DIR}/{path_to} && git clone "
         f"{url or conf.GIT_URL} "
         f"{f'-b {branch}' if branch else ''} {f'--depth {depth}' if depth else ''}"
     )
     print(clone_cmd)
     os.system(clone_cmd)
     # relax
     sleep(2)
```

### Comparing `youqu-2.5.3/youqu/src/git/code_statistics.py` & `youqu-2.5.4/youqu/src/git/code_statistics.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/git/commit.py` & `youqu-2.5.4/youqu/src/git/commit.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/plugins/allure_report_extend.py` & `youqu-2.5.4/youqu/src/plugins/allure_report_extend.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,65 +2,64 @@
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114,C0103,R0903
 import os
 from tkinter import Tk
+from functools import partial
 
 from setting.globalconfig import GlobalConfig
-from src.dbus_utils import DbusUtils
+from src.rtk._base import collect_result
 
 
 def wf(f, t):
     f.write(t.encode("unicode_escape").decode() + "\n")
 
 
 class AllureReportExtend:
-    """AllureReportExtend"""
-
     @staticmethod
-    def environment_info(session):
-        """写入环境变量"""
+    def environment_info(session, execute):
         try:
             allure_path = session.config.option.allure_report_dir
         except TypeError:
             return
         if not allure_path:
             return
         allure_fspath_path = os.path.join(
-            session.config.invocation_dir,
-            allure_path,
-            "environment.properties"
+            session.config.invocation_dir, allure_path, "environment.properties"
         )
         with open(allure_fspath_path, "w+", encoding="utf-8") as _f:
-            wf(_f, f"网络地址={GlobalConfig.USERNAME}@{GlobalConfig.HOST_IP}")
-            wf(_f, f"系统信息={GlobalConfig.PRODUCT_INFO}")
-            wf(_f, f"镜像版本={GlobalConfig.VERSION}")
-            wf(_f, f"目录={GlobalConfig.ROOT_DIR}")
+            w = partial(wf, _f)
 
-            screen = Tk()
-            wf(_f, f"分辨率={screen.winfo_screenwidth()}x{screen.winfo_screenheight()}")
+            py_case_info = ""
+            if execute:
+                total, failed, passed, skiped, _ = collect_result(execute)
+                py_case_info = f"{total}/{passed}/{failed}/{skiped}"
+
+            w(f"PMS用例维度(总数/通过/失败/跳过)={py_case_info}")
+            w(f"网络地址={GlobalConfig.USERNAME}@{GlobalConfig.HOST_IP}")
+            w(f"工作目录={GlobalConfig.ROOT_DIR}")
+            w(f"镜像版本={GlobalConfig.VERSION}")
 
-            _display = GlobalConfig.DisplayServer.wayland if GlobalConfig.IS_WAYLAND else GlobalConfig.DisplayServer.x11
-            wf(_f, f"显示协议={_display.title()}")
+            screen = Tk()
+            w(f"分辨率={screen.winfo_screenwidth()}x{screen.winfo_screenheight()}")
 
-            cpu_info = os.popen("cat /proc/cpuinfo | grep name | cut -f2 -d: | uniq -c").read().replace(" ", "")
-            if not cpu_info:
-                cpu_info = os.popen("cat /proc/cpuinfo | grep Hardware").read()
-            wf(_f, f"CPU信息={cpu_info}")
+            w(f"显示协议={GlobalConfig.DISPLAY_SERVER.title()}")
 
-            mem_info = os.popen("cat /proc/meminfo | grep MemTotal").read()
-            wf(_f, f"内存信息={mem_info}")
+            cpu_info = (
+                os.popen(
+                    f"echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode -s  processor-version"
+                )
+                .readlines()[0]
+                .strip("\n")
+            )
+            w(f"CPU信息={cpu_info}")
+
+            mem_info = os.popen(
+                f'''echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode|grep -A16 'Memory Device' | grep -v "Memory Device Mapped Address" | grep "Range Size"'''
+            ).readlines()
+            MEM_TOTAL = sum([int(i.split(":")[1].rstrip(" GB\n").strip()) for i in mem_info])
+            w(f"内存信息={MEM_TOTAL}G")
 
             os_info = os.popen("uname -a").read()
-            wf(_f, f"内核信息={os_info}")
-
-            try:
-                language_code = DbusUtils(
-                    "com.deepin.daemon.LangSelector",
-                    "/com/deepin/daemon/LangSelector",
-                    "com.deepin.daemon.LangSelector",
-                ).get_session_properties_value("CurrentLocale")
-                wf(_f, f"系统语言={GlobalConfig.LANGUAGE_INI.get(language_code, default=language_code)}")
-            except Exception:
-                pass
+            w(f"内核信息={os_info}")
```

### Comparing `youqu-2.5.3/youqu/src/plugins/emoji_hooks.py` & `youqu-2.5.4/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/pms/_base.py` & `youqu-2.5.4/youqu/src/pms/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,30 +42,30 @@
     """
     修改数据并进行编码解码操作，以完成u码转中文
     :param in_str: 字符串
     :return:/
     """
     local_in_str_replace = (
         in_str.replace(r"\"", '"')
-            .replace(r"\/", "/")
-            .replace(r"\\u", r"\u")
-            .replace(r"\\n", "")
-            .replace(r"\\r", "")
+        .replace(r"\/", "/")
+        .replace(r"\\u", r"\u")
+        .replace(r"\\n", "")
+        .replace(r"\\r", "")
     )
     if isinstance(local_in_str_replace, bytes):
         local_temp = str(local_in_str_replace, encoding="utf-8")
         local_out = local_temp.encode("utf-8").decode("unicode_escape")
     else:
         local_out = local_in_str_replace.encode("utf-8").decode("unicode_escape")
     return (
         local_out.replace('"data":"{', '"data":{')
-            .replace('","md5"', ',"md5"')
-            .replace(":null", ':"null"')
-            .replace(":true", ':"true"')
-            .replace(":false", ':"false"')
+        .replace('","md5"', ',"md5"')
+        .replace(":null", ':"null"')
+        .replace(":true", ':"true"')
+        .replace(":false", ':"false"')
     )
 
 
 def write_case_result(item, report):
     """写用例执行的结果"""
     case_result_tpl = {
         "at_case_id": None,
@@ -110,21 +110,24 @@
     abs_json_file_path = f"{case_res_path}/{json_file_name}"
     if exists(abs_json_file_path):
         with open(abs_json_file_path, "r", encoding="utf-8") as _f:
             case_res_from_json = json.load(_f)
 
         if item.execution_count >= 2:
             if (
-                    case_res_from_json.get("result") == "fail"
-                    and case_result_tpl["result"] == "pass"
-                    and case_res_from_json.get("item") == case_result_tpl["item"]
+                case_res_from_json.get("result") == "fail"
+                and case_result_tpl["result"] == "pass"
+                and case_res_from_json.get("item") == case_result_tpl["item"]
             ):
                 case_result_tpl["result"] = "cover-pass"
                 with open(abs_json_file_path, "w+", encoding="utf-8") as _f:
                     _f.write(json.dumps(case_result_tpl, indent=2, ensure_ascii=False))
         else:
-            if case_res_from_json.get("result") in ("pass", "cover-pass") and case_result_tpl["result"] == "fail":
+            if (
+                case_res_from_json.get("result") in ("pass", "cover-pass")
+                and case_result_tpl["result"] == "fail"
+            ):
                 with open(abs_json_file_path, "w+", encoding="utf-8") as _f:
                     _f.write(json.dumps(case_result_tpl, indent=2, ensure_ascii=False))
     else:
         with open(abs_json_file_path, "w+", encoding="utf-8") as _f:
             _f.write(json.dumps(case_result_tpl, indent=2, ensure_ascii=False))
```

### Comparing `youqu-2.5.3/youqu/src/pms/csv2pms.py` & `youqu-2.5.4/youqu/src/pms/csv2pms.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,47 +2,41 @@
 # _*_ coding:utf-8 _*_
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 # SPDX-License-Identifier: GPL-2.0-only
 import json
 import os
+
 # from concurrent.futures import ALL_COMPLETED
 # from concurrent.futures import ThreadPoolExecutor
 # from concurrent.futures import wait
 from time import sleep
 from urllib.parse import urlencode
 
 from setting import conf
 from setting.globalconfig import FixedCsvTitle
 from src.pms._base import _Base
 from src.rtk._base import transform_app_name
 
 __all__ = []
 
+
 class Csv2Pms(_Base):
     __author__ = "mikigo<huangmingqiang@uniontech.com>"
 
     config_error_log = "请检查您传递的 '命令行参数' 或 setting/globalconfig.ini 里的配置项"
 
-    def __init__(
-            self,
-            app_name: str = None,
-            user: str = None,
-            password: str = None,
-            csv_name=None
-    ):
+    def __init__(self, app_name: str = None, user: str = None, password: str = None, csv_name=None):
         super().__init__(user=user, password=password)
         self.username = user
         self.password = user
         self.base_url = "https://pms.uniontech.com"
         self.walk_dir = (
-            f"{conf.APPS_PATH}/{transform_app_name(app_name)}"
-            if app_name
-            else conf.APPS_PATH
+            f"{conf.APPS_PATH}/{transform_app_name(app_name)}" if app_name else conf.APPS_PATH
         )
         self.csv_name = csv_name or conf.CSV_NAME_TO_PMS
 
         if not self.csv_name:
             raise EnvironmentError(self.config_error_log)
 
     def get_csv_info(self):
@@ -70,29 +64,34 @@
         taglines = [txt.strip().split(",") for txt in txt_list[1:]]
         return csv_head_index_map, taglines
 
     def post_to_pms(self):
         csv_head_index_map, taglines = self.get_csv_info()
 
         def csv_map(x):
-            return csv_head_index_map.get(x).get('head_index')
+            return csv_head_index_map.get(x).get("head_index")
 
         def push(value, index):
             sleep(1)
             case_id = value[csv_map(FixedCsvTitle.pms_case_id.name)]
             case_url = f"{self.base_url}/testcase-view-{case_id}.json"
             case_res = json.loads(self.rx.open_url(case_url, timeout=10))
             case_data = json.loads(case_res.get("data"))
             case_title = case_data.get("title")
-            rel_case_title = case_title.split(case_id)[-1].rstrip(f"{case_data.get('libName')}").strip(" - ").strip(" ")
+            rel_case_title = (
+                case_title.split(case_id)[-1]
+                .rstrip(f"{case_data.get('libName')}")
+                .strip(" - ")
+                .strip(" ")
+            )
 
             edit_url = f"{self.base_url}/testcase-edit-{case_id}.html"
             data = {
-                'title': rel_case_title,
-                'isAutomation': '是',
+                "title": rel_case_title,
+                "isAutomation": "是",
             }
             try:
                 if value[csv_map(FixedCsvTitle.device_type.name)] == "PPL":
                     data["deviceType"] = "PPL(外设)"
             except AttributeError:
                 pass
             try:
@@ -107,19 +106,15 @@
                 pass
             try:
                 if value[csv_map(FixedCsvTitle.online_obj.name)] == "CICD":
                     data["lineCD"] = "是"
             except AttributeError:
                 pass
             bytes_data = urlencode(data).encode("utf-8")
-            res = self.rx.session.open(
-                fullurl=edit_url,
-                data=bytes_data,
-                timeout=10
-            )
+            res = self.rx.session.open(fullurl=edit_url, data=bytes_data, timeout=10)
             print(f"({index}) {case_id} {data} {res.status}")
 
         # tasks = []
         # executor = ThreadPoolExecutor()
         for index, value in enumerate(taglines):
             push(value, index)
             # t = executor.submit(push, value, index)
```

### Comparing `youqu-2.5.3/youqu/src/pms/pms2csv.py` & `youqu-2.5.4/youqu/src/pms/pms2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
             if app_name
             else GlobalConfig.APPS_PATH
         )
 
         conf = ConfigParser()
         conf.read(GlobalConfig.GLOBAL_CONFIG_FILE_PATH)
         ini_csv_names = conf.options("pmsctl-pms_link_csv")
-        ini_csv_pms_map = GetCfg(
-            GlobalConfig.GLOBAL_CONFIG_FILE_PATH, "pmsctl-pms_link_csv"
-        )
+        ini_csv_pms_map = GetCfg(GlobalConfig.GLOBAL_CONFIG_FILE_PATH, "pmsctl-pms_link_csv")
         cli_csv_pms_map = {}
         cli_csv_names = []
         if pms_link_csv:
             _cli_csv_names = pms_link_csv.split("/")
             for i in _cli_csv_names:
                 pls = i.split(":")
                 if len(pls) != 2:
@@ -55,17 +53,15 @@
 
         self.csv_names = cli_csv_names or ini_csv_names
         self.csv_link_cfg = cli_csv_pms_map or ini_csv_pms_map
 
         if not self.csv_names:
             raise ValueError(self.config_error_log)
 
-        self.pms_mark = GetCfg(
-            f"{GlobalConfig.SETTING_PATH}/pmsmark.ini", "pms-mark-to-csv-mark"
-        )
+        self.pms_mark = GetCfg(f"{GlobalConfig.SETTING_PATH}/pmsmark.ini", "pms-mark-to-csv-mark")
 
     def get_data_from_pms(self, app_case_id):
         """获取pms上数据"""
         if not app_case_id:
             raise ValueError(self.config_error_log)
         case_url = (
             f"https://pms.uniontech.com/{GlobalConfig.CASE_FROM}-browse-"
@@ -93,37 +89,32 @@
                 "case_level": f"L{case_level}",
                 "case_type": case_type,
                 "case_from": "BUG" if case_from == "是" else "",
                 "device_type": device_type.split("(")[0]
                 if device_type and device_type != "null"
                 else "",
                 "online_obj": "CICD" if online_obj == "是" else "",
-                "skip_reason": "skip-下线CD" if online_obj == "否" else None
+                "skip_reason": "skip-下线CD" if online_obj == "否" else None,
             }
         if not res_data:
             logger.error(f"未从pms获取到数据, {self.config_error_log}")
             raise ValueError
         return res_data
 
     def read_csv(self):
         """读取本地csv文件数据"""
         csv_path_dict = {}
         csv_bak_path = f"{GlobalConfig.REPORT_PATH}/pms2csv_back"
         if not os.path.exists(csv_bak_path):
             os.makedirs(csv_bak_path)
         for root, _, files in os.walk(self.walk_dir):
             for file in files:
-                if (
-                    file.endswith(".csv")
-                    and os.path.splitext(file)[0] in self.csv_names
-                ):
+                if file.endswith(".csv") and os.path.splitext(file)[0] in self.csv_names:
                     csv_path_dict[os.path.splitext(file)[0]] = f"{root}/{file}"
-                    os.system(
-                        f"cp {root}/{file} {csv_bak_path}/{GlobalConfig.TIME_STRING}_{file}"
-                    )
+                    os.system(f"cp {root}/{file} {csv_bak_path}/{GlobalConfig.TIME_STRING}_{file}")
         if not csv_path_dict:
             raise ValueError(f"{self.walk_dir} 目录下未找对应的到csv文件，{self.config_error_log}")
 
         res_tags = {}
         csv_heads_dict = {}
         for csv_name in csv_path_dict:
             with open(csv_path_dict.get(csv_name), "r", encoding="utf-8") as f:
@@ -188,39 +179,35 @@
                 online_obj_index = online_obj_name.get("head_index")
 
             skip_reason_name = csv_head_dict.get(FixedCsvTitle.skip_reason.name)
             if skip_reason_name:
                 skip_reason_index = skip_reason_name.get("head_index")
 
             new_csv_tags = []
-            new_csv_tags.append(
-                [i.get("head_name") for i in list(csv_head_dict.values())]
-            )
+            new_csv_tags.append([i.get("head_name") for i in list(csv_head_dict.values())])
             for csv_case_id in csv_tags_dict:
                 for pms_case_id in pms_tags_dict:
                     if pms_case_id == csv_case_id:
                         pms_tags = pms_tags_dict.get(pms_case_id)
                         case_level = pms_tags.get("case_level")
                         case_type = pms_tags.get("case_type")
                         case_from = pms_tags.get("case_from")
                         device_type = pms_tags.get("device_type")
                         online_obj = pms_tags.get("online_obj")
                         skip_reason = pms_tags.get("skip_reason")
                         flag = False
                         if (
                             pms_case_id_index
-                            and csv_tags_dict[csv_case_id][pms_case_id_index]
-                            != pms_case_id
+                            and csv_tags_dict[csv_case_id][pms_case_id_index] != pms_case_id
                         ):
                             csv_tags_dict[csv_case_id][pms_case_id_index] = pms_case_id
                             flag = True
                         if (
                             case_level_index
-                            and csv_tags_dict[csv_case_id][case_level_index]
-                            != case_level
+                            and csv_tags_dict[csv_case_id][case_level_index] != case_level
                         ):
                             csv_tags_dict[csv_case_id][case_level_index] = case_level
                             flag = True
                         if (
                             case_type_index
                             and csv_tags_dict[csv_case_id][case_type_index] != case_type
                         ):
@@ -230,40 +217,35 @@
                             case_from_index
                             and csv_tags_dict[csv_case_id][case_from_index] != case_from
                         ):
                             csv_tags_dict[csv_case_id][case_from_index] = case_from
                             flag = True
                         if (
                             device_type_index
-                            and csv_tags_dict[csv_case_id][device_type_index]
-                            != device_type
+                            and csv_tags_dict[csv_case_id][device_type_index] != device_type
                         ):
                             csv_tags_dict[csv_case_id][device_type_index] = device_type
                             flag = True
                         if (
                             online_obj_index
-                            and csv_tags_dict[csv_case_id][online_obj_index]
-                            != online_obj
+                            and csv_tags_dict[csv_case_id][online_obj_index] != online_obj
                         ):
                             csv_tags_dict[csv_case_id][online_obj_index] = online_obj
                             flag = True
                         if (
                             skip_reason_index
-                            and csv_tags_dict[csv_case_id][skip_reason_index]
-                            != skip_reason
+                            and csv_tags_dict[csv_case_id][skip_reason_index] != skip_reason
                         ):
                             if skip_reason:
                                 csv_tags_dict[csv_case_id][skip_reason_index] = skip_reason
                                 flag = True
 
                         new_tags = csv_tags_dict[csv_case_id]
                         if flag:
-                            logger.info(
-                                f"pms case id: {pms_case_id}, new tags:{new_tags}"
-                            )
+                            logger.info(f"pms case id: {pms_case_id}, new tags:{new_tags}")
                         new_csv_tags.append(new_tags)
                         break
                 else:
                     new_csv_tags.append(csv_tags_dict[csv_case_id])
 
             new_csv_file_tags[csv_path_dict.get(csv_name)] = new_csv_tags
         return new_csv_file_tags
@@ -271,13 +253,13 @@
     def write_new_csv(self):
         """写新的csv文件"""
         new_csv_file_tags = self.compare_pms_to_csv()
         for csv_file in new_csv_file_tags:
             new_csv_tags = new_csv_file_tags.get(csv_file)
             with open(csv_file, "w+", encoding="utf-8") as f:
                 for tags in new_csv_tags:
-                    f.write(",".join(tags) + "\n")
+                    f.write(",".join(["" if i is None else i for i in tags]) + "\n")
             logger.info(f"同步完成: {csv_file}")
 
 
 if __name__ == "__main__":
     Pms2Csv().write_new_csv()
```

### Comparing `youqu-2.5.3/youqu/src/pms/send2pms.py` & `youqu-2.5.4/youqu/src/pms/send2pms.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,15 @@
             "case": case_id,
             "version": "1",
             f"labels{steps_id}[]": "",
             f"files{steps_id}[]": "",
         }
         bytes_data = urlencode(data).encode("utf-8")
         # post请求接口
-        res = self.rx.session.open(
-            fullurl=run_case_html_url, data=bytes_data, timeout=10
-        )
+        res = self.rx.session.open(fullurl=run_case_html_url, data=bytes_data, timeout=10)
         status_code = res.status
         return status_code
 
     def send2pms(self, case_res_path, data_send_result_csv):
         """发送数据到PMS"""
         if exists(case_res_path):
             for case_name_json in os.listdir(case_res_path):
```

### Comparing `youqu-2.5.3/youqu/src/pms/suite.py` & `youqu-2.5.4/youqu/src/pms/suite.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=C0301,C0116,R1710,W0201,R0903
 import json
 import re
 from collections import deque
 
-from src  import logger
+from src import logger
 from src.pms._base import _Base
 from src.pms._base import _unicode_to_cn
 from src.pms._base import MAX_CASE_NUMBER
 
 
 class Suite(_Base):
     """获取测试套件关联的用例"""
```

### Comparing `youqu-2.5.3/youqu/src/pms/task.py` & `youqu-2.5.4/youqu/src/pms/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     def get_task_data(self, task_id):
         task_json_url = f"https://pms.uniontech.com/testtask-cases-{task_id}-all-0-id_desc-4-{MAX_CASE_NUMBER}-1.json"
         res = self.rx.open_url(task_json_url, timeout=10)
         res_str = _unicode_to_cn(res)
         try:
             res_dict = json.loads(res_str)
         except json.decoder.JSONDecodeError:
-            raise EnvironmentError(f"{task_json_url} 未获取到有效数据！\n 请检查你的PMS账号密码是否正确。")
+            raise EnvironmentError(
+                f"{task_json_url} 未获取到有效数据！\n 请检查你的PMS账号密码是否正确。"
+            )
         runs = res_dict.get("data").get("runs")
         runs_ids = deque()
         for run_case_id in runs:
             # 产品库ID
             case_id = runs.get(run_case_id).get("case")
             # 用例库ID
             from_case_id = runs.get(run_case_id).get("fromCaseID")
```

### Comparing `youqu-2.5.3/youqu/src/remotectl/_base.py` & `youqu-2.5.4/youqu/src/remotectl/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 # SPDX-License-Identifier: GPL-2.0-only
 
 import functools
+import inspect
+import multiprocessing
 import os
 import subprocess
 import sys
 import time
-import multiprocessing
-
 from os.path import dirname
-from os.path import basename
+from socketserver import ThreadingMixIn
+from xmlrpc.client import ServerProxy
+from xmlrpc.server import SimpleXMLRPCServer
 
 sys.path.append(dirname(dirname(dirname(os.path.abspath(__file__)))))
 
 from setting import conf
 from src.depends.colorama import Fore
 
 client_project_path = "/".join(conf.ROOT_DIR.split("/")[3:])
@@ -68,30 +70,28 @@
     os.system(
         f"sshpass -p '{password}' rsync -av -e ssh --exclude='__pycache__' "
         f"{conf.APPS_PATH}/{transfer_appname} {user}@{ip}:~/{client_project_path}/apps/"
     )
 
 
 def _transfer_to_client(ip, password, user):
-    os.system(
-        f'''{_ssh(ip, password, user)} "mkdir -p ~/{client_project_path}"'''
-    )
+    os.system(f'''{_ssh(ip, password, user)} "mkdir -p ~/{client_project_path}"''')
     os.system(
         f"sshpass -p '{password}' rsync -av -e ssh {_exclude()} {conf.ROOT_DIR}/* "
         f"{user}@{ip}:~/{client_project_path}/"
     )
     os.system(
         f'''{_ssh(ip, password, user)} "cd ~/{client_project_path}/ && mkdir apps && touch apps/__init__.py"'''
     )
-    os.system(
-        f'''{_ssh(ip, password, user)} "cd ~/{client_project_path}/apps/ && touch REMOTE"'''
-    )
-    if not os.popen(
-            f'''{_ssh(ip, password, user)} "cd ~/{client_project_path}/ && ls env_ok"'''
-    ).read().strip():
+    os.system(f'''{_ssh(ip, password, user)} "cd ~/{client_project_path}/apps/ && touch REMOTE"''')
+    if (
+            not os.popen(f'''{_ssh(ip, password, user)} "cd ~/{client_project_path}/ && ls env_ok"''')
+                    .read()
+                    .strip()
+    ):
         os.system(
             f'{_ssh(ip, password, user)} "cd ~/{client_project_path}/ && bash env.sh -p {password} && touch env_ok"'
         )
 
 
 def _start_client_service(ip, password, user, filename):
     _cmd = (
@@ -105,21 +105,20 @@
     time.sleep(1)
 
 
 def check_rpc_started(filename):
     def deco(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
-
-            user = kwargs.get('user') or args[0]
-            ip = kwargs.get('ip') or args[1]
+            user = kwargs.get("user") or args[0]
+            ip = kwargs.get("ip") or args[1]
             if not user or not ip:
                 raise ValueError("user and ip are required")
-            password = kwargs.get('password') or (args[2] if len(args) >= 3 else conf.PASSWORD)
-            transfer_appname = kwargs.get('transfer_appname')
+            password = kwargs.get("password") or (args[2] if len(args) >= 3 else conf.PASSWORD)
+            transfer_appname = kwargs.get("transfer_appname")
 
             _base_env_check()
             if transfer_appname:
                 _transfer_appname(ip, password, user, transfer_appname)
             tool_status = os.popen(
                 f'''{_ssh(ip, password, user)} "ps -aux |  grep {filename} | grep -v grep"'''
             ).read()
@@ -152,7 +151,23 @@
     try:
         import zerorpc
     except ImportError:
         raise ImportError("Please install zerorpc")
     server = zerorpc.Server(obj)
     server.bind(f"tcp://0.0.0.0:{port}")
     server.run()
+
+
+class ThreadXMLRPCServer(ThreadingMixIn, SimpleXMLRPCServer): ...
+
+
+def _remote_client(ip, port):
+    client = ServerProxy(f"http://{ip}:{port}", allow_none=True)
+    return client
+
+
+def _remote_server(obj, port):
+    server = ThreadXMLRPCServer(("0.0.0.0", port), allow_none=True)
+    for func, _ in inspect.getmembers(obj):
+        if not func.startswith("_"):
+            server.register_function(getattr(obj, func), func)
+    server.serve_forever()
```

### Comparing `youqu-2.5.3/youqu/src/remotectl/_remote_dogtail_ctl.py` & `youqu-2.5.4/youqu/src/remotectl/_remote_dogtail_ctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 
 @check_rpc_started(basename(__file__))
 def remote_dogtail_ctl(user=None, ip=None, password=None):
     return remote_client(ip=ip, port=dogtail_port)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from src.dogtail_utils import DogtailUtils
 
     remote_server(DogtailUtils(), dogtail_port)
```

### Comparing `youqu-2.5.3/youqu/src/remotectl/_remote_other_ctl.py` & `youqu-2.5.4/youqu/src/remotectl/_remote_other_ctl.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 
 @check_rpc_started(basename(__file__))
 def remote_other_ctl(user=None, ip=None, password=None, transfer_appname=None):
     return remote_client(ip=ip, port=port)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from src import Src
 
     remote_server(Src(), port)
```

### Comparing `youqu-2.5.3/youqu/src/remotectl/remote.py` & `youqu-2.5.4/youqu/src/remotectl/remote.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,50 +10,52 @@
 from src import Src
 from src.shortcut import ShortCut
 from src.cmdctl import CmdCtl
 from setting import conf
 
 
 class Remote(ShortCut, CmdCtl):
-
     def __init__(self, ip, user, password, transfer_appname=None):
         self.user = user
         self.ip = ip
         self.password = password
         self.transfer_appname = transfer_appname
         self.tmp_obj = None
 
     def __getattribute__(self, item):
         if not item.startswith("__") and not item.endswith("__"):
             for cls_obj in [ShortCut, CmdCtl]:
                 if hasattr(cls_obj, item):
                     self.tmp_obj = {"cls_obj": cls_obj, "item_obj": getattr(cls_obj, item)}
-                    delattr(cls_obj, item)
+                    while True:
+                        if hasattr(cls_obj, item):
+                            delattr(cls_obj, item)
+                        else:
+                            break
         return super().__getattribute__(item)
 
     def __getattr__(self, item):
         def func(*args, **kwargs):
             ar = ""
             if args:
                 for arg in args:
                     ar += f"'{arg}', "
             if kwargs:
                 for k, v in kwargs.items():
                     ar += f"{k}='{v}', "
-            logger.debug(
+            logger.info(
                 f"Remote(user='{self.user}', ip='{self.ip}', password='{self.password}').rctl.{item}({ar.rstrip(', ')})"
             )
             value = None
             try:
                 value = getattr(self.rctl, item)(*args, **kwargs)
             finally:
                 if self.tmp_obj:
                     setattr(self.tmp_obj["cls_obj"], item, self.tmp_obj["item_obj"])
-                if value is None:
-                    raise ValueError
+                    self.tmp_obj = None
             return value
 
         return func
 
     @property
     def rdog(self) -> DogtailUtils:
         return remote_dogtail_ctl(user=self.user, ip=self.ip, password=self.password)
@@ -64,18 +66,16 @@
     @property
     def rctl(self) -> Src:
         return remote_other_ctl(user=self.user, ip=self.ip, password=self.password)
 
     @property
     def rctl_plus(self) -> Src:
         return remote_other_ctl(
-            user=self.user, ip=self.ip, password=self.password, transfer_appname=self.transfer_appname
+            user=self.user,
+            ip=self.ip,
+            password=self.password,
+            transfer_appname=self.transfer_appname,
         )
 
     def find_image(self, image_path):
-        _image_path = image_path.replace(conf.HOME, "~", Maximum=1)
+        _image_path = image_path.replace(conf.HOME, "~", 1)
         return self.rctl_plus.find_image(_image_path)
-
-
-if __name__ == '__main__':
-    r = Remote(ip="", user="", password="")
-    r.ctrl_alt_t()
```

### Comparing `youqu-2.5.3/youqu/src/rtk/local_runner.py` & `youqu-2.5.4/youqu/src/rtk/local_runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,23 @@
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=C0301,R0913,R0914,W0613,R0912,R0915,E0401,C0413,C0103,C0116
 import json
 import re
 import sys
-from collections import Counter
 from os import chdir
 from os import environ
 from os import listdir
 from os import makedirs
 from os import system
 from os.path import exists
 from os.path import expanduser
 from os.path import isfile
 from os.path import join
-from time import sleep
 from tkinter import Tk
 
 import pytest
 from allure_custom import AllureCustom
 from allure_custom.conf import setting as al_setting
 
 from setting.globalconfig import GetCfg
@@ -32,79 +30,81 @@
 al_setting.html_title = GlobalConfig.REPORT_TITLE
 al_setting.report_name = GlobalConfig.REPORT_NAME
 al_setting.report_language = GlobalConfig.REPORT_LANGUAGE
 
 import letmego
 
 from src import logger
-from src.rtk._base import Args
+from src.rtk._base import Args, write_json
 from src.requestx import RequestX
 from src.rtk._base import transform_app_name
 
 environ["DISPLAY"] = ":0"
 
 
 class LocalRunner:
     """
     本地执行器
     """
+
     __author__ = "Mikigo <huangmingqiang@uniontech.com>"
 
     def __init__(
-            self,
-            app_name=None,
-            keywords=None,
-            tags=None,
-            report_formats=None,
-            max_fail=None,
-            reruns=None,
-            record_failed_case=None,
-            clean=None,
-            log_level=None,
-            timeout=None,
-            debug=False,
-            noskip=None,
-            ifixed=None,
-            send_pms=None,
-            task_id=None,
-            suite_id=None,
-            trigger=None,
-            resolution=None,
-            case_file=None,
-            deb_path=None,
-            pms_user=None,
-            pms_password=None,
-            pms_info_file=None,
-            top=None,
-            lastfailed=None,
-            duringfail=None,
-            repeat=None,
-            project_name=None,
-            build_location=None,
-            line=None,
-            collection_only=None,
-            autostart=None,
-            export_csv_file=None,
-            slaves=None,
-            **kwargs,
+        self,
+        app_name=None,
+        keywords=None,
+        tags=None,
+        report_formats=None,
+        max_fail=None,
+        reruns=None,
+        record_failed_case=None,
+        clean=None,
+        log_level=None,
+        timeout=None,
+        debug=False,
+        noskip=None,
+        ifixed=None,
+        send_pms=None,
+        task_id=None,
+        suite_id=None,
+        trigger=None,
+        resolution=None,
+        case_file=None,
+        deb_path=None,
+        pms_user=None,
+        pms_password=None,
+        pms_info_file=None,
+        top=None,
+        lastfailed=None,
+        duringfail=None,
+        repeat=None,
+        project_name=None,
+        build_location=None,
+        line=None,
+        collection_only=None,
+        autostart=None,
+        export_csv_file=None,
+        slaves=None,
+        **kwargs,
     ):
         logger("INFO")
         try:
             github_tags = RequestX().open_url(
-                f"https://api.github.com/repos/linuxdeepin/youqu/tags",
-                timeout=1
+                f"https://api.github.com/repos/linuxdeepin/youqu/tags", timeout=1
             )
             latest_tag = json.loads(github_tags)[0].get("name")
             if GlobalConfig.current_tag != latest_tag:
                 print(f"YouQu最新版本为: {latest_tag}，当前使用版本为: {GlobalConfig.current_tag}")
                 print(f"建议使用：sudo pip3 install youqu=={latest_tag} 升级版本")
         except Exception:
             pass
         self.default = {
-            Args.app_name.value: transform_app_name(app_name if app_name or case_file else GlobalConfig.APP_NAME),
+            Args.app_name.value: transform_app_name(
+                app_name if app_name or case_file else GlobalConfig.APP_NAME
+            ),
             Args.keywords.value: keywords or GlobalConfig.KEYWORDS,
             Args.tags.value: tags or GlobalConfig.TAGS,
             Args.report_formats.value: report_formats or GlobalConfig.REPORT_FORMAT,
             Args.max_fail.value: max_fail or GlobalConfig.MAX_FAIL,
             Args.reruns.value: reruns or GlobalConfig.RERUN,
             Args.record_failed_case.value: record_failed_case or GlobalConfig.RECORD_FAILED_CASE,
             Args.clean.value: clean or GlobalConfig.CLEAN_ALL,
@@ -119,17 +119,15 @@
             Args.trigger.value: trigger or GlobalConfig.TRIGGER,
             Args.resolution.value: resolution or GlobalConfig.RESOLUTION,
             Args.case_file.value: case_file or GlobalConfig.CASE_FILE,
             Args.deb_path.value: deb_path or GlobalConfig.DEB_PATH,
             Args.duringfail.value: duringfail or GlobalConfig.DURING_FAIL,
             Args.repeat.value: repeat or GlobalConfig.REPEAT,
             Args.top.value: top or GlobalConfig.TOP,
-            Args.pms_user.value: (pms_user or GlobalConfig.PMS_USER)
-            if not pms_info_file
-            else None,
+            Args.pms_user.value: (pms_user or GlobalConfig.PMS_USER) if not pms_info_file else None,
             Args.pms_password.value: (pms_password or GlobalConfig.PMS_PASSWORD)
             if not pms_info_file
             else None,
             Args.pms_info_file.value: pms_info_file,
             Args.autostart.value: autostart or GlobalConfig.AUTOSTART,
         }
         self.lastfailed = lastfailed
@@ -145,93 +143,77 @@
             x = screen.winfo_screenwidth()
             y = screen.winfo_screenheight()
             rls = [i.strip() for i in self.default.get(Args.resolution.value).split(",")]
             for rl in rls:
                 if rl in (f"{x}x{y}", "no"):
                     break
             else:
-                raise ValueError(f"当前分辨率为：{x}x{y},您配置的分辨率为：{GlobalConfig.RESOLUTION}")
+                raise ValueError(
+                    f"当前分辨率为：{x}x{y},您配置的分辨率为：{GlobalConfig.RESOLUTION}"
+                )
 
     @property
     def export_default(self):
         return self.default
 
     @staticmethod
     def make_dir(dirs):
-        """make_dir"""
         try:
             dirs = expanduser(dirs)
             if not exists(dirs):
                 makedirs(dirs)
         except FileExistsError:
             pass
 
     # 报告
     @classmethod
     def make_allure_report(cls, cmd, fmt, proj_path=None):
-        """make_allure_report"""
         allure_report_path = f"{proj_path}/report/allure"
         if proj_path is None:
             allure_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, fmt)
             cls.make_dir(allure_report_path)
         cmd.append(f"--alluredir={allure_report_path}")
 
     @classmethod
     def make_xml_report(cls, app_dir, case_file, cmd, fmt, proj_path=None):
-        """make_xml_report"""
         xml_report_path = f"{proj_path}/report/xml"
         if proj_path is None:
             xml_report_path = join(GlobalConfig.XML_REPORT_PATH, fmt)
             cls.make_dir(xml_report_path)
-        report_name = (
-            case_file.replace("/", "_").replace(".", "_")
-            if case_file
-            else app_dir
-        )
+        report_name = case_file.replace("/", "_").replace(".", "_") if case_file else app_dir
         cmd.append(
             f"--junit-xml={xml_report_path}/{report_name}{'-' if report_name else ''}{GlobalConfig.TIME_STRING}.xml"
         )
 
     def create_pytest_cmd(self, app_dir, default=None, proj_path=None):
-        """
-         创建 Pytest 及其命令行参数
-        :param app_dir:
-        :return:
-        """
         if default is None:
             default = self.default
         keywords_or_marker = True
         cmd = ["pytest"]
         if self.lastfailed:
             cmd.append("--lf")
             keywords_or_marker = False
         # 通过文件存放pms信息,Jenkins环境下不希望明文显示密码等信息,可信息存放在文件中
         elif default.get(Args.pms_info_file.value):
-            pms_info_file_path = (
-                f"{GlobalConfig.ROOT_DIR}/{default.get(Args.pms_info_file.value)}"
-            )
+            pms_info_file_path = f"{GlobalConfig.ROOT_DIR}/{default.get(Args.pms_info_file.value)}"
             if not exists(pms_info_file_path):
                 logger.error(pms_info_file_path)
                 raise FileNotFoundError
             pms_cfg = GetCfg(pms_info_file_path, "pms")
             cmd.extend(["--pms_user", pms_cfg.get("PMS_USER", default="")])
             cmd.extend(["--pms_password", pms_cfg.get("PMS_PASSWORD", default="")])
             keywords_or_marker = False
         # 通过pms测试套执行用例
-        elif default.get(Args.pms_user.value) and default.get(
-                Args.pms_password.value
-        ):
+        elif default.get(Args.pms_user.value) and default.get(Args.pms_password.value):
             cmd.extend(["--pms_user", default.get(Args.pms_user.value)])
             cmd.extend(["--pms_password", default.get(Args.pms_password.value)])
             keywords_or_marker = False
         # 通过本地测试套
         elif default.get(Args.case_file.value):
-            file_path = (
-                f"{GlobalConfig.ROOT_DIR}/{default.get(Args.case_file.value)}"
-            )
+            file_path = f"{GlobalConfig.ROOT_DIR}/{default.get(Args.case_file.value)}"
             if (not exists(file_path)) or (not isfile(file_path)):
                 logger.error(f"{file_path} 文件不存在.")
                 raise FileNotFoundError
             if not default.get(Args.case_file.value).endswith(".txt"):
                 logger.error(f"测试套文件{default.get(Args.case_file.value)},不是一个txt文件")
                 raise FileNotFoundError
             logger.info(f"本地测试套文件：{file_path}")
@@ -296,73 +278,60 @@
             cmd.extend(["--slaves", self.slaves])
 
         report_formats = default.get(Args.report_formats.value)
         if report_formats:
             report_formats = [i.strip() for i in report_formats.split(",")]
             # allure
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) and (
-                    GlobalConfig.ReportFormat.JSON not in report_formats
+                GlobalConfig.ReportFormat.JSON not in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
             # xml
             if GlobalConfig.ReportFormat.XML in report_formats:
                 self.make_xml_report(
                     app_dir,
                     default.get(Args.case_file.value),
                     cmd,
                     GlobalConfig.ReportFormat.XML,
                     proj_path,
                 )
             # json
             if (GlobalConfig.ReportFormat.ALLURE not in report_formats) and (
-                    GlobalConfig.ReportFormat.JSON in report_formats
+                GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
-                self.make_dir(
-                    join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON)
-                )
+                self.make_dir(join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON))
             # allure json
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) and (
-                    GlobalConfig.ReportFormat.JSON in report_formats
+                GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
-                self.make_dir(
-                    join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON)
-                )
+                self.make_dir(join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON))
         return cmd
 
     @staticmethod
     def set_recursion_limit(strings):
         len_tags = len(re.split("or |and |not ", strings))
         if len_tags >= 999:
             sys.setrecursionlimit(len_tags + 100)
 
     def change_working_dir(self):
-        """
-         切换工作区间
-        :param app_name:
-        :return:
-        """
         app_name: str = self.default.get(Args.app_name.value)
         if app_name:
             applications = listdir(GlobalConfig.APPS_PATH)
             for working_dir in applications:
                 if working_dir == app_name:
                     case_path = f"{GlobalConfig.APPS_PATH}/{working_dir}"
                     print(f"WorkSpace: \n{case_path}")
                     chdir(case_path)
                     return working_dir
             raise NotADirectoryError(f"apps 目录下未找到指定的 {app_name}")
         return GlobalConfig.APPS_PATH
 
     def local_run(self):
-        """
-         执行用例
-        :return:
-        """
         if not self.default.get(Args.autostart.value):
             # 备份 allure 报告
             allure_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, "allure")
             allure_report_back_path = join(
                 GlobalConfig.ALLURE_REPORT_PATH, "allure_back", GlobalConfig.TIME_STRING
             )
             if exists(allure_report_path) and listdir(allure_report_path):
@@ -378,36 +347,32 @@
         if self.default.get(Args.debug.value):
             logger.info("Debug 模式不执行用例!")
             return
         pytest.main([i.strip("'") for i in run_test_cmd_list[1:]])
 
         if self.collection_only:
             return
+
         if self.project_name and self.build_location and self.line:
-            self.write_json(
+            write_json(
                 project_name=self.project_name,
                 build_location=self.build_location,
                 line=self.line,
             )
-        allure_report_path = join(
-            GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.ALLURE
-        )
+        allure_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.ALLURE)
         allure_html_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, "allure_html")
 
-        json_report_path = join(
-            GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.JSON
-        )
+        json_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.JSON)
 
         if self.default.get(Args.report_formats.value):
             report_formats = [
-                i.strip()
-                for i in self.default.get(Args.report_formats.value).split(",")
+                i.strip() for i in self.default.get(Args.report_formats.value).split(",")
             ]
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) or (
-                    GlobalConfig.ReportFormat.JSON in report_formats
+                GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 if exists(allure_html_report_path):
                     system(f"rm -rf {allure_html_report_path}")
                 makedirs(allure_html_report_path)
 
                 AllureCustom.gen(allure_report_path, allure_html_report_path)
 
@@ -420,78 +385,15 @@
 
         if exists(letmego.conf.setting.RUNNING_MAN_FILE):
             letmego.unregister_autostart_service()
             letmego.clean_running_man(
                 copy_to=f"{GlobalConfig.REPORT_PATH}/_running_man_{GlobalConfig.TIME_STRING}.log"
             )
 
-    @classmethod
-    def get_result(cls, ci_result):
-        """
-         获取结果
-        :return:
-        """
-        with open(ci_result, "r", encoding="utf-8") as _f:
-            results_dict = json.load(_f)
-        res = Counter([results_dict.get(i).get("result") for i in results_dict])
-        total = sum(res.values())
-        skiped = res.get("skip", 0)
-        total = total - skiped
-        passed = res.get("pass", 0)
-        failed = total - passed
-        pass_rate = f"{round((passed / total) * 100, 1)}%" if passed else "0%"
-        return total, failed, passed, pass_rate
-
-    @classmethod
-    def write_json(cls, project_name=None, build_location=None, line=None):
-        """
-         写json报告
-        {
-          "project_name": "",
-          "build_location": "",
-          "line": "",
-          "total": "",
-          "fail": "",
-          "block": "",
-          "pass": "",
-          "pass_rate": ""
-        }
-        """
-        json_tpl_path = f"{GlobalConfig.SETTING_PATH}/template/ci.json"
-        if not exists(json_tpl_path):
-            raise FileNotFoundError
-        with open(json_tpl_path, "r", encoding="utf-8") as _f:
-            results = json.load(_f)
-
-        results["project_name"] = project_name
-        results["build_location"] = build_location
-        results["line"] = line
-        ci_result_path = f"{GlobalConfig.ROOT_DIR}/ci_result.json"
-        if not exists(ci_result_path):
-            return
-
-        (
-            results["total"],
-            results["fail"],
-            results["pass"],
-            results["pass_rate"],
-        ) = cls.get_result(ci_result_path)
-
-        json_res_path = f"{GlobalConfig.ROOT_DIR}/{project_name}_at.json"
-        with open(json_res_path, "w+", encoding="utf-8") as _f:
-            _f.write(json.dumps(results, indent=2, ensure_ascii=False))
-        sleep(1)
-        with open(json_res_path, "r", encoding="utf-8") as _f:
-            print("CICD数据结果:\n", _f.read())
-
     def install_deb(self):
-        """
-         安装本地 deb 包
-        :return:
-        """
         logger.info("安装deb包")
         system(
             f"cd {self.default.get(Args.deb_path.value)}/ && echo {GlobalConfig.PASSWORD} | sudo -S dpkg -i *.deb"
         )
         logger.info("deb包安装完成")
```

### Comparing `youqu-2.5.3/youqu/src/rtk/remote_runner.py` & `youqu-2.5.4/youqu/src/rtk/remote_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,31 +46,32 @@
     远程执行器：控制多台测试机远程执行用例。
     在 setting/remote.ini 里面配置要执行的测试机信息。
     """
 
     __author__ = "Mikigo <huangmingqiang@uniontech.com>"
 
     def __init__(
-            self,
-            remote_kwargs: dict = None,
-            local_kwargs: dict = None,
+        self,
+        remote_kwargs: dict = None,
+        local_kwargs: dict = None,
     ):
         self.remote_kwargs = remote_kwargs
         self.local_kwargs = local_kwargs
         logger("INFO")
         self.parallel = conf.PARALLEL
         self.clean_server_report_dir = conf.CLEAN_SERVER_REPORT_DIR
         self.clean_client_report_dir = conf.CLEAN_CLIENT_REPORT_DIR
         self.send_code = conf.SEND_CODE
         self.scan = int(conf.SCAN)
         self.client_env = conf.BUILD_ENV
         self.client_password = conf.CLIENT_PASSWORD
 
         self._default = {
-            Args.client_password.value: remote_kwargs.get("client_password") or self.client_password,
+            Args.client_password.value: remote_kwargs.get("client_password")
+            or self.client_password,
         }
 
         client_dict = {}
         _client = remote_kwargs.get("clients") or conf.CLIENTS
         if _client:
             clients = _client.split("/")
             for index, client in enumerate(clients):
@@ -84,40 +85,44 @@
         else:
             raise ValueError(
                 "未获取到测试机信息,请检查 setting/globalconfig.ini 中 CLIENT LIST 是否配置，"
                 "或通过命令行 remote -c user@ip:password 传入。"
             )
 
         self.default = {
-            Args.app_name.value: transform_app_name(local_kwargs.get("app_name") or GlobalConfig.APP_NAME),
+            Args.app_name.value: transform_app_name(
+                local_kwargs.get("app_name") or GlobalConfig.APP_NAME
+            ),
             Args.clients.value: client_dict,
             Args.send_code.value: remote_kwargs.get("send_code") or self.send_code,
             Args.build_env.value: remote_kwargs.get("build_env") or self.client_env,
             Args.parallel.value: remote_kwargs.get("parallel") or self.parallel,
         }
         # 客户端地址
         if "/home/" not in GlobalConfig.ROOT_DIR:
             raise EnvironmentError
         self.server_project_path = "/".join(GlobalConfig.ROOT_DIR.split("/")[3:])
-        self.client_report_path = (
-            lambda x: f"/home/{x}/{self.server_project_path}/report"
+        self.client_report_path = lambda x: f"/home/{x}/{self.server_project_path}/report"
+        self.client_allure_report_path = (
+            lambda x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('ALLURE_REPORT_PATH', default='report')}/allure".replace(
+                "//", "/"
+            )
         )
-        self.client_allure_report_path = lambda \
-                x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('ALLURE_REPORT_PATH', default='report')}/allure".replace(
-            "//", "/"
-        )
-        self.client_pms_json_report_path =  lambda x, y: f"/home/{x}/{self.server_project_path}/report/pms_{y}"
-
-        self.client_xml_report_path = lambda \
-                x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('XML_REPORT_PATH', default='report')}/xml".replace(
-            "//", "/"
+        self.client_pms_json_report_path = (
+            lambda x, y: f"/home/{x}/{self.server_project_path}/report/pms_{y}"
+        )
+
+        self.client_xml_report_path = (
+            lambda x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('XML_REPORT_PATH', default='report')}/xml".replace(
+                "//", "/"
+            )
         )
         self.client_list = list(self.default.get(Args.clients.value).keys())
         _pty = "t"
-        if len(self.client_list) >=2:
+        if len(self.client_list) >= 2:
             _pty = "T"
         self.ssh = f"sshpass -p '%s' ssh -{_pty}"
         self.scp = "sshpass -p '%s' scp -r"
         self.rsync = "sshpass -p '%s' rsync -av -e ssh"
         self.empty = "> /dev/null 2>&1"
         self.strf_time = strftime("%m%d%p%I%M%S")
 
@@ -288,39 +293,46 @@
             i[0] = f"--{i[0]}"
             i[1] = f"'{i[1]}'"
             if i[0] == "--app_name":
                 real_app_name = f"apps/{self.default.get(Args.app_name.value)}"
                 continue
 
             _tmp_args.extend(i)
-        cmd.extend([
-            f"~/{self.server_project_path}/{real_app_name}",
-            "&&",
-            "pipenv",
-            "run",
-        ])
+        cmd.extend(
+            [
+                f"~/{self.server_project_path}/{real_app_name}",
+                "&&",
+                "pipenv",
+                "run",
+            ]
+        )
         from src.rtk.local_runner import LocalRunner
+
         lr = LocalRunner(debug=True)
-        lr_args = {k:v for k, v in lr.export_default.items() if v}
-        rr_args = {k:v for k, v in self.local_kwargs.items() if v}
+        lr_args = {k: v for k, v in lr.export_default.items() if v}
+        rr_args = {k: v for k, v in self.local_kwargs.items() if v}
         lr_args.update(rr_args)
         if all(
             [
                 lr_args.get(Args.task_id.value),
                 lr_args.get(Args.pms_user.value),
                 lr_args.get(Args.pms_password.value),
                 lr_args.get(Args.send_pms.value) == "finish",
             ]
         ):
             lr_args[Args.trigger.value] = "hand"
             self.collection_json = True
             self.pms_user = lr_args.get(Args.pms_user.value)
             self.pms_password = lr_args.get(Args.pms_password.value)
             self.server_json_dir_id = lr_args.get(Args.task_id.value)
-        pytest_cmd = lr.create_pytest_cmd(real_app_name.replace("apps/", ""), default=lr_args, proj_path=f"/home/{user}/{self.server_project_path}")
+        pytest_cmd = lr.create_pytest_cmd(
+            real_app_name.replace("apps/", ""),
+            default=lr_args,
+            proj_path=f"/home/{user}/{self.server_project_path}",
+        )
 
         cmd.extend(pytest_cmd)
         cmd.append('"')
         cmd_str = " ".join(cmd)
         if self.default.get(Args.debug.value):
             logger.info(f"\n{cmd_str}\n")
             logger.info("DEBUG 模式不执行用例!")
@@ -329,17 +341,15 @@
 
     def pytest_co_cmd(self):
         """
          创建收集用例的命令行参数
         :return:
         """
         app_dir = (
-            self.default.get(Args.app_name.value)
-            if self.default.get(Args.app_name.value)
-            else ""
+            self.default.get(Args.app_name.value) if self.default.get(Args.app_name.value) else ""
         )
         cmd = [
             "pytest",
             f"{GlobalConfig.APPS_PATH}/{app_dir}",
         ]
         if self.default.get(Args.keywords.value):
             cmd.extend(["-k", f"'{self.default.get(Args.keywords.value)}'"])
@@ -472,15 +482,15 @@
         :param client_list:
         :return:
         """
         _ps = []
         executor = ThreadPoolExecutor()
         for client in client_list[:-1]:
             user, _ip, password = self.default.get(Args.clients.value).get(client)
-            _p3 = executor.submit(self.run_pytest_cmd,  user, _ip, password)
+            _p3 = executor.submit(self.run_pytest_cmd, user, _ip, password)
             _ps.append(_p3)
             sleep(1)
         user, _ip, password = self.default.get(Args.clients.value).get(client_list[-1])
         self.run_pytest_cmd(
             user,
             _ip,
             password,
@@ -541,15 +551,16 @@
         """
          远程执行主函数
         :return:
         """
         client_list = list(self.default.get(Args.clients.value).keys())
         self.pre_env()
         logger.info(
-            "\n测试机列表:\n" + "\n".join([str(i) for i in self.default.get(Args.clients.value).items()])
+            "\n测试机列表:\n"
+            + "\n".join([str(i) for i in self.default.get(Args.clients.value).items()])
         )
         if self.default.get(Args.build_env.value):
             self.mul_do(self.send_code_and_env, client_list)
         else:
             if self.default.get(Args.send_code.value):
                 self.mul_do(self.send_code_to_client, client_list)
         if self.default.get(Args.deb_path.value):
```

### Comparing `youqu-2.5.3/youqu/src/utils/check_python_source.py` & `youqu-2.5.4/youqu/src/utils/check_python_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from urllib.error import URLError
 from urllib.request import build_opener
 from http import cookiejar
 
 
 class RequestX:
     """RequestX"""
+
     def __init__(
-            self,
-            login_url=None,
-            headers=None,
-            data=None,
+        self,
+        login_url=None,
+        headers=None,
+        data=None,
     ):
         self.login_url = login_url
         self.headers = headers
         self.data = parse.urlencode(data).encode("utf-8") if data else None
         self.kwargs = {}
         if self.login_url:
             self.kwargs["url"] = self.login_url
```

### Comparing `youqu-2.5.3/youqu/src/utils/opencv_rpc_server.py` & `youqu-2.5.4/youqu/src/utils/opencv_rpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,18 +82,15 @@
     # else:
     loc = np.where(result >= rate)
     tmp_list_out = []
     tmp_list_in = []
     loc_list = list(zip(*loc))
     for i in range(0, len(loc_list) - 1):
         tmp_list_in.append(loc_list[i])
-        if (
-                loc_list[i + 1][0] != loc_list[i][0]
-                or (loc_list[i + 1][1] - loc_list[i][1]) > 1
-        ):
+        if loc_list[i + 1][0] != loc_list[i][0] or (loc_list[i + 1][1] - loc_list[i][1]) > 1:
             tmp_list_out.append(tmp_list_in)
             tmp_list_in = []
             continue
         if i == len(loc_list) - 2:
             tmp_list_in.append(loc_list[-1])
             tmp_list_out.append(tmp_list_in)
     result_list = []
```

### Comparing `youqu-2.5.3/youqu/src/utils/sslclone.sh` & `youqu-2.5.4/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/youqu/src/utils/sub_deb.py` & `youqu-2.5.4/youqu/src/utils/sub_deb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 py_debs = []
 for root, dirs, files in os.walk(os.path.abspath("../../apps")):
     for file in files:
         if file == "requirement_deb.txt":
             with open(f"{root}/{file}", "r", encoding="utf-8") as f:
                 py_debs.extend([i.strip() for i in f.read().split("\n")])
 
-print(" ".join(py_debs), end="")
+print(" ".join(py_debs), end="")
```

### Comparing `youqu-2.5.3/youqu/src/utils/vnc.sh` & `youqu-2.5.4/youqu/src/utils/vnc.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.3/pyproject.toml` & `youqu-2.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youqu"
-version = "2.5.3"
+version = "2.5.4"
 authors = [
     { name = "mikigo", email = "huangmingqiang@uniontech.com" },
 ]
 
 description = "youqu"
 readme = "youqu/README.md"
 requires-python = ">=3.7"
```

### Comparing `youqu-2.5.3/youqu/README.md` & `youqu-2.5.4/youqu/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 <p align="center">
-  <a href="https://linuxdeepin.github.io/youqu/">
-    <img src="./docs/logo.png" width="520" alt="YouQu">
+  <a href="https://linuxdeepin.github.io/youqu">
+    <img src="./docs/assets/logo.png" width="520" alt="YouQu">
   </a>
 </p>
 <p align="center">
     <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
 
 
+
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
 [![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
 
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
 ![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
-
 [![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
 <a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
-<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a> | <a href="https://deepin-community.gitee.io/youqu/" target="_blank">在线文档（国内加速）</a>
+<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
 
 ---
 
 YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
 
 ## YouQu（有趣）能做什么
 
@@ -72,196 +72,103 @@
 从 PyPI 安装:
 
 
 ```shell
 $ sudo pip3 install youqu
 ```
 
-创建项目:
+## 创建项目
+
+您可以在任意目录下，使用 `youqu-startproject` 命令创建一个项目：
 
 ```shell
 $ youqu-startproject my_project
 ```
 
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
-安装依赖:
+![](./docs/assets/install.gif)
+
+## 安装依赖
+
+安装部署 YouQu 执行所需环境： 
 
 ```shell
 $ cd my_project
-
-# 使用的默认密码是 1 ，您可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项
 $ bash env.sh
-
-# 也可以使用 -p 选项传入密码
-$ bash env.sh -p ${my_password}
 ```
 
-## 创建工程
+## 创建 APP 工程
 
-如果您已经有一个可用的 `APP` 工程，将应用库放到基础框架下 `apps` 目录下，像这样：
+使用 `startapp` 命令自动创建 APP 工程：
 
 ```shell
-my_project
-├── apps
-│   ├── autotest_deepin_music  # 应用库
-...
+$ youqu manage.py startapp autotest_deepin_some
 ```
 
-如果您还没有 `APP` 工程，建议使用框架提供的脚手架功能创建一个全新的 `APP` 工程。
+自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
-**创建一个 APP 工程**
+在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
-$ youqu manage.py startapp autotest_deepin_some
+my_project
+├── apps
+│   ├── autotest_deepin_some  # <----- APP 工程
+...     ├── ...
 ```
 
-这样在 `apps` 目录下会创建一个子项目工程 `autotest_deepin_some`，同时新建好工程模板目录和模板文件：
+在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
 
-```shell
-apps
-└── autotest_deepin_some
-    ├── case
-    │   ├── assert_res
-    │   │   └── readme
-    │   ├── base_case.py
-    │   └── __init__.py
-    ├── config.ini
-    ├── config.py
-    ├── conftest.py
-    ├── control
-    ├── deepin_some_assert.py
-    ├── deepin_some.csv
-    ├── __init__.py
-    └── widget
-        ├── base_widget.py
-        ├── case_res
-        │   └── readme
-        ├── deepin_some_widget.py
-        ├── __init__.py
-        ├── other.ini
-        ├── other_widget.py
-        ├── pic_res
-        │   └── readme
-        └── ui.ini
-```
-
-`autotest_deepin_some` 是你的工程名称，比如：`autotest_deepin_music` ；
+`autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
 
-在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
+`apps` 目录下可以存在任意多个 APP 工程。
 
 运行
 -------
 
-### 1. 工作空间
+### 1. 执行管理器
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
 ### 2. 本地执行
 
 
 ```shell
 $ youqu manage.py run
 ```
 
 #### 2.1. 命令行参数
 
-通过命令行参数配置参数，使用 `-h` 或 `--help` 可以查看所有支持的命令行参数：
-
-
-```shell
-$ youqu manage.py run -h
-```
-
 在一些 CI 环境下使用命令行参数会更加方便：
 
 
 ```shell
-$ youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags "xxx"
+$ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
 ```
 
-更多参数请查看【[命令行参数](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
+更多用法可以使用 `-h` 或 `--help` 查看。
 
 #### 2.2. 配置文件
 
 通过配置文件配置参数
 
-在配置文件 `setting/globalconfig.ini` 里面支持配置对执行的一些参数进行配置，配置完成之后，直接在命令行执行 `manage.py` 就好了。
-
-详细配置项请查看【[配置项](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
+在配置文件 [setting/globalconfig.ini](https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)  里面支持配置对执行的一些参数进行配置。
 
 ### 3. 远程执行
 
-远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同；
+远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同。
 
 使用 `remote` 命令：
 
 
 ```shell
 $ youqu manage.py remote
 ```
 
-以下为 `remote` 提供的一些参数选项：
-
-```coffeescript
-  -h, --help            show this help message and exit
-  -c CLIENTS, --clients CLIENTS
-                        远程机器的user@ip:password,多个机器用'/'连接,如果password不传入,默认取sett
-                        ing/remote.ini中CLIENT_PASSWORD的值,比如: uos@10.8.13.xx:1
-                        或 uos@10.8.13.xx
-  -s, --send_code       发送代码到测试机（不含report目录）
-  -e, --build_env       搭建测试环境,如果为yes，不管send_code是否为yes都会发送代码到测试机.
-  -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
-                        测试机密码（全局）
-  -y PARALLEL, --parallel PARALLEL
-                        yes:表示所有测试机并行跑，执行相同的测试用例;no:表示测试机分布式执行，服务端会根据收集到的测试用例自
-                        动分配给各个测试机执行。
-```
-
-除了这些特有参数以外，它同样支持本地执行的所有参数；
-
-在命令行这样运行：
-
-
-```shell
-$ youqu manage.py remote -a apps/autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx"
-```
-
-所有用例执行完之后会在 `report` 目录下回收各个测试机执行的测试报告。
-
-注意：如果远程机器没有搭建自动化测试环境，记得加上参数 `-e` ：
-
-
-```shell
-$ youqu manage.py remote -a ... -e
-```
-
-执行前确保远程机器已经开启了 ssh 服务，否则会提示无法连接，如果没有开启，请手动开启：
-
-
-```shell
-$ sudo systemctl restart ssh
-$ sudo systemctl enable ssh
-```
-
-配置文件其他相关配置项详细说明，请查看配置文件中的注释内容。
-
 ## 贡献
 
 [贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
 
 
 ## 开源许可证
 
-有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
-
-------------
-
-[__Github Star History__]()
-
-[![Stargazers over time](https://starchart.cc/linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu)
-
-
-
-[__Gitee Info__]()
-
-[![deepin-community/youqu](https://gitee.com/deepin-community/youqu/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/youqu)
+YouQu 在 [GPL-2.0](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
```

#### html2text {}

```diff
@@ -13,16 +13,15 @@
 pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
 badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
 project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
 (https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
 youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
 linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
-github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ |
-_å__¨_ç_º_¿_æ___æ_¡_£_ï_¼__å__½_å___å__ _é___ï_¼_ --
+github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --
 - YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ##
 YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] Linux æ¡é¢åºç¨ UI èªå¨åæµè¯ - [x]
 Linux æ¡é¢åºç¨ DBus/Gsettings æ¥å£èªå¨åæµè¯ - [x]
 å½ä»¤è¡èªå¨åæµè¯ - [x] HTTP æ¥å£èªå¨åæµè¯ - [x] Web UI
 èªå¨åæµè¯ - [ ] Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯
@@ -47,85 +46,40 @@
     * æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ãPMS
       æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
     * æ¯æåºäºæ·±åº¦å­¦ä¹ ç OCR
       åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼
     * å®ç¾å¼å®¹ Wayland å X11ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼
     * æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
     * æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼
-## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` åå»ºé¡¹ç®:
-```shell $ youqu-startproject my_project ``` å¦æ `youqu-startproject`
-åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ å®è£ä¾èµ:
-```shell $ cd my_project # ä½¿ç¨çé»è®¤å¯ç æ¯ 1
-ï¼æ¨å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/globalconfig.ini éé¢ç PASSWORD
-éç½®é¡¹ $ bash env.sh # ä¹å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç  $ bash env.sh -
-p ${my_password} ``` ## åå»ºå·¥ç¨ å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
-å·¥ç¨ï¼å°åºç¨åºæ¾å°åºç¡æ¡æ¶ä¸ `apps` ç®å½ä¸ï¼åè¿æ ·ï¼
-```shell my_project âââ apps â âââ autotest_deepin_music #
-åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
-å·¥ç¨ï¼å»ºè®®ä½¿ç¨æ¡æ¶æä¾çèææ¶åè½åå»ºä¸ä¸ªå¨æ°ç `APP`
-å·¥ç¨ã **åå»ºä¸ä¸ª APP å·¥ç¨** ```shell $ youqu manage.py startapp
-autotest_deepin_some ``` è¿æ ·å¨ `apps`
-ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
-`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell apps âââ autotest_deepin_some Â Â  âââ case Â Â  âÂ Â 
-âââ assert_res Â Â  âÂ Â  âÂ Â  âââ readme Â Â  âÂ Â 
-âââ base_case.py Â Â  âÂ Â  âââ __init__.py Â Â  âââ
-config.ini Â Â  âââ config.py Â Â  âââ conftest.py Â Â  âââ
-control Â Â  âââ deepin_some_assert.py Â Â  âââ deepin_some.csv
-Â Â  âââ __init__.py Â Â  âââ widget Â Â  âââ base_widget.py
-Â Â  âââ case_res Â Â  âÂ Â  âââ readme Â Â  âââ
-deepin_some_widget.py Â Â  âââ __init__.py Â Â  âââ other.ini Â Â 
-âââ other_widget.py Â Â  âââ pic_res Â Â  âÂ Â  âââ readme
-Â Â  âââ ui.ini ``` `autotest_deepin_some`
-æ¯ä½ çå·¥ç¨åç§°ï¼æ¯å¦ï¼`autotest_deepin_music` ï¼
-å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
-é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã è¿è¡ ------- ### 1.
-å·¥ä½ç©ºé´ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
+## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` ##
+åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
+å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ``` å¦æ
+`youqu-startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu`
+ï¼ ![](./docs/assets/install.gif) ## å®è£ä¾èµ å®è£é¨ç½² YouQu
+æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
+å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
+manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
+å·¥ç¨éµå¾ªå®æ´ç PO
+è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
+`apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
+å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
+```shell my_project âââ apps â âââ autotest_deepin_some # <----
+- APP å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
+ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
+`autotest_deepin_some` æ¯ä½ ç APP
+å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
+é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
+ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
+æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
 ### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
-å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ `--help`
-å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼ ```shell $ youqu manage.py run -
-h ``` å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $
-youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags
-"xxx" ``` æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://
-linuxdeepin.github.io/youqu/
-%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
-%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)ã #### 2.2. éç½®æä»¶
-éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ `setting/globalconfig.ini`
-éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ï¼éç½®å®æä¹åï¼ç´æ¥å¨å½ä»¤è¡æ§è¡
-`manage.py` å°±å¥½äºã è¯¦ç»éç½®é¡¹è¯·æ¥çã[éç½®é¡¹](https://
-linuxdeepin.github.io/youqu/
-%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
-%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)ã ### 3. è¿ç¨æ§è¡
-è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åï¼
-ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ä»¥ä¸ä¸º
-`remote` æä¾çä¸äºåæ°éé¡¹ï¼ ```coffeescript -h, --help show this
-help message and exit -c CLIENTS, --clients CLIENTS è¿ç¨æºå¨çuser@ip:
-password,å¤ä¸ªæºå¨ç¨'/'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
-remote.iniä¸­CLIENT_PASSWORDçå¼,æ¯å¦: uos@10.8.13.xx:1 æ uos@10.8.13.xx
--s, --send_code åéä»£ç å°æµè¯æºï¼ä¸å«reportç®å½ï¼ -e, --
-build_env
-æ­å»ºæµè¯ç¯å¢,å¦æä¸ºyesï¼ä¸ç®¡send_codeæ¯å¦ä¸ºyesé½ä¼åéä»£ç å°æµè¯æº.
--p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
-æµè¯æºå¯ç ï¼å¨å±ï¼ -y PARALLEL, --parallel PARALLEL yes:
-è¡¨ç¤ºæææµè¯æºå¹¶è¡è·ï¼æ§è¡ç¸åçæµè¯ç¨ä¾;no:
-è¡¨ç¤ºæµè¯æºåå¸å¼æ§è¡ï¼æå¡ç«¯ä¼æ ¹æ®æ¶éå°çæµè¯ç¨ä¾èª
-å¨åéç»åä¸ªæµè¯æºæ§è¡ã ```
-é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼
-å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼ ```shell $ youqu manage.py remote -a apps/
-autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
-ææç¨ä¾æ§è¡å®ä¹åä¼å¨ `report`
-ç®å½ä¸åæ¶åä¸ªæµè¯æºæ§è¡çæµè¯æ¥åã
-æ³¨æï¼å¦æè¿ç¨æºå¨æ²¡ææ­å»ºèªå¨åæµè¯ç¯å¢ï¼è®°å¾å ä¸åæ°
-`-e` ï¼ ```shell $ youqu manage.py remote -a ... -e ```
-æ§è¡åç¡®ä¿è¿ç¨æºå¨å·²ç»å¼å¯äº ssh
-æå¡ï¼å¦åä¼æç¤ºæ æ³è¿æ¥ï¼å¦ææ²¡æå¼å¯ï¼è¯·æå¨å¼å¯ï¼
-```shell $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
-éç½®æä»¶å¶ä»ç¸å³éç½®é¡¹è¯¦ç»è¯´æï¼è¯·æ¥çéç½®æä»¶ä¸­çæ³¨éåå®¹ã
-## è´¡ç® [è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
-CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://
-github.com/linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã ------------
-[__Github Star History__]() [![Stargazers over time](https://starchart.cc/
-linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu) [__Gitee
-Info__]() [![deepin-community/youqu](https://gitee.com/deepin-community/youqu/
-widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)]
-(https://gitee.com/deepin-community/youqu)
+å½ä»¤è¡åæ° å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
+```shell $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
+``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-h` æ `--help` æ¥çã #### 2.2. éç½®æä»¶
+éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ [setting/globalconfig.ini]
+(https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)
+éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### 3. è¿ç¨æ§è¡
+è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åã
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## è´¡ç®
+[è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
+CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ YouQu å¨ [GPL-2.0](https://github.com/
+linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã
```

### Comparing `youqu-2.5.3/PKG-INFO` & `youqu-2.5.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: youqu
-Version: 2.5.3
+Version: 2.5.4
 Summary: youqu
 Project-URL: Source, https://github.com/linuxdeepin/youqu
 Project-URL: Documentation, https://linuxdeepin.github.io/youqu
 Author-email: mikigo <huangmingqiang@uniontech.com>
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <a href="https://linuxdeepin.github.io/youqu/">
-    <img src="./docs/logo.png" width="520" alt="YouQu">
+  <a href="https://linuxdeepin.github.io/youqu">
+    <img src="./docs/assets/logo.png" width="520" alt="YouQu">
   </a>
 </p>
 <p align="center">
     <em>YouQu（有趣），一个使用简单且功能强大的自动化测试基础框架。</em>
 </p>
 
 
 
+
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/pulls)
 [![GitHub Discussions](https://img.shields.io/github/discussions/linuxdeepin/youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/discussions)
 
 [![PyPI](https://img.shields.io/pypi/v/youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)](https://pypi.org/project/youqu/)
 ![PyPI - License](https://img.shields.io/pypi/l/youqu?color=%23F79431)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/youqu?color=%23F79431)
 ![Static Badge](https://img.shields.io/badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
 
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu/month)](https://pepy.tech/project/youqu)
 [![Downloads](https://static.pepy.tech/badge/youqu)](https://pepy.tech/project/youqu)
-
 [![Hits](https://hits.sh/github.com/linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://github.com/linuxdeepin/youqu)
 
 ---
 
 <a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
-<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a> | <a href="https://deepin-community.gitee.io/youqu/" target="_blank">在线文档（国内加速）</a>
+<a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
 
 ---
 
 YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
 
 ## YouQu（有趣）能做什么
 
@@ -85,196 +85,103 @@
 从 PyPI 安装:
 
 
 ```shell
 $ sudo pip3 install youqu
 ```
 
-创建项目:
+## 创建项目
+
+您可以在任意目录下，使用 `youqu-startproject` 命令创建一个项目：
 
 ```shell
 $ youqu-startproject my_project
 ```
 
 如果 `youqu-startproject` 后面不加参数，默认的项目名称为：`youqu` ；
 
-安装依赖:
+![](./docs/assets/install.gif)
+
+## 安装依赖
+
+安装部署 YouQu 执行所需环境： 
 
 ```shell
 $ cd my_project
-
-# 使用的默认密码是 1 ，您可以修改配置文件 setting/globalconfig.ini 里面的 PASSWORD 配置项
 $ bash env.sh
-
-# 也可以使用 -p 选项传入密码
-$ bash env.sh -p ${my_password}
 ```
 
-## 创建工程
+## 创建 APP 工程
 
-如果您已经有一个可用的 `APP` 工程，将应用库放到基础框架下 `apps` 目录下，像这样：
+使用 `startapp` 命令自动创建 APP 工程：
 
 ```shell
-my_project
-├── apps
-│   ├── autotest_deepin_music  # 应用库
-...
+$ youqu manage.py startapp autotest_deepin_some
 ```
 
-如果您还没有 `APP` 工程，建议使用框架提供的脚手架功能创建一个全新的 `APP` 工程。
+自动创建的 APP 工程遵循完整的 PO 设计模式，让你可以专注于用例和方法的编写维护。
 
-**创建一个 APP 工程**
+在 `apps` 目录下会自动创建一个 APP 工程：`autotest_deepin_some`，同时新建好工程模板目录和模板文件：
 
 ```shell
-$ youqu manage.py startapp autotest_deepin_some
+my_project
+├── apps
+│   ├── autotest_deepin_some  # <----- APP 工程
+...     ├── ...
 ```
 
-这样在 `apps` 目录下会创建一个子项目工程 `autotest_deepin_some`，同时新建好工程模板目录和模板文件：
+在你的远程 Git 仓库中，只需要保存 APP 工程这部分代码即可。
 
-```shell
-apps
-└── autotest_deepin_some
-    ├── case
-    │   ├── assert_res
-    │   │   └── readme
-    │   ├── base_case.py
-    │   └── __init__.py
-    ├── config.ini
-    ├── config.py
-    ├── conftest.py
-    ├── control
-    ├── deepin_some_assert.py
-    ├── deepin_some.csv
-    ├── __init__.py
-    └── widget
-        ├── base_widget.py
-        ├── case_res
-        │   └── readme
-        ├── deepin_some_widget.py
-        ├── __init__.py
-        ├── other.ini
-        ├── other_widget.py
-        ├── pic_res
-        │   └── readme
-        └── ui.ini
-```
-
-`autotest_deepin_some` 是你的工程名称，比如：`autotest_deepin_music` ；
+`autotest_deepin_some` 是你的  APP 工程名称，在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
 
-在此基础上，你可以快速的开始你的 AT 项目，更重要的是确保创建工程的规范性。
+`apps` 目录下可以存在任意多个 APP 工程。
 
 运行
 -------
 
-### 1. 工作空间
+### 1. 执行管理器
 
 在项目根目录下有一个 `manage.py` ，它是一个执行器入口，提供了本地执行、远程执行等的功能。
 
 ### 2. 本地执行
 
 
 ```shell
 $ youqu manage.py run
 ```
 
 #### 2.1. 命令行参数
 
-通过命令行参数配置参数，使用 `-h` 或 `--help` 可以查看所有支持的命令行参数：
-
-
-```shell
-$ youqu manage.py run -h
-```
-
 在一些 CI 环境下使用命令行参数会更加方便：
 
 
 ```shell
-$ youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags "xxx"
+$ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
 ```
 
-更多参数请查看【[命令行参数](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)】
+更多用法可以使用 `-h` 或 `--help` 查看。
 
 #### 2.2. 配置文件
 
 通过配置文件配置参数
 
-在配置文件 `setting/globalconfig.ini` 里面支持配置对执行的一些参数进行配置，配置完成之后，直接在命令行执行 `manage.py` 就好了。
-
-详细配置项请查看【[配置项](https://linuxdeepin.github.io/youqu/%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)】
+在配置文件 [setting/globalconfig.ini](https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)  里面支持配置对执行的一些参数进行配置。
 
 ### 3. 远程执行
 
-远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同；
+远程执行就是用本地作为服务端控制远程机器执行，远程机器执行的用例相同。
 
 使用 `remote` 命令：
 
 
 ```shell
 $ youqu manage.py remote
 ```
 
-以下为 `remote` 提供的一些参数选项：
-
-```coffeescript
-  -h, --help            show this help message and exit
-  -c CLIENTS, --clients CLIENTS
-                        远程机器的user@ip:password,多个机器用'/'连接,如果password不传入,默认取sett
-                        ing/remote.ini中CLIENT_PASSWORD的值,比如: uos@10.8.13.xx:1
-                        或 uos@10.8.13.xx
-  -s, --send_code       发送代码到测试机（不含report目录）
-  -e, --build_env       搭建测试环境,如果为yes，不管send_code是否为yes都会发送代码到测试机.
-  -p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
-                        测试机密码（全局）
-  -y PARALLEL, --parallel PARALLEL
-                        yes:表示所有测试机并行跑，执行相同的测试用例;no:表示测试机分布式执行，服务端会根据收集到的测试用例自
-                        动分配给各个测试机执行。
-```
-
-除了这些特有参数以外，它同样支持本地执行的所有参数；
-
-在命令行这样运行：
-
-
-```shell
-$ youqu manage.py remote -a apps/autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx"
-```
-
-所有用例执行完之后会在 `report` 目录下回收各个测试机执行的测试报告。
-
-注意：如果远程机器没有搭建自动化测试环境，记得加上参数 `-e` ：
-
-
-```shell
-$ youqu manage.py remote -a ... -e
-```
-
-执行前确保远程机器已经开启了 ssh 服务，否则会提示无法连接，如果没有开启，请手动开启：
-
-
-```shell
-$ sudo systemctl restart ssh
-$ sudo systemctl enable ssh
-```
-
-配置文件其他相关配置项详细说明，请查看配置文件中的注释内容。
-
 ## 贡献
 
 [贡献文档](https://github.com/linuxdeepin/youqu/blob/master/CONTRIBUTING.md) 
 
 
 ## 开源许可证
 
-有趣 在 [GPL-2.0-only](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
-
-------------
-
-[__Github Star History__]()
-
-[![Stargazers over time](https://starchart.cc/linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu)
-
-
-
-[__Gitee Info__]()
-
-[![deepin-community/youqu](https://gitee.com/deepin-community/youqu/widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)](https://gitee.com/deepin-community/youqu)
+YouQu 在 [GPL-2.0](https://github.com/linuxdeepin/youqu/blob/master/LICENSE) 下发布。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.5.3 Summary: youqu Project-URL:
+Metadata-Version: 2.1 Name: youqu Version: 2.5.4 Summary: youqu Project-URL:
 Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
 //linuxdeepin.github.io/youqu Author-email: mikigo
 uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
@@ -20,16 +20,15 @@
 pypi/pyversions/youqu?color=%23F79431) ![Static Badge](https://img.shields.io/
 badge/UOS%2FDeepin/Ubuntu/Debian-Platform?style=flat&label=OS&color=%23F79431)
 [![Downloads](https://static.pepy.tech/badge/youqu/week)](https://pepy.tech/
 project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
 (https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
 youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
 linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
-github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ |
-_å__¨_ç_º_¿_æ___æ_¡_£_ï_¼__å__½_å___å__ _é___ï_¼_ --
+github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --
 - YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
 X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ##
 YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] Linux æ¡é¢åºç¨ UI èªå¨åæµè¯ - [x]
 Linux æ¡é¢åºç¨ DBus/Gsettings æ¥å£èªå¨åæµè¯ - [x]
 å½ä»¤è¡èªå¨åæµè¯ - [x] HTTP æ¥å£èªå¨åæµè¯ - [x] Web UI
 èªå¨åæµè¯ - [ ] Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯
@@ -54,85 +53,40 @@
     * æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ãPMS
       æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
     * æ¯æåºäºæ·±åº¦å­¦ä¹ ç OCR
       åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼
     * å®ç¾å¼å®¹ Wayland å X11ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼
     * æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
     * æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼
-## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` åå»ºé¡¹ç®:
-```shell $ youqu-startproject my_project ``` å¦æ `youqu-startproject`
-åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu` ï¼ å®è£ä¾èµ:
-```shell $ cd my_project # ä½¿ç¨çé»è®¤å¯ç æ¯ 1
-ï¼æ¨å¯ä»¥ä¿®æ¹éç½®æä»¶ setting/globalconfig.ini éé¢ç PASSWORD
-éç½®é¡¹ $ bash env.sh # ä¹å¯ä»¥ä½¿ç¨ -p éé¡¹ä¼ å¥å¯ç  $ bash env.sh -
-p ${my_password} ``` ## åå»ºå·¥ç¨ å¦ææ¨å·²ç»æä¸ä¸ªå¯ç¨ç `APP`
-å·¥ç¨ï¼å°åºç¨åºæ¾å°åºç¡æ¡æ¶ä¸ `apps` ç®å½ä¸ï¼åè¿æ ·ï¼
-```shell my_project âââ apps â âââ autotest_deepin_music #
-åºç¨åº ... ``` å¦ææ¨è¿æ²¡æ `APP`
-å·¥ç¨ï¼å»ºè®®ä½¿ç¨æ¡æ¶æä¾çèææ¶åè½åå»ºä¸ä¸ªå¨æ°ç `APP`
-å·¥ç¨ã **åå»ºä¸ä¸ª APP å·¥ç¨** ```shell $ youqu manage.py startapp
-autotest_deepin_some ``` è¿æ ·å¨ `apps`
-ç®å½ä¸ä¼åå»ºä¸ä¸ªå­é¡¹ç®å·¥ç¨
-`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
-```shell apps âââ autotest_deepin_some Â Â  âââ case Â Â  âÂ Â 
-âââ assert_res Â Â  âÂ Â  âÂ Â  âââ readme Â Â  âÂ Â 
-âââ base_case.py Â Â  âÂ Â  âââ __init__.py Â Â  âââ
-config.ini Â Â  âââ config.py Â Â  âââ conftest.py Â Â  âââ
-control Â Â  âââ deepin_some_assert.py Â Â  âââ deepin_some.csv
-Â Â  âââ __init__.py Â Â  âââ widget Â Â  âââ base_widget.py
-Â Â  âââ case_res Â Â  âÂ Â  âââ readme Â Â  âââ
-deepin_some_widget.py Â Â  âââ __init__.py Â Â  âââ other.ini Â Â 
-âââ other_widget.py Â Â  âââ pic_res Â Â  âÂ Â  âââ readme
-Â Â  âââ ui.ini ``` `autotest_deepin_some`
-æ¯ä½ çå·¥ç¨åç§°ï¼æ¯å¦ï¼`autotest_deepin_music` ï¼
-å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
-é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã è¿è¡ ------- ### 1.
-å·¥ä½ç©ºé´ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
+## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` ##
+åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
+å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ``` å¦æ
+`youqu-startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu`
+ï¼ ![](./docs/assets/install.gif) ## å®è£ä¾èµ å®è£é¨ç½² YouQu
+æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
+å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
+manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
+å·¥ç¨éµå¾ªå®æ´ç PO
+è®¾è®¡æ¨¡å¼ï¼è®©ä½ å¯ä»¥ä¸æ³¨äºç¨ä¾åæ¹æ³çç¼åç»´æ¤ã å¨
+`apps` ç®å½ä¸ä¼èªå¨åå»ºä¸ä¸ª APP
+å·¥ç¨ï¼`autotest_deepin_some`ï¼åæ¶æ°å»ºå¥½å·¥ç¨æ¨¡æ¿ç®å½åæ¨¡æ¿æä»¶ï¼
+```shell my_project âââ apps â âââ autotest_deepin_some # <----
+- APP å·¥ç¨ ... Â Â  âââ ... ``` å¨ä½ çè¿ç¨ Git
+ä»åºä¸­ï¼åªéè¦ä¿å­ APP å·¥ç¨è¿é¨åä»£ç å³å¯ã
+`autotest_deepin_some` æ¯ä½ ç APP
+å·¥ç¨åç§°ï¼å¨æ­¤åºç¡ä¸ï¼ä½ å¯ä»¥å¿«éçå¼å§ä½ ç AT
+é¡¹ç®ï¼æ´éè¦çæ¯ç¡®ä¿åå»ºå·¥ç¨çè§èæ§ã `apps`
+ç®å½ä¸å¯ä»¥å­å¨ä»»æå¤ä¸ª APP å·¥ç¨ã è¿è¡ ------- ### 1.
+æ§è¡ç®¡çå¨ å¨é¡¹ç®æ ¹ç®å½ä¸æä¸ä¸ª `manage.py`
 ï¼å®æ¯ä¸ä¸ªæ§è¡å¨å¥å£ï¼æä¾äºæ¬å°æ§è¡ãè¿ç¨æ§è¡ç­çåè½ã
 ### 2. æ¬å°æ§è¡ ```shell $ youqu manage.py run ``` #### 2.1.
-å½ä»¤è¡åæ° éè¿å½ä»¤è¡åæ°éç½®åæ°ï¼ä½¿ç¨ `-h` æ `--help`
-å¯ä»¥æ¥çæææ¯æçå½ä»¤è¡åæ°ï¼ ```shell $ youqu manage.py run -
-h ``` å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼ ```shell $
-youqu manage.py run --app apps/autotest_deepin_music --keywords "xxx" --tags
-"xxx" ``` æ´å¤åæ°è¯·æ¥çã[å½ä»¤è¡åæ°](https://
-linuxdeepin.github.io/youqu/
-%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
-%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#21)ã #### 2.2. éç½®æä»¶
-éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ `setting/globalconfig.ini`
-éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ï¼éç½®å®æä¹åï¼ç´æ¥å¨å½ä»¤è¡æ§è¡
-`manage.py` å°±å¥½äºã è¯¦ç»éç½®é¡¹è¯·æ¥çã[éç½®é¡¹](https://
-linuxdeepin.github.io/youqu/
-%E6%A1%86%E6%9E%B6%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D/
-%E6%89%A7%E8%A1%8C%E7%AE%A1%E7%90%86%E5%99%A8/#22)ã ### 3. è¿ç¨æ§è¡
-è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åï¼
-ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ä»¥ä¸ä¸º
-`remote` æä¾çä¸äºåæ°éé¡¹ï¼ ```coffeescript -h, --help show this
-help message and exit -c CLIENTS, --clients CLIENTS è¿ç¨æºå¨çuser@ip:
-password,å¤ä¸ªæºå¨ç¨'/'è¿æ¥,å¦æpasswordä¸ä¼ å¥,é»è®¤åsett ing/
-remote.iniä¸­CLIENT_PASSWORDçå¼,æ¯å¦: uos@10.8.13.xx:1 æ uos@10.8.13.xx
--s, --send_code åéä»£ç å°æµè¯æºï¼ä¸å«reportç®å½ï¼ -e, --
-build_env
-æ­å»ºæµè¯ç¯å¢,å¦æä¸ºyesï¼ä¸ç®¡send_codeæ¯å¦ä¸ºyesé½ä¼åéä»£ç å°æµè¯æº.
--p CLIENT_PASSWORD, --client_password CLIENT_PASSWORD
-æµè¯æºå¯ç ï¼å¨å±ï¼ -y PARALLEL, --parallel PARALLEL yes:
-è¡¨ç¤ºæææµè¯æºå¹¶è¡è·ï¼æ§è¡ç¸åçæµè¯ç¨ä¾;no:
-è¡¨ç¤ºæµè¯æºåå¸å¼æ§è¡ï¼æå¡ç«¯ä¼æ ¹æ®æ¶éå°çæµè¯ç¨ä¾èª
-å¨åéç»åä¸ªæµè¯æºæ§è¡ã ```
-é¤äºè¿äºç¹æåæ°ä»¥å¤ï¼å®åæ ·æ¯ææ¬å°æ§è¡çææåæ°ï¼
-å¨å½ä»¤è¡è¿æ ·è¿è¡ï¼ ```shell $ youqu manage.py remote -a apps/
-autotest_deepin_music -c uos@10.8.13.x3/uos@10.8.13.x4 -k "xxx" -t "xxx" ```
-ææç¨ä¾æ§è¡å®ä¹åä¼å¨ `report`
-ç®å½ä¸åæ¶åä¸ªæµè¯æºæ§è¡çæµè¯æ¥åã
-æ³¨æï¼å¦æè¿ç¨æºå¨æ²¡ææ­å»ºèªå¨åæµè¯ç¯å¢ï¼è®°å¾å ä¸åæ°
-`-e` ï¼ ```shell $ youqu manage.py remote -a ... -e ```
-æ§è¡åç¡®ä¿è¿ç¨æºå¨å·²ç»å¼å¯äº ssh
-æå¡ï¼å¦åä¼æç¤ºæ æ³è¿æ¥ï¼å¦ææ²¡æå¼å¯ï¼è¯·æå¨å¼å¯ï¼
-```shell $ sudo systemctl restart ssh $ sudo systemctl enable ssh ```
-éç½®æä»¶å¶ä»ç¸å³éç½®é¡¹è¯¦ç»è¯´æï¼è¯·æ¥çéç½®æä»¶ä¸­çæ³¨éåå®¹ã
-## è´¡ç® [è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
-CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ æè¶£ å¨ [GPL-2.0-only](https://
-github.com/linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã ------------
-[__Github Star History__]() [![Stargazers over time](https://starchart.cc/
-linuxdeepin/youqu.svg)](https://starchart.cc/linuxdeepin/youqu) [__Gitee
-Info__]() [![deepin-community/youqu](https://gitee.com/deepin-community/youqu/
-widgets/widget_card.svg?colors=4183c4,ffffff,ffffff,e3e9ed,666666,9b9b9b)]
-(https://gitee.com/deepin-community/youqu)
+å½ä»¤è¡åæ° å¨ä¸äº CI ç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åæ°ä¼æ´å æ¹ä¾¿ï¼
+```shell $ youqu manage.py run -a apps/autotest_deepin_some -k "xxx" -t "yyy"
+``` æ´å¤ç¨æ³å¯ä»¥ä½¿ç¨ `-h` æ `--help` æ¥çã #### 2.2. éç½®æä»¶
+éè¿éç½®æä»¶éç½®åæ° å¨éç½®æä»¶ [setting/globalconfig.ini]
+(https://github.com/linuxdeepin/youqu/blob/master/setting/globalconfig.ini)
+éé¢æ¯æéç½®å¯¹æ§è¡çä¸äºåæ°è¿è¡éç½®ã ### 3. è¿ç¨æ§è¡
+è¿ç¨æ§è¡å°±æ¯ç¨æ¬å°ä½ä¸ºæå¡ç«¯æ§å¶è¿ç¨æºå¨æ§è¡ï¼è¿ç¨æºå¨æ§è¡çç¨ä¾ç¸åã
+ä½¿ç¨ `remote` å½ä»¤ï¼ ```shell $ youqu manage.py remote ``` ## è´¡ç®
+[è´¡ç®ææ¡£](https://github.com/linuxdeepin/youqu/blob/master/
+CONTRIBUTING.md) ## å¼æºè®¸å¯è¯ YouQu å¨ [GPL-2.0](https://github.com/
+linuxdeepin/youqu/blob/master/LICENSE) ä¸åå¸ã
```

