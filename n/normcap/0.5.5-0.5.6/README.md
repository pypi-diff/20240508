# Comparing `tmp/normcap-0.5.5.tar.gz` & `tmp/normcap-0.5.6.tar.gz`

## Comparing `normcap-0.5.5.tar` & `normcap-0.5.6.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 normcap-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    19808 2020-02-02 00:00:00.000000 normcap-0.5.5/CHANGELOG
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 normcap-0.5.5/mkdocs.yml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 normcap-0.5.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 normcap-0.5.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 normcap-0.5.5/.github/ISSUE_TEMPLATE/detection_quality.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 normcap-0.5.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 normcap-0.5.5/.github/workflows/cicd.yaml
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/001-choose-transparent-windows-as-main-gui.md
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/002-choose-windows-with-screenshots-as-main-gui.md
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/003-use-system-tray-as-main-application.md
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/004-do-not-implement-hotkey.md
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/005-use-hatch-instead-poetry.md
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/006-use-jeepney-for-dbus-calls.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 normcap-0.5.5/adr/README.md
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/build.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/deps.py
--rwxr-xr-x   0        0        0     4854 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/l10n.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/metainfo
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-128.png
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-16.png
--rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-256.png
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-32.png
--rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-512.png
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap-64.png
--rw-r--r--   0        0        0   160026 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap.icns
--rw-r--r--   0        0        0   206511 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap.ico
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap.svg
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install.bmp
--rw-r--r--   0        0        0    29592 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install.icns
--rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install.png
--rw-r--r--   0        0        0    29784 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install.svg
--rw-r--r--   0        0        0   615402 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install_bg.bmp
--rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install_bg.png
--rw-r--r--   0        0        0    24064 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install_bg.svg
--rw-r--r--   0        0        0   114514 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/imgs/normcap_install_top.bmp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/platforms/__init__.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/platforms/linux_briefcase.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/platforms/macos_briefcase.py
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/platforms/utils.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 normcap-0.5.5/bundle/platforms/windows_briefcase.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.5/docs/contribute.md
--rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 normcap-0.5.5/docs/faqs.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 normcap-0.5.5/docs/index.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 normcap-0.5.5/docs/support.md
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 normcap-0.5.5/docs/usage.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/__main__.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/app.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/utils.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/main.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/structures.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/pbcopy.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/qtclipboard.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/windll.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/wlclipboard.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/xclip.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/clipboard/handlers/xsel.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/__init__.py
--rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/constants.py
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/dbus.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/downloader.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/introduction.py
--rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/localization.py
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/models.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/notification.py
--rw-r--r--   0        0        0   312761 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/resources.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/settings.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/system_info.py
--rw-r--r--   0        0        0    24259 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/tray.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/update_check.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/utils.py
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/gui/window.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/enhance.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/structures.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/tesseract.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformer.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/__init__.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/email.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/multi_line.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/paragraph.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/single_line.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/url.py
--rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/ocr/transformers/url_tlds.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/tray_done.png
--rw-r--r--   0        0        0    16316 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/icons/tray_processing.png
--rw-r--r--   0        0        0   145973 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/darwin-intro-1.png
--rw-r--r--   0        0        0   148696 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/darwin-intro-2.png
--rw-r--r--   0        0        0    98495 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/darwin-intro-3.png
--rw-r--r--   0        0        0   139526 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/darwin-intro-4.png
--rw-r--r--   0        0        0   455444 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/linux-intro-1.png
--rw-r--r--   0        0        0   466217 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/linux-intro-2.png
--rw-r--r--   0        0        0   299322 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/linux-intro-3.png
--rw-r--r--   0        0        0   399984 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/linux-intro-4.png
--rw-r--r--   0        0        0   415812 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/win32-intro-1.png
--rw-r--r--   0        0        0   425024 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/win32-intro-2.png
--rw-r--r--   0        0        0   267555 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/win32-intro-3.png
--rw-r--r--   0        0        0   408697 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/images/win32-intro-4.png
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/README.md
--rw-r--r--   0        0        0    12682 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/messages.pot
--rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    10179 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    10525 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/main.py
--rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/permissions.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/post_processing.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/structures.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/handlers/__init__.py
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/handlers/dbus_portal.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/handlers/dbus_shell.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/handlers/grim.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 normcap-0.5.5/normcap/screengrab/handlers/qt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/conftest.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/test_app.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/test_main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/test_normcap.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/test_settings_menu.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/test_tray_menu.py
--rw-r--r--   0        0        0    37267 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/00_parse_urls.png
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/01_parse_colored_url.png
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/02_detect_window_title.png
--rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/03_parse_emails.png
--rw-r--r--   0        0        0    61232 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/04_parse_email_skip_invalid.png
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/05_detect_text_with_low_contrast.png
--rw-r--r--   0        0        0    33416 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/06_detect_special_characters.png
--rw-r--r--   0        0        0   152224 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/07_parse_paragraphs_of_text.png
--rw-r--r--   0        0        0   168233 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/08_paragraphs.png
--rw-r--r--   0        0        0   277892 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/09_two_columns.png
--rw-r--r--   0        0        0    95751 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/10_font_sizes.png
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/11_paragraph_with_bullet_points.png
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/12_not_a_url.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/__init__.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/integration/testcases/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_main.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/__init__.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/test_pbcopy.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/test_qtclipboard.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/test_windll.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/test_wlclipboard.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_clipboard/test_handlers/test_xclip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_constants.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_downloader.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_introduction.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_language_manager.py
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_loading_indicator.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_menu_button.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_models.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_notification.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_resources.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_settings.py
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_system_info.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_tray.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_update_check.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_utils.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_gui/test_window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/__init__.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/test_enhance.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/test_recognize.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/test_structures.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/test_tesseract.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/test_transformer.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testcases/00_eng.png
--rw-r--r--   0        0        0    26208 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testcases/01_chi_sim.png
--rw-r--r--   0        0        0    20815 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testcases/02_jpn.png
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testcases/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testcases/data.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testimages/color.png
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testimages/dark.png
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/testimages/light.png
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/transformers/test_email.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/transformers/test_paragraph.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/transformers/test_single_line.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_ocr/transformers/test_url.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/split_full_desktop_to_screens.png
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_main.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_permissions.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_post_processing.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_system_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_handlers/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_handlers/test_dbus_portal.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_handlers/test_grim.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 normcap-0.5.5/tests/tests_screengrab/test_handlers/test_qt.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 normcap-0.5.5/.gitignore
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 normcap-0.5.5/LICENSE
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 normcap-0.5.5/README.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 normcap-0.5.5/hatch_build.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 normcap-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 normcap-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 normcap-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20040 2020-02-02 00:00:00.000000 normcap-0.5.6/CHANGELOG
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 normcap-0.5.6/mkdocs.yml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/detection_quality.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0    10582 2020-02-02 00:00:00.000000 normcap-0.5.6/.github/workflows/cicd.yaml
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/001-choose-transparent-windows-as-main-gui.md
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/002-choose-windows-with-screenshots-as-main-gui.md
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/003-use-system-tray-as-main-application.md
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/004-do-not-implement-hotkey.md
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/005-use-hatch-instead-poetry.md
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/006-use-jeepney-for-dbus-calls.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 normcap-0.5.6/adr/README.md
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/build.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/deps.py
+-rwxr-xr-x   0        0        0     4854 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/l10n.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/metainfo
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-128.png
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-16.png
+-rw-r--r--   0        0        0    26067 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-256.png
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-32.png
+-rw-r--r--   0        0        0    45156 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-512.png
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap-64.png
+-rw-r--r--   0        0        0   160026 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.icns
+-rw-r--r--   0        0        0   206511 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.ico
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap.svg
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.bmp
+-rw-r--r--   0        0        0    29592 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.icns
+-rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.png
+-rw-r--r--   0        0        0    29784 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install.svg
+-rw-r--r--   0        0        0   615402 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.bmp
+-rw-r--r--   0        0        0    12552 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.png
+-rw-r--r--   0        0        0    24064 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_bg.svg
+-rw-r--r--   0        0        0   114514 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/imgs/normcap_install_top.bmp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/__init__.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/linux_briefcase.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/macos_briefcase.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/utils.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 normcap-0.5.6/bundle/platforms/windows_briefcase.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/contribute.md
+-rw-r--r--   0        0        0    17691 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/faqs.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/index.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/support.md
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 normcap-0.5.6/docs/usage.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/__main__.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/app.py
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/utils.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/main.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/structures.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/pbcopy.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/qtclipboard.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/windll.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/wlclipboard.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/xclip.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/clipboard/handlers/xsel.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     7955 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/constants.py
+-rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/dbus.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/introduction.py
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/localization.py
+-rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/models.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/notification.py
+-rw-r--r--   0        0        0   312761 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/resources.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    24259 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/tray.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/utils.py
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/gui/window.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/structures.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformer.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/__init__.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/email.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/multi_line.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/paragraph.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/single_line.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/url.py
+-rw-r--r--   0        0        0     9831 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/ocr/transformers/url_tlds.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    15317 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16742 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray_done.png
+-rw-r--r--   0        0        0    16316 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/icons/tray_processing.png
+-rw-r--r--   0        0        0   145973 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-1.png
+-rw-r--r--   0        0        0   148696 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-2.png
+-rw-r--r--   0        0        0    98495 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-3.png
+-rw-r--r--   0        0        0   139526 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/darwin-intro-4.png
+-rw-r--r--   0        0        0   455444 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-1.png
+-rw-r--r--   0        0        0   466217 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-2.png
+-rw-r--r--   0        0        0   299322 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-3.png
+-rw-r--r--   0        0        0   399984 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/linux-intro-4.png
+-rw-r--r--   0        0        0   415812 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-1.png
+-rw-r--r--   0        0        0   425024 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-2.png
+-rw-r--r--   0        0        0   267555 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-3.png
+-rw-r--r--   0        0        0   408697 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/images/win32-intro-4.png
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/README.md
+-rw-r--r--   0        0        0    12682 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/messages.pot
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/main.py
+-rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/permissions.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/post_processing.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/structures.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/__init__.py
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/dbus_portal.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/dbus_shell.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/grim.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 normcap-0.5.6/normcap/screengrab/handlers/qt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/conftest.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_app.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_normcap.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_settings_menu.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/test_tray_menu.py
+-rw-r--r--   0        0        0    37267 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/00_parse_urls.png
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/01_parse_colored_url.png
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/02_detect_window_title.png
+-rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/03_parse_emails.png
+-rw-r--r--   0        0        0    61232 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/04_parse_email_skip_invalid.png
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/05_detect_text_with_low_contrast.png
+-rw-r--r--   0        0        0    33416 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/06_detect_special_characters.png
+-rw-r--r--   0        0        0   152224 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/07_parse_paragraphs_of_text.png
+-rw-r--r--   0        0        0   168233 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/08_paragraphs.png
+-rw-r--r--   0        0        0   277892 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/09_two_columns.png
+-rw-r--r--   0        0        0    95751 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/10_font_sizes.png
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/11_paragraph_with_bullet_points.png
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/12_not_a_url.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/__init__.py
+-rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/integration/testcases/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_main.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/__init__.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_pbcopy.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_qtclipboard.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_windll.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_wlclipboard.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_clipboard/test_handlers/test_xclip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_constants.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_downloader.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_introduction.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_language_manager.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_loading_indicator.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_menu_button.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_models.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_notification.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_resources.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_settings.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_system_info.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_tray.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_update_check.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_utils.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_gui/test_window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/__init__.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_enhance.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_recognize.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_structures.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_tesseract.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/test_transformer.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/00_eng.png
+-rw-r--r--   0        0        0    26208 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/01_chi_sim.png
+-rw-r--r--   0        0        0    20815 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/02_jpn.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testcases/data.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/color.png
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/dark.png
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/testimages/light.png
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_email.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_paragraph.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_single_line.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_ocr/transformers/test_url.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/split_full_desktop_to_screens.png
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_main.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_permissions.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_post_processing.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_system_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_dbus_portal.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_grim.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 normcap-0.5.6/tests/tests_screengrab/test_handlers/test_qt.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 normcap-0.5.6/.gitignore
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 normcap-0.5.6/LICENSE
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 normcap-0.5.6/README.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 normcap-0.5.6/hatch_build.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 normcap-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 normcap-0.5.6/PKG-INFO
```

### Comparing `normcap-0.5.5/.pre-commit-config.yaml` & `normcap-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/CHANGELOG` & `normcap-0.5.6/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 <!-- vim: syntax=Markdown -->
 
 # Changelog
 
