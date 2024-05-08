# Comparing `tmp/reflex_antd-0.0.5.tar.gz` & `tmp/reflex_antd-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.5.tar", last modified: Tue Apr 30 11:23:59 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.6.tar", last modified: Wed May  8 11:41:22 2024, max compression
```

## Comparing `reflex_antd-0.0.5.tar` & `reflex_antd-0.0.6.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.096709 reflex_antd-0.0.5/
--rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.5/LICENSE
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:23:59.089708 reflex_antd-0.0.5/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.5/README.md
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:55.453099 reflex_antd-0.0.5/custom_components/
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:55.726139 reflex_antd-0.0.5/custom_components/reflex_antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/__init__.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.051708 reflex_antd-0.0.5/custom_components/reflex_antd/antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/__init__.py
--rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     3547 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.py
--rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.py
--rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     3495 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.py
--rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1947 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.py
--rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2022 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/notification.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-04-30 11:13:33.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.py
--rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-04-30 11:13:35.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)    24090 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.5/custom_components/reflex_antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/constant.py
--rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/display.py
--rwxrwxrwx   0 see       (1000) see       (1000)      873 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/entry.py
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/feedback.py
--rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/general.py
--rwxrwxrwx   0 see       (1000) see       (1000)      152 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/helper.py
--rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-04-30 11:13:32.000000 reflex_antd-0.0.5/custom_components/reflex_antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/navigation.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-04-30 11:13:36.000000 reflex_antd-0.0.5/custom_components/reflex_antd/util.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-04-30 11:23:59.079707 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)     6855 2024-04-30 11:23:55.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/SOURCES.txt
--rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/dependency_links.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/requires.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-04-30 11:23:54.000000 reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/top_level.txt
--rwxrwxrwx   0 see       (1000) see       (1000)      794 2024-04-30 11:21:16.000000 reflex_antd-0.0.5/pyproject.toml
--rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-04-30 11:23:59.097707 reflex_antd-0.0.5/setup.cfg
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.811942 reflex_antd-0.0.6/
+-rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.6/LICENSE
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:41:22.804683 reflex_antd-0.0.6/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.6/README.md
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:19.050568 reflex_antd-0.0.6/custom_components/
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:19.325560 reflex_antd-0.0.6/custom_components/reflex_antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/__init__.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.768139 reflex_antd-0.0.6/custom_components/reflex_antd/antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/__init__.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     3547 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     5458 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1934 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2022 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4041 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/notification.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)    25316 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.6/custom_components/reflex_antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/constant.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/display.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      899 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/entry.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      515 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/feedback.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/general.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      152 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/helper.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-05-08 11:29:14.000000 reflex_antd-0.0.6/custom_components/reflex_antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/navigation.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/util.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.795683 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)     6855 2024-05-08 11:41:19.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/requires.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/top_level.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)      794 2024-05-08 11:40:05.000000 reflex_antd-0.0.6/pyproject.toml
+-rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-05-08 11:41:22.812478 reflex_antd-0.0.6/setup.cfg
```

### Comparing `reflex_antd-0.0.5/LICENSE` & `reflex_antd-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/PKG-INFO` & `reflex_antd-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/base.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/base.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     enter_button: Optional[Var[ReactNode]]
     loading: Optional[Var[bool]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            'on_search': lambda value, event, info: [value, event, info],
+            'on_search': lambda value, event, info: [value],
         })
         return _triggers
 
 
 class Password(Input):
     tag = 'Input.Password'
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,72 @@
 from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
 
-from reflex import Component, Var
+from ..base import AntdComponent, ContainVar, JsNode, ReactNode
 
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TypeType
 
+class TreeSelect(AntdComponent):
+    tag = 'TreeSelect'
 
