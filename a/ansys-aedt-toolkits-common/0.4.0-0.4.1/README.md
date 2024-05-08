# Comparing `tmp/ansys_aedt_toolkits_common-0.4.0.tar.gz` & `tmp/ansys_aedt_toolkits_common-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_aedt_toolkits_common-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_aedt_toolkits_common-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_aedt_toolkits_common-0.4.0.tar` & `ansys_aedt_toolkits_common-0.4.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1089 2024-05-06 16:57:47.089568 ansys_aedt_toolkits_common-0.4.0/LICENSE
--rw-r--r--   0        0        0     3531 2024-05-06 16:57:47.089568 ansys_aedt_toolkits_common-0.4.0/README.rst
--rw-r--r--   0        0        0     2763 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1230 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/__init__.py
--rw-r--r--   0        0        0    37347 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/api.py
--rw-r--r--   0        0        0      265 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/common_properties.toml
--rw-r--r--   0        0        0     1976 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/constants.py
--rw-r--r--   0        0        0     2517 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/logger_handler.py
--rw-r--r--   0        0        0     2541 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/models.py
--rw-r--r--   0        0        0     3706 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
--rw-r--r--   0        0        0     7884 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/rest_api.py
--rw-r--r--   0        0        0     3339 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/thread_manager.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/__init__.py
--rw-r--r--   0        0        0    21177 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/actions_generic.py
--rw-r--r--   0        0        0     1051 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_properties.toml
--rw-r--r--   0        0        0        0 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
--rw-r--r--   0        0        0     4997 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
--rw-r--r--   0        0        0     8951 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
--rw-r--r--   0        0        0     2381 2024-05-06 16:57:47.093568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/logger_handler.py
--rw-r--r--   0        0        0        0 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
--rw-r--r--   0        0        0    19844 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
--rw-r--r--   0        0        0     2997 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/models.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
--rw-r--r--   0        0        0     2406 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
--rw-r--r--   0        0        0     2487 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
--rw-r--r--   0        0        0    57746 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
--rw-r--r--   0        0        0    35360 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
--rw-r--r--   0        0        0     2379 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
--rw-r--r--   0        0        0      982 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
--rw-r--r--   0        0        0     1007 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
--rw-r--r--   0        0        0     5074 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
--rw-r--r--   0        0        0      819 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
--rw-r--r--   0        0        0     6058 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
--rw-r--r--   0        0        0     1124 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
--rw-r--r--   0        0        0     2436 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
--rw-r--r--   0        0        0     8449 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
--rw-r--r--   0        0        0     1615 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
--rw-r--r--   0        0        0     6064 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
--rw-r--r--   0        0        0    24133 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
--rw-r--r--   0        0        0     2300 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
--rw-r--r--   0        0        0     4241 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
--rw-r--r--   0        0        0     5091 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
--rw-r--r--   0        0        0     1969 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
--rw-r--r--   0        0        0      797 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
--rw-r--r--   0        0        0     1058 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
--rw-r--r--   0        0        0     2037 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
--rw-r--r--   0        0        0     3207 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
--rw-r--r--   0        0        0     1857 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
--rw-r--r--   0        0        0      344 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
--rw-r--r--   0        0        0     1877 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
--rw-r--r--   0        0        0     1749 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
--rw-r--r--   0        0        0     7977 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
--rw-r--r--   0        0        0      959 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
--rw-r--r--   0        0        0     1263 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
--rw-r--r--   0        0        0     3615 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
--rw-r--r--   0        0        0      448 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
--rw-r--r--   0        0        0     2255 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
--rw-r--r--   0        0        0      423 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
--rw-r--r--   0        0        0     3184 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
--rw-r--r--   0        0        0     8477 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
--rw-r--r--   0        0        0     2024 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
--rw-r--r--   0        0        0     3641 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
--rw-r--r--   0        0        0      897 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
--rw-r--r--   0        0        0      899 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
--rw-r--r--   0        0        0      868 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
--rw-r--r--   0        0        0      894 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
--rw-r--r--   0        0        0     1986 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
--rw-r--r--   0        0        0     1947 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
--rw-r--r--   0        0        0     1963 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
--rw-r--r--   0        0        0     2421 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
--rw-r--r--   0        0        0     2503 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
--rw-r--r--   0        0        0     5116 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
--rw-r--r--   0        0        0     4927 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
--rw-r--r--   0        0        0     2780 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
--rw-r--r--   0        0        0      603 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
--rw-r--r--   0        0        0     3871 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
--rw-r--r--   0        0        0     1821 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
--rw-r--r--   0        0        0     2587 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-06 16:57:47.097568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
--rw-r--r--   0        0        0      172 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
--rw-r--r--   0        0        0     7191 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
--rw-r--r--   0        0        0     6578 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
--rw-r--r--   0        0        0    10452 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
--rw-r--r--   0        0        0      471 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
--rw-r--r--   0        0        0     4120 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
--rw-r--r--   0        0        0      405 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
--rw-r--r--   0        0        0     2165 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
--rw-r--r--   0        0        0     1463 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
--rw-r--r--   0        0        0    12519 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
--rw-r--r--   0        0        0    11434 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
--rw-r--r--   0        0        0     4599 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
--rw-r--r--   0        0        0     4408 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
--rw-r--r--   0        0        0      290 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
--rw-r--r--   0        0        0     1153 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
--rw-r--r--   0        0        0    21788 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
--rw-r--r--   0        0        0     7002 2024-05-06 16:57:47.101568 ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/utils.py
--rw-r--r--   0        0        0     6156 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-08 12:10:02.727355 ansys_aedt_toolkits_common-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3531 2024-05-08 12:10:02.727355 ansys_aedt_toolkits_common-0.4.1/README.rst
+-rw-r--r--   0        0        0     2684 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1230 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/__init__.py
+-rw-r--r--   0        0        0    37347 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/api.py
+-rw-r--r--   0        0        0      265 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/common_properties.toml
+-rw-r--r--   0        0        0     1976 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/constants.py
+-rw-r--r--   0        0        0     2517 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/logger_handler.py
+-rw-r--r--   0        0        0     2541 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/models.py
+-rw-r--r--   0        0        0     3706 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/multithreading_server.py
+-rw-r--r--   0        0        0     7884 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/rest_api.py
+-rw-r--r--   0        0        0     3339 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/thread_manager.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/__init__.py
+-rw-r--r--   0        0        0    21177 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/actions_generic.py
+-rw-r--r--   0        0        0     1051 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_properties.toml
+-rw-r--r--   0        0        0        0 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/__init__.py
+-rw-r--r--   0        0        0     4997 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py
+-rw-r--r--   0        0        0     8951 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py
+-rw-r--r--   0        0        0     2381 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/logger_handler.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/__init__.py
+-rw-r--r--   0        0        0    19844 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py
+-rw-r--r--   0        0        0     2997 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/models.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py
+-rw-r--r--   0        0        0     2406 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg
+-rw-r--r--   0        0        0     2487 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg
+-rw-r--r--   0        0        0    57746 2024-05-08 12:10:02.735355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico
+-rw-r--r--   0        0        0    35360 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png
+-rw-r--r--   0        0        0     2379 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg
+-rw-r--r--   0        0        0      982 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg
+-rw-r--r--   0        0        0     1007 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg
+-rw-r--r--   0        0        0     5074 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg
+-rw-r--r--   0        0        0      819 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg
+-rw-r--r--   0        0        0     6058 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg
+-rw-r--r--   0        0        0     1124 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg
+-rw-r--r--   0        0        0     2436 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg
+-rw-r--r--   0        0        0     8449 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg
+-rw-r--r--   0        0        0     1615 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg
+-rw-r--r--   0        0        0     6064 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg
+-rw-r--r--   0        0        0    24133 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg
+-rw-r--r--   0        0        0     2300 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg
+-rw-r--r--   0        0        0     4241 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg
+-rw-r--r--   0        0        0     5091 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg
+-rw-r--r--   0        0        0     1969 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg
+-rw-r--r--   0        0        0      797 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg
+-rw-r--r--   0        0        0     1058 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg
+-rw-r--r--   0        0        0     2037 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg
+-rw-r--r--   0        0        0     3207 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg
+-rw-r--r--   0        0        0     1857 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg
+-rw-r--r--   0        0        0      344 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu.svg
+-rw-r--r--   0        0        0     1877 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg
+-rw-r--r--   0        0        0     1749 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg
+-rw-r--r--   0        0        0     7977 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg
+-rw-r--r--   0        0        0      959 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg
+-rw-r--r--   0        0        0     1263 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg
+-rw-r--r--   0        0        0     3615 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg
+-rw-r--r--   0        0        0      448 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_solve.svg
+-rw-r--r--   0        0        0     2255 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg
+-rw-r--r--   0        0        0      423 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/motor.svg
+-rw-r--r--   0        0        0     3184 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg
+-rw-r--r--   0        0        0     8477 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg
+-rw-r--r--   0        0        0     2024 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg
+-rw-r--r--   0        0        0     3641 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json
+-rw-r--r--   0        0        0      899 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json
+-rw-r--r--   0        0        0      868 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json
+-rw-r--r--   0        0        0      894 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json
+-rw-r--r--   0        0        0     1986 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py
+-rw-r--r--   0        0        0     1947 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui
+-rw-r--r--   0        0        0     1963 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui
+-rw-r--r--   0        0        0     2421 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py
+-rw-r--r--   0        0        0     2503 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py
+-rw-r--r--   0        0        0     5116 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui
+-rw-r--r--   0        0        0     4927 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py
+-rw-r--r--   0        0        0     2780 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py
+-rw-r--r--   0        0        0      603 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py
+-rw-r--r--   0        0        0     3871 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py
+-rw-r--r--   0        0        0     1821 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py
+-rw-r--r--   0        0        0      172 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py
+-rw-r--r--   0        0        0     7191 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py
+-rw-r--r--   0        0        0     6578 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py
+-rw-r--r--   0        0        0    10452 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py
+-rw-r--r--   0        0        0      471 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.739355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py
+-rw-r--r--   0        0        0     4120 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py
+-rw-r--r--   0        0        0      405 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py
+-rw-r--r--   0        0        0     2165 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py
+-rw-r--r--   0        0        0     1463 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py
+-rw-r--r--   0        0        0    12519 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py
+-rw-r--r--   0        0        0    11434 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py
+-rw-r--r--   0        0        0     4599 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py
+-rw-r--r--   0        0        0     4408 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py
+-rw-r--r--   0        0        0      290 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/styles.py
+-rw-r--r--   0        0        0     1153 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py
+-rw-r--r--   0        0        0    21788 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py
+-rw-r--r--   0        0        0     7012 2024-05-08 12:10:02.743355 ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/utils.py
+-rw-r--r--   0        0        0     6019 1970-01-01 00:00:00.000000 ansys_aedt_toolkits_common-0.4.1/PKG-INFO
```

### Comparing `ansys_aedt_toolkits_common-0.4.0/LICENSE` & `ansys_aedt_toolkits_common-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/README.rst` & `ansys_aedt_toolkits_common-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/pyproject.toml` & `ansys_aedt_toolkits_common-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,36 +22,36 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "build==1.2.1",
     "twine==5.0.0",