+## v0.5.6 (2024-05-08)
+
+- All: Fix minor typos in translations. ([#641](https://github.com/dynobo/normcap/pull/641))
+- Linux: Fix clipboard on Wayland desktops other than GNOME. ([#640](https://github.com/dynobo/normcap/pull/640))
+
 ## v0.5.5 (2024-05-07)
 
 - All: Add ukrainian translation. Thanks, [@thevllad](https://github.com/thevllad)! ([#625](https://github.com/dynobo/normcap/pull/625))
 - All: Add russian translation. Thanks, [@ViktorOn](https://github.com/ViktorOn)! ([#611](https://github.com/dynobo/normcap/pull/611))
 - All: Add italian translation. Thanks, [@albanobattistella](https://github.com/albanobattistella)! ([#622](https://github.com/dynobo/normcap/pull/622))
 - All: Add spanish translation. Thanks, [@haggen88](https://github.com/haggen88)! ([#614](https://github.com/dynobo/normcap/pull/614))
 - All: Add brazilian translation. Thanks, [@NameLessGO](https://github.com/NameLessGo)! ([#632](https://github.com/dynobo/normcap/pull/632))
```

### Comparing `normcap-0.5.5/mkdocs.yml` & `normcap-0.5.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `normcap-0.5.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/.github/ISSUE_TEMPLATE/detection_quality.yml` & `normcap-0.5.6/.github/ISSUE_TEMPLATE/detection_quality.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `normcap-0.5.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/.github/workflows/cicd.yaml` & `normcap-0.5.6/.github/workflows/cicd.yaml`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/001-choose-transparent-windows-as-main-gui.md` & `normcap-0.5.6/adr/001-choose-transparent-windows-as-main-gui.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/002-choose-windows-with-screenshots-as-main-gui.md` & `normcap-0.5.6/adr/002-choose-windows-with-screenshots-as-main-gui.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/003-use-system-tray-as-main-application.md` & `normcap-0.5.6/adr/003-use-system-tray-as-main-application.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/004-do-not-implement-hotkey.md` & `normcap-0.5.6/adr/004-do-not-implement-hotkey.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/005-use-hatch-instead-poetry.md` & `normcap-0.5.6/adr/005-use-hatch-instead-poetry.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/006-use-jeepney-for-dbus-calls.md` & `normcap-0.5.6/adr/006-use-jeepney-for-dbus-calls.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/adr/README.md` & `normcap-0.5.6/adr/README.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/build.py` & `normcap-0.5.6/bundle/build.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/deps.py` & `normcap-0.5.6/bundle/deps.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/l10n.py` & `normcap-0.5.6/bundle/l10n.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/metainfo` & `normcap-0.5.6/bundle/metainfo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-128.png` & `normcap-0.5.6/bundle/imgs/normcap-128.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-16.png` & `normcap-0.5.6/bundle/imgs/normcap-16.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-256.png` & `normcap-0.5.6/bundle/imgs/normcap-256.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-32.png` & `normcap-0.5.6/bundle/imgs/normcap-32.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-512.png` & `normcap-0.5.6/bundle/imgs/normcap-512.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap-64.png` & `normcap-0.5.6/bundle/imgs/normcap-64.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap.icns` & `normcap-0.5.6/bundle/imgs/normcap.icns`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap.ico` & `normcap-0.5.6/bundle/imgs/normcap.ico`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap.svg` & `normcap-0.5.6/bundle/imgs/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install.bmp` & `normcap-0.5.6/bundle/imgs/normcap_install.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install.icns` & `normcap-0.5.6/bundle/imgs/normcap_install.icns`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install.png` & `normcap-0.5.6/bundle/imgs/normcap_install.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install.svg` & `normcap-0.5.6/bundle/imgs/normcap_install.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install_bg.bmp` & `normcap-0.5.6/bundle/imgs/normcap_install_bg.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install_bg.png` & `normcap-0.5.6/bundle/imgs/normcap_install_bg.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install_bg.svg` & `normcap-0.5.6/bundle/imgs/normcap_install_bg.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/imgs/normcap_install_top.bmp` & `normcap-0.5.6/bundle/imgs/normcap_install_top.bmp`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/platforms/linux_briefcase.py` & `normcap-0.5.6/bundle/platforms/linux_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/platforms/macos_briefcase.py` & `normcap-0.5.6/bundle/platforms/macos_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/platforms/utils.py` & `normcap-0.5.6/bundle/platforms/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/bundle/platforms/windows_briefcase.py` & `normcap-0.5.6/bundle/platforms/windows_briefcase.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/docs/contribute.md` & `normcap-0.5.6/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/docs/faqs.md` & `normcap-0.5.6/docs/faqs.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/docs/index.md` & `normcap-0.5.6/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,29 @@
   - navigation
   - toc
 ---
 
 <div class="grid" markdown>
 
 <div markdown>
-# NormCap v0.5.5 {.md-title}
+# NormCap v0.5.6 {.md-title}
 
 <p class="md-subtitle">OCR-powered screenshot tool to capture text<br> instead of images.</p>
 
 Packages with the
 [latest changes](https://github.com/dynobo/normcap/blob/main/CHANGELOG) for your system:
 
 <div class="annotate" markdown>
-- [Download for **Windows**](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-Windows.msi)
+- [Download for **Windows**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
   <small>x86_64, ~120 MB</small>
-- [Download for **Linux**](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64.AppImage)
+- [Download for **Linux**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
   <small>x86_64, ~90 MB</small>
-- [Download for **macOS**](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-macOS.dmg)
+- [Download for **macOS**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
   <small>x86_64, ~80 MB</small>
-- [Download for **macOS (M1)**](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-arm64-macOS.dmg)
+- [Download for **macOS (M1)**](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
   <small>arm64, ~65 MB</small>
 </div>
 
 ... or install via
 [FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap),
 [AUR](https://aur.archlinux.org/packages/normcap) or
 [PyPi](https://pypi.org/project/normcap/).
```

### Comparing `normcap-0.5.5/docs/support.md` & `normcap-0.5.6/docs/support.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/docs/usage.md` & `normcap-0.5.6/docs/usage.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/app.py` & `normcap-0.5.6/normcap/app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/utils.py` & `normcap-0.5.6/normcap/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/main.py` & `normcap-0.5.6/normcap/clipboard/main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/structures.py` & `normcap-0.5.6/normcap/clipboard/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/system_info.py` & `normcap-0.5.6/normcap/clipboard/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/pbcopy.py` & `normcap-0.5.6/normcap/clipboard/handlers/pbcopy.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/qtclipboard.py` & `normcap-0.5.6/normcap/clipboard/handlers/qtclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/windll.py` & `normcap-0.5.6/normcap/clipboard/handlers/windll.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/wlclipboard.py` & `normcap-0.5.6/normcap/clipboard/handlers/wlclipboard.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         )
         return False
 
     if system_info.os_has_awesome_wm():
         logger.debug("%s is not compatible with Awesome WM", __name__)
         return False
 
-    gnome_version = system_info.get_gnome_version()
-    gnome_major = int(gnome_version.split(".")[0])
-    last_working_gnome_version = 44
-    if gnome_major > last_working_gnome_version:
-        logger.debug("%s is not compatible with Gnome %s", __name__, gnome_version)
-        return False
+    if gnome_version := system_info.get_gnome_version():
+        gnome_major = int(gnome_version.split(".")[0])
+        last_working_gnome_version = 44
+        if gnome_major > last_working_gnome_version:
+            logger.debug("%s is not compatible with Gnome %s", __name__, gnome_version)
+            return False
 
     logger.debug("%s is compatible", __name__)
     return True
 
 
 def is_installed() -> bool:
     if not (wl_copy_bin := shutil.which("wl-copy")):
```

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/xclip.py` & `normcap-0.5.6/normcap/clipboard/handlers/xclip.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/clipboard/handlers/xsel.py` & `normcap-0.5.6/normcap/clipboard/handlers/xsel.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/constants.py` & `normcap-0.5.6/normcap/gui/constants.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/dbus.py` & `normcap-0.5.6/normcap/gui/dbus.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/downloader.py` & `normcap-0.5.6/normcap/gui/downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/introduction.py` & `normcap-0.5.6/normcap/gui/introduction.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/language_manager.py` & `normcap-0.5.6/normcap/gui/language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/loading_indicator.py` & `normcap-0.5.6/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/menu_button.py` & `normcap-0.5.6/normcap/gui/menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/models.py` & `normcap-0.5.6/normcap/gui/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/notification.py` & `normcap-0.5.6/normcap/gui/notification.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/resources.py` & `normcap-0.5.6/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/settings.py` & `normcap-0.5.6/normcap/gui/settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/system_info.py` & `normcap-0.5.6/normcap/gui/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/tray.py` & `normcap-0.5.6/normcap/gui/tray.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/update_check.py` & `normcap-0.5.6/normcap/gui/update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/utils.py` & `normcap-0.5.6/normcap/gui/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/gui/window.py` & `normcap-0.5.6/normcap/gui/window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/enhance.py` & `normcap-0.5.6/normcap/ocr/enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/recognize.py` & `normcap-0.5.6/normcap/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/structures.py` & `normcap-0.5.6/normcap/ocr/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/tesseract.py` & `normcap-0.5.6/normcap/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformer.py` & `normcap-0.5.6/normcap/ocr/transformer.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/email.py` & `normcap-0.5.6/normcap/ocr/transformers/email.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/multi_line.py` & `normcap-0.5.6/normcap/ocr/transformers/multi_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/paragraph.py` & `normcap-0.5.6/normcap/ocr/transformers/paragraph.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/single_line.py` & `normcap-0.5.6/normcap/ocr/transformers/single_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/url.py` & `normcap-0.5.6/normcap/ocr/transformers/url.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/ocr/transformers/url_tlds.py` & `normcap-0.5.6/normcap/ocr/transformers/url_tlds.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/normcap.png` & `normcap-0.5.6/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/notification.png` & `normcap-0.5.6/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/parse.png` & `normcap-0.5.6/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/raw.png` & `normcap-0.5.6/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/resources.qrc` & `normcap-0.5.6/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/settings.png` & `normcap-0.5.6/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/tray.png` & `normcap-0.5.6/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/tray_done.png` & `normcap-0.5.6/normcap/resources/icons/tray_done.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/icons/tray_processing.png` & `normcap-0.5.6/normcap/resources/icons/tray_processing.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/darwin-intro-1.png` & `normcap-0.5.6/normcap/resources/images/darwin-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/darwin-intro-2.png` & `normcap-0.5.6/normcap/resources/images/darwin-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/darwin-intro-3.png` & `normcap-0.5.6/normcap/resources/images/darwin-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/darwin-intro-4.png` & `normcap-0.5.6/normcap/resources/images/darwin-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/linux-intro-1.png` & `normcap-0.5.6/normcap/resources/images/linux-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/linux-intro-2.png` & `normcap-0.5.6/normcap/resources/images/linux-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/linux-intro-3.png` & `normcap-0.5.6/normcap/resources/images/linux-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/linux-intro-4.png` & `normcap-0.5.6/normcap/resources/images/linux-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/win32-intro-1.png` & `normcap-0.5.6/normcap/resources/images/win32-intro-1.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/win32-intro-2.png` & `normcap-0.5.6/normcap/resources/images/win32-intro-2.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/win32-intro-3.png` & `normcap-0.5.6/normcap/resources/images/win32-intro-3.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/images/win32-intro-4.png` & `normcap-0.5.6/normcap/resources/images/win32-intro-4.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/README.md` & `normcap-0.5.6/normcap/resources/locales/README.md`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/messages.pot` & `normcap-0.5.6/normcap/resources/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/de_DE/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: de_DE\n"
-"Language-Team: de_DE <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language-Team: German <https://hosted.weblate.org/projects/normcap/ui/de/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "'{application}' is missing the permission for 'Screen Recording'.\n"
```

### Comparing `normcap-0.5.5/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/es_ES/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: NormCap 0.4.4\n"
 "Report-Msgid-Bugs-To: dynobo@mailbox.org\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: 2024-03-29 19:02-0300\n"
-"Last-Translator: \n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: es_ES\n"
-"Language-Team: es_ES <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/normcap/ui/es/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "'{application}' is missing the permission for 'Screen Recording'.\n"
@@ -290,15 +290,14 @@
 "GitHub.\n"
 "\n"
 "Do you want to visit the release website now?"
 msgstr ""
 "Puedes descargar la nueva versión de NormCap para tu sistema operativo desde "
 "GitHub.\n"
 "\n"
-"\n"
 "¿Quieres visitar la página web de la versión ahora?"
 
 msgid ""
 "You can upgrade NormCap via the command line, e.g. by running 'pip install "
 "normcap --upgrade'.\n"
 "\n"
 "Do you want to view the changelog on GitHub now?"
```

### Comparing `normcap-0.5.5/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/it_IT/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: NormCap 0.4.4\n"
 "Report-Msgid-Bugs-To: dynobo@mailbox.org\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: 2024-04-27 18:15+0100\n"
-"Last-Translator: Albano Battistella <albanobattistella@gmail.com>\n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: it_IT\n"
-"Language-Team: it_IT <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language-Team: Italian <https://hosted.weblate.org/projects/normcap/ui/it/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "'{application}' is missing the permission for 'Screen Recording'.\n"
@@ -81,15 +81,15 @@
 "<b>NormCap non dispone dell'autorizzazione per l'acquisizione dello schermo."
 "</b><br><br>Concedilatramite la finestra di dialogo che apparirà dopo aver "
 "fatto clic su 'Ok'.<br>Quindi avvia Di nuovo NormCap.<br><br><small>A volte, "
 "potrebbe non funzionare. Se questo ti interessa, per favore<br><a "
 "href='{issues_url}'>segnalalo come bug</a> su GitHub.</small>"
 
 msgid "About"
-msgstr "Informazioni"
+msgstr "Info su NormCap"
 
 msgid "Application"
 msgstr "Applicazioni"
 
 msgid "Available:"
 msgstr "Disponibile:"
 
@@ -240,15 +240,15 @@
 msgstr "Mostra all'avvio"
 
 msgid ""
 "Show status information via your system's desktop\n"
 "notification center."
 msgstr ""
 "Mostra informazioni sullo stato tramite il desktop del sistema\n"
-"centro notifiche\""
+"centro notifiche."
 
 msgid "Source code"
 msgstr "Codice sorgente"
 
 msgid ""
 "The detection result will be copied to your system's clipboard. Paste it "
 "into any application ({shortcut})."
```

### Comparing `normcap-0.5.5/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/pl_PL/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/pt_BR/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: pt_BR\n"
-"Language-Team: pt_BR <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
+"normcap/ui/pt_BR/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
 msgid ""
 "'{application}' is missing the permission for 'Screen Recording'.\n"
@@ -198,15 +199,15 @@
 "Open the menu using the gear icon in the upper right corner of corner your "
 "screen."
 msgstr ""
 "Abra o menu usando o ícone de engrenagem no canto superior direito do seu "
 "tela."
 
 msgid "Please try again."
-msgstr "Por favor, tente novamente"
+msgstr "Por favor, tente novamente."
 
 msgid ""
 "Processing takes time. Wait for a notification or a color change of the "
 "system tray icon."
 msgstr ""
 "O processamento leva tempo. Aguarde uma notificação ou uma mudança de cor do "
 "ícone da bandeja do sistema."
```

### Comparing `normcap-0.5.5/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/pt_PT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/ru_RU/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: 2024-03-19 12:00+0200\n"
-"Last-Translator: Victor <k3kelm4vw@mozmail.com>\n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: ru_RU\n"
-"Language-Team: ru_RU <LL@li.org>\n"
+"Language-Team: Russian <https://hosted.weblate.org/projects/normcap/ui/ru/>\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
@@ -265,15 +265,15 @@
 msgid ""
 "This installation of NormCap uses the Tesseract binary installed on your "
 "system. To install additional languages, please refer to the documentation "
 "of that Tesseract installation."
 msgstr ""
 "Эта установка NormCap использует двоичный файл Tesseract, установленный в "
 "вашей системе. Чтобы установить дополнительные языки, пожалуйста, обратитесь "
-"к документации по установке Tesseract"
+"к документации по установке Tesseract."
 
 msgid ""
 "Tries to determine the text's type (e.g. line,\n"
 "paragraph, URL, email) and formats the output\n"
 "accordingly.\n"
 "If the result is unexpected, try 'raw' mode instead."
 msgstr ""
@@ -308,14 +308,15 @@
 "normcap --upgrade'.\n"
 "\n"
 "Do you want to view the changelog on GitHub now?"
 msgstr ""
 "Вы можете обновить NormCap через командную строку, например, запустив «pip "
 "install normcap --upgrade».\n"
 "\n"
+"Хотите просмотреть журнал изменений на GitHub прямо сейчас?"
 
 msgid "You have v{version}"
 msgstr "У вас v{version}"
 
 msgid "add/remove..."
 msgstr "добавить/удалить..."
```

### Comparing `normcap-0.5.5/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/uk_UA/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: NormCap 0.4.4\n"
 "Report-Msgid-Bugs-To: dynobo@mailbox.org\n"
 "POT-Creation-Date: 2024-05-06 21:18+0200\n"
-"PO-Revision-Date: 2023-10-08 12:16+0200\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"PO-Revision-Date: 2024-05-08 12:08+0000\n"
+"Last-Translator: dynobo <dynobo@mailbox.org>\n"
 "Language: uk_UA\n"
-"Language-Team: uk_UA <LL@li.org>\n"
+"Language-Team: Ukrainian <https://hosted.weblate.org/projects/normcap/ui/uk/"
+">\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.15.0\n"
 
@@ -22,17 +23,17 @@
 "\n"
 "Then restart NormCap."
 msgstr ""
 "'{application}' не має дозволу на «Запис екрану».\n"
 "\n"
 "Надайте його за допомогою діалогового вікна, яке з'явиться після натискання "
 "кнопки «Гаразд»,або через «Налаштування системи» > «Конфіденційність і "
-"безпека. \n"
+"безпека». \n"
 "\n"
-"Потім перезапустіть NormCap.\""
+"Потім перезапустіть NormCap."
 
 msgid "... need more?"
 msgstr "... потрібно більше?"
 
 msgid "1 URL captured"
 msgid_plural "{count} URLs captured"
 msgstr[0] "{count} URL-адресу захоплено"
@@ -151,15 +152,15 @@
 msgstr "Часті запитання"
 
 msgid ""
 "Frequently fetch NormCap's releases online and display\n"
 "a message if a new version is available."
 msgstr ""
 "Регулярно перевіряти релізи NormCap в Інтернеті\n"
-"та повідомляти про появу нових версій"
+"та повідомляти про появу нових версій."
 
 msgid "Information"
 msgstr "Інформація"
 
 msgid "Installed:"
 msgstr "Встановлено:"
 
@@ -275,16 +276,17 @@
 msgid ""
 "Tries to determine the text's type (e.g. line,\n"
 "paragraph, URL, email) and formats the output\n"
 "accordingly.\n"
 "If the result is unexpected, try 'raw' mode instead."
 msgstr ""
 "Намагається визначити тип тексту (наприклад, рядок,\n"
-"абзац, URL, електронна пошта) та відповідним чином форматує виведення.\n"
-"Якщо результат непередбачуваний, спробуйте скористатися режимом «raw»."
+"абзац, URL, електронна пошта) та відповідним чином\n"
+"форматує виведення. Якщо результат непередбачуваний,\n"
+"спробуйте скористатися режимом «raw»."
 
 msgid ""
 "Wait until a pink border appears around your screen, then select the desired "
 "capture area."
 msgstr ""
 "Дочекайтесь, поки навколо екрана з'явиться рожева рамка, а потім виберіть "
 "потрібну область захоплення."
```

### Comparing `normcap-0.5.5/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo` & `normcap-0.5.6/normcap/resources/locales/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.5.6/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/resources/tessdata/README.txt` & `normcap-0.5.6/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/__init__.py` & `normcap-0.5.6/normcap/screengrab/__init__.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/main.py` & `normcap-0.5.6/normcap/screengrab/main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/permissions.py` & `normcap-0.5.6/normcap/screengrab/permissions.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/post_processing.py` & `normcap-0.5.6/normcap/screengrab/post_processing.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/structures.py` & `normcap-0.5.6/normcap/screengrab/structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/system_info.py` & `normcap-0.5.6/normcap/screengrab/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/handlers/dbus_portal.py` & `normcap-0.5.6/normcap/screengrab/handlers/dbus_portal.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/handlers/dbus_shell.py` & `normcap-0.5.6/normcap/screengrab/handlers/dbus_shell.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/handlers/grim.py` & `normcap-0.5.6/normcap/screengrab/handlers/grim.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/normcap/screengrab/handlers/qt.py` & `normcap-0.5.6/normcap/screengrab/handlers/qt.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/conftest.py` & `normcap-0.5.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/test_app.py` & `normcap-0.5.6/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/test_main.py` & `normcap-0.5.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/test_utils.py` & `normcap-0.5.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/test_normcap.py` & `normcap-0.5.6/tests/integration/test_normcap.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/test_settings_menu.py` & `normcap-0.5.6/tests/integration/test_settings_menu.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/test_tray_menu.py` & `normcap-0.5.6/tests/integration/test_tray_menu.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/00_parse_urls.png` & `normcap-0.5.6/tests/integration/testcases/00_parse_urls.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/01_parse_colored_url.png` & `normcap-0.5.6/tests/integration/testcases/01_parse_colored_url.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/02_detect_window_title.png` & `normcap-0.5.6/tests/integration/testcases/02_detect_window_title.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/03_parse_emails.png` & `normcap-0.5.6/tests/integration/testcases/03_parse_emails.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/04_parse_email_skip_invalid.png` & `normcap-0.5.6/tests/integration/testcases/04_parse_email_skip_invalid.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/05_detect_text_with_low_contrast.png` & `normcap-0.5.6/tests/integration/testcases/05_detect_text_with_low_contrast.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/06_detect_special_characters.png` & `normcap-0.5.6/tests/integration/testcases/06_detect_special_characters.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/07_parse_paragraphs_of_text.png` & `normcap-0.5.6/tests/integration/testcases/07_parse_paragraphs_of_text.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/08_paragraphs.png` & `normcap-0.5.6/tests/integration/testcases/08_paragraphs.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/09_two_columns.png` & `normcap-0.5.6/tests/integration/testcases/09_two_columns.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/10_font_sizes.png` & `normcap-0.5.6/tests/integration/testcases/10_font_sizes.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/11_paragraph_with_bullet_points.png` & `normcap-0.5.6/tests/integration/testcases/11_paragraph_with_bullet_points.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/12_not_a_url.png` & `normcap-0.5.6/tests/integration/testcases/12_not_a_url.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/integration/testcases/data.py` & `normcap-0.5.6/tests/integration/testcases/data.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_main.py` & `normcap-0.5.6/tests/tests_clipboard/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_system_info.py` & `normcap-0.5.6/tests/tests_clipboard/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_handlers/test_pbcopy.py` & `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_pbcopy.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_handlers/test_qtclipboard.py` & `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_qtclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_handlers/test_windll.py` & `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_windll.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_handlers/test_wlclipboard.py` & `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_wlclipboard.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_clipboard/test_handlers/test_xclip.py` & `normcap-0.5.6/tests/tests_clipboard/test_handlers/test_xclip.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_downloader.py` & `normcap-0.5.6/tests/tests_gui/test_downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_introduction.py` & `normcap-0.5.6/tests/tests_gui/test_introduction.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_language_manager.py` & `normcap-0.5.6/tests/tests_gui/test_language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_loading_indicator.py` & `normcap-0.5.6/tests/tests_gui/test_loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_menu_button.py` & `normcap-0.5.6/tests/tests_gui/test_menu_button.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_models.py` & `normcap-0.5.6/tests/tests_gui/test_models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_notification.py` & `normcap-0.5.6/tests/tests_gui/test_notification.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_resources.py` & `normcap-0.5.6/tests/tests_gui/test_resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_settings.py` & `normcap-0.5.6/tests/tests_gui/test_settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_system_info.py` & `normcap-0.5.6/tests/tests_gui/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_tray.py` & `normcap-0.5.6/tests/tests_gui/test_tray.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_update_check.py` & `normcap-0.5.6/tests/tests_gui/test_update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_utils.py` & `normcap-0.5.6/tests/tests_gui/test_utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_gui/test_window.py` & `normcap-0.5.6/tests/tests_gui/test_window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/test_enhance.py` & `normcap-0.5.6/tests/tests_ocr/test_enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/test_recognize.py` & `normcap-0.5.6/tests/tests_ocr/test_recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/test_structures.py` & `normcap-0.5.6/tests/tests_ocr/test_structures.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/test_tesseract.py` & `normcap-0.5.6/tests/tests_ocr/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/test_transformer.py` & `normcap-0.5.6/tests/tests_ocr/test_transformer.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testcases/00_eng.png` & `normcap-0.5.6/tests/tests_ocr/testcases/00_eng.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testcases/01_chi_sim.png` & `normcap-0.5.6/tests/tests_ocr/testcases/01_chi_sim.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testcases/02_jpn.png` & `normcap-0.5.6/tests/tests_ocr/testcases/02_jpn.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testcases/data.py` & `normcap-0.5.6/tests/tests_ocr/testcases/data.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testimages/color.png` & `normcap-0.5.6/tests/tests_ocr/testimages/color.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testimages/dark.png` & `normcap-0.5.6/tests/tests_ocr/testimages/dark.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/testimages/light.png` & `normcap-0.5.6/tests/tests_ocr/testimages/light.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/transformers/test_email.py` & `normcap-0.5.6/tests/tests_ocr/transformers/test_email.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/transformers/test_paragraph.py` & `normcap-0.5.6/tests/tests_ocr/transformers/test_paragraph.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/transformers/test_single_line.py` & `normcap-0.5.6/tests/tests_ocr/transformers/test_single_line.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_ocr/transformers/test_url.py` & `normcap-0.5.6/tests/tests_ocr/transformers/test_url.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/split_full_desktop_to_screens.png` & `normcap-0.5.6/tests/tests_screengrab/split_full_desktop_to_screens.png`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_main.py` & `normcap-0.5.6/tests/tests_screengrab/test_main.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_permissions.py` & `normcap-0.5.6/tests/tests_screengrab/test_permissions.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_post_processing.py` & `normcap-0.5.6/tests/tests_screengrab/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_system_info.py` & `normcap-0.5.6/tests/tests_screengrab/test_system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_handlers/test_dbus_portal.py` & `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_dbus_portal.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_handlers/test_grim.py` & `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_grim.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/tests/tests_screengrab/test_handlers/test_qt.py` & `normcap-0.5.6/tests/tests_screengrab/test_handlers/test_qt.py`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/.gitignore` & `normcap-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/LICENSE` & `normcap-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.5.5/README.md` & `normcap-0.5.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,34 +28,34 @@
 
 Choose **_one_** of the options for a prebuilt release. If you encounter an issue please
 take a look at the [FAQs](https://dynobo.github.io/normcap/#faqs) or
 [report](https://github.com/dynobo/normcap/issues) it.
 
 #### Windows
 
-- [NormCap-0.5.5-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-Windows.msi)
+- [NormCap-0.5.6-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
   (Installer)
 
 #### Linux
 
-- [NormCap-0.5.5-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64.AppImage)
+- [NormCap-0.5.6-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
   (Binary)
 - [`normcap` @ AUR](https://aur.archlinux.org/packages/normcap) (Arch/Manjaro)
 - [com.github.dynobo.normcap @ FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap)
   (FlatPak)
 
 #### macOS
 
 Note: You have to allow the unsigned application on first start: "System Preferences" →
 "Security & Privacy" → "General" → "Open anyway". You also have to allow NormCap to take
 screenshots. ([#135](https://github.com/dynobo/normcap/issues/135))
 
-- [NormCap-0.5.5-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-macOS.dmg)
+- [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
   (Installer for x86/64)
-- [NormCap-0.5.5-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-arm64-macOS.dmg)
+- [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
   (Installer for M1)
 
 ## Install Python package
 
 As an _alternative_ to a prebuilt package from above you can install the
 [NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**, but it
 is a bit more complicated:
```

#### html2text {}

```diff
@@ -21,28 +21,28 @@
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Choose **_one_** of the options for a
 prebuilt release. If you encounter an issue please take a look at the [FAQs]
 (https://dynobo.github.io/normcap/#faqs) or [report](https://github.com/dynobo/
-normcap/issues) it. #### Windows - [NormCap-0.5.5-x86_64-Windows.msi](https://
-github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-
-Windows.msi) (Installer) #### Linux - [NormCap-0.5.5-x86_64.AppImage](https://
-github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-
+normcap/issues) it. #### Windows - [NormCap-0.5.6-x86_64-Windows.msi](https://
+github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-
+Windows.msi) (Installer) #### Linux - [NormCap-0.5.6-x86_64.AppImage](https://
+github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-
 x86_64.AppImage) (Binary) - [`normcap` @ AUR](https://aur.archlinux.org/
 packages/normcap) (Arch/Manjaro) - [com.github.dynobo.normcap @ FlatHub](https:
 //flathub.org/apps/details/com.github.dynobo.normcap) (FlatPak) #### macOS
 Note: You have to allow the unsigned application on first start: "System
 Preferences" â "Security & Privacy" â "General" â "Open anyway". You also
 have to allow NormCap to take screenshots. ([#135](https://github.com/dynobo/
-normcap/issues/135)) - [NormCap-0.5.5-x86_64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-macOS.dmg)
-(Installer for x86/64) - [NormCap-0.5.5-arm64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-arm64-macOS.dmg)
+normcap/issues/135)) - [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
+(Installer for x86/64) - [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
 (Installer for M1) ## Install Python package As an _alternative_ to a prebuilt
 package from above you can install the [NormCap Python package](https://
 pypi.org/project/normcap/) for **Python >=3.9**, but it is a bit more
 complicated: #### On Linux ```sh # Install dependencies (Ubuntu/Debian) sudo
 apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev
 libleptonica-dev wl-clipboard ## Install dependencies (Arch) sudo pacman -
 S tesseract tesseract-data-eng wl-clipboard ## Install dependencies (Fedora)
```

### Comparing `normcap-0.5.5/pyproject.toml` & `normcap-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "normcap"
-version = "0.5.5"
+version = "0.5.6"
 description = "OCR-powered screen-capture tool to capture information instead of images."
 keywords = ["screenshot", "ocr", "capture", "clipboard"]
 readme = "README.md"
 requires-python = ">=3.9,<3.12"
 license = "GPL-3.0-or-later"
 authors = [{ name = "dynobo", email = "dynobo@mailbox.org" }]
 classifiers = [
@@ -226,15 +226,15 @@
 no_show = true
 cluster = true
 max_cluster_size = 1
 
 [tool.briefcase]
 project_name = "NormCap"
 bundle = "eu.dynobo"
-version = "0.5.5"
+version = "0.5.6"
 url = "https://github.com/dynobo/normcap"
 license = "GPLv3"
 author = 'dynobo'
 author_email = "dynobo@mailbox.org"
 
 [tool.briefcase.app.normcap]
 formal_name = "NormCap"
@@ -341,15 +341,15 @@
 """
 
 [tool.briefcase.app.normcap.windows]
 use_full_install_path = false
 
 
 [tool.tbump.version]
-current = "0.5.5"
+current = "0.5.6"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (\-
```

### Comparing `normcap-0.5.5/PKG-INFO` & `normcap-0.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: normcap
-Version: 0.5.5
+Version: 0.5.6
 Summary: OCR-powered screen-capture tool to capture information instead of images.
 Project-URL: Homepage, https://dynobo.github.io/normcap/
 Project-URL: Issues, https://github.com/dynobo/normcap/issues
 Project-URL: Source Code, https://github.com/dynobo/normcap
 Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs
 Project-URL: Changelog, https://github.com/dynobo/normcap/blob/main/CHANGELOG
 Author-email: dynobo <dynobo@mailbox.org>
@@ -60,34 +60,34 @@
 
 Choose **_one_** of the options for a prebuilt release. If you encounter an issue please
 take a look at the [FAQs](https://dynobo.github.io/normcap/#faqs) or
 [report](https://github.com/dynobo/normcap/issues) it.
 
 #### Windows
 
-- [NormCap-0.5.5-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-Windows.msi)
+- [NormCap-0.5.6-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-Windows.msi)
   (Installer)
 
 #### Linux
 
-- [NormCap-0.5.5-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64.AppImage)
+- [NormCap-0.5.6-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64.AppImage)
   (Binary)
 - [`normcap` @ AUR](https://aur.archlinux.org/packages/normcap) (Arch/Manjaro)
 - [com.github.dynobo.normcap @ FlatHub](https://flathub.org/apps/details/com.github.dynobo.normcap)
   (FlatPak)
 
 #### macOS
 
 Note: You have to allow the unsigned application on first start: "System Preferences" →
 "Security & Privacy" → "General" → "Open anyway". You also have to allow NormCap to take
 screenshots. ([#135](https://github.com/dynobo/normcap/issues/135))
 
-- [NormCap-0.5.5-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-macOS.dmg)
+- [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
   (Installer for x86/64)
-- [NormCap-0.5.5-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-arm64-macOS.dmg)
+- [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
   (Installer for M1)
 
 ## Install Python package
 
 As an _alternative_ to a prebuilt package from above you can install the
 [NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**, but it
 is a bit more complicated:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: normcap Version: 0.5.5 Summary: OCR-powered screen-
+Metadata-Version: 2.3 Name: normcap Version: 0.5.6 Summary: OCR-powered screen-
 capture tool to capture information instead of images. Project-URL: Homepage,
 https://dynobo.github.io/normcap/ Project-URL: Issues, https://github.com/
 dynobo/normcap/issues Project-URL: Source Code, https://github.com/dynobo/
 normcap Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs Project-URL:
 Changelog, https://github.com/dynobo/normcap/blob/main/CHANGELOG Author-email:
 dynobo
 mailbox.org> License-Expression: GPL-3.0-or-later License-File: LICENSE
@@ -41,28 +41,28 @@
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Choose **_one_** of the options for a
 prebuilt release. If you encounter an issue please take a look at the [FAQs]
 (https://dynobo.github.io/normcap/#faqs) or [report](https://github.com/dynobo/
-normcap/issues) it. #### Windows - [NormCap-0.5.5-x86_64-Windows.msi](https://
-github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-
-Windows.msi) (Installer) #### Linux - [NormCap-0.5.5-x86_64.AppImage](https://
-github.com/dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-
+normcap/issues) it. #### Windows - [NormCap-0.5.6-x86_64-Windows.msi](https://
+github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-
+Windows.msi) (Installer) #### Linux - [NormCap-0.5.6-x86_64.AppImage](https://
+github.com/dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-
 x86_64.AppImage) (Binary) - [`normcap` @ AUR](https://aur.archlinux.org/
 packages/normcap) (Arch/Manjaro) - [com.github.dynobo.normcap @ FlatHub](https:
 //flathub.org/apps/details/com.github.dynobo.normcap) (FlatPak) #### macOS
 Note: You have to allow the unsigned application on first start: "System
 Preferences" â "Security & Privacy" â "General" â "Open anyway". You also
 have to allow NormCap to take screenshots. ([#135](https://github.com/dynobo/
-normcap/issues/135)) - [NormCap-0.5.5-x86_64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-x86_64-macOS.dmg)
-(Installer for x86/64) - [NormCap-0.5.5-arm64-macOS.dmg](https://github.com/
-dynobo/normcap/releases/download/v0.5.5/NormCap-0.5.5-arm64-macOS.dmg)
+normcap/issues/135)) - [NormCap-0.5.6-x86_64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-x86_64-macOS.dmg)
+(Installer for x86/64) - [NormCap-0.5.6-arm64-macOS.dmg](https://github.com/
+dynobo/normcap/releases/download/v0.5.6/NormCap-0.5.6-arm64-macOS.dmg)
 (Installer for M1) ## Install Python package As an _alternative_ to a prebuilt
 package from above you can install the [NormCap Python package](https://
 pypi.org/project/normcap/) for **Python >=3.9**, but it is a bit more
 complicated: #### On Linux ```sh # Install dependencies (Ubuntu/Debian) sudo
 apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev
 libleptonica-dev wl-clipboard ## Install dependencies (Arch) sudo pacman -
 S tesseract tesseract-data-eng wl-clipboard ## Install dependencies (Fedora)
```