-class Modal(AntdComponent):
-    tag = 'Modal'
-
-    class_names: Optional[Var[ContainVar]]
-    styles: Optional[Var[ContainVar]]
-    cancel_button_props: Optional[Var[ContainVar]]
-    cancel_text: Optional[Var[ReactNode]]
-    centered: Optional[Var[bool]]
-    close_icon: Optional[Var[Union[ReactNode, bool]]]
-    confirm_loading: Optional[Var[bool]]
-    destroy_on_close: Optional[Var[bool]]
-    focus_trigger_after_close: Optional[Var[bool]]
-    footer: Optional[Var[ContainVar]]
-    force_render: Optional[Var[bool]]
-    get_container: Optional[Var[Union[bool, ContainVar]]]
-    keyboard: Optional[Var[bool]]
-    mask: Optional[Var[bool]]
-    mask_closable: Optional[Var[bool]]
-    modal_render: Optional[Var[ReactNode]]
-    ok_button_props: Optional[Var[ContainVar]]
-    ok_text: Optional[Var[ReactNode]]
-    ok_type: Optional[Var[TypeType]]
-    title: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    width: Optional[Var[Union[str, int]]]
-    wrapClassName: Optional[Var[str]]
-    zIndex: Optional[Var[int]]
+    allow_clear: Optional[Var[Union[bool, ReactNode]]]
+    auto_clear_search_value: Optional[Var[bool]]
+    default_value: Optional[Var[Union[str, List[str]]]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    dropdown_render: Optional[Var[JsNode]]
+    dropdown_style: Optional[Var[Dict]]
+    field_names: Optional[Var[Dict]]
+    filter_tree_node: Optional[Var[Union[bool, JsNode]]]
+    get_popup_container: Optional[Var[JsNode]]
+    label_in_value: Optional[Var[bool]]
+    list_height: Optional[Var[int]]
+    load_data: Optional[Var[JsNode]]
+    max_tag_count: Optional[Var[int]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsNode]]]
+    max_tag_text_length: Optional[Var[int]]
+    multiple: Optional[Var[bool]]
+    not_found_content: Optional[Var[ReactNode]]
+    placeholder: Optional[Var[str]]
+    placement: Optional[Var[str]]
+    search_value: Optional[Var[str]]
+    show_checked_strategy: Optional[Var[str]]
+    show_search: Optional[Var[bool]]
+    size: Optional[Var[str]]
+    status: Optional[Var[str]]
+    suffix_icon: Optional[Var[ReactNode]]
+    switcher_icon: Optional[Var[Union[ReactNode, ContainVar]]]
+    tag_render: Optional[Var[JsNode]]
+    tree_checkable: Optional[Var[bool]]
+    tree_check_strictly: Optional[Var[bool]]
+    tree_data: Optional[Var[List[Dict]]]
+    tree_data_simple_mode: Optional[Var[Union[bool, Dict]]]
+    tree_default_expand_all: Optional[Var[bool]]
+    tree_default_expanded_keys: Optional[Var[List]]
+    tree_expand_action: Optional[Var[Union[str, bool]]]
+    tree_expanded_keys: Optional[Var[List[str]]]
+    tree_icon: Optional[Var[bool]]
+    tree_line: Optional[Var[Union[bool, Dict]]]
+    tree_loaded_keys: Optional[Var[List[str]]]
+    tree_node_filter_prop: Optional[Var[str]]
+    tree_node_label_prop: Optional[Var[str]]
+    value: Optional[Var[Union[str, List[str]]]]
+    variant: Optional[Var[str]]
+    virtual: Optional[Var[str]]
 
     def get_event_triggers(self) -> Dict[str, Any]:
         _triggers = super().get_event_triggers()
         _triggers.update({
-            "after_close": lambda: [],
-            "on_cancel": lambda event: [],
-            "on_ok": lambda event: [],
-            "after_open_change": lambda open: [],
+            EventTriggers.ON_CHANGE: lambda value, label, extra: [value, label, extra],
+            EventTriggers.ON_SELECT: lambda value, node, extra: [value, node, extra],
+            "on_dropdown_visible_change": lambda open: [open],
+            "on_search": lambda value: [value],
+            "on_tree_expand": lambda keys: [keys],
+
+            "filter_tree_node": lambda node: [node],
+            "load_data": lambda node: [node],
         })
         return _triggers
 
 
-modal = Modal.create
+tree_select = TreeSelect.create
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/notification.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tour.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/antd/watermark.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/base.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional
+from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional, Self
 import sys
 from os import path
 from abc import ABC, abstractmethod
 from functools import lru_cache, wraps
 from hashlib import md5
 import uuid
 import dataclasses
