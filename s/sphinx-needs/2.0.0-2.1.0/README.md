# Comparing `tmp/sphinx_needs-2.0.0.tar.gz` & `tmp/sphinx_needs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_needs-2.0.0.tar", max compression
+gzip compressed data, was "sphinx_needs-2.1.0.tar", max compression
```

## Comparing `sphinx_needs-2.0.0.tar` & `sphinx_needs-2.1.0.tar`

### file list

```diff
@@ -1,678 +1,679 @@
--rw-r--r--   0        0        0     1076 2023-11-13 19:22:26.824688 sphinx_needs-2.0.0/LICENSE
--rw-r--r--   0        0        0     2938 2023-11-13 19:22:26.824688 sphinx_needs-2.0.0/README.rst
--rw-r--r--   0        0        0     4480 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/__init__.py
--rw-r--r--   0        0        0      218 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/api/__init__.py
--rw-r--r--   0        0        0     5268 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/api/configuration.py
--rw-r--r--   0        0        0      851 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/api/exceptions.py
--rw-r--r--   0        0        0    30719 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/api/need.py
--rw-r--r--   0        0        0     9713 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/builder.py
--rw-r--r--   0        0        0    14062 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/config.py
--rw-r--r--   0        0        0      998 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/blank/blank.css
--rw-r--r--   0        0        0     2388 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/blank/styles.css
--rw-r--r--   0        0        0     3284 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/common.css
--rw-r--r--   0        0        0     3727 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/dark/dark.css
--rw-r--r--   0        0        0     2676 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/dark/layouts.css
--rw-r--r--   0        0        0     2854 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/dark/styles.css
--rw-r--r--   0        0        0        1 2023-11-13 19:22:26.892688 sphinx_needs-2.0.0/sphinx_needs/css/grids.css
--rw-r--r--   0        0        0     2678 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/css/modern/layouts.css
--rw-r--r--   0        0        0      453 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/css/modern/modern.css
--rw-r--r--   0        0        0     3104 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/css/modern/styles.css
--rw-r--r--   0        0        0    19494 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/data.py
--rw-r--r--   0        0        0     6364 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/debug.py
--rw-r--r--   0        0        0     7101 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/defaults.py
--rw-r--r--   0        0        0     7345 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/diagrams_common.py
--rw-r--r--   0        0        0        0 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/__init__.py
--rw-r--r--   0        0        0     8952 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/list2need.py
--rw-r--r--   0        0        0    21586 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/need.py
--rw-r--r--   0        0        0    17599 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needbar.py
--rw-r--r--   0        0        0     7187 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needextend.py
--rw-r--r--   0        0        0     4899 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needextract.py
--rw-r--r--   0        0        0    10713 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needfilter.py
--rw-r--r--   0        0        0    20453 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needflow.py
--rw-r--r--   0        0        0    13446 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needgantt.py
--rw-r--r--   0        0        0    10180 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needimport.py
--rw-r--r--   0        0        0     1425 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needimport_template.rst
--rw-r--r--   0        0        0     4386 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needlist.py
--rw-r--r--   0        0        0    10433 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needpie.py
--rw-r--r--   0        0        0     3452 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needreport.py
--rw-r--r--   0        0        0     1671 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needreport_template.rst
--rw-r--r--   0        0        0    10043 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needsequence.py
--rw-r--r--   0        0        0     4575 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needservice.py
--rw-r--r--   0        0        0    14018 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needtable.py
--rw-r--r--   0        0        0    17271 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/needuml.py
--rw-r--r--   0        0        0     3216 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/directives/utils.py
--rw-r--r--   0        0        0     7594 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/environment.py
--rw-r--r--   0        0        0      199 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/errors.py
--rw-r--r--   0        0        0     5901 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/external_needs.py
--rw-r--r--   0        0        0    13108 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/filter_common.py
--rw-r--r--   0        0        0      647 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/functions/__init__.py
--rw-r--r--   0        0        0    15346 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/functions/common.py
--rw-r--r--   0        0        0    16179 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/functions/functions.py
--rw-r--r--   0        0        0    20831 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/avatar.png
--rw-r--r--   0        0        0    47870 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/avatar.svg
--rw-r--r--   0        0        0      433 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/activity.png
--rw-r--r--   0        0        0      485 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/airplay.png
--rw-r--r--   0        0        0      685 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/alert-circle.png
--rw-r--r--   0        0        0      445 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/alert-octagon.png
--rw-r--r--   0        0        0      598 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/alert-triangle.png
--rw-r--r--   0        0        0      325 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/align-center.png
--rw-r--r--   0        0        0      284 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/align-justify.png
--rw-r--r--   0        0        0      308 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/align-left.png
--rw-r--r--   0        0        0      311 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/align-right.png
--rw-r--r--   0        0        0      626 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/anchor.png
--rw-r--r--   0        0        0      842 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/aperture.png
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/archive.png
--rw-r--r--   0        0        0      729 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-down-circle.png
--rw-r--r--   0        0        0      283 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-down-left.png
--rw-r--r--   0        0        0      284 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-down-right.png
--rw-r--r--   0        0        0      328 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-down.png
--rw-r--r--   0        0        0      706 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-left-circle.png
--rw-r--r--   0        0        0      274 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-left.png
--rw-r--r--   0        0        0      709 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-right-circle.png
--rw-r--r--   0        0        0      262 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-right.png
--rw-r--r--   0        0        0      747 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-up-circle.png
--rw-r--r--   0        0        0      282 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-up-left.png
--rw-r--r--   0        0        0      277 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-up-right.png
--rw-r--r--   0        0        0      336 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-up.png
--rw-r--r--   0        0        0      796 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/at-sign.png
--rw-r--r--   0        0        0      669 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/award.png
--rw-r--r--   0        0        0      268 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bar-chart-2.png
--rw-r--r--   0        0        0      265 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bar-chart.png
--rw-r--r--   0        0        0      573 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/battery-charging.png
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/battery.png
--rw-r--r--   0        0        0      607 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bell-off.png
--rw-r--r--   0        0        0      559 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bell.png
--rw-r--r--   0        0        0      397 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bluetooth.png
--rw-r--r--   0        0        0      471 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bold.png
--rw-r--r--   0        0        0      441 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/book-open.png
--rw-r--r--   0        0        0      394 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/book.png
--rw-r--r--   0        0        0      414 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bookmark.png
--rw-r--r--   0        0        0      615 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/box.png
--rw-r--r--   0        0        0      485 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/briefcase.png
--rw-r--r--   0        0        0      499 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/calendar.png
--rw-r--r--   0        0        0      637 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/camera-off.png
--rw-r--r--   0        0        0      611 2023-11-13 19:22:26.896688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/camera.png
--rw-r--r--   0        0        0      549 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cast.png
--rw-r--r--   0        0        0      686 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/check-circle.png
--rw-r--r--   0        0        0      446 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/check-square.png
--rw-r--r--   0        0        0      281 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/check.png
--rw-r--r--   0        0        0      263 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevron-down.png
--rw-r--r--   0        0        0      246 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevron-left.png
--rw-r--r--   0        0        0      246 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevron-right.png
--rw-r--r--   0        0        0      263 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevron-up.png
--rw-r--r--   0        0        0      325 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevrons-down.png
--rw-r--r--   0        0        0      261 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevrons-left.png
--rw-r--r--   0        0        0      270 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevrons-right.png
--rw-r--r--   0        0        0      322 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chevrons-up.png
--rw-r--r--   0        0        0      830 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chrome.png
--rw-r--r--   0        0        0      634 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/circle.png
--rw-r--r--   0        0        0      454 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/clipboard.png
--rw-r--r--   0        0        0      701 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/clock.png
--rw-r--r--   0        0        0      692 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-drizzle.png
--rw-r--r--   0        0        0      670 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-lightning.png
--rw-r--r--   0        0        0      613 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-off.png
--rw-r--r--   0        0        0      684 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-rain.png
--rw-r--r--   0        0        0      656 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-snow.png
--rw-r--r--   0        0        0      578 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud.png
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/code.png
--rw-r--r--   0        0        0      552 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/codepen.png
--rw-r--r--   0        0        0      725 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/codesandbox.png
--rw-r--r--   0        0        0      559 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/coffee.png
--rw-r--r--   0        0        0      350 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/columns.png
--rw-r--r--   0        0        0      480 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/command.png
--rw-r--r--   0        0        0      785 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/compass.png
--rw-r--r--   0        0        0      512 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/copy.png
--rw-r--r--   0        0        0      354 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-down-left.png
--rw-r--r--   0        0        0      367 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-down-right.png
--rw-r--r--   0        0        0      393 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-left-down.png
--rw-r--r--   0        0        0      393 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-left-up.png
--rw-r--r--   0        0        0      397 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-right-down.png
--rw-r--r--   0        0        0      388 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-right-up.png
--rw-r--r--   0        0        0      369 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-up-left.png
--rw-r--r--   0        0        0      375 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/corner-up-right.png
--rw-r--r--   0        0        0      618 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cpu.png
--rw-r--r--   0        0        0      351 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/credit-card.png
--rw-r--r--   0        0        0      437 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/crop.png
--rw-r--r--   0        0        0      659 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/crosshair.png
--rw-r--r--   0        0        0      701 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/database.png
--rw-r--r--   0        0        0      446 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/delete.png
--rw-r--r--   0        0        0      731 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/disc.png
--rw-r--r--   0        0        0      510 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/dollar-sign.png
--rw-r--r--   0        0        0      624 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/download-cloud.png
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/download.png
--rw-r--r--   0        0        0      555 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/droplet.png
--rw-r--r--   0        0        0      390 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/edit-2.png
--rw-r--r--   0        0        0      392 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/edit-3.png
--rw-r--r--   0        0        0      548 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/edit.png
--rw-r--r--   0        0        0      532 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/external-link.png
--rw-r--r--   0        0        0      729 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/eye-off.png
--rw-r--r--   0        0        0      686 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/eye.png
--rw-r--r--   0        0        0      526 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/facebook.png
--rw-r--r--   0        0        0      442 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/fast-forward.png
--rw-r--r--   0        0        0      555 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/feather.png
--rw-r--r--   0        0        0      703 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/figma.png
--rw-r--r--   0        0        0      493 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file-minus.png
--rw-r--r--   0        0        0      553 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file-plus.png
--rw-r--r--   0        0        0      545 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file-text.png
--rw-r--r--   0        0        0      438 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file.png
--rw-r--r--   0        0        0      581 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/film.png
--rw-r--r--   0        0        0      489 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/filter.png
--rw-r--r--   0        0        0      451 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/flag.png
--rw-r--r--   0        0        0      462 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/folder-minus.png
--rw-r--r--   0        0        0      539 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/folder-plus.png
--rw-r--r--   0        0        0      421 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/folder.png
--rw-r--r--   0        0        0      465 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/framer.png
--rw-r--r--   0        0        0      717 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/frown.png
--rw-r--r--   0        0        0      583 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/gift.png
--rw-r--r--   0        0        0      515 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/git-branch.png
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/git-commit.png
--rw-r--r--   0        0        0      481 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/git-merge.png
--rw-r--r--   0        0        0      473 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/git-pull-request.png
--rw-r--r--   0        0        0      729 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/github.png
--rw-r--r--   0        0        0      707 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/gitlab.png
--rw-r--r--   0        0        0      764 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/globe.png
--rw-r--r--   0        0        0      466 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/grid.png
--rw-r--r--   0        0        0      514 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/hard-drive.png
--rw-r--r--   0        0        0      420 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/hash.png
--rw-r--r--   0        0        0      640 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/headphones.png
--rw-r--r--   0        0        0      547 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/heart.png
--rw-r--r--   0        0        0      767 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/help-circle.png
--rw-r--r--   0        0        0      461 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/hexagon.png
--rw-r--r--   0        0        0      501 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/home.png
--rw-r--r--   0        0        0      584 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/image.png
--rw-r--r--   0        0        0      566 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/inbox.png
--rw-r--r--   0        0        0      683 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/info.png
--rw-r--r--   0        0        0      697 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/instagram.png
--rw-r--r--   0        0        0      378 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/italic.png
--rw-r--r--   0        0        0      552 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/key.png
--rw-r--r--   0        0        0      443 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/layers.png
--rw-r--r--   0        0        0      397 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/layout.png
--rw-r--r--   0        0        0      776 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/life-buoy.png
--rw-r--r--   0        0        0      479 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/link-2.png
--rw-r--r--   0        0        0      654 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/link.png
--rw-r--r--   0        0        0      615 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/linkedin.png
--rw-r--r--   0        0        0      227 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/list.png
--rw-r--r--   0        0        0      396 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/loader.png
--rw-r--r--   0        0        0      486 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/lock.png
--rw-r--r--   0        0        0      446 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/log-in.png
--rw-r--r--   0        0        0      431 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/log-out.png
--rw-r--r--   0        0        0      549 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mail.png
--rw-r--r--   0        0        0      783 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/map-pin.png
--rw-r--r--   0        0        0      510 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/map.png
--rw-r--r--   0        0        0      430 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/maximize-2.png
--rw-r--r--   0        0        0      401 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/maximize.png
--rw-r--r--   0        0        0      681 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/meh.png
--rw-r--r--   0        0        0      207 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/menu.png
--rw-r--r--   0        0        0      616 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/message-circle.png
--rw-r--r--   0        0        0      364 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/message-square.png
--rw-r--r--   0        0        0      691 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mic-off.png
--rw-r--r--   0        0        0      591 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mic.png
--rw-r--r--   0        0        0      446 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minimize-2.png
--rw-r--r--   0        0        0      434 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minimize.png
--rw-r--r--   0        0        0      671 2023-11-13 19:22:26.900688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minus-circle.png
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minus-square.png
--rw-r--r--   0        0        0      204 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minus.png
--rw-r--r--   0        0        0      398 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/monitor.png
--rw-r--r--   0        0        0      618 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/moon.png
--rw-r--r--   0        0        0      301 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/more-horizontal.png
--rw-r--r--   0        0        0      347 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/more-vertical.png
--rw-r--r--   0        0        0      555 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mouse-pointer.png
--rw-r--r--   0        0        0      380 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/move.png
--rw-r--r--   0        0        0      559 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/music.png
--rw-r--r--   0        0        0      567 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/navigation-2.png
--rw-r--r--   0        0        0      573 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/navigation.png
--rw-r--r--   0        0        0      380 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/octagon.png
--rw-r--r--   0        0        0      664 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/package.png
--rw-r--r--   0        0        0      597 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/paperclip.png
--rw-r--r--   0        0        0      678 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pause-circle.png
--rw-r--r--   0        0        0      340 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pause.png
--rw-r--r--   0        0        0      686 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pen-tool.png
--rw-r--r--   0        0        0      481 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/percent.png
--rw-r--r--   0        0        0      810 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-call.png
--rw-r--r--   0        0        0      749 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-forwarded.png
--rw-r--r--   0        0        0      774 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-incoming.png
--rw-r--r--   0        0        0      762 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-missed.png
--rw-r--r--   0        0        0      715 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-off.png
--rw-r--r--   0        0        0      761 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-outgoing.png
--rw-r--r--   0        0        0      675 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone.png
--rw-r--r--   0        0        0      658 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pie-chart.png
--rw-r--r--   0        0        0      733 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/play-circle.png
--rw-r--r--   0        0        0      372 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/play.png
--rw-r--r--   0        0        0      714 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/plus-circle.png
--rw-r--r--   0        0        0      440 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/plus-square.png
--rw-r--r--   0        0        0      280 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/plus.png
--rw-r--r--   0        0        0      581 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pocket.png
--rw-r--r--   0        0        0      599 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/power.png
--rw-r--r--   0        0        0      495 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/printer.png
--rw-r--r--   0        0        0      653 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/radio.png
--rw-r--r--   0        0        0      646 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/refresh-ccw.png
--rw-r--r--   0        0        0      640 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/refresh-cw.png
--rw-r--r--   0        0        0      496 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/repeat.png
--rw-r--r--   0        0        0      478 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rewind.png
--rw-r--r--   0        0        0      635 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rotate-ccw.png
--rw-r--r--   0        0        0      628 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rotate-cw.png
--rw-r--r--   0        0        0      577 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rss.png
--rw-r--r--   0        0        0      502 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/save.png
--rw-r--r--   0        0        0      533 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/scissors.png
--rw-r--r--   0        0        0      588 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/search.png
--rw-r--r--   0        0        0      609 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/send.png
--rw-r--r--   0        0        0      364 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/server.png
--rw-r--r--   0        0        0      829 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/settings.png
--rw-r--r--   0        0        0      594 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/share-2.png
--rw-r--r--   0        0        0      418 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/share.png
--rw-r--r--   0        0        0      592 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shield-off.png
--rw-r--r--   0        0        0      536 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shield.png
--rw-r--r--   0        0        0      565 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shopping-bag.png
--rw-r--r--   0        0        0      537 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shopping-cart.png
--rw-r--r--   0        0        0      399 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shuffle.png
--rw-r--r--   0        0        0      352 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sidebar.png
--rw-r--r--   0        0        0      439 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/skip-back.png
--rw-r--r--   0        0        0      444 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/skip-forward.png
--rw-r--r--   0        0        0      681 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/slack.png
--rw-r--r--   0        0        0      659 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/slash.png
--rw-r--r--   0        0        0      531 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sliders.png
--rw-r--r--   0        0        0      364 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/smartphone.png
--rw-r--r--   0        0        0      710 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/smile.png
--rw-r--r--   0        0        0      609 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/speaker.png
--rw-r--r--   0        0        0      320 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/square.png
--rw-r--r--   0        0        0      651 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/star.png
--rw-r--r--   0        0        0      710 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/stop-circle.png
--rw-r--r--   0        0        0      570 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sun.png
--rw-r--r--   0        0        0      574 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sunrise.png
--rw-r--r--   0        0        0      571 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sunset.png
--rw-r--r--   0        0        0      367 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/tablet.png
--rw-r--r--   0        0        0      416 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/tag.png
--rw-r--r--   0        0        0      872 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/target.png
--rw-r--r--   0        0        0      310 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/terminal.png
--rw-r--r--   0        0        0      452 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/thermometer.png
--rw-r--r--   0        0        0      577 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/thumbs-down.png
--rw-r--r--   0        0        0      564 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/thumbs-up.png
--rw-r--r--   0        0        0      597 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/toggle-left.png
--rw-r--r--   0        0        0      595 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/toggle-right.png
--rw-r--r--   0        0        0      582 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/tool.png
--rw-r--r--   0        0        0      492 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/trash-2.png
--rw-r--r--   0        0        0      427 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/trash.png
--rw-r--r--   0        0        0      467 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/trello.png
--rw-r--r--   0        0        0      367 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/trending-down.png
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/trending-up.png
--rw-r--r--   0        0        0      551 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/triangle.png
--rw-r--r--   0        0        0      595 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/truck.png
--rw-r--r--   0        0        0      409 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/tv.png
--rw-r--r--   0        0        0      508 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/twitch.png
--rw-r--r--   0        0        0      729 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/twitter.png
--rw-r--r--   0        0        0      346 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/type.png
--rw-r--r--   0        0        0      566 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/umbrella.png
--rw-r--r--   0        0        0      406 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/underline.png
--rw-r--r--   0        0        0      501 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/unlock.png
--rw-r--r--   0        0        0      615 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/upload-cloud.png
--rw-r--r--   0        0        0      393 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/upload.png
--rw-r--r--   0        0        0      609 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-check.png
--rw-r--r--   0        0        0      579 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-minus.png
--rw-r--r--   0        0        0      614 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-plus.png
--rw-r--r--   0        0        0      649 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-x.png
--rw-r--r--   0        0        0      537 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user.png
--rw-r--r--   0        0        0      660 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/users.png
--rw-r--r--   0        0        0      558 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/video-off.png
--rw-r--r--   0        0        0      457 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/video.png
--rw-r--r--   0        0        0      536 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/voicemail.png
--rw-r--r--   0        0        0      442 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/volume-1.png
--rw-r--r--   0        0        0      547 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/volume-2.png
--rw-r--r--   0        0        0      450 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/volume-x.png
--rw-r--r--   0        0        0      344 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/volume.png
--rw-r--r--   0        0        0      676 2023-11-13 19:22:26.904688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/watch.png
--rw-r--r--   0        0        0      587 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wifi-off.png
--rw-r--r--   0        0        0      564 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wifi.png
--rw-r--r--   0        0        0      527 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wind.png
--rw-r--r--   0        0        0      705 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/x-circle.png
--rw-r--r--   0        0        0      510 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/x-octagon.png
--rw-r--r--   0        0        0      504 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/x-square.png
--rw-r--r--   0        0        0      265 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/x.png
--rw-r--r--   0        0        0      663 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/youtube.png
--rw-r--r--   0        0        0      607 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zap-off.png
--rw-r--r--   0        0        0      560 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zap.png
--rw-r--r--   0        0        0      657 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zoom-in.png
--rw-r--r--   0        0        0      629 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zoom-out.png
--rw-r--r--   0        0        0      282 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/activity.svg
--rw-r--r--   0        0        0      362 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/airplay.svg
--rw-r--r--   0        0        0      356 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/alert-circle.svg
--rw-r--r--   0        0        0      416 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/alert-octagon.svg
--rw-r--r--   0        0        0      424 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/alert-triangle.svg
--rw-r--r--   0        0        0      398 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/align-center.svg
--rw-r--r--   0        0        0      399 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/align-justify.svg
--rw-r--r--   0        0        0      396 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/align-left.svg
--rw-r--r--   0        0        0      397 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/align-right.svg
--rw-r--r--   0        0        0      345 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/anchor.svg
--rw-r--r--   0        0        0      568 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/aperture.svg
--rw-r--r--   0        0        0      361 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/archive.svg
--rw-r--r--   0        0        0      360 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-down-circle.svg
--rw-r--r--   0        0        0      315 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-down-left.svg
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-down-right.svg
--rw-r--r--   0        0        0      313 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-down.svg
--rw-r--r--   0        0        0      359 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-left-circle.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-left.svg
--rw-r--r--   0        0        0      361 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-right-circle.svg
--rw-r--r--   0        0        0      314 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-right.svg
--rw-r--r--   0        0        0      357 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-up-circle.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-up-left.svg
--rw-r--r--   0        0        0      314 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-up-right.svg
--rw-r--r--   0        0        0      310 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/arrow-up.svg
--rw-r--r--   0        0        0      322 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/at-sign.svg
--rw-r--r--   0        0        0      325 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/award.svg
--rw-r--r--   0        0        0      355 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bar-chart-2.svg
--rw-r--r--   0        0        0      353 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bar-chart.svg
--rw-r--r--   0        0        0      427 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/battery-charging.svg
--rw-r--r--   0        0        0      326 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/battery.svg
--rw-r--r--   0        0        0      460 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bell-off.svg
--rw-r--r--   0        0        0      321 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bell.svg
--rw-r--r--   0        0        0      298 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bluetooth.svg
--rw-r--r--   0        0        0      327 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bold.svg
--rw-r--r--   0        0        0      339 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/book-open.svg
--rw-r--r--   0        0        0      345 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/book.svg
--rw-r--r--   0        0        0      287 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/bookmark.svg
--rw-r--r--   0        0        0      462 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/box.svg
--rw-r--r--   0        0        0      343 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/briefcase.svg
--rw-r--r--   0        0        0      410 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/calendar.svg
--rw-r--r--   0        0        0      385 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/camera-off.svg
--rw-r--r--   0        0        0      356 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/camera.svg
--rw-r--r--   0        0        0      387 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cast.svg
--rw-r--r--   0        0        0      328 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/check-circle.svg
--rw-r--r--   0        0        0      345 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/check-square.svg
--rw-r--r--   0        0        0      262 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/check.svg
--rw-r--r--   0        0        0      269 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevron-down.svg
--rw-r--r--   0        0        0      270 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevron-left.svg
--rw-r--r--   0        0        0      270 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevron-right.svg
--rw-r--r--   0        0        0      268 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevron-up.svg
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevrons-down.svg
--rw-r--r--   0        0        0      318 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevrons-left.svg
--rw-r--r--   0        0        0      318 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevrons-right.svg
--rw-r--r--   0        0        0      316 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chevrons-up.svg
--rw-r--r--   0        0        0      448 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/chrome.svg
--rw-r--r--   0        0        0      258 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/circle.svg
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/clipboard.svg
--rw-r--r--   0        0        0      304 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/clock.svg
--rw-r--r--   0        0        0      557 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-drizzle.svg
--rw-r--r--   0        0        0      345 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-lightning.svg
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-off.svg
--rw-r--r--   0        0        0      421 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-rain.svg
--rw-r--r--   0        0        0      572 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-snow.svg
--rw-r--r--   0        0        0      280 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud.svg
--rw-r--r--   0        0        0      307 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/code.svg
--rw-r--r--   0        0        0      486 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/codepen.svg
--rw-r--r--   0        0        0      638 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/codesandbox.svg
--rw-r--r--   0        0        0      447 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/coffee.svg
--rw-r--r--   0        0        0      326 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/columns.svg
--rw-r--r--   0        0        0      421 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/command.svg
--rw-r--r--   0        0        0      342 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/compass.svg
--rw-r--r--   0        0        0      351 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/copy.svg
--rw-r--r--   0        0        0      314 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-down-left.svg
--rw-r--r--   0        0        0      318 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-down-right.svg
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-left-down.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-left-up.svg
--rw-r--r--   0        0        0      318 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-right-down.svg
--rw-r--r--   0        0        0      313 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-right-up.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-up-left.svg
--rw-r--r--   0        0        0      316 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/corner-up-right.svg
--rw-r--r--   0        0        0      667 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cpu.svg
--rw-r--r--   0        0        0      329 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/credit-card.svg
--rw-r--r--   0        0        0      310 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/crop.svg
--rw-r--r--   0        0        0      437 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/crosshair.svg
--rw-r--r--   0        0        0      372 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/database.svg
--rw-r--r--   0        0        0      374 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/delete.svg
--rw-r--r--   0        0        0      295 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/disc.svg
--rw-r--r--   0        0        0      334 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/dollar-sign.svg
--rw-r--r--   0        0        0      387 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/download-cloud.svg
--rw-r--r--   0        0        0      370 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/download.svg
--rw-r--r--   0        0        0      274 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/droplet.svg
--rw-r--r--   0        0        0      291 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/edit-2.svg
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/edit-3.svg
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/edit.svg
--rw-r--r--   0        0        0      388 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/external-link.svg
--rw-r--r--   0        0        0      460 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/eye-off.svg
--rw-r--r--   0        0        0      316 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/eye.svg
--rw-r--r--   0        0        0      303 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/facebook.svg
--rw-r--r--   0        0        0      323 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/fast-forward.svg
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/feather.svg
--rw-r--r--   0        0        0      553 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/figma.svg
--rw-r--r--   0        0        0      387 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/file-minus.svg
--rw-r--r--   0        0        0      431 2023-11-13 19:22:26.908688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/file-plus.svg
--rw-r--r--   0        0        0      473 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/file-text.svg
--rw-r--r--   0        0        0      337 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/file.svg
--rw-r--r--   0        0        0      586 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/film.svg
--rw-r--r--   0        0        0      290 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/filter.svg
--rw-r--r--   0        0        0      334 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/flag.svg
--rw-r--r--   0        0        0      361 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/folder-minus.svg
--rw-r--r--   0        0        0      405 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/folder-plus.svg
--rw-r--r--   0        0        0      311 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/folder.svg
--rw-r--r--   0        0        0      278 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/framer.svg
--rw-r--r--   0        0        0      390 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/frown.svg
--rw-r--r--   0        0        0      481 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/gift.svg
--rw-r--r--   0        0        0      377 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/git-branch.svg
--rw-r--r--   0        0        0      358 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/git-commit.svg
--rw-r--r--   0        0        0      336 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/git-merge.svg
--rw-r--r--   0        0        0      387 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/git-pull-request.svg
--rw-r--r--   0        0        0      527 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/github.svg
--rw-r--r--   0        0        0      490 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/gitlab.svg
--rw-r--r--   0        0        0      409 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/globe.svg
--rw-r--r--   0        0        0      404 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/grid.svg
--rw-r--r--   0        0        0      484 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/hard-drive.svg
--rw-r--r--   0        0        0      389 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/hash.svg
--rw-r--r--   0        0        0      395 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/headphones.svg
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/heart.svg
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/help-circle.svg
--rw-r--r--   0        0        0      358 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/hexagon.svg
--rw-r--r--   0        0        0      332 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/home.svg
--rw-r--r--   0        0        0      369 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/image.svg
--rw-r--r--   0        0        0      405 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/inbox.svg
--rw-r--r--   0        0        0      347 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/info.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/instagram.svg
--rw-r--r--   0        0        0      348 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/italic.svg
--rw-r--r--   0        0        0      352 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/key.svg
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/layers.svg
--rw-r--r--   0        0        0      364 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/layout.svg
--rw-r--r--   0        0        0      575 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/life-buoy.svg
--rw-r--r--   0        0        0      355 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/link-2.svg
--rw-r--r--   0        0        0      371 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/link.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/linkedin.svg
--rw-r--r--   0        0        0      482 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/list.svg
--rw-r--r--   0        0        0      614 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/loader.svg
--rw-r--r--   0        0        0      321 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/lock.svg
--rw-r--r--   0        0        0      368 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/log-in.svg
--rw-r--r--   0        0        0      367 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/log-out.svg
--rw-r--r--   0        0        0      354 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/mail.svg
--rw-r--r--   0        0        0      322 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/map-pin.svg
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/map.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/maximize-2.svg
--rw-r--r--   0        0        0      331 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/maximize.svg
--rw-r--r--   0        0        0      389 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/meh.svg
--rw-r--r--   0        0        0      346 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/menu.svg
--rw-r--r--   0        0        0      428 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/message-circle.svg
--rw-r--r--   0        0        0      305 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/message-square.svg
--rw-r--r--   0        0        0      494 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/mic-off.svg
--rw-r--r--   0        0        0      418 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/mic.svg
--rw-r--r--   0        0        0      404 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/minimize-2.svg
--rw-r--r--   0        0        0      331 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/minimize.svg
--rw-r--r--   0        0        0      308 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/minus-circle.svg
--rw-r--r--   0        0        0      330 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/minus-square.svg
--rw-r--r--   0        0        0      261 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/minus.svg
--rw-r--r--   0        0        0      370 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/monitor.svg
--rw-r--r--   0        0        0      281 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/moon.svg
--rw-r--r--   0        0        0      343 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/more-horizontal.svg
--rw-r--r--   0        0        0      341 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/more-vertical.svg
--rw-r--r--   0        0        0      311 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/mouse-pointer.svg
--rw-r--r--   0        0        0      486 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/move.svg
--rw-r--r--   0        0        0      327 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/music.svg
--rw-r--r--   0        0        0      279 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/navigation-2.svg
--rw-r--r--   0        0        0      277 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/navigation.svg
--rw-r--r--   0        0        0      318 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/octagon.svg
--rw-r--r--   0        0        0      517 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/package.svg
--rw-r--r--   0        0        0      352 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/paperclip.svg
--rw-r--r--   0        0        0      352 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/pause-circle.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/pause.svg
--rw-r--r--   0        0        0      391 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/pen-tool.svg
--rw-r--r--   0        0        0      350 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/percent.svg
--rw-r--r--   0        0        0      576 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-call.svg
--rw-r--r--   0        0        0      618 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-forwarded.svg
--rw-r--r--   0        0        0      617 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-incoming.svg
--rw-r--r--   0        0        0      613 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-missed.svg
--rw-r--r--   0        0        0      591 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-off.svg
--rw-r--r--   0        0        0      617 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-outgoing.svg
--rw-r--r--   0        0        0      520 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone.svg
--rw-r--r--   0        0        0      315 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/pie-chart.svg
--rw-r--r--   0        0        0      313 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/play-circle.svg
--rw-r--r--   0        0        0      263 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/play.svg
--rw-r--r--   0        0        0      351 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/plus-circle.svg
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/plus-square.svg
--rw-r--r--   0        0        0      304 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/plus.svg
--rw-r--r--   0        0        0      358 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/pocket.svg
--rw-r--r--   0        0        0      308 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/power.svg
--rw-r--r--   0        0        0      407 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/printer.svg
--rw-r--r--   0        0        0      389 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/radio.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/refresh-ccw.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/refresh-cw.svg
--rw-r--r--   0        0        0      392 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/repeat.svg
--rw-r--r--   0        0        0      319 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/rewind.svg
--rw-r--r--   0        0        0      317 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/rotate-ccw.svg
--rw-r--r--   0        0        0      321 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/rotate-cw.svg
--rw-r--r--   0        0        0      330 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/rss.svg
--rw-r--r--   0        0        0      392 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/save.svg
--rw-r--r--   0        0        0      444 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/scissors.svg
--rw-r--r--   0        0        0      308 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/search.svg
--rw-r--r--   0        0        0      314 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/send.svg
--rw-r--r--   0        0        0      431 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/server.svg
--rw-r--r--   0        0        0     1011 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/settings.svg
--rw-r--r--   0        0        0      445 2023-11-13 19:22:26.912688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/share-2.svg
--rw-r--r--   0        0        0      364 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/share.svg
--rw-r--r--   0        0        0      405 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/shield-off.svg
--rw-r--r--   0        0        0      279 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/shield.svg
--rw-r--r--   0        0        0      372 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/shopping-bag.svg
--rw-r--r--   0        0        0      383 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/shopping-cart.svg
--rw-r--r--   0        0        0      441 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/shuffle.svg
--rw-r--r--   0        0        0      323 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sidebar.svg
--rw-r--r--   0        0        0      313 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/skip-back.svg
--rw-r--r--   0        0        0      315 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/skip-forward.svg
--rw-r--r--   0        0        0      999 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/slack.svg
--rw-r--r--   0        0        0      312 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/slash.svg
--rw-r--r--   0        0        0      611 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sliders.svg
--rw-r--r--   0        0        0      332 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/smartphone.svg
--rw-r--r--   0        0        0      388 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/smile.svg
--rw-r--r--   0        0        0      366 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/speaker.svg
--rw-r--r--   0        0        0      280 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/square.svg
--rw-r--r--   0        0        0      339 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/star.svg
--rw-r--r--   0        0        0      309 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/stop-circle.svg
--rw-r--r--   0        0        0      650 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sun.svg
--rw-r--r--   0        0        0      589 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sunrise.svg
--rw-r--r--   0        0        0      588 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sunset.svg
--rw-r--r--   0        0        0      328 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/tablet.svg
--rw-r--r--   0        0        0      355 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/tag.svg
--rw-r--r--   0        0        0      336 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/target.svg
--rw-r--r--   0        0        0      310 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/terminal.svg
--rw-r--r--   0        0        0      297 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/thermometer.svg
--rw-r--r--   0        0        0      374 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/thumbs-down.svg
--rw-r--r--   0        0        0      354 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/thumbs-up.svg
--rw-r--r--   0        0        0      323 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/toggle-left.svg
--rw-r--r--   0        0        0      325 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/toggle-right.svg
--rw-r--r--   0        0        0      386 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/tool.svg
--rw-r--r--   0        0        0      448 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/trash-2.svg
--rw-r--r--   0        0        0      356 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/trash.svg
--rw-r--r--   0        0        0      373 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/trello.svg
--rw-r--r--   0        0        0      331 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/trending-down.svg
--rw-r--r--   0        0        0      328 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/trending-up.svg
--rw-r--r--   0        0        0      326 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/triangle.svg
--rw-r--r--   0        0        0      415 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/truck.svg
--rw-r--r--   0        0        0      320 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/tv.svg
--rw-r--r--   0        0        0      277 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/twitch.svg
--rw-r--r--   0        0        0      408 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/twitter.svg
--rw-r--r--   0        0        0      352 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/type.svg
--rw-r--r--   0        0        0      290 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/umbrella.svg
--rw-r--r--   0        0        0      319 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/underline.svg
--rw-r--r--   0        0        0      322 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/unlock.svg
--rw-r--r--   0        0        0      431 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/upload-cloud.svg
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/upload.svg
--rw-r--r--   0        0        0      367 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/user-check.svg
--rw-r--r--   0        0        0      365 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/user-minus.svg
--rw-r--r--   0        0        0      408 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/user-plus.svg
--rw-r--r--   0        0        0      404 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/user-x.svg
--rw-r--r--   0        0        0      313 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/user.svg
--rw-r--r--   0        0        0      400 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/users.svg
--rw-r--r--   0        0        0      379 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/video-off.svg
--rw-r--r--   0        0        0      329 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/video.svg
--rw-r--r--   0        0        0      358 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/voicemail.svg
--rw-r--r--   0        0        0      328 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/volume-1.svg
--rw-r--r--   0        0        0      359 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/volume-2.svg
--rw-r--r--   0        0        0      370 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/volume-x.svg
--rw-r--r--   0        0        0      280 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/volume.svg
--rw-r--r--   0        0        0      462 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/watch.svg
--rw-r--r--   0        0        0      569 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/wifi-off.svg
--rw-r--r--   0        0        0      401 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/wifi.svg
--rw-r--r--   0        0        0      326 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/wind.svg
--rw-r--r--   0        0        0      346 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/x-circle.svg
--rw-r--r--   0        0        0      406 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/x-octagon.svg
--rw-r--r--   0        0        0      368 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/x-square.svg
--rw-r--r--   0        0        0      299 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/x.svg
--rw-r--r--   0        0        0      565 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/youtube.svg
--rw-r--r--   0        0        0      433 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/zap-off.svg
--rw-r--r--   0        0        0      282 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/zap.svg
--rw-r--r--   0        0        0      397 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/zoom-in.svg
--rw-r--r--   0        0        0      354 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/zoom-out.svg
--rw-r--r--   0        0        0    49636 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/layout.py
--rw-r--r--   0        0        0     9263 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/css/buttons.dataTables.min.css
--rw-r--r--   0        0        0      431 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/css/common.scss
--rw-r--r--   0        0        0     3861 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/css/mixins.scss
--rw-r--r--   0        0        0     2805 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.colVis.min.js
--rw-r--r--   0        0        0    26003 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.flash.min.js
--rw-r--r--   0        0        0    42712 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.js
--rw-r--r--   0        0        0    23960 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.min.js
--rw-r--r--   0        0        0     1955 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.print.min.js
--rw-r--r--   0        0        0    17885 2023-11-13 19:22:26.916688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/dataTables.buttons.min.js
--rw-r--r--   0        0        0    64603 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/swf/flashExport.swf
--rw-r--r--   0        0        0      178 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/ColReorder-1.4.1/css/colReorder.dataTables.min.css
--rw-r--r--   0        0        0    12024 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/ColReorder-1.4.1/js/dataTables.colReorder.min.js
--rw-r--r--   0        0        0    14060 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/css/jquery.dataTables.min.css
--rw-r--r--   0        0        0      160 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_asc.png
--rw-r--r--   0        0        0      148 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_asc_disabled.png
--rw-r--r--   0        0        0      201 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_both.png
--rw-r--r--   0        0        0      158 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_desc.png
--rw-r--r--   0        0        0      146 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_desc_disabled.png
--rw-r--r--   0        0        0    81906 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/js/jquery.dataTables.min.js
--rw-r--r--   0        0        0      327 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedColumns-3.2.4/css/fixedColumns.dataTables.min.css
--rw-r--r--   0        0        0    16664 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedColumns-3.2.4/js/dataTables.fixedColumns.min.js
--rw-r--r--   0        0        0      267 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedHeader-3.1.3/css/fixedHeader.dataTables.min.css
--rw-r--r--   0        0        0     6730 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedHeader-3.1.3/js/dataTables.fixedHeader.min.js
--rw-r--r--   0        0        0    76985 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/JSZip-2.5.0/jszip.min.js
--rw-r--r--   0        0        0     3929 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Responsive-2.2.1/css/responsive.dataTables.min.css
--rw-r--r--   0        0        0    12713 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Responsive-2.2.1/js/dataTables.responsive.min.js
--rw-r--r--   0        0        0      369 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Scroller-1.4.4/css/scroller.dataTables.min.css
--rw-r--r--   0        0        0    12072 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/Scroller-1.4.4/js/dataTables.scroller.min.js
--rw-r--r--   0        0        0    29130 2023-11-13 19:22:26.920688 sphinx_needs-2.0.0/sphinx_needs/libs/html/datatables.min.css
--rw-r--r--   0        0        0  2261667 2023-11-13 19:22:26.932689 sphinx_needs-2.0.0/sphinx_needs/libs/html/datatables.min.js
--rw-r--r--   0        0        0      376 2023-11-13 19:22:26.932689 sphinx_needs-2.0.0/sphinx_needs/libs/html/datatables_loader.js
--rw-r--r--   0        0        0  1039577 2023-11-13 19:22:26.936689 sphinx_needs-2.0.0/sphinx_needs/libs/html/pdfmake-0.1.32/pdfmake.min.js
--rw-r--r--   0        0        0   955597 2023-11-13 19:22:26.940689 sphinx_needs-2.0.0/sphinx_needs/libs/html/pdfmake-0.1.32/vfs_fonts.js
--rw-r--r--   0        0        0     2118 2023-11-13 19:22:26.940689 sphinx_needs-2.0.0/sphinx_needs/libs/html/sphinx_needs_collapse.js
--rw-r--r--   0        0        0      171 2023-11-13 19:22:26.940689 sphinx_needs-2.0.0/sphinx_needs/logging.py
--rw-r--r--   0        0        0     4643 2023-11-13 19:22:26.940689 sphinx_needs-2.0.0/sphinx_needs/need_constraints.py
--rw-r--r--   0        0        0    21850 2023-11-13 19:22:26.940689 sphinx_needs-2.0.0/sphinx_needs/needs.py
--rw-r--r--   0        0        0     1493 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/needsfile.json
--rw-r--r--   0        0        0     7331 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/needsfile.py
--rw-r--r--   0        0        0      631 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/nodes/__init__.py
--rw-r--r--   0        0        0      516 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/__init__.py
--rw-r--r--   0        0        0     2001 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_count.py
--rw-r--r--   0        0        0      846 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_func.py
--rw-r--r--   0        0        0     3763 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_incoming.py
--rw-r--r--   0        0        0     6590 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_outgoing.py
--rw-r--r--   0        0        0     2878 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_part.py
--rw-r--r--   0        0        0     5991 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/roles/need_ref.py
--rw-r--r--   0        0        0        0 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/__init__.py
--rw-r--r--   0        0        0      498 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/base.py
--rw-r--r--   0        0        0        0 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/config/__init__.py
--rw-r--r--   0        0        0     1834 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/config/github.py
--rw-r--r--   0        0        0      422 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/config/open_needs.py
--rw-r--r--   0        0        0    14264 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/github.py
--rw-r--r--   0        0        0     1885 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/manager.py
--rw-r--r--   0        0        0     9948 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/services/open_needs.py
--rw-r--r--   0        0        0     2255 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/templates/permalink.html
--rw-r--r--   0        0        0     3939 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/templates/time_measurements.html
--rw-r--r--   0        0        0    24986 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/utils.py
--rw-r--r--   0        0        0     4535 2023-11-13 19:22:26.944689 sphinx_needs-2.0.0/sphinx_needs/warnings.py
--rw-r--r--   0        0        0     5509 1970-01-01 00:00:00.000000 sphinx_needs-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      755 2024-05-08 12:24:04.281272 sphinx_needs-2.1.0/AUTHORS
+-rw-r--r--   0        0        0     1076 2024-05-08 12:24:04.281272 sphinx_needs-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2938 2024-05-08 12:24:04.281272 sphinx_needs-2.1.0/README.rst
+-rw-r--r--   0        0        0     4846 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/__init__.py
+-rw-r--r--   0        0        0      218 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/api/__init__.py
+-rw-r--r--   0        0        0     5439 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/api/configuration.py
+-rw-r--r--   0        0        0      887 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/api/exceptions.py
+-rw-r--r--   0        0        0    33752 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/api/need.py
+-rw-r--r--   0        0        0     9995 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/builder.py
+-rw-r--r--   0        0        0    17106 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/config.py
+-rw-r--r--   0        0        0      998 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/blank/blank.css
+-rw-r--r--   0        0        0     2388 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/blank/styles.css
+-rw-r--r--   0        0        0     3284 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/common.css
+-rw-r--r--   0        0        0     3727 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/dark/dark.css
+-rw-r--r--   0        0        0     2676 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/dark/layouts.css
+-rw-r--r--   0        0        0     2854 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/dark/styles.css
+-rw-r--r--   0        0        0        1 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/grids.css
+-rw-r--r--   0        0        0     2678 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/modern/layouts.css
+-rw-r--r--   0        0        0      453 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/modern/modern.css
+-rw-r--r--   0        0        0     3104 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/css/modern/styles.css
+-rw-r--r--   0        0        0    21046 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/data.py
+-rw-r--r--   0        0        0     6490 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/debug.py
+-rw-r--r--   0        0        0     7035 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/defaults.py
+-rw-r--r--   0        0        0     7622 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/diagrams_common.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/__init__.py
+-rw-r--r--   0        0        0     9417 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/list2need.py
+-rw-r--r--   0        0        0    22940 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/need.py
+-rw-r--r--   0        0        0    18281 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needbar.py
+-rw-r--r--   0        0        0     8492 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needextend.py
+-rw-r--r--   0        0        0     5126 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needextract.py
+-rw-r--r--   0        0        0    11501 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needfilter.py
+-rw-r--r--   0        0        0    21280 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needflow.py
+-rw-r--r--   0        0        0    14360 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needgantt.py
+-rw-r--r--   0        0        0    10763 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needimport.py
+-rw-r--r--   0        0        0     1425 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needimport_template.rst
+-rw-r--r--   0        0        0     4788 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needlist.py
+-rw-r--r--   0        0        0    11140 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needpie.py
+-rw-r--r--   0        0        0     3090 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needreport.py
+-rw-r--r--   0        0        0     1727 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needreport_template.rst
+-rw-r--r--   0        0        0    10734 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needsequence.py
+-rw-r--r--   0        0        0     5031 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needservice.py
+-rw-r--r--   0        0        0    14364 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needtable.py
+-rw-r--r--   0        0        0    18924 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/needuml.py
+-rw-r--r--   0        0        0     3431 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/directives/utils.py
+-rw-r--r--   0        0        0     7779 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/environment.py
+-rw-r--r--   0        0        0      235 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/errors.py
+-rw-r--r--   0        0        0     6471 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/external_needs.py
+-rw-r--r--   0        0        0    13973 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/filter_common.py
+-rw-r--r--   0        0        0      647 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/functions/__init__.py
+-rw-r--r--   0        0        0    15673 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/functions/common.py
+-rw-r--r--   0        0        0    16968 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/functions/functions.py
+-rw-r--r--   0        0        0    20831 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/images/avatar.png
+-rw-r--r--   0        0        0    47870 2024-05-08 12:24:04.349274 sphinx_needs-2.1.0/sphinx_needs/images/avatar.svg
+-rw-r--r--   0        0        0      433 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/activity.png
+-rw-r--r--   0        0        0      485 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/airplay.png
+-rw-r--r--   0        0        0      685 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/alert-circle.png
+-rw-r--r--   0        0        0      445 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/alert-octagon.png
+-rw-r--r--   0        0        0      598 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/alert-triangle.png
+-rw-r--r--   0        0        0      325 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/align-center.png
+-rw-r--r--   0        0        0      284 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/align-justify.png
+-rw-r--r--   0        0        0      308 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/align-left.png
+-rw-r--r--   0        0        0      311 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/align-right.png
+-rw-r--r--   0        0        0      626 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/anchor.png
+-rw-r--r--   0        0        0      842 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/aperture.png
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/archive.png
+-rw-r--r--   0        0        0      729 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-down-circle.png
+-rw-r--r--   0        0        0      283 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-down-left.png
+-rw-r--r--   0        0        0      284 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-down-right.png
+-rw-r--r--   0        0        0      328 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-down.png
+-rw-r--r--   0        0        0      706 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-left-circle.png
+-rw-r--r--   0        0        0      274 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-left.png
+-rw-r--r--   0        0        0      709 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-right-circle.png
+-rw-r--r--   0        0        0      262 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-right.png
+-rw-r--r--   0        0        0      747 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-up-circle.png
+-rw-r--r--   0        0        0      282 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-up-left.png
+-rw-r--r--   0        0        0      277 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-up-right.png
+-rw-r--r--   0        0        0      336 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-up.png
+-rw-r--r--   0        0        0      796 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/at-sign.png
+-rw-r--r--   0        0        0      669 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/award.png
+-rw-r--r--   0        0        0      268 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bar-chart-2.png
+-rw-r--r--   0        0        0      265 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bar-chart.png
+-rw-r--r--   0        0        0      573 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/battery-charging.png
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/battery.png
+-rw-r--r--   0        0        0      607 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bell-off.png
+-rw-r--r--   0        0        0      559 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bell.png
+-rw-r--r--   0        0        0      397 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bluetooth.png
+-rw-r--r--   0        0        0      471 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bold.png
+-rw-r--r--   0        0        0      441 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/book-open.png
+-rw-r--r--   0        0        0      394 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/book.png
+-rw-r--r--   0        0        0      414 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bookmark.png
+-rw-r--r--   0        0        0      615 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/box.png
+-rw-r--r--   0        0        0      485 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/briefcase.png
+-rw-r--r--   0        0        0      499 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/calendar.png
+-rw-r--r--   0        0        0      637 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/camera-off.png
+-rw-r--r--   0        0        0      611 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/camera.png
+-rw-r--r--   0        0        0      549 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cast.png
+-rw-r--r--   0        0        0      686 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/check-circle.png
+-rw-r--r--   0        0        0      446 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/check-square.png
+-rw-r--r--   0        0        0      281 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/check.png
+-rw-r--r--   0        0        0      263 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevron-down.png
+-rw-r--r--   0        0        0      246 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevron-left.png
+-rw-r--r--   0        0        0      246 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevron-right.png
+-rw-r--r--   0        0        0      263 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevron-up.png
+-rw-r--r--   0        0        0      325 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevrons-down.png
+-rw-r--r--   0        0        0      261 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevrons-left.png
+-rw-r--r--   0        0        0      270 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevrons-right.png
+-rw-r--r--   0        0        0      322 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chevrons-up.png
+-rw-r--r--   0        0        0      830 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chrome.png
+-rw-r--r--   0        0        0      634 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/circle.png
+-rw-r--r--   0        0        0      454 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/clipboard.png
+-rw-r--r--   0        0        0      701 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/clock.png
+-rw-r--r--   0        0        0      692 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-drizzle.png
+-rw-r--r--   0        0        0      670 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-lightning.png
+-rw-r--r--   0        0        0      613 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-off.png
+-rw-r--r--   0        0        0      684 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-rain.png
+-rw-r--r--   0        0        0      656 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-snow.png
+-rw-r--r--   0        0        0      578 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud.png
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/code.png
+-rw-r--r--   0        0        0      552 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/codepen.png
+-rw-r--r--   0        0        0      725 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/codesandbox.png
+-rw-r--r--   0        0        0      559 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/coffee.png
+-rw-r--r--   0        0        0      350 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/columns.png
+-rw-r--r--   0        0        0      480 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/command.png
+-rw-r--r--   0        0        0      785 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/compass.png
+-rw-r--r--   0        0        0      512 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/copy.png
+-rw-r--r--   0        0        0      354 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-down-left.png
+-rw-r--r--   0        0        0      367 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-down-right.png
+-rw-r--r--   0        0        0      393 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-left-down.png
+-rw-r--r--   0        0        0      393 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-left-up.png
+-rw-r--r--   0        0        0      397 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-right-down.png
+-rw-r--r--   0        0        0      388 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-right-up.png
+-rw-r--r--   0        0        0      369 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-up-left.png
+-rw-r--r--   0        0        0      375 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/corner-up-right.png
+-rw-r--r--   0        0        0      618 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cpu.png
+-rw-r--r--   0        0        0      351 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/credit-card.png
+-rw-r--r--   0        0        0      437 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/crop.png
+-rw-r--r--   0        0        0      659 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/crosshair.png
+-rw-r--r--   0        0        0      701 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/database.png
+-rw-r--r--   0        0        0      446 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/delete.png
+-rw-r--r--   0        0        0      731 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/disc.png
+-rw-r--r--   0        0        0      510 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/dollar-sign.png
+-rw-r--r--   0        0        0      624 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/download-cloud.png
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/download.png
+-rw-r--r--   0        0        0      555 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/droplet.png
+-rw-r--r--   0        0        0      390 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/edit-2.png
+-rw-r--r--   0        0        0      392 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/edit-3.png
+-rw-r--r--   0        0        0      548 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/edit.png
+-rw-r--r--   0        0        0      532 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/external-link.png
+-rw-r--r--   0        0        0      729 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/eye-off.png
+-rw-r--r--   0        0        0      686 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/eye.png
+-rw-r--r--   0        0        0      526 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/facebook.png
+-rw-r--r--   0        0        0      442 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/fast-forward.png
+-rw-r--r--   0        0        0      555 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/feather.png
+-rw-r--r--   0        0        0      703 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/figma.png
+-rw-r--r--   0        0        0      493 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file-minus.png
+-rw-r--r--   0        0        0      553 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file-plus.png
+-rw-r--r--   0        0        0      545 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file-text.png
+-rw-r--r--   0        0        0      438 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file.png
+-rw-r--r--   0        0        0      581 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/film.png
+-rw-r--r--   0        0        0      489 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/filter.png
+-rw-r--r--   0        0        0      451 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/flag.png
+-rw-r--r--   0        0        0      462 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/folder-minus.png
+-rw-r--r--   0        0        0      539 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/folder-plus.png
+-rw-r--r--   0        0        0      421 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/folder.png
+-rw-r--r--   0        0        0      465 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/framer.png
+-rw-r--r--   0        0        0      717 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/frown.png
+-rw-r--r--   0        0        0      583 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/gift.png
+-rw-r--r--   0        0        0      515 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/git-branch.png
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/git-commit.png
+-rw-r--r--   0        0        0      481 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/git-merge.png
+-rw-r--r--   0        0        0      473 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/git-pull-request.png
+-rw-r--r--   0        0        0      729 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/github.png
+-rw-r--r--   0        0        0      707 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/gitlab.png
+-rw-r--r--   0        0        0      764 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/globe.png
+-rw-r--r--   0        0        0      466 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/grid.png
+-rw-r--r--   0        0        0      514 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/hard-drive.png
+-rw-r--r--   0        0        0      420 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/hash.png
+-rw-r--r--   0        0        0      640 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/headphones.png
+-rw-r--r--   0        0        0      547 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/heart.png
+-rw-r--r--   0        0        0      767 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/help-circle.png
+-rw-r--r--   0        0        0      461 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/hexagon.png
+-rw-r--r--   0        0        0      501 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/home.png
+-rw-r--r--   0        0        0      584 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/image.png
+-rw-r--r--   0        0        0      566 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/inbox.png
+-rw-r--r--   0        0        0      683 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/info.png
+-rw-r--r--   0        0        0      697 2024-05-08 12:24:04.353274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/instagram.png
+-rw-r--r--   0        0        0      378 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/italic.png
+-rw-r--r--   0        0        0      552 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/key.png
+-rw-r--r--   0        0        0      443 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/layers.png
+-rw-r--r--   0        0        0      397 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/layout.png
+-rw-r--r--   0        0        0      776 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/life-buoy.png
+-rw-r--r--   0        0        0      479 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/link-2.png
+-rw-r--r--   0        0        0      654 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/link.png
+-rw-r--r--   0        0        0      615 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/linkedin.png
+-rw-r--r--   0        0        0      227 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/list.png
+-rw-r--r--   0        0        0      396 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/loader.png
+-rw-r--r--   0        0        0      486 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/lock.png
+-rw-r--r--   0        0        0      446 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/log-in.png
+-rw-r--r--   0        0        0      431 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/log-out.png
+-rw-r--r--   0        0        0      549 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mail.png
+-rw-r--r--   0        0        0      783 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/map-pin.png
+-rw-r--r--   0        0        0      510 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/map.png
+-rw-r--r--   0        0        0      430 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/maximize-2.png
+-rw-r--r--   0        0        0      401 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/maximize.png
+-rw-r--r--   0        0        0      681 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/meh.png
+-rw-r--r--   0        0        0      207 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/menu.png
+-rw-r--r--   0        0        0      616 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/message-circle.png
+-rw-r--r--   0        0        0      364 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/message-square.png
+-rw-r--r--   0        0        0      691 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mic-off.png
+-rw-r--r--   0        0        0      591 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mic.png
+-rw-r--r--   0        0        0      446 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minimize-2.png
+-rw-r--r--   0        0        0      434 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minimize.png
+-rw-r--r--   0        0        0      671 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minus-circle.png
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minus-square.png
+-rw-r--r--   0        0        0      204 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minus.png
+-rw-r--r--   0        0        0      398 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/monitor.png
+-rw-r--r--   0        0        0      618 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/moon.png
+-rw-r--r--   0        0        0      301 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/more-horizontal.png
+-rw-r--r--   0        0        0      347 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/more-vertical.png
+-rw-r--r--   0        0        0      555 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mouse-pointer.png
+-rw-r--r--   0        0        0      380 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/move.png
+-rw-r--r--   0        0        0      559 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/music.png
+-rw-r--r--   0        0        0      567 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/navigation-2.png
+-rw-r--r--   0        0        0      573 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/navigation.png
+-rw-r--r--   0        0        0      380 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/octagon.png
+-rw-r--r--   0        0        0      664 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/package.png
+-rw-r--r--   0        0        0      597 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/paperclip.png
+-rw-r--r--   0        0        0      678 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pause-circle.png
+-rw-r--r--   0        0        0      340 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pause.png
+-rw-r--r--   0        0        0      686 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pen-tool.png
+-rw-r--r--   0        0        0      481 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/percent.png
+-rw-r--r--   0        0        0      810 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-call.png
+-rw-r--r--   0        0        0      749 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-forwarded.png
+-rw-r--r--   0        0        0      774 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-incoming.png
+-rw-r--r--   0        0        0      762 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-missed.png
+-rw-r--r--   0        0        0      715 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-off.png
+-rw-r--r--   0        0        0      761 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-outgoing.png
+-rw-r--r--   0        0        0      675 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone.png
+-rw-r--r--   0        0        0      658 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pie-chart.png
+-rw-r--r--   0        0        0      733 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/play-circle.png
+-rw-r--r--   0        0        0      372 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/play.png
+-rw-r--r--   0        0        0      714 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/plus-circle.png
+-rw-r--r--   0        0        0      440 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/plus-square.png
+-rw-r--r--   0        0        0      280 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/plus.png
+-rw-r--r--   0        0        0      581 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pocket.png
+-rw-r--r--   0        0        0      599 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/power.png
+-rw-r--r--   0        0        0      495 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/printer.png
+-rw-r--r--   0        0        0      653 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/radio.png
+-rw-r--r--   0        0        0      646 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/refresh-ccw.png
+-rw-r--r--   0        0        0      640 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/refresh-cw.png
+-rw-r--r--   0        0        0      496 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/repeat.png
+-rw-r--r--   0        0        0      478 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rewind.png
+-rw-r--r--   0        0        0      635 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rotate-ccw.png
+-rw-r--r--   0        0        0      628 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rotate-cw.png
+-rw-r--r--   0        0        0      577 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rss.png
+-rw-r--r--   0        0        0      502 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/save.png
+-rw-r--r--   0        0        0      533 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/scissors.png
+-rw-r--r--   0        0        0      588 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/search.png
+-rw-r--r--   0        0        0      609 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/send.png
+-rw-r--r--   0        0        0      364 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/server.png
+-rw-r--r--   0        0        0      829 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/settings.png
+-rw-r--r--   0        0        0      594 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/share-2.png
+-rw-r--r--   0        0        0      418 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/share.png
+-rw-r--r--   0        0        0      592 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shield-off.png
+-rw-r--r--   0        0        0      536 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shield.png
+-rw-r--r--   0        0        0      565 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shopping-bag.png
+-rw-r--r--   0        0        0      537 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shopping-cart.png
+-rw-r--r--   0        0        0      399 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shuffle.png
+-rw-r--r--   0        0        0      352 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sidebar.png
+-rw-r--r--   0        0        0      439 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/skip-back.png
+-rw-r--r--   0        0        0      444 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/skip-forward.png
+-rw-r--r--   0        0        0      681 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/slack.png
+-rw-r--r--   0        0        0      659 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/slash.png
+-rw-r--r--   0        0        0      531 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sliders.png
+-rw-r--r--   0        0        0      364 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/smartphone.png
+-rw-r--r--   0        0        0      710 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/smile.png
+-rw-r--r--   0        0        0      609 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/speaker.png
+-rw-r--r--   0        0        0      320 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/square.png
+-rw-r--r--   0        0        0      651 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/star.png
+-rw-r--r--   0        0        0      710 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/stop-circle.png
+-rw-r--r--   0        0        0      570 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sun.png
+-rw-r--r--   0        0        0      574 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sunrise.png
+-rw-r--r--   0        0        0      571 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sunset.png
+-rw-r--r--   0        0        0      367 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/tablet.png
+-rw-r--r--   0        0        0      416 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/tag.png
+-rw-r--r--   0        0        0      872 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/target.png
+-rw-r--r--   0        0        0      310 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/terminal.png
+-rw-r--r--   0        0        0      452 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/thermometer.png
+-rw-r--r--   0        0        0      577 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/thumbs-down.png
+-rw-r--r--   0        0        0      564 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/thumbs-up.png
+-rw-r--r--   0        0        0      597 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/toggle-left.png
+-rw-r--r--   0        0        0      595 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/toggle-right.png
+-rw-r--r--   0        0        0      582 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/tool.png
+-rw-r--r--   0        0        0      492 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/trash-2.png
+-rw-r--r--   0        0        0      427 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/trash.png
+-rw-r--r--   0        0        0      467 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/trello.png
+-rw-r--r--   0        0        0      367 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/trending-down.png
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/trending-up.png
+-rw-r--r--   0        0        0      551 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/triangle.png
+-rw-r--r--   0        0        0      595 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/truck.png
+-rw-r--r--   0        0        0      409 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/tv.png
+-rw-r--r--   0        0        0      508 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/twitch.png
+-rw-r--r--   0        0        0      729 2024-05-08 12:24:04.357274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/twitter.png
+-rw-r--r--   0        0        0      346 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/type.png
+-rw-r--r--   0        0        0      566 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/umbrella.png
+-rw-r--r--   0        0        0      406 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/underline.png
+-rw-r--r--   0        0        0      501 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/unlock.png
+-rw-r--r--   0        0        0      615 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/upload-cloud.png
+-rw-r--r--   0        0        0      393 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/upload.png
+-rw-r--r--   0        0        0      609 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-check.png
+-rw-r--r--   0        0        0      579 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-minus.png
+-rw-r--r--   0        0        0      614 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-plus.png
+-rw-r--r--   0        0        0      649 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-x.png
+-rw-r--r--   0        0        0      537 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user.png
+-rw-r--r--   0        0        0      660 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/users.png
+-rw-r--r--   0        0        0      558 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/video-off.png
+-rw-r--r--   0        0        0      457 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/video.png
+-rw-r--r--   0        0        0      536 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/voicemail.png
+-rw-r--r--   0        0        0      442 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/volume-1.png
+-rw-r--r--   0        0        0      547 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/volume-2.png
+-rw-r--r--   0        0        0      450 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/volume-x.png
+-rw-r--r--   0        0        0      344 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/volume.png
+-rw-r--r--   0        0        0      676 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/watch.png
+-rw-r--r--   0        0        0      587 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wifi-off.png
+-rw-r--r--   0        0        0      564 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wifi.png
+-rw-r--r--   0        0        0      527 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wind.png
+-rw-r--r--   0        0        0      705 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/x-circle.png
+-rw-r--r--   0        0        0      510 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/x-octagon.png
+-rw-r--r--   0        0        0      504 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/x-square.png
+-rw-r--r--   0        0        0      265 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/x.png
+-rw-r--r--   0        0        0      663 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/youtube.png
+-rw-r--r--   0        0        0      607 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zap-off.png
+-rw-r--r--   0        0        0      560 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zap.png
+-rw-r--r--   0        0        0      657 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zoom-in.png
+-rw-r--r--   0        0        0      629 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zoom-out.png
+-rw-r--r--   0        0        0      282 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/activity.svg
+-rw-r--r--   0        0        0      362 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/airplay.svg
+-rw-r--r--   0        0        0      356 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/alert-circle.svg
+-rw-r--r--   0        0        0      416 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/alert-octagon.svg
+-rw-r--r--   0        0        0      424 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/alert-triangle.svg
+-rw-r--r--   0        0        0      398 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/align-center.svg
+-rw-r--r--   0        0        0      399 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/align-justify.svg
+-rw-r--r--   0        0        0      396 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/align-left.svg
+-rw-r--r--   0        0        0      397 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/align-right.svg
+-rw-r--r--   0        0        0      345 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/anchor.svg
+-rw-r--r--   0        0        0      568 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/aperture.svg
+-rw-r--r--   0        0        0      361 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/archive.svg
+-rw-r--r--   0        0        0      360 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-down-circle.svg
+-rw-r--r--   0        0        0      315 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-down-left.svg
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-down-right.svg
+-rw-r--r--   0        0        0      313 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-down.svg
+-rw-r--r--   0        0        0      359 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-left-circle.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-left.svg
+-rw-r--r--   0        0        0      361 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-right-circle.svg
+-rw-r--r--   0        0        0      314 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-right.svg
+-rw-r--r--   0        0        0      357 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-up-circle.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-up-left.svg
+-rw-r--r--   0        0        0      314 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-up-right.svg
+-rw-r--r--   0        0        0      310 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/arrow-up.svg
+-rw-r--r--   0        0        0      322 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/at-sign.svg
+-rw-r--r--   0        0        0      325 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/award.svg
+-rw-r--r--   0        0        0      355 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bar-chart-2.svg
+-rw-r--r--   0        0        0      353 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bar-chart.svg
+-rw-r--r--   0        0        0      427 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/battery-charging.svg
+-rw-r--r--   0        0        0      326 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/battery.svg
+-rw-r--r--   0        0        0      460 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bell-off.svg
+-rw-r--r--   0        0        0      321 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bell.svg
+-rw-r--r--   0        0        0      298 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bluetooth.svg
+-rw-r--r--   0        0        0      327 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bold.svg
+-rw-r--r--   0        0        0      339 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/book-open.svg
+-rw-r--r--   0        0        0      345 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/book.svg
+-rw-r--r--   0        0        0      287 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/bookmark.svg
+-rw-r--r--   0        0        0      462 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/box.svg
+-rw-r--r--   0        0        0      343 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/briefcase.svg
+-rw-r--r--   0        0        0      410 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/calendar.svg
+-rw-r--r--   0        0        0      385 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/camera-off.svg
+-rw-r--r--   0        0        0      356 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/camera.svg
+-rw-r--r--   0        0        0      387 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cast.svg
+-rw-r--r--   0        0        0      328 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/check-circle.svg
+-rw-r--r--   0        0        0      345 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/check-square.svg
+-rw-r--r--   0        0        0      262 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/check.svg
+-rw-r--r--   0        0        0      269 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevron-down.svg
+-rw-r--r--   0        0        0      270 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevron-left.svg
+-rw-r--r--   0        0        0      270 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevron-right.svg
+-rw-r--r--   0        0        0      268 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevron-up.svg
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevrons-down.svg
+-rw-r--r--   0        0        0      318 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevrons-left.svg
+-rw-r--r--   0        0        0      318 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevrons-right.svg
+-rw-r--r--   0        0        0      316 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chevrons-up.svg
+-rw-r--r--   0        0        0      448 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/chrome.svg
+-rw-r--r--   0        0        0      258 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/circle.svg
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/clipboard.svg
+-rw-r--r--   0        0        0      304 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/clock.svg
+-rw-r--r--   0        0        0      557 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-drizzle.svg
+-rw-r--r--   0        0        0      345 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-lightning.svg
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-off.svg
+-rw-r--r--   0        0        0      421 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-rain.svg
+-rw-r--r--   0        0        0      572 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-snow.svg
+-rw-r--r--   0        0        0      280 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud.svg
+-rw-r--r--   0        0        0      307 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/code.svg
+-rw-r--r--   0        0        0      486 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/codepen.svg
+-rw-r--r--   0        0        0      638 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/codesandbox.svg
+-rw-r--r--   0        0        0      447 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/coffee.svg
+-rw-r--r--   0        0        0      326 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/columns.svg
+-rw-r--r--   0        0        0      421 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/command.svg
+-rw-r--r--   0        0        0      342 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/compass.svg
+-rw-r--r--   0        0        0      351 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/copy.svg
+-rw-r--r--   0        0        0      314 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-down-left.svg
+-rw-r--r--   0        0        0      318 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-down-right.svg
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-left-down.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-left-up.svg
+-rw-r--r--   0        0        0      318 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-right-down.svg
+-rw-r--r--   0        0        0      313 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-right-up.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-up-left.svg
+-rw-r--r--   0        0        0      316 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/corner-up-right.svg
+-rw-r--r--   0        0        0      667 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cpu.svg
+-rw-r--r--   0        0        0      329 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/credit-card.svg
+-rw-r--r--   0        0        0      310 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/crop.svg
+-rw-r--r--   0        0        0      437 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/crosshair.svg
+-rw-r--r--   0        0        0      372 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/database.svg
+-rw-r--r--   0        0        0      374 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/delete.svg
+-rw-r--r--   0        0        0      295 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/disc.svg
+-rw-r--r--   0        0        0      334 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/dollar-sign.svg
+-rw-r--r--   0        0        0      387 2024-05-08 12:24:04.361274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/download-cloud.svg
+-rw-r--r--   0        0        0      370 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/download.svg
+-rw-r--r--   0        0        0      274 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/droplet.svg
+-rw-r--r--   0        0        0      291 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/edit-2.svg
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/edit-3.svg
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/edit.svg
+-rw-r--r--   0        0        0      388 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/external-link.svg
+-rw-r--r--   0        0        0      460 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/eye-off.svg
+-rw-r--r--   0        0        0      316 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/eye.svg
+-rw-r--r--   0        0        0      303 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/facebook.svg
+-rw-r--r--   0        0        0      323 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/fast-forward.svg
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/feather.svg
+-rw-r--r--   0        0        0      553 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/figma.svg
+-rw-r--r--   0        0        0      387 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/file-minus.svg
+-rw-r--r--   0        0        0      431 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/file-plus.svg
+-rw-r--r--   0        0        0      473 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/file-text.svg
+-rw-r--r--   0        0        0      337 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/file.svg
+-rw-r--r--   0        0        0      586 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/film.svg
+-rw-r--r--   0        0        0      290 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/filter.svg
+-rw-r--r--   0        0        0      334 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/flag.svg
+-rw-r--r--   0        0        0      361 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/folder-minus.svg
+-rw-r--r--   0        0        0      405 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/folder-plus.svg
+-rw-r--r--   0        0        0      311 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/folder.svg
+-rw-r--r--   0        0        0      278 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/framer.svg
+-rw-r--r--   0        0        0      390 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/frown.svg
+-rw-r--r--   0        0        0      481 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/gift.svg
+-rw-r--r--   0        0        0      377 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/git-branch.svg
+-rw-r--r--   0        0        0      358 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/git-commit.svg
+-rw-r--r--   0        0        0      336 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/git-merge.svg
+-rw-r--r--   0        0        0      387 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/git-pull-request.svg
+-rw-r--r--   0        0        0      527 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/github.svg
+-rw-r--r--   0        0        0      490 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/gitlab.svg
+-rw-r--r--   0        0        0      409 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/globe.svg
+-rw-r--r--   0        0        0      404 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/grid.svg
+-rw-r--r--   0        0        0      484 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/hard-drive.svg
+-rw-r--r--   0        0        0      389 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/hash.svg
+-rw-r--r--   0        0        0      395 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/headphones.svg
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/heart.svg
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/help-circle.svg
+-rw-r--r--   0        0        0      358 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/hexagon.svg
+-rw-r--r--   0        0        0      332 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/home.svg
+-rw-r--r--   0        0        0      369 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/image.svg
+-rw-r--r--   0        0        0      405 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/inbox.svg
+-rw-r--r--   0        0        0      347 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/info.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/instagram.svg
+-rw-r--r--   0        0        0      348 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/italic.svg
+-rw-r--r--   0        0        0      352 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/key.svg
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/layers.svg
+-rw-r--r--   0        0        0      364 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/layout.svg
+-rw-r--r--   0        0        0      575 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/life-buoy.svg
+-rw-r--r--   0        0        0      355 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/link-2.svg
+-rw-r--r--   0        0        0      371 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/link.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/linkedin.svg
+-rw-r--r--   0        0        0      482 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/list.svg
+-rw-r--r--   0        0        0      614 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/loader.svg
+-rw-r--r--   0        0        0      321 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/lock.svg
+-rw-r--r--   0        0        0      368 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/log-in.svg
+-rw-r--r--   0        0        0      367 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/log-out.svg
+-rw-r--r--   0        0        0      354 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/mail.svg
+-rw-r--r--   0        0        0      322 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/map-pin.svg
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/map.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/maximize-2.svg
+-rw-r--r--   0        0        0      331 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/maximize.svg
+-rw-r--r--   0        0        0      389 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/meh.svg
+-rw-r--r--   0        0        0      346 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/menu.svg
+-rw-r--r--   0        0        0      428 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/message-circle.svg
+-rw-r--r--   0        0        0      305 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/message-square.svg
+-rw-r--r--   0        0        0      494 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/mic-off.svg
+-rw-r--r--   0        0        0      418 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/mic.svg
+-rw-r--r--   0        0        0      404 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/minimize-2.svg
+-rw-r--r--   0        0        0      331 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/minimize.svg
+-rw-r--r--   0        0        0      308 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/minus-circle.svg
+-rw-r--r--   0        0        0      330 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/minus-square.svg
+-rw-r--r--   0        0        0      261 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/minus.svg
+-rw-r--r--   0        0        0      370 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/monitor.svg
+-rw-r--r--   0        0        0      281 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/moon.svg
+-rw-r--r--   0        0        0      343 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/more-horizontal.svg
+-rw-r--r--   0        0        0      341 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/more-vertical.svg
+-rw-r--r--   0        0        0      311 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/mouse-pointer.svg
+-rw-r--r--   0        0        0      486 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/move.svg
+-rw-r--r--   0        0        0      327 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/music.svg
+-rw-r--r--   0        0        0      279 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/navigation-2.svg
+-rw-r--r--   0        0        0      277 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/navigation.svg
+-rw-r--r--   0        0        0      318 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/octagon.svg
+-rw-r--r--   0        0        0      517 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/package.svg
+-rw-r--r--   0        0        0      352 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/paperclip.svg
+-rw-r--r--   0        0        0      352 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/pause-circle.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/pause.svg
+-rw-r--r--   0        0        0      391 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/pen-tool.svg
+-rw-r--r--   0        0        0      350 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/percent.svg
+-rw-r--r--   0        0        0      576 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-call.svg
+-rw-r--r--   0        0        0      618 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-forwarded.svg
+-rw-r--r--   0        0        0      617 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-incoming.svg
+-rw-r--r--   0        0        0      613 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-missed.svg
+-rw-r--r--   0        0        0      591 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-off.svg
+-rw-r--r--   0        0        0      617 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-outgoing.svg
+-rw-r--r--   0        0        0      520 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone.svg
+-rw-r--r--   0        0        0      315 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/pie-chart.svg
+-rw-r--r--   0        0        0      313 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/play-circle.svg
+-rw-r--r--   0        0        0      263 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/play.svg
+-rw-r--r--   0        0        0      351 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/plus-circle.svg
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/plus-square.svg
+-rw-r--r--   0        0        0      304 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/plus.svg
+-rw-r--r--   0        0        0      358 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/pocket.svg
+-rw-r--r--   0        0        0      308 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/power.svg
+-rw-r--r--   0        0        0      407 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/printer.svg
+-rw-r--r--   0        0        0      389 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/radio.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/refresh-ccw.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/refresh-cw.svg
+-rw-r--r--   0        0        0      392 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/repeat.svg
+-rw-r--r--   0        0        0      319 2024-05-08 12:24:04.365274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/rewind.svg
+-rw-r--r--   0        0        0      317 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/rotate-ccw.svg
+-rw-r--r--   0        0        0      321 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/rotate-cw.svg
+-rw-r--r--   0        0        0      330 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/rss.svg
+-rw-r--r--   0        0        0      392 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/save.svg
+-rw-r--r--   0        0        0      444 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/scissors.svg
+-rw-r--r--   0        0        0      308 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/search.svg
+-rw-r--r--   0        0        0      314 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/send.svg
+-rw-r--r--   0        0        0      431 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/server.svg
+-rw-r--r--   0        0        0     1011 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/settings.svg
+-rw-r--r--   0        0        0      445 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/share-2.svg
+-rw-r--r--   0        0        0      364 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/share.svg
+-rw-r--r--   0        0        0      405 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/shield-off.svg
+-rw-r--r--   0        0        0      279 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/shield.svg
+-rw-r--r--   0        0        0      372 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/shopping-bag.svg
+-rw-r--r--   0        0        0      383 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/shopping-cart.svg
+-rw-r--r--   0        0        0      441 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/shuffle.svg
+-rw-r--r--   0        0        0      323 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sidebar.svg
+-rw-r--r--   0        0        0      313 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/skip-back.svg
+-rw-r--r--   0        0        0      315 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/skip-forward.svg
+-rw-r--r--   0        0        0      999 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/slack.svg
+-rw-r--r--   0        0        0      312 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/slash.svg
+-rw-r--r--   0        0        0      611 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sliders.svg
+-rw-r--r--   0        0        0      332 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/smartphone.svg
+-rw-r--r--   0        0        0      388 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/smile.svg
+-rw-r--r--   0        0        0      366 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/speaker.svg
+-rw-r--r--   0        0        0      280 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/square.svg
+-rw-r--r--   0        0        0      339 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/star.svg
+-rw-r--r--   0        0        0      309 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/stop-circle.svg
+-rw-r--r--   0        0        0      650 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sun.svg
+-rw-r--r--   0        0        0      589 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sunrise.svg
+-rw-r--r--   0        0        0      588 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sunset.svg
+-rw-r--r--   0        0        0      328 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/tablet.svg
+-rw-r--r--   0        0        0      355 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/tag.svg
+-rw-r--r--   0        0        0      336 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/target.svg
+-rw-r--r--   0        0        0      310 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/terminal.svg
+-rw-r--r--   0        0        0      297 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/thermometer.svg
+-rw-r--r--   0        0        0      374 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/thumbs-down.svg
+-rw-r--r--   0        0        0      354 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/thumbs-up.svg
+-rw-r--r--   0        0        0      323 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/toggle-left.svg
+-rw-r--r--   0        0        0      325 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/toggle-right.svg
+-rw-r--r--   0        0        0      386 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/tool.svg
+-rw-r--r--   0        0        0      448 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/trash-2.svg
+-rw-r--r--   0        0        0      356 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/trash.svg
+-rw-r--r--   0        0        0      373 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/trello.svg
+-rw-r--r--   0        0        0      331 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/trending-down.svg
+-rw-r--r--   0        0        0      328 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/trending-up.svg
+-rw-r--r--   0        0        0      326 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/triangle.svg
+-rw-r--r--   0        0        0      415 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/truck.svg
+-rw-r--r--   0        0        0      320 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/tv.svg
+-rw-r--r--   0        0        0      277 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/twitch.svg
+-rw-r--r--   0        0        0      408 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/twitter.svg
+-rw-r--r--   0        0        0      352 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/type.svg
+-rw-r--r--   0        0        0      290 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/umbrella.svg
+-rw-r--r--   0        0        0      319 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/underline.svg
+-rw-r--r--   0        0        0      322 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/unlock.svg
+-rw-r--r--   0        0        0      431 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/upload-cloud.svg
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/upload.svg
+-rw-r--r--   0        0        0      367 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/user-check.svg
+-rw-r--r--   0        0        0      365 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/user-minus.svg
+-rw-r--r--   0        0        0      408 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/user-plus.svg
+-rw-r--r--   0        0        0      404 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/user-x.svg
+-rw-r--r--   0        0        0      313 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/user.svg
+-rw-r--r--   0        0        0      400 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/users.svg
+-rw-r--r--   0        0        0      379 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/video-off.svg
+-rw-r--r--   0        0        0      329 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/video.svg
+-rw-r--r--   0        0        0      358 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/voicemail.svg
+-rw-r--r--   0        0        0      328 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/volume-1.svg
+-rw-r--r--   0        0        0      359 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/volume-2.svg
+-rw-r--r--   0        0        0      370 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/volume-x.svg
+-rw-r--r--   0        0        0      280 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/volume.svg
+-rw-r--r--   0        0        0      462 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/watch.svg
+-rw-r--r--   0        0        0      569 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/wifi-off.svg
+-rw-r--r--   0        0        0      401 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/wifi.svg
+-rw-r--r--   0        0        0      326 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/wind.svg
+-rw-r--r--   0        0        0      346 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/x-circle.svg
+-rw-r--r--   0        0        0      406 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/x-octagon.svg
+-rw-r--r--   0        0        0      368 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/x-square.svg
+-rw-r--r--   0        0        0      299 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/x.svg
+-rw-r--r--   0        0        0      565 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/youtube.svg
+-rw-r--r--   0        0        0      433 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/zap-off.svg
+-rw-r--r--   0        0        0      282 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/zap.svg
+-rw-r--r--   0        0        0      397 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/zoom-in.svg
+-rw-r--r--   0        0        0      354 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/zoom-out.svg
+-rw-r--r--   0        0        0    52314 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/layout.py
+-rw-r--r--   0        0        0     9263 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/css/buttons.dataTables.min.css
+-rw-r--r--   0        0        0      431 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/css/common.scss
+-rw-r--r--   0        0        0     3861 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/css/mixins.scss
+-rw-r--r--   0        0        0     2805 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.colVis.min.js
+-rw-r--r--   0        0        0    26003 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.flash.min.js
+-rw-r--r--   0        0        0    42712 2024-05-08 12:24:04.369274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.js
+-rw-r--r--   0        0        0    23960 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.min.js
+-rw-r--r--   0        0        0     1955 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.print.min.js
+-rw-r--r--   0        0        0    17885 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/dataTables.buttons.min.js
+-rw-r--r--   0        0        0    64603 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/swf/flashExport.swf
+-rw-r--r--   0        0        0      178 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/ColReorder-1.4.1/css/colReorder.dataTables.min.css
+-rw-r--r--   0        0        0    12024 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/ColReorder-1.4.1/js/dataTables.colReorder.min.js
+-rw-r--r--   0        0        0    14060 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/css/jquery.dataTables.min.css
+-rw-r--r--   0        0        0      160 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_asc.png
+-rw-r--r--   0        0        0      148 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_asc_disabled.png
+-rw-r--r--   0        0        0      201 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_both.png
+-rw-r--r--   0        0        0      158 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_desc.png
+-rw-r--r--   0        0        0      146 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/images/sort_desc_disabled.png
+-rw-r--r--   0        0        0    81906 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/js/jquery.dataTables.min.js
+-rw-r--r--   0        0        0      327 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedColumns-3.2.4/css/fixedColumns.dataTables.min.css
+-rw-r--r--   0        0        0    16664 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedColumns-3.2.4/js/dataTables.fixedColumns.min.js
+-rw-r--r--   0        0        0      267 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedHeader-3.1.3/css/fixedHeader.dataTables.min.css
+-rw-r--r--   0        0        0     6730 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedHeader-3.1.3/js/dataTables.fixedHeader.min.js
+-rw-r--r--   0        0        0    76985 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/JSZip-2.5.0/jszip.min.js
+-rw-r--r--   0        0        0     3929 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Responsive-2.2.1/css/responsive.dataTables.min.css
+-rw-r--r--   0        0        0    12713 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Responsive-2.2.1/js/dataTables.responsive.min.js
+-rw-r--r--   0        0        0      369 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Scroller-1.4.4/css/scroller.dataTables.min.css
+-rw-r--r--   0        0        0    12072 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/Scroller-1.4.4/js/dataTables.scroller.min.js
+-rw-r--r--   0        0        0    29130 2024-05-08 12:24:04.373274 sphinx_needs-2.1.0/sphinx_needs/libs/html/datatables.min.css
+-rw-r--r--   0        0        0  2261667 2024-05-08 12:24:04.385275 sphinx_needs-2.1.0/sphinx_needs/libs/html/datatables.min.js
+-rw-r--r--   0        0        0      376 2024-05-08 12:24:04.385275 sphinx_needs-2.1.0/sphinx_needs/libs/html/datatables_loader.js
+-rw-r--r--   0        0        0  1039577 2024-05-08 12:24:04.389275 sphinx_needs-2.1.0/sphinx_needs/libs/html/pdfmake-0.1.32/pdfmake.min.js
+-rw-r--r--   0        0        0   955597 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/libs/html/pdfmake-0.1.32/vfs_fonts.js
+-rw-r--r--   0        0        0     2118 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/libs/html/sphinx_needs_collapse.js
+-rw-r--r--   0        0        0      207 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/logging.py
+-rw-r--r--   0        0        0     4822 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/need_constraints.py
+-rw-r--r--   0        0        0    22811 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/needs.py
+-rw-r--r--   0        0        0     1493 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/needsfile.json
+-rw-r--r--   0        0        0     7604 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/needsfile.py
+-rw-r--r--   0        0        0      631 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/nodes/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/__init__.py
+-rw-r--r--   0        0        0     2478 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_count.py
+-rw-r--r--   0        0        0      901 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_func.py
+-rw-r--r--   0        0        0     4013 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_incoming.py
+-rw-r--r--   0        0        0     5699 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_outgoing.py
+-rw-r--r--   0        0        0     3450 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_part.py
+-rw-r--r--   0        0        0     6094 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/roles/need_ref.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/base.py
+-rw-r--r--   0        0        0        0 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/config/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/config/github.py
+-rw-r--r--   0        0        0      458 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/config/open_needs.py
+-rw-r--r--   0        0        0    15569 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/github.py
+-rw-r--r--   0        0        0     1977 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/manager.py
+-rw-r--r--   0        0        0    10337 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/services/open_needs.py
+-rw-r--r--   0        0        0     2294 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/templates/permalink.html
+-rw-r--r--   0        0        0     3939 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/templates/time_measurements.html
+-rw-r--r--   0        0        0    26555 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/utils.py
+-rw-r--r--   0        0        0     4967 2024-05-08 12:24:04.397275 sphinx_needs-2.1.0/sphinx_needs/warnings.py
+-rw-r--r--   0        0        0     5513 1970-01-01 00:00:00.000000 sphinx_needs-2.1.0/PKG-INFO
```

### Comparing `sphinx_needs-2.0.0/LICENSE` & `sphinx_needs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/README.rst` & `sphinx_needs-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/pyproject.toml` & `sphinx_needs-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sphinx-needs"
 
 # !! Don't miss updates in sphinx_needs.__version__, changelog.rst, and .github/workflows/docker !!!
-version = "2.0.0"
+version = "2.1.0"
 
 description = "Sphinx needs extension for managing needs/requirements and specifications"
 authors = ["team useblocks <info@useblocks.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "http://github.com/useblocks/sphinx-needs"
 documentation = "https://sphinx-needs.readthedocs.io/en/latest/"
@@ -44,19 +44,19 @@
 # for needpie / needbar
 matplotlib = { version = ">=3.3.0", optional = true }
 
 # [project.optional-dependencies.test]
 pytest = { version = "^7", optional = true }
 pytest-cov = { version = "^4", optional = true }
 lxml = { version = "^4.6.5", optional = true }
-requests-mock = { version = ">=1.9.3", optional = true }
 responses = { version = "^0.22.0", optional = true }
 sphinxcontrib-plantuml = { version = "^0", optional = true }
 syrupy = { version = "^3", optional = true }
 pytest-xprocess = { version = "^0.22.2", optional = true }
+defusedxml = { version = "^0.7.1", optional = true }
 
 # [project.optional-dependencies.test-parallel]
 pytest-xdist = { version = "*", optional = true }
 
 # [project.optional-dependencies.benchmark]
 pytest-benchmark = { version = "^4.0.0", optional = true }
 memray = { version = "^1.3.1", optional = true }
@@ -67,20 +67,20 @@
 sphinx-design = { version="^0.5", optional = true }
 sphinx-immaterial = { version="0.11.7", optional = true }
 pydantic = { version="2.4.2", optional = true }
 
 [tool.poetry.extras]
 plotting = ["matplotlib"]
 test = [
+  "defusedxml",
   "matplotlib",
   "pytest",
   "pytest-cov",
   "syrupy",
   "sphinxcontrib-plantuml",
-  "requests-mock",
   "lxml",
   "responses",
   "pytest-xprocess"
 ]
 test-parallel = ["pytest-xdist"]
 benchmark = ["pytest-benchmark", "memray"]
 docs = [
@@ -96,20 +96,33 @@
 [tool.poetry.dev-dependencies]
 pre-commit = "^3"
 
 [tool.pytest.ini_options]
 markers = [
     "jstest: marks tests as JavaScript test (deselect with '-m \"not jstest\"')",
 ]
+filterwarnings = [
+  "ignore:.*removed in Python 3.14.*:DeprecationWarning",
+  # "ignore::sphinx.deprecation.RemovedInSphinx90Warning"
+]
 
-[tool.black]
-line-length = 120
 
-[tool.isort]
-profile = "black"
+[tool.ruff.lint]
+extend-select = [
+  "B",   # flake8-bugbear  
+  "C4",  # flake8-comprehensions
+  "I",   # isort
+  "ICN", # flake8-import-conventions
+  "ISC", # flake8-implicit-str-concat
+  "N",   # pep8-naming
+  "RUF", # Ruff-specific rules
+  "SIM", # flake8-simplify
+  "UP",  # pyupgrade
+]
+extend-ignore = ["B904", "ISC001", "ICN001", "N818", "RUF005", "RUF013", "RUF012", "SIM108", "SIM118"]
 
 [tool.mypy]
 files = "sphinx_needs"
 strict = true
 show_error_codes = true
 implicit_reexport = true
 namespace_packages = true
@@ -128,31 +141,24 @@
   "sphinx_data_viewer.*",
   "sphinxcontrib.plantuml.*",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
-  'sphinx_needs.api.need',
-  'sphinx_needs.directives.needuml',
-]
-ignore_errors = true
-
-[[tool.mypy.overrides]]
-module = [
   "sphinx_needs.directives.needextend",
   "sphinx_needs.functions.functions",
+  "sphinx_needs.api.need",
 ]
 # TODO dynamically overriding TypeDict keys is a bit tricky
 disable_error_code = "literal-required"
 
 [[tool.mypy.overrides]]
 module = [
   "sphinx_needs.data"
 ]
 disable_error_code = ["attr-defined", "no-any-return"]
 
-
 [build-system]
 requires = ["setuptools", "poetry_core>=1.0.8"]  # setuptools for deps like plantuml
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/api/configuration.py` & `sphinx_needs-2.1.0/sphinx_needs/api/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 API to get or add specific sphinx needs configuration parameters.
 
 All functions here are available under ``sphinxcontrib.api``. So do not import this module directly.
 """
-from typing import Callable, List, Optional
+
+from __future__ import annotations
+
+from typing import Callable
 
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.util.logging import SphinxLoggerAdapter
 
 from sphinx_needs.api.exceptions import NeedsApiConfigException, NeedsApiConfigWarning
 from sphinx_needs.config import NEEDS_CONFIG, NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType
 from sphinx_needs.functions import register_func
 from sphinx_needs.functions.functions import DynamicFunction
 
 
-def get_need_types(app: Sphinx) -> List[str]:
+def get_need_types(app: Sphinx) -> list[str]:
     """
     Returns a list of directive-names from all configured need_types.
 
     **Usage**::
 
         from sphinx_needs.api import get_need_types
 
@@ -30,15 +33,20 @@
     :return: list of strings
     """
     needs_types = NeedsSphinxConfig(app.config).types
     return [x["directive"] for x in needs_types]
 
 
 def add_need_type(
-    app: Sphinx, directive: str, title: str, prefix: str, color: str = "#ffffff", style: str = "node"
+    app: Sphinx,
+    directive: str,
+    title: str,
+    prefix: str,
+    color: str = "#ffffff",
+    style: str = "node",
 ) -> None:
     """
     Adds a new need_type to the configuration.
 
     The given directive must no exist, otherwise NeedsApiConfigException gets raised.
 
     Same impact as using :ref:`needs_types` manually.
@@ -61,15 +69,23 @@
 
     needs_types = NeedsSphinxConfig(app.config).types
     type_names = [x["directive"] for x in needs_types]
 
     if directive in type_names:
         raise NeedsApiConfigException(f"{directive} already exists as need type")
 
-    needs_types.append({"directive": directive, "title": title, "prefix": prefix, "color": color, "style": style})
+    needs_types.append(
+        {
+            "directive": directive,
+            "title": title,
+            "prefix": prefix,
+            "color": color,
+            "style": style,
+        }
+    )
     app.add_directive(directive, sphinx_needs.directives.need.NeedDirective)
 
 
 def add_extra_option(app: Sphinx, name: str) -> None:
     """
     Adds an extra option to the configuration. This option can then later be used inside needs or ``add_need``.
 
@@ -86,15 +102,17 @@
     :return: None
     """
     if name in NEEDS_CONFIG.extra_options:
         raise NeedsApiConfigWarning(f"Option {name} already registered.")
     NEEDS_CONFIG.extra_options[name] = directives.unchanged
 
 
-def add_dynamic_function(app: Sphinx, function: DynamicFunction, name: Optional[str] = None) -> None:
+def add_dynamic_function(
+    app: Sphinx, function: DynamicFunction, name: str | None = None
+) -> None:
     """
     Registers a new dynamic function for sphinx-needs.
 
     If ``name`` is not given, the name to call the function is automatically taken from the provided function.
     The used name must be unique.
 
     **Usage**::
@@ -118,33 +136,39 @@
 
 
 # 'Need' is untyped, so we temporarily use 'Any' here
 WarningCheck = Callable[[NeedsInfoType, SphinxLoggerAdapter], bool]
 
 
 def add_warning(
-    app: Sphinx, name: str, function: Optional[WarningCheck] = None, filter_string: Optional[str] = None
+    app: Sphinx,
+    name: str,
+    function: WarningCheck | None = None,
+    filter_string: str | None = None,
 ) -> None:
     """
     Registers a warning.
 
     A warning can be based on the result of a given filter_string or an own defined function.
 
     :param app: Sphinx app object
     :param name: Name as string for the warning
     :param function: function to execute to check the warning
     :param filter_string: filter_string to use for the warning
     :return: None
     """
     if function is None and filter_string is None:
-        raise NeedsApiConfigException("Function or filter_string must be given for add_warning_func")
+        raise NeedsApiConfigException(
+            "Function or filter_string must be given for add_warning_func"
+        )
 
     if function is not None and filter_string is not None:
         raise NeedsApiConfigException(
-            "For add_warning_func only function or filter_string is allowed to be set, " "not both."
+            "For add_warning_func only function or filter_string is allowed to be set, "
+            "not both."
         )
 
     warning_check = function or filter_string
 
     if warning_check is None:
         raise NeedsApiConfigException("either function or filter_string must be given")
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/api/exceptions.py` & `sphinx_needs-2.1.0/sphinx_needs/api/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from sphinx.errors import SphinxError, SphinxWarning
 
 
 class NeedsApiConfigException(SphinxError):
     """
     A configuration changes collides with the already provided configuration by the user.
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/api/need.py` & `sphinx_needs-2.1.0/sphinx_needs/api/need.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,77 @@
+from __future__ import annotations
+
 import hashlib
 import os
 import re
-from typing import Any, List, Optional, Union
+from contextlib import contextmanager
+from typing import Any, Iterator
 
 from docutils import nodes
 from docutils.parsers.rst.states import RSTState
 from docutils.statemachine import StringList
 from jinja2 import Template
 from sphinx.application import Sphinx
-from sphinx.util.nodes import nested_parse_with_titles
+from sphinx.environment import BuildEnvironment
 
 from sphinx_needs.api.configuration import NEEDS_CONFIG
 from sphinx_needs.api.exceptions import (
     NeedsConstraintNotAllowed,
     NeedsDuplicatedId,
     NeedsInvalidException,
     NeedsInvalidOption,
     NeedsNoIdException,
     NeedsStatusNotAllowed,
     NeedsTagNotAllowed,
     NeedsTemplateException,
 )
-from sphinx_needs.config import NeedsSphinxConfig
+from sphinx_needs.config import GlobalOptionsType, NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.directives.needuml import Needuml, NeedumlException
 from sphinx_needs.filter_common import filter_single_need
 from sphinx_needs.logging import get_logger
 from sphinx_needs.nodes import Need
 from sphinx_needs.roles.need_part import find_parts, update_need_with_parts
 from sphinx_needs.utils import jinja_parse
 
 logger = get_logger(__name__)
 
 
 def add_need(
     app: Sphinx,
-    state,
-    docname: str,
-    lineno: int,
-    need_type,
+    state: None | RSTState,
+    docname: None | str,
+    lineno: None | int,
+    need_type: str,
     title: str,
-    id: Optional[str] = None,
-    content: str = "",
-    status: Optional[str] = None,
-    tags=None,
-    constraints=None,
-    constraints_passed=None,
-    links_string: Optional[str] = None,
+    *,
+    id: str | None = None,
+    content: str | StringList = "",
+    lineno_content: None | int = None,
+    status: str | None = None,
+    tags: None | str | list[str] = None,
+    constraints: None | str | list[str] = None,
+    constraints_passed: None | bool = None,
+    links_string: None | str | list[str] = None,
     delete: bool = False,
     jinja_content: bool = False,
     hide: bool = False,
     hide_tags: bool = False,
     hide_status: bool = False,
-    collapse=None,
-    style=None,
-    layout=None,
-    template=None,
-    pre_template: Optional[str] = None,
-    post_template: Optional[str] = None,
+    collapse: None | bool = None,
+    style: None | str = None,
+    layout: None | str = None,
+    template: None | str = None,
+    pre_template: str | None = None,
+    post_template: str | None = None,
     is_external: bool = False,
-    external_url: Optional[str] = None,
+    external_url: str | None = None,
     external_css: str = "external_link",
-    **kwargs,
-):
+    **kwargs: Any,
+) -> list[nodes.Node]:
     """
     Creates a new need and returns its node.
 
     ``add_need`` allows to create needs programmatically and use its returned node to be integrated in any
     docutils based structure.
 
     ``kwags`` can contain options defined in ``needs_extra_options`` and ``needs_extra_links``.
@@ -101,40 +106,51 @@
                                          need_type="req", title="my title", id="ID_001"
                                          content=self.content)
 
                 # Feel free to add custom stuff to main_section like sections, text, ...
 
                 return main_section
 
+    If the need is within the current project, i.e. not an external need,
+    the following parameters are used to help provide source mapped warnings and errors:
+
+    :param docname: documentation identifier, for the referencing document.
+    :param lineno: line number of the top of the directive (1-indexed).
+    :param lineno_content: line number of the content start of the directive (1-indexed).
+
+    Otherwise, the following parameters are used:
+
+    :param is_external: Is true, no node is created and need is referencing external url
+    :param external_url: URL as string, which is used as target if ``is_external`` is ``True``
+    :param external_css: CSS class name as string, which is set for the <a> tag.
+
+    Additional parameters:
+
     :param app: Sphinx application object.
     :param state: Current state object.
-    :param docname: documentation name.
-    :param lineno: line number.
     :param need_type: Name of the need type to create.
     :param title: String as title.
     :param id: ID as string. If not given, an id will get generated.
-    :param content: Content as single string.
+    :param content: Content of the need, either as a ``str``
+        or a ``StringList`` (a string with mapping to the source text).
     :param status: Status as string.
     :param tags: Tags as single string.
     :param constraints: Constraints as single, comma separated, string.
     :param constraints_passed: Contains bool describing if all constraints have passed
-    :param links_string: Links as single string.
+    :param links_string: Links as single string. (Not used)
     :param delete: boolean value (Remove the complete need).
     :param hide: boolean value.
     :param hide_tags: boolean value. (Not used with Sphinx-Needs >0.5.0)
     :param hide_status: boolean value. (Not used with Sphinx-Needs >0.5.0)
     :param collapse: boolean value.
     :param style: String value of class attribute of node.
     :param layout: String value of layout definition to use
     :param template: Template name to use for the content of this need
     :param pre_template: Template name to use for content added before need
     :param post_template: Template name to use for the content added after need
-    :param is_external: Is true, no node is created and need is referencing external url
-    :param external_url: URL as string, which is used as target if ``is_external`` is ``True``
-    :param external_css: CSS class name as string, which is set for the <a> tag.
 
     :return: node
     """
     #############################################################################################
     # Get environment
     #############################################################################################
     env = app.env
@@ -146,24 +162,28 @@
     type_style = ""
     found = False
 
     # Log messages for need elements that could not be imported.
     configured_need_types = [ntype["directive"] for ntype in types]
     if need_type not in configured_need_types:
         logger.warning(
-            "Couldn't create need {}. Reason: The need-type (i.e. `{}`) is not set "
-            "in the project's 'need_types' configuration in conf.py. [needs]".format(id, need_type),
+            f"Couldn't create need {id}. Reason: The need-type (i.e. `{need_type}`) is not set "
+            "in the project's 'need_types' configuration in conf.py. [needs.add]",
             type="needs",
+            subtype="add",
+            location=(docname, lineno) if docname else None,
         )
 
     for ntype in types:
         if ntype["directive"] == need_type:
             type_name = ntype["title"]
             type_prefix = ntype["prefix"]
-            type_color = ntype["color"] or "#000000"  # if no color set up user in config
+            type_color = (
+                ntype["color"] or "#000000"
+            )  # if no color set up user in config
             type_style = ntype["style"] or "node"  # if no style set up user in config
             found = True
             break
 
     if delete:
         # Don't generate a need object if the :delete: option is enabled.
         return [nodes.Text("")]
@@ -178,76 +198,100 @@
     # Get the id or generate a random string/hash string, which is hopefully unique
     # TODO: Check, if id was already given. If True, recalculate id
     # id = self.options.get("id", ''.join(random.SystemRandom().choice(string.ascii_uppercase + string.digits) for
     # _ in range(5)))
     if id is None and needs_config.id_required:
         raise NeedsNoIdException(
             "An id is missing for this need and must be set, because 'needs_id_required' "
-            "is set to True in conf.py. Need '{}' in {} ({})".format(title, docname, lineno)
+            f"is set to True in conf.py. Need '{title}' in {docname} ({lineno})"
         )
 
     if id is None:
-        need_id = make_hashed_id(app, need_type, title, content)
+        need_id = make_hashed_id(
+            app,
+            need_type,
+            title,
+            "\n".join(content) if isinstance(content, StringList) else content,
+        )
     else:
         need_id = id
 
-    if needs_config.id_regex and not re.match(needs_config.id_regex, need_id):
-        raise NeedsInvalidException(f"Given ID '{need_id}' does not match configured regex '{needs_config.id_regex}'")
+    if (
+        needs_config.id_regex
+        and not is_external
+        and not re.match(needs_config.id_regex, need_id)
+    ):
+        raise NeedsInvalidException(
+            f"Given ID '{need_id}' does not match configured regex '{needs_config.id_regex}'"
+        )
 
     # Handle status
     # Check if status is in needs_statuses. If not raise an error.
-    if needs_config.statuses and status not in [stat["name"] for stat in needs_config.statuses]:
+    if needs_config.statuses and status not in [
+        stat["name"] for stat in needs_config.statuses
+    ]:
         raise NeedsStatusNotAllowed(
-            f"Status {status} of need id {need_id} is not allowed " "by config value 'needs_statuses'."
+            f"Status {status} of need id {need_id} is not allowed "
+            "by config value 'needs_statuses'."
         )
 
     if tags is None:
         tags = []
     if len(tags) > 0:
         # tags should be a string, but it can also be already a list, which can be used.
         if isinstance(tags, str):
             tags = [tag.strip() for tag in re.split("[;,]", tags)]
         new_tags = []  # Shall contain only valid tags
         for i in range(len(tags)):
             if len(tags[i]) == 0 or tags[i].isspace():
                 logger.warning(
-                    f"Scruffy tag definition found in need {need_id}. " "Defined tag contains spaces only. [needs]",
+                    f"Scruffy tag definition found in need {need_id!r}. "
+                    "Defined tag contains spaces only. [needs.add]",
                     type="needs",
+                    subtype="add",
+                    location=(docname, lineno) if docname else None,
                 )
             else:
                 new_tags.append(tags[i])
 
         tags = new_tags
         # Check if tag is in needs_tags. If not raise an error.
         if needs_config.tags:
             for tag in tags:
                 needs_tags = [tag["name"] for tag in needs_config.tags]
                 if tag not in needs_tags:
                     raise NeedsTagNotAllowed(
-                        f"Tag {tag} of need id {need_id} is not allowed " "by config value 'needs_tags'."
+                        f"Tag {tag} of need id {need_id} is not allowed "
+                        "by config value 'needs_tags'."
                     )
         # This may have cut also dynamic function strings, as they can contain , as well.
         # So let put them together again
         # ToDo: There may be a smart regex for the splitting. This would avoid this mess of code...
+    else:
+        tags = []
     tags = _fix_list_dyn_func(tags)
 
     if constraints is None:
         constraints = []
     if len(constraints) > 0:
         # tags should be a string, but it can also be already a list,which can be used.
         if isinstance(constraints, str):
-            constraints = [constraint.strip() for constraint in re.split("[;,]", constraints)]
+            constraints = [
+                constraint.strip() for constraint in re.split("[;,]", constraints)
+            ]
 
         new_constraints = []  # Shall contain only valid constraints
         for i in range(len(constraints)):
             if len(constraints[i]) == 0 or constraints[i].isspace():
                 logger.warning(
-                    f"Scruffy tag definition found in need {need_id}. "
-                    "Defined constraint contains spaces only. [needs]",
+                    f"Scruffy constraint definition found in need {need_id!r}. "
+                    "Defined constraint contains spaces only. [needs.add]",
                     type="needs",
+                    subtype="add",
+                    location=(docname, lineno) if docname else None,
                 )
             else:
                 new_constraints.append(constraints[i])
 
         constraints = new_constraints
         # Check if constraint is in needs_constraints. If not raise an error.
         if needs_config.constraints:
@@ -256,14 +300,16 @@
                     raise NeedsConstraintNotAllowed(
                         f"Constraint {constraint} of need id {need_id} is not allowed "
                         "by config value 'needs_constraints'."
                     )
         # This may have cut also dynamic function strings, as they can contain , as well.
         # So let put them together again
         # ToDo: There may be a smart regex for the splitting. This would avoid this mess of code...
+    else:
+        constraints = []
     constraints = _fix_list_dyn_func(constraints)
 
     #############################################################################################
     # Add need to global need list
     #############################################################################################
 
     if need_id in SphinxNeedsData(env).get_or_create_needs():
@@ -288,223 +334,268 @@
         trimmed_title = title
     elif max_length <= 3:
         trimmed_title = title[:max_length]
     else:
         trimmed_title = title[: max_length - 3] + "..."
 
     # Calculate doc type, e.g. .rst or .md
-    if state and state.document and state.document.current_source:
-        doctype = os.path.splitext(state.document.current_source)[1]
-    else:
-        doctype = ".rst"
+    doctype = os.path.splitext(env.doc2path(docname))[1] if docname else ""
 
     # Add the need and all needed information
     needs_info: NeedsInfoType = {
         "docname": docname,
-        "doctype": doctype,
         "lineno": lineno,
+        "lineno_content": lineno_content,
+        "doctype": doctype,
         "target_id": need_id,
-        "external_url": external_url if is_external else None,
-        "content_node": None,  # gets set after rst parsing
-        "content_id": None,  # gets set after rst parsing
+        "content": "\n".join(content) if isinstance(content, StringList) else content,
+        "content_node": None,
+        "content_id": None,
         "type": need_type,
         "type_name": type_name,
         "type_prefix": type_prefix,
         "type_color": type_color,
         "type_style": type_style,
         "status": status,
         "tags": tags,
         "constraints": constraints,
         "constraints_passed": None,
         "constraints_results": {},
         "id": need_id,
         "title": trimmed_title,
         "full_title": title,
-        "content": content,
         "collapse": collapse,
         "arch": {},  # extracted later
         "style": style,
         "layout": layout,
         "template": template,
         "pre_template": pre_template,
         "post_template": post_template,
         "hide": hide,
         "delete": delete,
         "jinja_content": jinja_content,
         "parts": {},
         "is_part": False,
         "is_need": True,
+        "id_parent": need_id,
+        "id_complete": need_id,
         "is_external": is_external or False,
+        "external_url": external_url if is_external else None,
         "external_css": external_css or "external_link",
-        "is_modified": False,  # needed by needextend
-        "modifications": 0,  # needed by needextend
-        # these are set later in the analyse_need_locations transform
+        "is_modified": False,
+        "modifications": 0,
+        "has_dead_links": False,
+        "has_forbidden_dead_links": False,
         "sections": [],
         "section_name": "",
         "signature": "",
-        "parent_needs": [],
         "parent_need": "",
     }
     needs_extra_option_names = list(NEEDS_CONFIG.extra_options)
     _merge_extra_options(needs_info, kwargs, needs_extra_option_names)
 
     needs_global_options = needs_config.global_options
     _merge_global_options(app, needs_info, needs_global_options)
 
     link_names = [x["option"] for x in needs_config.extra_links]
     for keyword in kwargs:
         if keyword not in needs_extra_option_names and keyword not in link_names:
             raise NeedsInvalidOption(
-                "Unknown Option {}. "
+                f"Unknown Option {keyword}. "
                 "Use needs_extra_options or needs_extra_links in conf.py"
-                "to define this option.".format(keyword)
+                "to define this option."
             )
 
     # Merge links
     copy_links = []
 
     for link_type in needs_config.extra_links:
         # Check, if specific link-type got some arguments during method call
-        if link_type["option"] not in kwargs and link_type["option"] not in needs_global_options:
+        if (
+            link_type["option"] not in kwargs
+            and link_type["option"] not in needs_global_options
+        ):
             # if not we set no links, but entry in needS_info must be there
             links = []
         elif link_type["option"] in needs_global_options and (
-            link_type["option"] not in kwargs or len(str(kwargs[link_type["option"]])) == 0
+            link_type["option"] not in kwargs
+            or len(str(kwargs[link_type["option"]])) == 0
         ):
             # If it is in global option, value got already set during prior handling of them
-            links_string = needs_info[link_type["option"]]
-            links = _read_in_links(links_string)
+            links = _read_in_links(needs_info[link_type["option"]])
         else:
             # if it is set in kwargs, take this value and maybe override set value from global_options
-            links_string = kwargs[link_type["option"]]
-            links = _read_in_links(links_string)
+            links = _read_in_links(kwargs[link_type["option"]])
 
         needs_info[link_type["option"]] = links
         needs_info["{}_back".format(link_type["option"])] = []
 
         if "copy" not in link_type:
             link_type["copy"] = False
 
         if link_type["copy"] and link_type["option"] != "links":
             copy_links += links  # Save extra links for main-links
 
     needs_info["links"] += copy_links  # Set copied links to main-links
 
-    # Jinja support for need content
     if jinja_content:
         need_content_context = {**needs_info}
         need_content_context.update(**needs_config.filter_data)
         need_content_context.update(**needs_config.render_context)
-        new_content = jinja_parse(need_content_context, needs_info["content"])
-        # Overwrite current content
-        content = new_content
-        needs_info["content"] = new_content
-
-    SphinxNeedsData(env).get_or_create_needs()[need_id] = needs_info
-
-    # Template builds
-    ##############################
+        needs_info["content"] = content = jinja_parse(
+            need_content_context, needs_info["content"]
+        )
 
-    # template
     if needs_info["template"]:
-        new_content = _prepare_template(app, needs_info, "template")
-        # Overwrite current content
-        content = new_content
-        needs_info["content"] = new_content
+        needs_info["content"] = content = _prepare_template(app, needs_info, "template")
 
-    # pre_template
     if needs_info["pre_template"]:
-        pre_content = _prepare_template(app, needs_info, "pre_template")
-        needs_info["pre_content"] = pre_content
-    else:
-        pre_content = None
+        needs_info["pre_content"] = _prepare_template(app, needs_info, "pre_template")
 
-    # post_template
     if needs_info["post_template"]:
-        post_content = _prepare_template(app, needs_info, "post_template")
-        needs_info["post_content"] = post_content
-    else:
-        post_content = None
+        needs_info["post_content"] = _prepare_template(app, needs_info, "post_template")
+
+    SphinxNeedsData(env).get_or_create_needs()[need_id] = needs_info
 
     if needs_info["is_external"]:
         return []
 
-    # Adding of basic Need node.
-    ############################
-    # Title and meta data information gets added alter during event handling via process_need_nodes()
-    # We just add a basic need node and render the rst-based content, because this can not be done later.
-    style_classes = ["need", f"need-{need_type.lower()}"]
-    if style:
-        style_classes.append(style)
-
-    node_need = Need("", classes=style_classes, ids=[need_id], refid=need_id)
-
-    # Add lineno to node
-    node_need.line = needs_info["lineno"]
-
-    if needs_info["hide"]:
-        # still add node to doctree,
-        # so we can later compute its relative location in the document
+    assert state is not None, "parser state must be set if need is not external"
+
+    return _create_need_node(needs_info, env, state, content)
+
+
+@contextmanager
+def _reset_rst_titles(state: RSTState) -> Iterator[None]:
+    """Temporarily reset the title styles and section level in the parser state,
+    so that title styles can have different levels to the surrounding document.
+    """
+    # this is basically a horrible hack to get the docutils parser to work correctly with generated content
+    surrounding_title_styles = state.memo.title_styles
+    surrounding_section_level = state.memo.section_level
+    state.memo.title_styles = []
+    state.memo.section_level = 0
+    yield
+    state.memo.title_styles = surrounding_title_styles
+    state.memo.section_level = surrounding_section_level
+
+
+def _create_need_node(
+    data: NeedsInfoType,
+    env: BuildEnvironment,
+    state: RSTState,
+    content: str | StringList,
+) -> list[nodes.Node]:
+    """Create a Need node (and surrounding nodes) to be added to the document.
+
+    Note, some additional data is added to the node once the whole document has been processed
+    (see ``process_need_nodes()``).
+
+    :param data: The full data entry for this node.
+    :param env: The Sphinx environment.
+    :param state: The current parser state.
+    :param content: The main content to be rendered inside the need.
+        Note, this content my be different to ``data["content"]``,
+        in that it may be a ``StringList`` type with source-mapping directly parsed from a directive.
+    """
+    source = env.doc2path(data["docname"]) if data["docname"] else None
+
+    style_classes = ["need", f"need-{data['type'].lower()}"]
+    if data["style"]:
+        style_classes.append(data["style"])
+
+    node_need = Need("", classes=style_classes, ids=[data["id"]], refid=data["id"])
+    node_need.source, node_need.line = source, data["lineno"]
+
+    if data["hide"]:
+        # still add node to doctree, so we can later compute its relative location in the document
         # (see analyse_need_locations function)
         node_need["hidden"] = True
         return [node_need]
 
-    node_need_content = _render_template(content, docname, lineno, state)
+    return_nodes: list[nodes.Node] = []
+
+    if pre_content := data.get("pre_content"):
+        node = nodes.Element()
+        with _reset_rst_titles(state):
+            state.nested_parse(
+                StringList(pre_content.splitlines(), source=source),
+                (data["lineno"] - 1) if data["lineno"] else 0,
+                node,
+                match_titles=True,
+            )
+        return_nodes.extend(node.children)
+
+    # Calculate target id, to be able to set a link back
+    return_nodes.append(
+        nodes.target("", "", ids=[data["id"]], refid=data["id"], anonymous="")
+    )
+
+    content_offset = 0
+    if data["lineno_content"]:
+        content_offset = data["lineno_content"] - 1
+    elif data["lineno"]:
+        content_offset = data["lineno"] - 1
+    if isinstance(content, StringList):
+        state.nested_parse(content, content_offset, node_need, match_titles=False)
+    else:
+        state.nested_parse(
+            StringList(content.splitlines(), source=source),
+            content_offset,
+            node_need,
+            match_titles=False,
+        )
 
     # Extract plantuml diagrams and store needumls with keys in arch, e.g. need_info['arch']['diagram']
     node_need_needumls_without_key = []
     node_need_needumls_key_names = []
-    for child in node_need_content.children:
+    for child in node_need.children:
         if isinstance(child, Needuml):
             needuml_id = child.rawsource
-            try:
-                needuml = SphinxNeedsData(env).get_or_create_umls().get(needuml_id)
-                key_name = needuml["key"]
-                if key_name:
-                    # check if key_name already exists in needs_info["arch"]
-                    if key_name in node_need_needumls_key_names:
-                        raise NeedumlException(
-                            f"Inside need: {need_id}, found duplicate Needuml option key name: {key_name}"
-                        )
+            if needuml := SphinxNeedsData(env).get_or_create_umls().get(needuml_id):
+                try:
+                    key_name = needuml["key"]
+                    if key_name:
+                        # check if key_name already exists in needs_info["arch"]
+                        if key_name in node_need_needumls_key_names:
+                            raise NeedumlException(
+                                f"Inside need: {data['id']}, found duplicate Needuml option key name: {key_name}"
+                            )
+                        else:
+                            data["arch"][key_name] = needuml["content"]
+                            node_need_needumls_key_names.append(key_name)
                     else:
-                        needs_info["arch"][key_name] = needuml["content"]
-                        node_need_needumls_key_names.append(key_name)
-                else:
-                    node_need_needumls_without_key.append(needuml)
-            except KeyError:
-                pass
+                        node_need_needumls_without_key.append(needuml)
+                except KeyError:
+                    pass
 
     # only store the first needuml-node which has no key option under diagram
     if node_need_needumls_without_key:
-        needs_info["arch"]["diagram"] = node_need_needumls_without_key[0]["content"]
+        data["arch"]["diagram"] = node_need_needumls_without_key[0]["content"]
 
-    need_parts = find_parts(node_need_content)
-    update_need_with_parts(env, needs_info, need_parts)
+    need_parts = find_parts(node_need)
+    update_need_with_parts(env, data, need_parts)
 
-    node_need += node_need_content.children
-
-    needs_info["content_id"] = node_need["ids"][0]
+    data["content_id"] = node_need["ids"][0]
 
     # Create a copy of the content
-    needs_info["content_node"] = node_need.deepcopy()
+    data["content_node"] = node_need.deepcopy()
+
+    return_nodes.append(node_need)
 
-    return_nodes = [node_need]
-    if not is_external:
-        # Calculate target id, to be able to set a link back
-        target_node = nodes.target("", "", ids=[need_id], refid=need_id, anonymous="")
-        # TODO add to document?
-        return_nodes = [target_node, node_need]
-
-    if pre_content:
-        node_need_pre_content = _render_template(pre_content, docname, lineno, state)
-        return_nodes = node_need_pre_content.children + return_nodes
-
-    if post_content:
-        node_need_post_content = _render_template(post_content, docname, lineno, state)
-        return_nodes = return_nodes + node_need_post_content.children
+    if post_content := data.get("post_content"):
+        node = nodes.Element()
+        with _reset_rst_titles(state):
+            state.nested_parse(
+                StringList(post_content.splitlines(), source=source),
+                (data["lineno"] - 1) if data["lineno"] else 0,
+                node,
+                match_titles=True,
+            )
+        return_nodes.extend(node.children)
 
     return return_nodes
 
 
 def del_need(app: Sphinx, need_id: str) -> None:
     """
     Deletes an existing need.
@@ -518,26 +609,26 @@
         del needs[need_id]
     else:
         logger.warning(f"Given need id {need_id} not exists! [needs]", type="needs")
 
 
 def add_external_need(
     app: Sphinx,
-    need_type,
-    title: Optional[str] = None,
-    id: Optional[str] = None,
-    external_url: Optional[str] = None,
+    need_type: str,
+    title: str | None = None,
+    id: str | None = None,
+    external_url: str | None = None,
     external_css: str = "external_link",
     content: str = "",
-    status: Optional[str] = None,
-    tags: Optional[str] = None,
-    constraints: Optional[str] = None,
-    links_string: Optional[str] = None,
+    status: str | None = None,
+    tags: str | None = None,
+    constraints: str | None = None,
+    links_string: str | None = None,
     **kwargs: Any,
-):
+) -> list[nodes.Node]:
     """
     Adds an external need from an external source.
     This need does not have any representation in the current documentation project.
     However, it can be linked and filtered.
     It's reference will open a link to another, external  sphinx documentation project.
 
     It returns an empty list (without any nodes), so no nodes will be added to the document.
@@ -549,108 +640,104 @@
     :param external_url: URL as string, which shall be used as link to the original need source
     :param content: Content as single string.
     :param status: Status as string.
     :param tags: Tags as single string.
     :param constraints: constraints as single, comma separated string.
     :param links_string: Links as single string.
     :param external_css: CSS class name as string, which is set for the <a> tag.
-    :param kwargs:
 
-    :return: Empty list
     """
+    for fixed_key in ("state", "docname", "lineno", "is_external"):
+        if fixed_key in kwargs:
+            kwargs.pop(fixed_key)
+            # TODO Although it seems prudent to not silently ignore user input here,
+            # raising an error here currently breaks some existing tests
+            # raise ValueError(
+            #     f"{fixed_key} is not allowed in kwargs for add_external_need"
+            # )
+
+    return add_need(
+        app=app,
+        state=None,
+        docname=None,
+        lineno=None,
+        need_type=need_type,
+        id=id,
+        content=content,
+        # TODO a title being None is not "type compatible" with other parts of the code base,
+        # however, at present changing it to an empty string breaks some existing tests.
+        title=title,  # type: ignore
+        status=status,
+        tags=tags,
+        constraints=constraints,
+        links_string=links_string,
+        is_external=True,
+        external_url=external_url,
+        external_css=external_css,
+        **kwargs,
+    )
 
-    kwargs["state"] = None
-    kwargs["docname"] = None
-    kwargs["lineno"] = None
-    kwargs["need_type"] = need_type
-    kwargs["id"] = id
-    kwargs["content"] = content
-    kwargs["title"] = title
-    kwargs["status"] = status
-    kwargs["tags"] = tags
-    kwargs["constraints"] = constraints
-    kwargs["links_string"] = links_string
-    kwargs["is_external"] = True
-    kwargs["external_url"] = external_url
-    kwargs["external_css"] = external_css
-
-    return add_need(app=app, **kwargs)
 
-
-def _prepare_template(app: Sphinx, needs_info, template_key: str) -> str:
+def _prepare_template(app: Sphinx, needs_info: NeedsInfoType, template_key: str) -> str:
     needs_config = NeedsSphinxConfig(app.config)
     template_folder = needs_config.template_folder
     if not os.path.isabs(template_folder):
         template_folder = os.path.join(app.srcdir, template_folder)
 
     if not os.path.isdir(template_folder):
-        raise NeedsTemplateException(f"Template folder does not exist: {template_folder}")
+        raise NeedsTemplateException(
+            f"Template folder does not exist: {template_folder}"
+        )
 
     template_file_name = needs_info[template_key] + ".need"
     template_path = os.path.join(template_folder, template_file_name)
     if not os.path.isfile(template_path):
         raise NeedsTemplateException(f"Template does not exist: {template_path}")
 
     with open(template_path) as template_file:
         template_content = "".join(template_file.readlines())
     template_obj = Template(template_content)
     new_content = template_obj.render(**needs_info, **needs_config.render_context)
 
     return new_content
 
 
-def _render_template(content: str, docname: str, lineno: int, state: RSTState) -> nodes.Element:
-    rst = StringList()
-    for line in content.split("\n"):
-        rst.append(line, docname, lineno)
-    node_need_content = nodes.Element()
-    node_need_content.document = state.document
-    nested_parse_with_titles(state, rst, node_need_content)
-    return node_need_content
-
-
-def _render_plantuml_template(content: str, docname: str, lineno: int, state: RSTState) -> nodes.Element:
-    rst = StringList()
-    rst.append(".. needuml::", docname, lineno)
-    rst.append("", docname, lineno)  # Empty option line for needuml
-    for line in content.split("\n"):
-        line = f"   {line}"  # indent content under needuml
-        rst.append(line, docname, lineno)
-    node_need_content = nodes.Element()
-    node_need_content.document = state.document
-    nested_parse_with_titles(state, rst, node_need_content)
-    return node_need_content
-
-
-def _read_in_links(links_string: Union[str, List[str]]) -> List[str]:
+def _read_in_links(links_string: None | str | list[str]) -> list[str]:
     # Get links
     links = []
     if links_string:
         # Check if links_string is really a string, otherwise it will be a list, which can be used
         # without modifications
         if isinstance(links_string, str):
             link_list = re.split(";|,", links_string)
         else:
             link_list = links_string
         for link in link_list:
             if link.isspace():
                 logger.warning(
-                    f"Grubby link definition found in need {id}. " "Defined link contains spaces only. [needs]",
+                    f"Grubby link definition found in need {id}. "
+                    "Defined link contains spaces only. [needs]",
                     type="needs",
                 )
             else:
                 links.append(link.strip())
 
         # This may have cut also dynamic function strings, as they can contain , as well.
         # So let put them together again
         # ToDo: There may be a smart regex for the splitting. This would avoid this mess of code...
     return _fix_list_dyn_func(links)
 
 
-def make_hashed_id(app: Sphinx, need_type: str, full_title: str, content: str, id_length: Optional[int] = None) -> str:
+def make_hashed_id(
+    app: Sphinx,
+    need_type: str,
+    full_title: str,
+    content: str,
+    id_length: int | None = None,
+) -> str:
     """
     Creates an ID based on title or need.
 
     Also cares about the correct prefix, which is specified for each need type.
 
     :param app: Sphinx application object
     :param need_type: name of the need directive, e.g. req
@@ -665,29 +752,31 @@
         id_length = needs_config.id_length
     type_prefix = None
     for ntype in types:
         if ntype["directive"] == need_type:
             type_prefix = ntype["prefix"]
             break
     if type_prefix is None:
-        raise NeedsInvalidException(f"Given need_type {need_type} is unknown. File {app.env.docname}")
+        raise NeedsInvalidException(
+            f"Given need_type {need_type} is unknown. File {app.env.docname}"
+        )
 
     hashable_content = full_title or "\n".join(content)
     hashed_id = hashlib.sha1(hashable_content.encode("UTF-8")).hexdigest().upper()
 
     # check if needs_id_from_title is configured
     cal_hashed_id = hashed_id
     if needs_config.id_from_title:
         id_from_title = full_title.upper().replace(" ", "_") + "_"
         cal_hashed_id = id_from_title + hashed_id
 
     return f"{type_prefix}{cal_hashed_id[:id_length]}"
 
 
-def _fix_list_dyn_func(list: List[str]) -> List[str]:
+def _fix_list_dyn_func(list: list[str]) -> list[str]:
     """
     This searches a list for dynamic function fragments, which may have been cut by generic searches for ",|;".
 
     Example:
     `link_a, [[copy('links', need_id)]]` this will be splitted in list of 3 parts:
 
     #. link_a
@@ -723,54 +812,66 @@
             new_link.append(element)
         # Looks like it isn't a cut dyn_func, just add.
         else:
             new_list.append(element)
     return new_list
 
 
-def _merge_extra_options(needs_info, needs_kwargs, needs_extra_options):
+def _merge_extra_options(
+    needs_info: NeedsInfoType,
+    needs_kwargs: dict[str, Any],
+    needs_extra_options: list[str],
+) -> set[str]:
     """Add any extra options introduced via options_ext to needs_info"""
     extra_keys = set(needs_kwargs.keys()).difference(set(needs_info.keys()))
 
     for key in needs_extra_options:
         if key in extra_keys:
             needs_info[key] = str(needs_kwargs[key])
         elif key not in needs_info.keys():
             # Finally add all not used extra options with empty value to need_info.
             # Needed for filters, which need to access these empty/not used options.
             needs_info[key] = ""
 
     return extra_keys
 
 
-def _merge_global_options(app: Sphinx, needs_info, global_options) -> None:
+def _merge_global_options(
+    app: Sphinx, needs_info: NeedsInfoType, global_options: GlobalOptionsType
+) -> None:
     """Add all global defined options to needs_info"""
     if global_options is None:
         return
     config = NeedsSphinxConfig(app.config)
     for key, value in global_options.items():
         # If key already exists in needs_info, this global_option got overwritten manually in current need
-        if key in needs_info and needs_info[key]:
+        if needs_info.get(key):
             continue
 
         if isinstance(value, tuple):
             values = [value]
         elif isinstance(value, list):
             values = value
         else:
             needs_info[key] = value
             continue
 
         for single_value in values:
+            # TODO should first match break loop?
             if len(single_value) < 2 or len(single_value) > 3:
-                raise NeedsInvalidException(f"global option tuple has wrong amount of parameters: {key}")
+                # TODO this should be validated earlier at the "config" level
+                raise NeedsInvalidException(
+                    f"global option tuple has wrong amount of parameters: {key}"
+                )
             if filter_single_need(needs_info, config, single_value[1]):
                 # Set value, if filter has matched
                 needs_info[key] = single_value[0]
-            elif len(single_value) == 3 and (key not in needs_info.keys() or len(str(needs_info[key])) > 0):
+            elif len(single_value) == 3 and (
+                key not in needs_info.keys() or len(str(needs_info[key])) > 0
+            ):
                 # Otherwise set default, but only if no value was set before or value is "" and a default is defined
                 needs_info[key] = single_value[2]
             else:
                 # If not value was set until now, we have to set an empty value, so that we are sure that each need
                 # has at least the key.
                 if key not in needs_info.keys():
                     needs_info[key] = ""
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/builder.py` & `sphinx_needs-2.1.0/sphinx_needs/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import os
-from typing import Iterable, List, Optional, Sequence, Set
+from typing import Iterable, Sequence
 
 from docutils import nodes
 from sphinx import version_info
 from sphinx.application import Sphinx
 from sphinx.builders import Builder
 
 from sphinx_needs.config import NeedsSphinxConfig
@@ -44,15 +46,17 @@
         build_docnames: Iterable[str],
         updated_docnames: Sequence[str],
         method: str = "update",
     ) -> None:
         if not SphinxNeedsData(self.env).has_export_filters:
             return
         LOGGER.warning(
-            "At least one use of `export_id` directive option, requires a slower build", type="needs", subtype="build"
+            "At least one use of `export_id` directive option, requires a slower build",
+            type="needs",
+            subtype="build",
         )
         return super().write(build_docnames, updated_docnames, method)
 
     def finish(self) -> None:
         post_process_needs_data(self.app)
 
         data = SphinxNeedsData(self.env)
@@ -64,26 +68,31 @@
         if needs_config.file:
             needs_file = needs_config.file
             needs_list.load_json(needs_file)
         else:
             # check if needs.json file exists in conf.py directory
             needs_json = os.path.join(self.srcdir, "needs.json")
             if os.path.exists(needs_json):
-                LOGGER.info("needs.json found, but will not be used because needs_file not configured.")
+                LOGGER.info(
+                    "needs.json found, but will not be used because needs_file not configured."
+                )
 
         # Clean needs_list from already stored needs of the current version.
         # This is needed as needs could have been removed from documentation and if this is the case,
         # removed needs would stay in needs_list, if list gets not cleaned.
         needs_list.wipe_version(version)
         #
         from sphinx_needs.filter_common import filter_needs
 
         filter_string = needs_config.builder_filter
-        filtered_needs: List[NeedsInfoType] = filter_needs(
-            data.get_or_create_needs().values(), needs_config, filter_string
+        filtered_needs: list[NeedsInfoType] = filter_needs(
+            data.get_or_create_needs().values(),
+            needs_config,
+            filter_string,
+            append_warning="(from need_builder_filter)",
         )
 
         for need in filtered_needs:
             needs_list.add_need(version, need)
 
         for need_filter in filters.values():
             if need_filter["export_id"]:
@@ -92,19 +101,19 @@
         try:
             needs_list.write_json()
         except Exception as e:
             LOGGER.error(f"Error during writing json file: {e}")
         else:
             LOGGER.info("Needs successfully exported")
 
-    def get_target_uri(self, _docname: str, _typ: Optional[str] = None) -> str:
+    def get_target_uri(self, _docname: str, _typ: str | None = None) -> str:
         # only needed if the write phase is run
         return ""
 
-    def prepare_writing(self, _docnames: Set[str]) -> None:
+    def prepare_writing(self, _docnames: set[str]) -> None:
         # only needed if the write phase is run
         pass
 
     def write_doc(self, docname: str, doctree: nodes.document) -> None:
         # only needed if the write phase is run
         pass
 
@@ -164,21 +173,28 @@
     ) -> None:
         pass
 
     def finish(self) -> None:
         post_process_needs_data(self.app)
 
         data = SphinxNeedsData(self.env)
-        needs = data.get_or_create_needs().values()  # We need a list of needs for later filter checks
+        needs = (
+            data.get_or_create_needs().values()
+        )  # We need a list of needs for later filter checks
         version = getattr(self.env.config, "version", "unset")
         needs_config = NeedsSphinxConfig(self.env.config)
         filter_string = needs_config.builder_filter
         from sphinx_needs.filter_common import filter_needs
 
-        filtered_needs = filter_needs(needs, needs_config, filter_string)
+        filtered_needs = filter_needs(
+            needs,
+            needs_config,
+            filter_string,
+            append_warning="(from need_builder_filter)",
+        )
         needs_build_json_per_id_path = needs_config.build_json_per_id_path
         needs_dir = os.path.join(self.outdir, needs_build_json_per_id_path)
         if not os.path.exists(needs_dir):
             os.makedirs(needs_dir, exist_ok=True)
         for need in filtered_needs:
             needs_list = NeedsList(self.env.config, self.outdir, self.srcdir)
             needs_list.wipe_version(version)
@@ -238,24 +254,24 @@
                 LOGGER.info(f"Storing needuml data to file {save_path}.")
                 with open(save_path, "w") as f:
                     f.write(puml_content)
 
     def get_outdated_docs(self) -> Iterable[str]:
         return []
 
-    def prepare_writing(self, _docnames: Set[str]) -> None:
+    def prepare_writing(self, _docnames: set[str]) -> None:
         pass
 
     def write_doc_serialized(self, _docname: str, _doctree: nodes.document) -> None:
         pass
 
     def cleanup(self) -> None:
         pass
 
-    def get_target_uri(self, _docname: str, _typ: Optional[str] = None) -> str:
+    def get_target_uri(self, _docname: str, _typ: str | None = None) -> str:
         return ""
 
 
 def build_needumls_pumls(app: Sphinx, _exception: Exception) -> None:
     env = app.env
     config = NeedsSphinxConfig(env.config)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/blank/blank.css` & `sphinx_needs-2.1.0/sphinx_needs/css/blank/blank.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/blank/styles.css` & `sphinx_needs-2.1.0/sphinx_needs/css/blank/styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/common.css` & `sphinx_needs-2.1.0/sphinx_needs/css/common.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/dark/dark.css` & `sphinx_needs-2.1.0/sphinx_needs/css/dark/dark.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/dark/layouts.css` & `sphinx_needs-2.1.0/sphinx_needs/css/dark/layouts.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/dark/styles.css` & `sphinx_needs-2.1.0/sphinx_needs/css/dark/styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/modern/layouts.css` & `sphinx_needs-2.1.0/sphinx_needs/css/modern/layouts.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/css/modern/styles.css` & `sphinx_needs-2.1.0/sphinx_needs/css/modern/styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/data.py` & `sphinx_needs-2.1.0/sphinx_needs/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Module to control access to sphinx-needs data,
 which is stored in the Sphinx environment.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal, TypedDict
 
 if TYPE_CHECKING:
     from docutils.nodes import Element, Text
     from sphinx.application import Sphinx
     from sphinx.environment import BuildEnvironment
+    from typing_extensions import Required
 
     from sphinx_needs.services.manager import ServiceManager
 
 
 class NeedsFilterType(TypedDict):
     filter: str
     """Filter string."""
@@ -21,200 +23,206 @@
     types: list[str]
     result: list[str]
     amount: int
     export_id: str
     """If set, the filter is exported with this ID in the needs.json file."""
 
 
-class NeedsBaseDataType(TypedDict):
-    """A base type for all data."""
-
-    docname: str
-    """Name of the document where the need is defined."""
-    lineno: int
-    """Line number where the need is defined."""
-    target_id: str
-    """ID of the data."""
-
-
 class NeedsPartType(TypedDict):
     """Data for a single need part."""
 
     id: str
     """ID of the part"""
-
-    is_part: bool
-    is_need: bool
-
     content: str
     """Content of the part."""
-    document: str
-    """docname where the part is defined."""
     links: list[str]
     """List of need IDs, which are referenced by this part."""
     links_back: list[str]
     """List of need IDs, which are referencing this part."""
 
 
-class NeedsInfoType(NeedsBaseDataType):
+class NeedsInfoType(TypedDict, total=False):
     """Data for a single need."""
 
-    id: str
+    target_id: Required[str]
+    """ID of the data."""
+    id: Required[str]
     """ID of the data (same as target_id)"""
 
+    docname: Required[str | None]
+    """Name of the document where the need is defined (None if external)"""
+    lineno: Required[int | None]
+    """Line number where the need is defined (None if external)"""
+    lineno_content: Required[int | None]
+    """Line number on which the need content starts (None if external)"""
+
     # meta information
-    full_title: str
+    full_title: Required[str]
     """Title of the need, of unlimited length."""
-    title: str
+    title: Required[str]
     """Title of the need, trimmed to a maximum length."""
-    status: None | str
-    tags: list[str]
+    status: Required[None | str]
+    tags: Required[list[str]]
 
     # rendering information
-    collapse: bool
+    collapse: Required[None | bool]
     """hide the meta-data information of the need."""
-    hide: bool
+    hide: Required[bool]
     """If true, the need is not rendered."""
-    delete: bool
+    delete: Required[bool]
     """If true, the need is deleted entirely."""
-    layout: None | str
+    layout: Required[None | str]
     """Key of the layout, which is used to render the need."""
-    style: None | str
+    style: Required[None | str]
     """Comma-separated list of CSS classes (all appended by `needs_style_`)."""
 
     # TODO why is it called arch?
-    arch: dict[str, str]
+    arch: Required[dict[str, str]]
     """Mapping of uml key to uml content."""
 
     # external reference information
-    is_external: bool
+    is_external: Required[bool]
     """If true, no node is created and need is referencing external url"""
-    external_url: None | str
+    external_url: Required[None | str]
     """URL of the need, if it is an external need."""
-    external_css: str
+    external_css: Required[str]
     """CSS class name, added to the external reference."""
 
     # type information (based on needs_types config)
-    type: str
-    type_name: str
-    type_prefix: str
-    type_color: str
+    type: Required[str]
+    type_name: Required[str]
+    type_prefix: Required[str]
+    type_color: Required[str]
     """Hexadecimal color code of the type."""
-    type_style: str
+    type_style: Required[str]
 
-    is_modified: bool
+    is_modified: Required[bool]
     """Whether the need was modified by needextend."""
-    modifications: int
+    modifications: Required[int]
     """Number of modifications by needextend."""
 
-    # parts information
-    parts: dict[str, NeedsPartType]
-    is_need: bool
-    is_part: bool
+    # used to distinguish a part from a need
+    is_need: Required[bool]
+    is_part: Required[bool]
+    # Mapping of parts, a.k.a. sub-needs, IDs to data that overrides the need's data
+    parts: Required[dict[str, NeedsPartType]]
+    # additional information required for compatibility with parts
+    id_parent: Required[str]
+    """ID of the parent need, or self ID if not a part"""
+    id_complete: Required[str]
+    """ID of the parent need, followed by the part ID, 
+    delimited by a dot: ``<id_parent>.<id>``,
+    or self ID if not a part
+    """
 
     # content creation information
-    jinja_content: bool
-    template: None | str
-    pre_template: None | str
-    post_template: None | str
-    content: str
+    jinja_content: Required[bool]
+    template: Required[None | str]
+    pre_template: Required[None | str]
+    post_template: Required[None | str]
+    content: Required[str]
     pre_content: str
     post_content: str
-    content_id: None | str
-    """ID of the content node."""
-    content_node: None | Element
-    """deep copy of the content node."""
-
-    # link information
-    links: list[str]
-    """List of need IDs, which are referenced by this need."""
-    links_back: list[str]
-    """List of need IDs, which are referencing this need."""
-    # TODO there is more dynamically added link information;
-    # for each item in needs_extra_links config
-    # (and in prepare_env 'links' and 'parent_needs' are added if not present),
-    # you end up with a key named by the "option" field,
-    # and then another key named by the "option" field + "_back"
-    # these all have value type `list[str]`
-    # back links are all set in process_need_nodes (-> create_back_links) transform
+    content_id: Required[None | str]
+    """ID of the content node (set after parsing)."""
+    content_node: Required[None | Element]
+    """deep copy of the content node (set after parsing)."""
+
+    # these default to False and are updated in check_links post-process
+    has_dead_links: Required[bool]
+    """True if any links reference need ids that are not found in the need list."""
+    has_forbidden_dead_links: Required[bool]
+    """True if any links reference need ids that are not found in the need list,
+    and the link type does not allow dead links.
+    """
 
     # constraints information
-    constraints: list[str]
+    constraints: Required[list[str]]
     """List of constraint names, which are defined for this need."""
     # set in process_need_nodes (-> process_constraints) transform
-    constraints_results: dict[str, dict[str, bool]]
+    constraints_results: Required[dict[str, dict[str, bool]]]
     """Mapping of constraint name, to check name, to result."""
-    constraints_passed: None | bool
+    constraints_passed: Required[None | bool]
     """True if all constraints passed, False if any failed, None if not yet checked."""
     constraints_error: str
     """An error message set if any constraint failed, and `error_message` field is set in config."""
 
     # additional source information
-    doctype: str
+    doctype: Required[str]
     """Type of the document where the need is defined, e.g. '.rst'"""
     # set in analyse_need_locations transform
-    sections: list[str]
-    section_name: str
+    sections: Required[list[str]]
+    section_name: Required[str]
     """Simply the first section"""
-    signature: str | Text
+    signature: Required[str | Text]
     """Derived from a docutils desc_name node"""
+    parent_need: Required[str]
+    """Simply the first parent id"""
+
+    # link information
+    # Note, there is more dynamically added link information;
+    # for each item in needs_extra_links config
+    # (and in prepare_env 'links' and 'parent_needs' are added if not present),
+    # you end up with a key named by the "option" field,
+    # and then another key named by the "option" field + "_back"
+    # these all have value type `list[str]`
+    # back links are all set in process_need_nodes (-> create_back_links) transform
+    links: list[str]
+    """List of need IDs, which are referenced by this need."""
+    links_back: list[str]
+    """List of need IDs, which are referencing this need."""
     parent_needs: list[str]
     """List of parents of the this need (by id),
     i.e. if this need is nested in another
     """
     parent_needs_back: list[str]
     """List of children of this need (by id),
     i.e. if needs are nested within this one
     """
-    parent_need: str
-    """Simply the first parent id"""
 
-    # default extra options
-    # TODO these all default to "" which I don't think is good
-    hidden: str
-    duration: str
-    completion: str
-    # constraints: str  # this is already set in create_need
-    # these are updated in process_need_nodes (-> check_links) transform
-    has_dead_links: str | bool
-    has_forbidden_dead_links: str | bool
-    # options from `BaseService.options` get added to every need,
-    # via `ServiceManager.register`, which adds them to `extra_options``
-    # GithubService
+    # Fields added dynamically by services:
+    # options from ``BaseService.options`` get added to ``NEEDS_CONFIG.extra_options``,
+    # via `ServiceManager.register`,
+    # which in turn means they are added to every need via ``add_need``
+    # ``GithubService.options``
     avatar: str
     closed_at: str
     created_at: str
     max_amount: str
     service: str
     specific: str
-    # _type: str  # type is already set in create_need
+    ## type: str  # although this is already an internal field
     updated_at: str
     user: str
-    # OpenNeedsService
+    # ``OpenNeedsService.options``
     params: str
     prefix: str
     url_postfix: str
-    # shared GithubService and OpenNeedsService
+    # shared ``GithubService.options`` and ``OpenNeedsService.options``
     max_content_lines: str
     id_prefix: str
     query: str
     url: str
 
-    # Note there are also:
-    # - dynamic default options that can be set by needs_extra_options config
-    # - dynamic global options that can be set by needs_global_options config
+    # Note there are also these dynamic keys:
+    # - items in ``needs_extra_options`` + ``needs_duration_option`` + ``needs_completion_option``,
+    #   which get added to ``NEEDS_CONFIG.extra_options``,
+    #   and in turn means they are added to every need via ``add_need`` (as strings)
+    # - keys in ``needs_global_options`` config are added to every need via ``add_need``
+
 
+class NeedsBaseDataType(TypedDict):
+    """A base type for data items collected from directives."""
 
-class NeedsPartsInfoType(NeedsInfoType):
-    """Generated by prepare_need_list"""
-
-    document: str
-    """docname where the part is defined."""
-    id_parent: str
-    id_complete: str
+    docname: str
+    """Name of the document where the need is defined."""
+    lineno: int
+    """Line number where the need is defined."""
+    target_id: str
+    """ID of the data."""
 
 
 class NeedsBarType(NeedsBaseDataType):
     """Data for a single (matplotlib) bar diagram."""
 
     error_id: str
     title: None | str
@@ -262,14 +270,15 @@
     tags: list[str]
     types: list[str]
     filter: None | str
     sort_by: None | str
     filter_code: list[str]
     filter_func: None | str
     export_id: str
+    filter_warning: str
     """If set, the filter is exported with this ID in the needs.json file."""
 
 
 class NeedsFilteredDiagramBaseType(NeedsFilteredBaseType):
     """A base type for all filtered diagram data."""
 
     show_legend: bool
@@ -342,14 +351,15 @@
     explode: None | list[float]
     style: None | str
     labels: None | list[str]
     colors: None | list[str]
     text_color: None | str
     shadow: bool
     filter_func: None | str
+    filter_warning: str
 
 
 class NeedsSequenceType(NeedsFilteredDiagramBaseType):
     """Data for a single (filtered) sequence diagram."""
 
     start: str
 
@@ -585,15 +595,17 @@
         try:
             return self.env.needs_all_needumls
         except AttributeError:
             self.env.needs_all_needumls = {}
         return self.env.needs_all_needumls
 
 
-def merge_data(_app: Sphinx, env: BuildEnvironment, _docnames: list[str], other: BuildEnvironment) -> None:
+def merge_data(
+    _app: Sphinx, env: BuildEnvironment, _docnames: list[str], other: BuildEnvironment
+) -> None:
     """
     Performs data merge of parallel executed workers.
     Used only for parallel builds.
 
     Needs to update env manually for all data Sphinx-Needs collect during read phase
     """
 
@@ -614,22 +626,25 @@
             if isinstance(other_objects, dict) and isinstance(objects, dict):
                 if not is_complex_dict:
                     objects.update(other_objects)
                 else:
                     for other_key, other_value in other_objects.items():
                         # other_value is a list from here on!
                         if other_key in objects:
-                            objects[other_key] = list(set(objects[other_key]) | set(other_value))
+                            objects[other_key] = list(
+                                set(objects[other_key]) | set(other_value)
+                            )
                         else:
                             objects[other_key] = other_value
             elif isinstance(other_objects, list) and isinstance(objects, list):
                 objects = list(set(objects) | set(other_objects))
             else:
                 raise TypeError(
-                    f'Objects to "merge" must be dict or list, ' f"not {type(other_objects)} and {type(objects)}"
+                    f'Objects to "merge" must be dict or list, '
+                    f"not {type(other_objects)} and {type(objects)}"
                 )
 
     _merge("needs_all_docs", is_complex_dict=True)
     _merge("need_all_needbar")
     _merge("need_all_needextend")
     _merge("need_all_needextracts")
     _merge("need_all_needfilters")
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/debug.py` & `sphinx_needs-2.1.0/sphinx_needs/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Contains debug features to track down
 runtime and other problems with Sphinx-Needs
 """
+
 from __future__ import annotations
 
 import inspect
 import json
 import os.path
 from datetime import datetime
 from functools import wraps
@@ -13,22 +14,26 @@
 from timeit import default_timer as timer  # Used for timing measurements
 from typing import Any, Callable, TypeVar
 
 from jinja2 import Environment, PackageLoader, select_autoescape
 from sphinx.application import Sphinx
 
 TIME_MEASUREMENTS: dict[str, Any] = {}  # Stores the timing results
-EXECUTE_TIME_MEASUREMENTS = False  # Will be used to de/activate measurements. Set during a Sphinx Event
+EXECUTE_TIME_MEASUREMENTS = (
+    False  # Will be used to de/activate measurements. Set during a Sphinx Event
+)
 
 START_TIME = 0.0
 
 T = TypeVar("T", bound=Callable[..., Any])
 
 
-def measure_time(category: str | None = None, source: str = "internal", name: str | None = None) -> Callable[[T], T]:
+def measure_time(
+    category: str | None = None, source: str = "internal", name: str | None = None
+) -> Callable[[T], T]:
     """
     Decorator for measuring the needed execution time of a specific function.
 
     It measures:
 
     * Amount of executions
     * Overall time consumed
@@ -103,26 +108,35 @@
             if runtime_dict["min"] is None or runtime < runtime_dict["min"]:
                 runtime_dict["min"] = runtime
 
             if runtime_dict["max"] is None or runtime > runtime_dict["max"]:
                 runtime_dict["max"] = runtime
                 runtime_dict["max_params"] = {  # Store parameters as a shorten string
                     "args": str([str(arg)[:80] for arg in args]),
-                    "kwargs": str({key: str(value)[:80] for key, value in kwargs.items()}),
+                    "kwargs": str(
+                        {key: str(value)[:80] for key, value in kwargs.items()}
+                    ),
                 }
-            runtime_dict["min_max_spread"] = runtime_dict["max"] / runtime_dict["min"] * 100
+            runtime_dict["min_max_spread"] = (
+                runtime_dict["max"] / runtime_dict["min"] * 100
+            )
             runtime_dict["avg"] = runtime_dict["overall"] / runtime_dict["amount"]
             return result
 
         return wrapper  # type: ignore
 
     return inner
 
 
-def measure_time_func(func: T, category: str | None = None, source: str = "internal", name: str | None = None) -> T:
+def measure_time_func(
+    func: T,
+    category: str | None = None,
+    source: str = "internal",
+    name: str | None = None,
+) -> T:
     """Wrapper for measuring the needed execution time of a specific function.
 
     Usage as function::
 
         from sphinx_needs.utils import measure_time
 
         # Old call: my_cool_function(a,b,c)
@@ -149,15 +163,17 @@
 
     with open(json_result_path, "w", encoding="utf-8") as f:
         json.dump(data, f, indent=4)
     print(f"Timing measurement results (JSON) stored under {json_result_path}")
 
 
 def store_timing_results_html(outdir: str, build_data: dict[str, Any]) -> None:
-    jinja_env = Environment(loader=PackageLoader("sphinx_needs"), autoescape=select_autoescape())
+    jinja_env = Environment(
+        loader=PackageLoader("sphinx_needs"), autoescape=select_autoescape()
+    )
     template = jinja_env.get_template("time_measurements.html")
     out_file = Path(outdir) / "debug_measurement.html"
     with open(out_file, "w", encoding="utf-8") as f:
         f.write(template.render(data=TIME_MEASUREMENTS, build_data=build_data))
     print(f"Timing measurement report (HTML) stored under {out_file}")
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/defaults.py` & `sphinx_needs-2.1.0/sphinx_needs/defaults.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import os
-from typing import Any, Dict
+from typing import Any
 
 from docutils.parsers.rst import directives
 
 DEFAULT_DIAGRAM_TEMPLATE = """
 {%- if is_need -%}
 <size:12>{{type_name}}</size>\\n**{{title|wordwrap(15, wrapstring='**\\\\n**')}}**\\n<size:10>{{id}}</size>
 {%- else -%}
@@ -195,34 +197,32 @@
     skinparam Actor {
       BackgroundColor BLACK
       BorderColor BLACK
     }
     """,
 }
 
-TITLE_REGEX = r'([\w]+) as "([\w ]+)"'
+TITLE_REGEX = r'([^\s]+) as "([^"]+)"'
 
 
-NEED_DEFAULT_OPTIONS: Dict[str, Any] = {
+NEED_DEFAULT_OPTIONS: dict[str, Any] = {
     "id": directives.unchanged_required,
     "status": directives.unchanged_required,
     "tags": directives.unchanged_required,
     "links": directives.unchanged_required,
     "collapse": directives.unchanged_required,
     "delete": directives.unchanged,
     "jinja_content": directives.unchanged,
     "hide": directives.flag,
     "title_from_content": directives.flag,
     "style": directives.unchanged_required,
     "layout": directives.unchanged_required,
     "template": directives.unchanged_required,
     "pre_template": directives.unchanged_required,
     "post_template": directives.unchanged_required,
-    "duration": directives.unchanged_required,
-    "completion": directives.unchanged_required,
     "constraints": directives.unchanged_required,
     "constraints_passed": directives.unchanged_required,
     "constraints_results": directives.unchanged_required,
 }
 
 NEEDEXTEND_NOT_ALLOWED_OPTIONS = ["id"]
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/diagrams_common.py` & `sphinx_needs-2.1.0/sphinx_needs/diagrams_common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
 Diagrams common module, which stores all class definitions and functions, which get reused in
 diagram related directive. E.g. needflow and needsequence.
 """
 
+from __future__ import annotations
+
 import html
 import os
 import textwrap
-from typing import Any, Dict, List, Optional, Tuple, TypedDict
+from typing import Any, TypedDict
 from urllib.parse import urlparse
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.config import NeedsSphinxConfig
-from sphinx_needs.data import NeedsFilteredBaseType, NeedsPartsInfoType
+from sphinx_needs.data import NeedsFilteredBaseType, NeedsInfoType
 from sphinx_needs.errors import NoUri
 from sphinx_needs.logging import get_logger
 from sphinx_needs.utils import get_scale, split_link_types
 
 logger = get_logger(__name__)
 
 
 class DiagramAttributesType(TypedDict):
     show_legend: bool
     show_filters: bool
     show_link_names: bool
-    link_types: List[str]
+    link_types: list[str]
     config: str
     config_names: str
     scale: str
     highlight: str
-    align: Optional[str]
+    align: str | None
     debug: bool
-    caption: Optional[str]
+    caption: str | None
 
 
 class DiagramBase(SphinxDirective):
     has_content = True
 
     base_option_spec = {
         "show_legend": directives.flag,
@@ -48,15 +50,15 @@
         "config": directives.unchanged_required,
         "scale": directives.unchanged_required,
         "highlight": directives.unchanged_required,
         "align": directives.unchanged_required,
         "debug": directives.flag,
     }
 
-    def create_target(self, target_name: str) -> Tuple[int, str, nodes.target]:
+    def create_target(self, target_name: str) -> tuple[int, str, nodes.target]:
         id = self.env.new_serialno(target_name)
         targetid = f"{target_name}-{self.env.docname}-{id}"
         targetnode = nodes.target("", "", ids=[targetid])
 
         return id, targetid, targetnode
 
     def collect_diagram_attributes(self) -> DiagramAttributesType:
@@ -108,53 +110,71 @@
 
 
 def add_config(config: str) -> str:
     """Adds config section"""
     uml = ""
     if config and len(config) >= 3:
         # Remove all empty lines
-        config = "\n".join([line.strip() for line in config.split("\n") if line.strip()])
+        config = "\n".join(
+            [line.strip() for line in config.split("\n") if line.strip()]
+        )
         uml += "\n' Config\n\n"
         uml += config
         uml += "\n\n"
     return uml
 
 
 def get_filter_para(node_element: NeedsFilteredBaseType) -> nodes.paragraph:
     """Return paragraph containing the used filter description"""
     para = nodes.paragraph()
     filter_text = "Used filter:"
-    filter_text += " status(%s)" % " OR ".join(node_element["status"]) if len(node_element["status"]) > 0 else ""
+    filter_text += (
+        " status({})".format(" OR ".join(node_element["status"]))
+        if len(node_element["status"]) > 0
+        else ""
+    )
     if len(node_element["status"]) > 0 and len(node_element["tags"]) > 0:
         filter_text += " AND "
-    filter_text += " tags(%s)" % " OR ".join(node_element["tags"]) if len(node_element["tags"]) > 0 else ""
-    if (len(node_element["status"]) > 0 or len(node_element["tags"]) > 0) and len(node_element["types"]) > 0:
+    filter_text += (
+        " tags({})".format(" OR ".join(node_element["tags"]))
+        if len(node_element["tags"]) > 0
+        else ""
+    )
+    if (len(node_element["status"]) > 0 or len(node_element["tags"]) > 0) and len(
+        node_element["types"]
+    ) > 0:
         filter_text += " AND "
-    filter_text += " types(%s)" % " OR ".join(node_element["types"]) if len(node_element["types"]) > 0 else ""
+    filter_text += (
+        " types({})".format(" OR ".join(node_element["types"]))
+        if len(node_element["types"]) > 0
+        else ""
+    )
 
     filter_node = nodes.emphasis(filter_text, filter_text)
     para += filter_node
     return para
 
 
 def get_debug_container(puml_node: nodes.Element) -> nodes.container:
     """Return container containing the raw plantuml code"""
     debug_container = nodes.container()
     if isinstance(puml_node, nodes.figure):
-        data = puml_node.children[0]["uml"]
+        data = puml_node.children[0]["uml"]  # type: ignore
     else:
         data = puml_node["uml"]
     data = "\n".join([html.escape(line) for line in data.split("\n")])
     debug_para = nodes.raw("", f"<pre>{data}</pre>", format="html")
     debug_container += debug_para
 
     return debug_container
 
 
-def calculate_link(app: Sphinx, need_info: NeedsPartsInfoType, _fromdocname: str) -> str:
+def calculate_link(
+    app: Sphinx, need_info: NeedsInfoType, _fromdocname: None | str
+) -> str:
     """
     Link calculation
     All links we can get from docutils functions will be relative.
     But the generated link in the svg will be relative to the svg-file location
     (e.g. server.com/docs/_images/sqwxo499cnq329439dfjne.svg)
     and not to current documentation. Therefore we need to add ../ to get out of the image folder.
 
@@ -162,35 +182,41 @@
     :param need_info:
     :param fromdocname:
     :return:
     """
     builder = app.builder
     try:
         if need_info["is_external"]:
-            assert need_info["external_url"] is not None, "external_url must be set for external needs"
+            assert (
+                need_info["external_url"] is not None
+            ), "external_url must be set for external needs"
             link = need_info["external_url"]
             # check if need_info["external_url"] is relative path
             parsed_url = urlparse(need_info["external_url"])
             if not parsed_url.scheme and not os.path.isabs(need_info["external_url"]):
                 # only need to add ../ or ..\ to get out of the image folder
                 link = ".." + os.path.sep + need_info["external_url"]
-        else:
-            link = "../" + builder.get_target_uri(need_info["docname"]) + "#" + need_info["target_id"]
+        elif _docname := need_info["docname"]:
+            link = (
+                "../" + builder.get_target_uri(_docname) + "#" + need_info["target_id"]
+            )
             if need_info["is_part"]:
                 link = f"{link}.{need_info['id']}"
 
     except NoUri:
         link = ""
 
     return link
 
 
-def create_legend(need_types: List[Dict[str, Any]]) -> str:
-    def create_row(need_type: Dict[str, Any]) -> str:
-        return "\n|<back:{color}> {color} </back>| {name} |".format(color=need_type["color"], name=need_type["title"])
+def create_legend(need_types: list[dict[str, Any]]) -> str:
+    def create_row(need_type: dict[str, Any]) -> str:
+        return "\n|<back:{color}> {color} </back>| {name} |".format(
+            color=need_type["color"], name=need_type["title"]
+        )
 
     rows = map(create_row, need_types)
     table = "|= Color |= Type |" + "".join(rows)
 
     legend = textwrap.dedent(
         """
         ' Legend definition
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/list2need.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/list2need.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import hashlib
 import re
 from contextlib import suppress
-from typing import Any, List, Sequence
+from typing import Any, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from jinja2 import Template
 from sphinx.errors import SphinxError, SphinxWarning
 from sphinx.util.docutils import SphinxDirective
 
@@ -17,16 +19,20 @@
    {%- for name, value in options.items() %}:{{name}}: {{value}}
    {% endfor %}
 
    {{content}}
 
 """
 
-LINE_REGEX = re.compile(r"(?P<indent>[^\S\n]*)\*\s*(?P<text>.*)|[\S\*]*(?P<more_text>.*)")
-ID_REGEX = re.compile(r"(\((?P<need_id>[^\"'=\n]+)?\))")  # Exclude some chars, which are used by option list
+LINE_REGEX = re.compile(
+    r"(?P<indent>[^\S\n]*)\*\s*(?P<text>.*)|[\S\*]*(?P<more_text>.*)"
+)
+ID_REGEX = re.compile(
+    r"(\((?P<need_id>[^\"'=\n]+)?\))"
+)  # Exclude some chars, which are used by option list
 OPTION_AREA_REGEX = re.compile(r"\(\((.*)\)\)")
 OPTIONS_REGEX = re.compile(r"([^=,\s]*)=[\"']([^\"]*)[\"']")
 
 
 class List2Need(nodes.General, nodes.Element):
     pass
 
@@ -77,15 +83,17 @@
         # Create a dict, which delivers the need-type for the later level
         types = {}
         types_raw_list = [x.strip() for x in types_raw.split(",")]
         conf_types = [x["directive"] for x in needs_config.types]
         for x in range(0, len(types_raw_list)):
             types[x] = types_raw_list[x]
             if types[x] not in conf_types:
-                raise SphinxError(f"Unknown type configured: {types[x]}. Allowed are {', '.join(conf_types)}")
+                raise SphinxError(
+                    f"Unknown type configured: {types[x]}. Allowed are {', '.join(conf_types)}"
+                )
 
         down_links_raw = self.options.get("links-down")
         if down_links_raw is None or down_links_raw == "":
             down_links_raw = ""
 
         # Create a dict, which delivers the need-link for the later level
         down_links_types = {}
@@ -93,44 +101,54 @@
             down_links_raw_list = []
         else:
             down_links_raw_list = [x.strip() for x in down_links_raw.split(",")]
         link_types = [x["option"] for x in needs_config.extra_links]
         for i, down_link_raw in enumerate(down_links_raw_list):
             down_links_types[i] = down_link_raw
             if down_link_raw not in link_types:
-                raise SphinxError(f"Unknown link configured: {down_link_raw}. " f"Allowed are {', '.join(link_types)}")
+                raise SphinxError(
+                    f"Unknown link configured: {down_link_raw}. "
+                    f"Allowed are {', '.join(link_types)}"
+                )
         list_needs = []
         # Storing the data in a sorted list
         for content_line in content_raw.split("\n"):
             # for groups in line.findall(content_raw):
             match = LINE_REGEX.search(content_line)
             if not match:
                 continue
             indent, text, more_text = match.groups()
 
             if text:
                 indent = len(indent)
                 if not indent % 2 == 0:
-                    raise IndentationError("Indentation for list must be always a multiply of 2.")
+                    raise IndentationError(
+                        "Indentation for list must be always a multiply of 2."
+                    )
                 level = int(indent / 2)
 
                 if level not in types:
                     raise SphinxWarning(
-                        f"No need type defined for indentation level {level}." f" Defined types {types}"
+                        f"No need type defined for indentation level {level}."
+                        f" Defined types {types}"
                     )
 
                 if down_links_types and level > len(down_links_types):
-                    raise SphinxWarning(f"Not enough links-down defined for indentation level {level}.")
+                    raise SphinxWarning(
+                        f"Not enough links-down defined for indentation level {level}."
+                    )
 
                 splitted_text = text.split(delimiter)
                 title = splitted_text[0]
 
                 content = ""
                 with suppress(IndexError):
-                    content = delimiter.join(splitted_text[1:])  # Put the content together again
+                    content = delimiter.join(
+                        splitted_text[1:]
+                    )  # Put the content together again
 
                 need_id_result = ID_REGEX.search(title)
                 if need_id_result:
                     need_id = need_id_result.group(2)
                     title = ID_REGEX.sub("", title)
                 else:
                     # Calculate the hash value, so that we can later reuse it
@@ -152,15 +170,17 @@
                     "options": {},
                 }
                 list_needs.append(need)
             else:
                 more_text = more_text.lstrip()
                 if more_text.startswith(":"):
                     more_text = f"   {more_text}"
-                list_needs[-1]["content"] = f"{list_needs[-1]['content']}\n   {more_text}"
+                list_needs[-1]["content"] = (
+                    f"{list_needs[-1]['content']}\n   {more_text}"
+                )
 
         # Finally creating the rst code
         overall_text = []
         for index, list_need in enumerate(list_needs):
             # Search for meta data in the complete title/content
             search_string = list_need["title"] + list_need["content"]
             result = OPTION_AREA_REGEX.search(search_string)
@@ -173,39 +193,48 @@
                 list_need["title"] = OPTION_AREA_REGEX.sub("", list_need["title"])
                 list_need["content"] = OPTION_AREA_REGEX.sub("", list_need["content"])
 
             template = Template(NEED_TEMPLATE, autoescape=True)
 
             data = list_need
             need_links_down = self.get_down_needs(list_needs, index)
-            if down_links_types and list_need["level"] in down_links_types and need_links_down:
+            if (
+                down_links_types
+                and list_need["level"] in down_links_types
+                and need_links_down
+            ):
                 data["links_down"] = need_links_down
                 data["links_down_type"] = down_links_types[list_need["level"]]
                 data["set_links_down"] = True
             else:
                 data["set_links_down"] = False
 
             text = template.render(**list_need)
             text_list = text.split("\n")
             if presentation == "nested":
                 indented_text_list = ["   " * list_need["level"] + x for x in text_list]
                 text_list = indented_text_list
             overall_text += text_list
 
-        self.state_machine.insert_input(overall_text, self.state_machine.document.attributes["source"])
+        self.state_machine.insert_input(
+            overall_text, self.state_machine.document.attributes["source"]
+        )
 
         return []
 
     def make_hashed_id(self, type_prefix: str, title: str, id_length: int) -> str:
         hashable_content = title
         return "{}{}".format(
-            type_prefix, hashlib.sha1(hashable_content.encode("UTF-8")).hexdigest().upper()[:id_length]
+            type_prefix,
+            hashlib.sha1(hashable_content.encode("UTF-8"))
+            .hexdigest()
+            .upper()[:id_length],
         )
 
-    def get_down_needs(self, list_needs: List[Any], index: int) -> List[str]:
+    def get_down_needs(self, list_needs: list[Any], index: int) -> list[str]:
         """
         Return all needs which are directly under the one given by the index
         """
         current_level = list_needs[index]["level"]
 
         down_links = []
         next_index = index + 1
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/need.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/need.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
+
 import hashlib
 import re
-import typing
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst.states import RSTState, RSTStateMachine
 from docutils.statemachine import StringList
 from sphinx.addnodes import desc_name, desc_signature
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
@@ -24,17 +25,17 @@
     resolve_variants_options,
 )
 from sphinx_needs.functions.functions import check_and_get_content
 from sphinx_needs.layout import build_need
 from sphinx_needs.logging import get_logger
 from sphinx_needs.need_constraints import process_constraints
 from sphinx_needs.nodes import Need
-from sphinx_needs.utils import add_doc, profile, remove_node_from_tree
+from sphinx_needs.utils import add_doc, profile, remove_node_from_tree, split_need_id
 
-logger = get_logger(__name__)
+LOGGER = get_logger(__name__)
 
 NON_BREAKING_SPACE = re.compile("\xa0+")
 
 
 class NeedDirective(SphinxDirective):
     """
     Collects mainly all needed need-information and renders its rst-based content.
@@ -50,24 +51,34 @@
     option_spec = NEED_DEFAULT_OPTIONS
 
     final_argument_whitespace = True
 
     def __init__(
         self,
         name: str,
-        arguments: List[str],
-        options: Dict[str, Any],
+        arguments: list[str],
+        options: dict[str, Any],
         content: StringList,
         lineno: int,
         content_offset: int,
         block_text: str,
         state: RSTState,
         state_machine: RSTStateMachine,
     ):
-        super().__init__(name, arguments, options, content, lineno, content_offset, block_text, state, state_machine)
+        super().__init__(
+            name,
+            arguments,
+            options,
+            content,
+            lineno,
+            content_offset,
+            block_text,
+            state,
+            state_machine,
+        )
         self.needs_config = NeedsSphinxConfig(self.env.config)
         self.log = get_logger(__name__)
         self.full_title = self._get_full_title()
 
     @measure_time("need")
     def run(self) -> Sequence[nodes.Node]:
         #############################################################################################
@@ -101,67 +112,71 @@
                 jinja_content = False
             else:
                 raise Exception("jinja_content attribute must be true or false")
 
         hide = "hide" in self.options
 
         id = self.options.get("id")
-        content = "\n".join(self.content)
         status = self.options.get("status")
         if status:
-            status = status.replace("__", "")  # Support for multiline options, which must use __ for empty lines
+            status = status.replace(
+                "__", ""
+            )  # Support for multiline options, which must use __ for empty lines
         tags = self.options.get("tags", "")
         style = self.options.get("style")
         layout = self.options.get("layout", "")
         template = self.options.get("template")
         pre_template = self.options.get("pre_template")
         post_template = self.options.get("post_template")
-        duration = self.options.get("duration")
-        completion = self.options.get("completion")
+        constraints = self.options.get("constraints", [])
 
-        need_extra_options = {"duration": duration, "completion": completion}
+        need_extra_options = {}
         for extra_link in self.needs_config.extra_links:
-            need_extra_options[extra_link["option"]] = self.options.get(extra_link["option"], "")
+            need_extra_options[extra_link["option"]] = self.options.get(
+                extra_link["option"], ""
+            )
 
         for extra_option in NEEDS_CONFIG.extra_options:
             need_extra_options[extra_option] = self.options.get(extra_option, "")
 
         need_nodes = add_need(
             env.app,
             self.state,
             self.docname,
             self.lineno,
             need_type=self.name,
             title=self.trimmed_title,
             id=id,
-            content=content,
+            content=self.content,
+            lineno_content=self.content_offset + 1,
             status=status,
             tags=tags,
             hide=hide,
             template=template,
             pre_template=pre_template,
             post_template=post_template,
             collapse=collapse,
             style=style,
             layout=layout,
             delete=delete_opt,
             jinja_content=jinja_content,
+            constraints=constraints,
             **need_extra_options,
         )
         add_doc(env, self.docname)
-        return need_nodes  # type: ignore[no-any-return]
+        return need_nodes
 
-    def read_in_links(self, name: str) -> List[str]:
+    def read_in_links(self, name: str) -> list[str]:
         # Get links
         links_string = self.options.get(name)
         links = []
         if links_string:
             for link in re.split(r";|,", links_string):
                 if link.isspace():
-                    logger.warning(
+                    LOGGER.warning(
                         f"Grubby link definition found in need '{self.trimmed_title}'. "
                         "Defined link contains spaces only. [needs]",
                         type="needs",
                         location=(self.env.docname, self.lineno),
                     )
                 else:
                     links.append(link.strip())
@@ -170,20 +185,25 @@
             # So let put them together again
             # ToDo: There may be a smart regex for the splitting. This would avoid this mess of code...
         return _fix_list_dyn_func(links)
 
     def make_hashed_id(self, type_prefix: str, id_length: int) -> str:
         hashable_content = self.full_title or "\n".join(self.content)
         return "{}{}".format(
-            type_prefix, hashlib.sha1(hashable_content.encode("UTF-8")).hexdigest().upper()[:id_length]
+            type_prefix,
+            hashlib.sha1(hashable_content.encode("UTF-8"))
+            .hexdigest()
+            .upper()[:id_length],
         )
 
     @property
     def title_from_content(self) -> bool:
-        return "title_from_content" in self.options or self.needs_config.title_from_content
+        return (
+            "title_from_content" in self.options or self.needs_config.title_from_content
+        )
 
     @property
     def docname(self) -> str:
         return self.env.docname
 
     @property
     def trimmed_title(self) -> str:
@@ -206,45 +226,45 @@
         """
         Determines the title for the need in order of precedence:
         directive argument, first sentence of requirement (if
         `:title_from_content:` was set, and '' if no title is to be derived)."""
         if len(self.arguments) > 0:  # a title was passed
             if "title_from_content" in self.options:
                 self.log.warning(
-                    'need "{}" has :title_from_content: set, '
-                    "but a title was provided. (see file {}) [needs]".format(self.arguments[0], self.docname),
+                    f'need "{self.arguments[0]}" has :title_from_content: set, '
+                    f"but a title was provided. (see file {self.docname}) [needs]",
                     type="needs",
                     location=(self.env.docname, self.lineno),
                 )
             return self.arguments[0]  # type: ignore[no-any-return]
         elif self.title_from_content:
             first_sentence = re.split(r"[.\n]", "\n".join(self.content))[0]
             if not first_sentence:
                 raise NeedsInvalidException(
                     ":title_from_content: set, but "
                     "no content provided. "
-                    "(Line {} of file {}".format(self.lineno, self.docname)
+                    f"(Line {self.lineno} of file {self.docname}"
                 )
             return first_sentence
         else:
             return ""
 
 
 def get_sections_and_signature_and_needs(
-    need_node: Optional[nodes.Node],
-) -> Tuple[List[str], Optional[nodes.Text], List[str]]:
+    need_node: nodes.Node | None,
+) -> tuple[list[str], nodes.Text | None, list[str]]:
     """Gets the hierarchy of the section nodes as a list starting at the
     section of the current need and then its parent sections"""
     sections = []
-    parent_needs: List[str] = []
+    parent_needs: list[str] = []
     signature = None
     current_node = need_node
     while current_node:
         if isinstance(current_node, nodes.section):
-            title = typing.cast(str, current_node.children[0].astext())
+            title = current_node.children[0].astext()
             # If using auto-section numbering, then Sphinx inserts
             # multiple non-breaking space unicode characters into the title
             # we'll replace those with a simple space to make them easier to
             # use in filters
             title = NON_BREAKING_SPACE.sub(" ", title)
             sections.append(title)
 
@@ -255,15 +275,17 @@
             for sibling in current_node.parent.children:
                 # We want to check only "above" current node, so no need to check sibling after current_node.
                 if sibling == current_node:
                     break
                 if isinstance(sibling, desc_signature):
                     # Check the child of the found signature for the text content/node.
                     for desc_child in sibling.children:
-                        if isinstance(desc_child, desc_name) and isinstance(desc_child.children[0], nodes.Text):
+                        if isinstance(desc_child, desc_name) and isinstance(
+                            desc_child.children[0], nodes.Text
+                        ):
                             signature = desc_child.children[0]
                 if signature:
                     break
 
         # Check if the need is nested inside another need (so part of its content)
         # and we only want to find our parent and not add the grands, too.
         if isinstance(current_node, Need) and len(parent_needs) == 0:
@@ -296,15 +318,15 @@
     (i.e. ones that should not be rendered in the output)
     are removed from the doctree.
     """
     env = app.env
 
     needs = SphinxNeedsData(env).get_or_create_needs()
 
-    hidden_needs: List[Need] = []
+    hidden_needs: list[Need] = []
     for need_node in doctree.findall(Need):
         need_id = need_node["refid"]
         need_info = needs[need_id]
 
         # first we initialize to default values
         if "sections" not in need_info:
             need_info["sections"] = []
@@ -319,15 +341,17 @@
             need_info["parent_needs"] = []
 
         if "parent_need" not in need_info:
             need_info["parent_need"] = ""
 
         # Fetch values from need
         # Start from the target node, which is a sibling of the current need node
-        sections, signature, parent_needs = get_sections_and_signature_and_needs(previous_sibling(need_node))
+        sections, signature, parent_needs = get_sections_and_signature_and_needs(
+            previous_sibling(need_node)
+        )
 
         # append / set values from need
         if sections:
             need_info["sections"] = sections
             need_info["section_name"] = sections[0]
 
         if signature:
@@ -340,24 +364,24 @@
         if need_node.get("hidden"):
             hidden_needs.append(need_node)
 
     # now we have gathered all the information we need,
     # we can remove the hidden needs from the doctree
     for need_node in hidden_needs:
         if need_node.parent is not None:
-            need_node.parent.remove(need_node)  # type: ignore[attr-defined]
+            need_node.parent.remove(need_node)
 
 
-def previous_sibling(node: nodes.Node) -> Optional[nodes.Node]:
+def previous_sibling(node: nodes.Node) -> nodes.Node | None:
     """Return preceding sibling node or ``None``."""
     try:
-        i = node.parent.index(node)  # type: ignore
+        i = node.parent.index(node)
     except AttributeError:
         return None
-    return node.parent[i - 1] if i > 0 else None  # type: ignore
+    return node.parent[i - 1] if i > 0 else None
 
 
 @profile("NEEDS_POST_PROCESS")
 @measure_time("need_post_process")
 def post_process_needs_data(app: Sphinx) -> None:
     """In-place post-processing of needs data.
 
@@ -387,15 +411,15 @@
     Event handler to add title meta data (status, tags, links, ...) information to the Need node. Also processes
     constraints.
     """
     needs_config = NeedsSphinxConfig(app.config)
     if not needs_config.include_needs:
         for node in doctree.findall(Need):
             if node.parent is not None:
-                node.parent.remove(node)  # type: ignore
+                node.parent.remove(node)
         return
 
     needs_data = SphinxNeedsData(app.env)
 
     # If no needs were defined, we do not need to do anything
     if not needs_data.get_or_create_needs():
         return
@@ -405,94 +429,121 @@
     for extend_node in doctree.findall(Needextend):
         remove_node_from_tree(extend_node)
 
     format_need_nodes(app, doctree, fromdocname, list(doctree.findall(Need)))
 
 
 @profile("NEED_FORMAT")
-def format_need_nodes(app: Sphinx, doctree: nodes.document, fromdocname: str, found_needs_nodes: List[Need]) -> None:
+def format_need_nodes(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_needs_nodes: list[Need],
+) -> None:
     """Replace need nodes in the document with node trees suitable for output"""
     env = app.env
     needs = SphinxNeedsData(env).get_or_create_needs()
 
     # We try to avoid findall as much as possibles. so we reuse the already found need nodes in the current document.
     # for node_need in doctree.findall(Need):
     for node_need in found_needs_nodes:
         need_id = node_need.attributes["ids"][0]
         need_data = needs[need_id]
 
         find_and_replace_node_content(node_need, env, need_data)
         for index, attribute in enumerate(node_need.attributes["classes"]):
-            node_need.attributes["classes"][index] = check_and_get_content(attribute, need_data, env)
+            node_need.attributes["classes"][index] = check_and_get_content(
+                attribute, need_data, env
+            )
 
         layout = need_data["layout"] or NeedsSphinxConfig(app.config).default_layout
 
         build_need(layout, node_need, app, fromdocname=fromdocname)
 
 
-def check_links(needs: Dict[str, NeedsInfoType], config: NeedsSphinxConfig) -> None:
+def check_links(needs: dict[str, NeedsInfoType], config: NeedsSphinxConfig) -> None:
     """Checks if set links are valid or are dead (referenced need does not exist.)
 
     For needs with dead links, an extra ``has_dead_links`` field is added and,
     if the link is not allowed to be dead,
     the ``has_forbidden_dead_links`` field is also added.
     """
     extra_links = config.extra_links
+    report_dead_links = config.report_dead_links
     for need in needs.values():
         for link_type in extra_links:
-            dead_links_allowed = link_type.get("allow_dead_links", False)
-            need_link_value = (
-                [need[link_type["option"]]] if isinstance(need[link_type["option"]], str) else need[link_type["option"]]  # type: ignore
-            )
-            for link in need_link_value:
-                if "." in link:
-                    need_id, need_part_id = link.split(".")
-                else:
-                    need_id = link
-                    need_part_id = None
-                if need_id not in needs or (
-                    need_id in needs and need_part_id and need_part_id not in needs[need_id]["parts"]
+            _value = need[link_type["option"]]  # type: ignore[literal-required]
+            need_link_value = [_value] if isinstance(_value, str) else _value
+            for need_id_full in need_link_value:
+                need_id_main, need_id_part = split_need_id(need_id_full)
+
+                if need_id_main not in needs or (
+                    need_id_main in needs
+                    and need_id_part
+                    and need_id_part not in needs[need_id_main]["parts"]
                 ):
                     need["has_dead_links"] = True
-                    if not dead_links_allowed:
+                    if not link_type.get("allow_dead_links", False):
                         need["has_forbidden_dead_links"] = True
-                    break  # One found dead link is enough
-
-
-def create_back_links(needs: Dict[str, NeedsInfoType], config: NeedsSphinxConfig) -> None:
+                        if report_dead_links:
+                            message = f"Need '{need['id']}' has unknown outgoing link '{need_id_full}' in field '{link_type['option']}'"
+                            # if the need has been imported from an external URL,
+                            # we want to provide that URL as the location of the warning,
+                            # otherwise we use the location of the need in the source file
+                            if need.get("is_external", False):
+                                LOGGER.warning(
+                                    f"{need['external_url']}: {message} [needs.external_link_outgoing]",
+                                    type="needs",
+                                    subtype="external_link_outgoing",
+                                )
+                            else:
+                                LOGGER.warning(
+                                    f"{message} [needs.link_outgoing]",
+                                    location=(need["docname"], need["lineno"]),
+                                    type="needs",
+                                    subtype="link_outgoing",
+                                )
+
+
+def create_back_links(
+    needs: dict[str, NeedsInfoType], config: NeedsSphinxConfig
+) -> None:
     """Create back-links in all found needs.
 
     These are fields for each link type, ``<link_name>_back``,
     which contain a list of all IDs of needs that link to the current need.
     """
     for links in config.extra_links:
         option = links["option"]
         option_back = f"{option}_back"
 
         for key, need in needs.items():
-            need_link_value = [need[option]] if isinstance(need[option], str) else need[option]  # type: ignore[literal-required]
-            for link in need_link_value:
-                link_main = link.split(".")[0]
-                try:
-                    link_part = link.split(".")[1]
-                except IndexError:
-                    link_part = None
-
-                if link_main in needs:
-                    if key not in needs[link_main][option_back]:  # type: ignore[literal-required]
-                        needs[link_main][option_back].append(key)  # type: ignore[literal-required]
+            need_link_value: list[str] = (
+                [need[option]] if isinstance(need[option], str) else need[option]  # type: ignore[literal-required]
+            )
+            for need_id_full in need_link_value:
+                need_id_main, need_id_part = split_need_id(need_id_full)
+
+                if need_id_main in needs:
+                    if key not in needs[need_id_main][option_back]:  # type: ignore[literal-required]
+                        needs[need_id_main][option_back].append(key)  # type: ignore[literal-required]
 
                     # Handling of links to need_parts inside a need
-                    if link_part and link_part in needs[link_main]["parts"]:
-                        if option_back not in needs[link_main]["parts"][link_part].keys():
-                            needs[link_main]["parts"][link_part][option_back] = []  # type: ignore[literal-required]
-                        needs[link_main]["parts"][link_part][option_back].append(key)  # type: ignore[literal-required]
+                    if need_id_part and need_id_part in needs[need_id_main]["parts"]:
+                        if (
+                            option_back
+                            not in needs[need_id_main]["parts"][need_id_part].keys()
+                        ):
+                            needs[need_id_main]["parts"][need_id_part][option_back] = []  # type: ignore[literal-required]
+                        needs[need_id_main]["parts"][need_id_part][option_back].append(  # type: ignore[literal-required]
+                            key
+                        )
 
 
-def _fix_list_dyn_func(list: List[str]) -> List[str]:
+def _fix_list_dyn_func(list: list[str]) -> list[str]:
     """
     This searches a list for dynamic function fragments, which may have been cut by generic searches for ",|;".
 
     Example:
     `link_a, [[copy('links', need_id)]]` this will be split in list of 3 parts:
 
     #. link_a
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needbar.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import hashlib
 import math
-from typing import List, Sequence
+from typing import Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
@@ -76,15 +78,19 @@
 
         text_color = self.options.get("text_color")
         if text_color:
             text_color = text_color.strip()
 
         style = self.options.get("style")
         matplotlib = import_matplotlib()
-        style = style.strip() if style else (matplotlib.style.use("default") if matplotlib else "default")
+        style = (
+            style.strip()
+            if style
+            else (matplotlib.style.use("default") if matplotlib else "default")
+        )
 
         legend = "legend" in self.options
 
         colors = self.options.get("colors")
         if colors:
             colors = [x.strip() for x in colors.split(",")]
 
@@ -147,29 +153,37 @@
             "style": style,
             "colors": colors,
             "text_color": text_color,
         }
 
         add_doc(env, env.docname)
 
-        return [targetnode, Needbar("")]
+        bar_node = Needbar("")
+        self.set_source_info(bar_node)
+
+        return [targetnode, bar_node]
 
 
 # Algorithm:
 # 1. define constants
 # 2. pre process data
 # 3. process the labels (maybe from content)
 # 4. transpose the data if needed
 # 5. process content
 # 6. calculate index according to configuration and content size
 # 7. styling and coloring
 # 8. create figure
 # 9. final storage
 # 10. cleanup matplotlib
-def process_needbar(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needbar(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     env = app.env
     needs_data = SphinxNeedsData(env)
     needs_config = NeedsSphinxConfig(env.config)
 
     matplotlib = import_matplotlib()
 
     if matplotlib is None and found_nodes and needs_config.include_needs:
@@ -215,21 +229,27 @@
             local_data.append(row_data)
 
             if x == 0:
                 test_columns_length = len(row_data)
             else:
                 # We can only process content with the same lenght for each line
                 if test_columns_length != len(row_data):
-                    raise Exception(f"{error_id}: each content line must have the same length")
+                    raise Exception(
+                        f"{error_id}: each content line must have the same length"
+                    )
 
         # 3. process the labels (maybe from content)
         xlabels = current_needbar["xlabels"]
-        xlabels_in_content = bool(xlabels and len(xlabels) >= 1 and xlabels[0] == "FROM_DATA")
+        xlabels_in_content = bool(
+            xlabels and len(xlabels) >= 1 and xlabels[0] == "FROM_DATA"
+        )
         ylabels = current_needbar["ylabels"]
-        ylabels_in_content = bool(ylabels and len(ylabels) >= 1 and ylabels[0] == "FROM_DATA")
+        ylabels_in_content = bool(
+            ylabels and len(ylabels) >= 1 and ylabels[0] == "FROM_DATA"
+        )
 
         if xlabels_in_content:
             # get xlabels from content => first row in content
             xlabels = local_data[0]
             local_data = local_data[1:]  # remove the first row from further processing
             if ylabels_in_content:  # we have a ylabels in the content:
                 xlabels = xlabels[1:]  # first element (0) in the row has to be ignored
@@ -259,31 +279,38 @@
         if not len(ylabels) == len(local_data):
             raise Exception(
                 f"{error_id} length of ylabels: {len(ylabels)} is not equal with sum of rows: {len(local_data)}"
             )
 
         # 4. transpose the data if needed
         if current_needbar["transpose"]:
-            local_data = [[local_data[j][i] for j in range(len(local_data))] for i in range(len(local_data[0]))]
+            local_data = [
+                [local_data[j][i] for j in range(len(local_data))]
+                for i in range(len(local_data[0]))
+            ]
             tmp = ylabels
             ylabels = xlabels
             xlabels = tmp
 
         # 5. process content
         local_data_number = []
-        need_list = list(prepare_need_list(needs_data.get_or_create_needs().values()))  # adds parts to need_list
+        need_list = list(
+            prepare_need_list(needs_data.get_or_create_needs().values())
+        )  # adds parts to need_list
 
         for line in local_data:
             line_number = []
             for element in line:
                 element = element.strip()
                 if element.isdigit():
                     line_number.append(float(element))
                 else:
-                    result = len(filter_needs(need_list, needs_config, element))
+                    result = len(
+                        filter_needs(need_list, needs_config, element, location=node)
+                    )
                     line_number.append(float(result))
             local_data_number.append(line_number)
 
         # 6. calculate index according to configuration and content size
         index = []
         for row in range(len(local_data_number)):
             _line = []
@@ -329,15 +356,17 @@
             # Set default colors, if nothing is given
             colors = matplotlib.rcParams["axes.prop_cycle"].by_key()["color"]
         else:
             # extend given colors with default colors
             colors = colors + matplotlib.rcParams["axes.prop_cycle"].by_key()["color"]
         multi = math.ceil(len(local_data) / len(colors))
         if multi > 1:
-            print(f"{error_id} warning: color schema is smaller than data, double coloring is occurring")
+            print(
+                f"{error_id} warning: color schema is smaller than data, double coloring is occurring"
+            )
         colors = colors * multi
         colors = colors[: len(local_data)]
 
         y_offset = [0.0 for _ in range(len(local_data_number[0]))]
 
         # 8. create figure
         bar_labels = []
@@ -362,39 +391,49 @@
 
             if current_needbar["stacked"]:
                 # handle stacked bar
                 y_offset = [i + j for i, j in zip(y_offset, local_data_number[x])]
 
             if current_needbar["show_sum"]:
                 try:
-                    bar_label = axes.bar_label(bar, label_type="center")  # show label in the middel of each bar
+                    bar_label = axes.bar_label(
+                        bar, label_type="center"
+                    )  # show label in the middel of each bar
                     bar_labels.append(bar_label)
-                except AttributeError:  # bar_label is not support in older matplotlib versions
+                except (
+                    AttributeError
+                ):  # bar_label is not support in older matplotlib versions
                     current_needbar["show_sum"] = None
                     current_needbar["show_top_sum"] = None
 
             if current_needbar["show_top_sum"] and (
                 not current_needbar["stacked"] or (x == len(local_data_number) - 1)
             ):
                 # "show_top_sum" and ( not stacked or end of stack )
                 try:
                     bar_label = axes.bar_label(bar)
                     bar_labels.append(bar_label)
-                except AttributeError:  # bar_label is not support in older matplotlib versions
+                except (
+                    AttributeError
+                ):  # bar_label is not support in older matplotlib versions
                     current_needbar["show_sum"] = None
                     current_needbar["show_top_sum"] = None
 
         sum_rotation = current_needbar["sum_rotation"]
-        if sum_rotation and (current_needbar["show_top_sum"] or current_needbar["show_sum"]):
+        if sum_rotation and (
+            current_needbar["show_top_sum"] or current_needbar["show_sum"]
+        ):
             sum_rotation = sum_rotation.strip()
             # Rotate the bar labels
             if sum_rotation.isdigit():
                 matplotlib.pyplot.setp(bar_labels, rotation=int(sum_rotation))
 
-        centers = [(i + j) / 2.0 for i, j in zip(index[0], index[len(local_data_number) - 1])]
+        centers = [
+            (i + j) / 2.0 for i, j in zip(index[0], index[len(local_data_number) - 1])
+        ]
         if not current_needbar["horizontal"]:
             # We want to support even older version of matplotlib, which do not support axes.set_xticks(labels)
             axes.set_xticks(centers)
             axes.set_xticklabels(labels=xlabels)
         else:
             # We want to support even older version of matplotlib, which do not support axes.set_yticks(labels)
             axes.set_yticks(centers)
@@ -402,22 +441,26 @@
             axes.invert_yaxis()  # labels read top-to-bottom
 
         xlabels_rotation = current_needbar["xlabels_rotation"]
         if xlabels_rotation:
             xlabels_rotation = xlabels_rotation.strip()
             # Rotate the tick labels
             if xlabels_rotation.isdigit():
-                matplotlib.pyplot.setp(axes.get_xticklabels(), rotation=int(xlabels_rotation))
+                matplotlib.pyplot.setp(
+                    axes.get_xticklabels(), rotation=int(xlabels_rotation)
+                )
 
         ylabels_rotation = current_needbar["ylabels_rotation"]
         if ylabels_rotation:
             ylabels_rotation = ylabels_rotation.strip()
             # Rotate the tick labels
             if ylabels_rotation.isdigit():
-                matplotlib.pyplot.setp(axes.get_yticklabels(), rotation=int(ylabels_rotation))
+                matplotlib.pyplot.setp(
+                    axes.get_yticklabels(), rotation=int(ylabels_rotation)
+                )
 
         if current_needbar["title"]:
             axes.set_title(current_needbar["title"].strip())
 
         if current_needbar["x_axis_title"]:
             axes.set_xlabel(current_needbar["x_axis_title"].strip())
 
@@ -427,15 +470,17 @@
         if current_needbar["legend"]:
             axes.legend()
 
         # 9. final storage
 
         # We need to calculate an unique bar-image file name
         hash_value = hashlib.sha256(id.encode()).hexdigest()[:5]
-        image_node = save_matplotlib_figure(app, figure, f"need_bar_{hash_value}", fromdocname)
+        image_node = save_matplotlib_figure(
+            app, figure, f"need_bar_{hash_value}", fromdocname
+        )
 
         # Add lineno to node
         image_node.line = current_needbar["lineno"]
 
         # normally the title is more understandable for a person who needs alt
         if current_needbar["title"]:
             image_node["alt"] = current_needbar["title"].strip()
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needextend.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needextend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""
+from __future__ import annotations
 
-
-"""
 import re
-from typing import Any, Callable, Dict, Sequence
+from typing import Any, Callable, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.api.exceptions import NeedsInvalidFilter
 from sphinx_needs.config import NeedsSphinxConfig
@@ -29,34 +27,36 @@
     """
 
     has_content = False
     required_arguments = 1
     optional_arguments = 0
     final_argument_whitespace = True
 
-    option_spec: Dict[str, Callable[[str], Any]] = {
+    option_spec: dict[str, Callable[[str], Any]] = {
         "strict": directives.unchanged_required,
     }
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
         id = env.new_serialno("needextend")
         targetid = f"needextend-{env.docname}-{id}"
         targetnode = nodes.target("", "", ids=[targetid])
 
         extend_filter = self.arguments[0] if self.arguments else None
         if not extend_filter:
-            raise NeedsInvalidFilter(f"Filter of needextend must be set. See {env.docname}:{self.lineno}")
-
-        strict_option = self.options.get("strict", str(NeedsSphinxConfig(self.env.app.config).needextend_strict))
-        strict = True
-        if strict_option.upper() == "TRUE":
+            raise NeedsInvalidFilter(
+                f"Filter of needextend must be set. See {env.docname}:{self.lineno}"
+            )
+
+        strict = NeedsSphinxConfig(self.env.app.config).needextend_strict
+        strict_option: str = self.options.get("strict", "").upper()
+        if strict_option == "TRUE":
             strict = True
-        elif strict_option.upper() == "FALSE":
+        elif strict_option == "FALSE":
             strict = False
 
         data = SphinxNeedsData(env).get_or_create_extends()
         data[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
             "target_id": targetid,
@@ -67,68 +67,102 @@
 
         add_doc(env, env.docname)
 
         return [targetnode, Needextend("")]
 
 
 def extend_needs_data(
-    all_needs: Dict[str, NeedsInfoType], extends: Dict[str, NeedsExtendType], needs_config: NeedsSphinxConfig
+    all_needs: dict[str, NeedsInfoType],
+    extends: dict[str, NeedsExtendType],
+    needs_config: NeedsSphinxConfig,
 ) -> None:
     """Use data gathered from needextend directives to modify fields of existing needs."""
 
     list_values = ["tags", "links"] + [x["option"] for x in needs_config.extra_links]
     link_names = [x["option"] for x in needs_config.extra_links]
 
     for current_needextend in extends.values():
         need_filter = current_needextend["filter"]
         if need_filter in all_needs:
             # a single known ID
             found_needs = [all_needs[need_filter]]
-        elif need_filter is not None and re.fullmatch(needs_config.id_regex, need_filter):
+        elif need_filter is not None and re.fullmatch(
+            needs_config.id_regex, need_filter
+        ):
             # an unknown ID
-            error = f"Provided id {need_filter} for needextend does not exist."
+            error = f"Provided id {need_filter!r} for needextend does not exist. [needs.extend]"
             if current_needextend["strict"]:
                 raise NeedsInvalidFilter(error)
             else:
-                logger.info(error)
-                continue
+                logger.warning(
+                    error,
+                    type="needs",
+                    subtype="extend",
+                    location=(
+                        current_needextend["docname"],
+                        current_needextend["lineno"],
+                    ),
+                )
+            continue
         else:
             # a filter string
             try:
-                found_needs = filter_needs(all_needs.values(), needs_config, need_filter)
+                found_needs = filter_needs(
+                    all_needs.values(),
+                    needs_config,
+                    need_filter,
+                    location=(
+                        current_needextend["docname"],
+                        current_needextend["lineno"],
+                    ),
+                )
             except NeedsInvalidFilter as e:
-                raise NeedsInvalidFilter(
-                    f"Filter not valid for needextend on page {current_needextend['docname']}:\n{e}"
+                logger.warning(
+                    f"Invalid filter {need_filter!r}: {e} [needs.extend]",
+                    type="needs",
+                    subtype="extend",
+                    location=(
+                        current_needextend["docname"],
+                        current_needextend["lineno"],
+                    ),
                 )
+                continue
 
         for found_need in found_needs:
             # Work in the stored needs, not on the search result
             need = all_needs[found_need["id"]]
             need["is_modified"] = True
             need["modifications"] += 1
 
             for option, value in current_needextend["modifications"].items():
                 if option.startswith("+"):
                     option_name = option[1:]
                     if option_name in link_names:
-                        if value.strip().startswith("[[") and value.strip().endswith("]]"):  # dynamic function
+                        if value.strip().startswith("[[") and value.strip().endswith(
+                            "]]"
+                        ):  # dynamic function
                             need[option_name].append(value)
                         else:
                             for ref_need in [i.strip() for i in re.split(";|,", value)]:
                                 if ref_need not in all_needs:
                                     logger.warning(
                                         f"Provided link id {ref_need} for needextend does not exist. [needs]",
                                         type="needs",
-                                        location=(current_needextend["docname"], current_needextend["lineno"]),
+                                        location=(
+                                            current_needextend["docname"],
+                                            current_needextend["lineno"],
+                                        ),
                                     )
                                     continue
                                 if ref_need not in need[option_name]:
                                     need[option_name].append(ref_need)
                     elif option_name in list_values:
-                        if value.strip().startswith("[[") and value.strip().endswith("]]"):  # dynamic function
+                        if value.strip().startswith("[[") and value.strip().endswith(
+                            "]]"
+                        ):  # dynamic function
                             need[option_name].append(value)
                         else:
                             for item in [i.strip() for i in re.split(";|,", value)]:
                                 if item not in need[option_name]:
                                     need[option_name].append(item)
                     else:
                         if need[option_name]:
@@ -143,26 +177,33 @@
                     if option_name in list_values:
                         need[option_name] = []
                     else:
                         need[option_name] = ""
                 else:
                     if option in link_names:
                         need[option] = []
-                        if value.strip().startswith("[[") and value.strip().endswith("]]"):  # dynamic function
+                        if value.strip().startswith("[[") and value.strip().endswith(
+                            "]]"
+                        ):  # dynamic function
                             need[option].append(value)
                         else:
                             for ref_need in [i.strip() for i in re.split(";|,", value)]:
                                 if ref_need not in all_needs:
                                     logger.warning(
                                         f"Provided link id {ref_need} for needextend does not exist. [needs]",
                                         type="needs",
-                                        location=(current_needextend["docname"], current_needextend["lineno"]),
+                                        location=(
+                                            current_needextend["docname"],
+                                            current_needextend["lineno"],
+                                        ),
                                     )
                                     continue
                                 need[option].append(ref_need)
                     elif option in list_values:
-                        if value.strip().startswith("[[") and value.strip().endswith("]]"):  # dynamic function
+                        if value.strip().startswith("[[") and value.strip().endswith(
+                            "]]"
+                        ):  # dynamic function
                             need[option].append(value)
                         else:
                             need[option] = [i.strip() for i in re.split(";|,", value)]
                     else:
                         need[option] = value
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needextract.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needextract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-"""
+from __future__ import annotations
 
-
-"""
 import re
-from typing import List, Sequence
+from typing import Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from docutils.transforms.references import Substitutions
 from sphinx.application import Sphinx
 
 from sphinx_needs.api.exceptions import NeedsInvalidFilter
@@ -41,15 +39,17 @@
     }
     # Update the options_spec with values defined in the FilterBase class
     option_spec.update(FilterBase.base_option_spec)
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
-        targetid = "needextract-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needextract"))
+        targetid = "needextract-{docname}-{id}".format(
+            docname=env.docname, id=env.new_serialno("needextract")
+        )
         targetnode = nodes.target("", "", ids=[targetid])
 
         filter_arg = self.arguments[0] if self.arguments else None
 
         # Add the need and all needed information
         data = SphinxNeedsData(env).get_or_create_extracts()
         data[targetid] = {
@@ -65,15 +65,18 @@
 
         add_doc(env, env.docname, "needextract")
 
         return [targetnode, Needextract("")]
 
 
 def process_needextract(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     """
     Replace all needextract nodes with a list of the collected needs.
     """
     env = app.env
     needs_config = NeedsSphinxConfig(app.config)
 
@@ -81,27 +84,31 @@
         if not needs_config.include_needs:
             remove_node_from_tree(node)
             continue
 
         id = node.attributes["ids"][0]
         current_needextract = SphinxNeedsData(env).get_or_create_extracts()[id]
         all_needs = SphinxNeedsData(env).get_or_create_needs()
-        content: List[nodes.Element] = []
+        content: list[nodes.Element] = []
 
         # check if filter argument and option filter both exist
         need_filter_arg = current_needextract["filter_arg"]
         if need_filter_arg and current_needextract["filter"]:
-            raise NeedsInvalidFilter("Needextract can't have filter arguments and option filter at the same time.")
+            raise NeedsInvalidFilter(
+                "Needextract can't have filter arguments and option filter at the same time."
+            )
         elif need_filter_arg:
             # check if given filter argument is need-id
             if need_filter_arg in all_needs:
                 need_filter_arg = f'id == "{need_filter_arg}"'
             elif re.fullmatch(needs_config.id_regex, need_filter_arg):
                 # check if given filter argument is need-id, but not exists
-                raise NeedsInvalidFilter(f"Provided id {need_filter_arg} for needextract does not exist.")
+                raise NeedsInvalidFilter(
+                    f"Provided id {need_filter_arg} for needextract does not exist."
+                )
             current_needextract["filter"] = need_filter_arg
 
         found_needs = process_filters(app, all_needs.values(), current_needextract)
 
         for need_info in found_needs:
             # filter out need_part from found_needs, in order to generate
             # copies of filtered needs with custom layout and style
@@ -116,19 +123,21 @@
 
                 # Add lineno to node
                 need_extract.line = current_needextract["lineno"]
 
                 content.append(need_extract)
 
         if len(content) == 0:
-            content.append(no_needs_found_paragraph())
+            content.append(
+                no_needs_found_paragraph(current_needextract.get("filter_warning"))
+            )
 
         if current_needextract["show_filters"]:
             content.append(used_filter_paragraph(current_needextract))
 
         node.replace_self(content)
 
     if found_needs:
         # Run docutils/sphinx transformers for the by needextract added nodes.
         # Transformers use the complete document (doctree), so we perform this action once per
         # needextract. No matter if one or multiple needs got copied
-        Substitutions(doctree).apply()
+        Substitutions(doctree).apply()  # type: ignore[no-untyped-call]
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needfilter.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needfilter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from __future__ import annotations
+
 import os
-from typing import List, Sequence
+from contextlib import suppress
+from typing import Sequence
 from urllib.parse import urlparse
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from jinja2 import Template
 from sphinx.application import Sphinx
 from sphinx.errors import NoUri
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.diagrams_common import create_legend
+from sphinx_needs.directives.utils import no_needs_found_paragraph
 from sphinx_needs.filter_common import FilterBase, process_filters
 from sphinx_needs.utils import add_doc, remove_node_from_tree, row_col_maker
 
 
 class Needfilter(nodes.General, nodes.Element):
     pass
 
@@ -42,15 +46,17 @@
 
     # Update the options_spec with values defined in the FilterBase class
     option_spec.update(FilterBase.base_option_spec)
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
-        targetid = "needfilter-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needfilter"))
+        targetid = "needfilter-{docname}-{id}".format(
+            docname=env.docname, id=env.new_serialno("needfilter")
+        )
         targetnode = nodes.target("", "", ids=[targetid])
 
         # Add the need and all needed information
         data = SphinxNeedsData(env)._get_or_create_filters()
         data[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
@@ -65,15 +71,18 @@
 
         add_doc(env, env.docname)
 
         return [targetnode, Needfilter("")]
 
 
 def process_needfilters(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     # Replace all needlist nodes with a list of the collected needs.
     # Augment each need with a backlink to the original location.
     builder = app.builder
     env = app.env
     needs_config = NeedsSphinxConfig(env.config)
     all_needs = SphinxNeedsData(env).get_or_create_needs()
@@ -84,31 +93,31 @@
         if not needs_config.include_needs:
             remove_node_from_tree(node)
             continue
 
         id = node.attributes["ids"][0]
         current_needfilter = SphinxNeedsData(env)._get_or_create_filters()[id]
 
-        content: List[nodes.Element]
+        content: nodes.Element | list[nodes.Element]
         if current_needfilter["layout"] == "list":
             content = []
 
         elif current_needfilter["layout"] == "diagram":
             content = []
             try:
                 if "sphinxcontrib.plantuml" not in app.config.extensions:
                     raise ImportError
                 from sphinxcontrib.plantuml import plantuml
             except ImportError:
-                content = nodes.error()
-                para = nodes.paragraph()
+                error_node = nodes.error()
+                para_node = nodes.paragraph()
                 text = nodes.Text("PlantUML is not available!")
-                para += text
-                content.append(para)
-                node.replace_self(content)
+                para_node += text
+                error_node.append(para_node)
+                node.replace_self(error_node)
                 continue
 
             plantuml_block_text = ".. plantuml::\n" "\n" "   @startuml" "   @enduml"
             puml_node = plantuml(plantuml_block_text)
 
             # Add source origin
             puml_node.line = current_needfilter["lineno"]
@@ -122,15 +131,22 @@
             tgroup = nodes.tgroup()
             id_colspec = nodes.colspec(colwidth=5)
             title_colspec = nodes.colspec(colwidth=15)
             type_colspec = nodes.colspec(colwidth=5)
             status_colspec = nodes.colspec(colwidth=5)
             links_colspec = nodes.colspec(colwidth=5)
             tags_colspec = nodes.colspec(colwidth=5)
-            tgroup += [id_colspec, title_colspec, type_colspec, status_colspec, links_colspec, tags_colspec]
+            tgroup += [
+                id_colspec,
+                title_colspec,
+                type_colspec,
+                status_colspec,
+                links_colspec,
+                tags_colspec,
+            ]
             tgroup += nodes.thead(
                 "",
                 nodes.row(
                     "",
                     nodes.entry("", nodes.paragraph("", "ID")),
                     nodes.entry("", nodes.paragraph("", "Title")),
                     nodes.entry("", nodes.paragraph("", "Type")),
@@ -146,116 +162,137 @@
         found_needs = process_filters(app, all_needs.values(), current_needfilter)
 
         line_block = nodes.line_block()
         for need_info in found_needs:
             target_id = need_info["target_id"]
 
             if current_needfilter["layout"] == "list":
-                para = nodes.line()
+                line_node = nodes.line()
                 description = "{}: {}".format(need_info["id"], need_info["title"])
 
                 if current_needfilter["show_status"] and need_info["status"]:
-                    description += " (%s)" % need_info["status"]
+                    description += " ({})".format(need_info["status"])
 
                 if current_needfilter["show_tags"] and need_info["tags"]:
-                    description += " [%s]" % "; ".join(need_info["tags"])
+                    description += " [{}]".format("; ".join(need_info["tags"]))
 
                 title = nodes.Text(description)
 
                 # Create a reference
                 if need_info["hide"]:
-                    para += title
-                else:
+                    line_node += title
+                elif _docname := need_info["docname"]:
                     ref = nodes.reference("", "")
-                    ref["refdocname"] = need_info["docname"]
-                    ref["refuri"] = builder.get_relative_uri(fromdocname, need_info["docname"])
+                    ref["refdocname"] = _docname
+                    ref["refuri"] = builder.get_relative_uri(fromdocname, _docname)
                     ref["refuri"] += "#" + target_id
                     ref.append(title)
-                    para += ref
+                    line_node += ref
 
-                line_block.append(para)
+                line_block.append(line_node)
             elif current_needfilter["layout"] == "table":
                 row = nodes.row()
-                row += row_col_maker(app, fromdocname, all_needs, need_info, "id", make_ref=True)
+                row += row_col_maker(
+                    app, fromdocname, all_needs, need_info, "id", make_ref=True
+                )
                 row += row_col_maker(app, fromdocname, all_needs, need_info, "title")
-                row += row_col_maker(app, fromdocname, all_needs, need_info, "type_name")
+                row += row_col_maker(
+                    app, fromdocname, all_needs, need_info, "type_name"
+                )
                 row += row_col_maker(app, fromdocname, all_needs, need_info, "status")
-                row += row_col_maker(app, fromdocname, all_needs, need_info, "links", ref_lookup=True)
+                row += row_col_maker(
+                    app, fromdocname, all_needs, need_info, "links", ref_lookup=True
+                )
                 row += row_col_maker(app, fromdocname, all_needs, need_info, "tags")
                 tbody += row
             elif current_needfilter["layout"] == "diagram":
                 # Link calculation
                 # All links we can get from docutils functions will be relative.
                 # But the generated link in the svg will be relative to the svg-file location
                 # (e.g. server.com/docs/_images/sqwxo499cnq329439dfjne.svg)
                 # and not to current documentation. Therefore we need to add ../ to get out of the image folder.
-                try:
-                    link = (
-                        "../"
-                        + builder.get_target_uri(need_info["docname"])
-                        + "?highlight={}".format(urlparse(need_info["title"]))
-                        + "#"
-                        + target_id
-                    )  # Gets mostly called during latex generation
-                except NoUri:
-                    link = ""
+                link = ""
+                with suppress(NoUri):
+                    # Gets mostly called during latex generation
+                    if _docname := need_info["docname"]:
+                        link = (
+                            "../"
+                            + builder.get_target_uri(_docname)
+                            + "?highlight={}".format(urlparse(need_info["title"]))
+                            + "#"
+                            + target_id
+                        )
 
                 diagram_template = Template(needs_config.diagram_template)
-                node_text = diagram_template.render(**need_info, **needs_config.render_context)
+                node_text = diagram_template.render(
+                    **need_info, **needs_config.render_context
+                )
 
-                puml_node["uml"] += '{style} "{node_text}" as {id} [[{link}]] {color}\n'.format(
-                    id=need_info["id"],
-                    node_text=node_text,
-                    link=link,
-                    color=need_info["type_color"],
-                    style=need_info["type_style"],
+                puml_node["uml"] += (
+                    '{style} "{node_text}" as {id} [[{link}]] {color}\n'.format(
+                        id=need_info["id"],
+                        node_text=node_text,
+                        link=link,
+                        color=need_info["type_color"],
+                        style=need_info["type_style"],
+                    )
                 )
                 for link in need_info["links"]:
-                    puml_connections += "{id} --> {link}\n".format(id=need_info["id"], link=link)
+                    puml_connections += "{id} --> {link}\n".format(
+                        id=need_info["id"], link=link
+                    )
 
         if current_needfilter["layout"] == "list":
             content.append(line_block)
 
         if current_needfilter["layout"] == "diagram":
             puml_node["uml"] += puml_connections
 
             # Create a legend
 
             if current_needfilter["show_legend"]:
                 puml_node["uml"] += create_legend(needs_config.types)
             puml_node["uml"] += "@enduml"
             puml_node["incdir"] = os.path.dirname(current_needfilter["docname"])
-            puml_node["filename"] = os.path.split(current_needfilter["docname"])[1]  # Needed for plantuml >= 0.9
+            puml_node["filename"] = os.path.split(current_needfilter["docname"])[
+                1
+            ]  # Needed for plantuml >= 0.9
             content.append(puml_node)
 
         if len(content) == 0:
-            nothing_found = "No needs passed the filters"
-            para = nodes.line()
-            nothing_found_node = nodes.Text(nothing_found)
-            para += nothing_found_node
-            content.append(para)
+            content.append(
+                no_needs_found_paragraph(current_needfilter.get("filter_warning"))
+            )
         if current_needfilter["show_filters"]:
-            para = nodes.paragraph()
+            para_node = nodes.paragraph()
             filter_text = "Used filter:"
             filter_text += (
-                " status(%s)" % " OR ".join(current_needfilter["status"])
+                " status({})".format(" OR ".join(current_needfilter["status"]))
                 if len(current_needfilter["status"]) > 0
                 else ""
             )
-            if len(current_needfilter["status"]) > 0 and len(current_needfilter["tags"]) > 0:
+            if (
+                len(current_needfilter["status"]) > 0
+                and len(current_needfilter["tags"]) > 0
+            ):
                 filter_text += " AND "
             filter_text += (
-                " tags(%s)" % " OR ".join(current_needfilter["tags"]) if len(current_needfilter["tags"]) > 0 else ""
+                " tags({})".format(" OR ".join(current_needfilter["tags"]))
+                if len(current_needfilter["tags"]) > 0
+                else ""
             )
-            if (len(current_needfilter["status"]) > 0 or len(current_needfilter["tags"]) > 0) and len(
-                current_needfilter["types"]
-            ) > 0:
+            if (
+                len(current_needfilter["status"]) > 0
+                or len(current_needfilter["tags"]) > 0
+            ) and len(current_needfilter["types"]) > 0:
                 filter_text += " AND "
             filter_text += (
-                " types(%s)" % " OR ".join(current_needfilter["types"]) if len(current_needfilter["types"]) > 0 else ""
+                " types({})".format(" OR ".join(current_needfilter["types"]))
+                if len(current_needfilter["types"]) > 0
+                else ""
             )
 
             filter_node = nodes.emphasis(filter_text, filter_text)
-            para += filter_node
-            content.append(para)
+            para_node += filter_node
+            content.append(para_node)
 
         node.replace_self(content)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needflow.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
+from __future__ import annotations
+
 import html
 import os
-from typing import Dict, Iterable, List, Sequence
+from typing import Iterable, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from jinja2 import Template
 from sphinx.application import Sphinx
 from sphinxcontrib.plantuml import (
     generate_name,  # Need for plantuml filename calculation
 )
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import (
     NeedsFlowType,
     NeedsInfoType,
-    NeedsPartsInfoType,
     SphinxNeedsData,
 )
 from sphinx_needs.debug import measure_time
 from sphinx_needs.diagrams_common import calculate_link, create_legend
+from sphinx_needs.directives.utils import no_needs_found_paragraph
 from sphinx_needs.filter_common import FilterBase, filter_single_need, process_filters
 from sphinx_needs.logging import get_logger
 from sphinx_needs.utils import (
     add_doc,
     get_scale,
     remove_node_from_tree,
     split_link_types,
 )
 
 logger = get_logger(__name__)
 
 
-NEEDFLOW_TEMPLATES: Dict[str, Template] = {}
+NEEDFLOW_TEMPLATES: dict[str, Template] = {}
 
 
 class Needflow(nodes.General, nodes.Element):
     pass
 
 
 class NeedflowDirective(FilterBase):
@@ -67,15 +69,17 @@
         location = (env.docname, self.lineno)
 
         id = env.new_serialno("needflow")
         targetid = f"needflow-{env.docname}-{id}"
         targetnode = nodes.target("", "", ids=[targetid])
 
         all_link_types = ",".join(x["option"] for x in needs_config.extra_links)
-        link_types = split_link_types(self.options.get("link_types", all_link_types), location)
+        link_types = split_link_types(
+            self.options.get("link_types", all_link_types), location
+        )
 
         config_names = self.options.get("config")
         configs = []
         if config_names:
             for config_name in config_names.split(","):
                 config_name = config_name.strip()
                 if config_name and config_name in needs_config.flow_configs:
@@ -116,15 +120,15 @@
 
 
 def get_need_node_rep_for_plantuml(
     app: Sphinx,
     fromdocname: str,
     current_needflow: NeedsFlowType,
     all_needs: Iterable[NeedsInfoType],
-    need_info: NeedsPartsInfoType,
+    need_info: NeedsInfoType,
 ) -> str:
     """Calculate need node representation for plantuml."""
     needs_config = NeedsSphinxConfig(app.config)
     diagram_template = get_template(needs_config.diagram_template)
 
     node_text = diagram_template.render(**need_info, **needs_config.render_context)
 
@@ -158,16 +162,16 @@
 
 
 def walk_curr_need_tree(
     app: Sphinx,
     fromdocname: str,
     current_needflow: NeedsFlowType,
     all_needs: Iterable[NeedsInfoType],
-    found_needs: List[NeedsPartsInfoType],
-    need: NeedsPartsInfoType,
+    found_needs: list[NeedsInfoType],
+    need: NeedsInfoType,
 ) -> str:
     """
     Walk through each need to find all its child needs and need parts recursively and wrap them together in nested structure.
     """
 
     curr_need_tree = ""
 
@@ -213,27 +217,32 @@
                     child_need_node = get_need_node_rep_for_plantuml(
                         app, fromdocname, current_needflow, all_needs, curr_child_need
                     )
                     curr_need_tree += child_need_node
                     # check curr need child has children or has parts
                     if curr_child_need["parent_needs_back"] or curr_child_need["parts"]:
                         curr_need_tree += walk_curr_need_tree(
-                            app, fromdocname, current_needflow, all_needs, found_needs, curr_child_need
+                            app,
+                            fromdocname,
+                            current_needflow,
+                            all_needs,
+                            found_needs,
+                            curr_child_need,
                         )
                     # add newline for next element
                     curr_need_tree += "\n"
             idx += 1
 
     # We processed embedded needs or need parts, so we will close with "}"
     curr_need_tree += "}"
 
     return curr_need_tree
 
 
-def get_root_needs(found_needs: List[NeedsPartsInfoType]) -> List[NeedsPartsInfoType]:
+def get_root_needs(found_needs: list[NeedsInfoType]) -> list[NeedsInfoType]:
     return_list = []
     for current_need in found_needs:
         if current_need["is_need"]:
             if "parent_need" not in current_need or current_need["parent_need"] == "":
                 # need has no parent, we have to add the need to the root needs
                 return_list.append(current_need)
             else:
@@ -248,21 +257,23 @@
 
 
 def cal_needs_node(
     app: Sphinx,
     fromdocname: str,
     current_needflow: NeedsFlowType,
     all_needs: Iterable[NeedsInfoType],
-    found_needs: List[NeedsPartsInfoType],
+    found_needs: list[NeedsInfoType],
 ) -> str:
     """Calculate and get needs node representaion for plantuml including all child needs and need parts."""
     top_needs = get_root_needs(found_needs)
     curr_need_tree = ""
     for top_need in top_needs:
-        top_need_node = get_need_node_rep_for_plantuml(app, fromdocname, current_needflow, all_needs, top_need)
+        top_need_node = get_need_node_rep_for_plantuml(
+            app, fromdocname, current_needflow, all_needs, top_need
+        )
         curr_need_tree += (
             top_need_node
             + walk_curr_need_tree(
                 app,
                 fromdocname,
                 current_needflow,
                 all_needs,
@@ -271,15 +282,20 @@
             )
             + "\n"
         )
     return curr_need_tree
 
 
 @measure_time("needflow")
-def process_needflow(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needflow(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     # Replace all needflow nodes with a list of the collected needs.
     # Augment each need with a backlink to the original location.
     env = app.env
     needs_config = NeedsSphinxConfig(app.config)
     env_data = SphinxNeedsData(env)
     all_needs = env_data.get_or_create_needs()
 
@@ -298,33 +314,36 @@
         current_needflow = env_data.get_or_create_flows()[id]
 
         option_link_types = [link.upper() for link in current_needflow["link_types"]]
         for lt in option_link_types:
             if lt not in link_type_names:
                 logger.warning(
                     "Unknown link type {link_type} in needflow {flow}. Allowed values: {link_types} [needs]".format(
-                        link_type=lt, flow=current_needflow["target_id"], link_types=",".join(link_type_names)
+                        link_type=lt,
+                        flow=current_needflow["target_id"],
+                        link_types=",".join(link_type_names),
                     ),
                     type="needs",
                 )
 
-        content = []
         try:
             if "sphinxcontrib.plantuml" not in app.config.extensions:
                 raise ImportError
             from sphinxcontrib.plantuml import plantuml
         except ImportError:
-            content = nodes.error()
+            error_node = nodes.error()
             para = nodes.paragraph()
             text = nodes.Text("PlantUML is not available!")
             para += text
-            content.append(para)
-            node.replace_self(content)
+            error_node.append(para)
+            node.replace_self(error_node)
             continue
 
+        content: list[nodes.Element] = []
+
         found_needs = process_filters(app, all_needs.values(), current_needflow)
 
         if found_needs:
             plantuml_block_text = ".. plantuml::\n" "\n" "   @startuml" "   @enduml"
             puml_node = plantuml(plantuml_block_text)
 
             # Add source origin
@@ -334,99 +353,117 @@
             puml_node["uml"] = "@startuml\n"
             puml_connections = ""
 
             # Adding config
             config = current_needflow["config"]
             if config and len(config) >= 3:
                 # Remove all empty lines
-                config = "\n".join([line.strip() for line in config.split("\n") if line.strip()])
+                config = "\n".join(
+                    [line.strip() for line in config.split("\n") if line.strip()]
+                )
                 puml_node["uml"] += "\n' Config\n\n"
                 puml_node["uml"] += config
                 puml_node["uml"] += "\n\n"
 
             puml_node["uml"] += "\n' Nodes definition \n\n"
 
             for need_info in found_needs:
                 for link_type in link_types:
                     # Skip link-type handling, if it is not part of a specified list of allowed link_types or
                     # if not part of the overall configuration of needs_flow_link_types
-                    if (current_needflow["link_types"] and link_type["option"].upper() not in option_link_types) or (
+                    if (
+                        current_needflow["link_types"]
+                        and link_type["option"].upper() not in option_link_types
+                    ) or (
                         not current_needflow["link_types"]
-                        and link_type["option"].upper() not in allowed_link_types_options
+                        and link_type["option"].upper()
+                        not in allowed_link_types_options
                     ):
                         continue
 
                     # skip creating links from child needs to their own parent need
                     if link_type["option"] == "parent_needs":
                         continue
 
                     for link in need_info[link_type["option"]]:  # type: ignore[literal-required]
                         # If source or target of link is a need_part, a specific style is needed
                         if "." in link or "." in need_info["id_complete"]:
                             final_link = link
-                            if current_needflow["show_link_names"] or needs_config.flow_show_links:
+                            if (
+                                current_needflow["show_link_names"]
+                                or needs_config.flow_show_links
+                            ):
                                 desc = link_type["outgoing"] + "\\n"
                                 comment = f": {desc}"
                             else:
                                 comment = ""
 
-                            if "style_part" in link_type and link_type["style_part"]:
-                                link_style = "[{style}]".format(style=link_type["style_part"])
+                            if _style_part := link_type.get("style_part"):
+                                link_style = f"[{_style_part}]"
                             else:
                                 link_style = "[dotted]"
                         else:
                             final_link = link
-                            if current_needflow["show_link_names"] or needs_config.flow_show_links:
+                            if (
+                                current_needflow["show_link_names"]
+                                or needs_config.flow_show_links
+                            ):
                                 comment = ": {desc}".format(desc=link_type["outgoing"])
                             else:
                                 comment = ""
 
-                            if "style" in link_type and link_type["style"]:
-                                link_style = "[{style}]".format(style=link_type["style"])
+                            if _style := link_type.get("style"):
+                                link_style = f"[{_style}]"
                             else:
                                 link_style = ""
 
                         # Do not create an links, if the link target is not part of the search result.
-                        if final_link not in [x["id"] for x in found_needs if x["is_need"]] and final_link not in [
+                        if final_link not in [
+                            x["id"] for x in found_needs if x["is_need"]
+                        ] and final_link not in [
                             x["id_complete"] for x in found_needs if x["is_part"]
                         ]:
                             continue
 
-                        if "style_start" in link_type and link_type["style_start"]:
-                            style_start = link_type["style_start"]
+                        if _style_start := link_type.get("style_start"):
+                            style_start = _style_start
                         else:
                             style_start = "-"
 
-                        if "style_end" in link_type and link_type["style_end"]:
-                            style_end = link_type["style_end"]
+                        if _style_end := link_type.get("style_end"):
+                            style_end = _style_end
                         else:
                             style_end = "->"
 
                         puml_connections += "{id} {style_start}{link_style}{style_end} {link}{comment}\n".format(
                             id=make_entity_name(need_info["id_complete"]),
                             link=make_entity_name(final_link),
                             comment=comment,
                             link_style=link_style,
                             style_start=style_start,
                             style_end=style_end,
                         )
 
             # calculate needs node representation for plantuml
-            puml_node["uml"] += cal_needs_node(app, fromdocname, current_needflow, all_needs.values(), found_needs)
+            puml_node["uml"] += cal_needs_node(
+                app, fromdocname, current_needflow, all_needs.values(), found_needs
+            )
 
             puml_node["uml"] += "\n' Connection definition \n\n"
             puml_node["uml"] += puml_connections
 
             # Create a legend
             if current_needflow["show_legend"]:
                 puml_node["uml"] += create_legend(needs_config.types)
 
             puml_node["uml"] += "\n@enduml"
             puml_node["incdir"] = os.path.dirname(current_needflow["docname"])
-            puml_node["filename"] = os.path.split(current_needflow["docname"])[1]  # Needed for plantuml >= 0.9
+            puml_node["filename"] = os.path.split(current_needflow["docname"])[
+                1
+            ]  # Needed for plantuml >= 0.9
 
             scale = int(current_needflow["scale"])
             # if scale != 100:
             puml_node["scale"] = scale
 
             puml_node = nodes.figure("", puml_node)
 
@@ -444,66 +481,79 @@
                         file_ext = "png"
                 except Exception:
                     file_ext = "png"
 
                 gen_flow_link = generate_name(app, puml_node.children[0], file_ext)
                 current_file_parts = fromdocname.split("/")
                 subfolder_amount = len(current_file_parts) - 1
-                img_locaton = "../" * subfolder_amount + "_images/" + gen_flow_link[0].split("/")[-1]
-                flow_ref = nodes.reference("t", current_needflow["caption"], refuri=img_locaton)
+                img_locaton = (
+                    "../" * subfolder_amount
+                    + "_images/"
+                    + gen_flow_link[0].split("/")[-1]
+                )
+                flow_ref = nodes.reference(
+                    "t", current_needflow["caption"], refuri=img_locaton
+                )
                 puml_node += nodes.caption("", "", flow_ref)
 
             # Add lineno to node
             puml_node.line = current_needflow["lineno"]
 
             content.append(puml_node)
         else:  # no needs found
-            nothing_found = "No needs passed the filters"
-            para = nodes.paragraph()
-            nothing_found_node = nodes.Text(nothing_found)
-            para += nothing_found_node
-            content.append(para)
+            content.append(
+                no_needs_found_paragraph(current_needflow.get("filter_warning"))
+            )
 
         if current_needflow["show_filters"]:
             para = nodes.paragraph()
             filter_text = "Used filter:"
             filter_text += (
-                " status(%s)" % " OR ".join(current_needflow["status"]) if len(current_needflow["status"]) > 0 else ""
+                " status({})".format(" OR ".join(current_needflow["status"]))
+                if len(current_needflow["status"]) > 0
+                else ""
             )
-            if len(current_needflow["status"]) > 0 and len(current_needflow["tags"]) > 0:
+            if (
+                len(current_needflow["status"]) > 0
+                and len(current_needflow["tags"]) > 0
+            ):
                 filter_text += " AND "
             filter_text += (
-                " tags(%s)" % " OR ".join(current_needflow["tags"]) if len(current_needflow["tags"]) > 0 else ""
+                " tags({})".format(" OR ".join(current_needflow["tags"]))
+                if len(current_needflow["tags"]) > 0
+                else ""
             )
-            if (len(current_needflow["status"]) > 0 or len(current_needflow["tags"]) > 0) and len(
-                current_needflow["types"]
-            ) > 0:
+            if (
+                len(current_needflow["status"]) > 0 or len(current_needflow["tags"]) > 0
+            ) and len(current_needflow["types"]) > 0:
                 filter_text += " AND "
             filter_text += (
-                " types(%s)" % " OR ".join(current_needflow["types"]) if len(current_needflow["types"]) > 0 else ""
+                " types({})".format(" OR ".join(current_needflow["types"]))
+                if len(current_needflow["types"]) > 0
+                else ""
             )
 
             filter_node = nodes.emphasis(filter_text, filter_text)
             para += filter_node
             content.append(para)
 
         # We have to restrustructer the needflow
         # If this block should be organized differently
         if current_needflow["debug"] and found_needs:
             # We can only access puml_node if found_needs is set.
             # Otherwise it was not been set, or we get outdated data
             debug_container = nodes.container()
             if isinstance(puml_node, nodes.figure):
-                data = puml_node.children[0]["uml"]
+                data = puml_node.children[0]["uml"]  # type: ignore
             else:
                 data = puml_node["uml"]
             data = "\n".join([html.escape(line) for line in data.split("\n")])
             debug_para = nodes.raw("", f"<pre>{data}</pre>", format="html")
             debug_container += debug_para
-            content += debug_container
+            content.append(debug_container)
 
         node.replace_self(content)
 
 
 def get_template(template_name: str) -> Template:
     """Checks if a template got already rendered, if it's the case, return it"""
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needgantt.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needgantt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import os
 import re
 from datetime import datetime
-from typing import List, Sequence
+from typing import Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinxcontrib.plantuml import (
     generate_name,  # Need for plantuml filename calculation
 )
@@ -16,15 +18,18 @@
     DiagramBase,
     add_config,
     create_legend,
     get_debug_container,
     get_filter_para,
     no_plantuml,
 )
-from sphinx_needs.directives.utils import SphinxNeedsLinkTypeException
+from sphinx_needs.directives.utils import (
+    SphinxNeedsLinkTypeException,
+    no_needs_found_paragraph,
+)
 from sphinx_needs.filter_common import FilterBase, filter_single_need, process_filters
 from sphinx_needs.logging import get_logger
 from sphinx_needs.utils import MONTH_NAMES, add_doc, remove_node_from_tree
 
 logger = get_logger(__name__)
 
 
@@ -69,33 +74,39 @@
         start_date = self.options.get("start_date")
         if start_date:
             try:
                 datetime.strptime(start_date, "%Y-%m-%d")
                 # datetime.fromisoformat(start_date) # > py3.7 only
             except Exception:
                 raise NeedGanttException(
-                    "Given start date {} is not valid. Please use YYYY-MM-DD as format. "
-                    "E.g. 2020-03-27".format(start_date)
+                    f"Given start date {start_date} is not valid. Please use YYYY-MM-DD as format. "
+                    "E.g. 2020-03-27"
                 )
         else:
             start_date = None  # If None we do not set a start date later
 
         timeline = self.options.get("timeline")
         timeline_options = ["daily", "weekly", "monthly"]
         if timeline and timeline not in timeline_options:
             raise NeedGanttException(
-                "Given scale value {} is invalid. Please use: " "{}".format(timeline, ",".join(timeline_options))
+                "Given scale value {} is invalid. Please use: " "{}".format(
+                    timeline, ",".join(timeline_options)
+                )
             )
         else:
             timeline = None  # Timeline/scale not set later
 
         no_color = "no_color" in self.options
 
-        duration_option = self.options.get("duration_option", needs_config.duration_option)
-        completion_option = self.options.get("completion_option", needs_config.completion_option)
+        duration_option = self.options.get(
+            "duration_option", needs_config.duration_option
+        )
+        completion_option = self.options.get(
+            "completion_option", needs_config.completion_option
+        )
 
         # Add the needgantt and all needed information
         SphinxNeedsData(env).get_or_create_gantts()[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
             "target_id": targetid,
             "starts_with_links": starts_with_links,
@@ -109,35 +120,46 @@
             "completion_option": completion_option,
             **self.collect_filter_attributes(),
             **self.collect_diagram_attributes(),
         }
 
         add_doc(env, env.docname)
 
-        return [targetnode] + [Needgantt("")]
+        gantt_node = Needgantt("")
+        self.set_source_info(gantt_node)
+
+        return [targetnode, gantt_node]
 
-    def get_link_type_option(self, name: str, default: str = "") -> List[str]:
-        link_types = [x.strip() for x in re.split(";|,", self.options.get(name, default))]
+    def get_link_type_option(self, name: str, default: str = "") -> list[str]:
+        link_types = [
+            x.strip() for x in re.split(";|,", self.options.get(name, default))
+        ]
         conf_link_types = NeedsSphinxConfig(self.env.config).extra_links
         conf_link_types_name = [x["option"] for x in conf_link_types]
 
         final_link_types = []
         for link_type in link_types:
             if link_type is None or link_type == "":
                 continue
             if link_type not in conf_link_types_name:
                 raise SphinxNeedsLinkTypeException(
-                    link_type + "does not exist in configuration option needs_extra_links"
+                    link_type
+                    + "does not exist in configuration option needs_extra_links"
                 )
 
             final_link_types.append(link_type)
         return final_link_types
 
 
-def process_needgantt(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needgantt(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     # Replace all needgantt nodes with a list of the collected needs.
     env = app.env
     needs_config = NeedsSphinxConfig(app.config)
 
     # link_types = needs_config.extra_links
     # allowed_link_types_options = [link.upper() for link in needs_config.flow_link_types]
 
@@ -187,15 +209,17 @@
         if start_date_string:
             try:
                 start_date = datetime.strptime(start_date_string, "%Y-%m-%d")
                 # start_date = datetime.fromisoformat(start_date_string)  # > py3.7 only
             except Exception:
                 raise NeedGanttException(
                     'start_date "{}"for needgantt is invalid. '
-                    'File: {}:current_needgantt["lineno"]'.format(start_date_string, current_needgantt["docname"])
+                    'File: {}:current_needgantt["lineno"]'.format(
+                        start_date_string, current_needgantt["docname"]
+                    )
                 )
 
             month = MONTH_NAMES[int(start_date.strftime("%m"))]
             start_date_plantuml = start_date.strftime(f"%dth of {month} %Y")
         if start_date_plantuml:
             puml_node["uml"] += f"Project starts the {start_date_plantuml}\n"
 
@@ -203,44 +227,63 @@
         puml_node["uml"] += "\n' Elements definition \n\n"
         el_completion_string = ""
         el_color_string = ""
         for need in found_needs:
             complete = None
 
             if current_needgantt["milestone_filter"]:
-                is_milestone = filter_single_need(need, needs_config, current_needgantt["milestone_filter"])
+                is_milestone = filter_single_need(
+                    need, needs_config, current_needgantt["milestone_filter"]
+                )
             else:
                 is_milestone = False
 
             if current_needgantt["milestone_filter"] and is_milestone:
-                gantt_element = "[{}] as [{}] lasts 0 days\n".format(need["title"], need["id"])
+                gantt_element = "[{}] as [{}] lasts 0 days\n".format(
+                    need["title"], need["id"]
+                )
             else:  # Normal gantt element handling
                 duration_option = current_needgantt["duration_option"]
                 duration = need[duration_option]  # type: ignore[literal-required]
                 complete_option = current_needgantt["completion_option"]
                 complete = need[complete_option]  # type: ignore[literal-required]
                 if not (duration and duration.isdigit()):
+                    need_location = (
+                        f" (located: {need['docname']}:{need['lineno']})"
+                        if need["docname"]
+                        else ""
+                    )
                     logger.warning(
                         "Duration not set or invalid for needgantt chart. "
-                        "Need: {}. Duration: {} [needs]".format(need["id"], duration),
+                        f"Need: {need['id']!r}{need_location}. Duration: {duration!r} [needs.gantt]",
                         type="needs",
+                        subtype="gantt",
+                        location=node,
                     )
                     duration = 1
-                gantt_element = "[{}] as [{}] lasts {} days\n".format(need["title"], need["id"], duration)
+                gantt_element = "[{}] as [{}] lasts {} days\n".format(
+                    need["title"], need["id"], duration
+                )
 
             if complete:
                 complete = complete.replace("%", "")
-                el_completion_string += "[{}] is {}% completed\n".format(need["title"], complete)
+                el_completion_string += "[{}] is {}% completed\n".format(
+                    need["title"], complete
+                )
 
-            el_color_string += "[{}] is colored in {}\n".format(need["title"], need["type_color"])
+            el_color_string += "[{}] is colored in {}\n".format(
+                need["title"], need["type_color"]
+            )
 
             puml_node["uml"] += gantt_element
 
         puml_node["uml"] += "\n' Element links definition \n\n"
-        puml_node["uml"] += "\n' Deactivated, as currently supported by plantuml beta only"
+        puml_node["uml"] += (
+            "\n' Deactivated, as currently supported by plantuml beta only"
+        )
 
         puml_node["uml"] += "\n' Element completion definition \n\n"
         puml_node["uml"] += el_completion_string + "\n"
 
         puml_node["uml"] += "\n' Element color definition \n\n"
         if current_needgantt["no_color"]:
             puml_node["uml"] += "' Color support deactivated via flag"
@@ -248,18 +291,24 @@
             puml_node["uml"] += el_color_string + "\n"
 
         # Constrain handling
         puml_node["uml"] += "\n' Constraints definition \n\n"
         puml_node["uml"] += "\n' Constraints definition \n\n"
         for need in found_needs:
             if current_needgantt["milestone_filter"]:
-                is_milestone = filter_single_need(need, needs_config, current_needgantt["milestone_filter"])
+                is_milestone = filter_single_need(
+                    need, needs_config, current_needgantt["milestone_filter"]
+                )
             else:
                 is_milestone = False
-            for con_type in ("starts_with_links", "starts_after_links", "ends_with_links"):
+            for con_type in (
+                "starts_with_links",
+                "starts_after_links",
+                "ends_with_links",
+            ):
                 if is_milestone:
                     keyword = "happens"
                 elif con_type in ["starts_with_links", "starts_after_links"]:
                     keyword = "starts"
                 else:
                     keyword = "ends"
 
@@ -279,15 +328,17 @@
 
         # Create a legend
         if current_needgantt["show_legend"]:
             puml_node["uml"] += create_legend(needs_config.types)
 
         puml_node["uml"] += "\n@endgantt"
         puml_node["incdir"] = os.path.dirname(current_needgantt["docname"])
-        puml_node["filename"] = os.path.split(current_needgantt["docname"])[1]  # Needed for plantuml >= 0.9
+        puml_node["filename"] = os.path.split(current_needgantt["docname"])[
+            1
+        ]  # Needed for plantuml >= 0.9
 
         scale = int(current_needgantt["scale"])
         # if scale != 100:
         puml_node["scale"] = scale
 
         puml_node = nodes.figure("", puml_node)
 
@@ -302,26 +353,28 @@
                     file_ext = "png"
             except Exception:
                 file_ext = "png"
 
             gen_flow_link = generate_name(app, puml_node.children[0], file_ext)
             current_file_parts = fromdocname.split("/")
             subfolder_amount = len(current_file_parts) - 1
-            img_location = "../" * subfolder_amount + "_images/" + gen_flow_link[0].split("/")[-1]
-            flow_ref = nodes.reference("t", current_needgantt["caption"], refuri=img_location)
+            img_location = (
+                "../" * subfolder_amount + "_images/" + gen_flow_link[0].split("/")[-1]
+            )
+            flow_ref = nodes.reference(
+                "t", current_needgantt["caption"], refuri=img_location
+            )
             puml_node += nodes.caption("", "", flow_ref)
 
         content.append(puml_node)
 
-        if len(content) == 0:
-            nothing_found = "No needs passed the filters"
-            para = nodes.paragraph()
-            nothing_found_node = nodes.Text(nothing_found)
-            para += nothing_found_node
-            content.append(para)
+        if len(found_needs) == 0:
+            content = [
+                no_needs_found_paragraph(current_needgantt.get("filter_warning"))
+            ]
         if current_needgantt["show_filters"]:
             content.append(get_filter_para(current_needgantt))
 
         if current_needgantt["debug"]:
             content += get_debug_container(puml_node)
 
         puml_node["class"] = ["needgantt"]
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needimport.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needimport.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import json
 import os
 import re
-from typing import Dict, Sequence
+from typing import Sequence
 from urllib.parse import urlparse
 
 import requests
 from docutils import nodes
 from docutils.parsers.rst import directives
 from requests_file import FileAdapter
 from sphinx.util.docutils import SphinxDirective
@@ -67,46 +69,58 @@
             s.mount("file://", FileAdapter())
             try:
                 response = s.get(need_import_path)
                 needs_import_list = (
                     response.json()
                 )  # The downloaded file MUST be json. Everything else we do not handle!
             except Exception as e:
-                raise NeedimportException(f"Getting {need_import_path} didn't work. Reason: {e}.")
+                raise NeedimportException(
+                    f"Getting {need_import_path} didn't work. Reason: {e}."
+                )
         else:
             logger.info(f"Importing needs from {need_import_path}")
 
             if not os.path.isabs(need_import_path):
                 # Relative path should start from current rst file directory
                 curr_dir = os.path.dirname(self.docname)
-                new_need_import_path = os.path.join(self.env.app.srcdir, curr_dir, need_import_path)
+                new_need_import_path = os.path.join(
+                    self.env.app.srcdir, curr_dir, need_import_path
+                )
 
                 correct_need_import_path = new_need_import_path
                 if not os.path.exists(new_need_import_path):
                     # Check the old way that calculates relative path starting from conf.py directory
-                    old_need_import_path = os.path.join(self.env.app.srcdir, need_import_path)
+                    old_need_import_path = os.path.join(
+                        self.env.app.srcdir, need_import_path
+                    )
                     if os.path.exists(old_need_import_path):
                         correct_need_import_path = old_need_import_path
                         logger.warning(
                             "Deprecation warning: Relative path must be relative to the current document in future, "
                             "not to the conf.py location. Use a starting '/', like '/needs.json', to make the path "
                             "relative to conf.py. [needs]",
                             type="needs",
                             location=(self.env.docname, self.lineno),
                         )
             else:
                 # Absolute path starts with /, based on the source directory. The / need to be striped
-                correct_need_import_path = os.path.join(self.env.app.srcdir, need_import_path[1:])
+                correct_need_import_path = os.path.join(
+                    self.env.app.srcdir, need_import_path[1:]
+                )
 
             if not os.path.exists(correct_need_import_path):
-                raise ReferenceError(f"Could not load needs import file {correct_need_import_path}")
+                raise ReferenceError(
+                    f"Could not load needs import file {correct_need_import_path}"
+                )
 
             errors = check_needs_file(correct_need_import_path)
             if errors.schema:
-                logger.info(f"Schema validation errors detected in file {correct_need_import_path}:")
+                logger.info(
+                    f"Schema validation errors detected in file {correct_need_import_path}:"
+                )
                 for error in errors.schema:
                     logger.info(f'  {error.message} -> {".".join(error.path)}')
 
             try:
                 with open(correct_need_import_path) as needs_file:
                     needs_import_list = json.load(needs_file)
             except json.JSONDecodeError as e:
@@ -115,21 +129,27 @@
 
         if version is None:
             try:
                 version = needs_import_list["current_version"]
                 if not isinstance(version, str):
                     raise KeyError
             except KeyError:
-                raise CorruptedNeedsFile(f"Key 'current_version' missing or corrupted in {correct_need_import_path}")
+                raise CorruptedNeedsFile(
+                    f"Key 'current_version' missing or corrupted in {correct_need_import_path}"
+                )
         if version not in needs_import_list["versions"].keys():
-            raise VersionNotFound(f"Version {version} not found in needs import file {correct_need_import_path}")
+            raise VersionNotFound(
+                f"Version {version} not found in needs import file {correct_need_import_path}"
+            )
 
         needs_config = NeedsSphinxConfig(self.config)
         # TODO this is not exactly NeedsInfoType, because the export removes/adds some keys
-        needs_list: Dict[str, NeedsInfoType] = needs_import_list["versions"][version]["needs"]
+        needs_list: dict[str, NeedsInfoType] = needs_import_list["versions"][version][
+            "needs"
+        ]
 
         # Filter imported needs
         needs_list_filtered = {}
         for key, need in needs_list.items():
             if filter_string is None:
                 needs_list_filtered[key] = need
             else:
@@ -139,37 +159,42 @@
                 # "content" is the sphinx internal name for this kind of information
                 filter_context["content"] = need["description"]  # type: ignore[typeddict-item]
                 try:
                     if filter_single_need(filter_context, needs_config, filter_string):
                         needs_list_filtered[key] = need
                 except Exception as e:
                     logger.warning(
-                        "needimport: Filter {} not valid. Error: {}. {}{} [needs]".format(
-                            filter_string, e, self.docname, self.lineno
-                        ),
+                        f"needimport: Filter {filter_string} not valid. Error: {e}. {self.docname}{self.lineno} [needs]",
                         type="needs",
                         location=(self.env.docname, self.lineno),
                     )
 
         needs_list = needs_list_filtered
 
         # If we need to set an id prefix, we also need to manipulate all used ids in the imported data.
         extra_links = needs_config.extra_links
         if id_prefix:
             for need in needs_list.values():
                 for id in needs_list:
                     # Manipulate links in all link types
                     for extra_link in extra_links:
-                        if extra_link["option"] in need and id in need[extra_link["option"]]:  # type: ignore[literal-required]
+                        if (
+                            extra_link["option"] in need
+                            and id in need[extra_link["option"]]  # type: ignore[literal-required]
+                        ):
                             for n, link in enumerate(need[extra_link["option"]]):  # type: ignore[literal-required]
                                 if id == link:
-                                    need[extra_link["option"]][n] = "".join([id_prefix, id])  # type: ignore[literal-required]
+                                    need[extra_link["option"]][n] = "".join(  # type: ignore[literal-required]
+                                        [id_prefix, id]
+                                    )
                     # Manipulate descriptions
                     # ToDo: Use regex for better matches.
-                    need["description"] = need["description"].replace(id, "".join([id_prefix, id]))  # type: ignore[typeddict-item]
+                    need["description"] = need["description"].replace(  # type: ignore[typeddict-item]
+                        id, "".join([id_prefix, id])
+                    )
 
         # tags update
         for need in needs_list.values():
             need["tags"] = need["tags"] + tags
 
         known_options = (
             "title",
@@ -181,23 +206,28 @@
             "template",
             "pre_template",
             "post_template",
             "collapse",
             "style",
             "layout",
             "need_type",
+            "constraints",
             *[x["option"] for x in extra_links],
             *NEEDS_CONFIG.extra_options,
         )
         need_nodes = []
         for need in needs_list.values():
             # Set some values based on given option or value from imported need.
             need["template"] = self.options.get("template", need.get("template"))
-            need["pre_template"] = self.options.get("pre_template", need.get("pre_template"))
-            need["post_template"] = self.options.get("post_template", need.get("post_template"))
+            need["pre_template"] = self.options.get(
+                "pre_template", need.get("pre_template")
+            )
+            need["post_template"] = self.options.get(
+                "post_template", need.get("post_template")
+            )
             need["layout"] = self.options.get("layout", need.get("layout"))
             need["style"] = self.options.get("style", need.get("style"))
 
             if "hide" in self.options:
                 need["hide"] = True
             else:
                 need["hide"] = need.get("hide", False)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needimport_template.rst` & `sphinx_needs-2.1.0/sphinx_needs/directives/needimport_template.rst`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needlist.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needlist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-"""
+from __future__ import annotations
 
-
-"""
-from typing import List, Sequence
+from typing import Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
@@ -39,15 +37,17 @@
 
     # Update the options_spec with values defined in the FilterBase class
     option_spec.update(FilterBase.base_option_spec)
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
-        targetid = "needlist-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needlist"))
+        targetid = "needlist-{docname}-{id}".format(
+            docname=env.docname, id=env.new_serialno("needlist")
+        )
         targetnode = nodes.target("", "", ids=[targetid])
 
         # Add the need and all needed information
         SphinxNeedsData(env).get_or_create_lists()[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
             "target_id": targetid,
@@ -58,15 +58,20 @@
         }
 
         add_doc(env, env.docname)
 
         return [targetnode, Needlist("")]
 
 
-def process_needlist(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needlist(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     """
     Replace all needlist nodes with a list of the collected needs.
     Augment each need with a backlink to the original location.
     """
     builder = app.builder
     env = app.env
 
@@ -75,57 +80,63 @@
     for node in found_nodes:
         if not include_needs:
             remove_node_from_tree(node)
             continue
 
         id = node.attributes["ids"][0]
         current_needfilter = SphinxNeedsData(env).get_or_create_lists()[id]
-        content: List[nodes.Node] = []
+        content: list[nodes.Node] = []
         all_needs = list(SphinxNeedsData(env).get_or_create_needs().values())
         found_needs = process_filters(app, all_needs, current_needfilter)
 
-        line_block = nodes.line_block()
+        if len(found_needs) > 0:
+            line_block = nodes.line_block()
 
-        # Add lineno to node
-        line_block.line = current_needfilter["lineno"]
-        for need_info in found_needs:
-            para = nodes.line()
-            description = "{}: {}".format(need_info["id"], need_info["title"])
-
-            if current_needfilter["show_status"] and need_info["status"]:
-                description += " (%s)" % need_info["status"]
-
-            if current_needfilter["show_tags"] and need_info["tags"]:
-                description += " [%s]" % "; ".join(need_info["tags"])
-
-            title = nodes.Text(description)
-
-            # Create a reference
-            if need_info["hide"]:
-                para += title
-            elif need_info["is_external"]:
-                assert need_info["external_url"] is not None, "External need without URL"
-                ref = nodes.reference("", "")
-
-                ref["refuri"] = check_and_calc_base_url_rel_path(need_info["external_url"], fromdocname)
-
-                ref["classes"].append(need_info["external_css"])
-                ref.append(title)
-                para += ref
-            else:
-                target_id = need_info["target_id"]
-                ref = nodes.reference("", "")
-                ref["refdocname"] = need_info["docname"]
-                ref["refuri"] = builder.get_relative_uri(fromdocname, need_info["docname"])
-                ref["refuri"] += "#" + target_id
-                ref.append(title)
-                para += ref
-            line_block.append(para)
-        content.append(line_block)
+            # Add lineno to node
+            line_block.line = current_needfilter["lineno"]
+            for need_info in found_needs:
+                para = nodes.line()
+                description = "{}: {}".format(need_info["id"], need_info["title"])
+
+                if current_needfilter["show_status"] and need_info["status"]:
+                    description += " ({})".format(need_info["status"])
+
+                if current_needfilter["show_tags"] and need_info["tags"]:
+                    description += " [{}]".format("; ".join(need_info["tags"]))
+
+                title = nodes.Text(description)
+
+                # Create a reference
+                if need_info["hide"]:
+                    para += title
+                elif need_info["is_external"]:
+                    assert (
+                        need_info["external_url"] is not None
+                    ), "External need without URL"
+                    ref = nodes.reference("", "")
+
+                    ref["refuri"] = check_and_calc_base_url_rel_path(
+                        need_info["external_url"], fromdocname
+                    )
+
+                    ref["classes"].append(need_info["external_css"])
+                    ref.append(title)
+                    para += ref
+                elif _docname := need_info["docname"]:
+                    target_id = need_info["target_id"]
+                    ref = nodes.reference("", "")
+                    ref["refdocname"] = _docname
+                    ref["refuri"] = builder.get_relative_uri(fromdocname, _docname)
+                    ref["refuri"] += "#" + target_id
+                    ref.append(title)
+                    para += ref
+                line_block.append(para)
+            content.append(line_block)
 
         if len(content) == 0:
-            content.append(no_needs_found_paragraph())
-
+            content.append(
+                no_needs_found_paragraph(current_needfilter.get("filter_warning"))
+            )
         if current_needfilter["show_filters"]:
             content.append(used_filter_paragraph(current_needfilter))
 
         node.replace_self(content)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needpie.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needpie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import hashlib
-from typing import Iterable, List, Sequence
+from typing import Any, Iterable, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.debug import measure_time
+from sphinx_needs.directives.utils import no_needs_found_paragraph
 from sphinx_needs.filter_common import FilterBase, filter_needs, prepare_need_list
 from sphinx_needs.logging import get_logger
 from sphinx_needs.utils import (
     add_doc,
     check_and_get_external_filter_func,
     import_matplotlib,
     remove_node_from_tree,
@@ -43,14 +46,15 @@
         "explode": directives.unchanged_required,
         "labels": directives.unchanged_required,
         "style": directives.unchanged_required,
         "colors": directives.unchanged_required,
         "text_color": directives.unchanged_required,
         "shadow": directives.flag,
         "filter-func": FilterBase.base_option_spec["filter-func"],
+        "filter_warning": FilterBase.base_option_spec["filter_warning"],
     }
 
     # Update the options_spec only with value filter-func defined in the FilterBase class
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
@@ -90,22 +94,31 @@
             "explode": explode,
             "style": style,
             "labels": labels,
             "colors": colors,
             "shadow": shadow,
             "text_color": text_color,
             "filter_func": self.collect_filter_attributes()["filter_func"],
+            "filter_warning": self.collect_filter_attributes()["filter_warning"],
         }
         add_doc(env, env.docname)
 
-        return [targetnode, Needpie("")]
+        pie_node = Needpie("")
+        self.set_source_info(pie_node)
+
+        return [targetnode, pie_node]
 
 
 @measure_time("needpie")
-def process_needpie(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needpie(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     env = app.env
     needs_data = SphinxNeedsData(env)
     needs_config = NeedsSphinxConfig(env.config)
 
     matplotlib = import_matplotlib()
 
     if matplotlib is None and found_nodes and needs_config.include_needs:
@@ -140,42 +153,48 @@
             matplotlib.style.use(current_needpie["style"])
         else:
             matplotlib.style.use("default")
 
         content = current_needpie["content"]
 
         sizes = []
-        need_list = list(prepare_need_list(needs_data.get_or_create_needs().values()))  # adds parts to need_list
+        need_list = list(
+            prepare_need_list(needs_data.get_or_create_needs().values())
+        )  # adds parts to need_list
         if content and not current_needpie["filter_func"]:
             for line in content:
                 if line.isdigit():
                     sizes.append(abs(float(line)))
                 else:
-                    result = len(filter_needs(need_list, needs_config, line))
+                    result = len(
+                        filter_needs(need_list, needs_config, line, location=node)
+                    )
                     sizes.append(result)
         elif current_needpie["filter_func"] and not content:
             try:
                 # check and get filter_func
-                filter_func, filter_args = check_and_get_external_filter_func(current_needpie.get("filter_func"))
+                filter_func, filter_args = check_and_get_external_filter_func(
+                    current_needpie.get("filter_func")
+                )
                 # execute filter_func code
                 # Provides only a copy of needs to avoid data manipulations.
-                context = {
+                context: dict[str, Any] = {
                     "needs": need_list,
                     "results": [],
                 }
                 args = []
                 if filter_args:
                     args = filter_args.split(",")
                 for index, arg in enumerate(args):
                     # All rgs are strings, but we must transform them to requested type, e.g. 1 -> int, "1" -> str
                     context[f"arg{index + 1}"] = arg
 
                 if filter_func:
                     filter_func(**context)
-                sizes = context["results"]  # type: ignore[assignment]
+                sizes = context["results"]
                 # check items in sizes
                 if not isinstance(sizes, list):
                     logger.error(
                         f"The returned values from the given filter_func {filter_func.__name__} is not valid."
                         " It must be a list."
                     )
                 for item in sizes:
@@ -183,15 +202,17 @@
                         logger.error(
                             f"The returned values from the given filter_func {filter_func.__name__} is not valid. "
                             "It must be a list with items of type int/float."
                         )
             except Exception as e:
                 raise e
         elif current_needpie["filter_func"] and content:
-            logger.error("filter_func and content can't be used at the same time for needpie.")
+            logger.error(
+                "filter_func and content can't be used at the same time for needpie."
+            )
         else:
             logger.error("Both filter_func and content are not used for needpie.")
 
         labels = current_needpie["labels"]
         if labels is None:
             labels = [""] * len(sizes)
 
@@ -206,29 +227,33 @@
         explode = current_needpie["explode"]
         if explode is None:
             explode = [0] * len(labels)
 
         shadow = current_needpie["shadow"]
         text_color = current_needpie["text_color"]
 
-        fig, axes = matplotlib.pyplot.subplots(figsize=(8, 4), subplot_kw={"aspect": "equal"})
+        fig, axes = matplotlib.pyplot.subplots(
+            figsize=(8, 4), subplot_kw={"aspect": "equal"}
+        )
 
         pie_kwargs = {
             "labels": labels,
             "startangle": 90,
             "explode": explode,
             "autopct": lambda pct: label_calc(pct, sizes),  # noqa: B023
             "shadow": shadow,
             "colors": colors,
         }
 
         if text_color:
             pie_kwargs["textprops"] = {"color": text_color}
 
-        wedges, _texts, autotexts = axes.pie(sizes, normalize=sum(float(s) for s in sizes) >= 1, **pie_kwargs)
+        wedges, _texts, autotexts = axes.pie(
+            sizes, normalize=sum(float(s) for s in sizes) >= 1, **pie_kwargs
+        )
 
         ratio = 20  # we will remove all labels with size smaller 5%
         legend_enforced = False
         for i in range(len(sizes)):
             # remove leading and following spaces from the labels
             labels[i] = labels[i].strip()
             if sizes[i] < (sum(sizes) / ratio) or sizes[i] == 0:
@@ -238,46 +263,57 @@
                 legend_enforced = True
 
         # We have to add the percent and absolut number to the legend,
         # as not all elements are now visible.
         if legend_enforced:
             for i in range(len(sizes)):
                 if sum(sizes) > 0:
-                    labels[i] = "{label} {percent:.1f}% ({size:.0f})".format(
-                        label=labels[i], percent=100 * sizes[i] / sum(sizes), size=sizes[i]
+                    labels[i] = (
+                        f"{labels[i]} {100 * sizes[i] / sum(sizes):.1f}% ({sizes[i]:.0f})"
                     )
                 else:
-                    labels[i] = "{label} {percent:.1f}% ({size:.0f})".format(
-                        label=labels[i], percent=0.0, size=sizes[i]
-                    )
+                    labels[i] = f"{labels[i]} {0.0:.1f}% ({sizes[i]:.0f})"
 
         if text_color:
             for autotext in autotexts:
                 autotext.set_color(text_color)
         axes.axis("equal")
 
         # Legend preparation
         if current_needpie["legend"]:
-            axes.legend(wedges, labels, title="legend", loc="center left", bbox_to_anchor=(0.8, 0, 0.5, 1))
+            axes.legend(
+                wedges,
+                labels,
+                title="legend",
+                loc="center left",
+                bbox_to_anchor=(0.8, 0, 0.5, 1),
+            )
 
         matplotlib.pyplot.setp(autotexts, size=8, weight="bold")
 
         if current_needpie["title"]:
             axes.set_title(current_needpie["title"])
 
         # Final storage
 
         # We need to calculate an unique pie-image file name
         hash_value = hashlib.sha256(id.encode()).hexdigest()[:5]
-        image_node = save_matplotlib_figure(app, fig, f"need_pie_{hash_value}", fromdocname)
+        image_node = save_matplotlib_figure(
+            app, fig, f"need_pie_{hash_value}", fromdocname
+        )
 
         # Add lineno to node
         image_node.line = current_needpie["lineno"]
 
-        node.replace_self(image_node)
+        if len(sizes) == 0 or all(s == 0 for s in sizes):
+            node.replace_self(
+                no_needs_found_paragraph(current_needpie.get("filter_warning"))
+            )
+        else:
+            node.replace_self(image_node)
 
         # Cleanup matplotlib
         # Reset the style configuration:
         matplotlib.rcParams = style_previous_to_script_execution
 
         # Close the figure, to free consumed memory.
         # Otherwise we will get: RuntimeWarning from matplotlib:
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needreport.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needreport.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,88 @@
-import os
+from __future__ import annotations
+
+from pathlib import Path
 from typing import Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from jinja2 import Template
-from sphinx.errors import SphinxError
+from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.directives.utils import analyse_needs_metrics
 from sphinx_needs.utils import add_doc
 
-
-class NeedsReportException(SphinxError):
-    pass
+LOGGER = logging.getLogger(__name__)
 
 
 class NeedReportDirective(SphinxDirective):
     final_argument_whitespace = True
     option_spec = {
-        "types": directives.unchanged,
-        "links": directives.unchanged,
-        "options": directives.unchanged,
-        "usage": directives.unchanged,
+        "types": directives.flag,
+        "links": directives.flag,
+        "options": directives.flag,
+        "usage": directives.flag,
+        "template": directives.unchanged,
     }
 
     def run(self) -> Sequence[nodes.raw]:
         env = self.env
         needs_config = NeedsSphinxConfig(env.config)
 
-        if len(self.options.keys()) == 0:  # Check if options is empty
-            error_file, error_line = self.state_machine.input_lines.items[0]
-            error_msg = "{}:{}: NeedReportError: No options specified to generate need report.".format(
-                error_file, error_line + self.state_machine.input_lines.data.index(".. needreport::") + 1
+        if not set(self.options).intersection({"types", "links", "options", "usage"}):
+            LOGGER.warning(
+                "No options specified to generate need report [needs.report]",
+                location=self.get_location(),
+                type="needs",
+                subtype="report",
             )
-            raise NeedsReportException(error_msg)
-
-        types = self.options.get("types")
-        extra_links = self.options.get("links")
-        extra_options = self.options.get("options")
-        usage = self.options.get("usage")
-
-        needs_types = []
-        needs_extra_links = []
-        needs_extra_options = []
-        needs_metrics = {}
-
-        if types is not None and isinstance(types, str):
-            needs_types = needs_config.types
-        if extra_links is not None and isinstance(extra_links, str):
-            needs_extra_links = needs_config.extra_links
-        if extra_options is not None and isinstance(extra_options, str):
-            needs_extra_options = needs_config.extra_options
-        if usage is not None and isinstance(usage, str):
-            needs_metrics = analyse_needs_metrics(env)
+            return []
 
         report_info = {
-            "types": needs_types,
-            "options": needs_extra_options,
-            "links": needs_extra_links,
-            "usage": needs_metrics,
+            "types": needs_config.types if "types" in self.options else [],
+            "options": needs_config.extra_options if "options" in self.options else [],
+            "links": needs_config.extra_links if "links" in self.options else [],
+            "usage": analyse_needs_metrics(env) if "usage" in self.options else {},
+            "report_directive": "dropdown",
         }
         report_info.update(**needs_config.render_context)
 
-        need_report_template_path: str = needs_config.report_template
-        # Absolute path starts with /, based on the conf.py directory. The / need to be striped
-        correct_need_report_template_path = os.path.join(env.app.srcdir, need_report_template_path.lstrip("/"))
-
-        if len(need_report_template_path) == 0:
-            default_template_path = "needreport_template.rst"
-            correct_need_report_template_path = os.path.join(os.path.dirname(__file__), default_template_path)
+        if "template" in self.options:
+            need_report_template_path = Path(
+                self.env.relfn2path(self.options["template"], self.env.docname)[1]
+            )
+        elif needs_config.report_template:
+            # Absolute path starts with /, based on the conf.py directory. The / need to be striped
+            need_report_template_path = Path(
+                str(env.app.srcdir)
+            ) / needs_config.report_template.lstrip("/")
+        else:
+            need_report_template_path = (
+                Path(__file__).parent / "needreport_template.rst"
+            )
 
-        if not os.path.exists(correct_need_report_template_path):
-            raise ReferenceError(f"Could not load needs report template file {correct_need_report_template_path}")
+        if not need_report_template_path.is_file():
+            LOGGER.warning(
+                f"Could not load needs report template file {need_report_template_path} [needs.report]",
+                location=self.get_location(),
+                type="needs",
+                subtype="report",
+            )
+            return []
 
-        with open(correct_need_report_template_path) as needs_report_template_file:
-            needs_report_template_file_content = needs_report_template_file.read()
+        needs_report_template_file_content = need_report_template_path.read_text(
+            encoding="utf8"
+        )
 
         template = Template(needs_report_template_file_content, autoescape=True)
-
         text = template.render(**report_info)
-        self.state_machine.insert_input(text.split("\n"), self.state_machine.document.attributes["source"])
+        self.state_machine.insert_input(
+            text.split("\n"), self.state_machine.document.attributes["source"]
+        )
 
         report_node = nodes.raw()
 
         add_doc(env, env.docname)
 
         return [report_node]
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needreport_template.rst` & `sphinx_needs-2.1.0/sphinx_needs/directives/needreport_template.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {# Output for needs_types #}
 {% if types|length != 0 %}
 
-.. dropdown:: Need Types
+.. {{ report_directive }}:: Need Types
 
    .. list-table::
       :widths: 40 20 20 20
       :header-rows: 1
 
       * - TITLE
         - DIRECTIVE
@@ -19,15 +19,15 @@
       {% endfor %}
 {% endif %}
 {# Output for needs_types #}
 
 {# Output for needs_extra_links #}
 {% if links|length != 0 %}
 
-.. dropdown:: Need Extra Links
+.. {{ report_directive }}:: Need Extra Links
 
    .. list-table::
       :widths: 10 30 30 5 20
       :header-rows: 1
 
       * - OPTION
         - INCOMING
@@ -43,26 +43,26 @@
       {% endfor %}
 {% endif %}
 {# Output for needs_extra_links #}
 
 {# Output for needs_options #}
 {% if options|length != 0 %}
 
-.. dropdown:: Need Extra Options
+.. {{ report_directive }}:: Need Extra Options
 
    {% for option in options %}
    * {{ option }}
    {% endfor %}
 {% endif %}
 {# Output for needs_options #}
 
 {# Output for needs metrics #}
 {% if usage|length != 0 %}
 
-.. dropdown:: Need Metrics
+.. {{ report_directive }}:: Need Metrics
 
    .. list-table::
       :widths: 40 40
       :header-rows: 1
 
       * - NEEDS TYPES
         - NEEDS PER TYPE
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needsequence.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needsequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import os
 import re
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinxcontrib.plantuml import (
     generate_name,  # Need for plantuml filename calculation
 )
@@ -15,14 +17,15 @@
     DiagramBase,
     add_config,
     create_legend,
     get_debug_container,
     get_filter_para,
     no_plantuml,
 )
+from sphinx_needs.directives.utils import no_needs_found_paragraph
 from sphinx_needs.filter_common import FilterBase
 from sphinx_needs.logging import get_logger
 from sphinx_needs.utils import add_doc, remove_node_from_tree
 
 logger = get_logger(__name__)
 
 
@@ -50,15 +53,16 @@
         env = self.env
 
         _, targetid, targetnode = self.create_target("needsequence")
 
         start = self.options.get("start")
         if start is None or len(start.strip()) == 0:
             raise NeedSequenceException(
-                "No valid start option given for needsequence. " "See file {}:{}".format(env.docname, self.lineno)
+                "No valid start option given for needsequence. "
+                f"See file {env.docname}:{self.lineno}"
             )
 
         # Add the needsequence and all needed information
         SphinxNeedsData(env).get_or_create_sequences()[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
             "target_id": targetid,
@@ -69,15 +73,18 @@
 
         add_doc(env, env.docname)
 
         return [targetnode] + [Needsequence("")]
 
 
 def process_needsequence(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     # Replace all needsequence nodes with a list of the collected needs.
     env = app.env
     needs_data = SphinxNeedsData(env)
     all_needs_dict = needs_data.get_or_create_needs()
 
     needs_config = NeedsSphinxConfig(env.config)
@@ -91,21 +98,25 @@
         if not include_needs:
             remove_node_from_tree(node)
             continue
 
         id = node.attributes["ids"][0]
         current_needsequence = needs_data.get_or_create_sequences()[id]
 
-        option_link_types = [link.upper() for link in current_needsequence["link_types"]]
+        option_link_types = [
+            link.upper() for link in current_needsequence["link_types"]
+        ]
         for lt in option_link_types:
             if lt not in link_type_names:
                 logger.warning(
                     "Unknown link type {link_type} in needsequence {flow}. Allowed values:"
                     " {link_types} [needs]".format(
-                        link_type=lt, flow=current_needsequence["target_id"], link_types=",".join(link_type_names)
+                        link_type=lt,
+                        flow=current_needsequence["target_id"],
+                        link_types=",".join(link_type_names),
                     ),
                     type="needs",
                 )
 
         content = []
         try:
             if "sphinxcontrib.plantuml" not in app.config.extensions:
@@ -124,15 +135,17 @@
 
         puml_node["uml"] = "@startuml\n"
 
         # Adding config
         config = current_needsequence["config"]
         puml_node["uml"] += add_config(config)
 
-        start_needs_id = [x.strip() for x in re.split(";|,", current_needsequence["start"])]
+        start_needs_id = [
+            x.strip() for x in re.split(";|,", current_needsequence["start"])
+        ]
         if len(start_needs_id) == 0:
             # TODO this should be a warning (and not tested)
             raise NeedSequenceException(
                 "No start-id set for needsequence"
                 f" docname {current_needsequence['docname']}"
                 f":{current_needsequence['lineno']}"
             )
@@ -143,17 +156,19 @@
         p_string = ""
         c_string = ""
         for need_id in start_needs_id:
             try:
                 need = all_needs_dict[need_id.strip()]
             except KeyError:
                 raise NeedSequenceException(
-                    "Given {} in needsequence unknown."
-                    " File {}"
-                    ":{}".format(need_id, current_needsequence["docname"], current_needsequence["lineno"])
+                    "Given {} in needsequence unknown." " File {}" ":{}".format(
+                        need_id,
+                        current_needsequence["docname"],
+                        current_needsequence["lineno"],
+                    )
                 )
 
             # Add children of participants
             _msg_receiver_needs, p_string_new, c_string_new = get_message_needs(
                 app,
                 need,
                 current_needsequence["link_types"],
@@ -170,15 +185,17 @@
 
         # Create a legend
         if current_needsequence["show_legend"]:
             puml_node["uml"] += create_legend(needs_types)
 
         puml_node["uml"] += "\n@enduml"
         puml_node["incdir"] = os.path.dirname(current_needsequence["docname"])
-        puml_node["filename"] = os.path.split(current_needsequence["docname"])[1]  # Needed for plantuml >= 0.9
+        puml_node["filename"] = os.path.split(current_needsequence["docname"])[
+            1
+        ]  # Needed for plantuml >= 0.9
 
         scale = int(current_needsequence["scale"])
         # if scale != 100:
         puml_node["scale"] = scale
 
         puml_node = nodes.figure("", puml_node)
 
@@ -196,78 +213,100 @@
                     file_ext = "png"
             except Exception:
                 file_ext = "png"
 
             gen_flow_link = generate_name(app, puml_node.children[0], file_ext)
             current_file_parts = fromdocname.split("/")
             subfolder_amount = len(current_file_parts) - 1
-            img_locaton = "../" * subfolder_amount + "_images/" + gen_flow_link[0].split("/")[-1]
-            flow_ref = nodes.reference("t", current_needsequence["caption"], refuri=img_locaton)
+            img_locaton = (
+                "../" * subfolder_amount + "_images/" + gen_flow_link[0].split("/")[-1]
+            )
+            flow_ref = nodes.reference(
+                "t", current_needsequence["caption"], refuri=img_locaton
+            )
             puml_node += nodes.caption("", "", flow_ref)
 
         # Add lineno to node
         puml_node.line = current_needsequence["lineno"]
 
         content.append(puml_node)
 
-        if len(content) == 0:
-            nothing_found = "No needs passed the filters"
-            para = nodes.paragraph()
-            nothing_found_node = nodes.Text(nothing_found)
-            para += nothing_found_node
-            content.append(para)
+        if (
+            len(c_string) == 0 and p_string.count("participant") == 1
+        ):  # no connections and just one (start) participant
+            content = [
+                (no_needs_found_paragraph(current_needsequence.get("filter_warning")))
+            ]
         if current_needsequence["show_filters"]:
             content.append(get_filter_para(current_needsequence))
 
         if current_needsequence["debug"]:
             content += get_debug_container(puml_node)
 
         node.replace_self(content)
 
 
 def get_message_needs(
     app: Sphinx,
     sender: NeedsInfoType,
-    link_types: List[str],
-    all_needs_dict: Dict[str, NeedsInfoType],
-    tracked_receivers: Optional[List[str]] = None,
-    filter: Optional[str] = None,
-) -> Tuple[Dict[str, Dict[str, Any]], str, str]:
-    msg_needs: List[Dict[str, Any]] = []
+    link_types: list[str],
+    all_needs_dict: dict[str, NeedsInfoType],
+    tracked_receivers: list[str] | None = None,
+    filter: str | None = None,
+) -> tuple[dict[str, dict[str, Any]], str, str]:
+    msg_needs: list[dict[str, Any]] = []
     if tracked_receivers is None:
         tracked_receivers = []
     for link_type in link_types:
         msg_needs += [all_needs_dict[x] for x in sender[link_type]]  # type: ignore
 
-    messages: Dict[str, Dict[str, Any]] = {}
+    messages: dict[str, dict[str, Any]] = {}
     p_string = ""
     c_string = ""
     for msg_need in msg_needs:
-        messages[msg_need["id"]] = {"id": msg_need["id"], "title": msg_need["title"], "receivers": {}}
+        messages[msg_need["id"]] = {
+            "id": msg_need["id"],
+            "title": msg_need["title"],
+            "receivers": {},
+        }
         if sender["id"] not in tracked_receivers:
             p_string += 'participant "{}" as {}\n'.format(sender["title"], sender["id"])
             tracked_receivers.append(sender["id"])
         for link_type in link_types:
             receiver_ids = msg_need[link_type]
             for rec_id in receiver_ids:
                 if filter:
                     from sphinx_needs.filter_common import filter_single_need
 
                     if not filter_single_need(
-                        all_needs_dict[rec_id], NeedsSphinxConfig(app.config), filter, needs=all_needs_dict.values()
+                        all_needs_dict[rec_id],
+                        NeedsSphinxConfig(app.config),
+                        filter,
+                        needs=all_needs_dict.values(),
                     ):
                         continue
 
-                rec_data = {"id": rec_id, "title": all_needs_dict[rec_id]["title"], "messages": []}
+                rec_data = {
+                    "id": rec_id,
+                    "title": all_needs_dict[rec_id]["title"],
+                    "messages": [],
+                }
 
-                c_string += "{} -> {}: {}\n".format(sender["id"], rec_data["id"], msg_need["title"])
+                c_string += "{} -> {}: {}\n".format(
+                    sender["id"], rec_data["id"], msg_need["title"]
+                )
 
                 if rec_id not in tracked_receivers:
                     rec_messages, p_string_new, c_string_new = get_message_needs(
-                        app, all_needs_dict[rec_id], link_types, all_needs_dict, tracked_receivers, filter=filter
+                        app,
+                        all_needs_dict[rec_id],
+                        link_types,
+                        all_needs_dict,
+                        tracked_receivers,
+                        filter=filter,
                     )
                     p_string += p_string_new
                     c_string += c_string_new
 
                     rec_data["messages"] = rec_messages
 
                 messages[msg_need["id"]]["receivers"][rec_id] = rec_data
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needservice.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needservice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Any, Dict, List, Sequence
+from __future__ import annotations
+
+from typing import Any, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from docutils.parsers.rst.states import RSTState, RSTStateMachine
 from docutils.statemachine import StringList
 from sphinx.util.docutils import SphinxDirective
 from sphinx_data_viewer.api import get_data_viewer_node
 
 from sphinx_needs.api import add_need
 from sphinx_needs.config import NeedsSphinxConfig
+from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.directives.need import NeedDirective
 from sphinx_needs.logging import get_logger
-from sphinx_needs.services.base import BaseService
 from sphinx_needs.utils import add_doc
 
 
 class Needservice(nodes.General, nodes.Element):
     pass
 
 
@@ -33,41 +35,51 @@
     option_spec.update(NeedDirective.option_spec)
 
     final_argument_whitespace = True
 
     def __init__(
         self,
         name: str,
-        arguments: List[str],
-        options: Dict[str, Any],
+        arguments: list[str],
+        options: dict[str, Any],
         content: StringList,
         lineno: int,
         content_offset: int,
         block_text: str,
         state: RSTState,
         state_machine: RSTStateMachine,
     ):
-        super().__init__(name, arguments, options, content, lineno, content_offset, block_text, state, state_machine)
+        super().__init__(
+            name,
+            arguments,
+            options,
+            content,
+            lineno,
+            content_offset,
+            block_text,
+            state,
+            state_machine,
+        )
         self.log = get_logger(__name__)
 
     def run(self) -> Sequence[nodes.Node]:
         docname = self.env.docname
         app = self.env.app
         needs_config = NeedsSphinxConfig(self.config)
         need_types = needs_config.types
         all_data = needs_config.service_all_data
-        needs_services: Dict[str, BaseService] = getattr(app, "needs_services", {})
+        needs_services = SphinxNeedsData(self.env).get_or_create_services()
 
         service_name = self.arguments[0]
         service = needs_services.get(service_name)
         assert service is not None
         section = []
 
         if "debug" not in self.options:
-            service_data = service.request(self.options)
+            service_data = service.request_from_directive(self)
             for datum in service_data:
                 options = {}
 
                 try:
                     content = datum["content"].split("\n")
                 except KeyError:
                     content = []
@@ -88,16 +100,20 @@
                     del datum["title"]
 
                 # We need to check if all given options from services are really available as configured
                 # extra_option or extra_link
                 missing_options = {}
                 for element in datum.keys():
                     defined_options = list(self.__class__.option_spec.keys())
-                    defined_options.append("content")  # Add content, so that it gets not detected as missing
-                    if element not in defined_options and element not in getattr(app.config, "needs_extra_links", []):
+                    defined_options.append(
+                        "content"
+                    )  # Add content, so that it gets not detected as missing
+                    if element not in defined_options and element not in getattr(
+                        app.config, "needs_extra_links", []
+                    ):
                         missing_options[element] = datum[element]
 
                 # Finally delete not found options
                 for missing_option in missing_options:
                     del datum[missing_option]
 
                 if all_data:
@@ -106,19 +122,31 @@
 
                 # content.insert(0, '.. code-block:: text\n')
                 options["content"] = "\n".join(content)
                 # Replace values in datum with calculated/checked ones.
                 datum.update(options)
 
                 # ToDo: Tags and Status are not set (but exist in data)
-                section += add_need(self.env.app, self.state, docname, self.lineno, need_type, need_title, **datum)
+                section += add_need(
+                    self.env.app,
+                    self.state,
+                    docname,
+                    self.lineno,
+                    need_type,
+                    need_title,
+                    **datum,
+                )
         else:
             try:
                 service_debug_data = service.debug(self.options)
             except NotImplementedError:
-                service_debug_data = {"error": f'Service {service_name} does not support "debug" output.'}
-            viewer_node = get_data_viewer_node(title="Debug data", data=service_debug_data)
+                service_debug_data = {
+                    "error": f'Service {service_name} does not support "debug" output.'
+                }
+            viewer_node = get_data_viewer_node(
+                title="Debug data", data=service_debug_data
+            )
             section.append(viewer_node)
 
         add_doc(self.env, self.env.docname)
 
         return section
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needtable.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needtable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import re
-from typing import Any, Callable, List, Sequence
+from typing import Any, Callable, Sequence
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 
 from sphinx_needs.api.exceptions import NeedsInvalidException
 from sphinx_needs.config import NeedsSphinxConfig
@@ -13,14 +15,15 @@
     get_option_list,
     get_title,
     no_needs_found_paragraph,
     used_filter_paragraph,
 )
 from sphinx_needs.filter_common import FilterBase, process_filters
 from sphinx_needs.functions.functions import check_and_get_content
+from sphinx_needs.roles.need_part import iter_need_parts
 from sphinx_needs.utils import add_doc, profile, remove_node_from_tree, row_col_maker
 
 
 class Needtable(nodes.General, nodes.Element):
     pass
 
 
@@ -46,15 +49,17 @@
     # Update the options_spec with values defined in the FilterBase class
     option_spec.update(FilterBase.base_option_spec)
 
     @profile("NEEDTABLE_RUN")
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
-        targetid = "needtable-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needtable"))
+        targetid = "needtable-{docname}-{id}".format(
+            docname=env.docname, id=env.new_serialno("needtable")
+        )
         targetnode = nodes.target("", "", ids=[targetid])
 
         columns_str = str(self.options.get("columns", ""))
         if len(columns_str) == 0:
             columns_str = NeedsSphinxConfig(env.app.config).table_columns
         if isinstance(columns_str, str):
             _columns = [col.strip() for col in re.split(";|,", columns_str)]
@@ -62,15 +67,17 @@
             _columns = columns_str
 
         columns = [get_title(col) for col in _columns]
 
         colwidths = str(self.options.get("colwidths", ""))
         colwidths_list = []
         if colwidths:
-            colwidths_list = [int(width.strip()) for width in re.split(";|,", colwidths)]
+            colwidths_list = [
+                int(width.strip()) for width in re.split(";|,", colwidths)
+            ]
             if len(columns) != len(colwidths_list):
                 raise NeedsInvalidException(
                     f"Amount of elements in colwidths and columns do not match: "
                     f"colwidths: {len(colwidths_list)} and columns: {len(columns)}"
                 )
 
         classes = get_option_list(self.options, "class")
@@ -109,15 +116,18 @@
 
         return [targetnode] + [Needtable("")]
 
 
 @measure_time("needtable")
 @profile("NEEDTABLE")
 def process_needtables(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     """
     Replace all needtables nodes with a table of filtered nodes.
     """
     env = app.env
     needs_config = NeedsSphinxConfig(app.config)
     needs_data = SphinxNeedsData(env)
@@ -143,15 +153,17 @@
         if not needs_config.include_needs:
             remove_node_from_tree(node)
             continue
 
         id = node.attributes["ids"][0]
         current_needtable = needs_data.get_or_create_tables()[id]
 
-        if current_needtable["style"] == "" or current_needtable["style"].upper() not in ["TABLE", "DATATABLES"]:
+        if current_needtable["style"] == "" or current_needtable[
+            "style"
+        ].upper() not in ["TABLE", "DATATABLES"]:
             if needs_config.table_style == "":
                 style = "DATATABLES"
             else:
                 style = needs_config.table_style.upper()
         else:
             style = current_needtable["style"].upper()
 
@@ -193,15 +205,17 @@
         table_node += tgroup
 
         # Add lineno to node
         table_node.line = current_needtable["lineno"]
 
         # Perform filtering of needs
         try:
-            filtered_needs = process_filters(app, list(all_needs.values()), current_needtable)
+            filtered_needs = process_filters(
+                app, list(all_needs.values()), current_needtable
+            )
         except Exception as e:
             raise e
 
         def get_sorter(key: str) -> Callable[[NeedsInfoType], Any]:
             """
             Returns a sort-function for a given need-key.
             :param key: key of need object as string
@@ -222,62 +236,79 @@
                 return value
 
             return sort
 
         filtered_needs.sort(key=get_sorter(current_needtable["sort"]))
 
         for need_info in filtered_needs:
-            style_row = check_and_get_content(current_needtable["style_row"], need_info, env)
-            style_row = style_row.replace(" ", "_")  # Replace whitespaces with _ to get valid css name
+            style_row = check_and_get_content(
+                current_needtable["style_row"], need_info, env
+            )
+            style_row = style_row.replace(
+                " ", "_"
+            )  # Replace whitespaces with _ to get valid css name
 
             temp_need = need_info.copy()
             if temp_need["is_need"]:
                 row = nodes.row(classes=["need", style_row])
                 prefix = ""
             else:
                 row = nodes.row(classes=["need_part", style_row])
                 temp_need["id"] = temp_need["id_complete"]
                 prefix = needs_config.part_prefix
                 temp_need["title"] = temp_need["content"]
 
             for option, _title in current_needtable["columns"]:
                 if option == "ID":
-                    row += row_col_maker(app, fromdocname, all_needs, temp_need, "id", make_ref=True, prefix=prefix)
+                    row += row_col_maker(
+                        app,
+                        fromdocname,
+                        all_needs,
+                        temp_need,
+                        "id",
+                        make_ref=True,
+                        prefix=prefix,
+                    )
                 elif option == "TITLE":
-                    row += row_col_maker(app, fromdocname, all_needs, temp_need, "title", prefix=prefix)
+                    row += row_col_maker(
+                        app, fromdocname, all_needs, temp_need, "title", prefix=prefix
+                    )
                 elif option in link_type_list:
                     link_type = link_type_list[option]
-                    if option in ["INCOMING", link_type["option"].upper() + "_BACK", link_type["incoming"].upper()]:
+                    if option in [
+                        "INCOMING",
+                        link_type["option"].upper() + "_BACK",
+                        link_type["incoming"].upper(),
+                    ]:
                         row += row_col_maker(
                             app,
                             fromdocname,
                             all_needs,
                             temp_need,
                             link_type["option"] + "_back",
                             ref_lookup=True,
                         )
                     else:
                         row += row_col_maker(
-                            app, fromdocname, all_needs, temp_need, link_type["option"], ref_lookup=True
+                            app,
+                            fromdocname,
+                            all_needs,
+                            temp_need,
+                            link_type["option"],
+                            ref_lookup=True,
                         )
                 else:
-                    row += row_col_maker(app, fromdocname, all_needs, temp_need, option.lower())
+                    row += row_col_maker(
+                        app, fromdocname, all_needs, temp_need, option.lower()
+                    )
             tbody += row
 
             # Need part rows
             if current_needtable["show_parts"] and need_info["is_need"]:
-                for part in need_info["parts"].values():
-                    # update the part with all information from its parent
-                    # this is required to make ID links work
-                    # The dict has to be manipulated, so that row_col_maker() can be used
-                    temp_part: NeedsInfoType = {**need_info, **part.copy()}  # type: ignore[typeddict-unknown-key]
-                    temp_part["id_complete"] = f"{need_info['id']}.{temp_part['id']}"  # type: ignore[typeddict-unknown-key]
-                    temp_part["id_parent"] = need_info["id"]  # type: ignore[typeddict-unknown-key]
-                    temp_part["docname"] = need_info["docname"]
-
+                for temp_part in iter_need_parts(need_info):
                     row = nodes.row(classes=["need_part"])
 
                     for option, _title in current_needtable["columns"]:
                         if option == "ID":
                             row += row_col_maker(
                                 app,
                                 fromdocname,
@@ -309,31 +340,34 @@
                                 fromdocname,
                                 all_needs,
                                 temp_part,
                                 link_type_list[option]["option"] + "_back",
                                 ref_lookup=True,
                             )
                         else:
-                            row += row_col_maker(app, fromdocname, all_needs, temp_part, option.lower())
+                            row += row_col_maker(
+                                app, fromdocname, all_needs, temp_part, option.lower()
+                            )
 
                     tbody += row
 
+        content: nodes.Element
         if len(filtered_needs) == 0:
-            table_node.append(no_needs_found_paragraph())
-
+            content = no_needs_found_paragraph(current_needtable.get("filter_warning"))
+        else:
+            # Put the table in a div-wrapper, so that we can control overflow / scroll layout
+            if style == "TABLE":
+                table_wrapper = nodes.container(classes=["needstable_wrapper"])
+                table_wrapper.insert(0, table_node)
+                content = table_wrapper
+            else:
+                content = table_node
         # add filter information to output
         if current_needtable["show_filters"]:
             table_node.append(used_filter_paragraph(current_needtable))
 
         if current_needtable["caption"]:
             title_text = current_needtable["caption"]
-            title = nodes.title(title_text, "", nodes.Text(title_text))
-            table_node.insert(0, title)
-
-        # Put the table in a div-wrapper, so that we can control overflow / scroll layout
-        if style == "TABLE":
-            table_wrapper = nodes.container(classes=["needstable_wrapper"])
-            table_wrapper.insert(0, table_node)
-            node.replace_self(table_wrapper)
+            title_node = nodes.title(title_text, "", nodes.Text(title_text))
+            table_node.insert(0, title_node)
 
-        else:
-            node.replace_self(table_node)
+        node.replace_self(content)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/needuml.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/needuml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+from __future__ import annotations
+
 import html
 import os
-from typing import List, Sequence
+from typing import TYPE_CHECKING, Any, Dict, List, Sequence, TypedDict
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from jinja2 import BaseLoader, Environment, Template
 from sphinx.application import Sphinx
 from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.config import NeedsSphinxConfig
-from sphinx_needs.data import SphinxNeedsData
+from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.debug import measure_time
 from sphinx_needs.diagrams_common import calculate_link
 from sphinx_needs.directives.needflow import make_entity_name
 from sphinx_needs.filter_common import filter_needs
 from sphinx_needs.utils import add_doc
 
+if TYPE_CHECKING:
+    from sphinxcontrib.plantuml import plantuml
+
+
+class ProcessedDataType(TypedDict):
+    art: str
+    key: None | str
+    arguments: dict[str, Any]
+
+
+ProcessedNeedsType = Dict[str, List[ProcessedDataType]]
+
 
 class Needuml(nodes.General, nodes.Element):
     pass
 
 
 class NeedumlDirective(SphinxDirective):
     """
@@ -39,18 +53,22 @@
         "save": directives.unchanged_required,
     }
 
     def run(self) -> Sequence[nodes.Node]:
         env = self.env
 
         if self.name == "needarch":
-            targetid = "needarch-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needarch"))
+            targetid = "needarch-{docname}-{id}".format(
+                docname=env.docname, id=env.new_serialno("needarch")
+            )
             is_arch = True
         else:
-            targetid = "needuml-{docname}-{id}".format(docname=env.docname, id=env.new_serialno("needuml"))
+            targetid = "needuml-{docname}-{id}".format(
+                docname=env.docname, id=env.new_serialno("needuml")
+            )
             is_arch = False
 
         targetnode = nodes.target("", "", ids=[targetid])
 
         scale = self.options.get("scale", "").replace("%", "")
         align = self.options.get("align", "center")
 
@@ -81,15 +99,17 @@
         if key_name == "diagram":
             raise NeedumlException(f"Needuml option key name can't be: {key_name}")
 
         save_path = self.options.get("save")
         plantuml_code_out_path = None
         if save_path:
             if os.path.isabs(save_path):
-                raise NeedumlException(f"Given save path: {save_path}, is not a relative path.")
+                raise NeedumlException(
+                    f"Given save path: {save_path}, is not a relative path."
+                )
             else:
                 plantuml_code_out_path = save_path
 
         SphinxNeedsData(env).get_or_create_umls()[targetid] = {
             "docname": env.docname,
             "lineno": self.lineno,
             "target_id": targetid,
@@ -117,15 +137,22 @@
     Directive inherits from Needuml, but works only inside a need object.
     """
 
     def run(self) -> Sequence[nodes.Node]:
         return NeedumlDirective.run(self)
 
 
-def transform_uml_to_plantuml_node(app, uml_content: str, parent_need_id: str, key: str, kwargs: dict, config: str):
+def transform_uml_to_plantuml_node(
+    app: Sphinx,
+    uml_content: str,
+    parent_need_id: None | str,
+    key: None | str,
+    kwargs: dict[str, Any],
+    config: str,
+) -> plantuml:
     try:
         if "sphinxcontrib.plantuml" not in app.config.extensions:
             raise ImportError
         from sphinxcontrib.plantuml import plantuml
     except ImportError:
         error_node = nodes.error()
         para = nodes.paragraph()
@@ -144,60 +171,67 @@
     # Adding config
     if config:
         puml_node["uml"] += "\n' Config\n\n"
         puml_node["uml"] += config
         puml_node["uml"] += "\n\n"
 
     # jinja2uml to translate jinja statements to uml text
-    (uml_content_return, processed_need_ids_return) = jinja2uml(
+    (uml_content_return, _) = jinja2uml(
         app=app,
         fromdocname=None,
         uml_content=uml_content,
         parent_need_id=parent_need_id,
         key=key,
         processed_need_ids={},
         kwargs=kwargs,
     )
-    # silently discard processed_need_ids_return
 
     puml_node["uml"] += f"\n{uml_content_return}"
     puml_node["uml"] += "\n@enduml\n"
     return puml_node
 
 
-def get_debug_node_from_puml_node(puml_node):
+def get_debug_node_from_puml_node(puml_node: plantuml) -> nodes.container:
     if isinstance(puml_node, nodes.figure):
-        data = puml_node.children[0]["uml"]
+        data = puml_node.children[0]["uml"]  # type: ignore[index]
     data = puml_node.get("uml", "")
     data = "\n".join([html.escape(line) for line in data.split("\n")])
     debug_para = nodes.raw("", f"<pre>{data}</pre>", format="html")
     debug_container = nodes.container()
     debug_container += debug_para
     return debug_container
 
 
 def jinja2uml(
-    app, fromdocname, uml_content: str, parent_need_id: str, key: str, processed_need_ids: {}, kwargs: dict
-) -> (str, {}):
+    app: Sphinx,
+    fromdocname: None | str,
+    uml_content: str,
+    parent_need_id: None | str,
+    key: None | str,
+    processed_need_ids: ProcessedNeedsType,
+    kwargs: dict[str, Any],
+) -> tuple[str, ProcessedNeedsType]:
     # Let's render jinja templates with uml content template to 'plantuml syntax' uml
     # 1. Remove @startuml and @enduml
     uml_content = uml_content.replace("@startuml", "").replace("@enduml", "")
 
     # 2. Prepare jinja template
-    mem_template = Environment(loader=BaseLoader).from_string(uml_content)
+    mem_template = Environment(loader=BaseLoader()).from_string(uml_content)
 
     # 3. Get a new instance of Jinja Helper Functions
     jinja_utils = JinjaFunctions(app, fromdocname, parent_need_id, processed_need_ids)
 
     # 4. Append need_id to processed_need_ids, so it will not been processed again
     if parent_need_id:
-        jinja_utils.append_need_to_processed_needs(need_id=parent_need_id, art="uml", key=key, kwargs=kwargs)
+        jinja_utils.append_need_to_processed_needs(
+            need_id=parent_need_id, art="uml", key=key, kwargs=kwargs
+        )
 
     # 5. Get data for the jinja processing
-    data = {}
+    data: dict[str, Any] = {}
     # 5.1 Set default config to data
     data.update(**NeedsSphinxConfig(app.config).render_context)
     # 5.2 Set uml() kwargs to data and maybe overwrite default settings
     data.update(kwargs)
     # 5.3 Make the helpers available during rendering and overwrite maybe wrongly default and uml() kwargs settings
     data.update(
         {
@@ -223,67 +257,91 @@
 class JinjaFunctions:
     """
     Contains Jinja helper functions
 
     Provides access to sphinx-app and all Needs objects.
     """
 
-    def __init__(self, app: Sphinx, fromdocname, parent_need_id: str, processed_need_ids: dict):
+    def __init__(
+        self,
+        app: Sphinx,
+        fromdocname: None | str,
+        parent_need_id: None | str,
+        processed_need_ids: ProcessedNeedsType,
+    ) -> None:
         self.needs = SphinxNeedsData(app.env).get_or_create_needs()
         self.app = app
         self.fromdocname = fromdocname
         self.parent_need_id = parent_need_id
         if parent_need_id and parent_need_id not in self.needs:
-            raise NeedumlException(f"JinjaFunctions initialized with undefined parent_need_id: '{parent_need_id}'")
+            raise NeedumlException(
+                f"JinjaFunctions initialized with undefined parent_need_id: '{parent_need_id}'"
+            )
         self.processed_need_ids = processed_need_ids
 
-    def need_to_processed_data(self, art: str, key: str, kwargs: dict) -> {}:
-        d = {
+    def need_to_processed_data(
+        self, art: str, key: None | str, kwargs: dict[str, Any]
+    ) -> ProcessedDataType:
+        d: ProcessedDataType = {
             "art": art,
             "key": key,
             "arguments": kwargs,
         }
         return d
 
-    def append_need_to_processed_needs(self, need_id: str, art: str, key: str, kwargs: dict) -> None:
+    def append_need_to_processed_needs(
+        self, need_id: str, art: str, key: None | str, kwargs: dict[str, Any]
+    ) -> None:
         data = self.need_to_processed_data(art=art, key=key, kwargs=kwargs)
         if need_id not in self.processed_need_ids:
             self.processed_need_ids[need_id] = []
         if data not in self.processed_need_ids[need_id]:
             self.processed_need_ids[need_id].append(data)
 
-    def append_needs_to_processed_needs(self, processed_needs_data: dict) -> None:
+    def append_needs_to_processed_needs(
+        self, processed_needs_data: ProcessedNeedsType
+    ) -> None:
         for k, v in processed_needs_data.items():
             if k not in self.processed_need_ids:
                 self.processed_need_ids[k] = []
             for d in v:
                 if d not in self.processed_need_ids[k]:
                     self.processed_need_ids[k].append(d)
 
-    def data_in_processed_data(self, need_id: str, art: str, key: str, kwargs: dict) -> bool:
+    def data_in_processed_data(
+        self, need_id: str, art: str, key: str, kwargs: dict[str, Any]
+    ) -> bool:
         data = self.need_to_processed_data(art=art, key=key, kwargs=kwargs)
-        return (need_id in self.processed_need_ids) and (data in self.processed_need_ids[need_id])
+        return (need_id in self.processed_need_ids) and (
+            data in self.processed_need_ids[need_id]
+        )
 
-    def get_processed_need_ids(self) -> {}:
+    def get_processed_need_ids(self) -> ProcessedNeedsType:
         return self.processed_need_ids
 
-    def uml_from_need(self, need_id: str, key: str = "diagram", **kwargs) -> str:
+    def uml_from_need(self, need_id: str, key: str = "diagram", **kwargs: Any) -> str:
         if need_id not in self.needs:
-            raise NeedumlException(f"Jinja function uml() is called with undefined need_id: '{need_id}'.")
-
-        if self.data_in_processed_data(need_id=need_id, art="uml", key=key, kwargs=kwargs):
+            raise NeedumlException(
+                f"Jinja function uml() is called with undefined need_id: '{need_id}'."
+            )
+
+        if self.data_in_processed_data(
+            need_id=need_id, art="uml", key=key, kwargs=kwargs
+        ):
             return ""
 
         need_info = self.needs[need_id]
 
         if key != "diagram":
             if need_info["arch"][key]:
                 uml_content = need_info["arch"][key]
             else:
-                raise NeedumlException(f"Option key name: {key} does not exist in need {need_id}.")
+                raise NeedumlException(
+                    f"Option key name: {key} does not exist in need {need_id}."
+                )
         else:
             if "diagram" in need_info["arch"] and need_info["arch"]["diagram"]:
                 uml_content = need_info["arch"]["diagram"]
             else:
                 return self.flow(need_id)
 
         # We need to re-render the fetched content, as it may contain also Jinja statements.
@@ -299,23 +357,27 @@
         )
 
         # Append processed needs to current proccessing
         self.append_needs_to_processed_needs(processed_need_ids_return)
 
         return uml
 
-    def flow(self, need_id) -> str:
+    def flow(self, need_id: str) -> str:
         if need_id not in self.needs:
-            raise NeedumlException(f"Jinja function flow is called with undefined need_id: '{need_id}'.")
+            raise NeedumlException(
+                f"Jinja function flow is called with undefined need_id: '{need_id}'."
+            )
 
         if self.data_in_processed_data(need_id=need_id, art="flow", key="", kwargs={}):
             return ""
 
         # append need_id to processed_need_ids, so it will not been processed again
-        self.append_need_to_processed_needs(need_id=need_id, art="flow", key="", kwargs={})
+        self.append_need_to_processed_needs(
+            need_id=need_id, art="flow", key="", kwargs={}
+        )
 
         need_info = self.needs[need_id]
         link = calculate_link(self.app, need_info, self.fromdocname)
 
         needs_config = NeedsSphinxConfig(self.app.config)
         diagram_template = Template(needs_config.diagram_template)
         node_text = diagram_template.render(**need_info, **needs_config.render_context)
@@ -326,61 +388,79 @@
             link=link,
             color=need_info["type_color"].replace("#", ""),
             style=need_info["type_style"],
         )
 
         return need_uml
 
-    def ref(self, need_id: str, option: str = None, text: str = None) -> str:
+    def ref(
+        self, need_id: str, option: None | str = None, text: None | str = None
+    ) -> str:
         if need_id not in self.needs:
-            raise NeedumlException(f"Jinja function ref is called with undefined need_id: '{need_id}'.")
+            raise NeedumlException(
+                f"Jinja function ref is called with undefined need_id: '{need_id}'."
+            )
         if (option and text) and (not option and not text):
-            raise NeedumlException("Jinja function ref requires exactly one entry 'option' or 'text'")
+            raise NeedumlException(
+                "Jinja function ref requires exactly one entry 'option' or 'text'"
+            )
 
         need_info = self.needs[need_id]
         link = calculate_link(self.app, need_info, self.fromdocname)
 
         need_uml = " [[{link} {content}]]".format(
             link=link,
             content=need_info.get(option, "") if option else text,
         )
 
         return need_uml
 
-    def filter(self, filter_string):
+    def filter(self, filter_string: str) -> list[NeedsInfoType]:
         """
         Return a list of found needs that pass the given filter string.
         """
         needs_config = NeedsSphinxConfig(self.app.config)
 
-        return filter_needs(list(self.needs.values()), needs_config, filter_string=filter_string)
+        return filter_needs(
+            list(self.needs.values()), needs_config, filter_string=filter_string
+        )
 
-    def imports(self, *args):
+    def imports(self, *args: str) -> str:
         if not self.parent_need_id:
-            raise NeedumlException("Jinja function 'import()' is not supported in needuml directive.")
+            raise NeedumlException(
+                "Jinja function 'import()' is not supported in needuml directive."
+            )
         # gets all need ids from need links/extra_links options and wrap into jinja function uml()
         need_info = self.needs[self.parent_need_id]
         uml_ids = []
         for option_name in args:
             # check if link option_name exists in current need object
-            if option_name in need_info and need_info[option_name]:
-                for id in need_info[option_name]:
+            if option_value := need_info.get(option_name):
+                try:
+                    iterable_value = list(option_value)  # type: ignore
+                except TypeError:
+                    raise NeedumlException(
+                        f"Option value for {option_name!r} is not iterable."
+                    )
+                for id in iterable_value:
                     uml_ids.append(id)
         umls = ""
         if uml_ids:
             for uml_id in uml_ids:
                 local_uml_from_need = self.uml_from_need(uml_id)
                 if not local_uml_from_need.endswith("\n"):
                     local_uml_from_need += "\n"
                 umls += local_uml_from_need
         return umls
 
-    def need(self):
+    def need(self) -> NeedsInfoType:
         if not self.parent_need_id:
-            raise NeedumlException("Jinja function 'need()' is not supported in needuml directive.")
+            raise NeedumlException(
+                "Jinja function 'need()' is not supported in needuml directive."
+            )
         return self.needs[self.parent_need_id]
 
 
 def is_element_of_need(node: nodes.Element) -> str:
     """
     Checks if a node is part of a need in the doctree.
 
@@ -401,36 +481,45 @@
                 break
             node = node.parent
 
     return is_element_of
 
 
 @measure_time("needuml")
-def process_needuml(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_needuml(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     env = app.env
 
     # for node in doctree.findall(Needuml):
     for node in found_nodes:
         id = node.attributes["ids"][0]
         current_needuml = SphinxNeedsData(env).get_or_create_umls()[id]
 
         parent_need_id = None
         # Check if current needuml is needarch
         if current_needuml["is_arch"]:
             # Check if needarch is only used inside a need
             parent_need_id = is_element_of_need(node)
             if not parent_need_id:
-                raise NeedArchException("Directive needarch can only be used inside a need.")
+                raise NeedArchException(
+                    "Directive needarch can only be used inside a need."
+                )
         content = []
 
         # Adding config
         config = current_needuml["config"]
         if config and len(config) >= 3:
             # Remove all empty lines
-            config = "\n".join([line.strip() for line in config.split("\n") if line.strip()])
+            config = "\n".join(
+                [line.strip() for line in config.split("\n") if line.strip()]
+            )
 
         puml_node = transform_uml_to_plantuml_node(
             app=app,
             uml_content=current_needuml["content"],
             parent_need_id=parent_need_id,
             key=current_needuml["key"],
             kwargs=current_needuml["extra"],
@@ -453,15 +542,17 @@
 
         if current_needuml["align"]:
             puml_node["align"] = current_needuml["align"]
         else:
             puml_node["align"] = "center"
 
         puml_node["incdir"] = os.path.dirname(current_needuml["docname"])
-        puml_node["filename"] = os.path.split(current_needuml["docname"])[1]  # Needed for plantuml >= 0.9
+        puml_node["filename"] = os.path.split(current_needuml["docname"])[
+            1
+        ]  # Needed for plantuml >= 0.9
 
         content.append(puml_node)
 
         if current_needuml["caption"]:
             title_text = current_needuml["caption"]
             title = nodes.title(title_text, "", nodes.Text(title_text))
             content.insert(0, title)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/directives/utils.py` & `sphinx_needs-2.1.0/sphinx_needs/directives/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,60 @@
+from __future__ import annotations
+
 import re
-from typing import Any, Dict, List, Tuple
+from typing import Any
 
 from docutils import nodes
 from sphinx.environment import BuildEnvironment
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import NeedsFilteredBaseType, SphinxNeedsData
 from sphinx_needs.defaults import TITLE_REGEX
 
 
-def no_needs_found_paragraph() -> nodes.paragraph:
-    nothing_found = "No needs passed the filters"
+def no_needs_found_paragraph(message: str | None) -> nodes.paragraph:
+    nothing_found = "No needs passed the filters" if message is None else message
     para = nodes.paragraph()
+    para["classes"].append("needs_filter_warning")
     nothing_found_node = nodes.Text(nothing_found)
     para += nothing_found_node
     return para
 
 
 def used_filter_paragraph(current_needfilter: NeedsFilteredBaseType) -> nodes.paragraph:
     para = nodes.paragraph()
     filter_text = "Used filter:"
     filter_text += (
-        " status(%s)" % " OR ".join(current_needfilter["status"]) if len(current_needfilter["status"]) > 0 else ""
+        " status({})".format(" OR ".join(current_needfilter["status"]))
+        if len(current_needfilter["status"]) > 0
+        else ""
     )
     if len(current_needfilter["status"]) > 0 and len(current_needfilter["tags"]) > 0:
         filter_text += " AND "
-    filter_text += " tags(%s)" % " OR ".join(current_needfilter["tags"]) if len(current_needfilter["tags"]) > 0 else ""
-    if (len(current_needfilter["status"]) > 0 or len(current_needfilter["tags"]) > 0) and len(
-        current_needfilter["types"]
-    ) > 0:
+    filter_text += (
+        " tags({})".format(" OR ".join(current_needfilter["tags"]))
+        if len(current_needfilter["tags"]) > 0
+        else ""
+    )
+    if (
+        len(current_needfilter["status"]) > 0 or len(current_needfilter["tags"]) > 0
+    ) and len(current_needfilter["types"]) > 0:
         filter_text += " AND "
     filter_text += (
-        " types(%s)" % " OR ".join(current_needfilter["types"]) if len(current_needfilter["types"]) > 0 else ""
+        " types({})".format(" OR ".join(current_needfilter["types"]))
+        if len(current_needfilter["types"]) > 0
+        else ""
     )
 
     filter_node = nodes.emphasis(filter_text, filter_text)
     para += filter_node
     return para
 
 
-def get_title(option_string: str) -> Tuple[str, str]:
+def get_title(option_string: str) -> tuple[str, str]:
     """
     Returns a tuple of uppercase option and calculated title of given option string.
 
     :param option_string:
     :return: string
     """
     if option_string.upper() == "ID":
@@ -54,43 +65,45 @@
 
     option_name = match.group(1)
     title = match.group(2)
 
     return option_name.upper(), title
 
 
-def get_option_list(options: Dict[str, Any], name: str) -> List[str]:
+def get_option_list(options: dict[str, Any], name: str) -> list[str]:
     """
     Gets and creates a list of a given directive option value in a safe way
     :param options: List of options
     :param name: Name of the option
     :return: List with strings
     """
     values = str(options.get(name, ""))
     values_list = []
     if isinstance(values, str):
         values_list = [value.strip() for value in re.split("[;,]", values)]
 
     return values_list
 
 
-def analyse_needs_metrics(env: BuildEnvironment) -> Dict[str, Any]:
+def analyse_needs_metrics(env: BuildEnvironment) -> dict[str, Any]:
     """
     Function to generate metrics about need objects.
 
     :param env: Sphinx build environment
     :return: Dictionary consisting of needs metrics.
     """
     needs = SphinxNeedsData(env).get_or_create_needs()
-    metric_data: Dict[str, Any] = {"needs_amount": len(needs)}
+    metric_data: dict[str, Any] = {"needs_amount": len(needs)}
     needs_types = {i["directive"]: 0 for i in NeedsSphinxConfig(env.config).types}
 
     for i in needs.values():
         if i["type"] in needs_types:
             needs_types[i["type"]] += 1
 
-    metric_data["needs_types"] = {i[0]: i[1] for i in sorted(needs_types.items(), key=lambda x: x[0])}
+    metric_data["needs_types"] = {
+        i[0]: i[1] for i in sorted(needs_types.items(), key=lambda x: x[0])
+    }
     return metric_data
 
 
 class SphinxNeedsLinkTypeException(BaseException):
     """Raised if problems with link types happen"""
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/environment.py` & `sphinx_needs-2.1.0/sphinx_needs/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 from pathlib import Path, PurePosixPath
-from typing import Iterable, List
+from typing import Iterable
 
 from jinja2 import Environment, PackageLoader, select_autoescape
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx.util.console import brown  # type: ignore[attr-defined]
 from sphinx.util.osutil import copyfile
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.utils import logger
 
 try:
-    from sphinx.util.display import status_iterator  # type: ignore
+    from sphinx.util.display import status_iterator
 except ImportError:
     # will be removed in Sphinx 8.0
-    from sphinx.util import status_iterator
+    from sphinx.util import status_iterator  # type: ignore
 
 IMAGE_DIR_NAME = "_static"
 
 
 def safe_add_file(filename: Path, app: Sphinx) -> None:
     """
     Adds files to builder resources only, if the given filename was not already
@@ -34,21 +36,29 @@
     builder = app.builder
     # Use PurePosixPath, so that the path can be used as "web"-path
     pure_path = PurePosixPath(filename)
     static_data_file = PurePosixPath("_static") / pure_path
 
     if pure_path.suffix == ".js":
         # Make sure the calculated (posix)-path is not already registered as "web"-path
-        if hasattr(builder, "script_files") and str(static_data_file) not in builder.script_files:
+        if (
+            hasattr(builder, "script_files")
+            and str(static_data_file) not in builder.script_files
+        ):
             app.add_js_file(str(pure_path))
     elif pure_path.suffix == ".css":
-        if hasattr(builder, "css_files") and str(static_data_file) not in builder.css_files:
+        if (
+            hasattr(builder, "css_files")
+            and str(static_data_file) not in builder.css_files
+        ):
             app.add_css_file(str(pure_path))
     else:
-        raise NotImplementedError(f"File type {pure_path.suffix} not support by save_add_file")
+        raise NotImplementedError(
+            f"File type {pure_path.suffix} not support by save_add_file"
+        )
 
 
 def safe_remove_file(filename: Path, app: Sphinx) -> None:
     """
     Removes a given resource file from builder resources.
 
     Needed mostly during test, if multiple sphinx-build are started. During these tests
@@ -114,30 +124,33 @@
         source_file_path = Path(source_file_path)
 
         if not source_file_path.is_absolute():
             source_file_path = css_root / source_file_path
 
         if not source_file_path.exists():
             source_file_path = css_root / "blank" / "blank.css"
-            logger.warning(f"{source_file_path} not found. Copying sphinx-internal blank.css [needs]", type="needs")
+            logger.warning(
+                f"{source_file_path} not found. Copying sphinx-internal blank.css [needs]",
+                type="needs",
+            )
 
         dest_file = dest_dir / source_file_path.name
         dest_dir.mkdir(exist_ok=True)
 
         copyfile(str(source_file_path), str(dest_file))
 
         relative_path = Path(dest_file).relative_to(statics_dir)
         safe_add_file(relative_path, app)
 
 
 def install_static_files(
     app: Sphinx,
     source_dir: Path,
     destination_dir: Path,
-    files_to_copy: List[Path],
+    files_to_copy: list[Path],
     message: str,
 ) -> None:
     builder = app.builder
     # Do not copy static_files for our "needs" builder
     if builder.name == "needs":
         return
 
@@ -209,15 +222,17 @@
     """
     builder = app.builder
     # Do not copy static_files for our "needs" builder
     if builder.name == "needs":
         return
 
     # load jinja template
-    jinja_env = Environment(loader=PackageLoader("sphinx_needs"), autoescape=select_autoescape())
+    jinja_env = Environment(
+        loader=PackageLoader("sphinx_needs"), autoescape=select_autoescape()
+    )
     template = jinja_env.get_template("permalink.html")
 
     # save file to build dir
     sphinx_config = NeedsSphinxConfig(env.config)
     out_file = Path(builder.outdir) / Path(sphinx_config.permalink_file).name
     with open(out_file, "w", encoding="utf-8") as f:
         f.write(
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/external_needs.py` & `sphinx_needs-2.1.0/sphinx_needs/external_needs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import os
 from functools import lru_cache
 
 import requests
 from jinja2 import Environment, Template
 from requests_file import FileAdapter
@@ -25,14 +27,15 @@
     Can be cached, as the template is always the same for a given target_url
     """
     mem_template = Environment().from_string(target_url)
     return mem_template
 
 
 def load_external_needs(app: Sphinx, env: BuildEnvironment, _docname: str) -> None:
+    """Load needs from configured external sources."""
     needs_config = NeedsSphinxConfig(app.config)
     for source in needs_config.external_needs:
         if source["base_url"].endswith("/"):
             source["base_url"] = source["base_url"][:-1]
 
         target_url = source.get("target_url", "")
 
@@ -41,88 +44,111 @@
                 clean_log(
                     "json_path and json_url are both configured, but only one is allowed.\n"
                     f"json_path: {source['json_path']}\n"
                     f"json_url: {source['json_url']}."
                 )
             )
         elif not (source.get("json_url", False) or source.get("json_path", False)):
-            raise NeedsExternalException("json_path or json_url must be configured to use external_needs.")
+            raise NeedsExternalException(
+                "json_path or json_url must be configured to use external_needs."
+            )
 
         if source.get("json_url", False):
-            log.info(clean_log(f"Loading external needs from url {source['json_url']}."))
+            log.info(
+                clean_log(f"Loading external needs from url {source['json_url']}.")
+            )
             s = requests.Session()
             s.mount("file://", FileAdapter())
             try:
                 response = s.get(source["json_url"])
-                needs_json = response.json()  # The downloaded file MUST be json. Everything else we do not handle!
+                needs_json = (
+                    response.json()
+                )  # The downloaded file MUST be json. Everything else we do not handle!
             except Exception as e:
                 raise NeedsExternalException(
-                    clean_log("Getting {} didn't work. Reason: {}".format(source["json_url"], e))
+                    clean_log(
+                        "Getting {} didn't work. Reason: {}".format(
+                            source["json_url"], e
+                        )
+                    )
                 )
 
         if source.get("json_path", False):
             if os.path.isabs(source["json_path"]):
                 json_path = source["json_path"]
             else:
                 json_path = os.path.join(app.srcdir, source["json_path"])
 
             if not os.path.exists(json_path):
-                raise NeedsExternalException(f"Given json_path {json_path} does not exist.")
+                raise NeedsExternalException(
+                    f"Given json_path {json_path} does not exist."
+                )
 
             with open(json_path) as json_file:
                 needs_json = json.load(json_file)
 
         version = source.get("version", needs_json.get("current_version"))
         if not version:
             raise NeedsExternalException(
                 'No version defined in "needs_external_needs" or by "current_version" from loaded json file'
             )
 
         try:
             needs = needs_json["versions"][version]["needs"]
         except KeyError:
             raise NeedsExternalException(
-                clean_log(f"Version {version} not found in json file from {source['json_url']}")
+                clean_log(
+                    f"Version {version} not found in json file from {source['json_url']}"
+                )
             )
 
         log.debug(f"Loading {len(needs)} needs.")
 
         prefix = source.get("id_prefix", "").upper()
         import_prefix_link_edit(needs, prefix, needs_config.extra_links)
         for need in needs.values():
             need_params = {**need}
 
             extra_links = [x["option"] for x in needs_config.extra_links]
             for key in list(need_params.keys()):
                 if (
                     key not in needs_config.extra_options
                     and key not in extra_links
-                    and key not in ["title", "type", "id", "description", "tags", "docname", "status"]
+                    and key
+                    not in [
+                        "title",
+                        "type",
+                        "id",
+                        "description",
+                        "tags",
+                        "docname",
+                        "status",
+                    ]
                 ):
                     del need_params[key]
 
             need_params["need_type"] = need["type"]
             need_params["id"] = f'{prefix}{need["id"]}'
             need_params["external_css"] = source.get("css_class")
 
             if target_url:
                 # render jinja content
                 mem_template = get_target_template(target_url)
                 cal_target_url = mem_template.render(**{"need": need})
                 need_params["external_url"] = f'{source["base_url"]}/{cal_target_url}'
             else:
-                need_params[
-                    "external_url"
-                ] = f'{source["base_url"]}/{need.get("docname", "__error__")}.html#{need["id"]}'
+                need_params["external_url"] = (
+                    f'{source["base_url"]}/{need.get("docname", "__error__")}.html#{need["id"]}'
+                )
 
             need_params["content"] = need["description"]
             need_params["links"] = need.get("links", [])
             need_params["tags"] = ",".join(need.get("tags", []))
             need_params["status"] = need.get("status")
-            need_params["constraints"] = ",".join(need.get("constraints", []))
+            need_params["constraints"] = need.get("constraints", [])
 
             del need_params["description"]
 
             # check if external needs already exist
             ext_need_id = need_params["id"]
 
             need = SphinxNeedsData(env).get_or_create_needs().get(ext_need_id)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/filter_common.py` & `sphinx_needs-2.1.0/sphinx_needs/filter_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 """
 filter_base is used to provide common filter functionality for directives
 like needtable, needlist and needflow.
 """
+
 from __future__ import annotations
 
 import re
 from types import CodeType
 from typing import Any, Iterable, TypedDict, TypeVar
 
+from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.api.exceptions import NeedsInvalidFilter
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import (
     NeedsFilteredBaseType,
     NeedsInfoType,
-    NeedsPartsInfoType,
     SphinxNeedsData,
 )
 from sphinx_needs.debug import measure_time, measure_time_func
+from sphinx_needs.roles.need_part import iter_need_parts
 from sphinx_needs.utils import check_and_get_external_filter_func
 from sphinx_needs.utils import logger as log
 
 
 class FilterAttributesType(TypedDict):
     status: list[str]
     tags: list[str]
     types: list[str]
     filter: str
     sort_by: str
     filter_code: list[str]
     filter_func: str
     export_id: str
+    filter_warning: str
     """If set, the filter is exported with this ID in the needs.json file."""
 
 
 class FilterBase(SphinxDirective):
     has_content = True
 
     base_option_spec = {
         "status": directives.unchanged_required,
         "tags": directives.unchanged_required,
         "types": directives.unchanged_required,
         "filter": directives.unchanged_required,
         "filter-func": directives.unchanged_required,
         "sort_by": directives.unchanged,
         "export_id": directives.unchanged,
+        "filter_warning": directives.unchanged,
     }
 
     def collect_filter_attributes(self) -> FilterAttributesType:
         _tags = str(self.options.get("tags", ""))
-        tags = [tag.strip() for tag in re.split(";|,", _tags) if len(tag) > 0] if _tags else []
+        tags = (
+            [tag.strip() for tag in re.split(";|,", _tags) if len(tag) > 0]
+            if _tags
+            else []
+        )
 
         status = self.options.get("status")
         if status:
             try:
                 status = str(status)
                 status = [stat.strip() for stat in re.split(";|,", status)]
             except Exception:
@@ -79,97 +87,125 @@
             "tags": tags,
             "types": types,
             "filter": self.options.get("filter"),
             "sort_by": self.options.get("sort_by"),
             "filter_code": self.content,
             "filter_func": self.options.get("filter-func"),
             "export_id": self.options.get("export_id", ""),
+            "filter_warning": self.options.get("filter_warning"),
         }
         return collected_filter_options
 
 
 def process_filters(
-    app: Sphinx, all_needs: Iterable[NeedsInfoType], filter_data: NeedsFilteredBaseType, include_external: bool = True
-) -> list[NeedsPartsInfoType]:
+    app: Sphinx,
+    all_needs: Iterable[NeedsInfoType],
+    filter_data: NeedsFilteredBaseType,
+    include_external: bool = True,
+) -> list[NeedsInfoType]:
     """
     Filters all needs with given configuration.
     Used by needlist, needtable and needflow.
 
     :param app: Sphinx application object
     :param filter_data: Filter configuration
     :param all_needs: List of all needs inside document
     :param include_external: Boolean, which decides to include external needs or not
 
     :return: list of needs, which passed the filters
     """
     needs_config = NeedsSphinxConfig(app.config)
-    found_needs: list[NeedsPartsInfoType]
+    found_needs: list[NeedsInfoType]
     sort_key = filter_data["sort_by"]
     if sort_key:
         try:
             all_needs = sorted(all_needs, key=lambda node: node[sort_key] or "")  # type: ignore[literal-required]
         except KeyError as e:
-            log.warning(f"Sorting parameter {sort_key} not valid: Error: {e} [needs]", type="needs")
+            log.warning(
+                f"Sorting parameter {sort_key} not valid: Error: {e} [needs]",
+                type="needs",
+            )
 
     # check if include external needs
     checked_all_needs: Iterable[NeedsInfoType]
     if not include_external:
         checked_all_needs = []
         for need in all_needs:
             if not need["is_external"]:
                 checked_all_needs.append(need)
     else:
         checked_all_needs = all_needs
 
-    found_needs_by_options: list[NeedsPartsInfoType] = []
+    found_needs_by_options: list[NeedsInfoType] = []
 
     # Add all need_parts of given needs to the search list
     all_needs_incl_parts = prepare_need_list(checked_all_needs)
 
     # Check if external filter code is defined
-    filter_func, filter_args = check_and_get_external_filter_func(filter_data.get("filter_func"))
+    filter_func, filter_args = check_and_get_external_filter_func(
+        filter_data.get("filter_func")
+    )
 
     filter_code = None
     # Get filter_code from
     if not filter_code and filter_data["filter_code"]:
         filter_code = "\n".join(filter_data["filter_code"])
 
     if (not filter_code or filter_code.isspace()) and not filter_func:
         if bool(filter_data["status"] or filter_data["tags"] or filter_data["types"]):
             for need_info in all_needs_incl_parts:
                 status_filter_passed = False
-                if not filter_data["status"] or need_info["status"] and need_info["status"] in filter_data["status"]:
+                if (
+                    not filter_data["status"]
+                    or need_info["status"]
+                    and need_info["status"] in filter_data["status"]
+                ):
                     # Filtering for status was not requested or match was found
                     status_filter_passed = True
 
                 tags_filter_passed = False
-                if len(set(need_info["tags"]) & set(filter_data["tags"])) > 0 or len(filter_data["tags"]) == 0:
+                if (
+                    len(set(need_info["tags"]) & set(filter_data["tags"])) > 0
+                    or len(filter_data["tags"]) == 0
+                ):
                     tags_filter_passed = True
 
                 type_filter_passed = False
                 if (
                     need_info["type"] in filter_data["types"]
                     or need_info["type_name"] in filter_data["types"]
                     or len(filter_data["types"]) == 0
                 ):
                     type_filter_passed = True
 
                 if status_filter_passed and tags_filter_passed and type_filter_passed:
                     found_needs_by_options.append(need_info)
             # Get need by filter string
-            found_needs_by_string = filter_needs(all_needs_incl_parts, needs_config, filter_data["filter"])
+            found_needs_by_string = filter_needs(
+                all_needs_incl_parts,
+                needs_config,
+                filter_data["filter"],
+                location=(filter_data["docname"], filter_data["lineno"]),
+            )
             # Make an intersection of both lists
-            found_needs = intersection_of_need_results(found_needs_by_options, found_needs_by_string)
+            found_needs = intersection_of_need_results(
+                found_needs_by_options, found_needs_by_string
+            )
         else:
             # There is no other config as the one for filter string.
             # So we only need this result.
-            found_needs = filter_needs(all_needs_incl_parts, needs_config, filter_data["filter"])
+            found_needs = filter_needs(
+                all_needs_incl_parts,
+                needs_config,
+                filter_data["filter"],
+                location=(filter_data["docname"], filter_data["lineno"]),
+            )
     else:
         # Provides only a copy of needs to avoid data manipulations.
-        context = {
+        context: dict[str, Any] = {
             "needs": all_needs_incl_parts,
             "results": [],
         }
 
         if filter_code:  # code from content
             exec(filter_code, context)
         elif filter_func:  # code from external file
@@ -177,22 +213,24 @@
             if filter_args:
                 args = filter_args.split(",")
             for index, arg in enumerate(args):
                 # All args are strings, but we must transform them to requested type, e.g. 1 -> int, "1" -> str
                 context[f"arg{index+1}"] = arg
 
             # Decorate function to allow time measurments
-            filter_func = measure_time_func(filter_func, category="filter_func", source="user")
+            filter_func = measure_time_func(
+                filter_func, category="filter_func", source="user"
+            )
             filter_func(**context)
         else:
             log.warning("Something went wrong running filter [needs]", type="needs")
             return []
 
         # The filter results may be dirty, as it may continue manipulated needs.
-        found_dirty_needs: list[NeedsPartsInfoType] = context["results"]  # type: ignore
+        found_dirty_needs: list[NeedsInfoType] = context["results"]
         found_needs = []
 
         # Check if config allow unsafe filters
         if needs_config.allow_unsafe_filters:
             found_needs = found_dirty_needs
         else:
             # Just take the ids from search result and use the related, but original need
@@ -215,37 +253,29 @@
         "result": found_needs_ids,
         "amount": len(found_needs_ids),
     }
 
     return found_needs
 
 
-def prepare_need_list(need_list: Iterable[NeedsInfoType]) -> list[NeedsPartsInfoType]:
+def prepare_need_list(need_list: Iterable[NeedsInfoType]) -> list[NeedsInfoType]:
     # all_needs_incl_parts = need_list.copy()
-    all_needs_incl_parts: list[NeedsPartsInfoType]
+    all_needs_incl_parts: list[NeedsInfoType]
     try:
         all_needs_incl_parts = need_list[:]  # type: ignore
     except TypeError:
         try:
             all_needs_incl_parts = need_list.copy()  # type: ignore
         except AttributeError:
-            all_needs_incl_parts = list(need_list)[:]  # type: ignore
+            all_needs_incl_parts = list(need_list)[:]
 
     for need in need_list:
-        for part in need["parts"].values():
-            id_complete = ".".join([need["id"], part["id"]])
-            filter_part: NeedsPartsInfoType = {**need, **part, **{"id_parent": need["id"], "id_complete": id_complete}}
+        for filter_part in iter_need_parts(need):
             all_needs_incl_parts.append(filter_part)
 
-        # Be sure extra attributes, which makes only sense for need_parts, are also available on
-        # need level so that no KeyError gets raised, if search/filter get executed on needs with a need-part argument.
-        if "id_parent" not in need:
-            need["id_parent"] = need["id"]  # type: ignore[typeddict-unknown-key]
-        if "id_complete" not in need:
-            need["id_complete"] = need["id"]  # type: ignore[typeddict-unknown-key]
     return all_needs_incl_parts
 
 
 T = TypeVar("T")
 
 
 def intersection_of_need_results(list_a: list[T], list_b: list[T]) -> list[T]:
@@ -257,49 +287,69 @@
 
 @measure_time("filtering")
 def filter_needs(
     needs: Iterable[V],
     config: NeedsSphinxConfig,
     filter_string: None | str = "",
     current_need: NeedsInfoType | None = None,
+    *,
+    location: tuple[str, int | None] | nodes.Node | None = None,
+    append_warning: str = "",
 ) -> list[V]:
     """
     Filters given needs based on a given filter string.
     Returns all needs, which pass the given filter.
 
     :param needs: list of needs, which shall be filtered
     :param config: NeedsSphinxConfig object
     :param filter_string: strings, which gets evaluated against each need
     :param current_need: current need, which uses the filter.
+    :param location: source location for error reporting (docname, line number)
+    :param append_warning: additional text to append to any failed filter warning
 
     :return: list of found needs
     """
     if not filter_string:
         return list(needs)
 
     found_needs = []
 
     # https://docs.python.org/3/library/functions.html?highlight=compile#compile
     filter_compiled = compile(filter_string, "<string>", "eval")
     error_reported = False
     for filter_need in needs:
         try:
             if filter_single_need(
-                filter_need, config, filter_string, needs, current_need, filter_compiled=filter_compiled
+                filter_need,
+                config,
+                filter_string,
+                needs,
+                current_need,
+                filter_compiled=filter_compiled,
             ):
                 found_needs.append(filter_need)
         except Exception as e:
-            if not error_reported:  # Let's report a filter-problem only onces
-                location = (current_need["docname"], current_need["lineno"]) if current_need else None
-                log.warning(str(e) + " [needs]", type="needs", location=location)
+            if not error_reported:  # Let's report a filter-problem only once
+                if append_warning:
+                    append_warning = f" {append_warning}"
+                log.warning(
+                    f"{e}{append_warning} [needs.filter]",
+                    type="needs",
+                    subtype="filter",
+                    location=location,
+                )
                 error_reported = True
 
     return found_needs
 
 
+def need_search(*args: Any, **kwargs: Any) -> bool:
+    return re.search(*args, **kwargs) is not None
+
+
 @measure_time("filtering")
 def filter_single_need(
     need: NeedsInfoType,
     config: NeedsSphinxConfig,
     filter_string: str = "",
     needs: Iterable[NeedsInfoType] | None = None,
     current_need: NeedsInfoType | None = None,
@@ -323,19 +373,23 @@
         filter_context["current_need"] = current_need
     else:
         filter_context["current_need"] = need
 
     # Get needs external filter data and merge to filter_context
     filter_context.update(config.filter_data)
 
-    filter_context["search"] = re.search
+    filter_context["search"] = need_search
     result = False
     try:
         # Set filter_context as globals and not only locals in eval()!
         # Otherwise, the vars not be accessed in list comprehensions.
         if filter_compiled:
-            result = bool(eval(filter_compiled, filter_context))
+            result = eval(filter_compiled, filter_context)
         else:
-            result = bool(eval(filter_string, filter_context))
+            result = eval(filter_string, filter_context)
+        if not isinstance(result, bool):
+            raise NeedsInvalidFilter(
+                f"Filter did not evaluate to a boolean, instead {type(result)}: {result}"
+            )
     except Exception as e:
-        raise NeedsInvalidFilter(f"Filter {filter_string} not valid. Error: {e}.")
+        raise NeedsInvalidFilter(f"Filter {filter_string!r} not valid. Error: {e}.")
     return result
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/functions/__init__.py` & `sphinx_needs-2.1.0/sphinx_needs/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/functions/common.py` & `sphinx_needs-2.1.0/sphinx_needs/functions/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """
 Collection of common sphinx-needs functions for dynamic values
 
 .. note:: The function parameters ``app``, ``need``, ``needs`` are set automatically and can not be overridden by user.
 """
 
+from __future__ import annotations
+
 import contextlib
 import re
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 from sphinx.application import Sphinx
 
 from sphinx_needs.api.exceptions import NeedsInvalidFilter
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType
 from sphinx_needs.filter_common import filter_needs, filter_single_need
 from sphinx_needs.utils import logger
 
 
-def test(app: Sphinx, need: NeedsInfoType, needs: Dict[str, NeedsInfoType], *args: Any, **kwargs: Any) -> str:
+def test(
+    app: Sphinx,
+    need: NeedsInfoType,
+    needs: dict[str, NeedsInfoType],
+    *args: Any,
+    **kwargs: Any,
+) -> str:
     """
     Test function for dynamic functions in sphinx needs.
 
     Collects every given args and kwargs and returns a single string, which contains their values/keys.
 
     .. code-block:: jinja
 
@@ -35,15 +43,20 @@
 
     :return: single test string
     """
     return f"Test output of need {need['id']}. args: {args}. kwargs: {kwargs}"
 
 
 def echo(
-    app: Sphinx, need: NeedsInfoType, needs: Dict[str, NeedsInfoType], text: str, *args: Any, **kwargs: Any
+    app: Sphinx,
+    need: NeedsInfoType,
+    needs: dict[str, NeedsInfoType],
+    text: str,
+    *args: Any,
+    **kwargs: Any,
 ) -> str:
     """
     .. versionadded:: 0.6.3
 
     Just returns the given string back.
     Mostly useful for tests.
 
@@ -56,20 +69,20 @@
     """
     return text
 
 
 def copy(
     app: Sphinx,
     need: NeedsInfoType,
-    needs: Dict[str, NeedsInfoType],
+    needs: dict[str, NeedsInfoType],
     option: str,
-    need_id: Optional[str] = None,
+    need_id: str | None = None,
     lower: bool = False,
     upper: bool = False,
-    filter: Optional[str] = None,
+    filter: str | None = None,
 ) -> Any:
     """
     Copies the value of one need option to another
 
     .. code-block:: jinja
 
         .. req:: copy-example
@@ -148,15 +161,21 @@
     :param filter: :ref:`filter_string`, which first result is used as copy source.
     :return: string of copied need option
     """
     if need_id:
         need = needs[need_id]
 
     if filter:
-        result = filter_needs(needs.values(), NeedsSphinxConfig(app.config), filter, need)
+        result = filter_needs(
+            needs.values(),
+            NeedsSphinxConfig(app.config),
+            filter,
+            need,
+            location=(need["docname"], need["lineno"]) if need["docname"] else None,
+        )
         if result:
             need = result[0]
 
     value = need[option]  # type: ignore[literal-required]
 
     # TODO check if str?
 
@@ -167,19 +186,19 @@
 
     return value
 
 
 def check_linked_values(
     app: Sphinx,
     need: NeedsInfoType,
-    needs: Dict[str, NeedsInfoType],
+    needs: dict[str, NeedsInfoType],
     result: Any,
     search_option: str,
     search_value: Any,
-    filter_string: Optional[str] = None,
+    filter_string: str | None = None,
     one_hit: bool = False,
 ) -> Any:
     """
     Returns a specific value, if for all linked needs a given option has a given value.
 
     The linked needs can be filtered by using the ``filter`` option.
 
@@ -317,31 +336,34 @@
     for link in links:
         need = needs[link]
         if filter_string:
             try:
                 if not filter_single_need(need, needs_config, filter_string):
                     continue
             except Exception as e:
-                logger.warning(f"CheckLinkedValues: Filter {filter_string} not valid: Error: {e} [needs]", type="needs")
+                logger.warning(
+                    f"CheckLinkedValues: Filter {filter_string} not valid: Error: {e} [needs]",
+                    type="needs",
+                )
 
         need_value = need[search_option]  # type: ignore[literal-required]
         if not one_hit and need_value not in search_value:
             return None
         elif one_hit and need_value in search_value:
             return result
 
     return result
 
 
 def calc_sum(
     app: Sphinx,
     need: NeedsInfoType,
-    needs: Dict[str, NeedsInfoType],
+    needs: dict[str, NeedsInfoType],
     option: str,
-    filter: Optional[str] = None,
+    filter: str | None = None,
     links_only: bool = False,
 ) -> float:
     """
     Sums the values of a given option in filtered needs up to single number.
 
     Useful e.g. for calculating the amount of needed hours for implementation of all linked
     specification needs.
@@ -416,41 +438,45 @@
     :param option: Options, from which the numbers shall be taken
     :param filter: Filter string, which all needs must passed to get their value added.
     :param links_only: If "True", only linked needs are taken into account.
 
     :return: A float number
     """
     needs_config = NeedsSphinxConfig(app.config)
-    check_needs = [needs[link] for link in need["links"]] if links_only else needs.values()
+    check_needs = (
+        [needs[link] for link in need["links"]] if links_only else needs.values()
+    )
 
     calculated_sum = 0.0
 
     for check_need in check_needs:
         if filter:
             try:
                 if not filter_single_need(check_need, needs_config, filter):
                     continue
             except ValueError:
                 pass
             except NeedsInvalidFilter as ex:
-                logger.warning(f"Given filter is not valid. Error: {ex} [needs]", type="needs")
+                logger.warning(
+                    f"Given filter is not valid. Error: {ex} [needs]", type="needs"
+                )
 
         with contextlib.suppress(ValueError):
             calculated_sum += float(check_need[option])  # type: ignore[literal-required]
 
     return calculated_sum
 
 
 def links_from_content(
     app: Sphinx,
     need: NeedsInfoType,
-    needs: Dict[str, NeedsInfoType],
-    need_id: Optional[str] = None,
-    filter: Optional[str] = None,
-) -> List[str]:
+    needs: dict[str, NeedsInfoType],
+    need_id: str | None = None,
+    filter: str | None = None,
+) -> list[str]:
     """
     Extracts links from content of a need.
 
     All need-links set by using ``:need:`NEED_ID``` get extracted.
 
     Same links are only added once.
 
@@ -508,12 +534,14 @@
         elif link[1] and link[0] not in raw_links:
             raw_links.append(link[1])
 
     if filter:
         needs_config = NeedsSphinxConfig(app.config)
         filtered_links = []
         for link in raw_links:
-            if link not in filtered_links and filter_single_need(needs[link], needs_config, filter):
+            if link not in filtered_links and filter_single_need(
+                needs[link], needs_config, filter
+            ):
                 filtered_links.append(link)
         return filtered_links
 
     return raw_links
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/functions/functions.py` & `sphinx_needs-2.1.0/sphinx_needs/functions/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 Sphinx-needs functions module
 =============================
 
 Cares about the correct registration and execution of sphinx-needs functions to support dynamic values
 in need configurations.
 """
 
+from __future__ import annotations
+
 import ast
 import re
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Union
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx.errors import SphinxError
 
 from sphinx_needs.config import NeedsSphinxConfig
@@ -23,19 +25,20 @@
 
 logger = get_logger(__name__)
 unicode = str
 ast_boolean = ast.NameConstant
 
 # TODO these functions also take optional *args and **kwargs
 DynamicFunction = Callable[
-    [Sphinx, NeedsInfoType, Dict[str, NeedsInfoType]], Union[str, int, float, List[Union[str, int, float]]]
+    [Sphinx, NeedsInfoType, Dict[str, NeedsInfoType]],
+    Union[str, int, float, List[Union[str, int, float]]],
 ]
 
 
-def register_func(need_function: DynamicFunction, name: Optional[str] = None) -> None:
+def register_func(need_function: DynamicFunction, name: str | None = None) -> None:
     """
     Registers a new sphinx-needs function for the given sphinx environment.
     :param env: Sphinx environment
     :param need_function: Python method
     :param name: Name of the function as string
     :return: None
     """
@@ -49,15 +52,17 @@
     else:
         func_name = name
 
     if func_name in NEEDS_FUNCTIONS:
         # We can not throw an exception here, as using sphinx-needs in different sphinx-projects with the
         # same python interpreter session does not clean NEEDS_FUNCTIONS.
         # This is mostly the case during tet runs.
-        logger.info(f"sphinx-needs: Function name {func_name} already registered. Ignoring the new one!")
+        logger.info(
+            f"sphinx-needs: Function name {func_name} already registered. Ignoring the new one!"
+        )
 
     NEEDS_FUNCTIONS[func_name] = {"name": func_name, "function": need_function}
 
 
 def execute_func(app: Sphinx, need: NeedsInfoType, func_string: str) -> Any:
     """Executes a given function string.
 
@@ -66,71 +71,87 @@
     :param func_string: string of the found function. Without ``[[ ]]``
     :return: return value of executed function
     """
     global NEEDS_FUNCTIONS
     func_name, func_args, func_kwargs = _analyze_func_string(func_string, need)
 
     if func_name not in NEEDS_FUNCTIONS:
-        raise SphinxError("Unknown dynamic sphinx-needs function: {}. Found in need: {}".format(func_name, need["id"]))
+        raise SphinxError(
+            "Unknown dynamic sphinx-needs function: {}. Found in need: {}".format(
+                func_name, need["id"]
+            )
+        )
 
-    func = measure_time_func(NEEDS_FUNCTIONS[func_name]["function"], category="dyn_func", source="user")
-    func_return = func(app, need, SphinxNeedsData(app.env).get_or_create_needs(), *func_args, **func_kwargs)
+    func = measure_time_func(
+        NEEDS_FUNCTIONS[func_name]["function"], category="dyn_func", source="user"
+    )
+    func_return = func(
+        app,
+        need,
+        SphinxNeedsData(app.env).get_or_create_needs(),
+        *func_args,
+        **func_kwargs,
+    )
 
     if not isinstance(func_return, (str, int, float, list, unicode)) and func_return:
         raise SphinxError(
-            "Return value of function {} is of type {}. Allowed are str, int, float".format(
-                func_name, type(func_return)
-            )
+            f"Return value of function {func_name} is of type {type(func_return)}. Allowed are str, int, float"
         )
 
     if isinstance(func_return, list):
         for element in func_return:
             if not isinstance(element, (str, int, float, unicode)):
                 raise SphinxError(
-                    "Element of return list of function {} is of type {}. "
-                    "Allowed are str, int, float".format(func_name, type(func_return))
+                    f"Element of return list of function {func_name} is of type {type(func_return)}. "
+                    "Allowed are str, int, float"
                 )
     return func_return
 
 
 func_pattern = re.compile(r"\[\[(.*?)\]\]")  # RegEx to detect function strings
 
 
-def find_and_replace_node_content(node: nodes.Node, env: BuildEnvironment, need: NeedsInfoType) -> nodes.Node:
+def find_and_replace_node_content(
+    node: nodes.Node, env: BuildEnvironment, need: NeedsInfoType
+) -> nodes.Node:
     """
     Search inside a given node and its children for nodes of type Text,
     if found, check if it contains a function string and run/replace it.
 
     :param node: Node to analyse
     :return: None
     """
     new_children = []
-    if not node.children and isinstance(node, nodes.Text) or isinstance(node, nodes.reference):
+    if (
+        not node.children
+        and isinstance(node, nodes.Text)
+        or isinstance(node, nodes.reference)
+    ):
         if isinstance(node, nodes.reference):
             try:
                 new_text = node.attributes["refuri"]
             except KeyError:
                 # If no refuri is set, we don't need to modify anything.
                 # So stop here and return the untouched node.
-                return node  # type: ignore
+                return node
         else:
             new_text = node
         func_match = func_pattern.findall(new_text)
         for func_string in func_match:
             # sphinx is replacing ' and " with language specific quotation marks (up and down), which makes
             # it impossible for the later used AST render engine to detect a python function call in the given
             # string. Therefor a replacement is needed for the execution of the found string.
             func_string_org = func_string[:]
             func_string = func_string.replace("„", '"')
             func_string = func_string.replace("“", '"')
             func_string = func_string.replace("”", '"')
             func_string = func_string.replace("”", '"')
 
-            func_string = func_string.replace("‘", "'")
-            func_string = func_string.replace("’", "'")
+            func_string = func_string.replace("‘", "'")  # noqa: RUF001
+            func_string = func_string.replace("’", "'")  # noqa: RUF001
             func_return = execute_func(env.app, need, func_string)
 
             # This should never happen, but we can not be sure.
             if isinstance(func_return, list):
                 func_return = ", ".join(func_return)
 
             new_text = new_text.replace(f"[[{func_string_org}]]", func_return)
@@ -140,24 +161,24 @@
             # Call normal handling for children of reference node (will contain related Text node with link-text)
             for child in node.children:
                 new_child = find_and_replace_node_content(child, env, need)
                 new_children.append(new_child)
                 node.children = new_children
         else:
             node = nodes.Text(new_text)
-        return node  # type: ignore
+        return node
     else:
         for child in node.children:
             new_child = find_and_replace_node_content(child, env, need)
             new_children.append(new_child)
         node.children = new_children
     return node
 
 
-def resolve_dynamic_values(needs: Dict[str, NeedsInfoType], app: Sphinx) -> None:
+def resolve_dynamic_values(needs: dict[str, NeedsInfoType], app: Sphinx) -> None:
     """
     Resolve dynamic values inside need data.
 
     Rough workflow:
 
     #. Parse all needs and their field values for a string like ``[[ my_func(a, b, c) ]]``
     #. Extract function name and call parameters
@@ -170,72 +191,92 @@
     - ``need``: Need data
     - ``all_needs``: All needs of the current sphinx project
     - ``*args``: optional arguments (specified in the function string)
     - ``**kwargs``: optional keyword arguments (specified in the function string)
     """
     for need in needs.values():
         for need_option in need:
-            if need_option in ["docname", "lineno", "content", "content_node", "content_id"]:
+            if need_option in [
+                "docname",
+                "lineno",
+                "content",
+                "content_node",
+                "content_id",
+            ]:
                 # dynamic values in this data are not allowed.
                 continue
             if not isinstance(need[need_option], (list, set)):
-                func_call: Optional[str] = "init"
+                func_call: str | None = "init"
                 while func_call:
                     try:
-                        func_call, func_return = _detect_and_execute(need[need_option], need, app)
+                        func_call, func_return = _detect_and_execute(
+                            need[need_option], need, app
+                        )
                     except FunctionParsingException:
                         raise SphinxError(
                             "Function definition of {option} in file {file}:{line} has "
                             "unsupported parameters. "
                             "supported are str, int/float, list".format(
-                                option=need_option, file=need["docname"], line=need["lineno"]
+                                option=need_option,
+                                file=need["docname"],
+                                line=need["lineno"],
                             )
                         )
 
                     if func_call is None:
                         continue
                     # Replace original function string with return value of function call
                     if func_return is None:
-                        need[need_option] = need[need_option].replace(f"[[{func_call}]]", "")
+                        need[need_option] = need[need_option].replace(
+                            f"[[{func_call}]]", ""
+                        )
                     else:
-                        need[need_option] = need[need_option].replace(f"[[{func_call}]]", str(func_return))
+                        need[need_option] = need[need_option].replace(
+                            f"[[{func_call}]]", str(func_return)
+                        )
 
                     if need[need_option] == "":
                         need[need_option] = None
             else:
                 new_values = []
                 for element in need[need_option]:
                     try:
                         func_call, func_return = _detect_and_execute(element, need, app)
                     except FunctionParsingException:
                         raise SphinxError(
                             "Function definition of {option} in file {file}:{line} has "
                             "unsupported parameters. "
                             "supported are str, int/float, list".format(
-                                option=need_option, file=need["docname"], line=need["lineno"]
+                                option=need_option,
+                                file=need["docname"],
+                                line=need["lineno"],
                             )
                         )
                     if func_call is None:
                         new_values.append(element)
                     else:
                         # Replace original function string with return value of function call
                         if isinstance(need[need_option], (str, int, float)):
-                            new_values.append(element.replace(f"[[{func_call}]]", str(func_return)))
+                            new_values.append(
+                                element.replace(f"[[{func_call}]]", str(func_return))
+                            )
                         else:
                             if isinstance(need[need_option], (list, set)):
                                 if isinstance(func_return, (list, set)):
                                     new_values += func_return
                                 else:
                                     new_values += [func_return]
 
                 need[need_option] = new_values
 
 
 def resolve_variants_options(
-    needs: Dict[str, NeedsInfoType], needs_config: NeedsSphinxConfig, tags: Dict[str, bool]
+    needs: dict[str, NeedsInfoType],
+    needs_config: NeedsSphinxConfig,
+    tags: dict[str, bool],
 ) -> None:
     """
     Resolve variants options inside need data.
 
     These are fields specified by the user,
     that have string values with a special markup syntax like ``var_a:open``.
     These need to be resolved to the actual value.
@@ -248,29 +289,37 @@
     variants_options = needs_config.variant_options
 
     if not variants_options:
         return
 
     for need in needs.values():
         # Data to use as filter context.
-        need_context: Dict[str, Any] = {**need}
-        need_context.update(**needs_config.filter_data)  # Add needs_filter_data to filter context
+        need_context: dict[str, Any] = {**need}
+        need_context.update(
+            **needs_config.filter_data
+        )  # Add needs_filter_data to filter context
         need_context.update(**tags)  # Add sphinx tags to filter context
 
         for var_option in variants_options:
             if var_option in need and need[var_option] not in (None, "", []):
                 if not isinstance(need[var_option], (list, set, tuple)):
                     option_value: str = need[var_option]
-                    need[var_option] = match_variants(option_value, need_context, needs_config.variants)
+                    need[var_option] = match_variants(
+                        option_value, need_context, needs_config.variants
+                    )
                 else:
                     option_value = need[var_option]
-                    need[var_option] = match_variants(option_value, need_context, needs_config.variants)
+                    need[var_option] = match_variants(
+                        option_value, need_context, needs_config.variants
+                    )
 
 
-def check_and_get_content(content: str, need: NeedsInfoType, env: BuildEnvironment) -> str:
+def check_and_get_content(
+    content: str, need: NeedsInfoType, env: BuildEnvironment
+) -> str:
     """
     Checks if the given content is a function call.
     If not, content is returned.
     If it is, the functions gets executed and its returns value replaces the related part in content.
 
     :param content: option content string
     :param need: need
@@ -284,39 +333,47 @@
         content = content.encode("utf-8")  # type: ignore
 
     func_match = func_pattern.search(content)
     if func_match is None:
         return content
 
     func_call = func_match.group(1)  # Extract function call
-    func_return = execute_func(env.app, need, func_call)  # Execute function call and get return value
+    func_return = execute_func(
+        env.app, need, func_call
+    )  # Execute function call and get return value
 
     # Replace the function_call with the calculated value
     content = content.replace(f"[[{func_call}]]", func_return)
     return content
 
 
-def _detect_and_execute(content: Any, need: NeedsInfoType, app: Sphinx) -> Tuple[Optional[str], Any]:
+def _detect_and_execute(
+    content: Any, need: NeedsInfoType, app: Sphinx
+) -> tuple[str | None, Any]:
     """Detects if given content is a function call and executes it."""
     try:
         content = str(content)
     except UnicodeEncodeError:
         content = content.encode("utf-8")
 
     func_match = func_pattern.search(content)
     if func_match is None:
         return None, None
 
     func_call = func_match.group(1)  # Extract function call
-    func_return = execute_func(app, need, func_call)  # Execute function call and get return value
+    func_return = execute_func(
+        app, need, func_call
+    )  # Execute function call and get return value
 
     return func_call, func_return
 
 
-def _analyze_func_string(func_string: str, need: Optional[NeedsInfoType]) -> Tuple[str, List[Any], Dict[str, Any]]:
+def _analyze_func_string(
+    func_string: str, need: NeedsInfoType | None
+) -> tuple[str, list[Any], dict[str, Any]]:
     """
     Analyze given function string and extract:
 
     * function name
     * function arguments
     * function keyword arguments
 
@@ -325,29 +382,33 @@
     :param func_string: string of the function
     :return: function name, arguments, keyword arguments
     """
     try:
         func = ast.parse(func_string)
     except SyntaxError as e:
         need_id = need["id"] if need else "UNKNOWN"
-        raise SphinxError(f"Parsing function string failed for need {need_id}: {func_string}. {e}")
+        raise SphinxError(
+            f"Parsing function string failed for need {need_id}: {func_string}. {e}"
+        )
     try:
         func_call = func.body[0].value  # type: ignore
         func_name = func_call.func.id
     except AttributeError:
-        raise SphinxError(f"Given dynamic function string is not a valid python call. Got: {func_string}")
+        raise SphinxError(
+            f"Given dynamic function string is not a valid python call. Got: {func_string}"
+        )
 
-    func_args: List[Any] = []
+    func_args: list[Any] = []
     for arg in func_call.args:
         if isinstance(arg, ast.Num):
             func_args.append(arg.n)
         elif isinstance(arg, (ast.Str, ast.BoolOp)):
             func_args.append(arg.s)  # type: ignore
         elif isinstance(arg, ast.List):
-            arg_list: List[Any] = []
+            arg_list: list[Any] = []
             for element in arg.elts:
                 if isinstance(element, ast.Num):
                     arg_list.append(element.n)
                 elif isinstance(element, ast.Str):
                     arg_list.append(element.s)
             func_args.append(arg_list)
         elif isinstance(arg, ast.Attribute):
@@ -360,18 +421,18 @@
                 func_args.append(arg.value)
             else:
                 raise FunctionParsingException(
                     "Unsupported type found in function definition. Supported are numbers, strings, bool and list"
                 )
         else:
             raise FunctionParsingException(
-                "Unsupported type found in function definition: {}. "
-                "Supported are numbers, strings, bool and list".format(func_string)
+                f"Unsupported type found in function definition: {func_string}. "
+                "Supported are numbers, strings, bool and list"
             )
-    func_kargs: Dict[str, Any] = {}
+    func_kargs: dict[str, Any] = {}
     for keyword in func_call.keywords:
         kvalue = keyword.value
         kkey = keyword.arg
         if isinstance(kvalue, ast.Num):
             func_kargs[kkey] = kvalue.n
         elif isinstance(kvalue, ast.Str):
             func_kargs[kkey] = kvalue.s
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/avatar.png` & `sphinx_needs-2.1.0/sphinx_needs/images/avatar.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/avatar.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/avatar.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/alert-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/alert-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/alert-triangle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/alert-triangle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/anchor.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/anchor.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/aperture.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/aperture.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-down-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-down-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-left-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-left-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-right-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-right-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/arrow-up-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/arrow-up-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/at-sign.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/at-sign.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/award.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/award.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/battery-charging.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/battery-charging.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bell-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bell-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/bell.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/bell.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/box.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/box.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/camera-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/camera-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/camera.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/camera.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cast.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cast.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/check-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/check-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/chrome.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/chrome.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/clock.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/clock.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-drizzle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-drizzle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-lightning.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-lightning.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-rain.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-rain.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud-snow.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud-snow.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cloud.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cloud.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/codepen.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/codepen.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/codesandbox.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/codesandbox.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/coffee.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/coffee.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/compass.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/compass.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/copy.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/copy.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/cpu.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/cpu.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/crosshair.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/crosshair.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/database.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/database.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/disc.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/disc.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/download-cloud.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/download-cloud.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/droplet.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/droplet.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/edit.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/edit.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/external-link.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/external-link.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/eye-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/eye-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/eye.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/eye.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/facebook.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/facebook.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/feather.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/feather.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/figma.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/figma.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file-plus.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file-plus.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/file-text.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/file-text.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/film.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/film.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/folder-plus.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/folder-plus.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/frown.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/frown.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/gift.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/gift.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/git-branch.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/git-branch.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/github.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/github.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/gitlab.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/gitlab.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/globe.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/globe.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/hard-drive.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/hard-drive.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/headphones.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/headphones.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/heart.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/heart.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/help-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/help-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/image.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/image.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/inbox.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/inbox.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/info.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/info.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/instagram.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/instagram.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/key.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/key.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/life-buoy.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/life-buoy.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/link.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/link.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/linkedin.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/linkedin.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mail.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mail.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/map-pin.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/map-pin.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/meh.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/meh.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/message-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/message-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mic-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mic-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mic.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mic.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/minus-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/minus-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/moon.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/moon.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/mouse-pointer.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/mouse-pointer.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/music.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/music.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/navigation-2.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/navigation-2.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/navigation.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/navigation.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/package.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/package.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/paperclip.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/paperclip.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pause-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pause-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pen-tool.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pen-tool.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-call.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-call.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-forwarded.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-forwarded.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-incoming.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-incoming.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-missed.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-missed.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone-outgoing.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone-outgoing.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/phone.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/phone.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pie-chart.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pie-chart.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/play-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/play-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/plus-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/plus-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/pocket.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/pocket.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/power.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/power.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/radio.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/radio.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/refresh-ccw.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/refresh-ccw.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/refresh-cw.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/refresh-cw.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rotate-ccw.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rotate-ccw.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rotate-cw.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rotate-cw.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/rss.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/rss.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/scissors.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/scissors.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/search.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/search.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/send.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/send.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/settings.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/settings.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/share-2.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/share-2.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shield-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shield-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shield.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shield.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shopping-bag.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shopping-bag.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/shopping-cart.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/shopping-cart.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/slack.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/slack.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/slash.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/slash.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sliders.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sliders.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/smile.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/smile.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/speaker.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/speaker.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/star.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/star.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/stop-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/stop-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sun.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sun.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sunrise.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sunrise.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/sunset.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/sunset.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/target.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/target.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/thumbs-down.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/thumbs-down.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/thumbs-up.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/thumbs-up.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/toggle-left.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/toggle-left.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/toggle-right.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/toggle-right.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/tool.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/tool.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/triangle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/triangle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/truck.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/truck.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/twitter.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/twitter.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/umbrella.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/umbrella.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/upload-cloud.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/upload-cloud.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-check.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-check.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-minus.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-minus.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-plus.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-plus.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user-x.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user-x.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/user.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/user.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/users.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/users.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/video-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/video-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/voicemail.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/voicemail.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/volume-2.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/volume-2.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/watch.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/watch.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wifi-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wifi-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wifi.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wifi.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/wind.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/wind.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/x-circle.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/x-circle.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/youtube.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/youtube.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zap-off.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zap-off.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zap.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zap.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zoom-in.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zoom-in.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_png/zoom-out.png` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_png/zoom-out.png`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/aperture.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/aperture.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-drizzle.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cloud-snow.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/codesandbox.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/cpu.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/cpu.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/figma.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/figma.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/film.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/film.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/github.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/github.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/life-buoy.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/loader.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/loader.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/package.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/package.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-call.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-call.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-forwarded.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-incoming.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-missed.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-off.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-off.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone-outgoing.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/phone.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/phone.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/settings.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/settings.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/slack.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/slack.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sliders.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sliders.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sun.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sun.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sunrise.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sunrise.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/sunset.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/sunset.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/wifi-off.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/images/feather_svg/youtube.svg` & `sphinx_needs-2.1.0/sphinx_needs/images/feather_svg/youtube.svg`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/layout.py` & `sphinx_needs-2.1.0/sphinx_needs/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Cares about the correct creation and handling of need layout.
 
 Based on https://github.com/useblocks/sphinxcontrib-needs/issues/102
 """
+
+from __future__ import annotations
+
 import os
 import re
 import uuid
 from contextlib import suppress
 from functools import lru_cache
 from optparse import Values
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, cast
 from urllib.parse import urlparse
 
 import requests
 from docutils import nodes
 from docutils.frontend import OptionParser
 from docutils.parsers.rst import Parser, languages
 from docutils.parsers.rst.states import Inliner, Struct
@@ -26,15 +29,19 @@
 from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.debug import measure_time
 from sphinx_needs.utils import INTERNALS, match_string_link
 
 
 @measure_time("need")
 def create_need(
-    need_id: str, app: Sphinx, layout: Optional[str] = None, style: Optional[str] = None, docname: Optional[str] = None
+    need_id: str,
+    app: Sphinx,
+    layout: str | None = None,
+    style: str | None = None,
+    docname: str | None = None,
 ) -> nodes.container:
     """
     Creates a new need-node for a given layout.
 
     Need must already exist in internal dictionary.
     This creates a new representation only.
     :param need_id: need id
@@ -52,15 +59,18 @@
 
     need_data = needs[need_id]
 
     # Resolve internal references.
     # This is done for original need content automatically.
     # But as we are working on  a copy, we have to trigger this on our own.
     if docname is None:
-        docname = needs[need_id]["docname"]  # needed to calculate relative references
+        # needed to calculate relative references
+        # TODO ideally we should not cast here:
+        # the docname can still be None, if the need is external, although practically these are not rendered
+        docname = cast(str, needs[need_id]["docname"])
 
     node_container = nodes.container()
     # node_container += needs[need_id]["need_node"].children
 
     # We must create a standalone copy of the content_node, as it may be reused several time
     # (multiple needextract for the same need) and the Sphinx ImageTransformator add location specific
     # uri to some nodes, which are not valid for all locations.
@@ -71,39 +81,43 @@
     # Rerun some important Sphinx collectors for need-content coming from "needsexternal".
     # This is needed, as Sphinx needs to know images and download paths.
     # Normally this gets done much earlier in the process, so that for the copied need-content this
     # handling was and will not be done by Sphinx itself anymore.
 
     # Overwrite the docname, which must be the original one from the reused need, as all used paths are relative
     # to the original location, not to the current document.
-    env.temp_data["docname"] = need_data["docname"]  # Dirty, as in this phase normally no docname is set anymore in env
+    env.temp_data["docname"] = need_data[
+        "docname"
+    ]  # Dirty, as in this phase normally no docname is set anymore in env
     ImageCollector().process_doc(app, node_inner)  # type: ignore[arg-type]
     DownloadFileCollector().process_doc(app, node_inner)  # type: ignore[arg-type]
 
     del env.temp_data["docname"]  # Be sure our env is as it was before
 
     node_container.append(node_inner)
 
     # resolve_references() ignores the given docname and takes the docname from the pending_xref node.
     # Therefore, we need to manipulate this first, before we can ask Sphinx to perform the normal
     # reference handling for us.
     replace_pending_xref_refdoc(node_container, docname)
-    env.resolve_references(node_container, docname, env.app.builder)
+    env.resolve_references(node_container, docname, env.app.builder)  # type: ignore[arg-type]
 
     node_container.attributes["ids"].append(need_id)
 
     needs_config = NeedsSphinxConfig(app.config)
     layout = layout or need_data["layout"] or needs_config.default_layout
     style = style or need_data["style"] or needs_config.default_style
 
     build_need(layout, node_container, app, style, docname)
 
     # set the layout and style for the new need
-    node_container[0].attributes = node_container.parent.children[0].attributes
-    node_container[0].children[0].attributes = node_container.parent.children[0].children[0].attributes
+    node_container[0].attributes = node_container.parent.children[0].attributes  # type: ignore
+    node_container[0].children[0].attributes = (  # type: ignore
+        node_container.parent.children[0].children[0].attributes  # type: ignore
+    )
 
     node_container.attributes["ids"] = []
 
     return node_container
 
 
 def replace_pending_xref_refdoc(node: nodes.Element, new_refdoc: str) -> None:
@@ -122,15 +136,19 @@
     else:
         for child in node.children:
             replace_pending_xref_refdoc(child, new_refdoc)  # type: ignore[arg-type]
 
 
 @measure_time("need")
 def build_need(
-    layout: str, node: nodes.Element, app: Sphinx, style: Optional[str] = None, fromdocname: Optional[str] = None
+    layout: str,
+    node: nodes.Element,
+    app: Sphinx,
+    style: str | None = None,
+    fromdocname: str | None = None,
 ) -> None:
     """
     Builds a need based on a given layout for a given need-node.
 
     The created table must have the following docutils structure::
 
         - table
@@ -150,15 +168,15 @@
     node_container = nodes.container()
 
     need_id = node.attributes["ids"][0]
     need_data = needs[need_id]
 
     if need_data["hide"]:
         if node.parent:
-            node.parent.replace(node, [])  # type: ignore
+            node.parent.replace(node, [])
         return
 
     if fromdocname is None:
         fromdocname = need_data["docname"]
 
     lh = LayoutHandler(app, need_data, layout, node, style, fromdocname)
     new_need_node = lh.get_need_table()
@@ -166,19 +184,19 @@
 
     container_id = "SNCB-" + str(uuid.uuid4())[:8]
     node_container.attributes["ids"] = [container_id]
     node_container.attributes["classes"] = ["need_container"]
 
     # We need to replace the current need-node (containing content only) with our new table need node.
     # node.parent.replace(node, node_container)
-    node.parent.replace(node, node_container)  # type: ignore
+    node.parent.replace(node, node_container)
 
 
 @lru_cache(1)
-def _generate_inline_parser() -> Tuple[Values, Inliner]:
+def _generate_inline_parser() -> tuple[Values, Inliner]:
     doc_settings = OptionParser(components=(Parser,)).get_default_values()
     inline_parser = Inliner()
     inline_parser.init_customizations(doc_settings)  # type: ignore
     return doc_settings, inline_parser
 
 
 class LayoutHandler:
@@ -188,41 +206,45 @@
 
     def __init__(
         self,
         app: Sphinx,
         need: NeedsInfoType,
         layout: str,
         node: nodes.Element,
-        style: Optional[str] = None,
-        fromdocname: Optional[str] = None,
+        style: str | None = None,
+        fromdocname: str | None = None,
     ) -> None:
         self.app = app
         self.need = need
         self.needs_config = NeedsSphinxConfig(app.config)
 
         self.layout_name = layout
         available_layouts = self.needs_config.layouts
-        if self.layout_name not in available_layouts.keys():
+        if self.layout_name not in available_layouts:
             raise SphinxNeedLayoutException(
                 'Given layout "{}" is unknown for need {}. Registered layouts are: {}'.format(
-                    self.layout_name, need["id"], " ,".join(available_layouts.keys())
+                    self.layout_name, need["id"], " ,".join(available_layouts)
                 )
             )
         self.layout = available_layouts[self.layout_name]
 
         self.node = node
 
         # Used, if you need is referenced from another page
         if fromdocname is None:
             self.fromdocname = need["docname"]
         else:
             self.fromdocname = fromdocname
 
         # For ReadTheDocs Theme we need to add 'rtd-exclude-wy-table'.
-        classes = ["need", "needs_grid_" + self.layout["grid"], "needs_layout_" + self.layout_name]
+        classes = [
+            "need",
+            "needs_grid_" + self.layout["grid"],
+            "needs_layout_" + self.layout_name,
+        ]
         classes.extend(self.needs_config.table_classes)
 
         self.style = style or self.need["style"] or self.needs_config.default_style
 
         if self.style:
             for style in self.style.strip().split(","):
                 style = style.strip()
@@ -234,84 +256,148 @@
 
         self.node_table = nodes.table(classes=classes, ids=[self.need["id"]])
         self.node_tbody = nodes.tbody()
 
         self.grids = {
             "simple": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [100], "side_left": False, "side_right": False, "footer": False},
+                "configs": {
+                    "colwidths": [100],
+                    "side_left": False,
+                    "side_right": False,
+                    "footer": False,
+                },
             },
             "simple_footer": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [100], "side_left": False, "side_right": False, "footer": True},
+                "configs": {
+                    "colwidths": [100],
+                    "side_left": False,
+                    "side_right": False,
+                    "footer": True,
+                },
             },
             "simple_side_left": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [30, 70], "side_left": "full", "side_right": False, "footer": False},
+                "configs": {
+                    "colwidths": [30, 70],
+                    "side_left": "full",
+                    "side_right": False,
+                    "footer": False,
+                },
             },
             "simple_side_right": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [70, 30], "side_left": False, "side_right": "full", "footer": False},
+                "configs": {
+                    "colwidths": [70, 30],
+                    "side_left": False,
+                    "side_right": "full",
+                    "footer": False,
+                },
             },
             "simple_side_left_partial": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [20, 80], "side_left": "part", "side_right": False, "footer": False},
+                "configs": {
+                    "colwidths": [20, 80],
+                    "side_left": "part",
+                    "side_right": False,
+                    "footer": False,
+                },
             },
             "simple_side_right_partial": {
                 "func": self._grid_simple,
-                "configs": {"colwidths": [80, 20], "side_left": False, "side_right": "part", "footer": False},
+                "configs": {
+                    "colwidths": [80, 20],
+                    "side_left": False,
+                    "side_right": "part",
+                    "footer": False,
+                },
             },
             "complex": self._grid_complex,
             "content": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [100], "side_left": False, "side_right": False, "footer": False},
+                "configs": {
+                    "colwidths": [100],
+                    "side_left": False,
+                    "side_right": False,
+                    "footer": False,
+                },
             },
             "content_footer": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [100], "side_left": False, "side_right": False, "footer": True},
+                "configs": {
+                    "colwidths": [100],
+                    "side_left": False,
+                    "side_right": False,
+                    "footer": True,
+                },
             },
             "content_side_left": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [5, 95], "side_left": True, "side_right": False, "footer": False},
+                "configs": {
+                    "colwidths": [5, 95],
+                    "side_left": True,
+                    "side_right": False,
+                    "footer": False,
+                },
             },
             "content_side_right": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [95, 5], "side_left": False, "side_right": True, "footer": False},
+                "configs": {
+                    "colwidths": [95, 5],
+                    "side_left": False,
+                    "side_right": True,
+                    "footer": False,
+                },
             },
             "content_footer_side_left": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [5, 95], "side_left": True, "side_right": False, "footer": True},
+                "configs": {
+                    "colwidths": [5, 95],
+                    "side_left": True,
+                    "side_right": False,
+                    "footer": True,
+                },
             },
             "content_footer_side_right": {
                 "func": self._grid_content,
-                "configs": {"colwidths": [95, 5], "side_left": False, "side_right": True, "footer": True},
+                "configs": {
+                    "colwidths": [95, 5],
+                    "side_left": False,
+                    "side_right": True,
+                    "footer": True,
+                },
             },
         }
 
         # Dummy Document setup
         self.doc_settings, self.inline_parser = _generate_inline_parser()
         self.dummy_doc = new_document("dummy", self.doc_settings)
-        self.doc_language = languages.get_language(self.dummy_doc.settings.language_code)
+        self.doc_language = languages.get_language(
+            self.dummy_doc.settings.language_code
+        )
         self.doc_memo = Struct(
             document=self.dummy_doc,
             reporter=self.dummy_doc.reporter,
             language=self.doc_language,
             title_styles=[],
             section_level=0,
             section_bubble_up_kludge=False,
             inliner=None,
         )
 
-        self.functions: Dict[str, Callable[..., Union[None, nodes.Node, List[nodes.Node]]]] = {
-            "meta": self.meta,
+        self.functions: dict[
+            str, Callable[..., None | nodes.Node | list[nodes.Node]]
+        ] = {
+            "meta": self.meta,  # type: ignore[dict-item]
             "meta_all": self.meta_all,
             "meta_links": self.meta_links,
-            "meta_links_all": self.meta_links_all,
+            "meta_links_all": self.meta_links_all,  # type: ignore[dict-item]
             "meta_id": self.meta_id,
-            "image": self.image,
+            "image": self.image,  # type: ignore[dict-item]
             "link": self.link,
             "collapse_button": self.collapse_button,
             "permalink": self.permalink,
         }
 
         # Prepare string_links dict, so that regex and templates get not recompiled too often.
         #
@@ -327,73 +413,77 @@
                 "options": link_conf["options"],
                 "name": link_name,
             }
 
     def get_need_table(self) -> nodes.table:
         if self.layout["grid"] not in self.grids.keys():
             raise SphinxNeedLayoutException(
-                "Unknown layout-grid: {}. Supported are {}".format(self.layout["grid"], ", ".join(self.grids.keys()))
+                "Unknown layout-grid: {}. Supported are {}".format(
+                    self.layout["grid"], ", ".join(self.grids.keys())
+                )
             )
 
         func = self.grids[self.layout["grid"]]
         if callable(func):
             func()
         else:
             func["func"](**func["configs"])  # type: ignore[index]
 
         return self.node_table
 
-    def get_section(self, section: str) -> Optional[nodes.line_block]:
+    def get_section(self, section: str) -> nodes.line_block | list[nodes.Element]:
         try:
             lines = self.layout["layout"][section]
         except KeyError:
             # Return nothing, if not specific configuration is given for layout section
-            return None
+            return []
 
         # Needed for PDF/Latex output, where empty line_blocks raise exceptions during build
         if len(lines) == 0:
-            return None
+            return []
 
         lines_container = nodes.line_block(classes=[f"needs_{section}"])
 
         for line in lines:
             # line_block_node = nodes.line_block()
             line_node = nodes.line()
 
             line_parsed = self._parse(line)
             line_ready = self._func_replace(line_parsed)
             line_node += line_ready
             lines_container.append(line_node)
 
         return lines_container
 
-    def _parse(self, line: str) -> List[nodes.Node]:
+    def _parse(self, line: str) -> list[nodes.Node]:
         """
         Parses a single line/string for inline rst statements, like strong, emphasis, literal, ...
 
         :param line: string to parse
         :return: nodes
         """
-        result, message = self.inline_parser.parse(line, 0, self.doc_memo, self.dummy_doc)  # type: ignore
+        result, message = self.inline_parser.parse(  # type: ignore
+            line, 0, self.doc_memo, self.dummy_doc
+        )
         if message:
             raise SphinxNeedLayoutException(message)
         return result  # type: ignore[no-any-return]
 
-    def _func_replace(self, section_nodes: List[nodes.Node]) -> List[nodes.Node]:
+    def _func_replace(self, section_nodes: list[nodes.Node]) -> list[nodes.Node]:
         """
         Replaces a function definition like ``<<meta(a, ,b)>>`` with the related docutils nodes.
 
         It takes an already existing docutils-node-tree and searches for Text-nodes containing ``<<..>>``.
         These nodes get then replaced by the return value (also a node) from the related function.
 
         :param section_nodes: docutils node (tree)
         :return: docutils nodes
         """
         return_nodes = []
-        result: Union[None, nodes.Node, List[nodes.Node]]
+        result: None | nodes.Node | list[nodes.Node]
         for node in section_nodes:
             if not isinstance(node, nodes.Text):
                 for child in node.children:
                     new_child = self._func_replace([child])
                     node.replace(child, new_child)  # type: ignore[attr-defined]
                 return_nodes.append(node)
             else:
@@ -413,15 +503,17 @@
                     # Check if function_definition was detected
                     elif len(text) == 0 and len(func_def) > 1:
                         from sphinx_needs.functions.functions import (
                             _analyze_func_string,
                         )
 
                         func_def_clean = func_def.replace("<<", "").replace(">>", "")
-                        func_name, func_args, func_kargs = _analyze_func_string(func_def_clean, None)
+                        func_name, func_args, func_kargs = _analyze_func_string(
+                            func_def_clean, None
+                        )
 
                         # Replace place holders
                         # Looks for {{name}}, where name must be an option of need, and replaces it with the
                         # related need content
                         for index, arg in enumerate(func_args):
                             # If argument is not a string, nothing to replace
                             # (replacement in string-lists is not supported)
@@ -477,15 +569,17 @@
                 raise SphinxNeedLayoutException(item)
             # To escape { we need to use 2 of them.
             # So {{ becomes {{{{
             replace_string = f"{{{{{item}}}}}"
             data = data.replace(replace_string, self.need[item])  # type: ignore[literal-required]
         return data
 
-    def meta(self, name: str, prefix: Optional[str] = None, show_empty: bool = False) -> nodes.inline:
+    def meta(
+        self, name: str, prefix: str | None = None, show_empty: bool = False
+    ) -> nodes.inline | list[nodes.Element]:
         """
         Returns the specific metadata of a need inside docutils nodes.
         Usage::
 
             <<meta('status', prefix='\\*\\*status\\*\\*: ', show_empty=True)>>
 
         .. note::
@@ -513,19 +607,19 @@
         elif data is None and show_empty:
             data = ""
 
         if isinstance(data, str):
             if len(data) == 0 and not show_empty:
                 return []
 
-            needs_string_links_option: List[str] = []
+            needs_string_links_option: list[str] = []
             for v in self.needs_config.string_links.values():
                 needs_string_links_option.extend(v["options"])
 
-            data_list: List[str] = (
+            data_list: list[str] = (
                 [i.strip() for i in re.split(r",|;", data) if len(i) != 0]
                 if name in needs_string_links_option
                 else [data]
             )
 
             matching_link_confs = []
             for link_conf in self.string_links.values():
@@ -543,15 +637,17 @@
                         render_context=self.needs_config.render_context,
                     )
                 else:
                     # Normal text handling
                     ref_item = nodes.Text(datum)
                     data_node += ref_item
 
-                if (name in needs_string_links_option and index + 1 < len(data)) or index + 1 < len([data]):
+                if (
+                    name in needs_string_links_option and index + 1 < len(data)
+                ) or index + 1 < len([data]):
                     data_node += nodes.emphasis("; ", "; ")
 
             data_container.append(data_node)
 
         elif isinstance(data, list):
             if len(data) == 0 and not show_empty:
                 return []
@@ -582,41 +678,41 @@
         :return: docutils node
         """
         from sphinx.util.nodes import make_refnode
 
         id_container = nodes.inline(classes=["needs-id"])
 
         nodes_id_text = nodes.Text(self.need["id"])
-        id_ref = make_refnode(
-            self.app.builder,
-            # fromdocname=self.need['docname'],
-            fromdocname=self.fromdocname,
-            todocname=self.need["docname"],
-            targetid=self.need["id"],
-            child=nodes_id_text.deepcopy(),
-            title=self.need["id"],
-        )
-        id_container += id_ref
+        if self.fromdocname and (_docname := self.need["docname"]):
+            id_ref = make_refnode(
+                self.app.builder,
+                fromdocname=self.fromdocname,
+                todocname=_docname,
+                targetid=self.need["id"],
+                child=nodes_id_text.deepcopy(),
+                title=self.need["id"],
+            )
+            id_container += id_ref
         return id_container
 
     def meta_all(
         self,
         prefix: str = "",
         postfix: str = "",
-        exclude: Optional[List[str]] = None,
+        exclude: list[str] | None = None,
         no_links: bool = False,
         defaults: bool = True,
         show_empty: bool = False,
     ) -> nodes.inline:
         """
         ``meta_all()`` excludes by default the output of: ``docname``, ``lineno``, ``refid``,
         ``content``, ``collapse``, ``parts``, ``id_parent``,
         ``id_complete``, ``title``, ``full_title``, ``is_part``, ``is_need``,
         ``type_prefix``, ``type_color``, ``type_style``, ``type``, ``type_name``, ``id``,
-        ``hide``, ``hide_status``, ``hide_tags``, ``sections``, ``section_name``.
+        ``hide``, ``sections``, ``section_name``.
 
         To exclude further need-data, use ``exclude``, like ``exclude=['status', 'tags']``
 
         To exclude nothing, set ``defaults`` to ``False``.
 
         Usage::
 
@@ -631,15 +727,15 @@
         :param exclude: List of value names, which are excluded from output
         :param no_links: excludes all incoming and outgoing extra link types from output
         :param defaults: If True, default excludes are added. This filters out all internal data, which is normally not
                          relevant for the user.
         :param show_empty: If true, also need data with no value will be printed. Mostly useful for debugging.
         :return: docutils nodes
         """
-        default_excludes = INTERNALS.copy()
+        default_excludes = list(INTERNALS)
 
         if exclude is None or not isinstance(exclude, list):
             if defaults:
                 exclude = default_excludes
             else:
                 exclude = []
         elif defaults:
@@ -685,82 +781,97 @@
         #     link_name = self.config.extra_links[name]['incoming']
         # else:
         #     link_name = self.config.extra_links[name]['outgoing']
 
         from sphinx_needs.roles.need_incoming import NeedIncoming
         from sphinx_needs.roles.need_outgoing import NeedOutgoing
 
-        if incoming:
-            node_links = NeedIncoming(reftarget=self.need["id"], link_type=f"{name}_back")
-        else:
-            node_links = NeedOutgoing(reftarget=self.need["id"], link_type=f"{name}")
+        node_links = (
+            NeedIncoming(reftarget=self.need["id"], link_type=f"{name}_back")
+            if incoming
+            else NeedOutgoing(reftarget=self.need["id"], link_type=f"{name}")
+        )
         node_links.append(nodes.inline(self.need["id"], self.need["id"]))
         data_container.append(node_links)
         return data_container
 
     def meta_links_all(
-        self, prefix: str = "", postfix: str = "", exclude: Optional[List[str]] = None
-    ) -> List[nodes.line]:
+        self, prefix: str = "", postfix: str = "", exclude: list[str] | None = None
+    ) -> list[nodes.line]:
         """
         Documents all used link types for the current need automatically.
 
         :param prefix:  prefix string
         :param postfix:  postfix string
         :param exclude:  list of extra link type names, which are excluded from output
         :return: docutils nodes
         """
         exclude = exclude or []
         data_container = []
         for link_type in self.needs_config.extra_links:
             type_key = link_type["option"]
             if self.need[type_key] and type_key not in exclude:  # type: ignore[literal-required]
                 outgoing_line = nodes.line()
-                outgoing_label = prefix + "{}:".format(link_type["outgoing"]) + postfix + " "
+                outgoing_label = (
+                    prefix + "{}:".format(link_type["outgoing"]) + postfix + " "
+                )
                 outgoing_line += self._parse(outgoing_label)
                 outgoing_line += self.meta_links(link_type["option"], incoming=False)
                 data_container.append(outgoing_line)
 
             type_key = link_type["option"] + "_back"
             if self.need[type_key] and type_key not in exclude:  # type: ignore[literal-required]
                 incoming_line = nodes.line()
-                incoming_label = prefix + "{}:".format(link_type["incoming"]) + postfix + " "
+                incoming_label = (
+                    prefix + "{}:".format(link_type["incoming"]) + postfix + " "
+                )
                 incoming_line += self._parse(incoming_label)
                 incoming_line += self.meta_links(link_type["option"], incoming=True)
                 data_container.append(incoming_line)
 
         return data_container
 
     def image(
         self,
         url: str,
-        height: Optional[str] = None,
-        width: Optional[str] = None,
-        align: Optional[str] = None,
+        height: str | None = None,
+        width: str | None = None,
+        align: str | None = None,
         no_link: bool = False,
         prefix: str = "",
         is_external: bool = False,
         img_class: str = "",
-    ) -> nodes.inline:
+    ) -> nodes.inline | list[nodes.Element]:
         """
         See https://docutils.sourceforge.io/docs/ref/rst/directives.html#images
 
-        If url starts with ``icon:`` the following string is taken is icon-name and the related icon is shown.
+        If **url** starts with ``icon:`` the following string is taken as icon-name and the related icon is shown.
         Example: ``icon:activity`` will show:
 
         .. image:: _static/activity.png
 
         For all icons, see https://feathericons.com/.
 
         Examples::
 
             '<<image("_images/useblocks_logo.png", height="50px", align="center")>>',
             '<<image("icon:bell", height="20px", align="center")>>'
             '<<image("field:url", height="60px", align="center")>>'  # Get url from need['url']
 
-        :param url:
+        If **url** starts with ``:field`` the URL value is taken from the defined field of the current need
+        object.
+
+        .. hint:: Relative URLs
+
+           If a relative path for the URL parameter is given, it must be relative to the documentation
+           root folder and not relative to the current need location, for which it gets executed.
+
+           Example: ``<<image("_static/picture.png")>>``,
+
+        :param url: Relative path to the project folder or an absolute path
         :param height:
         :param width:
         :param align:
         :param no_link:
         :param prefix: Prefix string in front of the image
         :param is_external: If ``True`` url references an external image, which needs to be downloaded
         :param img_class: Custom class name for image element
@@ -783,15 +894,17 @@
             options["height"] = height
         if width:
             options["width"] = width
         if align:
             options["align"] = align
 
         if url is None or not isinstance(url, str):
-            raise SphinxNeedLayoutException("not valid url given for image function in layout")
+            raise SphinxNeedLayoutException(
+                "not valid url given for image function in layout"
+            )
 
         if url.startswith("icon:"):
             if any(x in builder.name.upper() for x in ["PDF", "LATEX"]):
                 # latexpdf can't handle svg files. We not to use the png format here.
                 builder_extension = "png"
             else:
                 builder_extension = "svg"
@@ -820,18 +933,14 @@
                 value = ""
 
             if value is None or len(value) == 0:
                 return []
 
             url = value
 
-            if not is_external and not os.path.isabs(url):
-                subfolder_amount = self.need["docname"].count("/")
-                url = "../" * subfolder_amount + url
-
         if is_external:
             url_parsed = urlparse(url)
             filename = os.path.basename(url_parsed.path) + ".png"
             path = os.path.join(self.app.srcdir, "images")
             file_path = os.path.join(path, filename)
 
             # Download only, if file not downloaded yet
@@ -859,26 +968,27 @@
         image_node["candidates"] = {"*": url}
         # image_node['candidates'] = '*'
         image_node["uri"] = url
 
         # Sphinx voodoo needed here.
         # It is not enough to just add a doctuils nodes.image, we also have to register the imag location for sphinx
         # Otherwise the images gets not copied to the later build-output location
-        env.images.add_file(self.need["docname"], url)
+        if _docname := self.need["docname"]:
+            env.images.add_file(_docname, url)
 
         data_container.append(image_node)
         return data_container
 
     def link(
         self,
         url: str,
-        text: Optional[str] = None,
-        image_url: Optional[str] = None,
-        image_height: Optional[str] = None,
-        image_width: Optional[str] = None,
+        text: str | None = None,
+        image_url: str | None = None,
+        image_height: str | None = None,
+        image_width: str | None = None,
         prefix: str = "",
         is_dynamic: bool = False,
     ) -> nodes.inline:
         """
         Shows a link.
         Link can be a text, an image or both
 
@@ -918,16 +1028,20 @@
             link_node.append(image_node)
 
         data_container.append(link_node)
 
         return data_container
 
     def collapse_button(
-        self, target: str = "meta", collapsed: str = "Show", visible: str = "Close", initial: bool = False
-    ) -> Optional[nodes.inline]:
+        self,
+        target: str = "meta",
+        collapsed: str = "Show",
+        visible: str = "Close",
+        initial: bool = False,
+    ) -> nodes.inline | None:
         """
         To show icons instead of text on the button, use collapse_button() like this::
 
             <<collapse_button("icon:arrow-down-circle", visible="icon:arrow-right-circle", initial=False)>>
 
         For the builders ``latex`` and ``latexpdf`` no output is returned, as their build results are really static
         and collapse-feature can not be implemented..
@@ -944,35 +1058,49 @@
             return None
 
         coll_node_collapsed = nodes.inline(classes=["needs", "collapsed"])
         coll_node_visible = nodes.inline(classes=["needs", "visible"])
 
         if collapsed.startswith("image:") or collapsed.startswith("icon:"):
             coll_node_collapsed.append(
-                self.image(collapsed.replace("image:", ""), width="17px", no_link=True, img_class="sn_collapse_img")
+                self.image(
+                    collapsed.replace("image:", ""),
+                    width="17px",
+                    no_link=True,
+                    img_class="sn_collapse_img",
+                )
             )
         elif collapsed.startswith("Debug view"):
-            coll_node_collapsed.append(nodes.container(classes=["debug_on_layout_btn"]))  # For debug layout
+            coll_node_collapsed.append(
+                nodes.container(classes=["debug_on_layout_btn"])
+            )  # For debug layout
         else:
             coll_node_collapsed.append(nodes.Text(collapsed))
 
         if visible.startswith("image:") or visible.startswith("icon:"):
             coll_node_visible.append(
-                self.image(visible.replace("image:", ""), width="17px", no_link=True, img_class="sn_collapse_img")
+                self.image(
+                    visible.replace("image:", ""),
+                    width="17px",
+                    no_link=True,
+                    img_class="sn_collapse_img",
+                )
             )
         elif visible.startswith("Debug view"):
             coll_node_visible.append(nodes.container(classes=["debug_off_layout_btn"]))
         else:
             coll_node_visible.append(nodes.Text(visible))
 
         coll_container = nodes.inline(classes=["needs", "needs_collapse"])
         # docutils doesn't allow has to add any html-attributes beside class and id to nodes.
         # So we misused "id" for this and use "__" (2x _) as separator for row-target names
 
-        if (not self.need["collapse"]) or (self.need["collapse"] is None and not initial):
+        if (not self.need["collapse"]) or (
+            self.need["collapse"] is None and not initial
+        ):
             status = "show"
 
         if (self.need["collapse"]) or (not self.need["collapse"] and initial):
             status = "hide"
 
         target_strings = target.split(",")
         final_targets = [x.strip() for x in target_strings]
@@ -981,18 +1109,18 @@
         coll_container.append(coll_node_collapsed)
         coll_container.append(coll_node_visible)
 
         return coll_container
 
     def permalink(
         self,
-        image_url: Optional[str] = None,
-        image_height: Optional[str] = None,
-        image_width: Optional[str] = None,
-        text: Optional[str] = None,
+        image_url: str | None = None,
+        image_height: str | None = None,
+        image_width: str | None = None,
+        text: str | None = None,
         prefix: str = "",
     ) -> nodes.inline:
         """
         Shows a permanent link to the need.
         Link can be a text, an image or both
 
         :param image_url: image for an image link
@@ -1011,31 +1139,35 @@
 
         if image_url is None and text is None:
             image_url = "icon:share-2"
             image_width = "17px"
 
         permalink = self.needs_config.permalink_file
         id = self.need["id"]
-        docname = self.need["docname"]
         permalink_url = ""
-        for _ in range(0, len(docname.split("/")) - 1):
-            permalink_url += "../"
+        if docname := self.need["docname"]:
+            for _ in range(0, len(docname.split("/")) - 1):
+                permalink_url += "../"
         permalink_url += permalink + "?id=" + id
 
         return self.link(
             url=permalink_url,
             text=text,
             image_url=image_url,
             image_width=image_width,
             image_height=image_height,
             prefix=prefix,
         )
 
     def _grid_simple(
-        self, colwidths: List[int], side_left: Union[bool, str], side_right: Union[bool, str], footer: bool
+        self,
+        colwidths: list[int],
+        side_left: bool | str,
+        side_right: bool | str,
+        footer: bool,
     ) -> None:
         """
         Creates most "simple" grid layouts.
         Side parts and footer can be activated via config.
 
         .. code-block:: text
 
@@ -1098,43 +1230,51 @@
             node_colspec = nodes.colspec(colwidth=width)
             node_tgroup += node_colspec
 
         # HEAD row
         head_row = nodes.row(classes=["need", "head"])
 
         if side_left:
-            side_entry = nodes.entry(classes=["need", "side"], morerows=side_left_morerows)
+            side_entry = nodes.entry(
+                classes=["need", "side"], morerows=side_left_morerows
+            )
             side_entry += self.get_section("side")
             head_row += side_entry
 
         head_entry = nodes.entry(classes=["need", "head"])
         head_entry += self.get_section("head")
         head_row += head_entry
 
         if side_right:
-            side_entry = nodes.entry(classes=["need", "side"], morerows=side_right_morerows)
+            side_entry = nodes.entry(
+                classes=["need", "side"], morerows=side_right_morerows
+            )
             side_entry += self.get_section("side")
             head_row += side_entry
 
         # META row
         meta_row = nodes.row(classes=["need", "meta"])
         meta_entry = nodes.entry(classes=["need", "meta"])
         meta_entry += self.get_section("meta")
         meta_row += meta_entry
 
         # CONTENT row
         content_row = nodes.row(classes=["need", "content"])
-        content_entry = nodes.entry(classes=["need", "content"], morecols=common_more_cols)
+        content_entry = nodes.entry(
+            classes=["need", "content"], morecols=common_more_cols
+        )
         content_entry.insert(0, self.node.children)
         content_row += content_entry
 
         # FOOTER row
         if footer:
             footer_row = nodes.row(classes=["need", "footer"])
-            footer_entry = nodes.entry(classes=["need", "footer"], morecols=common_more_cols)
+            footer_entry = nodes.entry(
+                classes=["need", "footer"], morecols=common_more_cols
+            )
             footer_entry += self.get_section("footer")
             footer_row += footer_entry
 
         # Construct table
         self.node_tbody += head_row
         self.node_tbody += meta_row
         self.node_tbody += content_row
@@ -1201,15 +1341,17 @@
         footer_right_entry = nodes.entry(classes=["footer_right"], morecols=1)
         footer_right_entry += self.get_section("footer_right")
         footer_row += footer_right_entry
 
         # Construct table
         node_tgroup += self.node_tbody
 
-    def _grid_content(self, colwidths: List[int], side_left: bool, side_right: bool, footer: bool) -> None:
+    def _grid_content(
+        self, colwidths: list[int], side_left: bool, side_right: bool, footer: bool
+    ) -> None:
         """
         Creates most "content" based grid layouts.
         Side parts and footer can be activated via config.
 
         +------+---------+------+
         |      | Content |      |
         | Side +---------+ Side |
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/css/buttons.dataTables.min.css` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/css/buttons.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/css/mixins.scss` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/css/mixins.scss`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.colVis.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.flash.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.flash.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.print.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/buttons.print.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/js/dataTables.buttons.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Buttons-1.5.1/swf/flashExport.swf` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Buttons-1.5.1/swf/flashExport.swf`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/ColReorder-1.4.1/js/dataTables.colReorder.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/ColReorder-1.4.1/js/dataTables.colReorder.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/css/jquery.dataTables.min.css` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/DataTables-1.10.16/js/jquery.dataTables.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/DataTables-1.10.16/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedColumns-3.2.4/js/dataTables.fixedColumns.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedColumns-3.2.4/js/dataTables.fixedColumns.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/FixedHeader-3.1.3/js/dataTables.fixedHeader.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/FixedHeader-3.1.3/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/JSZip-2.5.0/jszip.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/JSZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Responsive-2.2.1/css/responsive.dataTables.min.css` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Responsive-2.2.1/css/responsive.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Responsive-2.2.1/js/dataTables.responsive.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Responsive-2.2.1/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/Scroller-1.4.4/js/dataTables.scroller.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/Scroller-1.4.4/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/datatables.min.css` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/datatables.min.css`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/datatables.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/datatables.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/pdfmake-0.1.32/pdfmake.min.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/pdfmake-0.1.32/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/pdfmake-0.1.32/vfs_fonts.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/pdfmake-0.1.32/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/libs/html/sphinx_needs_collapse.js` & `sphinx_needs-2.1.0/sphinx_needs/libs/html/sphinx_needs_collapse.js`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/need_constraints.py` & `sphinx_needs-2.1.0/sphinx_needs/need_constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import Dict
+from __future__ import annotations
 
 import jinja2
 
 from sphinx_needs.api.exceptions import NeedsConstraintFailed, NeedsConstraintNotAllowed
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType
 from sphinx_needs.filter_common import filter_single_need
 from sphinx_needs.logging import get_logger
 
 logger = get_logger(__name__)
 
 
-def process_constraints(needs: Dict[str, NeedsInfoType], config: NeedsSphinxConfig) -> None:
+def process_constraints(
+    needs: dict[str, NeedsInfoType], config: NeedsSphinxConfig
+) -> None:
     """Analyse constraints of all needs,
     and set corresponding fields on the need data item:
     ``constraints_passed`` and ``constraints_results``.
 
     The ``style`` field may also be changed, if a constraint fails
     (depending on the config value ``constraint_failed_options``)
     """
     config_constraints = config.constraints
 
-    error_templates_cache: Dict[str, jinja2.Template] = {}
+    error_templates_cache: dict[str, jinja2.Template] = {}
 
     for need in needs.values():
         need_id = need["id"]
         constraints = need["constraints"]
 
         # flag that is set to False if any check fails
         need["constraints_passed"] = True
@@ -52,15 +54,17 @@
                     need["constraints_results"].setdefault(constraint, {})[name] = True
                 else:
                     need["constraints_results"].setdefault(constraint, {})[name] = False
                     need["constraints_passed"] = False
 
                     if "error_message" in executable_constraints:
                         msg = str(executable_constraints["error_message"])
-                        template = error_templates_cache.setdefault(msg, jinja2.Template(msg))
+                        template = error_templates_cache.setdefault(
+                            msg, jinja2.Template(msg)
+                        )
                         need["constraints_error"] = template.render(**need)
 
                     if "severity" not in executable_constraints:
                         raise NeedsConstraintFailed(
                             f"'severity' key not set for constraint {constraint!r} in config 'needs_constraints'"
                         )
                     severity = executable_constraints["severity"]
@@ -84,17 +88,21 @@
                             f"FAILED a breaking constraint: >> {cmd} << for need "
                             f"{need_id} FAILED! breaking build process"
                         )
 
                     # set styles
                     old_style = need["style"]
                     if old_style and len(old_style) > 0:
-                        new_styles = "".join(", " + x for x in failed_options.get("style", []))
+                        new_styles = "".join(
+                            ", " + x for x in failed_options.get("style", [])
+                        )
                     else:
                         old_style = ""
-                        new_styles = "".join(x + "," for x in failed_options.get("style", []))
+                        new_styles = "".join(
+                            x + "," for x in failed_options.get("style", [])
+                        )
 
                     if failed_options.get("force_style", False):
                         need["style"] = new_styles.strip(", ")
                     else:
                         constraint_failed_style = old_style + new_styles
                         need["style"] = constraint_failed_style
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/needs.py` & `sphinx_needs-2.1.0/sphinx_needs/needs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from timeit import default_timer as timer  # Used for timing measurements
 from typing import Any, Callable, Dict, List, Type
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.config import Config
@@ -13,15 +15,15 @@
     NeedsBuilder,
     NeedsIdBuilder,
     NeedumlsBuilder,
     build_needs_id_json,
     build_needs_json,
     build_needumls_pumls,
 )
-from sphinx_needs.config import NEEDS_CONFIG, NeedsSphinxConfig
+from sphinx_needs.config import NEEDS_CONFIG, LinkOptionsType, NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData, merge_data
 from sphinx_needs.defaults import (
     LAYOUTS,
     NEED_DEFAULT_OPTIONS,
     NEEDEXTEND_NOT_ALLOWED_OPTIONS,
     NEEDFLOW_CONFIG_DEFAULTS,
 )
@@ -100,18 +102,21 @@
 from sphinx_needs.roles.need_part import NeedPart, process_need_part
 from sphinx_needs.roles.need_ref import NeedRef, process_need_ref
 from sphinx_needs.services.github import GithubService
 from sphinx_needs.services.open_needs import OpenNeedsService
 from sphinx_needs.utils import INTERNALS, NEEDS_FUNCTIONS, node_match
 from sphinx_needs.warnings import process_warnings
 
-__version__ = VERSION = "2.0.0"
+__version__ = VERSION = "2.1.0"
 NEEDS_FUNCTIONS.clear()
 
-_NODE_TYPES_T = Dict[Type[nodes.Element], Callable[[Sphinx, nodes.document, str, List[nodes.Element]], None]]
+_NODE_TYPES_T = Dict[
+    Type[nodes.Element],
+    Callable[[Sphinx, nodes.document, str, List[nodes.Element]], None],
+]
 
 NODE_TYPES_PRIO: _NODE_TYPES_T = {  # Node types to be checked before most others
     Needextract: process_needextract,
 }
 
 NODE_TYPES: _NODE_TYPES_T = {
     Needbar: process_needbar,
@@ -128,30 +133,33 @@
     NeedRef: process_need_ref,
     NeedIncoming: process_need_incoming,
     NeedOutgoing: process_need_outgoing,
     NeedCount: process_need_count,
     NeedFunc: process_need_func,
 }
 
+LOGGER = get_logger(__name__)
+
 
-def setup(app: Sphinx) -> Dict[str, Any]:
-    log = get_logger(__name__)
-    log.debug("Starting setup of Sphinx-Needs")
-    log.debug("Load Sphinx-Data-Viewer for Sphinx-Needs")
+def setup(app: Sphinx) -> dict[str, Any]:
+    LOGGER.debug("Starting setup of Sphinx-Needs")
+    LOGGER.debug("Load Sphinx-Data-Viewer for Sphinx-Needs")
     app.setup_extension("sphinx_data_viewer")
     app.setup_extension("sphinxcontrib.jquery")
 
     app.add_builder(NeedsBuilder)
     app.add_builder(NeedumlsBuilder)
     app.add_builder(NeedsIdBuilder)
 
     NeedsSphinxConfig.add_config_values(app)
 
     # Define nodes
-    app.add_node(Need, html=(html_visit, html_depart), latex=(latex_visit, latex_depart))
+    app.add_node(
+        Need, html=(html_visit, html_depart), latex=(latex_visit, latex_depart)
+    )
     app.add_node(
         Needfilter,
     )
     app.add_node(Needbar)
     app.add_node(Needimport)
     app.add_node(Needlist)
     app.add_node(Needtable)
@@ -160,15 +168,19 @@
     app.add_node(Needsequence)
     app.add_node(Needgantt)
     app.add_node(Needextract)
     app.add_node(Needservice)
     app.add_node(Needextend)
     app.add_node(Needuml)
     app.add_node(List2Need)
-    app.add_node(NeedPart, html=(visitor_dummy, visitor_dummy), latex=(visitor_dummy, visitor_dummy))
+    app.add_node(
+        NeedPart,
+        html=(visitor_dummy, visitor_dummy),
+        latex=(visitor_dummy, visitor_dummy),
+    )
 
     ########################################################################
     # DIRECTIVES
     ########################################################################
 
     # Define directives
     app.add_directive("needbar", NeedbarDirective)
@@ -188,31 +200,62 @@
     app.add_directive("needarch", NeedarchDirective)
     app.add_directive("list2need", List2NeedDirective)
 
     ########################################################################
     # ROLES
     ########################################################################
     # Provides :need:`ABC_123` for inline links.
-    app.add_role("need", NeedsXRefRole(nodeclass=NeedRef, innernodeclass=nodes.emphasis, warn_dangling=True))
+    app.add_role(
+        "need",
+        NeedsXRefRole(
+            nodeclass=NeedRef, innernodeclass=nodes.emphasis, warn_dangling=True
+        ),
+    )
 
     app.add_role(
-        "need_incoming", NeedsXRefRole(nodeclass=NeedIncoming, innernodeclass=nodes.emphasis, warn_dangling=True)
+        "need_incoming",
+        NeedsXRefRole(
+            nodeclass=NeedIncoming, innernodeclass=nodes.emphasis, warn_dangling=True
+        ),
     )
 
     app.add_role(
-        "need_outgoing", NeedsXRefRole(nodeclass=NeedOutgoing, innernodeclass=nodes.emphasis, warn_dangling=True)
+        "need_outgoing",
+        NeedsXRefRole(
+            nodeclass=NeedOutgoing, innernodeclass=nodes.emphasis, warn_dangling=True
+        ),
     )
 
-    app.add_role("need_part", NeedsXRefRole(nodeclass=NeedPart, innernodeclass=nodes.inline, warn_dangling=True))
+    app.add_role(
+        "need_part",
+        NeedsXRefRole(
+            nodeclass=NeedPart, innernodeclass=nodes.inline, warn_dangling=True
+        ),
+    )
     # Shortcut for need_part
-    app.add_role("np", NeedsXRefRole(nodeclass=NeedPart, innernodeclass=nodes.inline, warn_dangling=True))
+    app.add_role(
+        "np",
+        NeedsXRefRole(
+            nodeclass=NeedPart, innernodeclass=nodes.inline, warn_dangling=True
+        ),
+    )
 
-    app.add_role("need_count", NeedsXRefRole(nodeclass=NeedCount, innernodeclass=nodes.inline, warn_dangling=True))
+    app.add_role(
+        "need_count",
+        NeedsXRefRole(
+            nodeclass=NeedCount, innernodeclass=nodes.inline, warn_dangling=True
+        ),
+    )
 
-    app.add_role("need_func", NeedsXRefRole(nodeclass=NeedFunc, innernodeclass=nodes.inline, warn_dangling=True))
+    app.add_role(
+        "need_func",
+        NeedsXRefRole(
+            nodeclass=NeedFunc, innernodeclass=nodes.inline, warn_dangling=True
+        ),
+    )
 
     ########################################################################
     # EVENTS
     ########################################################################
     # Make connections to events
     app.connect("config-inited", load_config)
     app.connect("config-inited", check_configuration)
@@ -234,15 +277,19 @@
     # There is also the event doctree-read.
     # But it looks like in this event no references are already solved, which
     # makes trouble in our code.
     # However, some sphinx-internal actions (like image collection) are already called during
     # doctree-read. So manipulating the doctree may result in conflicts, as e.g. images get not
     # registered for sphinx. So some sphinx-internal tasks/functions may be called by hand again...
     # See also https://github.com/sphinx-doc/sphinx/issues/7054#issuecomment-578019701 for an example
-    app.connect("doctree-resolved", process_creator(NODE_TYPES_PRIO, "needextract"), priority=100)
+    app.connect(
+        "doctree-resolved",
+        process_creator(NODE_TYPES_PRIO, "needextract"),
+        priority=100,
+    )
     app.connect("doctree-resolved", process_need_nodes)
     app.connect("doctree-resolved", process_creator(NODE_TYPES))
 
     app.connect("build-finished", process_warnings)
     app.connect("build-finished", build_needs_json)
     app.connect("build-finished", build_needs_id_json)
     app.connect("build-finished", build_needumls_pumls)
@@ -273,69 +320,80 @@
 
         Reason: In the past all process-xy handles have parsed the doctree by their own, so the same doctree
         got parsed several times. This is now done at a single place and the related process-xy get a
         list of found docutil node-object for their case.
         """
         # We only need to analyse docs, which have Sphinx-Needs directives in it.
         if (
-            fromdocname not in SphinxNeedsData(app.env).get_or_create_docs().get(doc_category, [])
+            fromdocname
+            not in SphinxNeedsData(app.env).get_or_create_docs().get(doc_category, [])
             and fromdocname != f"{app.config.root_doc}"
         ):
             return
-        current_nodes: Dict[Type[nodes.Element], List[nodes.Element]] = {}
+        current_nodes: dict[type[nodes.Element], list[nodes.Element]] = {}
         check_nodes = list(node_list.keys())
         for node_need in doctree.findall(node_match(check_nodes)):
             for check_node in node_list:
                 if isinstance(node_need, check_node):
                     if check_node not in current_nodes:
                         current_nodes[check_node] = []
                     current_nodes[check_node].append(node_need)
                     break  # We found the related type for the need
 
         # Let's call the handlers
         for check_node, check_func in node_list.items():
             # Call the handler only, if it defined, and we found some nodes for it
-            if check_node in current_nodes and check_func is not None and current_nodes[check_node]:
+            if (
+                check_node in current_nodes
+                and check_func is not None
+                and current_nodes[check_node]
+            ):
                 check_func(app, doctree, fromdocname, current_nodes[check_node])
 
     return process_caller
 
 
 def load_config(app: Sphinx, *_args: Any) -> None:
     """
     Register extra options and directive based on config from conf.py
     """
-    log = get_logger(__name__)
-
     needs_config = NeedsSphinxConfig(app.config)
 
     if isinstance(needs_config.extra_options, dict):
-        log.info(
+        LOGGER.info(
             'Config option "needs_extra_options" supports list and dict. However new default type since '
             "Sphinx-Needs 0.7.2 is list. Please see docs for details."
         )
 
-    extra_options = NEEDS_CONFIG.extra_options
     for option in needs_config.extra_options:
-        if option in extra_options:
-            log.warning(f'extra_option "{option}" already registered. [needs.config]', type="needs", subtype="config")
+        if option in NEEDS_CONFIG.extra_options:
+            LOGGER.warning(
+                f'extra_option "{option}" already registered. [needs.config]',
+                type="needs",
+                subtype="config",
+            )
         NEEDS_CONFIG.extra_options[option] = directives.unchanged
 
+    # ensure options for ``needgantt`` functionality are added to the extra options
+    for option in (needs_config.duration_option, needs_config.completion_option):
+        if option not in NEEDS_CONFIG.extra_options:
+            NEEDS_CONFIG.extra_options[option] = directives.unchanged_required
+
     # Get extra links and create a dictionary of needed options.
     extra_links_raw = needs_config.extra_links
     extra_links = {}
     for extra_link in extra_links_raw:
         extra_links[extra_link["option"]] = directives.unchanged
 
     title_optional = needs_config.title_optional
     title_from_content = needs_config.title_from_content
 
     # Update NeedDirective to use customized options
-    NeedDirective.option_spec.update(extra_options)
-    NeedserviceDirective.option_spec.update(extra_options)
+    NeedDirective.option_spec.update(NEEDS_CONFIG.extra_options)
+    NeedserviceDirective.option_spec.update(NEEDS_CONFIG.extra_options)
 
     # Update NeedDirective to use customized links
     NeedDirective.option_spec.update(extra_links)
     NeedserviceDirective.option_spec.update(extra_links)
 
     # Update NeedextendDirective with option modifiers.
     for key, value in NEED_DEFAULT_OPTIONS.items():
@@ -368,15 +426,15 @@
     NeedextendDirective.option_spec.update(
         {
             "links_back": NEED_DEFAULT_OPTIONS["links"],
             "+links_back": NEED_DEFAULT_OPTIONS["links"],
             "-links_back": directives.flag,
         }
     )
-    for key, value in extra_options.items():
+    for key, value in NEEDS_CONFIG.extra_options.items():
         NeedextendDirective.option_spec.update(
             {
                 key: value,
                 f"+{key}": value,
                 f"-{key}": directives.flag,
             }
         )
@@ -389,25 +447,34 @@
         # Register requested types of needs
         app.add_directive(t["directive"], NeedDirective)
 
     for name, check in needs_config.warnings.items():
         if name not in NEEDS_CONFIG.warnings:
             NEEDS_CONFIG.warnings[name] = check
         else:
-            log.warning(
-                f"{name!r} in 'needs_warnings' is already registered. [needs.config]", type="needs", subtype="config"
+            LOGGER.warning(
+                f"{name!r} in 'needs_warnings' is already registered. [needs.config]",
+                type="needs",
+                subtype="config",
             )
 
     if needs_config.constraints_failed_color:
-        log.warning(
+        LOGGER.warning(
             'Config option "needs_constraints_failed_color" is deprecated. Please use "needs_constraint_failed_options" styles instead. [needs.config]',
             type="needs",
             subtype="config",
         )
 
+    if needs_config.report_dead_links is not True:
+        LOGGER.warning(
+            'Config option "needs_constraints_failed_color" is deprecated. Please use `suppress_warnings = ["needs.link_outgoing"]` instead. [needs.config]',
+            type="needs",
+            subtype="config",
+        )
+
 
 def visitor_dummy(*_args: Any, **_kwargs: Any) -> None:
     """
     Dummy class for visitor methods, which does nothing.
     """
     pass
 
@@ -427,37 +494,35 @@
     services.register("github-issues", GithubService, gh_type="issue")
     services.register("github-prs", GithubService, gh_type="pr")
     services.register("github-commits", GithubService, gh_type="commit")
     services.register("open-needs", OpenNeedsService)
 
     # Register user defined services
     for name, service in needs_config.services.items():
-        if name not in services.services and "class" in service and "class_init" in service:
+        if (
+            name not in services.services
+            and "class" in service
+            and "class_init" in service
+        ):
             # We found a not yet registered service
             # But only register, if service-config contains class and class_init.
             # Otherwise, the service may get registered later by an external sphinx-needs extension
             services.register(name, service["class"], **service["class_init"])
 
     # Register built-in functions
     for need_common_func in NEEDS_COMMON_FUNCTIONS:
         register_func(need_common_func)
 
     # Register functions configured by user
     for needs_func in needs_config.functions:
         register_func(needs_func)
 
-    # Own extra options
-    for option in ["hidden", "duration", "completion", "has_dead_links", "has_forbidden_dead_links", "constraints"]:
-        # Check if not already set by user
-        if option not in NEEDS_CONFIG.extra_options:
-            NEEDS_CONFIG.extra_options[option] = directives.unchanged
-
     # The default link name. Must exist in all configurations. Therefore we set it here
     # for the user.
-    common_links = []
+    common_links: list[LinkOptionsType] = []
     link_types = needs_config.extra_links
     basic_link_type_found = False
     parent_needs_link_type_found = False
     for link_type in link_types:
         if link_type["option"] == "links":
             basic_link_type_found = True
         elif link_type["option"] == "parent_needs":
@@ -493,75 +558,79 @@
     # Set time measurement flag
     if needs_config.debug_measurement:
         debug.START_TIME = timer()  # Store the rough start time of Sphinx build
         debug.EXECUTE_TIME_MEASUREMENTS = True
 
 
 def check_configuration(_app: Sphinx, config: Config) -> None:
-    """
-    Checks the configuration for invalid options.
+    """Checks the configuration for invalid options.
 
     E.g. defined need-option, which is already defined internally
-
-    :param app:
-    :param config:
-    :return:
     """
-    extra_options = config["needs_extra_options"]
-    link_types = [x["option"] for x in config["needs_extra_links"]]
+    needs_config = NeedsSphinxConfig(config)
+    extra_options = needs_config.extra_options
+    link_types = [x["option"] for x in needs_config.extra_links]
 
-    external_filter = getattr(config, "needs_filter_data", {})
+    external_filter = needs_config.filter_data
     for extern_filter, value in external_filter.items():
         # Check if external filter values is really a string
         if not isinstance(value, str):
             raise NeedsConfigException(
                 f"External filter value: {value} from needs_filter_data {external_filter} is not a string."
             )
         # Check if needs external filter and extra option are using the same name
         if extern_filter in extra_options:
             raise NeedsConfigException(
-                "Same name for external filter and extra option: {}." " This is not allowed.".format(extern_filter)
+                f"Same name for external filter and extra option: {extern_filter}."
+                " This is not allowed."
             )
 
     # Check for usage of internal names
     for internal in INTERNALS:
         if internal in extra_options:
             raise NeedsConfigException(
-                'Extra option "{}" already used internally. ' " Please use another name.".format(internal)
+                f'Extra option "{internal}" already used internally. '
+                " Please use another name."
             )
         if internal in link_types:
             raise NeedsConfigException(
-                'Link type name "{}" already used internally. ' " Please use another name.".format(internal)
+                f'Link type name "{internal}" already used internally. '
+                " Please use another name."
             )
 
     # Check if option and link are using the same name
     for link in link_types:
         if link in extra_options:
             raise NeedsConfigException(
-                "Same name for link type and extra option: {}." " This is not allowed.".format(link)
+                f"Same name for link type and extra option: {link}."
+                " This is not allowed."
             )
         if link + "_back" in extra_options:
             raise NeedsConfigException(
                 "Same name for automatically created link type and extra option: {}."
                 " This is not allowed.".format(link + "_back")
             )
 
-    external_variants = getattr(config, "needs_variants", {})
-    external_variant_options = getattr(config, "needs_variant_options", [])
+    external_variants = needs_config.variants
+    external_variant_options = needs_config.variant_options
     for value in external_variants.values():
         # Check if external filter values is really a string
         if not isinstance(value, str):
             raise NeedsConfigException(
                 f"Variant filter value: {value} from needs_variants {external_variants} is not a string."
             )
 
     for option in external_variant_options:
         # Check variant option is added in either extra options or extra links or NEED_DEFAULT_OPTIONS
-        if option not in extra_options and option not in link_types and option not in NEED_DEFAULT_OPTIONS.keys():
+        if (
+            option not in extra_options
+            and option not in link_types
+            and option not in NEED_DEFAULT_OPTIONS.keys()
+        ):
             raise NeedsConfigException(
-                "Variant option `{}` is not added in either extra options or extra links. "
-                "This is not allowed.".format(option)
+                f"Variant option `{option}` is not added in either extra options or extra links. "
+                "This is not allowed."
             )
 
 
 class NeedsConfigException(SphinxError):
     pass
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/needsfile.json` & `sphinx_needs-2.1.0/sphinx_needs/needsfile.json`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/needsfile.py` & `sphinx_needs-2.1.0/sphinx_needs/needsfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Cares about the correct handling with ``needs.json`` files.
 
 Creates, checks and imports ``needs.json`` files.
 """
+
+from __future__ import annotations
+
 import json
 import os
 import sys
 from datetime import datetime
-from typing import Any, List
+from typing import Any
 
 from jsonschema import Draft7Validator
 from sphinx.config import Config
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import NeedsFilterType, NeedsInfoType
 from sphinx_needs.logging import get_logger
@@ -19,21 +22,20 @@
 log = get_logger(__name__)
 
 
 class NeedsList:
     JSON_KEY_EXCLUSIONS_NEEDS = {
         "links_back",
         "type_color",
-        "hide_status",
         "hide",
         "type_prefix",
         "lineno",
+        "lineno_content",
         "collapse",
         "type_style",
-        "hide_tags",
         "content",
         "content_node",
         # id_parent, id_parent are added on calls to `prepare_need_list`
         # but are only relevant to parts
         "id_parent",
         "id_complete",
     }
@@ -41,14 +43,15 @@
     JSON_KEY_EXCLUSIONS_FILTERS = {
         "links_back",
         "type_color",
         "hide_status",
         "hide",
         "type_prefix",
         "lineno",
+        "lineno_content",
         "collapse",
         "type_style",
         "hide_tags",
         "content",
         "content_node",
     }
 
@@ -87,24 +90,38 @@
             self.needs_list["versions"][version]["needs"] = {}
 
         if not self.needs_config.reproducible_json:
             self.needs_list["versions"][version]["created"] = datetime.now().isoformat()
 
     def add_need(self, version: str, need_info: NeedsInfoType) -> None:
         self.update_or_add_version(version)
-        writable_needs = {key: need_info[key] for key in need_info if key not in self._exclude_need_keys}  # type: ignore[literal-required]
+        writable_needs = {
+            key: need_info[key]  # type: ignore[literal-required]
+            for key in need_info
+            if key not in self._exclude_need_keys
+        }
         writable_needs["description"] = need_info["content"]
         self.needs_list["versions"][version]["needs"][need_info["id"]] = writable_needs
-        self.needs_list["versions"][version]["needs_amount"] = len(self.needs_list["versions"][version]["needs"])
+        self.needs_list["versions"][version]["needs_amount"] = len(
+            self.needs_list["versions"][version]["needs"]
+        )
 
     def add_filter(self, version: str, need_filter: NeedsFilterType) -> None:
         self.update_or_add_version(version)
-        writable_filters = {key: need_filter[key] for key in need_filter if key not in self._exclude_filter_keys}  # type: ignore[literal-required]
-        self.needs_list["versions"][version]["filters"][need_filter["export_id"].upper()] = writable_filters
-        self.needs_list["versions"][version]["filters_amount"] = len(self.needs_list["versions"][version]["filters"])
+        writable_filters = {
+            key: need_filter[key]  # type: ignore[literal-required]
+            for key in need_filter
+            if key not in self._exclude_filter_keys
+        }
+        self.needs_list["versions"][version]["filters"][
+            need_filter["export_id"].upper()
+        ] = writable_filters
+        self.needs_list["versions"][version]["filters_amount"] = len(
+            self.needs_list["versions"][version]["filters"]
+        )
 
     def wipe_version(self, version: str) -> None:
         if version in self.needs_list["versions"]:
             del self.needs_list["versions"][version]
 
     def write_json(self, needs_file: str = "needs.json", needs_path: str = "") -> None:
         # We need to rewrite some data, because this kind of data gets overwritten during needs.json import.
@@ -123,37 +140,41 @@
             json.dump(self.needs_list, f, indent=4, sort_keys=True)
 
     def load_json(self, file: str) -> None:
         if not os.path.isabs(file):
             file = os.path.join(self.confdir, file)
 
         if not os.path.exists(file):
-            self.log.warning(f"Could not load needs json file {file} [needs]", type="needs")
+            self.log.warning(
+                f"Could not load needs json file {file} [needs]", type="needs"
+            )
         else:
             errors = check_needs_file(file)
             # We only care for schema errors here, all other possible errors
             # are not important for need-imports.
             if errors.schema:
                 self.log.info(f"Schema validation errors detected in file {file}:")
                 for error in errors.schema:
                     self.log.info(f'  {error.message} -> {".".join(error.path)}')
 
             with open(file) as needs_file:
                 try:
                     needs_list = json.load(needs_file)
                 except json.JSONDecodeError:
-                    self.log.warning(f"Could not decode json file {file} [needs]", type="needs")
+                    self.log.warning(
+                        f"Could not decode json file {file} [needs]", type="needs"
+                    )
                 else:
                     self.needs_list = needs_list
 
             self.log.debug(f"needs.json file loaded: {file}")
 
 
 class Errors:
-    def __init__(self, schema_errors: List[Any]):
+    def __init__(self, schema_errors: list[Any]):
         self.schema = schema_errors
 
 
 def check_needs_file(path: str) -> Errors:
     """
     Checks a given json-file, if it passes our needs.json structure tests.
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/nodes/__init__.py` & `sphinx_needs-2.1.0/sphinx_needs/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/__init__.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_count.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_count.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 """
 Provide the role ``need_count``, which output is the amount of needs found by a given filter-string.
 
 Based on https://github.com/useblocks/sphinxcontrib-needs/issues/37
 """
 
-from typing import List
+from __future__ import annotations
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
 from sphinx_needs.api.exceptions import NeedsInvalidFilter
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.filter_common import filter_needs, prepare_need_list
 from sphinx_needs.logging import get_logger
 
 log = get_logger(__name__)
 
 
-class NeedCount(nodes.Inline, nodes.Element):  # type: ignore
+class NeedCount(nodes.Inline, nodes.Element):
     pass
 
 
 def process_need_count(
-    app: Sphinx, doctree: nodes.document, _fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    _fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     needs_config = NeedsSphinxConfig(app.config)
     for node_need_count in found_nodes:
         all_needs = list(SphinxNeedsData(app.env).get_or_create_needs().values())
         filter = node_need_count["reftarget"]
 
         if filter:
             filters = filter.split(" ? ")
             if len(filters) == 1:
                 need_list = prepare_need_list(all_needs)  # adds parts to need_list
-                amount = str(len(filter_needs(need_list, needs_config, filters[0])))
+                amount = str(
+                    len(
+                        filter_needs(
+                            need_list,
+                            needs_config,
+                            filters[0],
+                            location=node_need_count,
+                        )
+                    )
+                )
             elif len(filters) == 2:
                 need_list = prepare_need_list(all_needs)  # adds parts to need_list
-                amount_1 = len(filter_needs(need_list, needs_config, filters[0]))
-                amount_2 = len(filter_needs(need_list, needs_config, filters[1]))
+                amount_1 = len(
+                    filter_needs(
+                        need_list, needs_config, filters[0], location=node_need_count
+                    )
+                )
+                amount_2 = len(
+                    filter_needs(
+                        need_list, needs_config, filters[1], location=node_need_count
+                    )
+                )
                 amount = f"{amount_1 / amount_2 * 100:2.1f}"
             elif len(filters) > 2:
                 raise NeedsInvalidFilter(
                     "Filter not valid. Got too many filter elements. Allowed are 1 or 2. "
                     'Use " ? " only once to separate filters.'
                 )
         else:
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_func.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """
 Provide the role ``need_func``, which executes a dynamic function.
 """
 
-from typing import List
+from __future__ import annotations
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
 from sphinx_needs.functions.functions import check_and_get_content
 from sphinx_needs.logging import get_logger
 
 log = get_logger(__name__)
 
 
-class NeedFunc(nodes.Inline, nodes.Element):  # type: ignore
+class NeedFunc(nodes.Inline, nodes.Element):
     pass
 
 
 def process_need_func(
-    app: Sphinx, doctree: nodes.document, _fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    _fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     env = app.env
     # for node_need_func in doctree.findall(NeedFunc):
     for node_need_func in found_nodes:
-        result = check_and_get_content(node_need_func.attributes["reftarget"], {"id": "need_func_dummy"}, env)  # type: ignore
+        result = check_and_get_content(
+            node_need_func.attributes["reftarget"],
+            {"id": "need_func_dummy"},  # type: ignore
+            env,
+        )
         new_node_func = nodes.Text(str(result))
         node_need_func.replace_self(new_node_func)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_incoming.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_incoming.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import List
+from __future__ import annotations
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.util.nodes import make_refnode
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.errors import NoUri
 from sphinx_needs.utils import check_and_calc_base_url_rel_path, logger
 
 
-class NeedIncoming(nodes.Inline, nodes.Element):  # type: ignore
+class NeedIncoming(nodes.Inline, nodes.Element):
     pass
 
 
 def process_need_incoming(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     builder = app.builder
     env = app.env
     needs_config = NeedsSphinxConfig(env.config)
     all_needs = SphinxNeedsData(env).get_or_create_needs()
 
     # for node_need_backref in doctree.findall(NeedIncoming):
@@ -50,26 +53,32 @@
                     if needs_config.show_link_type:
                         link_text += " [{type}]".format(type=target_need["type_name"])
 
                     # if index + 1 < len(ref_need["links_back"]):
                     #     link_text += ", "
                     node_need_backref[0] = nodes.Text(link_text)
 
-                    if not target_need["is_external"]:
+                    if not target_need["is_external"] and (
+                        _docname := target_need["docname"]
+                    ):
                         new_node_ref = make_refnode(
                             builder,
                             fromdocname,
-                            target_need["docname"],
+                            _docname,
                             target_need["target_id"],
                             node_need_backref[0].deepcopy(),
                             node_need_backref["reftarget"],
                         )
                     else:
-                        assert target_need["external_url"] is not None, "External URL must not be set"
-                        new_node_ref = nodes.reference(target_need["id"], target_need["id"])
+                        assert (
+                            target_need["external_url"] is not None
+                        ), "External URL must not be set"
+                        new_node_ref = nodes.reference(
+                            target_need["id"], target_need["id"]
+                        )
                         new_node_ref["refuri"] = check_and_calc_base_url_rel_path(
                             target_need["external_url"], fromdocname
                         )
                         new_node_ref["classes"].append(target_need["external_css"])
 
                     node_link_container += new_node_ref
 
@@ -78,13 +87,16 @@
                         node_link_container += nodes.Text(", ")
 
                 except NoUri:
                     # If the given need id can not be found, we must pass here....
                     pass
 
             else:
-                logger.warning(f"need {node_need_backref['reftarget']} not found [needs]", location=node_need_backref)
+                logger.warning(
+                    f"need {node_need_backref['reftarget']} not found [needs]",
+                    location=node_need_backref,
+                )
 
         if len(node_link_container.children) == 0:
             node_link_container += nodes.Text("None")
 
         node_need_backref.replace_self(node_link_container)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_outgoing.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_outgoing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from typing import List
+from __future__ import annotations
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.util.nodes import make_refnode
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import SphinxNeedsData
 from sphinx_needs.errors import NoUri
 from sphinx_needs.logging import get_logger
-from sphinx_needs.utils import check_and_calc_base_url_rel_path
+from sphinx_needs.utils import check_and_calc_base_url_rel_path, split_need_id
 
 log = get_logger(__name__)
 
 
-class NeedOutgoing(nodes.Inline, nodes.Element):  # type: ignore
+class NeedOutgoing(nodes.Inline, nodes.Element):
     pass
 
 
 def process_need_outgoing(
-    app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
 ) -> None:
     builder = app.builder
     env = app.env
     needs_config = NeedsSphinxConfig(app.config)
-    report_dead_links = needs_config.report_dead_links
+    link_lookup = {link["option"]: link for link in needs_config.extra_links}
+
     # for node_need_ref in doctree.findall(NeedOutgoing):
     for node_need_ref in found_nodes:
         node_link_container = nodes.inline()
         needs_all_needs = SphinxNeedsData(env).get_or_create_needs()
         ref_need = needs_all_needs[node_need_ref["reftarget"]]
 
         # Let's check if NeedIncoming shall follow a specific link type
@@ -37,32 +41,33 @@
         # if not, follow back to default links
         else:
             links = ref_need["links"]
             link_type = "links"
 
         link_list = [links] if isinstance(links, str) else links
 
-        for index, link in enumerate(link_list):
-            link_split = link.split(".")
-            link = link_split[0]
-            try:
-                link_part = link_split[1]
-            except IndexError:
-                link_part = None
+        for index, need_id_full in enumerate(link_list):
+            need_id_main, need_id_part = split_need_id(need_id_full)
 
             # If the need target exists, let's create the reference
-            if (link in needs_all_needs and not link_part) or (
-                link_part and link in needs_all_needs and link_part in needs_all_needs[link]["parts"]
+            if (need_id_main in needs_all_needs and not need_id_part) or (
+                need_id_part
+                and need_id_main in needs_all_needs
+                and need_id_part in needs_all_needs[need_id_main]["parts"]
             ):
                 try:
-                    target_need = needs_all_needs[link]
-                    if link_part and link_part in target_need["parts"]:
-                        part_content = target_need["parts"][link_part]["content"]
-                        target_title = part_content if len(part_content) < 30 else part_content[:27] + "..."
-                        target_id = ".".join([link, link_part])
+                    target_need = needs_all_needs[need_id_main]
+                    if need_id_part and need_id_part in target_need["parts"]:
+                        part_content = target_need["parts"][need_id_part]["content"]
+                        target_title = (
+                            part_content
+                            if len(part_content) < 30
+                            else part_content[:27] + "..."
+                        )
+                        target_id = ".".join([need_id_main, need_id_part])
                     else:
                         target_title = target_need["title"]
                         target_id = target_need["id"]
 
                     if needs_config.show_link_title:
                         link_text = f"{target_title}"
 
@@ -72,81 +77,59 @@
                         link_text = target_id
 
                     if needs_config.show_link_type:
                         link_text += " [{type}]".format(type=target_need["type_name"])
 
                     node_need_ref[0] = nodes.Text(link_text)
 
-                    if not target_need["is_external"]:
+                    if not target_need["is_external"] and (
+                        _docname := target_need["docname"]
+                    ):
                         new_node_ref = make_refnode(
                             builder,
                             fromdocname,
-                            target_need["docname"],
+                            _docname,
                             target_id,
                             node_need_ref[0].deepcopy(),
                             node_need_ref["reftarget"],
                         )
                     else:
-                        assert target_need["external_url"] is not None, "External URL must be set"
-                        new_node_ref = nodes.reference(target_need["id"], target_need["id"])
+                        assert (
+                            target_need["external_url"] is not None
+                        ), "External URL must be set"
+                        new_node_ref = nodes.reference(
+                            target_need["id"], target_need["id"]
+                        )
                         new_node_ref["refuri"] = check_and_calc_base_url_rel_path(
                             target_need["external_url"], fromdocname
                         )
                         new_node_ref["classes"].append(target_need["external_css"])
 
                     node_link_container += new_node_ref
 
                 except NoUri:
                     # If the given need id can not be found, we must pass here....
                     pass
 
             else:
                 # Let's add a normal text here instead of a link.
                 # So really each link set by the user gets shown.
-                link_text = f"{link}"
-                if link_part:
-                    link_text += f".{link_part}"
+                link_text = f"{need_id_main}"
+                if need_id_part:
+                    link_text += f".{need_id_part}"
                 dead_link_text = nodes.Text(link_text)
                 dead_link_para = nodes.inline(classes=["needs_dead_link"])
                 dead_link_para.append(dead_link_text)
                 node_link_container += dead_link_para
 
-                extra_links = getattr(env.config, "needs_extra_links", [])
-                extra_links_dict = {x["option"]: x for x in extra_links}
-
-                # Reduce log level to INFO, if dead links are allowed
-                if (
-                    "allow_dead_links" in extra_links_dict[link_type]
-                    and extra_links_dict[link_type]["allow_dead_links"]
-                ):
-                    log_level = "INFO"
-                    kwargs = {}
-                else:
-                    # Set an extra css class, if link type is not configured to allow dead links
+                # add a CSS class for disallowed unknown links
+                # note a warning is already emitted when validating the needs list
+                # so we don't need to do it here
+                if not link_lookup.get(link_type, {}).get("allow_dead_links", False):  # type: ignore
                     dead_link_para.attributes["classes"].append("forbidden")
-                    log_level = "WARNING"
-                    kwargs = {"type": "needs"}
-
-                if report_dead_links:
-                    if node_need_ref and node_need_ref.line:
-                        log.log(
-                            log_level,
-                            f"linked need {link} not found "
-                            f"(Line {node_need_ref.line} of file {node_need_ref.source}) [needs]",
-                            **kwargs,
-                        )
-                    else:
-                        log.log(
-                            log_level,
-                            "outgoing linked need {} not found (document: {}, "
-                            "source need {} on line {} ) [needs]".format(
-                                link, ref_need["docname"], ref_need["id"], ref_need["lineno"]
-                            ),
-                            **kwargs,
-                        )
 
             # If we have several links, we add an empty text between them
             if (index + 1) < len(link_list):
                 node_link_container += nodes.Text(", ")
 
         if len(node_link_container.children) == 0:
             node_link_container += nodes.Text("None")
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_part.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_part.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,51 +2,79 @@
 NeedPart module
 ---------------
 Provides the ability to mark specific parts of a need with an own id.
 
 Most voodoo is done in need.py
 
 """
+
+from __future__ import annotations
+
 import hashlib
 import re
-from typing import List, cast
+from typing import Iterable, cast
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
+from sphinx.util.nodes import make_refnode
 
 from sphinx_needs.data import NeedsInfoType
 from sphinx_needs.logging import get_logger
 
 log = get_logger(__name__)
 
 
-class NeedPart(nodes.Inline, nodes.Element):  # type: ignore
+class NeedPart(nodes.Inline, nodes.Element):
     pass
 
 
-def process_need_part(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_need_part(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     pass
 
 
 part_pattern = re.compile(r"\(([\w-]+)\)(.*)")
 
 
-def update_need_with_parts(env: BuildEnvironment, need: NeedsInfoType, part_nodes: List[NeedPart]) -> None:
+def iter_need_parts(need: NeedsInfoType) -> Iterable[NeedsInfoType]:
+    """Yield all parts, a.k.a sub-needs, from a need.
+
+    A sub-need is a child of a need, which has its own ID,
+    and overrides the content of the parent need.
+    """
+    for part in need["parts"].values():
+        full_part: NeedsInfoType = {**need, **part}
+        full_part["id_complete"] = f"{need['id']}.{part['id']}"
+        full_part["id_parent"] = need["id"]
+        full_part["is_need"] = False
+        full_part["is_part"] = True
+
+        yield full_part
+
+
+def update_need_with_parts(
+    env: BuildEnvironment, need: NeedsInfoType, part_nodes: list[NeedPart]
+) -> None:
     app = env.app
-    builder = app.builder
     for part_node in part_nodes:
         content = cast(str, part_node.children[0].children[0])  # ->inline->Text
         result = part_pattern.match(content)
         if result:
             inline_id = result.group(1)
             part_content = result.group(2)
         else:
             part_content = content
-            inline_id = hashlib.sha1(part_content.encode("UTF-8")).hexdigest().upper()[:3]
+            inline_id = (
+                hashlib.sha1(part_content.encode("UTF-8")).hexdigest().upper()[:3]
+            )
 
         if "parts" not in need:
             need["parts"] = {}
 
         if inline_id in need["parts"]:
             log.warning(
                 "part_need id {} in need {} is already taken. need_part may get overridden. [needs]".format(
@@ -54,42 +82,43 @@
                 ),
                 type="needs",
             )
 
         need["parts"][inline_id] = {
             "id": inline_id,
             "content": part_content,
-            "document": need["docname"],
-            "links_back": [],
-            "is_part": True,
-            "is_need": False,
             "links": [],
+            "links_back": [],
         }
 
         part_id_ref = "{}.{}".format(need["id"], inline_id)
-        part_id_show = inline_id
+
         part_node["reftarget"] = part_id_ref
 
-        part_link_text = f" {part_id_show}"
-        part_link_node = nodes.Text(part_link_text)
         part_text_node = nodes.Text(part_content)
 
-        from sphinx.util.nodes import make_refnode
-
-        part_ref_node = make_refnode(builder, need["docname"], need["docname"], part_id_ref, part_link_node)
-        part_ref_node["classes"] += ["needs-id"]
-
         part_node.children = []
         node_need_part_line = nodes.inline(ids=[part_id_ref], classes=["need-part"])
         node_need_part_line.append(part_text_node)
-        node_need_part_line.append(part_ref_node)
+
+        if docname := need["docname"]:
+            part_id_show = inline_id
+            part_link_text = f" {part_id_show}"
+            part_link_node = nodes.Text(part_link_text)
+
+            part_ref_node = make_refnode(
+                app.builder, docname, docname, part_id_ref, part_link_node
+            )
+            part_ref_node["classes"] += ["needs-id"]
+            node_need_part_line.append(part_ref_node)
+
         part_node.append(node_need_part_line)
 
 
-def find_parts(node: nodes.Node) -> List[NeedPart]:
+def find_parts(node: nodes.Node) -> list[NeedPart]:
     found_nodes = []
     for child in node.children:
         if isinstance(child, NeedPart):
             found_nodes.append(child)
         else:
             found_nodes += find_parts(child)
     return found_nodes
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/roles/need_ref.py` & `sphinx_needs-2.1.0/sphinx_needs/roles/need_ref.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
+from __future__ import annotations
+
 import contextlib
 from collections.abc import Iterable
-from typing import Dict, List, Union
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.util.nodes import make_refnode
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.errors import NoUri
 from sphinx_needs.logging import get_logger
-from sphinx_needs.utils import check_and_calc_base_url_rel_path
+from sphinx_needs.utils import check_and_calc_base_url_rel_path, split_need_id
 
 log = get_logger(__name__)
 
 
-class NeedRef(nodes.Inline, nodes.Element):  # type: ignore
+class NeedRef(nodes.Inline, nodes.Element):
     pass
 
 
-def transform_need_to_dict(need: NeedsInfoType) -> Dict[str, str]:
+def transform_need_to_dict(need: NeedsInfoType) -> dict[str, str]:
     """
     The function will transform a need in a dictionary of strings. Used to
     be given e.g. to a python format string.
 
     Parameters
     ----------
     need : need
@@ -46,15 +47,20 @@
             dict_need[element] = ";".join([str(i) for i in value])
         else:
             dict_need[element] = str(value)
 
     return dict_need
 
 
-def process_need_ref(app: Sphinx, doctree: nodes.document, fromdocname: str, found_nodes: List[nodes.Element]) -> None:
+def process_need_ref(
+    app: Sphinx,
+    doctree: nodes.document,
+    fromdocname: str,
+    found_nodes: list[nodes.Element],
+) -> None:
     builder = app.builder
     env = app.env
     needs_config = NeedsSphinxConfig(env.config)
     all_needs = SphinxNeedsData(env).get_or_create_needs()
     # for node_need_ref in doctree.findall(NeedRef):
     for node_need_ref in found_nodes:
         # Let's create a dummy node, for the case we will not be able to create a real reference
@@ -67,44 +73,41 @@
             node_need_ref["reftarget"] + "?",
         )
 
         # It is possible to change the prefix / postfix easily here.
         prefix = "[["
         postfix = "]]"
 
-        ref_id_complete = node_need_ref["reftarget"]
-
-        if "." in ref_id_complete:
-            ref_id, part_id = ref_id_complete.split(".")
-        else:
-            ref_id = ref_id_complete
-            part_id = None
+        need_id_full = node_need_ref["reftarget"]
+        need_id_main, need_id_part = split_need_id(need_id_full)
 
-        if ref_id in all_needs:
-            target_need = all_needs[ref_id]
+        if need_id_main in all_needs:
+            target_need = all_needs[need_id_main]
 
-            dict_need = transform_need_to_dict(target_need)  # Transform a dict in a dict of {str, str}
+            dict_need = transform_need_to_dict(
+                target_need
+            )  # Transform a dict in a dict of {str, str}
 
             # We set the id to the complete id maintained in node_need_ref["reftarget"]
-            dict_need["id"] = ref_id_complete
+            dict_need["id"] = need_id_full
 
-            if part_id:
+            if need_id_part:
                 # If part_id, we have to fetch the title from the content.
-                dict_need["title"] = target_need["parts"][part_id]["content"]
+                dict_need["title"] = target_need["parts"][need_id_part]["content"]
 
             # Shorten title, if necessary
             max_length = needs_config.role_need_max_title_length
             if 3 < max_length < len(dict_need["title"]):
                 title = dict_need["title"]
                 title = f"{title[: max_length - 3]}..."
                 dict_need["title"] = title
 
-            ref_name: Union[None, str, nodes.Text] = node_need_ref.children[0].children[0]  # type: ignore[assignment]
+            ref_name: None | str | nodes.Text = node_need_ref.children[0].children[0]  # type: ignore[assignment]
             # Only use ref_name, if it differs from ref_id
-            if str(ref_id_complete) == str(ref_name):
+            if str(need_id_full) == str(ref_name):
                 ref_name = None
 
             if ref_name and prefix in ref_name and postfix in ref_name:
                 # if ref_name is set and has prefix to process, we will do so.
                 ref_name = ref_name.replace(prefix, "{").replace(postfix, "}")
                 try:
                     link_text = ref_name.format(**dict_need)
@@ -117,38 +120,43 @@
             else:
                 if ref_name:
                     # If ref_name differs from the need id, we treat the "ref_name content" as title.
                     dict_need["title"] = ref_name
                 try:
                     link_text = needs_config.role_need_template.format(**dict_need)
                 except KeyError as e:
-                    link_text = (
-                        '"the config parameter needs_role_need_template uses not supported placeholders: %s "' % e
-                    )
+                    link_text = f'"the config parameter needs_role_need_template uses not supported placeholders: {e} "'
                     log.warning(link_text + " [needs]", type="needs")
 
             node_need_ref[0].children[0] = nodes.Text(link_text)  # type: ignore[index]
 
             with contextlib.suppress(NoUri):
-                if not target_need.get("is_external", False):
+                if not target_need.get("is_external", False) and (
+                    _docname := target_need["docname"]
+                ):
                     new_node_ref = make_refnode(
                         builder,
                         fromdocname,
-                        target_need["docname"],
+                        _docname,
                         node_need_ref["reftarget"],
                         node_need_ref[0].deepcopy(),
                         node_need_ref["reftarget"],
                     )
                 else:
-                    assert target_need["external_url"] is not None, "external_url must be set for external needs"
+                    assert (
+                        target_need["external_url"] is not None
+                    ), "external_url must be set for external needs"
                     new_node_ref = nodes.reference(target_need["id"], target_need["id"])
-                    new_node_ref["refuri"] = check_and_calc_base_url_rel_path(target_need["external_url"], fromdocname)
+                    new_node_ref["refuri"] = check_and_calc_base_url_rel_path(
+                        target_need["external_url"], fromdocname
+                    )
                     new_node_ref["classes"].append(target_need["external_css"])
 
         else:
             log.warning(
-                f"linked need {node_need_ref['reftarget']} not found [needs]",
+                f"linked need {node_need_ref['reftarget']} not found [needs.link_ref]",
                 type="needs",
+                subtype="link_ref",
                 location=node_need_ref,
             )
 
         node_need_ref.replace_self(new_node_ref)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/services/config/github.py` & `sphinx_needs-2.1.0/sphinx_needs/services/config/github.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,54 @@
+from __future__ import annotations
+
 EXTRA_DATA_OPTIONS = ["user", "created_at", "updated_at", "closed_at", "service"]
 EXTRA_LINK_OPTIONS = ["url"]
 EXTRA_IMAGE_OPTIONS = ["avatar"]
-CONFIG_OPTIONS = ["type", "query", "specific", "max_amount", "max_content_lines", "id_prefix"]
-GITHUB_DATA = ["status", "tags"] + EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS
-GITHUB_DATA_STR = '"' + '","'.join(EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS) + '"'
+CONFIG_OPTIONS = [
+    "type",
+    "query",
+    "specific",
+    "max_amount",
+    "max_content_lines",
+    "id_prefix",
+]
+GITHUB_DATA = (
+    ["status", "tags"] + EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS
+)
+GITHUB_DATA_STR = (
+    '"'
+    + '","'.join(EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS)
+    + '"'
+)
 CONFIG_DATA_STR = '"' + '","'.join(CONFIG_OPTIONS) + '"'
 GITHUB_LAYOUT = {
     "grid": "complex",
     "layout": {
         "head_left": [
             "<<meta_id()>>",
             '<<collapse_button("meta,footer", collapsed="icon:arrow-down-circle", '
             'visible="icon:arrow-right-circle", initial=True)>>',
         ],
         "head": [
             '**<<meta("title")>>** ('
             + ", ".join(
-                ['<<link("{value}", text="{value}", is_dynamic=True)>>'.format(value=x) for x in EXTRA_LINK_OPTIONS]
+                [
+                    f'<<link("{x}", text="{x}", is_dynamic=True)>>'
+                    for x in EXTRA_LINK_OPTIONS
+                ]
             )
             + ")"
         ],
-        "head_right": ['<<image("field:avatar", width="40px", align="middle")>>', '<<meta("user")>>'],
-        "meta_left": ['<<meta("{value}", prefix="{value}: ")>>'.format(value=x) for x in EXTRA_DATA_OPTIONS]
+        "head_right": [
+            '<<image("field:avatar", width="40px", align="middle")>>',
+            '<<meta("user")>>',
+        ],
+        "meta_left": [f'<<meta("{x}", prefix="{x}: ")>>' for x in EXTRA_DATA_OPTIONS]
         + [
-            '<<link("{value}", text="Link", prefix="{value}: ", is_dynamic=True)>>'.format(value=x)
+            f'<<link("{x}", text="Link", prefix="{x}: ", is_dynamic=True)>>'
             for x in EXTRA_LINK_OPTIONS
         ],
         "meta_right": [
             '<<meta("type_name", prefix="type: ")>>',
             f'<<meta_all(no_links=True, exclude=["layout","style",{GITHUB_DATA_STR}, {CONFIG_DATA_STR}])>>',
             "<<meta_links_all()>>",
         ],
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/services/github.py` & `sphinx_needs-2.1.0/sphinx_needs/services/github.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,53 @@
+from __future__ import annotations
+
 import os
 import textwrap
 import time
 from contextlib import suppress
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
 from urllib.parse import urlparse
 
 import requests
 from sphinx.application import Sphinx
+from sphinx.util.docutils import SphinxDirective
+from sphinx.util.logging import getLogger
 
 from sphinx_needs.api import add_need_type
 from sphinx_needs.api.exceptions import NeedsApiConfigException
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.services.base import BaseService
 from sphinx_needs.services.config.github import (
     CONFIG_OPTIONS,
     EXTRA_DATA_OPTIONS,
     EXTRA_IMAGE_OPTIONS,
     EXTRA_LINK_OPTIONS,
     GITHUB_DATA,
     GITHUB_LAYOUT,
 )
 
+LOGGER = getLogger(__name__)
 
-class GithubService(BaseService):
-    options = CONFIG_OPTIONS + EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS
 
-    def __init__(self, app: Sphinx, name: str, config: Dict[str, Any], **kwargs: Any) -> None:
+class GithubService(BaseService):
+    options = (
+        CONFIG_OPTIONS + EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS + EXTRA_IMAGE_OPTIONS
+    )
+
+    def __init__(
+        self, app: Sphinx, name: str, config: dict[str, Any], **kwargs: Any
+    ) -> None:
         self.app = app
         self.name = name
         self.config = config
 
         self.url = self.config.get("url", "https://api.github.com/")
         if not self.url.endswith("/"):
             self.url = f"{self.url}/"
+        self.retry_delay = self.config.get("retry_delay", 61)
         self.max_amount = self.config.get("max_amount", -1)
         self.max_content_lines = self.config.get("max_content_lines", -1)
         self.id_prefix = self.config.get("id_prefix", "GITHUB_")
         self.layout = self.config.get("layout", "github")
         self.download_avatars = self.config.get("download_avatars", True)
         self.download_folder = self.config.get("download_folder", "github_images")
 
@@ -44,15 +55,19 @@
         self.token = self.config.get("token")
 
         layouts = NeedsSphinxConfig(self.app.config).layouts
         if "github" not in layouts:
             layouts["github"] = GITHUB_LAYOUT
 
         self.gh_type_config = {
-            "issue": {"url": "search/issues", "query": "is:issue", "need_type": "issue"},
+            "issue": {
+                "url": "search/issues",
+                "query": "is:issue",
+                "need_type": "issue",
+            },
             "pr": {"url": "search/issues", "query": "is:pr", "need_type": "pr"},
             "commit": {"url": "search/commits", "query": "", "need_type": "commit"},
         }
 
         with suppress(NeedsApiConfigException):
             # Issue already exists, so we are fine
             add_need_type(self.app, "issue", "Issue", "IS_", "#cccccc", "card")
@@ -62,23 +77,29 @@
             add_need_type(self.app, "commit", "Commit", "C_", "#888888", "card")
 
         if "gh_type" in kwargs:
             self.gh_type = kwargs["gh_type"]
 
         if self.gh_type not in self.gh_type_config.keys():
             raise KeyError(
-                'github type "{}" not supported. Use: {}'.format(self.gh_type, ", ".join(self.gh_type_config.keys()))
+                'github type "{}" not supported. Use: {}'.format(
+                    self.gh_type, ", ".join(self.gh_type_config.keys())
+                )
             )
 
         # Set need_type to use by default
-        self.need_type = self.config.get("need_type", self.gh_type_config[self.gh_type]["need_type"])
+        self.need_type = self.config.get(
+            "need_type", self.gh_type_config[self.gh_type]["need_type"]
+        )
 
         super().__init__()
 
-    def _send(self, query: str, options: Dict[str, Any], specific: bool = False) -> Dict[str, Any]:
+    def _send(
+        self, query: str, options: dict[str, Any], specific: bool = False
+    ) -> dict[str, Any]:
         headers = {}
         if self.gh_type == "commit":
             headers["Accept"] = "application/vnd.github.cloak-preview+json"
 
         if specific:
             try:
                 specific_elements = query.split("/")
@@ -87,246 +108,296 @@
                 number = specific_elements[2]
                 if self.gh_type == "issue":
                     single_type = "issues"
                 elif self.gh_type == "pr":
                     single_type = "pulls"
                 else:
                     single_type = "commits"
-                url = self.url + "repos/{owner}/{repo}/{single_type}/{number}".format(
-                    owner=owner, repo=repo, single_type=single_type, number=number
-                )
+                url = self.url + f"repos/{owner}/{repo}/{single_type}/{number}"
             except IndexError:
-                raise NeedGithubServiceException('Single option ot valid, must follow "owner/repo/number"')
+                raise _SendException(
+                    'Single option ot valid, must follow "owner/repo/number"'
+                )
 
             params = {}
         else:
             url = self.url + self.gh_type_config[self.gh_type]["url"]
             query = "{} {}".format(query, self.gh_type_config[self.gh_type]["query"])
-            params = {"q": query, "per_page": options.get("max_amount", self.max_amount)}
+            params = {
+                "q": query,
+                "per_page": options.get("max_amount", self.max_amount),
+            }
 
         self.log.info(f"Service {self.name} requesting data for query: {query}")
 
-        auth: Optional[Tuple[str, str]]
+        auth: tuple[str, str] | None
         if self.username:
             # TODO token can be None
             auth = (self.username, self.token)  # type: ignore
         else:
             auth = None
 
         resp = requests.get(url, params=params, auth=auth, headers=headers)
 
         if resp.status_code > 299:
             extra_info = ""
             # Lets try to get information about the rate limit, as this is mostly the main problem.
             if "rate limit" in resp.json()["message"]:
                 resp_limit = requests.get(self.url + "rate_limit", auth=auth)
                 extra_info = resp_limit.json()
-                self.log.info("GitHub: API rate limit exceeded. We need to wait 60 secs...")
+                self.log.info(
+                    f"GitHub: API rate limit exceeded. trying again in {self.retry_delay} seconds..."
+                )
                 self.log.info(extra_info)
-                time.sleep(61)
+                time.sleep(self.retry_delay)
                 resp = requests.get(url, params=params, auth=auth, headers=headers)
                 if resp.status_code > 299:
                     if "rate limit" in resp.json()["message"]:
-                        raise NeedGithubServiceException("GitHub: API rate limit exceeded (twice). Stop here.")
+                        raise _SendException(
+                            "GitHub: API rate limit exceeded (twice). Stop here."
+                        )
                     else:
-                        raise NeedGithubServiceException(
+                        raise _SendException(
                             "Github service error during request.\n"
-                            "Status code: {}\n"
-                            "Error: {}\n"
-                            "{}".format(resp.status_code, resp.text, extra_info)
+                            f"Status code: {resp.status_code}\n"
+                            f"Error: {resp.text}\n"
+                            f"{extra_info}"
                         )
             else:
-                raise NeedGithubServiceException(
+                raise _SendException(
                     "Github service error during request.\n"
-                    "Status code: {}\n"
-                    "Error: {}\n"
-                    "{}".format(resp.status_code, resp.text, extra_info)
+                    f"Status code: {resp.status_code}\n"
+                    f"Error: {resp.text}\n"
+                    f"{extra_info}"
                 )
 
         if specific:
             return {"items": [resp.json()]}
         return resp.json()  # type: ignore
 
-    def request(self, options: Optional[Dict[str, Any]] = None) -> List[Dict[str, Any]]:
-        if options is None:
-            options = {}
+    def request_from_directive(
+        self, directive: SphinxDirective, /
+    ) -> list[dict[str, Any]]:
         self.log.debug(f"Requesting data for service {self.name}")
+        options = directive.options
 
         if "query" not in options and "specific" not in options:
-            raise NeedGithubServiceException('"query" or "specific" missing as option for github service.')
-        elif "query" in options and "specific" in options:
-            raise NeedGithubServiceException('Only "query" or "specific" allowed for github service. Not both!')
-        elif "query" in options:
+            create_warning(
+                directive,
+                '"query" or "specific" missing as option for github service.',
+            )
+            return []
+
+        if "query" in options and "specific" in options:
+            create_warning(
+                directive,
+                'Only "query" or "specific" allowed for github service. Not both!',
+            )
+            return []
+
+        if "query" in options:
             query = options["query"]
             specific = False
         else:
             query = options["specific"]
             specific = True
 
-        response = self._send(query, options, specific=specific)
+        try:
+            response = self._send(query, options, specific=specific)
+        except _SendException as e:
+            create_warning(directive, str(e))
+            return []
         if "items" not in response:
             if "errors" in response:
-                raise NeedGithubServiceException(
-                    "GitHub service query error: {}\n" "Used query: {}".format(response["errors"][0]["message"], query)
+                create_warning(
+                    directive,
+                    "GitHub service query error: {}\n" "Used query: {}".format(
+                        response["errors"][0]["message"], query
+                    ),
                 )
+                return []
             else:
-                raise NeedGithubServiceException("Github service: Unknown error.")
+                create_warning(directive, "Github service: Unknown error")
+                return []
 
         if self.gh_type == "issue" or self.gh_type == "pr":
-            data = self.prepare_issue_data(response["items"], options)
+            data = self.prepare_issue_data(response["items"], directive)
         elif self.gh_type == "commit":
-            data = self.prepare_commit_data(response["items"], options)
+            data = self.prepare_commit_data(response["items"], directive)
         else:
-            raise NeedGithubServiceException("Github service failed. Wrong gh_type...")
+            create_warning(directive, "Github service failed. Wrong gh_type...")
+            return []
 
         return data
 
-    def prepare_issue_data(self, items: List[Dict[str, Any]], options: Dict[str, Any]) -> List[Dict[str, Any]]:
+    def prepare_issue_data(
+        self, items: list[dict[str, Any]], directive: SphinxDirective
+    ) -> list[dict[str, Any]]:
         data = []
         for item in items:
             # ensure that "None" can not reach .splitlines()
             if item["body"] is None:
                 item["body"] = ""
 
             # wraps content lines, if they are too long. Respects already existing newlines.
             content_lines = [
-                "\n   ".join(textwrap.wrap(line, 60, break_long_words=True, replace_whitespace=False))
+                "\n   ".join(
+                    textwrap.wrap(
+                        line, 60, break_long_words=True, replace_whitespace=False
+                    )
+                )
                 for line in item["body"].splitlines()  # type: ignore
                 if line.strip()
             ]
 
             content = "\n\n   ".join(content_lines)
             # Reduce content length, if requested by config
-            if self.max_content_lines > 0:
-                max_lines = int(options.get("max_content_lines", self.max_content_lines))
+            if (self.max_content_lines > 0) or (
+                "max_content_lines" in directive.options
+            ):
+                max_lines = int(
+                    directive.options.get("max_content_lines", self.max_content_lines)
+                )
                 content_lines = content.splitlines()
                 if len(content_lines) > max_lines:
                     content_lines = content_lines[0:max_lines]
                     content_lines.append("\n   [...]\n")  # Mark, if content got cut
                 content = "\n".join(content_lines)
 
             # Be sure the content gets not interpreted as rst or html code, so we put
             # everything in a safe code-block
             content = ".. code-block:: text\n\n   " + content
 
-            prefix = options.get("id_prefix", self.id_prefix)
+            prefix = directive.options.get("id_prefix", self.id_prefix)
             need_id = prefix + str(item["number"])
-            given_tags = options.get("tags", False)
+            given_tags = directive.options.get("tags", False)
             github_tags = ",".join([x["name"] for x in item["labels"]])
             if given_tags:
                 tags = str(given_tags) + ", " + str(github_tags)
             else:
                 tags = github_tags
 
-            avatar_file_path = self._get_avatar(item["user"]["avatar_url"])
+            avatar_file_path = self._get_avatar(item["user"]["avatar_url"], directive)
 
             element_data = {
                 "service": self.name,
-                "type": options.get("type", self.need_type),
-                "layout": options.get("layout", self.layout),
+                "type": directive.options.get("type", self.need_type),
+                "layout": directive.options.get("layout", self.layout),
                 "id": need_id,
                 "title": item["title"],
                 "content": content,
                 "status": item["state"],
                 "tags": tags,
                 "user": item["user"]["login"],
                 "url": item["html_url"],
                 "avatar": avatar_file_path,
                 "created_at": item["created_at"],
                 "updated_at": item["updated_at"],
                 "closed_at": item["closed_at"],
             }
-            self._add_given_options(options, element_data)
+            self._add_given_options(directive.options, element_data)
             data.append(element_data)
 
         return data
 
-    def prepare_commit_data(self, items: List[Dict[str, Any]], options: Dict[str, Any]) -> List[Dict[str, Any]]:
+    def prepare_commit_data(
+        self, items: list[dict[str, Any]], directive: SphinxDirective
+    ) -> list[dict[str, Any]]:
         data = []
 
         for item in items:
-            avatar_file_path = self._get_avatar(item["author"]["avatar_url"])
+            avatar_file_path = self._get_avatar(item["author"]["avatar_url"], directive)
 
             element_data = {
                 "service": self.name,
-                "type": options.get("type", self.need_type),
-                "layout": options.get("layout", self.layout),
+                "type": directive.options.get("type", self.need_type),
+                "layout": directive.options.get("layout", self.layout),
                 "id": self.id_prefix + item["sha"][:6],
-                "title": item["commit"]["message"].split("\n")[0][:60],  # 1. line, max length 60 chars
+                "title": item["commit"]["message"].split("\n")[0][
+                    :60
+                ],  # 1. line, max length 60 chars
                 "content": item["commit"]["message"],
                 "user": item["author"]["login"],
                 "url": item["html_url"],
                 "avatar": avatar_file_path,
                 "created_at": item["commit"]["author"]["date"],
             }
-            self._add_given_options(options, element_data)
+            self._add_given_options(directive.options, element_data)
             data.append(element_data)
 
         return data
 
-    def _get_avatar(self, avatar_url: str) -> str:
-        """
-        Download and store avatar image
-
-        :param avatar_url:
-        :return:
-        """
+    def _get_avatar(self, avatar_url: str, directive: SphinxDirective) -> str:
+        """Download and store avatar image"""
         url_parsed = urlparse(avatar_url)
         filename = os.path.basename(url_parsed.path) + ".png"
         path = os.path.join(self.app.srcdir, self.download_folder)
         avatar_file_path = os.path.join(path, filename)
 
         # Placeholder avatar, if things go wrong or avatar download is deactivated
-        default_avatar_file_path = os.path.join(os.path.dirname(__file__), "../images/avatar.png")
+        default_avatar_file_path = os.path.join(
+            os.path.dirname(__file__), "../images/avatar.png"
+        )
         if self.download_avatars:
             # Download only, if file not downloaded yet
             if not os.path.exists(avatar_file_path):
                 with suppress(FileExistsError):
                     os.mkdir(path)
                 if self.username and self.token:
                     auth = (self.username, self.token)
                 else:
                     auth = None
                 response = requests.get(avatar_url, auth=auth, allow_redirects=False)
                 if response.status_code == 200:
                     with open(avatar_file_path, "wb") as f:
                         f.write(response.content)
                 elif response.status_code == 302:
-                    self.log.warning(
-                        "GitHub service {} could not download avatar image "
-                        "from {}.\n"
-                        "    Status code: {}\n"
+                    create_warning(
+                        directive,
+                        f"GitHub service {self.name} could not download avatar image "
+                        f"from {avatar_url}.\n"
+                        f"    Status code: {response.status_code}\n"
                         "    Reason: Looks like the authentication provider tries to redirect you."
                         " This is not supported and is a common problem, "
-                        "if you use GitHub Enterprise. [needs]".format(self.name, avatar_url, response.status_code),
-                        type="needs",
+                        "if you use GitHub Enterprise.",
                     )
                     avatar_file_path = default_avatar_file_path
                 else:
-                    self.log.warning(
-                        "GitHub service {} could not download avatar image "
-                        "from {}.\n"
-                        "    Status code: {} [needs]".format(self.name, avatar_url, response.status_code),
-                        type="needs",
+                    create_warning(
+                        directive,
+                        f"GitHub service {self.name} could not download avatar image "
+                        f"from {avatar_url}.\n"
+                        f"    Status code: {response.status_code}",
                     )
                     avatar_file_path = default_avatar_file_path
         else:
             avatar_file_path = default_avatar_file_path
 
         return avatar_file_path
 
-    def _add_given_options(self, options: Dict[str, Any], element_data: Dict[str, Any]) -> None:
+    def _add_given_options(
+        self, options: dict[str, Any], element_data: dict[str, Any]
+    ) -> None:
         """
         Add data from options, which was defined by user but is not set by this service
 
         :param options:
         :param element_data:
         :return:
         """
         for key, value in options.items():
             # Check if given option is not already handled and is not part of the service internal options
             if key not in element_data.keys() and key not in GITHUB_DATA:
                 element_data[key] = value
 
 
-class NeedGithubServiceException(BaseException):
+class _SendException(Exception):
     pass
+
+
+def create_warning(directive: SphinxDirective, message: str) -> None:
+    LOGGER.warning(
+        message + " [needs.github]",
+        type="needs",
+        subtype="github",
+        location=directive.get_location(),
+    )
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/services/manager.py` & `sphinx_needs-2.1.0/sphinx_needs/services/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Dict, Type
+from __future__ import annotations
+
+from typing import Any
 
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 
 from sphinx_needs.api.configuration import NEEDS_CONFIG
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.directives.needservice import NeedserviceDirective
@@ -11,21 +13,23 @@
 
 
 class ServiceManager:
     def __init__(self, app: Sphinx):
         self.app = app
 
         self.log = get_logger(__name__)
-        self.services: Dict[str, BaseService] = {}
+        self.services: dict[str, BaseService] = {}
 
-    def register(self, name: str, klass: Type[BaseService], **kwargs: Any) -> None:
+    def register(self, name: str, klass: type[BaseService], **kwargs: Any) -> None:
         try:
             config = NeedsSphinxConfig(self.app.config).services[name]
         except KeyError:
-            self.log.debug(f"No service config found for {name}. Add it in your conf.py to needs_services dictionary.")
+            self.log.debug(
+                f"No service config found for {name}. Add it in your conf.py to needs_services dictionary."
+            )
             config = {}
 
         # Register options from service class
         for option in klass.options:
             if option not in NEEDS_CONFIG.extra_options:
                 self.log.debug(f'Register option "{option}" for service "{name}"')
                 NEEDS_CONFIG.extra_options[option] = directives.unchanged
@@ -37,13 +41,15 @@
         self.services[name] = klass(self.app, name, config, **kwargs)
 
     def get(self, name: str) -> BaseService:
         if name in self.services:
             return self.services[name]
         else:
             raise NeedsServiceException(
-                "Service {} could not be found. " "Available services are {}".format(name, ", ".join(self.services))
+                "Service {} could not be found. " "Available services are {}".format(
+                    name, ", ".join(self.services)
+                )
             )
 
 
 class NeedsServiceException(BaseException):
     pass
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/services/open_needs.py` & `sphinx_needs-2.1.0/sphinx_needs/services/open_needs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import re
 from random import choices
-from typing import Any, Dict, List
+from typing import Any
 
 import requests
 from jinja2 import Template
 from sphinx.application import Sphinx
+from sphinx.util.docutils import SphinxDirective
 
 from sphinx_needs.config import NeedsSphinxConfig
 from sphinx_needs.utils import dict_get, jinja_parse
 
 from .base import BaseService
 from .config.open_needs import (
     CONFIG_OPTIONS,
@@ -18,15 +21,17 @@
     MAPPINGS_REPLACES_DEFAULT,
 )
 
 
 class OpenNeedsService(BaseService):
     options = CONFIG_OPTIONS + EXTRA_DATA_OPTIONS + EXTRA_LINK_OPTIONS
 
-    def __init__(self, app: Sphinx, name: str, config: Dict[str, Any], **kwargs: Any) -> None:
+    def __init__(
+        self, app: Sphinx, name: str, config: dict[str, Any], **kwargs: Any
+    ) -> None:
         self.app = app
         self.name = name
         self.config = config
 
         self.url: str = self.config.get("url", "http://127.0.0.1:9595")
         if self.url.endswith("/"):
             self.url = self.url.rstrip("/")
@@ -34,18 +39,20 @@
         if not self.url_postfix.startswith("/"):
             self.url_postfix = "/" + self.url_postfix
         self.max_content_lines = self.config.get("max_content_lines", -1)
 
         self.id_prefix = self.config.get("id_prefix", "OPEN_NEEDS_")
         self.query = self.config.get("query", "")
         self.content = self.config.get("content", DEFAULT_CONTENT)
-        self.mappings: Dict[str, Any] = self.config.get("mappings", {})
-        self.mapping_replaces = self.config.get("mappings_replaces", MAPPINGS_REPLACES_DEFAULT)
+        self.mappings: dict[str, Any] = self.config.get("mappings", {})
+        self.mapping_replaces = self.config.get(
+            "mappings_replaces", MAPPINGS_REPLACES_DEFAULT
+        )
 
-        self.extra_data: Dict[str, Any] = self.config.get("extra_data", {})
+        self.extra_data: dict[str, Any] = self.config.get("extra_data", {})
         self.params = self.config.get("params", "skip=0,limit=100")
 
         super().__init__(**kwargs)
 
     def _oauthorization(self) -> None:
         username = self.config.get("user")
         password = self.config.get("password")
@@ -53,29 +60,34 @@
             auth = {"username": username, "password": password}
             login_postfix = "/auth/jwt/login"
             url: str = self.url + login_postfix
             login_resp = requests.post(url, data=auth)
             if login_resp.status_code != 200:
                 raise OpenNeedsServiceException(
                     "ONS service error during request.\n"
-                    "Status code: {}\n"
-                    "Error: {}\n".format(login_resp.status_code, login_resp.text)
+                    f"Status code: {login_resp.status_code}\n"
+                    f"Error: {login_resp.text}\n"
                 )
             oauth_credentials = dict(**login_resp.json())
             self.token_type = oauth_credentials.get("token_type")
             self.access_token = oauth_credentials.get("access_token")
 
     def _prepare_request(self, options: Any) -> Any:
         if options is None:
             options = {}
         url: str = options.get("url", self.url)
         url = url + str(self.url_postfix)
 
-        headers: Dict[str, str] = {"Authorization": f"{self.token_type} {self.access_token}"}
-        params: List[str] = [param.strip() for param in re.split(r";|,", options.get("params", self.params))]
+        headers: dict[str, str] = {
+            "Authorization": f"{self.token_type} {self.access_token}"
+        }
+        params: list[str] = [
+            param.strip()
+            for param in re.split(r";|,", options.get("params", self.params))
+        ]
         new_params: str = "&".join(params)
 
         url = f"{url}?{new_params}"
 
         request: Any = {"url": url, "headers": headers}
         return request
 
@@ -87,18 +99,22 @@
         This request-data gets mostly defined by using ``prepare_request``.
         :param request: dict
         :return: request answer
         """
 
         result: Any = requests.get(**request)
         if result.status_code >= 300:
-            raise OpenNeedsServiceException(f"Problem accessing {result.url}.\nReason: {result.text}")
+            raise OpenNeedsServiceException(
+                f"Problem accessing {result.url}.\nReason: {result.text}"
+            )
         return result
 
-    def _extract_data(self, data: List[Dict[str, Any]], options: Dict[str, Any]) -> List[Dict[str, Any]]:
+    def _extract_data(
+        self, data: list[dict[str, Any]], options: dict[str, Any]
+    ) -> list[dict[str, Any]]:
         """
         Extract data of a list/dictionary, which was retrieved via send_request.
         :param data: list or dict
         :param options: dict of set directive options
         :return: list of need-data
         """
         needs_config = NeedsSphinxConfig(self.app.config)
@@ -170,51 +186,58 @@
                     need_values[name] = selector
                 else:
                     value = dict_get(item, selector)
                     if isinstance(value, (tuple, list)):
                         if name == "links":
                             # Add a prefix to the referenced link if it is an ID of a need object in
                             # the data retrieved from the Open Needs Server or don't add prefix
-                            value = [(prefix + link if link in ids_of_needs_data else link) for link in value]
+                            value = [
+                                (prefix + link if link in ids_of_needs_data else link)
+                                for link in value
+                            ]
                         value = ";".join(value)
                     # Ensures mapping option with value == None is not implemented. E.g. the links option
                     # can't be == None since there will be nothing to link to and that will raise a warning
                     if value is not None:
                         need_values[name] = value
 
                 for regex, new_str in self.mapping_replaces.items():
-                    need_values[name] = re.sub(regex, new_str, need_values.get(name, ""))
+                    need_values[name] = re.sub(
+                        regex, new_str, need_values.get(name, "")
+                    )
 
                 if name == "id":
                     need_values[name] = str(prefix) + str(need_values.get(name, ""))
 
             finale_data = {"content": content}
             finale_data.update(need_values)
 
             need_data.append(finale_data)
         return need_data
 
-    def request(self, options: Any = None, *args: Any, **kwargs: Any) -> Any:
+    def request_from_directive(
+        self, directive: SphinxDirective, /
+    ) -> list[dict[str, Any]]:
         self.log.info(f"Requesting data for service {self.name}")
         self._oauthorization()  # Get authorization token
-        params = self._prepare_request(options)
+        params = self._prepare_request(directive.options)
 
         request_params = {
             "url": params["url"],
             "headers": params["headers"],
         }
         answer = self._send_request(request_params)
         data = answer.json()
 
         for datum in data:
             # Be sure "description" is set and valid
             if "description" not in datum or datum["description"] is None:
                 datum["description"] = ""
 
-        need_data = self._extract_data(data, options)
+        need_data = self._extract_data(data, directive.options)
 
         return need_data
 
     def debug(self, *args: Any, **kwargs: Any) -> Any:
         self.log.debug(f"Requesting data for service {self.name}")
         self._oauthorization()  # Get authorization token
         params = self._prepare_request(*args)
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/templates/permalink.html` & `sphinx_needs-2.1.0/sphinx_needs/templates/permalink.html`

 * *Files 3% similar despite different names*

```diff
@@ -59,10 +59,11 @@
 
         window.addEventListener('DOMContentLoaded', main);
     </script>
 
 </head>
 
 <body>
+    <h1>Searching, Please Wait...</h1>
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -0,0 +1 @@
+************ SSeeaarrcchhiinngg,, PPlleeaassee WWaaiitt...... ************
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/templates/time_measurements.html` & `sphinx_needs-2.1.0/sphinx_needs/templates/time_measurements.html`

 * *Files identical despite different names*

### Comparing `sphinx_needs-2.0.0/sphinx_needs/utils.py` & `sphinx_needs-2.1.0/sphinx_needs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,24 @@
+from __future__ import annotations
+
 import cProfile
 import importlib
 import operator
 import os
 import re
 from functools import lru_cache, reduce, wraps
 from re import Pattern
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Callable, TypeVar
 from urllib.parse import urlparse
 
 from docutils import nodes
 from jinja2 import Environment, Template
 from sphinx.application import BuildEnvironment, Sphinx
 
-from sphinx_needs.config import NeedsSphinxConfig
+from sphinx_needs.config import LinkOptionsType, NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.defaults import NEEDS_PROFILING
 from sphinx_needs.logging import get_logger
 
 try:
     from typing import TypedDict
 except ImportError:
@@ -40,26 +31,27 @@
     from sphinx_needs.functions.functions import DynamicFunction
 
 logger = get_logger(__name__)
 
 
 class NeedFunctionsType(TypedDict):
     name: str
-    function: "DynamicFunction"
+    function: DynamicFunction
 
 
-NEEDS_FUNCTIONS: Dict[str, NeedFunctionsType] = {}
+NEEDS_FUNCTIONS: dict[str, NeedFunctionsType] = {}
 
 # List of internal need option names. They should not be used by or presented to user.
-INTERNALS = [
+INTERNALS = (
     "docname",
     "doctype",
     "lineno",
     "refid",
     "content",
+    "lineno_content",
     "pre_content",
     "post_content",
     "collapse",
     "parts",
     "id_parent",
     "id_complete",
     "title",
@@ -69,16 +61,14 @@
     "type_prefix",
     "type_color",
     "type_style",
     "type",
     "type_name",
     "id",
     "hide",
-    "hide_status",
-    "hide_tags",
     "sections",
     "section_name",
     "content_node",
     "content_id",
     # "parent_needs",
     "parent_need",
     # "child_needs",
@@ -87,15 +77,17 @@
     "is_modified",
     "modifications",
     "constraints",
     "constraints_passed",
     "constraints_results",
     "arch",
     "target_id",
-]
+    "has_dead_links",
+    "has_forbidden_dead_links",
+)
 
 MONTH_NAMES = [
     "January",
     "February",
     "March",
     "April",
     "May",
@@ -105,18 +97,34 @@
     "September",
     "October",
     "November",
     "December",
 ]
 
 
+def split_need_id(need_id_full: str) -> tuple[str, str | None]:
+    """A need id can be a combination of a main id and a part id,
+    split by a dot.
+    This function splits them:
+    If there is no dot, the part id is None,
+    otherwise everything before the first dot is the main id,
+    and everything after the first dot is the part id.
+    """
+    if "." in need_id_full:
+        need_id, need_part_id = need_id_full.split(".", maxsplit=1)
+    else:
+        need_id = need_id_full
+        need_part_id = None
+    return need_id, need_part_id
+
+
 def row_col_maker(
     app: Sphinx,
     fromdocname: str,
-    all_needs: Dict[str, NeedsInfoType],
+    all_needs: dict[str, NeedsInfoType],
     need_info: NeedsInfoType,
     need_key: str,
     make_ref: bool = False,
     ref_lookup: bool = False,
     prefix: str = "",
 ) -> nodes.entry:
     """
@@ -135,15 +143,15 @@
     builder = app.builder
     env = app.env
     needs_config = NeedsSphinxConfig(env.config)
 
     row_col = nodes.entry(classes=["needs_" + need_key])
     para_col = nodes.paragraph()
 
-    needs_string_links_option: List[str] = []
+    needs_string_links_option: list[str] = []
     for v in needs_config.string_links.values():
         needs_string_links_option.extend(v["options"])
 
     if need_key in need_info and need_info[need_key] is not None:  # type: ignore[literal-required]
         value = need_info[need_key]  # type: ignore[literal-required]
         if isinstance(value, (list, set)):
             data = value
@@ -162,16 +170,20 @@
                 link_list.append(link_type["option"])
                 link_list.append(link_type["option"] + "_back")
 
             # For needs_string_links
             link_string_list = {}
             for link_name, link_conf in needs_config.string_links.items():
                 link_string_list[link_name] = {
-                    "url_template": Environment(autoescape=True).from_string(link_conf["link_url"]),
-                    "name_template": Environment(autoescape=True).from_string(link_conf["link_name"]),
+                    "url_template": Environment(autoescape=True).from_string(
+                        link_conf["link_url"]
+                    ),
+                    "name_template": Environment(autoescape=True).from_string(
+                        link_conf["link_name"]
+                    ),
                     "regex_compiled": re.compile(link_conf["regex"]),
                     "options": link_conf["options"],
                     "name": link_name,
                 }
 
             matching_link_confs = []
             for link_conf in link_string_list.values():
@@ -192,70 +204,88 @@
                         # Mark references as "internal" so that if the rinohtype builder is being used it produces an
                         # internal reference within the generated PDF instead of an external link. This replicates the
                         # behaviour of references created with the sphinx utility `make_refnode`.
                         ref_col = nodes.reference("", "", internal=True)
 
                     if make_ref:
                         if need_info["is_external"]:
-                            assert need_info["external_url"] is not None, "external_url must be set for external needs"
-                            ref_col["refuri"] = check_and_calc_base_url_rel_path(need_info["external_url"], fromdocname)
+                            assert (
+                                need_info["external_url"] is not None
+                            ), "external_url must be set for external needs"
+                            ref_col["refuri"] = check_and_calc_base_url_rel_path(
+                                need_info["external_url"], fromdocname
+                            )
                             ref_col["classes"].append(need_info["external_css"])
                             row_col["classes"].append(need_info["external_css"])
-                        else:
-                            ref_col["refuri"] = builder.get_relative_uri(fromdocname, need_info["docname"])
+                        elif _docname := need_info["docname"]:
+                            ref_col["refuri"] = builder.get_relative_uri(
+                                fromdocname, _docname
+                            )
                             ref_col["refuri"] += "#" + datum
                     elif ref_lookup:
                         temp_need = all_needs[link_id]
                         if temp_need["is_external"]:
-                            assert temp_need["external_url"] is not None, "external_url must be set for external needs"
-                            ref_col["refuri"] = check_and_calc_base_url_rel_path(temp_need["external_url"], fromdocname)
+                            assert (
+                                temp_need["external_url"] is not None
+                            ), "external_url must be set for external needs"
+                            ref_col["refuri"] = check_and_calc_base_url_rel_path(
+                                temp_need["external_url"], fromdocname
+                            )
                             ref_col["classes"].append(temp_need["external_css"])
                             row_col["classes"].append(temp_need["external_css"])
-                        else:
-                            ref_col["refuri"] = builder.get_relative_uri(fromdocname, temp_need["docname"])
+                        elif _docname := temp_need["docname"]:
+                            ref_col["refuri"] = builder.get_relative_uri(
+                                fromdocname, _docname
+                            )
                             ref_col["refuri"] += "#" + temp_need["id"]
                             if link_part:
                                 ref_col["refuri"] += "." + link_part
 
                 except KeyError:
                     para_col += text_col
                 else:
                     ref_col.append(text_col)
                     para_col += ref_col
             elif matching_link_confs:
                 para_col += match_string_link(
-                    datum_text, datum, need_key, matching_link_confs, render_context=needs_config.render_context
+                    datum_text,
+                    datum,
+                    need_key,
+                    matching_link_confs,
+                    render_context=needs_config.render_context,
                 )
             else:
                 para_col += text_col
 
             if index + 1 < len(data):
                 para_col += nodes.emphasis("; ", "; ")
 
     row_col += para_col
 
     return row_col
 
 
-def rstjinja(app: Sphinx, docname: str, source: List[str]) -> None:
+def rstjinja(app: Sphinx, docname: str, source: list[str]) -> None:
     """
     Render our pages as a jinja template for fancy templating goodness.
     """
     builder = app.builder
     # Make sure we're outputting HTML
     if builder.format != "html":
         return
     src = source[0]
     rendered = builder.templates.render_string(
         src, app.config.html_context, **NeedsSphinxConfig(app.config).render_context
     )
     source[0] = rendered
 
 
-def import_prefix_link_edit(needs: Dict[str, Any], id_prefix: str, needs_extra_links: List[Dict[str, Any]]) -> None:
+def import_prefix_link_edit(
+    needs: dict[str, Any], id_prefix: str, needs_extra_links: list[LinkOptionsType]
+) -> None:
     """
     Changes existing links to support given prefix.
     Only link-ids get touched, which are part of ``needs`` (so are linking them).
     Other links do not get the prefix, as they are treated as "external" links.
 
     :param needs: Dict of all needs
     :param id_prefix: Prefix as string
@@ -274,15 +304,17 @@
             for extra_link in needs_extra_links:
                 if extra_link["option"] in need and id in need[extra_link["option"]]:
                     for n, link in enumerate(need[extra_link["option"]]):
                         if id == link:
                             need[extra_link["option"]][n] = f"{id_prefix}{id}"
             # Manipulate descriptions
             # ToDo: Use regex for better matches.
-            need["description"] = need["description"].replace(id, "".join([id_prefix, id]))
+            need["description"] = need["description"].replace(
+                id, "".join([id_prefix, id])
+            )
 
 
 FuncT = TypeVar("FuncT")
 
 
 def profile(keyword: str) -> Callable[[FuncT], FuncT]:
     """
@@ -321,90 +353,103 @@
     """
     ref_uri = external_url
     # check if given base_url is url or relative path
     parsed_url = urlparse(external_url)
     # get path sep considering plattform dependency, '\' for Windows, '/' fro Unix
     curr_path_sep = os.path.sep
     # check / or \ to determine the relative path to conf.py directory
-    if not parsed_url.scheme and not os.path.isabs(external_url) and curr_path_sep in fromdocname:
+    if (
+        not parsed_url.scheme
+        and not os.path.isabs(external_url)
+        and curr_path_sep in fromdocname
+    ):
         sub_level = len(fromdocname.split(curr_path_sep)) - 1
         ref_uri = os.path.join(sub_level * (".." + curr_path_sep), external_url)
 
     return ref_uri
 
 
-def check_and_get_external_filter_func(filter_func_ref: Optional[str]) -> Tuple[Any, str]:
+def check_and_get_external_filter_func(filter_func_ref: str | None) -> tuple[Any, str]:
     """Check and import filter function from external python file."""
     # Check if external filter code is defined
     filter_func = None
     filter_args = ""
 
     if filter_func_ref:
         try:
             filter_module, filter_function = filter_func_ref.rsplit(".")
         except ValueError:
             logger.warning(
-                f'Filter function not valid "{filter_func_ref}". Example: my_module:my_func [needs]', type="needs"
+                f'Filter function not valid "{filter_func_ref}". Example: my_module:my_func [needs]',
+                type="needs",
             )
             return filter_func, filter_args
 
         result = re.search(r"^(\w+)(?:\((.*)\))*$", filter_function)
         if not result:
             return filter_func, filter_args
         filter_function = result.group(1)
         filter_args = result.group(2) or ""
 
         try:
             final_module = importlib.import_module(filter_module)
             filter_func = getattr(final_module, filter_function)
         except Exception:
-            logger.warning(f"Could not import filter function: {filter_func_ref} [needs]", type="needs")
+            logger.warning(
+                f"Could not import filter function: {filter_func_ref} [needs]",
+                type="needs",
+            )
             return filter_func, filter_args
 
     return filter_func, filter_args
 
 
-def jinja_parse(context: Dict[str, Any], jinja_string: str) -> str:
+def jinja_parse(context: dict[str, Any], jinja_string: str) -> str:
     """
     Function to parse mapping options set to a string containing jinja template format.
 
     :param context: Data to be used as context in rendering jinja template
     :type context: dict
     :param jinja_string: A jinja template string
     :type jinja_string: str
     :return: A rendered jinja template as string
     :rtype: str
 
     """
     try:
         content_template = Template(jinja_string, autoescape=True)
     except Exception as e:
-        raise ReferenceError(f'There was an error in the jinja statement: "{jinja_string}". ' f"Error Msg: {e}")
+        raise ReferenceError(
+            f'There was an error in the jinja statement: "{jinja_string}". '
+            f"Error Msg: {e}"
+        )
 
     content = content_template.render(**context)
     return content
 
 
-@lru_cache()
-def import_matplotlib() -> Optional["matplotlib"]:
+@lru_cache
+def import_matplotlib() -> matplotlib | None:
     """Import and return matplotlib, or return None if it cannot be imported.
 
     Also sets the interactive backend to ``Agg``, if ``DISPLAY`` is not set.
     """
     try:
         import matplotlib
         import matplotlib.pyplot
     except ImportError:
         return None
     if not os.environ.get("DISPLAY"):
         matplotlib.use("Agg")
     return matplotlib
 
 
-def save_matplotlib_figure(app: Sphinx, figure: "FigureBase", basename: str, fromdocname: str) -> nodes.image:
+def save_matplotlib_figure(
+    app: Sphinx, figure: FigureBase, basename: str, fromdocname: str
+) -> nodes.image:
     builder = app.builder
     env = app.env
 
     image_folder = os.path.join(builder.outdir, builder.imagedir)
     os.makedirs(image_folder, exist_ok=True)
 
     # Determine a common mimetype between matplotlib and the builder.
@@ -435,15 +480,15 @@
 
     # look at uri value for source path, relative to the srcdir folder
     image_node["candidates"] = {mimetype: abs_file_path}
 
     return image_node
 
 
-def dict_get(root: Dict[str, Any], items: Any, default: Any = None) -> Any:
+def dict_get(root: dict[str, Any], items: Any, default: Any = None) -> Any:
     """
     Access a nested object in root by item sequence.
 
     Usage::
        data = {"nested": {"a_list": [{"finally": "target_data"}]}}
        value = dict_get(["nested", "a_list", 0, "finally"], "Not_found")
 
@@ -453,70 +498,88 @@
     except (KeyError, IndexError, TypeError) as e:
         logger.debug(e)
         return default
     return value
 
 
 def match_string_link(
-    text_item: str, data: str, need_key: str, matching_link_confs: List[Dict[str, Any]], render_context: Dict[str, Any]
+    text_item: str,
+    data: str,
+    need_key: str,
+    matching_link_confs: list[dict[str, Any]],
+    render_context: dict[str, Any],
 ) -> Any:
     try:
         link_name = None
         link_url = None
-        link_conf = matching_link_confs[0]  # We only handle the first matching string_link
+        link_conf = matching_link_confs[
+            0
+        ]  # We only handle the first matching string_link
         match = link_conf["regex_compiled"].search(data)
         if match:
             render_content = match.groupdict()
-            link_url = link_conf["url_template"].render(**render_content, **render_context)
-            link_name = link_conf["name_template"].render(**render_content, **render_context)
-        if link_name:
-            ref_item = nodes.reference(link_name, link_name, refuri=link_url)
-        else:
-            # if no string_link match was made, we handle it as normal string value
-            ref_item = nodes.Text(text_item)
+            link_url = link_conf["url_template"].render(
+                **render_content, **render_context
+            )
+            link_name = link_conf["name_template"].render(
+                **render_content, **render_context
+            )
+
+        # if no string_link match was made, we handle it as normal string value
+        ref_item = (
+            nodes.reference(link_name, link_name, refuri=link_url)
+            if link_name
+            else nodes.Text(text_item)
+        )
 
     except Exception as e:
         logger.warning(
             f'Problems dealing with string to link transformation for value "{data}" of '
             f'option "{need_key}". Error: {e} [needs]',
             type="needs",
         )
     else:
         return ref_item
 
 
 def match_variants(
-    option_value: Union[str, List[str]], keywords: Dict[str, Any], needs_variants: Dict[str, str]
-) -> Union[None, str, List[str]]:
+    option_value: str | list[str],
+    keywords: dict[str, Any],
+    needs_variants: dict[str, str],
+) -> None | str | list[str]:
     """
     Function to handle variant option management.
 
     :param option_value: Value assigned to an option
     :param keywords: Data to use as filtering context
     :param needs_variants: Needs variants data set in users conf.py
     :return: A string, list, or None to be used as value for option.
     :rtype: Union[str, List, None]
     """
 
     def variant_handling(
-        variant_definitions: List[str], variant_data: Dict[str, Any], variant_pattern: Pattern  # type: ignore[type-arg]
-    ) -> Optional[str]:
+        variant_definitions: list[str],
+        variant_data: dict[str, Any],
+        variant_pattern: Pattern,  # type: ignore[type-arg]
+    ) -> str | None:
         filter_context = variant_data
         # filter_result = []
         no_variants_in_option = False
         variants_in_option = False
         for variant_definition in variant_definitions:
             # Test if definition is a variant definition
             check_definition = variant_pattern.search(variant_definition)
             if check_definition:
                 variants_in_option = True
                 # Separate variant definition from value to use for the option
-                filter_string, output, _ = re.split(r"(:[\w':.\-\" ]+)$", variant_definition)
+                filter_string, output, _ = re.split(
+                    r"(:[\w':.\-\" ]+)$", variant_definition
+                )
                 filter_string = re.sub(r"^\[|[:\]]$", "", filter_string)
-                filter_string = needs_variants[filter_string] if filter_string in needs_variants else filter_string
+                filter_string = needs_variants.get(filter_string, filter_string)
                 try:
                     # https://docs.python.org/3/library/functions.html?highlight=compile#compile
                     filter_compiled = compile(filter_string, "<string>", "eval")
                     # Set filter_context as globals and not only locals in eval()!
                     # Otherwise, the vars not be accessed in list comprehensions.
                     if filter_compiled:
                         eval_result = bool(eval(filter_compiled, filter_context))
@@ -524,15 +587,16 @@
                         eval_result = bool(eval(filter_string, filter_context))
                     # First matching variant definition defines the output
                     if eval_result:
                         no_variants_in_option = False
                         return output.lstrip(":")
                 except Exception as e:
                     logger.warning(
-                        f'There was an error in the filter statement: "{filter_string}". ' f"Error Msg: {e} [needs]",
+                        f'There was an error in the filter statement: "{filter_string}". '
+                        f"Error Msg: {e} [needs]",
                         type="needs",
                     )
             else:
                 no_variants_in_option = True
 
         if no_variants_in_option and not variants_in_option:
             return None
@@ -546,33 +610,43 @@
     split_pattern = r"([\[\]]{1}[\w=:'. \-\"]+[\[\(\{]{1}[\w=,.': \-\"]*[\]\)\}]{1}[\[\]]{1}:[\w.\- ]+)|([\[\]]{1}[\w=:.'\-\[\] \"]+[\[\]]{1}:[\w.\- ]+)|([\w.: ]+[,;]{1})"
     variant_rule_pattern = r"^[\w'=,:.\-\"\[\] ]+:[\w'=:.\-\"\[\] ]+$"
     variant_splitting = re.compile(split_pattern)
     variant_rule_matching = re.compile(variant_rule_pattern)
 
     # Handling multiple variant definitions
     if isinstance(option_value, str):
-        multiple_variants: List[str] = variant_splitting.split(rf"""{option_value}""")
+        multiple_variants: list[str] = variant_splitting.split(rf"""{option_value}""")
         multiple_variants = [
-            re.sub(r"^([;, ]+)|([;, ]+$)", "", i) for i in multiple_variants if i not in (None, ";", "", " ")
+            re.sub(r"^([;, ]+)|([;, ]+$)", "", i)
+            for i in multiple_variants
+            if i not in (None, ";", "", " ")
         ]
-        if len(multiple_variants) == 1 and not variant_rule_matching.search(multiple_variants[0]):
+        if len(multiple_variants) == 1 and not variant_rule_matching.search(
+            multiple_variants[0]
+        ):
             return option_value
-        new_option_value = variant_handling(multiple_variants, keywords, variant_rule_matching)
+        new_option_value = variant_handling(
+            multiple_variants, keywords, variant_rule_matching
+        )
         if new_option_value is None:
             return option_value
         return new_option_value
     elif isinstance(option_value, (list, set, tuple)):
         multiple_variants = list(option_value)
         # In case an option value is a list (:tags: open; close), and does not contain any variant definition,
         # then return the unmodified value
         # options = all([bool(not variant_rule_matching.search(i)) for i in multiple_variants])
-        options = all(bool(not variant_rule_matching.search(i)) for i in multiple_variants)
+        options = all(
+            bool(not variant_rule_matching.search(i)) for i in multiple_variants
+        )
         if options:
             return option_value
-        new_option_value = variant_handling(multiple_variants, keywords, variant_rule_matching)
+        new_option_value = variant_handling(
+            multiple_variants, keywords, variant_rule_matching
+        )
         return new_option_value
     else:
         return option_value
 
 
 pattern = r"(https://|http://|www\.|[\w]*?)([\w\-/.]+):([\w\-/.]+)@([\w\-/.]+)"
 data_compile = re.compile(pattern)
@@ -587,15 +661,17 @@
     :return: Cleaned login string or None
     """
 
     clean_credentials = data_compile.sub(r"\1****:****@\4", data)
     return clean_credentials
 
 
-def node_match(node_types: Union[Type[nodes.Element], List[Type[nodes.Element]]]) -> Callable[[nodes.Node], bool]:
+def node_match(
+    node_types: type[nodes.Element] | list[type[nodes.Element]],
+) -> Callable[[nodes.Node], bool]:
     """
     Returns a condition function for doctuils.nodes.findall()
 
     It takes a single or a list of node-types, if a findall() finds that node-type, the node
     get returned by findall() inside a generator-object.
 
     Use it like::
@@ -609,34 +685,36 @@
             raise Exception('Not requested node type')
 
     :param node_types: List of docutils node types
     :return: function, which can be used as constraint-function for docutils findall()
     """
     node_types_list = node_types if isinstance(node_types, list) else [node_types]
 
-    def condition(node: nodes.Node, node_types: List[Type[nodes.Element]] = node_types_list) -> bool:
+    def condition(
+        node: nodes.Node, node_types: list[type[nodes.Element]] = node_types_list
+    ) -> bool:
         return any(isinstance(node, x) for x in node_types)
 
     return condition
 
 
-def add_doc(env: BuildEnvironment, docname: str, category: Optional[str] = None) -> None:
+def add_doc(env: BuildEnvironment, docname: str, category: str | None = None) -> None:
     """Stores a docname, to know later all need-relevant docs"""
     docs = SphinxNeedsData(env).get_or_create_docs()
     if docname not in docs["all"]:
         docs["all"].append(docname)
 
     if category:
         if category not in docs:
             docs[category] = []
         if docname not in docs[category]:
             docs[category].append(docname)
 
 
-def split_link_types(link_types: str, location: Any) -> List[str]:
+def split_link_types(link_types: str, location: Any) -> list[str]:
     """Split link_types string into list of link_types."""
 
     def _is_valid(link_type: str) -> bool:
         if len(link_type) == 0 or link_type.isspace():
             logger.warning(
                 "Scruffy link_type definition found. Defined link_type contains spaces only. [needs]",
                 type="needs",
@@ -649,15 +727,15 @@
         filter(
             _is_valid,
             (x.strip() for x in re.split(";|,", link_types)),
         )
     )
 
 
-def get_scale(options: Dict[str, Any], location: Any) -> str:
+def get_scale(options: dict[str, Any], location: Any) -> str:
     """Get scale for diagram, from directive option."""
     scale: str = options.get("scale", "100").replace("%", "")
     if not scale.isdigit():
         logger.warning(
             f'scale value must be a number. "{scale}" found [needs]',
             type="needs",
             location=location,
```

### Comparing `sphinx_needs-2.0.0/sphinx_needs/warnings.py` & `sphinx_needs-2.1.0/sphinx_needs/warnings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Cares about handling and execution warnings.
 
 """
-from typing import Dict, Optional
+
+from __future__ import annotations
 
 from sphinx.application import Sphinx
 from sphinx.util import logging
 
 from sphinx_needs.config import NEEDS_CONFIG, NeedsSphinxConfig
 from sphinx_needs.data import NeedsInfoType, SphinxNeedsData
 from sphinx_needs.filter_common import filter_needs
 from sphinx_needs.logging import get_logger
 
 logger = get_logger(__name__)
 
 
-def process_warnings(app: Sphinx, exception: Optional[Exception]) -> None:
+def process_warnings(app: Sphinx, exception: Exception | None) -> None:
     """
     Checks the configured warnings.
 
     This func gets called by the latest sphinx-event, so that really everything is already done.
 
     :param app: application
     :param exception: raised exceptions
@@ -42,37 +43,45 @@
     # on first execution
     if hasattr(env, "needs_warnings_executed") and env.needs_warnings_executed:
         return
 
     env.needs_warnings_executed = True  # type: ignore[attr-defined]
 
     # Exclude external needs for warnings check
-    checked_needs: Dict[str, NeedsInfoType] = {}
+    checked_needs: dict[str, NeedsInfoType] = {}
     for need_id, need in needs.items():
         if not need["is_external"]:
             checked_needs[need_id] = need
 
     needs_config = NeedsSphinxConfig(app.config)
     warnings_always_warn = needs_config.warnings_always_warn
 
     with logging.pending_logging():
         logger.info("\nChecking sphinx-needs warnings")
         warning_raised = False
         for warning_name, warning_filter in NEEDS_CONFIG.warnings.items():
             if isinstance(warning_filter, str):
                 # filter string used
-                result = filter_needs(checked_needs.values(), needs_config, warning_filter)
+                result = filter_needs(
+                    checked_needs.values(),
+                    needs_config,
+                    warning_filter,
+                    append_warning=f"(from warning filter {warning_name!r})",
+                )
             elif callable(warning_filter):
                 # custom defined filter code used from conf.py
                 result = []
                 for need in checked_needs.values():
                     if warning_filter(need, logger):
                         result.append(need)
             else:
-                logger.warning(f"Unknown needs warnings filter {warning_filter}! [needs]", type="needs")
+                logger.warning(
+                    f"Unknown needs warnings filter {warning_filter}! [needs]",
+                    type="needs",
+                )
 
             if len(result) == 0:
                 logger.info(f"{warning_name}: passed")
             else:
                 need_ids = [x["id"] for x in result]
 
                 # Set Sphinx statuscode to 1, only if -W is used with sphinx-build
@@ -89,21 +98,30 @@
                     warning_text = warning_filter.__name__
                 elif isinstance(warning_filter, str):
                     warning_text = warning_filter
 
                 if warnings_always_warn:
                     logger.warning(
                         "{}: failed\n\t\tfailed needs: {} ({})\n\t\tused filter: {} [needs]".format(
-                            warning_name, len(need_ids), ", ".join(need_ids), warning_text
+                            warning_name,
+                            len(need_ids),
+                            ", ".join(need_ids),
+                            warning_text,
                         ),
                         type="needs",
                     )
                 else:
                     logger.info(
                         "{}: failed\n\t\tfailed needs: {} ({})\n\t\tused filter: {}".format(
-                            warning_name, len(need_ids), ", ".join(need_ids), warning_text
+                            warning_name,
+                            len(need_ids),
+                            ", ".join(need_ids),
+                            warning_text,
                         )
                     )
                     warning_raised = True
 
         if warning_raised:
-            logger.warning("warnings were raised. See console / log output for details. [needs]", type="needs")
+            logger.warning(
+                "warnings were raised. See console / log output for details. [needs]",
+                type="needs",
+            )
```

### Comparing `sphinx_needs-2.0.0/PKG-INFO` & `sphinx_needs-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-needs
-Version: 2.0.0
+Version: 2.1.0
 Summary: Sphinx needs extension for managing needs/requirements and specifications
 Home-page: http://github.com/useblocks/sphinx-needs
 License: MIT
 Author: team useblocks
 Author-email: info@useblocks.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,27 +22,27 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Provides-Extra: benchmark
 Provides-Extra: docs
 Provides-Extra: plotting
 Provides-Extra: test
 Provides-Extra: test-parallel
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0) ; extra == "test"
 Requires-Dist: jsonschema (>=3.2.0)
 Requires-Dist: lxml (>=4.6.5,<5.0.0) ; extra == "test"
 Requires-Dist: matplotlib (>=3.3.0) ; extra == "plotting" or extra == "test" or extra == "docs"
 Requires-Dist: memray (>=1.3.1,<2.0.0) ; extra == "benchmark"
 Requires-Dist: pydantic (==2.4.2) ; extra == "docs"
 Requires-Dist: pytest (>=7,<8) ; extra == "test"
 Requires-Dist: pytest-benchmark (>=4.0.0,<5.0.0) ; extra == "benchmark"
 Requires-Dist: pytest-cov (>=4,<5) ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test-parallel"
 Requires-Dist: pytest-xprocess (>=0.22.2,<0.23.0) ; extra == "test"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: requests-file (>=1.5.1,<2.0.0)
-Requires-Dist: requests-mock (>=1.9.3) ; extra == "test"
 Requires-Dist: responses (>=0.22.0,<0.23.0) ; extra == "test"
 Requires-Dist: sphinx (>=5.0,<8)
 Requires-Dist: sphinx-copybutton (>=0.5,<0.6) ; extra == "docs"
 Requires-Dist: sphinx-data-viewer (>=0.1.1,<0.2.0)
 Requires-Dist: sphinx-design (>=0.5,<0.6) ; extra == "docs"
 Requires-Dist: sphinx-immaterial (==0.11.7) ; extra == "docs"
 Requires-Dist: sphinxcontrib-jquery (>=4,<5)
```