-    "pyaedt>=0.8.0,<0.9",
+    "pyaedt>=0.8.0,<0.10",
     "pydantic",
     "tomli; python_version < '3.12'",
 ]
 
 [project.optional-dependencies]
 all = [
-    "pyaedt[all]>=0.8.0,<0.9",
+    "pyaedt[all]>=0.8.0,<0.10",
     "flask",
     "PySide6-Essentials",
     "pyqtgraph",
     "qdarkstyle",
     "pyvistaqt",
 ]
 tests = [
-    "pyaedt[all]>=0.8.0,<0.9",
+    "pyaedt[all]>=0.8.0,<0.10",
     "flask",
     "pytest>=7.4.0,<8.3",
     "pytest-cov>=4.0.0,<5.1",
 ]
 doc = [
-    "pyaedt[all]>=0.8.0,<0.9",
+    "pyaedt[all]>=0.8.0,<0.10",
     "recommonmark>=0.7.0,<0.8",
     "PySide6-Essentials",
     "ansys-sphinx-theme>=0.10.0,<0.16",
     "numpydoc>=1.5.0,<1.8",
     "Sphinx>=7.1.0,<7.4",
     "sphinx-copybutton>=0.5.0,<0.6",
     "sphinx-autobuild==2021.3.14; python_version == '3.8'",
@@ -59,18 +59,14 @@
     "nbsphinx>=0.9.0,<0.10",
     "sphinx_design",
     "jupytext",
     "ipython>=8.13.0,<8.25",
     "jupyterlab>=4.0.0,<4.3",
     "pypandoc>=1.10.0,<1.14",
 ]