@@ -143,20 +143,23 @@
 
     def serialize(self) -> str:
         return f'<{self.item.tag}/>'
 
 
 class JsEvent:
     hd: EventHandler
+    # event_trigger use for custom trigger, must work with fmt=True
+    event_trigger: Callable
 
-    def __init__(self, hd: Any, js: str, fmt: bool = False):
+    def __init__(self, hd: Any, js: str = '', fmt: bool = False, event_trigger: Callable = None):
         assert isinstance(hd, EventHandler)
         self.hd = hd
         self.js = js
         self.fmt = fmt
+        self.event_trigger = event_trigger
 
     def get_state_full_name(self) -> str:
         name = str(self.hd.fn).split(' ')[1]
         _base = format.to_snake_case(name)
         return f'state.{_base}'
 
     def get_event_args(self) -> str:
@@ -164,14 +167,18 @@
         rs = []
         for idx, _arg in enumerate(_args.args):
             if idx == 0:  # ignore self
                 continue
             rs.append(f'{_arg}:{self.args[idx-1]}')
         return ','.join(rs)
 
+    def get_ex_item(self, parent, key) -> ExItem:
+        item = ExEventHandlerItem(self, parent, key=key)
+        return item
+
 
 js_event = JsEvent
 
 
 class ExEventHandlerItem(ExItem):
     item: JsEvent
 
@@ -181,14 +188,15 @@
 
     @property
     def hd_item(self) -> 'ExLambdaHandlerItem':
         try:
             return self._hd_item
         except AttributeError:
             self._hd_item = ExLambdaHandlerItem(self.item.hd, self.parent, key=self.key)
+            self._hd_item.event_trigger = self.item.event_trigger
             return self._hd_item
 
     def _get_fn_name(self) -> str:
         return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}_{id(self)}"
 
     def serialize(self) -> str:
         hd_name = self.hd_item.serialize()
@@ -209,26 +217,29 @@
 
     def get_imports(self) -> imports.ImportDict:
         return self.hd_item.get_imports()
 
 
 class ExLambdaHandlerItem(ExItem):
     item: Callable
+    event_trigger: Callable = None
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
         return isinstance(item, Callable)
 
     def _get_fn_name(self) -> str:
         return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}_{id(self)}"
 
     def _get_event_trigger_key(self) -> str:
         return RE_KEY_IDX.sub('.*.', self.key)
 
     def _get_event_trigger(self) -> Callable:
+        if self.event_trigger is not None:
+            return self.event_trigger
         triggers = self.parent.get_event_triggers()
         rs = triggers.get(self._get_event_trigger_key(), lambda: [])
         return rs
 
     def serialize(self) -> str:
         return self._get_fn_name()
 
@@ -289,25 +300,43 @@
     def get_hooks(self) -> Set[str] | Dict[str, None]:
         return self.item._var_data.hooks
 
     def get_state(self) -> str:
         return self.item._var_data.state
 
 
+class FakeComponentMixin:
+    def _create_event_chain(self, *args, **kwargs):
+        return Component._create_event_chain(self, *args, **kwargs)
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        return {}
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return {}
+
+    def get_imports(self) -> imports.ImportDict:
+        return {}
+
+
 class JsValue:
     value: Callable | str
 
     def __init__(self, value: Union[str, Callable, Any] = None, **kwargs):
         self.value = value
         self._init(**kwargs)
 
     def _init(self, **kwargs) -> None:
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+    def get_ex_item(self, parent, key) -> ExItem:
+        item = ExJsItem(self, parent, key=key)
+        return item
+
     def serialize(self) -> str:
         return self.value
 
     def get_imports(self) -> imports.ImportDict:
         return {}
 
     def get_state(self) -> str:
@@ -470,14 +499,19 @@
 
         def _dict(_v: Dict, pkey: str) -> Dict[str, Any]:
             return dict((format.to_camel_case(k), _op(v, key=f'{pkey}.{k}')) for k, v in _v.items() if v is not None)
 
         rs = _op(value, key=self.name)
         self._value = rs
 