-ci = [
-    "pypandoc-binary>=1.10.0,<1.14",
-    "vtk-osmesa==9.2.20230527.dev0",
-]
 
 [tool.flit.module]
 name = "ansys.aedt.toolkits.common"
 
 [project.urls]
 Source = "https://github.com/ansys/pyaedt-toolkits-common.git"
 Issues = "https://github.com/ansys/pyaedt-toolkits-common/issues"
```

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 """
 pyaedt-toolkits.
 
 ansys.aedt.toolkits.common
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/api.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/api.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/constants.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/models.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/multithreading_server.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/multithreading_server.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/rest_api.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/rest_api.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/backend/thread_manager.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/backend/thread_manager.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/actions_generic.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/actions_generic.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_properties.toml` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_properties.toml`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/home_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/common_windows/settings_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/logger_handler.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/logger_handler.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/main_window/main_window_layout.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/models.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/models.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-black.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/ansys-primary-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/icon.ico`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/files/logo.png`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/additive-print-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/antenna.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/autonomous-vehicles-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/box_plot.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/connect-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cubes_solid.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/cylindrical_data_graphic.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/design-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/diagram.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-mission-engineering-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/digital-twins-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/electromagnetics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/embedded-software-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/fluids-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_folder_open.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_home.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_incident_wave.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_log.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_maximize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_menu_close.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_minimize.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_mode.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_2d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_plot_3d.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/icon_settings.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/materials-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/optics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/icons/photonics-gold.svg`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/images/load_images.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_dark.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/ansys_light.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/barbie.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/dracula.json`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/themes/json_themes.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/left_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/right_column.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/columns/ui_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/main_pages.ui`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/ui_templates/pages/ui_main_pages.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/py_combo_box.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_combo_box/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_credits/py_credits.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_div/py_div.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon/py_icon.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_icon_button/py_icon_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_label/py_label.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_column/py_left_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_left_menu/py_left_menu_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_line_edit/py_line_edit.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_logger/py_logger.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_progress/py_progress.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_push_button/py_push_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_right_column/py_right_column.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/py_slider.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_slider/styles.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_bar.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_title_bar/py_title_button.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_toggle/py_toggle.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/widgets/py_window/py_window.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/ui/utils/windows/common_window_utils.py`

 * *Files identical despite different names*

### Comparing `ansys_aedt_toolkits_common-0.4.0/src/ansys/aedt/toolkits/common/utils.py` & `ansys_aedt_toolkits_common-0.4.1/src/ansys/aedt/toolkits/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     is_student = False
     if "PYAEDT_SCRIPT_VERSION" in os.environ and "PYAEDT_SCRIPT_PORT" in os.environ:
         desktop_version = os.environ["PYAEDT_SCRIPT_VERSION"]
         desktop_pid = os.environ["PYAEDT_SCRIPT_PORT"]
         grpc = desktop_version > "2023.2" or is_linux
         if "PYAEDT_STUDENT_VERSION" in os.environ:
             is_student = os.environ["PYAEDT_STUDENT_VERSION"]