+    def get_ex_item(self, key: str) -> ExItem | None:
+        for i in self._coms.values():
+            if i.key == key:
+                return i
+
     def get_value(self) -> str:
         v = pretty_dumps(self._value)
         for k, ex in self._coms.items():
             v = v.replace(f'"{k}"', ex.serialize())
         return v
 
     def get_imports(self) -> imports.ImportDict:
@@ -543,44 +577,51 @@
     _var_fmt: ExFormatter = dataclasses.field(default=None)
 
     @property
     def _var_full_name(self) -> str:
         return self._var_name
 
     @classmethod
-    def create(cls, _args_: Any = None, **kwargs) -> Var | None:
+    def create(cls, _args_: Any = None, **kwargs) -> Self:
         value = _args_ if _args_ is not None else kwargs
         # v: BaseVar = super().create(_name, _var_is_local=_var_is_local, _var_is_string=_var_is_string)
         return cls(
             _var_name='',
             _var_type=cls,
             _var_is_local=True,
             _var_is_string=False,
             _var_data=None,
             _var_value=value,
         )
 
-    def init(self, parent: Component, name: str):
+    def init(self, parent: Component, name: str) -> Self:
         fmt = ExFormatter(self._var_value, parent=parent, name=name)
         self._var_fmt = fmt
         self._var_name = fmt.get_value()
         self._var_data = fmt.get_var_data()
+        return self
 
     def get_custom_components(self) -> set[CustomComponent]:
         rs = set()
         for ex in self._var_fmt._coms.values():
             rs |= ex.get_custom_components()
         return rs
 
     def get_custom_code(self) -> Set[str]:
         rs = set()
         for ex in self._var_fmt._coms.values():
             rs |= ex.get_custom_code()
         return rs
 
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self._var_data.hooks
+
+    def get_imports(self) -> imports.ImportDict:
+        return self._var_data.imports
+
 
 contain = ContainVar.create
 
 
 # no use
 class VarDataMixin:
     def __iter__(self):
@@ -678,21 +719,19 @@
         for k, v in contains.items():
             v.init(self, k)
             self._custom_components |= v.get_custom_components()
             setattr(self, k, v)
 
         event_keys = self.get_event_triggers().keys()
         for k, v in exs.items():
-            if isinstance(v, JsValue):
-                item = ExJsItem(v, self, key=k)
-                self._custom_components |= item.get_custom_components()
-            elif isinstance(v, JsEvent):
-                item = ExEventHandlerItem(v, self, key=k)
+            if isinstance(v, (JsValue, JsEvent)):
+                item = v.get_ex_item(self, k)
             else:
                 raise NotImplementedError(f"Unsupported type: {type(v)}")
+            self._custom_components |= item.get_custom_components()
             _v = BaseVar(
                 _var_name=item.serialize(),
                 _var_is_local=True,
                 _var_data=item.get_var_data(),
             )
             if k in event_keys:
                 self.event_triggers[k] = _v
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.6/custom_components/reflex_antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/constant.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/display.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .antd.auto_complete import auto_complete  # noqa
 from .antd.cascader import cascader  # noqa
 from .antd.checkbox import checkbox_group, checkbox  # noqa
 from .antd.color_picker import color_picker  # noqa
 from .antd.date_picker import dayjs, date_picker, range_picker  # noqa
-from .antd.form import form, form_item, form_list, form_provider  # noqa
+from .antd.form import form, form_item, form_list, form_provider, confirm_form, modal_form  # noqa
 from .antd.input import input, text_area, search, password  # noqa
 from .antd.input_number import input_number  # noqa
 from .antd.mentions import mention  # noqa
 from .antd.radio import radio, radio_button, radio_group  # noqa
 from .antd.rate import rate  # noqa
 from .antd.select import select  # noqa
 from .antd.tree_select import tree_select  # noqa
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd/util.py` & `reflex_antd-0.0.6/custom_components/reflex_antd/util.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.5
+Version: 0.0.6
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.5/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.5/pyproject.toml` & `reflex_antd-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-antd"
-version = "0.0.5"
+version = "0.0.6"
 description = "Reflex custom component antd"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
 keywords = [
     "reflex",
```