-        if is_student:
+        if is_student == "True":
             desktop_version += " STUDENT"
 
     elif len(sys.argv) == 3:
         desktop_pid, desktop_version = sys.argv[1], sys.argv[2]
 
     if desktop_pid and desktop_version:
         new_properties = {
```

### Comparing `ansys_aedt_toolkits_common-0.4.0/PKG-INFO` & `ansys_aedt_toolkits_common-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 Metadata-Version: 2.1
 Name: ansys-aedt-toolkits-common
-Version: 0.4.0
+Version: 0.4.1
 Summary: User interface example repository to create your toolkit.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: build==1.2.1
 Requires-Dist: twine==5.0.0
-Requires-Dist: pyaedt>=0.8.0,<0.9
+Requires-Dist: pyaedt>=0.8.0,<0.10
 Requires-Dist: pydantic
 Requires-Dist: tomli; python_version < '3.12'
-Requires-Dist: pyaedt[all]>=0.8.0,<0.9 ; extra == "all"
+Requires-Dist: pyaedt[all]>=0.8.0,<0.10 ; extra == "all"
 Requires-Dist: flask ; extra == "all"
 Requires-Dist: PySide6-Essentials ; extra == "all"
 Requires-Dist: pyqtgraph ; extra == "all"
 Requires-Dist: qdarkstyle ; extra == "all"
 Requires-Dist: pyvistaqt ; extra == "all"
-Requires-Dist: pypandoc-binary>=1.10.0,<1.14 ; extra == "ci"
-Requires-Dist: vtk-osmesa==9.2.20230527.dev0 ; extra == "ci"
-Requires-Dist: pyaedt[all]>=0.8.0,<0.9 ; extra == "doc"
+Requires-Dist: pyaedt[all]>=0.8.0,<0.10 ; extra == "doc"
 Requires-Dist: recommonmark>=0.7.0,<0.8 ; extra == "doc"
 Requires-Dist: PySide6-Essentials ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.16 ; extra == "doc"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc"
 Requires-Dist: Sphinx>=7.1.0,<7.4 ; extra == "doc"
 Requires-Dist: sphinx-copybutton>=0.5.0,<0.6 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc" and ( python_version == '3.8')
 Requires-Dist: sphinx-autobuild==2024.4.16 ; extra == "doc" and ( python_version > '3.8')
 Requires-Dist: nbsphinx>=0.9.0,<0.10 ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
 Requires-Dist: jupytext ; extra == "doc"
 Requires-Dist: ipython>=8.13.0,<8.25 ; extra == "doc"
 Requires-Dist: jupyterlab>=4.0.0,<4.3 ; extra == "doc"
 Requires-Dist: pypandoc>=1.10.0,<1.14 ; extra == "doc"
-Requires-Dist: pyaedt[all]>=0.8.0,<0.9 ; extra == "tests"
+Requires-Dist: pyaedt[all]>=0.8.0,<0.10 ; extra == "tests"
 Requires-Dist: flask ; extra == "tests"
 Requires-Dist: pytest>=7.4.0,<8.3 ; extra == "tests"
 Requires-Dist: pytest-cov>=4.0.0,<5.1 ; extra == "tests"
 Project-URL: Discussions, https://github.com/ansys/pyaedt-toolkits-common/discussions
 Project-URL: Documentation, https://aedt.common.toolkit.docs.pyansys.com
 Project-URL: Issues, https://github.com/ansys/pyaedt-toolkits-common/issues
 Project-URL: Releases, https://github.com/ansys/pyaedt-toolkits-common/releases
 Project-URL: Source, https://github.com/ansys/pyaedt-toolkits-common.git
 Provides-Extra: all
-Provides-Extra: ci
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyAEDT Common Toolkit
 =====================
 
 |pyansys| |PythonVersion| |GH-CI| |MIT| |coverage| |black|
```

