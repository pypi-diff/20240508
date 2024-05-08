# Comparing `tmp/saenopy-1.0.2.tar.gz` & `tmp/saenopy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saenopy-1.0.2.tar", max compression
+gzip compressed data, was "saenopy-1.0.4.tar", max compression
```

## Comparing `saenopy-1.0.2.tar` & `saenopy-1.0.4.tar`

### file list

```diff
@@ -1,115 +1,178 @@
--rw-r--r--   0        0        0     1065 2023-07-28 17:42:27.967829 saenopy-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2183 2023-07-28 17:42:27.967829 saenopy-1.0.2/README.md
--rw-r--r--   0        0        0     1307 2023-07-28 17:42:28.087828 saenopy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      348 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/build_beams.py
--rw-r--r--   0        0        0     1279 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/conjugate_gradient.py
--rw-r--r--   0        0        0     7716 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/examples.py
--rw-r--r--   0        0        0    15307 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/get_deformations.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/__init__.py
--rw-r--r--   0        0        0     3918 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/code_editor.py
--rw-r--r--   0        0        0     7389 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/gui_code.py
--rw-r--r--   0        0        0     4605 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/script_file.py
--rw-r--r--   0        0        0     7099 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/syntax.py
--rw-r--r--   0        0        0    19372 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/QExtendedGraphicsView.py
--rw-r--r--   0        0        0    46067 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/QtShortCuts.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/__init__.py
--rw-r--r--   0        0        0    21886 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/gui_classes.py
--rw-r--r--   0        0        0    33357 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/lif_reader.py
--rw-r--r--   0        0        0     6027 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/patch_lifreader.py
--rw-r--r--   0        0        0      282 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/resources.py
--rw-r--r--   0        0        0    15449 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/sigmoid_widget.py
--rw-r--r--   0        0        0     6583 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_preview.py
--rw-r--r--   0        0        0     3848 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector.py
--rw-r--r--   0        0        0    10884 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_crop.py
--rw-r--r--   0        0        0     3096 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_leica.py
--rw-r--r--   0        0        0    12184 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_tif.py
--rw-r--r--   0        0        0     7932 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/gui_master.py
--rw-r--r--   0        0        0    16079 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/material_fit/gui_fit.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/orientation/__init__.py
--rw-r--r--   0        0        0    51650 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/orientation/gui_orientation.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/analyze/__init__.py
--rw-r--r--   0        0        0    20715 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/analyze/plot_window.py
--rw-r--r--   0        0        0     1575 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/gui_solver.py
--rw-r--r--   0        0        0    16215 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/BatchEvaluate.py
--rw-r--r--   0        0        0    11801 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/DeformationDetector.py
--rw-r--r--   0        0        0     4203 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/FittedMesh.py
--rw-r--r--   0        0        0    11660 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/MeshCreator.py
--rw-r--r--   0        0        0    10563 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/PipelineModule.py
--rw-r--r--   0        0        0     1103 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/QTimeSlider.py
--rw-r--r--   0        0        0    15201 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/Regularizer.py
--rw-r--r--   0        0        0    11278 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/ResultView.py
--rw-r--r--   0        0        0    20076 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/StackDisplay.py
--rw-r--r--   0        0        0    12999 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/VTK_Toolbar.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/__init__.py
--rw-r--r--   0        0        0      541 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/code_export.py
--rw-r--r--   0        0        0     6645 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
--rw-r--r--   0        0        0    48390 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/Exporter.py
--rw-r--r--   0        0        0    13704 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
--rw-r--r--   0        0        0    17357 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
--rw-r--r--   0        0        0    18697 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/FiberViewer.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/__init__.py
--rw-r--r--   0        0        0    11704 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/load_measurement_dialog.py
--rw-r--r--   0        0        0     3868 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/path_editor.py
--rw-r--r--   0        0        0    12328 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/showVectorField.py
--rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/spheroid/__init__.py
--rw-r--r--   0        0        0    93350 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/spheroid/gui_deformation_spheroid.py
--rw-r--r--   0        0        0    53944 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Icon.ico
--rw-r--r--   0        0        0    42217 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo.png
--rw-r--r--   0        0        0    88874 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo.svg
--rw-r--r--   0        0        0    37691 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo_black.png
--rw-r--r--   0        0        0    19301 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame00.png
--rw-r--r--   0        0        0    19413 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame01.png
--rw-r--r--   0        0        0    19360 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame02.png
--rw-r--r--   0        0        0    19344 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame03.png
--rw-r--r--   0        0        0    19267 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame04.png
--rw-r--r--   0        0        0    18999 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame05.png
--rw-r--r--   0        0        0    31030 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame06.png
--rw-r--r--   0        0        0    32933 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame07.png
--rw-r--r--   0        0        0    34748 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame08.png
--rw-r--r--   0        0        0    35475 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame09.png
--rw-r--r--   0        0        0    37528 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame10.png
--rw-r--r--   0        0        0    39777 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame11.png
--rw-r--r--   0        0        0    41902 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame12.png
--rw-r--r--   0        0        0    41897 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame13.png
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/arrowscale.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/autoscale0.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/autoscale1.ico
--rw-r--r--   0        0        0    48947 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/buttons.svg
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/center0.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/center1.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/contrast0.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/contrast1.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid2.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid3.ico
--rw-r--r--   0        0        0    38885 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/logo_splash.png
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/nan0.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/nan1.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image2.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image3.ico
--rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice0.ico
--rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice1.ico
--rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice2.ico
--rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice_all.ico
--rw-r--r--   0        0        0   121664 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/BFTFM.png
--rw-r--r--   0        0        0   132449 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/BFTFM_2.png
--rw-r--r--   0        0        0   180081 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/Bead_example_icon.png
--rw-r--r--   0        0        0   202759 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/Dynamic_icon.png
--rw-r--r--   0        0        0   554429 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/StainedOrganoid_icon.png
--rw-r--r--   0        0        0   263760 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/liver_fibroblast_icon.png
--rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/view_single.ico
--rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/view_two.ico
--rw-r--r--   0        0        0    12316 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/macro.py
--rw-r--r--   0        0        0    12253 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/materials.py
--rw-r--r--   0        0        0     3701 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/mesh.py
--rw-r--r--   0        0        0     5635 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/multigrid_helper.py
--rw-r--r--   0        0        0    24079 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/result_file.py
--rw-r--r--   0        0        0     7754 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/saveable.py
--rw-r--r--   0        0        0    47872 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/solver.py
--rw-r--r--   0        0        0    11130 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/stack.py
--rw-r--r--   0        0        0    17259 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/unused/macro.py
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-08 11:51:01.378636 saenopy-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     2183 2024-05-08 11:51:01.378636 saenopy-1.0.4/README.md
+-rw-r--r--   0        0        0     1526 2024-05-08 11:51:01.506637 saenopy-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      444 2024-05-08 11:51:01.506637 saenopy-1.0.4/saenopy/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-08 11:51:01.506637 saenopy-1.0.4/saenopy/build_beams.py
+-rw-r--r--   0        0        0     1279 2024-05-08 11:51:01.506637 saenopy-1.0.4/saenopy/conjugate_gradient.py
+-rw-r--r--   0        0        0    13566 2024-05-08 11:51:01.506637 saenopy-1.0.4/saenopy/examples.py
+-rw-r--r--   0        0        0     5261 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/export_html.py
+-rw-r--r--   0        0        0    15307 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/get_deformations.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code/code_editor.py
+-rw-r--r--   0        0        0     7386 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code/gui_code.py
+-rw-r--r--   0        0        0     4605 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code/script_file.py
+-rw-r--r--   0        0        0     7099 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code/syntax.py
+-rw-r--r--   0        0        0     4782 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/code_evluate_normal.py
+-rw-r--r--   0        0        0     7443 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/AddFilesDialog.py
+-rw-r--r--   0        0        0    12869 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/BatchEvaluate.py
+-rw-r--r--   0        0        0     2375 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/ModuleColorBar.py
+-rw-r--r--   0        0        0     2024 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/ModuleScaleBar.py
+-rw-r--r--   0        0        0    11040 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/PipelineModule.py
+-rw-r--r--   0        0        0    19372 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/QExtendedGraphicsView.py
+-rw-r--r--   0        0        0     1103 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/QTimeSlider.py
+-rw-r--r--   0        0        0    46833 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/QtShortCuts.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/__init__.py
+-rw-r--r--   0        0        0      541 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/code_export.py
+-rw-r--r--   0        0        0    23134 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/gui_classes.py
+-rw-r--r--   0        0        0    33357 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/lif_reader.py
+-rw-r--r--   0        0        0     6027 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/patch_lifreader.py
+-rw-r--r--   0        0        0    20008 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/plot_window.py
+-rw-r--r--   0        0        0      282 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/resources.py
+-rw-r--r--   0        0        0    15449 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/sigmoid_widget.py
+-rw-r--r--   0        0        0     6575 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/stack_preview.py
+-rw-r--r--   0        0        0     3848 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/stack_selector.py
+-rw-r--r--   0        0        0    10886 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/stack_selector_crop.py
+-rw-r--r--   0        0        0     3096 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/stack_selector_leica.py
+-rw-r--r--   0        0        0    12184 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/common/stack_selector_tif.py
+-rw-r--r--   0        0        0    10273 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/gui_master.py
+-rw-r--r--   0        0        0    16080 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/material_fit/gui_fit.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/orientation/__init__.py
+-rw-r--r--   0        0        0    48069 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/orientation/gui_orientation.py
+-rw-r--r--   0        0        0     5509 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/orientation/modules/AddFilesDialog.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/analyze/__init__.py
+-rw-r--r--   0        0        0     2539 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/analyze/plot_window.py
+-rw-r--r--   0        0        0     1595 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/gui_solver.py
+-rw-r--r--   0        0        0     6167 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    11855 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4239 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/FittedMesh.py
+-rw-r--r--   0        0        0    11714 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/MeshCreator.py
+-rw-r--r--   0        0        0    15303 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/Regularizer.py
+-rw-r--r--   0        0        0    11314 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/ResultView.py
+-rw-r--r--   0        0        0    18228 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/StackDisplay.py
+-rw-r--r--   0        0        0    13362 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/VTK_Toolbar.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/__init__.py
+-rw-r--r--   0        0        0     5175 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
+-rw-r--r--   0        0        0    50770 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/Exporter.py
+-rw-r--r--   0        0        0    18284 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
+-rw-r--r--   0        0        0    17907 2024-05-08 11:51:01.510637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
+-rw-r--r--   0        0        0    18683 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/FiberViewer.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/solver/modules/exporter/__init__.py
+-rw-r--r--   0        0        0     5597 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/solver/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     3868 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/solver/modules/path_editor.py
+-rw-r--r--   0        0        0    12680 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/solver/modules/showVectorField.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/analyze/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/analyze/plot_window.py
+-rw-r--r--   0        0        0     6665 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/gui_deformation_spheroid.py
+-rw-r--r--   0        0        0     5687 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/AddFilesDialog.py
+-rw-r--r--   0        0        0     2571 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    17175 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4385 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/ForceCalculator.py
+-rw-r--r--   0        0        0     5065 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/ListWidget.py
+-rw-r--r--   0        0        0    20838 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/LookupTable.py
+-rw-r--r--   0        0        0     2012 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/MatplotlibWidget.py
+-rw-r--r--   0        0        0     1501 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/QSlider.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/__init__.py
+-rw-r--r--   0        0        0      865 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/helper.py
+-rw-r--r--   0        0        0     2484 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/path_editor.py
+-rw-r--r--   0        0        0     8079 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/spheroid/modules/result.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/analyze/__init__.py
+-rw-r--r--   0        0        0     5964 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/analyze/plot_window.py
+-rw-r--r--   0        0        0     1585 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/gui_2d.py
+-rw-r--r--   0        0        0     9927 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0     4845 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/CalculateDisplacements.py
+-rw-r--r--   0        0        0     2597 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/CalculateForceGeneration.py
+-rw-r--r--   0        0        0     4271 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/CalculateForces.py
+-rw-r--r--   0        0        0     3009 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/CalculateStress.py
+-rw-r--r--   0        0        0     2102 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/DisplayCellImage.py
+-rw-r--r--   0        0        0     2340 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/DisplayDeformed.py
+-rw-r--r--   0        0        0      550 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/DisplayRelaxed.py
+-rw-r--r--   0        0        0    10491 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/PipelineModule.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/__init__.py
+-rw-r--r--   0        0        0    11084 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/draw.py
+-rw-r--r--   0        0        0     3069 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     2298 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/path_editor.py
+-rw-r--r--   0        0        0    10133 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tfm2d/modules/result.py
+-rw-r--r--   0        0        0     9986 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tmp/render_results2.py
+-rw-r--r--   0        0        0     3047 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/gui/tmp/render_surface_comparison.py
+-rw-r--r--   0        0        0    53944 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/Icon.ico
+-rw-r--r--   0        0        0    42217 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/Logo.png
+-rw-r--r--   0        0        0    88874 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/Logo.svg
+-rw-r--r--   0        0        0    37691 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/Logo_black.png
+-rw-r--r--   0        0        0    19301 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/animation/frame00.png
+-rw-r--r--   0        0        0    19413 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/animation/frame01.png
+-rw-r--r--   0        0        0    19360 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/animation/frame02.png
+-rw-r--r--   0        0        0    19344 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/animation/frame03.png
+-rw-r--r--   0        0        0    19267 2024-05-08 11:51:01.514637 saenopy-1.0.4/saenopy/img/animation/frame04.png
+-rw-r--r--   0        0        0    18999 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame05.png
+-rw-r--r--   0        0        0    31030 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame06.png
+-rw-r--r--   0        0        0    32933 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame07.png
+-rw-r--r--   0        0        0    34748 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame08.png
+-rw-r--r--   0        0        0    35475 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame09.png
+-rw-r--r--   0        0        0    37528 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame10.png
+-rw-r--r--   0        0        0    39777 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame11.png
+-rw-r--r--   0        0        0    41902 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame12.png
+-rw-r--r--   0        0        0    41897 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/animation/frame13.png
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/arrowscale.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/autoscale0.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/autoscale1.ico
+-rw-r--r--   0        0        0    48947 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/buttons.svg
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/center0.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/center1.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/contrast0.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/contrast1.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/grid.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/grid2.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/grid3.ico
+-rw-r--r--   0        0        0    38885 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/logo_splash.png
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/nan0.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/nan1.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/show_image.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/show_image2.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/show_image3.ico
+-rw-r--r--   0        0        0     3606 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/slice0.ico
+-rw-r--r--   0        0        0     3606 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/slice1.ico
+-rw-r--r--   0        0        0     3606 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/slice2.ico
+-rw-r--r--   0        0        0     1150 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/slice_all.ico
+-rw-r--r--   0        0        0   121664 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/thumbnails/BFTFM.png
+-rw-r--r--   0        0        0   132449 2024-05-08 11:51:01.518637 saenopy-1.0.4/saenopy/img/thumbnails/BFTFM_2.png
+-rw-r--r--   0        0        0   180081 2024-05-08 11:51:01.522637 saenopy-1.0.4/saenopy/img/thumbnails/Bead_example_icon.png
+-rw-r--r--   0        0        0   712992 2024-05-08 11:51:01.522637 saenopy-1.0.4/saenopy/img/thumbnails/CellFibers.png
+-rw-r--r--   0        0        0   202759 2024-05-08 11:51:01.522637 saenopy-1.0.4/saenopy/img/thumbnails/Dynamic_icon.png
+-rw-r--r--   0        0        0   203085 2024-05-08 11:51:01.522637 saenopy-1.0.4/saenopy/img/thumbnails/MCF7-time-lapse.png
+-rw-r--r--   0        0        0   144494 2024-05-08 11:51:01.522637 saenopy-1.0.4/saenopy/img/thumbnails/SpheroidBlue.png
+-rw-r--r--   0        0        0   554429 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/img/thumbnails/StainedOrganoid_icon.png
+-rw-r--r--   0        0        0   263760 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/img/thumbnails/liver_fibroblast_icon.png
+-rw-r--r--   0        0        0   167929 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/img/thumbnails/pyTFM_WTKO.png
+-rw-r--r--   0        0        0     3606 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/img/view_single.ico
+-rw-r--r--   0        0        0     3606 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/img/view_two.ico
+-rw-r--r--   0        0        0    12316 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/macro.py
+-rw-r--r--   0        0        0    12410 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/materials.py
+-rw-r--r--   0        0        0     3701 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/mesh.py
+-rw-r--r--   0        0        0     5687 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/multigrid_helper.py
+-rw-r--r--   0        0        0     3256 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/TFM_functions.py
+-rw-r--r--   0        0        0    12273 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/TFM_tractions.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_deformation.py
+-rw-r--r--   0        0        0      513 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_forces.py
+-rw-r--r--   0        0        0     1377 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_strain_energy.py
+-rw-r--r--   0        0        0     7919 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress.py
+-rw-r--r--   0        0        0        0 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/__init__.py
+-rw-r--r--   0        0        0    23254 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/find_borders.py
+-rwxr-xr-x   0        0        0    17058 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/graph_theory_for_cell_boundaries.py
+-rw-r--r--   0        0        0    14541 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/grid_setup_solids_py.py
+-rw-r--r--   0        0        0     1492 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/mask_interpolation.py
+-rw-r--r--   0        0        0    15415 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/calculate_stress_imports/stress_functions.py
+-rw-r--r--   0        0        0     2631 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/correct_stage_drift.py
+-rw-r--r--   0        0        0    12260 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/plotting.py
+-rw-r--r--   0        0        0      343 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/suppress_warnings.py
+-rwxr-xr-x   0        0        0      694 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/pyTFM/utilities_TFM.py
+-rw-r--r--   0        0        0    27860 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/result_file.py
+-rw-r--r--   0        0        0     7958 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/saveable.py
+-rw-r--r--   0        0        0    48172 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/solver.py
+-rw-r--r--   0        0        0    11130 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/stack.py
+-rw-r--r--   0        0        0    17259 2024-05-08 11:51:01.526637 saenopy-1.0.4/saenopy/unused/macro.py
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 saenopy-1.0.4/PKG-INFO
```

### Comparing `saenopy-1.0.2/LICENSE.txt` & `saenopy-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/README.md` & `saenopy-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.3/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.3/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

### Comparing `saenopy-1.0.2/pyproject.toml` & `saenopy-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saenopy"
-version = "1.0.2"
+version = "1.0.4"
 description = "Semi-elastic fiber optimisation in python."
 authors = ["rgerum <14153051+rgerum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "saenopy"}]
 
 
@@ -15,37 +15,46 @@
 tqdm = "^4.64.1"
 qimage2ndarray = "^1.9.0"
 natsort = "^8.2.0"
 pyvista = "^0.37.0"
 pyvistaqt = "^0.9.0"
 imagecodecs = "^2022.9.26"
 openpiv = "^0.24.2"
-pyqt5 = "^5.15.7"
+pyqt5 = "=5.15.9"
+pyqt5-qt5 = "=5.15.2"
 qtawesome = "^1.2.1"
 jointforces = "^1.0.1"
 numba = "^0.56.4"
-sphinx = { version = "^6.1.3", optional = true }
-sphinx-rtd-theme = { version = "^1.2.0", optional = true }
-nbsphinx = { version = "^0.8.10", optional = true }
-sphinx-gallery = {version = "^0.11.1", optional = true }
 appdirs = "^1.4.4"
 nptyping = "^2.4.1"
 qtrangeslider = "^0.1.5"
 h5py = "^3.8.0"
 pyfields = "^1.7.0"
-
+sphinx = { version = ">=1.6,<7", optional = true }
+sphinx-rtd-theme = { version = "^1.2.2", optional = true }
+nbsphinx = { version = "^0.9.2", optional = true }
+sphinx-gallery = {version = "^0.13.0", optional = true }
+solidspy = "*"
+black = { version="^24.4.0", optional = true }
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme", "nbsphinx", "sphinx-gallery"]
 
 
 [tool.poetry.scripts]
 saenopy = "saenopy.gui.gui_master:main"
 
 
+[tool.poetry.group.docs.dependencies]
+sphinx = ">=1.6,<7"
+sphinx-rtd-theme = "^1.2.2"
+nbsphinx = "^0.9.2"
+sphinx-gallery = "^0.13.0"
+
+
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^5.9.0"
 auto-py-to-exe = "^2.33.0"
 pytest = "^7.2.2"
 coverage = "^5.0.0"
 hypothesis = "^6.74.1"
 coveralls = "^3.3.1"
```

### Comparing `saenopy-1.0.2/saenopy/build_beams.py` & `saenopy-1.0.4/saenopy/build_beams.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/conjugate_gradient.py` & `saenopy-1.0.4/saenopy/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/get_deformations.py` & `saenopy-1.0.4/saenopy/get_deformations.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/code/code_editor.py` & `saenopy-1.0.4/saenopy/gui/code/code_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/code/gui_code.py` & `saenopy-1.0.4/saenopy/gui/code/gui_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         with QtShortCuts.QVBoxLayout(self):
             with QtShortCuts.QVBoxLayout():
                 with QtShortCuts.QHBoxLayout():
                     self.button = QtShortCuts.QPushButton(None, "Open File", self.load, icon=qta.icon("fa5s.folder-open"))
                     self.tabs = QtWidgets.QTabBar().addToLayout()
                     self.tabs.setTabsClosable(True)
                     self.tabs.setMaximumHeight(32)
-                    QtShortCuts.current_layout.addStretch()
-                    QtShortCuts.current_layout.setSpacing(11)
+                    QtShortCuts.currentLayout().addStretch()
+                    QtShortCuts.currentLayout().setSpacing(11)
                 QtShortCuts.QHLine().addToLayout()
-                QtShortCuts.current_layout.setSpacing(0)
+                QtShortCuts.currentLayout().setSpacing(0)
 
             with QtShortCuts.QHBoxLayout():
                 self.input_filename = QtShortCuts.QInputString()
                 self.input_filename.setDisabled(True)
                 self.button_stop = QtShortCuts.QPushButton(None, "stop", self.stop, icon=qta.icon("fa5s.stop"))
                 self.button_run = QtShortCuts.QPushButton(None, "run", self.run, icon=qta.icon("fa5s.play"))
             with QtShortCuts.QHBoxLayout():
@@ -90,14 +90,18 @@
         self.editor.textChanged.connect(self.editor_text_changed)
         self.tabs.currentChanged.connect(self.select_tab)
         self.tabs.tabCloseRequested.connect(self.remove_tab)
         self.process_finished.connect(self.script_status_changed)
 
         self.select_tab(-1)
 
+        for arg in sys.argv[1:]:
+            if arg.endswith(".py"):
+                self.do_load(arg)
+
     def update_console(self, open_script):
         if len(self.open_scripts) and open_script == self.open_scripts[self.open_scripts_index]:
             self.console.setText(open_script.console)
 
     def load(self):
         new_path = QtWidgets.QFileDialog.getOpenFileName(None, "Open Script", os.getcwd(), "Python File (*.py)")
         if new_path:
@@ -183,13 +187,9 @@
         ctypes.windll.shell32.SetCurrentProcessExplicitAppUserModelID(myappid)
     print(sys.argv)
     window = MainWindowCode()
     window.setMinimumWidth(1600)
     window.setMinimumHeight(900)
     window.setWindowTitle("Saenopy Viewer")
     window.setWindowIcon(resource_icon("Icon.ico"))
-    for arg in sys.argv[1:]:
-        if arg.endswith(".py"):
-            pass
-            window.do_load(arg)
     window.show()
     sys.exit(app.exec_())
```

### Comparing `saenopy-1.0.2/saenopy/gui/code/script_file.py` & `saenopy-1.0.4/saenopy/gui/code/script_file.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/code/syntax.py` & `saenopy-1.0.4/saenopy/gui/code/syntax.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/QExtendedGraphicsView.py` & `saenopy-1.0.4/saenopy/gui/common/QExtendedGraphicsView.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/QtShortCuts.py` & `saenopy-1.0.4/saenopy/gui/common/QtShortCuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 import colorsys
 import os
 
 import matplotlib as mpl
 import numpy as np
 from qtpy import QtCore, QtGui, QtWidgets
 
-current_layout = None
 
 def setCurrentLayout(layout):
-    global current_layout
-    current_layout = layout
+    app = QtWidgets.QApplication.instance()
+    app.current_layout = layout
 
 def currentLayout():
-    return current_layout
+    app = QtWidgets.QApplication.instance()
+    return getattr(app, 'current_layout', None)
 
 def addToLayout(self, layout=None):
-    if layout is None and current_layout is not None:
-        layout = current_layout
+    if layout is None and currentLayout() is not None:
+        layout = currentLayout()
     layout.addWidget(self)
     return self
 
 QtWidgets.QWidget.addToLayout = addToLayout
 def connect(self, target):
     super().connect(target)
     return self
@@ -67,16 +67,16 @@
         # initialize the super widget
         super(QInput, self).__init__()
 
         # initialize the layout of this widget
         QtWidgets.QHBoxLayout(self)
         self.layout().setContentsMargins(0, 0, 0, 0)
 
-        if layout is None and current_layout is not None:
-            layout = current_layout
+        if layout is None and currentLayout() is not None:
+            layout = currentLayout()
 
         # add me to a parent layout
         if layout is not None:
             if stretch is True:
                 self.wrapper_layout = QtWidgets.QHBoxLayout()
                 self.wrapper_layout.setContentsMargins(0, 0, 0, 0)
                 self.wrapper_layout.addWidget(self)
@@ -695,44 +695,44 @@
     def value(self):
         # return the color
         return self.line.text()
 
 class QPushButton(QtWidgets.QPushButton):
     def __init__(self, layout, name, connect=None, icon=None, tooltip=None):
         super().__init__(name)
-        if layout is None and current_layout is not None:
-            layout = current_layout
+        if layout is None and currentLayout() is not None:
+            layout = currentLayout()
         layout.addWidget(self)
         if connect is not None:
             self.clicked.connect(connect)
         if icon is not None:
             self.setIcon(icon)
         if tooltip is not None:
             self.setToolTip(tooltip)
 
 class QGroupBox(QtWidgets.QGroupBox):
     def __init__(self, layout, name):
         super().__init__(name)
-        if layout is None and current_layout is not None:
-            layout = current_layout
+        if layout is None and currentLayout() is not None:
+            layout = currentLayout()
         layout.addWidget(self)
         self.layout = QVBoxLayout(self)
 
     def __enter__(self):
         return self, self.layout.__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.layout.__exit__(exc_type, exc_val, exc_tb)
 
 class QTabWidget(QtWidgets.QTabWidget):
 
     def __init__(self, layout, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        if layout is None and current_layout is not None:
-            layout = current_layout
+        if layout is None and currentLayout() is not None:
+            layout = currentLayout()
         layout.addWidget(self)
 
     def createTab(self, name):
         tab_stack = QtWidgets.QWidget()
         self.addTab(tab_stack, name)
         v_layout = QVBoxLayout(tab_stack)
         return v_layout
@@ -740,44 +740,71 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
 
+class QTabBarWidget(QtWidgets.QTabBar):
+
+    def __init__(self, layout, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if layout is None and currentLayout() is not None:
+            layout = currentLayout()
+        layout.addWidget(self)
+        self.widgets = []
+
+
+    def createTab(self, name):
+        tab_stack = QtWidgets.QWidget()
+        self.widgets.append(tab_stack)
+        self.addTab(name)
+        v_layout = QVBoxLayout(tab_stack)
+        return v_layout
+
+    def currentWidget(self):
+        return self.widgets[self.currentIndex()]
+
+    def widget(self, i):
+        return self.widgets[i]
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
 class EnterableLayout:
     def __enter__(self):
-        global current_layout
-        self.old_layout = current_layout
-        current_layout = self.layout
+        self.old_layout = currentLayout()
+        setCurrentLayout(self.layout)
         return self.layout
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        global current_layout
-        current_layout = self.old_layout
+        setCurrentLayout(self.old_layout)
 
 
 class QVBoxLayout(QtWidgets.QVBoxLayout, EnterableLayout):
     def __init__(self, parent=None, no_margins=False):
-        if parent is None and current_layout is not None:
-            parent = current_layout
+        if parent is None and currentLayout() is not None:
+            parent = currentLayout()
         if getattr(parent, "addLayout", None) is None:
             super().__init__(parent)
         else:
             super().__init__()
             parent.addLayout(self)
         self.layout = self
         if no_margins is True:
             self.setContentsMargins(0, 0, 0, 0)
 
 
 class QHBoxLayout(QtWidgets.QHBoxLayout, EnterableLayout):
     def __init__(self, parent=None, no_margins=False):
-        if parent is None and current_layout is not None:
-            parent = current_layout
+        if parent is None and currentLayout() is not None:
+            parent = currentLayout()
         if getattr(parent, "addLayout", None) is None:#isinstance(parent, QtWidgets.QWidget):
             super().__init__(parent)
         else:
             super().__init__()
             parent.addLayout(self)
         self.layout = self
         if no_margins is True:
@@ -785,38 +812,38 @@
 
 
 def QVLine(layout=None):
     line = QtWidgets.QFrame()
     line.setFrameShape(QtWidgets.QFrame.VLine)
     line.setFrameShadow(QtWidgets.QFrame.Sunken)
 
-    if current_layout is not None:
-        current_layout.addWidget(line)
+    if currentLayout() is not None:
+        currentLayout().addWidget(line)
     else:
         layout.addWidget(line)
     return line
 
 
 def QHLine(layout=None):
     line = QtWidgets.QFrame()
     line.setFrameShape(QtWidgets.QFrame.HLine)
     line.setFrameShadow(QtWidgets.QFrame.Sunken)
 
-    if current_layout is not None:
-        current_layout.addWidget(line)
+    if currentLayout() is not None:
+        currentLayout().addWidget(line)
     else:
         layout.addWidget(line)
     return line
 
 
 class QSplitter(QtWidgets.QSplitter, EnterableLayout):
     def __init__(self, *args):
         super().__init__(*args)
-        if current_layout is not None:
-            current_layout.addWidget(self)
+        if currentLayout() is not None:
+            currentLayout().addWidget(self)
         self.layout = self
         self.widgets = []
 
     def addLayout(self, layout):
         widget = QtWidgets.QWidget()
         self.widgets.append(widget)
         self.addWidget(widget)
```

### Comparing `saenopy-1.0.2/saenopy/gui/common/gui_classes.py` & `saenopy-1.0.4/saenopy/gui/common/gui_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                 self.label.clicked.connect(self.toggle)
 
                 headerLine = QtWidgets.QFrame().addToLayout()
                 headerLine.setFrameShape(QtWidgets.QFrame.HLine)
                 headerLine.setFrameShadow(QtWidgets.QFrame.Sunken)
                 headerLine.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Maximum)
 
-                #QtShortCuts.current_layout.addStretch()
+                #QtShortCuts.currentLayout().addStretch()
                 if url is not None:
                     self.label2 = QtWidgets.QPushButton(qta.icon("fa5s.question"), "").addToLayout()
                     self.label2.setToolTip("open the documentation in the browser")
                     #self.label2.setMaximumWidth(30)
                     self.label2.setStyleSheet("QPushButton { border: none; background: none; }")
                     self.label2.clicked.connect(lambda x: QtGui.QDesktopServices.openUrl(QtCore.QUrl(url)))
             self.child_widget = QtWidgets.QWidget().addToLayout()
@@ -284,40 +284,51 @@
 
 class ListWidget(QtWidgets.QListWidget):
     itemSelectionChanged2 = QtCore.Signal()
     itemChanged2 = QtCore.Signal()
     addItemClicked = QtCore.Signal()
     signal_act_copy_clicked = QtCore.Signal()
     signal_act_paste_clicked = QtCore.Signal()
+    signal_act_paste2_clicked = QtCore.Signal()
     signal_act_paths_clicked = QtCore.Signal()
+    signal_act_paths2_clicked = QtCore.Signal()
+    signal_act_paths3_clicked = QtCore.Signal()
 
     data = []
-    def __init__(self, layout, editable=False, add_item_button=False, color_picker=False, copy_params=False, allow_paste_callback=None):
+    def __init__(self, layout, editable=False, add_item_button=False, color_picker=False, copy_params=False,
+                 allow_paste_callback=None, copy_to_callback=None):
         super().__init__()
         layout.addWidget(self)
         self.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.list2_context_menu)
         self.itemChanged.connect(self.list2_checked_changed)
         self.itemChanged = self.itemChanged2
-        self.act_delete = QtWidgets.QAction(qta.icon("fa5.trash-alt"), "Remove", self)
+        self.act_delete = QtWidgets.QAction(qta.icon("fa5s.minus"), "Remove", self)
         self.act_delete.triggered.connect(self.delete_item)
 
         self.act_color = None
         if color_picker is True:
             self.act_color = QtWidgets.QAction(qta.icon("fa5s.paint-brush"), "Change Color", self)
             self.act_color.triggered.connect(self.change_color)
         self.act_copy = None
         if copy_params is True:
             self.act_copy = QtWidgets.QAction(qta.icon("fa5.copy"), "Copy Parameters", self)
             self.act_copy.triggered.connect(self.signal_act_copy_clicked)
             self.act_paste = QtWidgets.QAction(qta.icon("fa5s.paste"), "Paste Parameters", self)
             self.act_paste.triggered.connect(self.signal_act_paste_clicked)
+            self.act_paste2 = QtWidgets.QAction(qta.icon("fa5s.paste"), "Paste Parameters to All", self)
+            self.act_paste2.triggered.connect(self.signal_act_paste2_clicked)
             self.allow_paste_callback = allow_paste_callback
+            self.copy_to_callback = copy_to_callback
             self.act_path = QtWidgets.QAction(qta.icon("mdi.folder-multiple-image"), "Adjust Paths", self)
             self.act_path.triggered.connect(self.signal_act_paths_clicked)
+            self.act_path2 = QtWidgets.QAction(qta.icon("mdi.folder"), "Open in Explorer", self)
+            self.act_path2.triggered.connect(self.signal_act_paths2_clicked)
+            self.act_path3 = QtWidgets.QAction(qta.icon("fa5.copy"), "Copy Path", self)
+            self.act_path3.triggered.connect(self.signal_act_paths3_clicked)
 
         self.setDragDropMode(QtWidgets.QAbstractItemView.InternalMove)
 
         self.flags = QtCore.Qt.ItemIsSelectable | QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsUserCheckable
         if editable:
             self.flags |= QtCore.Qt.ItemIsEditable | QtCore.Qt.ItemIsDragEnabled
 
@@ -368,16 +379,27 @@
             menu = QtWidgets.QMenu()
 
             if self.act_color is not None:
                 menu.addAction(self.act_color)
             if self.act_copy is not None:
                 menu.addAction(self.act_copy)
                 self.act_paste.setDisabled(not self.allow_paste_callback())
+                self.act_paste2.setDisabled(not self.allow_paste_callback())
                 menu.addAction(self.act_paste)
+                menu.addAction(self.act_paste2)
+                menu.addSeparator()
+                menu.addAction(self.act_path3)
+                menu.addAction(self.act_path2)
                 menu.addAction(self.act_path)
+                menu.addSeparator()
+                if self.copy_to_callback:
+                    m = self.copy_to_callback()
+                    if m:
+                        menu.addMenu(m)
+                        menu.addSeparator()
 
             menu.addAction(self.act_delete)
 
             # open menu at mouse click position
             if menu:
                 menu.exec_(self.viewport().mapToGlobal(position))
```

### Comparing `saenopy-1.0.2/saenopy/gui/common/lif_reader.py` & `saenopy-1.0.4/saenopy/gui/common/lif_reader.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/patch_lifreader.py` & `saenopy-1.0.4/saenopy/gui/common/patch_lifreader.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/sigmoid_widget.py` & `saenopy-1.0.4/saenopy/gui/common/sigmoid_widget.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/stack_preview.py` & `saenopy-1.0.4/saenopy/gui/common/stack_preview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import qtawesome as qta
 from qtpy import QtCore, QtWidgets, QtGui
 import numpy as np
 
 from qimage2ndarray import array2qimage
 from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
-from saenopy.gui.solver.modules.QTimeSlider import QTimeSlider
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from saenopy.gui.solver.modules.StackDisplay import ModuleScaleBar
 
 
 def crop(im, z, t, cropped):
     if "x" not in cropped:
         cropped["x"] = (None, None)
     minx = cropped["x"][0] or 0
```

### Comparing `saenopy-1.0.2/saenopy/gui/common/stack_selector.py` & `saenopy-1.0.4/saenopy/gui/common/stack_selector.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/stack_selector_crop.py` & `saenopy-1.0.4/saenopy/gui/common/stack_selector_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 self.input_cropy.valueChanged.connect(self.z_moved)
                 self.input_cropz.valueChanged.connect(self.z_moved)
                 self.input_cropx.setDisabled(True)
                 self.input_cropy.setDisabled(True)
                 self.input_cropz.setDisabled(True)
                 self.input_voxel_size.setDisabled(True)
 
-                QtShortCuts.current_layout.addStretch()
+                QtShortCuts.currentLayout().addStretch()
 
             with QtShortCuts.QVBoxLayout():
                 with QtShortCuts.QHBoxLayout():
                     self.input_time_dt = QtShortCuts.QInputString(None, "Time Delta", "0",
                                                                      validator=self.validator_time, type=float)
                     self.input_time_dt.setEnabled(False)
                     self.input_time_dt.emitValueChanged()
@@ -104,15 +104,15 @@
                     self.input_time_dt.line_edit.setCompleter(self.completer2)
 
                 self.input_cropt = QtShortCuts.QRangeSlider(None, "crop t", 0, 200)
                 self.input_cropt.setRange(0, 1)
                 self.input_cropt.setValue((0, 1))
                 self.input_cropt.valueChanged.connect(self.z_moved)
                 self.input_t_label = QtWidgets.QLabel().addToLayout()
-                QtShortCuts.current_layout.addStretch()
+                QtShortCuts.currentLayout().addStretch()
 
                 self.input_cropt.setDisabled(True)
                 self.input_tbar_unit.setDisabled(True)
                 self.input_time_dt.setDisabled(True)
 
         self.parent_selector.stack_changed.connect(self.update_ranges)
         self.parent2 = parent2
```

### Comparing `saenopy-1.0.2/saenopy/gui/common/stack_selector_leica.py` & `saenopy-1.0.4/saenopy/gui/common/stack_selector_leica.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/common/stack_selector_tif.py` & `saenopy-1.0.4/saenopy/gui/common/stack_selector_tif.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/gui_master.py` & `saenopy-1.0.4/saenopy/gui/gui_master.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import json
 import sys
 import traceback
 
 from qtpy import QtCore, QtWidgets, QtGui
 import multiprocessing
 # keep import for pyinstaller
+import skimage.exposure.exposure
 import skimage.filters.ridges
 import skimage.filters.thresholding
 
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.solver.gui_solver import MainWindowSolver as SolverMain
 from saenopy.gui.spheroid.gui_deformation_spheroid import MainWindow as SpheroidMain
 from saenopy.gui.orientation.gui_orientation import MainWindow as OrientationMain
 from saenopy.gui.code.gui_code import MainWindowCode
 from saenopy.gui.material_fit.gui_fit import MainWindowFit
+from saenopy.gui.tfm2d.gui_2d import MainWindow2D
 from saenopy.gui.common.resources import resource_path, resource_icon
 
 
 class InfoBox(QtWidgets.QWidget):
     def __init__(self, name, func):
         super().__init__()
         self.setMinimumWidth(200)
@@ -24,14 +27,16 @@
         with QtShortCuts.QHBoxLayout(self) as l:
             with QtShortCuts.QGroupBox(l, name):
                 with QtShortCuts.QVBoxLayout() as l2:
                     if name == "Solver":
                         self.text = QtWidgets.QLabel("Calculate the forces from a\n3D stack or a series of 3D stacks.").addToLayout()
                     elif name == "Spheroid":
                         self.text = QtWidgets.QLabel("Calculate the forces of\nmulticellular aggregates\nfrom a timeseries of 2D images.").addToLayout()
+                    elif name == "PyTFM":
+                        self.text = QtWidgets.QLabel("Calculate the forces from\n2D images using PyTFM.").addToLayout()
                     else:
                         self.text = QtWidgets.QLabel("Measure the orientations\nof fiberes in 2D images.\n\nAs a proxy for contractility.").addToLayout()
                     self.button1 = QtShortCuts.QPushButton(None, name, func)
 
 
 class MainWindow(QtWidgets.QWidget):
 
@@ -78,39 +83,84 @@
                         layout2.addStretch()
                         InfoBox("Solver", lambda: self.setTab(2)).addToLayout()
                         layout2.addStretch()
                         InfoBox("Spheroid", lambda: self.setTab(3)).addToLayout()
                         layout2.addStretch()
                         InfoBox("Orientation", lambda: self.setTab(4)).addToLayout()
                         layout2.addStretch()
+                        InfoBox("PyTFM", lambda: self.setTab(5)).addToLayout()
+                        layout2.addStretch()
                     layout.addStretch()
                 with self.tabs.createTab("Material Fit") as self.layout_code:
-                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
                     self.fitter = MainWindowFit().addToLayout()
 
                 with self.tabs.createTab("Solver") as self.layout_solver:
-                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
 
                 with self.tabs.createTab("Spheroid") as self.layout_spheroid:
-                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
 
                 with self.tabs.createTab("Orientation") as self.layout_orientation:
-                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
+
+                with self.tabs.createTab("PyTFM") as self.layout_pytfm:
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
 
                 with self.tabs.createTab("Code") as self.layout_code:
-                    QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                    QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
                     self.coder = MainWindowCode().addToLayout()
 
         #self.tabs.setCurrentIndex(self.settings.value("master_tab", 0))
         self.first_tab_change = False
 
+        for file in sys.argv[1:]:
+            print(file)
+            if file.endswith(".json"):
+                try:
+                    with open(file, "r") as fp:
+                        data = json.load(fp)
+                    filename = data[0]["paths"][0]["path"]
+                    if filename.endswith(".saenopy"):
+                        self.setTab(2)
+                        self.solver.tabs.setCurrentIndex(1)
+                        self.solver.plotting_window.load(file)
+                    elif filename.endswith("saenopy2D"):
+                        self.setTab(5)
+                        self.pytfm2d.tabs.setCurrentIndex(1)
+                        self.pytfm2d.plotting_window.load(file)
+                    elif filename.endswith(".saenopySpheroid"):
+                        self.setTab(3)
+                        self.spheroid.tabs.setCurrentIndex(1)
+                        self.spheroid.plotting_window.load(file)
+                    elif filename.endswith(".saenopyOrientation"):
+                        self.setTab(4)
+                        self.orientation.tabs.setCurrentIndex(1)
+                        self.orientation.plotting_window.load(file)
+                    continue
+                except (IndexError, KeyError):
+                    continue
+            if file.endswith(".py"):
+                self.setTab(6)
+            elif file.endswith(".saenopy"):
+                self.setTab(2)
+            elif file.endswith(".saenopy2D"):
+                self.setTab(5)
+            elif file.endswith(".saenopySpheroid"):
+                self.setTab(3)
+            elif file.endswith(".saenopyOrientation"):
+                self.setTab(4)
+            else:
+                raise ValueError("Unknown file type")
+
     first_tab_change = True
     solver = None
     spheroid = None
     orientation = None
+    pytfm2d = None
     def changedTab(self, value):
         if self.first_tab_change is False:
             self.settings.setValue("master_tab", value)
 
         if value == 2 and self.solver is None:
             self.solver = SolverMain().addToLayout(self.layout_solver)
             self.setMinimumWidth(1600)
@@ -119,14 +169,18 @@
             self.spheroid = SpheroidMain().addToLayout(self.layout_spheroid)
             self.setMinimumWidth(1600)
             self.setMinimumHeight(900)
         if value == 4 and self.orientation is None:  # pragma: no cover
             self.orientation = OrientationMain().addToLayout(self.layout_orientation)
             self.setMinimumWidth(1600)
             self.setMinimumHeight(900)
+        if value == 5 and self.pytfm2d is None:  # pragma: no cover
+            self.pytfm2d = MainWindow2D().addToLayout(self.layout_pytfm)
+            self.setMinimumWidth(1600)
+            self.setMinimumHeight(900)
 
     def setTab(self, value):
         self.tabs.setCurrentIndex(value)
 
 
 def main():  # pragma: no cover
     app = QtWidgets.QApplication(sys.argv)
@@ -147,41 +201,35 @@
         # Close the splash screen. It does not matter when the call
         # to this function is made, the splash screen remains open until
         # this function is called or the Python program is terminated.
         pyi_splash.close()
     except (ImportError, RuntimeError):
         pass
 
-    while True:
-        try:
-            res = app.exec_()
-            break
-        except Exception as err:
-            traceback.print_traceback(err)
-            QtWidgets.QMessageBox.critical(window, "Error", f"An Error occurred:\n{err}")
-            continue
+    from traceback import format_exception
+    def except_hook(type_, value, tb):
+        print(*format_exception(type_, value, tb), file=sys.stderr)
+        QtWidgets.QMessageBox.critical(window, "Error", f"An Error occurred:\n{type_.__name__}: {value}")
+        return
+
+    sys.excepthook = except_hook
+
+    res = app.exec_()
     sys.exit(res)
 
 
 if __name__ == '__main__':  # pragma: no cover
     # On Windows calling this function is necessary.
     multiprocessing.freeze_support()
 
-    if len(sys.argv) >= 2 and sys.argv[1].endswith(".py"):
-        source = open(sys.argv[1]).read()
+    if len(sys.argv) >= 3 and sys.argv[1] == "run" and sys.argv[2].endswith(".py"):
+        source = open(sys.argv[2]).read()
         code = compile(source, sys.argv[1], 'exec')
         exec(code)
         exit(0)
 
-
-    """ some magic to prevent PyQt5 from swallowing exceptions """
-    # Back up the reference to the exceptionhook
-    sys._excepthook = sys.excepthook
-    # Set the exception hook to our wrapping function
-    sys.excepthook = lambda *args: sys._excepthook(*args)
-
     for arg in sys.argv:
         if arg == "--demo":
             import os
             os.environ["DEMO"] = "true"
 
     main()
```

### Comparing `saenopy-1.0.2/saenopy/gui/material_fit/gui_fit.py` & `saenopy-1.0.4/saenopy/gui/material_fit/gui_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                 self.input_type.setDisabled(True)
                 self.input_type.valueChanged.connect(lambda x: self.set_value(x, "type"))
 
                 self.input_params = QtShortCuts.QInputString(None, "params", "").addToLayout()
                 self.input_params.setDisabled(True)
                 self.input_params.valueChanged.connect(lambda x: self.set_value(x, "params"))
 
-                self.list = ListWidget(QtShortCuts.current_layout, add_item_button="add measurements", color_picker=True)
+                self.list = ListWidget(QtShortCuts.currentLayout(), add_item_button="add measurements", color_picker=True)
                 self.list.addItemClicked.connect(self.add_measurement)
                 self.list.itemSelectionChanged.connect(self.listSelected)
 
             with QtShortCuts.QVBoxLayout():
                 self.all_params = AllParameters().addToLayout()
                 self.canvas = MatplotlibWidget(self).addToLayout()
                 self.button_run = QtShortCuts.QPushButton(None, "run", self.run).addToLayout()
```

### Comparing `saenopy-1.0.2/saenopy/gui/orientation/gui_orientation.py` & `saenopy-1.0.4/saenopy/gui/orientation/gui_orientation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import glob
 import imageio
 import threading
 import glob
 import re
 from pathlib import Path
 
+from saenopy.gui.orientation.modules.AddFilesDialog import AddFilesDialog
+from saenopy.examples import get_examples_orientation
 
 
 ################
 
 # QSettings
 settings = QtCore.QSettings("FabryLab", "CompactionAnalyzer")
 
@@ -36,21 +38,24 @@
         self.setWindowTitle("CompactionAnalyzer")
 
         main_layout = QtWidgets.QHBoxLayout(self)
 
         with QtShortCuts.QTabWidget(main_layout) as self.tabs:
 
             """ """
-            with self.tabs.createTab("Compaction") as v_layout:
+            with self.tabs.createTab("Analyse Measurements") as v_layout:
+                v_layout.setContentsMargins(0, 0, 0, 0)
                 with QtShortCuts.QHBoxLayout() as h_layout:
+                    h_layout.setContentsMargins(0, 0, 0, 0)
                     #self.deformations = Deformation(h_layout, self)
                     self.deformations = BatchEvaluate(self)
                     h_layout.addWidget(self.deformations)
                     self.description = QtWidgets.QTextEdit()
-                    self.description.setDisabled(True)
+                    self.description.setReadOnly(True)
+                    self.description.setStyleSheet("QTextEdit { background: #f0f0f0}")
                     self.description.setMaximumWidth(300)
                     h_layout.addWidget(self.description)
                     self.description.setText("""
                     <h1>Start Evaluation</h1>
                     
                     As a measure of the contractile strength for cells/organoids in fibrous materials, we quantify the tissue 
                     compaction by the re-orientation of the fiber structure towards the cell centre and 
@@ -79,22 +84,25 @@
                 with QtShortCuts.QHBoxLayout() as h_layout:
                     h_layout.addStretch()
                     self.button_previous = QtShortCuts.QPushButton(None, "back", self.previous)
                     self.button_next = QtShortCuts.QPushButton(None, "next", self.next)
 
             """ """
             with self.tabs.createTab("Data Analysis") as v_layout:
+                v_layout.setContentsMargins(0, 0, 0, 0)
                 with QtShortCuts.QHBoxLayout() as h_layout:
+                    h_layout.setContentsMargins(0, 0, 0, 0)
 
                     #self.deformations = Force(h_layout, self)
                     self.deformations = PlottingWindow(self)
                     h_layout.addWidget(self.deformations)
 
                     self.description = QtWidgets.QTextEdit()
-                    self.description.setDisabled(True)
+                    self.description.setReadOnly(True)
+                    self.description.setStyleSheet("QTextEdit { background: #f0f0f0}")
                     h_layout.addWidget(self.description)
                     self.description.setText("""
                             <h1>Data Analysis</h1>
                            
                             In this step we can analyze our results. <br/>
                             <br/>                    
                             
@@ -194,15 +202,15 @@
                             self.sigma_tensor = QtShortCuts.QInputString(None, "sigma_tensor", "7.0", type=float, settings=settings, settings_key="orientation/sigma_tensor")
                             self.sigma_tensor_type = QtShortCuts.QInputChoice(None, "", "um", ["um", "pixel"], settings=settings, settings_key="orientation/sigma_tensor_unit")
                             self.sigma_tensor_button = QtShortCuts.QPushButton(None, "detect", self.sigma_tensor_button_clicked)
                             self.sigma_tensor_button.setDisabled(True)
                         with QtShortCuts.QHBoxLayout():
                             self.edge = QtShortCuts.QInputString(None, "edge", "40", type=int, settings=settings, settings_key="orientation/edge", tooltip="How many pixels to cut at the edge of the image.")
                             QtWidgets.QLabel("px").addToLayout()
-                            self.max_dist = QtShortCuts.QInputString(None, "max_dist", "None", type=int, settings=settings, settings_key="orientation/max_dist", tooltip="Optional: specify the maximal distance around the cell center")
+                            self.max_dist = QtShortCuts.QInputString(None, "max_dist", "None", type=int, settings=settings, settings_key="orientation/max_dist", tooltip="Optional: specify the maximal distance around the cell center", none_value=None)
                             QtWidgets.QLabel("px").addToLayout()
 
                         with QtShortCuts.QHBoxLayout():
                             self.sigma_first_blur = QtShortCuts.QInputString(None, "sigma_first_blur", "0.5", type=float, settings=settings, settings_key="orientation/sigma_first_blur")
                             QtWidgets.QLabel("px").addToLayout()
                         with QtShortCuts.QHBoxLayout():
                             self.angle_sections = QtShortCuts.QInputString(None, "angle_sections", "5", type=int, settings=settings, settings_key="orientation/angle_sections")
@@ -373,89 +381,37 @@
         for widget in [self.segmention_thres, self.seg_gaus1, self.seg_gaus2]:
             widget.setDisabled(self.individual_data.value())
         if not self.individual_data.value():
             for widget in [self.segmention_thres_indi, self.seg_gaus1_indi, self.seg_gaus2_indi]:
                 widget.setValue("None")
 
     def show_files(self):
-        from CompactionAnalyzer.CompactionFunctions import generate_lists
-
-        class AddFilesDialog(QtWidgets.QDialog):
-            def __init__(self, parent):
-                super().__init__(parent)
-                self.setWindowTitle("Add Files")
-                with QtShortCuts.QVBoxLayout(self) as layout:
-                    self.label = QtWidgets.QLabel(
-                        "Select two paths as an input wildcard. Use * to specify a placeholder. One should be for the fiber images and one for the cell images.")
-                    layout.addWidget(self.label)
-
-                    self.cellText = QtShortCuts.QInputFilename(None, "Cell Images", file_type="Image (*.tif *.png *.jpg)", settings=settings,
-                                                                settings_key="batch/wildcard_cell", existing=True,
-                                                                allow_edit=True)
-                    self.fiberText = QtShortCuts.QInputFilename(None, "Fiber Images", file_type="Image (*.tif *.png *.jpg)", settings=settings,
-                                                                settings_key="batch/wildcard_fiber", existing=True,
-                                                                allow_edit=True)
-                    self.outputText = QtShortCuts.QInputFolder(None, "output", settings=settings,
-                                                               settings_key="batch/output_folder", allow_edit=True)
-
-                    def changed():
-                        fiber_list_string = os.path.normpath(self.fiberText.value())
-                        cell_list_string = os.path.normpath(self.cellText.value())
-                        output_folder = os.path.normpath(self.outputText.value())
-                        fiber_list, cell_list, out_list = generate_lists(fiber_list_string, cell_list_string,
-                                                                         output_main=output_folder)
-                        if self.fiberText.value() == "" or self.cellText.value() == "":
-                            self.label2.setText("")
-                            self.label2.setStyleSheet("QLabel { color : red; }")
-                            self.button_addList1.setDisabled(True)
-                        elif len(fiber_list) != len(cell_list):
-                            self.label2.setText(f"Warning: {len(fiber_list)} fiber images found and {len(cell_list)} cell images found. Numbers do not match.")
-                            self.label2.setStyleSheet("QLabel { color : red; }")
-                            self.button_addList1.setDisabled(True)
-                        else:
-                            if "*" not in fiber_list_string:
-                                if len(fiber_list) == 0:
-                                    self.label2.setText(f"'Fiber Images' not found")
-                                    self.label2.setStyleSheet("QLabel { color : red; }")
-                                    self.button_addList1.setDisabled(True)
-                                elif len(cell_list) == 0:
-                                    self.label2.setText(f"'Cell Images' not found")
-                                    self.label2.setStyleSheet("QLabel { color : red; }")
-                                    self.button_addList1.setDisabled(True)
-                                else:
-                                    self.label2.setText(f"No * found in 'Fiber Images', will only import a single image.")
-                                    self.label2.setStyleSheet("QLabel { color : orange; }")
-                                    self.button_addList1.setDisabled(False)
-                            else:
-                                self.label2.setText(
-                                    f"{len(fiber_list)} fiber images found and {len(cell_list)} cell images found.")
-                                self.label2.setStyleSheet("QLabel { color : green; }")
-                                self.button_addList1.setDisabled(False)
-                    self.fiberText.line.textChanged.connect(changed)
-                    self.cellText.line.textChanged.connect(changed)
-                    self.label2 = QtWidgets.QLabel()#.addToLayout()
-                    layout.addWidget(self.label2)
 
-                    with QtShortCuts.QHBoxLayout() as layout3:
-                        # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
-                        layout3.addStretch()
-                        self.button_addList2 = QtShortCuts.QPushButton(None, "cancel", self.reject)
-                        self.button_addList1 = QtShortCuts.QPushButton(None, "ok", self.accept)
-                    changed()
 
-        dialog = AddFilesDialog(self)
+        dialog = AddFilesDialog(self, settings)
         if not dialog.exec():
             return
 
         import glob
         import re
-        fiber_list_string = os.path.normpath(dialog.fiberText.value())
-        cell_list_string = os.path.normpath(dialog.cellText.value())
-        output_folder = os.path.normpath(dialog.outputText.value())
+        if dialog.mode == "new":
+            fiber_list_string = os.path.normpath(dialog.fiberText.value())
+            cell_list_string = os.path.normpath(dialog.cellText.value())
+            output_folder = os.path.normpath(dialog.outputText.value())
+        elif dialog.mode == "example":
+            # get the date from the example referenced by name
+            example = get_examples_orientation()[dialog.mode_data]
+            fiber_list_string = str(example["input_fiber"])
+            cell_list_string = str(example["input_cell"])
+            output_folder = str(example["output_path"])
+            print(fiber_list_string)
+            print(cell_list_string)
+            print(output_folder)
 
+        from CompactionAnalyzer.CompactionFunctions import generate_lists
         fiber_list, cell_list, out_list = generate_lists(fiber_list_string, cell_list_string, output_main=output_folder)
 
         import matplotlib as mpl
         for fiber, cell, out in zip(fiber_list, cell_list, out_list):
             self.list.addData(fiber, True, [fiber, cell, out, {"segmention_thres": None, "seg_gaus1": None, "seg_gaus2": None}], mpl.colors.to_hex(f"gray"))
 
     def clear_files(self):
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/analyze/plot_window.py` & `saenopy-1.0.4/saenopy/gui/common/plot_window.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_qt import NavigationToolbar2QT as NavigationToolbar
 from qtpy import QtWidgets, QtCore, QtGui
+import qtawesome as qta
 
-from saenopy import Result
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import ListWidget, MatplotlibWidget, execute
 
 
 class AddFilesDialog(QtWidgets.QDialog):
-    def __init__(self, parent, settings):
+
+    def __init__(self, parent, settings, file_extension):
         super().__init__(parent)
         self.setWindowTitle("Add Files")
         with QtShortCuts.QVBoxLayout(self) as layout:
             self.label = QtWidgets.QLabel(
                 "Select a path as an input wildcard. Use * to specify a placeholder. All paths that match the wildcard will be added.")
             layout.addWidget(self.label)
 
             def checker(filename):
-                return filename + "/**/*.saenopy"
+                return filename + "/**/*"+file_extension
 
             self.inputText = QtShortCuts.QInputFolder(None, None, settings=settings, filename_checker=checker,
                                                       settings_key="batch_eval/analyse_force_wildcard", allow_edit=True)
             with QtShortCuts.QHBoxLayout() as layout3:
                 # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
                 layout3.addStretch()
                 self.button_addList = QtShortCuts.QPushButton(None, "cancel", self.reject)
@@ -54,32 +55,71 @@
 
 
 class PlottingWindow(QtWidgets.QWidget):
     progress_signal = QtCore.Signal(int, int, int, int)
     finished_signal = QtCore.Signal()
     thread = None
 
-    def __init__(self, parent=None):
+    settings_key = "Seanopy_deformation"
+    file_extension = ".saenopy"
+
+    def add_parameters(self):
+        pass
+
+    def load_file(self, file):
+        pass
+
+    def get_label(self):
+        return "", ""
+
+    def get_copy_to_menu(self, filename):
+        menu2 = QtWidgets.QMenu("Copy to Analysis")
+        menu2.setIcon(qta.icon("mdi.clipboard-arrow-right-outline"))
+        self.copy_to_actions = []
+        for index, folder in enumerate(self.data_folders):
+            name, checked, files, color = folder
+            act = QtWidgets.QAction(qta.icon("fa5s.circle", options=[dict(color=color)]), name, self)
+            def clicked(*, index=index):
+                self.list.setCurrentRow(index)
+                try:
+                    self.add_files([filename])
+                except Exception as e:
+                    QtWidgets.QMessageBox.critical(self, "Error", f"Measurement could not be added to Analysis.\n"
+                                                                  f"Is it evaluated completely?")
+                    return
+                self.list2.setCurrentRow(self.list2.count()-2)
+            act.triggered.connect(clicked)
+            menu2.addAction(act)
+            self.copy_to_actions.append(act)
+        menu2.addSeparator()
+        return menu2
+
+    def __init__(self, parent=None, batch_evluate_instance=None):
         super().__init__(parent)
 
+        self.batch_evluate_instance = batch_evluate_instance
+        if batch_evluate_instance is not None:
+            self.batch_evluate_instance.set_plot_window(self)
+
         # QSettings
-        self.settings = QtCore.QSettings("Saenopy", "Saenopy")
+        self.settings = QtCore.QSettings("Saenopy", self.settings_key)
 
         self.setMinimumWidth(800)
         self.setMinimumHeight(400)
         self.setWindowTitle("Saenopy Evaluation")
 
         self.images = []
         self.data_folders = []
         self.current_plot_func = lambda: None
 
         with QtShortCuts.QVBoxLayout(self) as main_layout0:
+         main_layout0.setContentsMargins(0, 0, 0, 0)
          with QtShortCuts.QHBoxLayout() as main_layout00:
-             self.button_save = QtShortCuts.QPushButton(None, "save", self.save)
-             self.button_load = QtShortCuts.QPushButton(None, "load", self.load)
+             self.button_save = QtShortCuts.QPushButton(None, "save", lambda x: self.save())
+             self.button_load = QtShortCuts.QPushButton(None, "load", lambda x: self.load())
              main_layout00.addStretch()
          with QtShortCuts.QHBoxLayout() as main_layout:
             with QtShortCuts.QVBoxLayout() as layout:
                 with QtShortCuts.QGroupBox(None, "Groups") as (_, layout2):
                     layout2.setContentsMargins(0, 3, 0, 1)
                     self.list = ListWidget(layout2, True, add_item_button="add group", color_picker=True)
                     self.list.setStyleSheet("QListWidget{border: none}")
@@ -95,19 +135,15 @@
                     self.list2.itemSelectionChanged.connect(self.run2)
                     self.list2.itemChanged.connect(self.replot)
                     self.list2.addItemClicked.connect(self.addFiles)
 
                     self.setAcceptDrops(True)
 
             with QtShortCuts.QGroupBox(main_layout, "Plot Forces") as (_, layout):
-                self.type = QtShortCuts.QInputChoice(None, "type", "strain_energy", ["strain_energy", "contractility", "polarity", "99_percentile_deformation", "99_percentile_force"])
-                self.type.valueChanged.connect(self.replot)
-                self.agg = QtShortCuts.QInputChoice(None, "aggregate", "mean",
-                                                     ["mean", "max", "min", "median"])
-                self.agg.valueChanged.connect(self.replot)
+                self.add_parameters()
 
                 self.canvas = MatplotlibWidget(self)
                 layout.addWidget(self.canvas)
                 layout.addWidget(NavigationToolbar(self.canvas, self))
 
                 with QtShortCuts.QHBoxLayout() as layout2:
                     self.button_export = QtShortCuts.QPushButton(layout2, "Export", self.export)
@@ -119,32 +155,34 @@
                     for button in self.plot_buttons:
                         button.setCheckable(True)
 
         self.list.setData(self.data_folders)
         self.addGroup()
         self.current_plot_func = self.run2
 
-    def save(self):
-        new_path = QtWidgets.QFileDialog.getSaveFileName(None, "Save Session", os.getcwd(), "JSON File (*.json)")
-        if new_path:
-            if not new_path.endswith(".json"):
-                new_path += ".json"
+    def save(self, filename=None):
+        if filename is None:
+            filename = QtWidgets.QFileDialog.getSaveFileName(None, "Save Session", os.getcwd(), "JSON File (*.json)")
+        if filename:
+            if not filename.endswith(".json"):
+                filename += ".json"
             list_new = []
             for item in self.list.data:
                 list_new.append({"name": item[0], "selected": item[1], "color": item[3], "paths": []})
                 for item2 in item[2]:
                     list_new[-1]["paths"].append({"path": item2[0], "selected": item[1]})
 
-            with open(new_path, "w") as fp:
+            with open(filename, "w") as fp:
                 json.dump(list_new, fp, indent=2)
 
-    def load(self):
-        new_path = QtWidgets.QFileDialog.getOpenFileName(None, "Load Session", os.getcwd(), "JSON File (*.json)")
-        if new_path:
-            with open(new_path, "r") as fp:
+    def load(self, filename=None):
+        if filename is None:
+            filename = QtWidgets.QFileDialog.getOpenFileName(None, "Load Session", os.getcwd(), "JSON File (*.json)")
+        if filename:
+            with open(filename, "r") as fp:
                 list_new = json.load(fp)
             self.list.clear()
             self.list.setData([[i["name"], i["selected"], [], i["color"]] for i in list_new])
             self.data_folders = self.list.data
 
             for i, d in enumerate(list_new):
                 self.list.setCurrentRow(i)
@@ -169,62 +207,53 @@
 
     def dropEvent(self, event: QtCore.QEvent):
         urls = []
         for url in event.mimeData().urls():
             url = url.toLocalFile()
             if url[0] == "/" and url[2] == ":":
                 url = url[1:]
-            if url.endswith(".saenopy"):
+            if url.endswith(self.file_extension):
                 urls += [url]
             else:
-                urls += glob.glob(url + "/**/*.saenopy", recursive=True)
+                urls += glob.glob(url + "/**/*"+self.file_extension, recursive=True)
         self.add_files(urls)
 
     def add_files(self, urls):
         current_group = self.list2.data
         current_files = [d[0] for d in current_group]
         for file in urls:
             if file in current_files:
                 print("File already in list", file)
                 continue
             try:
                 print("Add file", file)
-                res: Result = Result.load(file)
-                res.resulting_data = []
-                if len(res.solvers) == 0 or res.solvers[0] is None or res.solvers[0].regularisation_results is None:
+                res = self.load_file(file)
+                if res is None:
                     continue
-                for i, M in enumerate(res.solvers):
-                    res.resulting_data.append({
-                        "t": i*res.time_delta if res.time_delta else 0,
-                        "strain_energy": M.mesh.strain_energy,
-                        "contractility": M.get_contractility(center_mode="force"),
-                        "polarity": M.get_polarity(),
-                        "99_percentile_deformation": np.nanpercentile(np.linalg.norm(M.mesh.displacements_target[M.mesh.regularisation_mask], axis=1), 99),
-                        "99_percentile_force": np.nanpercentile(np.linalg.norm(M.mesh.forces[M.mesh.regularisation_mask], axis=1), 99),
-                        "filename": file,
-                    })
-                res.resulting_data = pd.DataFrame(res.resulting_data)
                 if self.list2.data is current_group:
                     self.list2.addData(file, True, res)
-                    self.replot()
+                    #self.replot()
                 #app.processEvents()
             except FileNotFoundError:
                 continue
         self.check_results_with_time()
 
     def check_results_with_time(self):
         time_values = False
         for name, checked, files, color in self.data_folders:
             if checked != 0:
                 for name2, checked2, res, color in files:
-                    if len(res.solvers) > 1:
+                    data = res.get_data_structure()
+                    if data["time_delta"] is not None:
                         time_values = True
+        print("time_values", time_values)
         if time_values is False:
             self.barplot()
-        self.agg.setEnabled(time_values)
+        if getattr(self, "agg", None) is not None:
+            self.agg.setEnabled(time_values)
         self.button_run.setEnabled(time_values)
         self.button_run2.setEnabled(time_values)
 
 
     def update_group_name(self):
         if self.list.currentItem() is not None:
             self.box_group.setTitle(f"Files for '{self.list.currentItem().text()}'")
@@ -235,15 +264,15 @@
     def addGroup(self):
         text = f"Group{1+len(self.data_folders)}"
         item = self.list.addData(text, True, [], mpl.colors.to_hex(f"C{len(self.data_folders)}"))
         self.list.setCurrentItem(item)
         self.list.editItem(item)
 
     def addFiles(self):
-        dialog = AddFilesDialog(self, self.settings)
+        dialog = AddFilesDialog(self, self.settings, self.file_extension)
         if not dialog.exec():
             return
 
         text = os.path.normpath(dialog.inputText.value())
         files = glob.glob(text, recursive=True)
 
         self.add_files(files)
@@ -255,16 +284,18 @@
             return
         self.update_group_name()
         self.list2.setData(data[2])
 
     def getAllCurrentPandasData(self):
         results = []
         for name, checked, files, color in self.data_folders:
+            print(name, checked, files)
             if checked != 0:
                 for name2, checked2, res, color in files:
+                    print("name2", name2, checked2)
                     if checked2 != 0:
                         res.resulting_data["group"] = name
                         results.append(res.resulting_data)
         res = pd.concat(results)
         #res["t"] = res["index"] * self.dt.value() / 60
         res.to_csv("tmp_pandas.csv")
         return res
@@ -276,40 +307,29 @@
     def barplot(self):
         for button in self.plot_buttons:
             button.setChecked(False)
         self.button_run3.setChecked(True)
         self.current_plot_func = self.barplot
         self.canvas.setActive()
         plt.cla()
-        if self.type.value() == "strain_energy":
-            mu_name = 'strain_energy'
-            y_label = 'Strain Energy'
-        elif self.type.value() == "contractility":
-            mu_name = 'contractility'
-            y_label = 'Contractility'
-        elif self.type.value() == "polarity":
-            mu_name = 'polarity'
-            y_label = 'Polarity'
-        elif self.type.value() == "99_percentile_deformation":
-            mu_name = '99_percentile_deformation'
-            y_label = 'Deformation'
-        elif self.type.value() == "99_percentile_force":
-            mu_name = '99_percentile_force'
-            y_label = 'Force'
+        mu_name, y_label = self.get_label()
 
         # get all the data as a pandas dataframe
         res = self.getAllCurrentPandasData()
 
-        # limit the dataframe to the comparison time
-        res0 = res.groupby("filename").agg("max")
-        del res["group"]
-        res = res.groupby("filename").agg(self.agg.value())
-        res["group"] = res0["group"]
-        #index = self.get_comparison_index()
-        #res = res[res.index == index]
+        if getattr(self, "agg", None) is not None:
+            # limit the dataframe to the comparison time
+            res0 = res.groupby("filename").agg("max")
+            del res["group"]
+            res = res.groupby("filename").agg(self.agg.value())
+            res["group"] = res0["group"]
+        else:
+            # limit the dataframe to the comparison time
+            index = self.get_comparison_index()
+            res = res[res.index == index]
 
         code_data = [res, ["group", mu_name]]
 
         color_dict = {d[0]: d[3] for d in self.data_folders}
 
         def plot(res, mu_name, y_label, color_dict2):
             # define the colors
@@ -339,36 +359,27 @@
         self.export_data = [code, code_data]
 
     def plot_groups(self):
         for button in self.plot_buttons:
             button.setChecked(False)
         self.button_run2.setChecked(True)
         self.current_plot_func = self.plot_groups
-        if self.type.value() == "strain_energy":
-            mu_name = 'strain_energy'
-            y_label = 'Strain Energy'
-        elif self.type.value() == "contractility":
-            mu_name = 'contractility'
-            y_label = 'Contractility'
-        elif self.type.value() == "polarity":
-            mu_name = 'polarity'
-            y_label = 'Polarity'
-        elif self.type.value() == "99_percentile_deformation":
-            mu_name = '99_percentile_deformation'
-            y_label = 'Deformation'
-        elif self.type.value() == "99_percentile_force":
-            mu_name = '99_percentile_force'
-            y_label = 'Force'
+        mu_name, y_label = self.get_label()
 
         self.canvas.setActive()
         plt.cla()
         res = self.getAllCurrentPandasData()
 
         code_data = [res, ["t", "group", mu_name, "filename"]]
 
+        # add a vertical line where the comparison time is
+        if getattr(self, "input_tbar", None) and self.input_tbar.value() is not None:
+            comp_h = self.get_comparison_index() * (res.iloc[1]["t"] - res.iloc[0]["t"])
+            plt.axvline(comp_h, color="k")
+
         color_dict = {d[0]: d[3] for d in self.data_folders}
 
         def plot(res, mu_name, y_label, color_dict2):
             # define the colors
             color_dict = color_dict2
 
             # iterate over the groups
@@ -400,29 +411,15 @@
         if not self.button_run.isEnabled():
             return
         for button in self.plot_buttons:
             button.setChecked(False)
         self.button_run.setChecked(True)
         #return
         self.current_plot_func = self.run2
-        if self.type.value() == "strain_energy":
-            mu_name = 'strain_energy'
-            y_label = 'Strain Energy'
-        elif self.type.value() == "contractility":
-            mu_name = 'contractility'
-            y_label = 'Contractility'
-        elif self.type.value() == "polarity":
-            mu_name = 'polarity'
-            y_label = 'Polarity'
-        elif self.type.value() == "99_percentile_deformation":
-            mu_name = '99_percentile_deformation'
-            y_label = 'Deformation'
-        elif self.type.value() == "99_percentile_force":
-            mu_name = '99_percentile_force'
-            y_label = 'Force'
+        mu_name, y_label = self.get_label()
         if 0:
             if self.type.value() == "Contractility":
                 mu_name = 'Mean Contractility (µN)'
                 std_name = 'St.dev. Contractility (µN)'
                 y_label = 'Contractility (µN)'
             else:
                 mu_name = 'Mean Pressure (Pa)'
@@ -466,14 +463,15 @@
         dialog = ExportDialog(self, self.settings)
         if not dialog.exec():
             return
 
         with open(str(dialog.inputText.value()), "wb") as fp:
             code = ""
             code += "import matplotlib.pyplot as plt\n"
+            code += "import numpy as np\n"
             code += "import pandas as pd\n"
             code += "import io\n"
             code += "\n"
             code += "# the data for the plot\n"
             res, columns = self.export_data[1]
             if dialog.strip_data.value() is False:
                 columns = None
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/gui_solver.py` & `saenopy-1.0.4/saenopy/gui/solver/gui_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
         main_layout = QtWidgets.QHBoxLayout(self)
 
         with QtShortCuts.QTabWidget(main_layout) as self.tabs:
             with self.tabs.createTab("Analyse Measurements"):
                 with QtShortCuts.QHBoxLayout():
                     self.deformations = BatchEvaluate(self)
-                    QtShortCuts.current_layout.addWidget(self.deformations)
+                    QtShortCuts.currentLayout().addWidget(self.deformations)
 
             with self.tabs.createTab("Data Analysis"):
                 with QtShortCuts.QHBoxLayout():
-                    self.plotting_window = PlottingWindow(self).addToLayout()
+                    self.plotting_window = PlottingWindow(self, self.deformations).addToLayout()
 
 
 if __name__ == '__main__':  # pragma: no cover
     app = QtWidgets.QApplication(sys.argv)
     if sys.platform.startswith('win'):
         import ctypes
         myappid = 'fabrylab.saenopy.master'  # arbitrary string
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/BatchEvaluate.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/Regularizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,402 +1,278 @@
-import json
-import sys
 import os
-
-import qtawesome as qta
-from qtpy import QtCore, QtWidgets, QtGui
+import time
+from qtpy import QtCore, QtWidgets
 import numpy as np
-import glob
-import threading
-from pathlib import Path
-import matplotlib as mpl
-
-import traceback
+from pyvistaqt import QtInteractor
+import inspect
+from typing import Tuple
 
-from saenopy import get_stacks
+import saenopy
+import saenopy.multigrid_helper
 from saenopy import Result
+import saenopy.get_deformations
+import saenopy.materials
 from saenopy.gui.common import QtShortCuts
-from saenopy.gui.common.gui_classes import ListWidget
-from saenopy.gui.common.stack_selector_tif import add_last_voxel_size, add_last_time_delta
+from saenopy.gui.common.gui_classes import CheckAbleGroup, MatplotlibWidget, NavigationToolbar
+
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
+from .VTK_Toolbar import VTK_Toolbar
+from .showVectorField import showVectorField, getVectorFieldImage
+from .DeformationDetector import CamPos
+from saenopy.gui.common.code_export import get_code
+
+
+class Regularizer(PipelineModule):
+    pipeline_name = "fit forces"
+    iteration_finished = QtCore.Signal(object, object, int, int)
+
+    def __init__(self, parent: "BatchEvaluate", layout):
+        super().__init__(parent, layout)
+
+        with QtShortCuts.QVBoxLayout(self) as layout:
+            layout.setContentsMargins(0, 0, 0, 0)
+            with CheckAbleGroup(self, "fit forces (regularize)", url="https://saenopy.readthedocs.io/en/latest/interface_solver.html#fit-deformations-and-calculate-forces").addToLayout() as self.group:
+
+                with QtShortCuts.QVBoxLayout() as main_layout:
+                    with QtShortCuts.QGroupBox(None, "Material Parameters") as self.material_parameters:
+                        with QtShortCuts.QHBoxLayout() as layout2:
+                            self.input_k = QtShortCuts.QInputString(None, "k", "1645", type=float, tooltip="the stiffness of the material's fibers")
+                            self.input_d_0 = QtShortCuts.QInputString(None, "d_0", "0.0008", type=float, tooltip="the bluckling strength of the material's fibers")
+                            self.input_lamda_s = QtShortCuts.QInputString(None, "λ_s", "0.0075", type=float, tooltip="the length at which strain stiffening of the material's fibers starts")
+                            self.input_d_s = QtShortCuts.QInputString(None, "d_s", "0.033", type=float, tooltip="the strain stiffening strength of the material's fibers")
+
+                    with QtShortCuts.QGroupBox(None, "Regularisation Parameters") as self.material_parameters:
+                        self.input_previous_t_as_start = QtShortCuts.QInputBool(None, "use previous time steps deformation field", True,
+                                                                tooltip="wether to use the previous time steps deformation field as a starting value for the next regularisation")
+                        with QtShortCuts.QHBoxLayout(None) as layout:
+                            self.input_alpha = QtShortCuts.QInputString(None, "alpha", "1e10", type="exp", tooltip="the strength of the regularisation (higher values mean weaker forces)")
+                            self.input_step_size = QtShortCuts.QInputString(None, "step size", "0.33", type=float, tooltip="the step with of the iteration algorithm")
+                        with QtShortCuts.QHBoxLayout(None) as layout:
+                            self.input_imax = QtShortCuts.QInputNumber(None, "max iterations", 100, float=False, tooltip="the maximum number of iterations after which to abort the iteration algorithm")
+                            self.input_conv_crit = QtShortCuts.QInputString(None, "rel. conv. crit.", 0.01, type=float, tooltip="the convergence criterion of the iteration algorithm")
+
+                    self.input_button = QtShortCuts.QPushButton(None, "calculate forces", self.start_process, tooltip="run the force calculation")
+
+                    self.canvas = MatplotlibWidget(self).addToLayout()
+                    #NavigationToolbar(self.canvas, self).addToLayout()
+
+        with self.parent.tabs.createTab("Forces") as self.tab:
+            with QtShortCuts.QVBoxLayout() as layout:
+                self.label_tab = QtWidgets.QLabel("The fitted regularized forces.").addToLayout()
 
-from .DeformationDetector import DeformationDetector
-from .FittedMesh import FittedMesh
-from .MeshCreator import MeshCreator
-from .Regularizer import Regularizer
-from .ResultView import ResultView
-from .StackDisplay import StackDisplay
-from saenopy.gui.solver.modules.exporter.Exporter import ExportViewer
-from .load_measurement_dialog import AddFilesDialog, FileExistsDialog
-from .path_editor import start_path_change
-from saenopy.examples import get_examples
-
-
-class SharedProperties:
-    properties = None
-
-    def __init__(self):
-        self.properties = {}
-
-    def add_property(self, name, target):
-        if name not in self.properties:
-            self.properties[name] = []
-        self.properties[name].append(target)
-
-    def change_property(self, name, value, target):
-        if name in self.properties:
-            for t in self.properties[name]:
-                if t != target:
-                    t.property_changed(name, value)
-
-
-class BatchEvaluate(QtWidgets.QWidget):
-    result_changed = QtCore.Signal(object)
-    tab_changed = QtCore.Signal(object)
-    set_current_result = QtCore.Signal(object)
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-        self.shared_properties = SharedProperties()
-
-        self.settings = QtCore.QSettings("Saenopy", "Seanopy_deformation")
-
-        with QtShortCuts.QHBoxLayout(self) as main_layout:
-            main_layout.setContentsMargins(0, 0, 0, 0)
-            with QtShortCuts.QSplitter() as lay:
-                with QtShortCuts.QVBoxLayout() as layout:
-                    layout.setContentsMargins(0, 0, 0, 0)
-                    self.list = ListWidget(layout, add_item_button="add measurements", copy_params=True, allow_paste_callback=self.allow_paste)
-                    self.list.addItemClicked.connect(self.add_measurement)
-                    self.list.signal_act_copy_clicked.connect(self.copy_params)
-                    self.list.signal_act_paste_clicked.connect(self.paste_params)
-                    self.list.signal_act_paths_clicked.connect(self.path_editor)
-                    self.list.itemSelectionChanged.connect(self.listSelected)
-                    self.progressbar = QtWidgets.QProgressBar().addToLayout()
-                    self.progressbar.setOrientation(QtCore.Qt.Horizontal)
                 with QtShortCuts.QHBoxLayout() as layout:
-                    layout.setContentsMargins(0, 0, 0, 0)
-                    with QtShortCuts.QTabWidget(layout) as self.tabs:
-                        self.tabs.setMinimumWidth(500)
-                        old_tab = None
-                        cam_pos = None
-                        def tab_changed(x):
-                            nonlocal old_tab, cam_pos
-                            tab = self.tabs.currentWidget()
-                            if old_tab is not None and getattr(old_tab, "plotter", None):
-                                cam_pos = old_tab.plotter.camera_position
-                            if cam_pos is not None and getattr(tab, "plotter", None):
-                                tab.plotter.camera_position = cam_pos
-                            if old_tab is not None:
-                                tab.t_slider.setValue(old_tab.t_slider.value())
-                            old_tab = tab
-                            self.tab_changed.emit(tab)
-                        self.tabs.currentChanged.connect(tab_changed)
-                        pass
-                with QtShortCuts.QVBoxLayout() as layout0:
-                    layout0.parent().setMaximumWidth(420)
-                    layout0.setContentsMargins(0, 0, 0, 0)
-                    self.sub_module_stacks = StackDisplay(self, layout0)
-                    self.sub_module_deformation = DeformationDetector(self, layout0)
-                    self.sub_module_mesh = MeshCreator(self, layout0)
-                    self.sub_module_fitted_mesh = FittedMesh(self, layout0)
-                    self.sub_module_regularize = Regularizer(self, layout0)
-                    self.sub_module_view = ResultView(self, layout0)
-                    #self.sub_module_fiber = FiberViewer(self, layout0)
-                    self.sub_module_export = ExportViewer(self, layout0)
-                    layout0.addStretch()
-                    self.button_start_all = QtShortCuts.QPushButton(None, "run all", self.run_all)
-                    with QtShortCuts.QHBoxLayout():
-                        self.button_code = QtShortCuts.QPushButton(None, "export code", self.generate_code)
-                        self.button_export = QtShortCuts.QPushButton(None, "export images", lambda x: self.sub_module_export.export_window.show())
-
-        self.data = []
-        self.list.setData(self.data)
-
-        self.setAcceptDrops(True)
-
-        self.tasks = []
-        self.current_task_id = 0
-        self.thread = None
-        self.signal_task_finished.connect(self.run_finished)
-
-        # load paths
-        self.load_from_path([arg for arg in sys.argv if arg.endswith(".saenopy")])
-
-        # disable all tabs
-        for i in range(self.tabs.count()-1, -1, -1):
-            self.tabs.setTabEnabled(i, False)
-
-    def copy_params(self):
-        result = self.list.data[self.list.currentRow()][2]
-        params = {
-            "piv_parameters": result.piv_parameters_tmp,
-            "mesh_parameters": result.mesh_parameters_tmp,
-            "material_parameters": result.material_parameters_tmp,
-            "solve_parameters": result.solve_parameters_tmp,
-        }
-        print(params)
-        for group in params:
-            if params[group] is None:
-                continue
-            for g in params[group]:
-                if type(params[group][g]) == np.bool_:
-                    params[group][g] = bool(params[group][g])
-                if type(params[group][g]) == np.int64:
-                    params[group][g] = int(params[group][g])
-        text = json.dumps(params, indent=2)
-        cb = QtGui.QGuiApplication.clipboard()
-        cb.setText(text, mode=cb.Clipboard)
-
-    def allow_paste(self):
-        cb = QtGui.QGuiApplication.clipboard()
-        text = cb.text(mode=cb.Clipboard)
+                    self.plotter = QtInteractor(self, auto_update=False)  # , theme=pv.themes.DocumentTheme())
+                    self.tab.parent().plotter = self.plotter
+                    self.plotter.set_background("black")
+                    layout.addWidget(self.plotter.interactor)
+
+                    self.z_slider = QTimeSlider("z", self.z_slider_value_changed, "set z position",
+                                                QtCore.Qt.Vertical).addToLayout()
+                    self.z_slider.t_slider.valueChanged.connect(
+                        lambda value: parent.shared_properties.change_property("z_slider", value, self))
+                    parent.shared_properties.add_property("z_slider", self)
+
+                self.vtk_toolbar = VTK_Toolbar(self.plotter, self.update_display, center=True, shared_properties=self.parent.shared_properties).addToLayout()
+
+                self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
+                self.tab.parent().t_slider = self.t_slider
+
+        self.setParameterMapping("material_parameters", {
+            "k": self.input_k,
+            "d_0": self.input_d_0,
+            "lambda_s": self.input_lamda_s,
+            "d_s": self.input_d_s,
+        })
+        self.setParameterMapping("solve_parameters", {
+            "alpha": self.input_alpha,
+            "step_size": self.input_step_size,
+            "max_iterations": self.input_imax,
+            "rel_conv_crit": self.input_conv_crit,
+            "prev_t_as_start": self.input_previous_t_as_start,
+        })
+
+        self.iteration_finished.connect(self.iteration_callback)
+        self.iteration_finished.emit(None, np.ones([10, 3]), 0, None)
+
+    def z_slider_value_changed(self):
+        self.update_display()
+
+    def check_available(self, result: Result):
         try:
-            data = json.loads(text)
-            if "piv_parameters" in data and \
-                "mesh_parameters" in data and \
-                "material_parameters" in data and \
-                "solve_parameters" in data:
-                return True
-        except (ValueError, TypeError):
+            return self.result.solvers[0] is not None
+        except (AttributeError, IndexError, TypeError):
             return False
-        return False
 
-    def paste_params(self):
-        cb = QtGui.QGuiApplication.clipboard()
-        text = cb.text(mode=cb.Clipboard)
+    def check_evaluated(self, result: Result) -> bool:
         try:
-            data = json.loads(text)
-        except ValueError:
+            if self.result is not None and self.result.solvers is not None:
+                relrec = getattr(self.result.solvers[self.t_slider.value()], "relrec", None)
+                if relrec is not None:
+                    return True
+            return getattr(self.result.solvers[0], "regularisation_results", None) is not None
+        except (AttributeError, IndexError, TypeError):
             return False
-        result = self.list.data[self.list.currentRow()][2]
-        params = ["piv_parameters", "mesh_parameters", "material_parameters", "solve_parameters"]
-        for par in params:
-            if par in data:
-                setattr(result, par+"_tmp", data[par])
-        self.set_current_result.emit(result)
-
-    def path_editor(self):
-        result = self.list.data[self.list.currentRow()][2]
-        start_path_change(self, result)
-
-    def progress(self, tup):
-        n, total = tup
-        self.progressbar.setMaximum(total)
-        self.progressbar.setValue(n)
-
-    def generate_code(self):
-        new_path = QtWidgets.QFileDialog.getSaveFileName(None, "Save Session as Script", os.getcwd(), "Python File (*.py)")
-        if new_path:
-            # ensure filename ends in .py
-            if not new_path.endswith(".py"):
-                new_path += ".py"
-
-            import_code = ""
-            run_code = ""
-            for module in [self.sub_module_stacks, self.sub_module_deformation, self.sub_module_mesh, self.sub_module_regularize]:
-                code1, code2 = module.get_code()
-                import_code += code1
-                run_code += code2 +"\n"
-            run_code = import_code + "\n\n" + run_code
-            #print(run_code)
-            with open(new_path, "w") as fp:
-                fp.write(run_code)
-
-    def run_all(self):
-        for i in range(len(self.data)):
-            if not self.data[i][1]:
-                continue
-            result = self.data[i][2]
-            if self.sub_module_deformation.group.value() is True:
-                self.sub_module_deformation.start_process(result=result)
-            if self.sub_module_mesh.group.value() is True:
-                self.sub_module_mesh.start_process(result=result)
-            if self.sub_module_regularize.group.value() is True:
-                self.sub_module_regularize.start_process(result=result)
-
-    def addTask(self, task, result, params, name):
-        self.tasks.append([task, result, params, name])
-        if self.thread is None:
-            self.run_next()
-
-    signal_task_finished = QtCore.Signal()
-
-    def run_next(self):
-        task, result, params, name = self.tasks[self.current_task_id]
-        self.thread = threading.Thread(target=self.run_thread, args=(task, result, params, name), daemon=True)
-        self.thread.start()
-
-    def run_thread(self, task, result, params, name):
-        result.state = True
-        self.update_icons()
-        task(result, params)
-        self.signal_task_finished.emit()
-        result.state = False
-        self.update_icons()
-
-    def run_finished(self):
-        self.current_task_id += 1
-        self.thread = None
-        if self.current_task_id < len(self.tasks):
-            self.run_next()
-
-    def dragEnterEvent(self, event: QtGui.QDragEnterEvent):
-        # accept url lists (files by drag and drop)
-        for url in event.mimeData().urls():
-            # if str(url.toString()).strip().endswith(".npz"):
-            event.accept()
-            return
-        event.ignore()
 
-    def dragMoveEvent(self, event: QtGui.QDragMoveEvent):
-        event.acceptProposedAction()
+    def iteration_callback(self, result, relrec, i=0, imax=None):
+        if imax is not None:
+            self.parent.progressbar.setRange(0, imax)
+            self.parent.progressbar.setValue(i)
+        if result is self.result:
+            for i in range(self.parent.tabs.count()):
+                if self.parent.tabs.widget(i) == self.tab.parent():
+                    self.parent.tabs.setTabEnabled(i, self.check_evaluated(result))
+            if self.canvas is not None:
+                relrec = np.array(relrec).reshape(-1, 3)
+                self.canvas.figure.axes[0].cla()
+                self.canvas.figure.axes[0].semilogy(relrec[:, 0], label="total loss")
+                self.canvas.figure.axes[0].semilogy(relrec[:, 1], ":", label="least squares loss")
+                self.canvas.figure.axes[0].semilogy(relrec[:, 2], "--", label="regularize loss")
+                self.canvas.figure.axes[0].legend()
+                self.canvas.figure.axes[0].spines["top"].set_visible(False)
+                self.canvas.figure.axes[0].spines["right"].set_visible(False)
+                ticks = self.canvas.figure.axes[0].get_xticks()
+                self.canvas.figure.axes[0].set_xticks([t for t in ticks if t < self.canvas.figure.axes[0].get_xlim()[1]*0.7])
 
-    def dropEvent(self, event: QtCore.QEvent):
-        urls = []
-        for url in event.mimeData().urls():
-
-            url = url.toLocalFile()  # path()
-
-            if url[0] == "/" and url[2] == ":":
-                url = url[1:]
-            urls.append(url)
-        self.load_from_path(urls)
-
-    def load_from_path(self, paths):
-        # make sure that paths is a list
-        if isinstance(paths, (str, Path)):
-            paths = [paths]
-
-        # iterate over all paths
-        for path in paths:
-            # if it is a directory search all saenopy files in it
-            path = Path(path)
-            if path.is_dir():
-                path = str(path) + "/**/*.saenopy"
-            # glob over the path (or just use the path if it does not contain a *)
-            for p in sorted(glob.glob(str(path), recursive=True)):
-                print(p)
+                self.canvas.figure.axes[0].text(0, 1, "error  ", ha="right", transform=self.canvas.figure.axes[0].transAxes)
+                self.canvas.figure.axes[0].text(1, 0, "\n\niteration", ha="right", va="center", transform=self.canvas.figure.axes[0].transAxes)
                 try:
-                    self.add_data(Result.load(p))
-                except Exception as err:
-                    QtWidgets.QMessageBox.critical(self, "Open Files", f"File {p} is not a valid Saenopy file.")
-                    traceback.print_exc()
-        self.update_icons()
-
-    def add_data(self, data):
-        self.list.addData(data.output, True, data, mpl.colors.to_hex(f"gray"))
-
-    def update_icons(self):
-        for j in range(self.list.count( ) -1):
-            if self.data[j][2].state is True:
-                self.list.item(j).setIcon(qta.icon("fa5s.hourglass-half", options=[dict(color="orange")]))
-            else:
-                self.list.item(j).setIcon(qta.icon("fa5.circle", options=[dict(color="gray")]))
-
-    def add_measurement(self):
-        last_decision = None
-        def do_overwrite(filename):
-            nonlocal last_decision
-
-            # if we are in demo mode always load the files
-            if os.environ.get("DEMO") == "true":  # pragma: no cover
-                return "read"
-
-            # if there is a last decistion stored use that
-            if last_decision is not None:
-                return last_decision
-
-            # ask the user if they want to overwrite or read the existing file
-            dialog = FileExistsDialog(self, filename)
-            result = dialog.exec()
-            # if the user clicked cancel
-            if not result:
-                return 0
-            # if the user wants to remember the last decision
-            if dialog.use_for_all.value():
-                last_decision = dialog.mode
-            # return the decision
-            return dialog.mode
-
-        # getStack
-        dialog = AddFilesDialog(self, self.settings)
-        if not dialog.exec():
+                    self.canvas.figure.tight_layout(pad=0)
+                except np.linalg.LinAlgError:
+                    pass
+                self.canvas.draw()
+
+    def process(self, result: Result, material_parameters: dict, solve_parameters: dict):
+        # demo run
+        if os.environ.get("DEMO") == "true":
+            imax = 100
+            self.parent.progressbar.setRange(0, imax)
+            for i in range(len(result.solver_relrec_demo)):
+                time.sleep(0.2)
+                self.iteration_finished.emit(result, result.solver_relrec_demo[:i], i, imax)
+            result.solvers[0].regularisation_results = result.solver_relrec_demo
             return
 
-        # create a new measurement object
-        if dialog.mode == "new":
-            # if there was a reference stack selected
-            if dialog.reference_choice.value() == 1:
-                reference_stack = dialog.stack_reference_input.text()
-            else:
-                reference_stack = None
+        for i in range(len(result.solvers)):
+            M = result.solvers[i]
 
-            # the active selected stack
-            active_stack = dialog.stack_data_input.text()
+            if i > 0 and solve_parameters["prev_t_as_start"]:
+                M.mesh.displacements[:] = result.solvers[i-1].mesh.displacements.copy()
 
-            # if there was a time specified, get the time delta
-            if "{t}" in active_stack:
-                time_delta = dialog.stack_data.getTimeDelta()
-                add_last_time_delta(dialog.stack_data.getTimeDelta())
+            def callback(M, relrec, i, imax):
+                self.iteration_finished.emit(result, relrec, i, imax)
+
+            M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
+                               material_parameters["k"],
+                               material_parameters["d_0"] if material_parameters["d_0"] != "None" else None,
+                               material_parameters["lambda_s"] if material_parameters["lambda_s"] != "None" else None,
+                               material_parameters["d_s"] if material_parameters["d_s"] != "None" else None,
+                               ))
+
+            M.solve_regularized(step_size=solve_parameters["step_size"], max_iterations=solve_parameters["max_iterations"],
+                                alpha=solve_parameters["alpha"], rel_conv_crit=solve_parameters["rel_conv_crit"],
+                                callback=callback, verbose=True)
+
+            # clear the cache of the solver
+            result.clear_cache(i)
+
+    def property_changed(self, name, value):
+        if name == "z_slider":
+            self.z_slider.setValue(value)
+
+    def setResult(self, result: Result):
+        super().setResult(result)
+        if result and result.stacks and result.stacks[0]:
+            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
+            self.z_slider.setValue(self.result.stacks[0].shape[2] // 2)
+
+            if result.stacks[0].channels:
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
+                self.vtk_toolbar.channel_select.setVisible(True)
             else:
-                time_delta = None
+                self.vtk_toolbar.channel_select.setValue(0)
+                self.vtk_toolbar.channel_select.setVisible(False)
+
+    def update_display(self):
+        if self.current_tab_selected is False:
+            self.current_result_plotted = False
+            return
 
-            try:
-                # load the stack
-                results = get_stacks(
-                    active_stack,
-                    reference_stack=reference_stack,
-                    output_path=dialog.outputText.value(),
-                    voxel_size=dialog.stack_data.getVoxelSize(),
-                    time_delta=time_delta,
-                    crop=dialog.stack_data.get_crop(),
-                    exist_overwrite_callback=do_overwrite,
-                )
-            except Exception as err:
-                # notify the user if errors occured
-                QtWidgets.QMessageBox.critical(self, "Load Stacks", str(err))
-                traceback.print_exc()
+        if self.check_evaluated(self.result):
+            cam_pos = None
+            if self.plotter.camera_position is not None and CamPos.cam_pos_initialized is True:
+                cam_pos = self.plotter.camera_position
+            CamPos.cam_pos_initialized = True
+            M = self.result.solvers[self.t_slider.value()]
+            mesh = M.mesh
+            self.plotter.interactor.setToolTip(str(self.result.solve_parameters) + f"\nNodes {mesh.nodes.shape[0]}\nTets {mesh.tetrahedra.shape[0]}")
+            center = None
+            if self.vtk_toolbar.use_center.value() is True:
+                center = M.get_center(mode="Force")
+            display_image = getVectorFieldImage(self)
+            if len(self.result.stacks):
+                stack_shape = np.array(self.result.stacks[0].shape[:3]) * np.array(self.result.stacks[0].voxel_size)
+            else:
+                stack_shape = None
+                
+            if M.mesh.regularisation_mask is not None:
+                f = -M.mesh.forces * M.mesh.regularisation_mask[:, None]
             else:
-                # store the last voxel size
-                add_last_voxel_size(dialog.stack_data.getVoxelSize())
-                # add the loaded measruement objects
-                for data in results:
-                    self.add_data(data)
-
-        # load existing files
-        elif dialog.mode == "existing":
-            self.load_from_path(dialog.outputText3.value())
-
-        # load from the examples database
-        elif dialog.mode == "example":
-            # get the date from the example referenced by name
-            example = get_examples()[dialog.mode_data]
-
-            # generate a stack with the examples data
-            results = get_stacks(
-                example["stack"],
-                reference_stack=example.get("reference_stack", None),
-                output_path=example["output_path"],
-                voxel_size=example["voxel_size"],
-                time_delta=example.get("time_delta", None),
-                crop=example.get("crop", None),
-                exist_overwrite_callback=do_overwrite,
-            )
-            # load all the measurement objects
-            for data in results:
-                if getattr(data, "is_read", False) is False:
-                    data.piv_parameters = example["piv_parameters"]
-                    data.mesh_parameters = example["mesh_parameters"]
-                    data.material_parameters = example["material_parameters"]
-                    data.solve_parameters = example["solve_parameters"]
-                self.add_data(data)
-        elif dialog.mode == "example_evaluated":
-                self.load_from_path(dialog.examples_output)
-
-        # update the icons
-        self.update_icons()
-
-    def listSelected(self):
-        if self.list.currentRow() is not None and self.list.currentRow() < len(self.data):
-            pipe = self.data[self.list.currentRow()][2]
-            self.set_current_result.emit(pipe)
+                f =  -M.mesh.forces
+                
+            showVectorField(self.plotter, M.mesh, f, "forces", center=center,
+                            factor=0.15 * self.vtk_toolbar.arrow_scale.value(),
+                            colormap=self.vtk_toolbar.colormap_chooser.value(),
+                            colormap2=self.vtk_toolbar.colormap_chooser2.value(),
+                            scalebar_max=self.vtk_toolbar.getScaleMax(), show_nan=self.vtk_toolbar.use_nans.value(),
+                            display_image=display_image, show_grid=self.vtk_toolbar.show_grid.value(),
+                            stack_shape=stack_shape, log_scale=self.vtk_toolbar.use_log.value())
+            if cam_pos is not None:
+                self.plotter.camera_position = cam_pos
+            relrec = getattr(self.result.solvers[self.t_slider.value()], "relrec", None)
+            if relrec is None:
+                relrec = self.result.solvers[self.t_slider.value()].regularisation_results
+            self.iteration_callback(self.result, relrec)
+        else:
+            self.plotter.interactor.setToolTip("")
+
+    def get_code(self) -> Tuple[str, str]:
+        import_code = "import saenopy\n"
+        results: Result = None
+        def code(my_reg_params1, my_reg_params2):  # pragma: no cover
+            # define the parameters to generate the solver mesh and interpolate the piv mesh onto it
+            material_parameters = my_reg_params1
+            solve_parameters = my_reg_params2
+
+            # iterate over all the results objects
+            for result in results:
+                result.material_parameters = material_parameters
+                result.solve_parameters = solve_parameters
+                for index, M in enumerate(result.solvers):
+                    # optionally copy the displacement field from the previous time step as a starting value
+                    if index > 0 and solve_parameters["prev_t_as_start"]:
+                        M.mesh.displacements[:] = result.solvers[index - 1].mesh.displacements.copy()
+
+                    # set the material model
+                    M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
+                        material_parameters["k"],
+                        material_parameters["d_0"],
+                        material_parameters["lambda_s"],
+                        material_parameters["d_s"],
+                    ))
+                    # find the regularized force solution
+                    M.solve_regularized(alpha=solve_parameters["alpha"], step_size=solve_parameters["step_size"],
+                                        max_iterations=solve_parameters["max_iterations"], rel_conv_crit=solve_parameters["rel_conv_crit"],
+                                        verbose=True)
+                    # save the forces
+                    result.save()
+                    # clear the cache of the solver
+                    result.clear_cache(index)
+
+        # params with convert text Nones to real Nones
+        data = {
+            "my_reg_params1": {k: None if v == "None" else v for k, v in self.result.material_parameters_tmp.items()},
+            "my_reg_params2": {k: None if v == "None" else v for k, v in self.result.solve_parameters_tmp.items()},
+        }
+
+        code = get_code(code, data)
+        return import_code, code
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/DeformationDetector.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/DeformationDetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import saenopy.multigrid_helper
 import saenopy.materials
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import CheckAbleGroup, QProcess, ProcessSimple
 import saenopy.get_deformations
 
-from .PipelineModule import PipelineModule
-from .QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
 from .showVectorField import showVectorField, showVectorField2
-from .code_export import get_code
+from saenopy.gui.common.code_export import get_code
 
 
 class CamPos:
     cam_pos_initialized = False
 
 
 class DeformationDetector(PipelineModule):
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/FittedMesh.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/FittedMesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 from qtpy import QtCore, QtWidgets
 from pyvistaqt import QtInteractor
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import MatplotlibWidget, NavigationToolbar
 from saenopy import Result
 
-from .PipelineModule import PipelineModule
-from .QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
 from .showVectorField import showVectorField2
 from .DeformationDetector import CamPos
 
 
 class FittedMesh(PipelineModule):
     pipeline_name = "fit forces"
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/MeshCreator.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/MeshCreator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 from saenopy.saveable import Saveable
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
 from saenopy.gui.common.gui_classes import Spoiler, CheckAbleGroup, QHLine, QVLine, MatplotlibWidget, NavigationToolbar, execute, kill_thread, ListWidget, QProcess, ProcessSimple
 from saenopy.gui.common.stack_selector import StackSelector
 
 
-from .PipelineModule import PipelineModule
-from .QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from .VTK_Toolbar import VTK_Toolbar
 from .showVectorField import showVectorField, showVectorField2
 from .DeformationDetector import CamPos
-from .code_export import get_code
+from saenopy.gui.common.code_export import get_code
 
 class MeshSizeWidget(QtWidgets.QWidget):
     valueChanged = QtCore.Signal(object)
 
     def __init__(self):
         super().__init__()
         with QtShortCuts.QVBoxLayout(self):
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/PipelineModule.py` & `saenopy-1.0.4/saenopy/gui/tfm2d/modules/PipelineModule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import qtawesome as qta
 from qtpy import QtCore, QtWidgets
-from saenopy import Result
+from .result import Result2D
 from typing import Tuple, List
 import traceback
 
 
 class ParameterMapping:
     params_name: str = None
     parameter_dict: dict = None
 
-    result: Result = None
+    result: Result2D = None
 
     def __init__(self, params_name: str = None, parameter_dict: dict=None):
         self.params_name = params_name
         self.parameter_dict = parameter_dict
         for name, widget in self.parameter_dict.items():
             widget.valueChanged.connect(lambda x, name=name: self.setParameter(name, x))
 
@@ -42,15 +42,15 @@
                     params_tmp[name] = widget.value()
 
     def setDisabled(self, disabled):
         # disable all the widgets
         for name, widget in self.parameter_dict.items():
             widget.setDisabled(disabled)
 
-    def setResult(self, result: Result):
+    def setResult(self, result: Result2D):
         """ set a new active result object """
         self.result = result
 
         # if a result file is given
         if result is not None:
             self.ensure_tmp_params_initialized(result)
             params_tmp = getattr(result, self.params_name + "_tmp")
@@ -61,15 +61,15 @@
 
 
 class PipelineModule(QtWidgets.QWidget):
     processing_finished = QtCore.Signal()
     processing_progress = QtCore.Signal(tuple)
     processing_state_changed = QtCore.Signal(object)
     processing_error = QtCore.Signal(str)
-    result: Result = None
+    result: Result2D = None
     tab: QtWidgets.QTabWidget = None
 
     parameter_mappings: List[ParameterMapping] = None
     params_name: None
 
     def __init__(self, parent: "BatchEvaluate", layout):
         super().__init__()
@@ -106,32 +106,32 @@
             self.current_tab_selected = True
             if self.current_result_plotted is False:
                 self.update_display()
                 self.current_result_plotted = True
         else:
             self.current_tab_selected = False
 
-    def check_available(self, result: Result) -> bool:
+    def check_available(self, result: Result2D) -> bool:
         return False
 
-    def check_evaluated(self, result: Result) -> bool:
+    def check_evaluated(self, result: Result2D) -> bool:
         return False
 
-    def resultChanged(self, result: Result):
+    def resultChanged(self, result: Result2D):
         """ called when the contents of result changed. Only update view if it is the currently displayed one. """
         if result is self.result:
             if self.tab is not None:
                 for i in range(self.parent.tabs.count()):
                     if self.parent.tabs.widget(i) == self.tab.parent():
                        self.parent.tabs.setTabEnabled(i, self.check_evaluated(result))
             if self.current_tab_selected is True:
                 self.update_display()
             self.state_changed(result)
 
-    def state_changed(self, result: Result):
+    def state_changed(self, result: Result2D):
         if result is self.result and getattr(self, "group", None) is not None:
             state = getattr(result, self.params_name + "_state", "")
             if state == "scheduled":
                 self.group.label.setIcon(qta.icon("fa5s.hourglass-start", options=[dict(color="gray")]))
                 self.group.label.setToolTip("scheduled")
             elif state == "running":
                 self.group.label.setIcon(qta.icon("fa5s.hourglass-half", options=[dict(color="orange")]))
@@ -157,27 +157,24 @@
                 for mapping in self.parameter_mappings:
                     mapping.setDisabled(False)
                 if getattr(self, "input_button", None):
                     self.input_button.setEnabled(self.check_available(result))
             #if getattr(self, "input_button", None):
             #    self.input_button.setEnabled(self.check_available(result))
 
-    def setResult(self, result: Result):
+    def setResult(self, result: Result2D):
         """ set a new active result object """
         #if result == self.result:
         #    return
         self.current_result_plotted = False
         self.result = result
 
         for mapping in self.parameter_mappings:
             mapping.setResult(result)
 
-        if result is not None:
-            self.t_slider.setRange(0, len(result.stacks) - 2)
-
         self.state_changed(result)
         if self.tab is not None:
             for i in range(self.parent.tabs.count()):
                 if self.parent.tabs.widget(i) == self.tab.parent():
                     self.parent.tabs.setTabEnabled(i, self.check_evaluated(result))
 
         # check if the results instance can be evaluated currently with this module
@@ -219,15 +216,15 @@
         for mapping in self.parameter_mappings:
             mapping.ensure_tmp_params_initialized(result)
             params[mapping.params_name] = getattr(result, mapping.params_name + "_tmp")
         setattr(result, self.params_name + "_state", "scheduled")
         self.processing_state_changed.emit(result)
         return self.parent.addTask(self.process_thread, result, params, "xx")
 
-    def process_thread(self, result: Result, params: dict):
+    def process_thread(self, result: Result2D, params: dict):
         #params = getattr(result, self.params_name + "_tmp")
         self.parent.progressbar.setRange(0, 0)
         setattr(result, self.params_name + "_state", "running")
         self.processing_state_changed.emit(result)
         try:
             self.process(result, **params)
             # store the parameters that have been used for evaluation
@@ -239,15 +236,15 @@
             self.processing_finished.emit()
         except Exception as err:
             traceback.print_exc()
             setattr(result, self.params_name + "_state", "failed")
             self.processing_state_changed.emit(result)
             self.processing_error.emit(str(err))
 
-    def process(self, result: Result, params: dict):
+    def process(self, result: Result2D, params: dict):
         pass
 
     def finished_process(self):
         self.parent.progressbar.setRange(0, 1)
 
     def errored_process(self, text: str):
         QtWidgets.QMessageBox.critical(self, "Deformation Detector", text)
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/QTimeSlider.py` & `saenopy-1.0.4/saenopy/gui/common/QTimeSlider.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/ResultView.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/ResultView.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from pyvistaqt import QtInteractor
 
 import imageio
 from saenopy.gui.common import QtShortCuts
 from saenopy import Result, Solver
 from saenopy.materials import SemiAffineFiberMaterial
 
-from .PipelineModule import PipelineModule
-from .QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 
 
 result_view = None
 class ResultView(PipelineModule):
     M: Solver = None
 
     def __init__(self, parent: "BatchEvaluate", layout):
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/StackDisplay.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/StackDisplay.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 import saenopy.get_deformations
 import saenopy.multigrid_helper
 import saenopy.materials
 from saenopy import Result
 from saenopy.gui.common.resources import resource_icon
 
 
-from .PipelineModule import PipelineModule
-from .QTimeSlider import QTimeSlider
-from .code_export import get_code
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
+from saenopy.gui.common.code_export import get_code
+from saenopy.gui.common.ModuleScaleBar import ModuleScaleBar
 
 
 class StackDisplay(PipelineModule):
     view_single = False
     view_single_timer = None
     view_single_switch = 0
 
@@ -349,67 +350,7 @@
                     time_delta1=self.result.time_delta,
                     crop1=self.result.stacks[0].crop,
                     result_file=str(self.result.output),
                 )
 
         code = get_code(code, data)
         return import_code, code
-
-
-class ModuleScaleBar(QtWidgets.QGroupBox):
-    pixtomu = None
-
-    def __init__(self, parent, view):
-        QtWidgets.QWidget.__init__(self)
-        self.parent = parent
-
-        self.font = QtGui.QFont()
-        self.font.setPointSize(16)
-
-        self.scale = 1
-
-        self.scalebar = QtWidgets.QGraphicsRectItem(0, 0, 1, 1, view.hud_lowerRight)
-        self.scalebar.setBrush(QtGui.QBrush(QtGui.QColor("white")))
-        self.scalebar.setPen(QtGui.QPen(QtGui.QColor("white")))
-        self.scalebar.setPos(-20, -20)
-        self.scalebar_text = QtWidgets.QGraphicsTextItem("", view.hud_lowerRight)
-        self.scalebar_text.setFont(self.font)
-        self.scalebar_text.setDefaultTextColor(QtGui.QColor("white"))
-
-        self.time_text = QtWidgets.QGraphicsTextItem("", view.hud_upperRight)
-        self.time_text.setFont(self.font)
-        self.time_text.setDefaultTextColor(QtGui.QColor("white"))
-
-        view.signal_zoom.connect(self.zoomEvent)
-
-        self.updateStatus()
-
-    def updateStatus(self):
-        self.updateBar()
-
-    def zoomEvent(self, scale, pos):
-        self.scale = scale
-        self.updateBar()
-
-    def setScale(self, voxel_size):
-        self.pixtomu = voxel_size[0]
-        self.updateBar()
-
-    def updateBar(self):
-        if self.scale == 0 or self.pixtomu is None:
-            return
-        mu = 100*self.pixtomu/self.scale
-        values = [1, 5, 10, 25, 50, 75, 100, 150, 200, 250, 500, 1000, 1500, 2000, 2500, 5000, 10000]
-        old_v = mu
-        for v in values:
-            if mu < v:
-                mu = old_v
-                break
-            old_v = v
-        if np.abs(self.pixtomu) < 1e-10:
-            pixel = 0
-        else:
-            pixel = mu/(self.pixtomu)*self.scale
-        self.scalebar.setRect(0, 0, -pixel, 5)
-        self.scalebar_text.setPos(-pixel-20-25, -20-30)
-        self.scalebar_text.setTextWidth(pixel+50)
-        self.scalebar_text.setHtml(u"<center>%d&thinsp;µm</center>" % mu)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/VTK_Toolbar.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/VTK_Toolbar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import numpy as np
 import qtawesome as qta
 from qtpy import QtWidgets
 import pyvista as pv
 from pyvistaqt import QtInteractor
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.resources import resource_icon
 
@@ -92,14 +93,18 @@
             self.button_arrow_scale.setIcon(resource_icon("arrowscale.ico"))
 
             self.use_nans = QtShortCuts.QInputBool(None, "", icon=[
                 resource_icon("nan0.ico"),
                 resource_icon("nan1.ico"),
             ], group=False, tooltip="Display nodes which do not have values associated as gray dots.")
 
+            if self.is_force_plot:
+                self.use_log = QtShortCuts.QInputBool(None, "log", tooltip="Display arrow length and color in logarithmic scale.")
+                self.use_log.valueChanged.connect(self.update_display)
+
             self.use_nans.valueChanged.connect(self.update_display)
             self.show_grid = QtShortCuts.QInputBool(None, "", True,
                                                      tooltip="Display a grid or a bounding box.", icon=[
                     resource_icon("grid.ico"),
                     resource_icon("grid2.ico"),
                     resource_icon("grid3.ico"),
                     resource_icon("grid3.ico"),
@@ -226,24 +231,26 @@
             if value != self.arrow_scale.value():
                 self.arrow_scale.setValue(value)
                 self.update_display()
 
     def scale_max_changed(self):
         self.scale_max.setDisabled(self.auto_scale.value())
         scalebar_max = self.getScaleMax()
-        print(scalebar_max, self.plotter.auto_value, type(self.plotter.auto_value))
-        if scalebar_max is None:
-            self.plotter.update_scalar_bar_range([0, self.plotter.auto_value])
-        else:
-            self.plotter.update_scalar_bar_range([0, scalebar_max])
+        if getattr(self.plotter, "auto_value", None) is not None:
+            if scalebar_max is None:
+                self.plotter.update_scalar_bar_range([0, self.plotter.auto_value])
+            else:
+                self.plotter.update_scalar_bar_range([0, scalebar_max])
         self.update_display()
 
     def getScaleMax(self):
         if self.auto_scale.value():
             return None
+        if self.is_force_plot and self.use_log.value():
+            return np.log10(self.scale_max.value())
         return self.scale_max.value()
 
     def new_plotter(self, x, no_recursion=False):
         if self.plotter.theme == x:
             return
         if no_recursion is False:
             for widget in vtk_toolbars:
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/code_export.py` & `saenopy-1.0.4/saenopy/gui/common/code_export.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,74 @@
 import datetime
 import numpy as np
+from saenopy.gui.spheroid.modules.result import ResultSpheroid
 
+class Mesh2D:
+    pass
 
 def get_mesh_arrows(params, result):
-    if params["arrows"] == "piv":
-        if result is not None:
-            mesh = result.mesh_piv[params["time"]["t"]]
-            if mesh is not None and mesh.displacements_measured is not None:
-                return mesh, mesh.displacements_measured, params["deformation_arrows"], "displacements_measured"
-    elif params["arrows"] == "target deformations":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return M.mesh, M.mesh.displacements_target, params["deformation_arrows"], "displacements_target"
-    elif params["arrows"] == "fitted deformations":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return M.mesh, M.mesh.displacements, params["deformation_arrows"], "displacements"
-    elif params["arrows"] == "fitted forces":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return M.mesh, -M.mesh.forces * M.mesh.regularisation_mask[:, None], params["force_arrows"], "forces"
+    data = result.get_data_structure()
+    if params["arrows"] not in data["fields"]:
+        return None, None, {}, ""
+    mesh, field = result.get_field_data(params["arrows"], params["time"]["t"])
+    if data["fields"][params["arrows"]]["measure"] == "deformation":
+        if mesh is not None and field is not None:
+            return mesh, field, params["deformation_arrows"], data["fields"][params["arrows"]]["name"]
+        else:
+            return None, None, params["deformation_arrows"], data["fields"][params["arrows"]]["name"]
+    if data["fields"][params["arrows"]]["measure"] == "force":
+        if mesh is not None and field is not None:
+            return mesh, field, params["force_arrows"], data["fields"][params["arrows"]]["name"]
+        else:
+            return None, None, params["force_arrows"], data["fields"][params["arrows"]]["name"]
     return None, None, {}, ""
 
 
-def get_mesh_extent(params, result):
-    if params["arrows"] == "piv":
-        mesh = result.mesh_piv[params["time"]["t"]]
-        if mesh is not None and mesh.displacements_measured is not None:
-            return [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
-    elif params["arrows"] == "target deformations":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
-    elif params["arrows"] == "fitted deformations":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
-    elif params["arrows"] == "fitted forces":
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
+def get_mesh_extent(params, result): 
+    mesh, field = result.get_field_data(params["arrows"], params["time"]["t"]) 
+    if mesh is None:
+        return None
     else:
-        M = result.solvers[params["time"]["t"]]
-        if M is not None:
-            return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
-        else:
-            M = result.mesh_piv[params["time"]["t"]]
-            if M is not None:
-                return [M.mesh.nodes.min(axis=0) * 1e6, M.mesh.nodes.max(axis=0) * 1e6]
-    return None
+        return [mesh.nodes.min(axis=0) * 1e6, mesh.nodes.max(axis=0) * 1e6]
+  
+
+
 
 
 def getVectorFieldImage(result, params, use_fixed_contrast_if_available=False, use_2D=False, exporter=None):
+    data = result.get_data_structure()
     try:
         image = params["stack"]["image"]
         if use_2D:
             image = 1
-        if image and params["time"]["t"] < len(result.stacks):
-            if params["stack"]["use_reference_stack"] and result.stack_reference:
-                stack = result.stack_reference
-            else:
-                stack = result.stacks[params["time"]["t"]]
-            channel = params["stack"]["channel"]
-            if isinstance(channel, str):
-                try:
-                    channel = result.stacks[0].channels.index(channel)
-                except ValueError:
-                    channel = 0
-            if channel >= len(stack.channels):
-                im = stack[:, :, :, params["stack"]["z"], 0]
-            else:
-                im = stack[:, :, :, params["stack"]["z"], channel]
+        if image and params["time"]["t"] < data["time_point_count"]:
+            stack = result.get_image_data(params["time"]["t"], params["stack"]["channel"], params["stack"]["use_reference_stack"])
             if params["stack"]["z_proj"]:
                 z_range = [0, 5, 10, 1000][params["stack"]["z_proj"]]
-                start = np.clip(params["stack"]["z"] - z_range, 0, stack.shape[2])
-                end = np.clip(params["stack"]["z"] + z_range, 0, stack.shape[2])
-                im = stack[:, :, :, start:end, channel]
+                start = np.clip(params["stack"]["z"] - z_range, 0, stack.shape[3])
+                end = np.clip(params["stack"]["z"] + z_range, 0, stack.shape[3])
+                im = stack[:, :, :, start:end]
                 im = np.max(im, axis=3)
+            else:
+                im = stack[:, :, :, params["stack"]["z"]]
 
             if params["stack"]["use_contrast_enhance"]:
                 if use_fixed_contrast_if_available and params["stack"]["contrast_enhance"]:
                     (min, max) = params["stack"]["contrast_enhance"]
                 else:
                     (min, max) = np.percentile(im, (1, 99))
                     if exporter:
                         exporter.vtk_toolbar.contrast_enhance_values.setValue((min, max))
                 im = im.astype(np.float32) - min
                 im = im.astype(np.float64) * 255 / (max - min)
                 im = np.clip(im, 0, 255).astype(np.uint8)
 
-            display_image = [im, stack.voxel_size, params["stack"]["z"] - stack.shape[2] / 2]
+            display_image = [im, data["voxel_size"], params["stack"]["z"] - data["z_slices_count"] / 2]
             if params["stack"]["image"] == 2:
-                display_image[2] = -stack.shape[2] / 2
+                display_image[2] = -stack.shape[3] / 2
         else:
             display_image = None
     except FileNotFoundError:
         display_image = None
     return display_image
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/Exporter.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/exporter/Exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 import imageio
 import appdirs
 import json
 
 from pathlib import Path
 
 from saenopy import Result
+from saenopy.gui.spheroid.modules.result import ResultSpheroid
 from saenopy.gui.common import QtShortCuts, QExtendedGraphicsView
 from saenopy.gui.common.resources import resource_path
 from saenopy.gui.solver.modules.exporter.FiberViewer import ChannelProperties
 from saenopy.gui.solver.modules.exporter.ExporterRender3D import render_3d
 from saenopy.gui.solver.modules.exporter.ExporterRender2D import render_2d
 
-from saenopy.gui.solver.modules.PipelineModule import PipelineModule
-from saenopy.gui.solver.modules.QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from saenopy.gui.solver.modules.VTK_Toolbar import VTK_Toolbar
 
 
 class Writer:
     writer = None
     def __init__(self, filename, fps=None, qui_parent=None):
         self.filename_base = Path(filename)
@@ -165,20 +166,21 @@
 
         with QtShortCuts.QHBoxLayout(self.export_window):
             with QtShortCuts.QVBoxLayout():
                 with QtShortCuts.QHBoxLayout():
                     QtShortCuts.QPushButton(None, "save parameters", self.save_parameters)
                     QtShortCuts.QPushButton(None, "load parameters", self.load_parameters)
                     QtShortCuts.QPushButton(None, "copy to clipboard parameters", self.copy_parameters)
+                    QtShortCuts.QPushButton(None, "export code", self.generate_code)
 
                 with QtShortCuts.QHBoxLayout():
                     self.input_use2D = QtShortCuts.QInputBool(None, "", False, icon=["3D", "2D"], group=True)
                     self.input_use2D.valueChanged.connect(self.hide2D)
                     self.input_use2D.valueChanged.connect(self.update_display)
-                    QtShortCuts.current_layout.addStretch()
+                    QtShortCuts.currentLayout().addStretch()
 
                 with QtShortCuts.QGroupBox(None, "image dimensions"):
                     with QtShortCuts.QHBoxLayout():
                         self.input_width = QtShortCuts.QInputNumber(None, "width", 1024, float=False)
                         self.input_height = QtShortCuts.QInputNumber(None, "height", 768, float=False)
                         self.input_scale = QtShortCuts.QInputNumber(None, "scale", 1, min=0.1, max=10,
                                                                     use_slider=True, log_slider=True)
@@ -212,15 +214,15 @@
                                                     shared_properties=self.parent.shared_properties)  # .addToLayout()
                     self.z_slider = QTimeSlider("z", self.update_display, "set z position", QtCore.Qt.Vertical).addToLayout()
                 self.t_slider = QTimeSlider(connected=self.update_display).addToLayout()
             self.widget_settings = QtWidgets.QWidget().addToLayout()
             self.widget_settings.setMaximumWidth(700)
             self.widget_settings.setMinimumWidth(700)
             with QtShortCuts.QVBoxLayout(self.widget_settings):
-                QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
                 with QtShortCuts.QGroupBox(None, "camera") as (self.box_camera, _):
                     with QtShortCuts.QHBoxLayout() as layout:
                         self.input_elevation = QtShortCuts.QInputNumber(None, "elevation", 35, min=-90, max=90, use_slider=True, step=10)
                         self.input_azimuth = QtShortCuts.QInputNumber(None, "azimuth", 45, min=-180, max=180, use_slider=True, step=10)
                         self.input_distance = QtShortCuts.QInputNumber(None, "distance", 0, min=0, float=False, step=100)
 
                         self.input_elevation.valueChanged.connect(self.render_view)
@@ -238,24 +240,24 @@
                 with QtShortCuts.QGroupBox(None, "general") as layout:
                     with QtShortCuts.QHBoxLayout() as layout:
                         self.vtk_toolbar.theme.addToLayout()
                         self.vtk_toolbar.show_grid.addToLayout()
                         self.vtk_toolbar.use_nans.addToLayout()
                         self.input_reference_stack = QtShortCuts.QInputBool(None, "show reference stack", False)
                         self.input_reference_stack.valueChanged.connect(self.update_display)
-                        QtShortCuts.current_layout.addStretch()
+                        QtShortCuts.currentLayout().addStretch()
 
                 with QtShortCuts.QHBoxLayout() as layout:
                     self.input_arrows = QtShortCuts.QInputChoice(None, "arrows", "piv", values=["None", "piv", "target deformations", "fitted deformations", "fitted forces"])
                     self.input_arrows.valueChanged.connect(self.update_display)
                     self.input_arrows.valueChanged.connect(self.hide_arrow)
                     self.input_average_range = QtShortCuts.QInputNumber(None, "averaging z thickness", min=0, max=0,
                                                                         step=10)
                     self.input_average_range.valueChanged.connect(self.update_display)
-                    QtShortCuts.current_layout.addStretch()
+                    QtShortCuts.currentLayout().addStretch()
 
                 with QtShortCuts.QHBoxLayout() as layout:
                     with QtShortCuts.QGroupBox(None, "deformation arrows") as (self.box_deformation_arrows, _):
                         with QtShortCuts.QHBoxLayout() as layout:
                             self.vtk_toolbar.auto_scale.addToLayout()
                             self.vtk_toolbar.scale_max.addToLayout()
                             self.input_arrow_opacity = QtShortCuts.QInputNumber(None, "opacity", 1, min=0, max=1, float=True, step=0.1)
@@ -267,14 +269,15 @@
                         self.vtk_toolbar.arrow_scale.addToLayout()
 
                     with QtShortCuts.QGroupBox(None, "force arrows") as (self.box_force_arrows, _):
                         with QtShortCuts.QHBoxLayout() as layout:
                             self.vtk_toolbar2.auto_scale.addToLayout()
                             self.vtk_toolbar2.scale_max.addToLayout()
                             self.vtk_toolbar2.use_center.addToLayout()
+                            self.vtk_toolbar2.use_log.addToLayout()
                             self.input_arrow_opacity2 = QtShortCuts.QInputNumber(None, "opacity", 1, min=0, max=1,
                                                                                 float=True, step=0.1)
                             self.input_arrow_opacity2.valueChanged.connect(self.update_display)
                             self.input_arrow_skip2 = QtShortCuts.QInputNumber(None, "skip", 1, min=1, max=10,
                                                                              float=False)
                             self.input_arrow_skip2.valueChanged.connect(self.update_display)
                         self.vtk_toolbar2.colormap_chooser.addToLayout()
@@ -292,19 +295,19 @@
 
                         QtShortCuts.QVLine().addToLayout()
                         self.channel_selectB = QtShortCuts.QInputChoice(None, "", "", [""], ["       "],
                                                                        tooltip="From which channel to display the stack image.")
                         self.channel_selectB.valueChanged.connect(self.update_display)
                         self.colormap_chooserB = QtShortCuts.QDragableColor("gray").addToLayout()
                         self.colormap_chooserB.valueChanged.connect(self.update_display)
-                        QtShortCuts.current_layout.addStretch()
+                        QtShortCuts.currentLayout().addStretch()
 
                 with QtShortCuts.QGroupBox(None, "scale bar") as (self.box_scalebar, _):
                     with QtShortCuts.QHBoxLayout():
-                        self.input_scalebar_um = QtShortCuts.QInputNumber(None, "length", 0, min=0, max=10000)
+                        self.input_scalebar_um = QtShortCuts.QInputNumber(None, "length", 0, min=0, max=10000, unit="µm")
                         self.input_scalebar_um.valueChanged.connect(self.update_display)
                         self.input_scalebar_width = QtShortCuts.QInputNumber(None, "width", 5, min=0, max=100)
                         self.input_scalebar_width.valueChanged.connect(self.update_display)
                         self.input_scalebar_xpos = QtShortCuts.QInputNumber(None, "xpos", 15, min=0, max=100)
                         self.input_scalebar_xpos.valueChanged.connect(self.update_display)
                         self.input_scalebar_ypos = QtShortCuts.QInputNumber(None, "ypos", 10, min=0, max=100)
                         self.input_scalebar_ypos.valueChanged.connect(self.update_display)
@@ -319,23 +322,23 @@
                         self.input_2darrow_headlength = QtShortCuts.QInputNumber(None, "head length", 5, min=0, max=100)
                         self.input_2darrow_headlength.valueChanged.connect(self.update_display)
                         self.input_2darrow_headwidth = QtShortCuts.QInputNumber(None, "head width", 5, min=0, max=100)
                         self.input_2darrow_headwidth.valueChanged.connect(self.update_display)
 
                 with QtShortCuts.QGroupBox(None, "fiber display") as (self.box_fiberdisplay, _):
                     with QtShortCuts.QVBoxLayout():
-                        QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                        QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
                         self.input_cropx = QtShortCuts.QRangeSlider(None, "crop x", 0, 200)
                         self.input_cropy = QtShortCuts.QRangeSlider(None, "crop y", 0, 200)
                         self.input_cropz = QtShortCuts.QRangeSlider(None, "crop z", 0, 200)
                         self.input_cropx.editingFinished.connect(self.update_display)
                         self.input_cropy.editingFinished.connect(self.update_display)
                         self.input_cropz.editingFinished.connect(self.update_display)
                     with QtShortCuts.QHBoxLayout():
-                        QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+                        QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
                         self.channel0_properties = ChannelProperties().addToLayout()
                         self.channel0_properties.valueChanged.connect(self.update_display)
                         self.channel1_properties = ChannelProperties(True).addToLayout()
                         self.channel1_properties.valueChanged.connect(self.update_display)
                         self.channel0_properties.input_show.setValue(False)
                         self.channel0_properties.checkDisabled()
                         self.channel1_properties.input_show.setValue(False)
@@ -386,15 +389,15 @@
                     with QtShortCuts.QVBoxLayout():
                         self.button_export_zscan = QtShortCuts.QPushButton(None, "export z-scan", self.do_export_zscan)
                         with QtShortCuts.QHBoxLayout():
                             self.zscan_fps = QtShortCuts.QInputNumber(None, "fps", 30)
                             self.zscan_steps = QtShortCuts.QInputNumber(None, "steps", 1, float=False)
                 self.render_progress = QtWidgets.QProgressBar().addToLayout()
                 self.render_progress.setRange(0, 100)
-                QtShortCuts.current_layout.addStretch()
+                QtShortCuts.currentLayout().addStretch()
 
         self.parameter_map = {
             "image": {
                 "width": self.input_width,
                 "height": self.input_height,
                 "logo_size": self.input_logosize,
                 "scale": self.input_scale,
@@ -426,14 +429,15 @@
                 "skip": self.input_arrow_skip,
             },
 
             "force_arrows": {
                 "autoscale": self.vtk_toolbar2.auto_scale,
                 "scale_max": self.vtk_toolbar2.scale_max,
                 "use_center": self.vtk_toolbar2.use_center,
+                "use_log": self.vtk_toolbar2.use_log,
                 "colormap": self.vtk_toolbar2.colormap_chooser,
                 "arrow_scale": self.vtk_toolbar2.arrow_scale,
                 "arrow_opacity": self.input_arrow_opacity2,
                 "skip": self.input_arrow_skip2,
             },
 
             "stack": {
@@ -524,36 +528,44 @@
 
         self.box_fiberdisplay.setVisible(is3D)
 
         self.button_export_rotate.setEnabled(is3D)
         self.rotate_fps.setEnabled(is3D)
         self.rotate_steps.setEnabled(is3D)
 
+        if is2D:
+            self.pixmap1.sceneEvent = None
+        else:
+            self.pixmap1.sceneEvent = self.sceneEventFilter
+
     def hide_timestamp(self):
-        isTimeAvailable = self.result is not None and self.result.time_delta is not None
+        data = self.result.get_data_structure() if self.result is not None else None
+        isTimeAvailable = data and data["time_delta"] is not None
         self.time_check.setEnabled(isTimeAvailable)
         self.button_export_time.setEnabled(isTimeAvailable)
         self.time_fps.setEnabled(isTimeAvailable)
         self.time_steps.setEnabled(isTimeAvailable)
-        isTime = self.time_check.value() and self.result is not None and self.result.time_delta is not None
+        isTime = self.time_check.value() and self.result is not None and data["time_delta"] is not None
         self.time_format.setEnabled(isTime)
         self.time_start.setEnabled(isTime)
         self.time_size.setEnabled(isTime)
 
     def hide_fiber(self):
         isActive = self.channel0_properties.input_show.value() or self.channel1_properties.input_show.value()
         self.input_cropx.setEnabled(isActive)
         self.input_cropy.setEnabled(isActive)
         self.input_cropz.setEnabled(isActive)
         isActiveBoth = self.channel0_properties.input_show.value() and self.channel1_properties.input_show.value()
         self.input_thresh.setEnabled(isActiveBoth)
 
     def hide_arrow(self):
-        isDeformation = self.input_arrows.value() in ["piv", "target deformations", "fitted deformations"]
-        isForce = self.input_arrows.value() in ["fitted forces"]
+        data = self.result.get_data_structure() if self.result is not None else {}
+        measure = data.get("fields", {}).get(self.input_arrows.value(), {}).get("measure", "")
+        isDeformation = measure == "deformation"
+        isForce = measure == "force"
 
         self.box_deformation_arrows.setEnabled(isDeformation)
         self.box_force_arrows.setEnabled(isForce)
 
     def hide_stack_image(self):
         isActive = self.vtk_toolbar.show_image.value() != 0 or self.input_use2D.value()
         self.vtk_toolbar.channel_select.setEnabled(isActive)
@@ -583,14 +595,35 @@
                 self.update_display()
 
     def copy_parameters(self):
         text = repr(self.get_parameters())
         cb = QtGui.QGuiApplication.clipboard()
         cb.setText(text, mode=cb.Clipboard)
 
+    def generate_code(self):
+        if self.result is None:
+            return
+        new_path = QtWidgets.QFileDialog.getSaveFileName(None, "Save Session as Script", os.getcwd(), "Python File (*.py)")
+        if new_path:
+            # ensure filename ends in .py
+            if not new_path.endswith(".py"):
+                new_path += ".py"
+
+            run_code = f"""import matplotlib.pyplot as plt
+import saenopy
+
+params = {json.dumps(self.get_parameters(), indent=2).replace("true", "True").replace("false", "False").replace("null", "None")}
+
+im = saenopy.render_image(params, saenopy.load("{self.result.output}"))
+plt.imsave("output.png", im)
+"""
+            #print(run_code)
+            with open(new_path, "w") as fp:
+                fp.write(run_code)
+
     def progress_iterator(self, iter):
         self.render_progress.setRange(0, len(iter))
         self.render_progress.setValue(0)
         for i, value in enumerate(iter):
             yield value
             self.render_progress.setValue(i+1)
 
@@ -627,63 +660,91 @@
         with Writer(self.outputText3.value(), self.zscan_fps.value(), self) as writer:
             for t in self.progress_iterator(range(0, self.z_slider.t_slider.maximum() + 1, self.zscan_steps.value())):
                 self.z_slider.setValue(t)
                 self.update_display()
                 writer.write(self.im)
 
     def check_evaluated(self, result: Result) -> bool:
-        return self.result is not None and result.stacks is not None and len(result.stacks) > 0
+        if result is None:
+            return False
+        return True
 
     def setResult(self, result: Result, no_update_display=False):
         self.result = result
-        if result and result.stacks and result.stacks[0]:
-            self.z_slider.setRange(0, result.stacks[0].shape[2] - 1)
-            self.z_slider.setValue(result.stacks[0].shape[2] // 2)
+        if result:
+            data = result.get_data_structure()
+            self.input_arrows.setValues(["None"] + list(data["fields"].keys()))
+            self.input_arrows.setValue(next(iter(data["fields"].items()))[0])
+
+            #if len(data["channels"]) == 1:
+            #    self.channel_selectB.setVisible(False)
+            #    self.colormap_chooserB.setVisible(False)
+            #else:
+            #    self.channel_selectB.setVisible(True)
+            #    self.colormap_chooserB.setVisible(True)
+
+            if data["dimensions"] == 2:
+                self.input_use2D.setValue(True)
+                self.input_use2D.setVisible(False)
+                self.hide2D()
+                self.z_slider.setVisible(False)
+                self.input_average_range.setVisible(False)
+                self.vtk_toolbar.button_z_proj.setVisible(False)
+
+                self.button_export_zscan.setEnabled(False)
+                self.zscan_fps.setEnabled(False)
+                self.zscan_steps.setEnabled(False)
+            else:
+                self.z_slider.setRange(0, data["z_slices_count"] - 1)
+                self.z_slider.setValue( data["z_slices_count"] // 2)
 
-            if result.stacks[0].channels:
+            if len(data["channels"]) > 1:
                 value = self.vtk_toolbar.channel_select.value()
-                self.vtk_toolbar.channel_select.setValues(np.arange(len(result.stacks[0].channels)), result.stacks[0].channels)
+                self.vtk_toolbar.channel_select.setValues(np.arange(len(data["channels"])), data["channels"])
                 self.vtk_toolbar.channel_select.setValue(value)
                 self.vtk_toolbar.channel_select.setVisible(True)
 
                 value = self.channel_selectB.value()
-                self.channel_selectB.setValues([-1] + list(np.arange(len(result.stacks[0].channels))),
-                                               [""] + result.stacks[0].channels)
+                self.channel_selectB.setValues([-1] + list(np.arange(len(data["channels"]))),
+                                               [""] + data["channels"])
                 self.channel_selectB.setValue("")
                 self.channel_selectB.setVisible(True)
+                self.colormap_chooserB.setVisible(True)
 
                 value = self.channel1_properties.channel_select.value()
-                self.channel1_properties.channel_select.setValues(np.arange(len(result.stacks[0].channels))[1:],
-                                                                  result.stacks[0].channels[1:])
+                self.channel1_properties.channel_select.setValues(np.arange(len(data["channels"]))[1:],
+                                                                  data["channels"])
                 self.channel1_properties.channel_select.setValue(value)
                 self.channel1_properties.channel_select.setVisible(True)
             else:
                 self.vtk_toolbar.channel_select.setValue(0)
                 self.vtk_toolbar.channel_select.setVisible(False)
                 self.channel_selectB.setVisible(False)
+                self.colormap_chooserB.setVisible(False)
 
-            shape = result.stacks[0].shape
+            shape = data["im_shape"]
             self.input_cropx.setRange(0, shape[1])
             self.input_cropx.setValue((shape[1] // 2 - 100, shape[1] // 2 + 100))
             self.input_cropy.setRange(0, shape[0])
             self.input_cropy.setValue((shape[0] // 2 - 100, shape[0] // 2 + 100))
             self.input_cropz.setRange(0, shape[2])
             self.input_cropz.setValue((shape[2] // 2 - 25, shape[2] // 2 + 25))
 
-            if result.stacks[0].shape[-1] == 1:
+            if data["channels"] == 1:
                 self.channel1_properties.input_show.setValue(False)
                 self.channel1_properties.setDisabled(True)
             else:
                 self.channel1_properties.setDisabled(False)
 
-            self.input_average_range.setRange(0, shape[2] * result.stacks[0].voxel_size[2])
+            self.input_average_range.setRange(0, shape[2] * data["voxel_size"][2])
             self.input_average_range.setValue(10)
 
         super().setResult(result)
         self.hide_timestamp()
+        self.hide_arrow()
         if not no_update_display:
             self.update_display()
 
     def get_parameters(self):
         def get_params(parameter_map):
             params = {}
             for name, widget in parameter_map.items():
@@ -942,14 +1003,15 @@
             return True
         return False
 
 app = None
 exporter = None
 def render_image(params, result):
     global app, exporter
+    app = QtWidgets.QApplication.instance()
     if app is None:
         app = QtWidgets.QApplication([])
     if exporter is None:
         exporter = ExportViewer(None, None)
     exporter.set_parameters(params)
     exporter.setResult(result, no_update_display=True)
     exporter.set_parameters(params)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender2D.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExporterRender2D.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 
 def render_2d(params, result, exporter=None):
     pil_image, display_image, im_scale, aa_scale = render_2d_image(params, result, exporter)
     if pil_image is None:
         return np.zeros((10, 10))
 
-    pil_image = render_2d_arrows(params, result, pil_image, im_scale, aa_scale, display_image)
+    pil_image, disp_params = render_2d_arrows(params, result, pil_image, im_scale, aa_scale, display_image, return_scale=True)
 
     if aa_scale == 2:
         pil_image = pil_image.resize([pil_image.width // 2, pil_image.height // 2])
         aa_scale = 1
 
     pil_image = render_2d_scalebar(params, result, pil_image, im_scale, aa_scale)
+    if disp_params != None:
+        pil_image = render_2d_colorbar(params, result, pil_image, im_scale, aa_scale, scale_max=disp_params["scale_max"], colormap=disp_params["colormap"])
 
     pil_image = render_2d_time(params, result, pil_image)
 
     pil_image = render_2d_logo(params, result, pil_image, aa_scale)
 
     return np.asarray(pil_image)
 
@@ -57,102 +59,146 @@
 
     pil_image = Image.fromarray(im).convert("RGB")
     pil_image = pil_image.resize([int(pil_image.width * im_scale * aa_scale), int(pil_image.height * im_scale * aa_scale)])
 
     return pil_image, display_image, im_scale, aa_scale
 
 
-def render_2d_arrows(params, result, pil_image, im_scale, aa_scale, display_image):
+def render_2d_arrows(params, result, pil_image, im_scale, aa_scale, display_image, return_scale=False):
     def project_data(R, field, skip=1):
         length = np.linalg.norm(field, axis=1)
         angle = np.arctan2(field[:, 1], field[:, 0])
         data = pd.DataFrame(np.hstack((R, length[:, None], angle[:, None])),
                             columns=["x", "y", "length", "angle"])
         data = data.sort_values(by="length", ascending=False)
         d2 = data.groupby(["x", "y"]).first()
         # optional slice
         if skip > 1:
             d2 = d2.loc[(slice(None, None, skip), slice(None, None, skip)), :]
         return np.array([i for i in d2.index]), d2[["length", "angle"]]
 
     mesh, field, params_arrows, name = get_mesh_arrows(params, result)
 
+    if params_arrows is None:
+        scale_max = None
+    else:
+        scale_max = params_arrows["scale_max"] if not params_arrows["autoscale"] else None
+        colormap = params_arrows["colormap"]
+        skip = params_arrows["skip"]
+        alpha = params_arrows["arrow_opacity"]
+
     if mesh is None:
+        if return_scale:
+            if scale_max is None:
+                return pil_image, None
+            else:
+                return pil_image, {"scale_max": scale_max, "colormap": colormap}
+            return pil_image, None
         return pil_image
 
-    scale_max = params_arrows["scale_max"] if params_arrows["autoscale"] else None
-    colormap = params_arrows["colormap"]
-    skip = params_arrows["skip"]
-    alpha = params_arrows["arrow_opacity"]
-
     if field is not None:
         # rescale and offset
         scale = 1e6 / display_image[1][0]
         offset = np.array(display_image[0].shape[0:2]) / 2
 
         R = mesh.nodes.copy()
+        is3D = R.shape[1] == 3
         field = field.copy()
-        R = R[:, :2][:, ::-1] * scale + offset
-        field = field[:, :2][:, ::-1] * scale * params_arrows["arrow_scale"]
-        if name == "forces":
-            field *= 1e4
+        if getattr(mesh, "units", None) == "pixels":
+            R = R[:, :2]
+            R[:, 1] = display_image[0].shape[0] - R[:, 1]
+            field = field[:, :2] * params_arrows["arrow_scale"]
+            field[:, 1] = -field[:, 1]
+        else:  # "microns" + 3D
+            R = R[:, :2][:, ::-1] * scale + offset
+            field = field[:, :2][:, ::-1] * scale * params_arrows["arrow_scale"]
+
+            if name == "forces":
+                field *= 1e4
 
         if scale_max is None:
             max_length = np.nanmax(np.linalg.norm(field, axis=1))# * params_arrows["arrow_scale"]
+            scale_max = max_length / params_arrows["arrow_scale"]
         else:
             max_length = scale_max * params_arrows["arrow_scale"]
 
-        z_center = (params["averaging_size"] - result.stacks[0].shape[2] / 2) * display_image[1][2] * 1e-6
-        z_min = z_center - params["averaging_size"] * 1e-6
-        z_max = z_center + params["averaging_size"] * 1e-6
-
-        index = (z_min < mesh.nodes[:, 2]) & (mesh.nodes[:, 2] < z_max)
-
-        R = R[index]
-        field = field[index]
-        R, field = project_data(R, field, skip=skip)
+        if is3D:
+            z_center = (params["averaging_size"] - result.stacks[0].shape[2] / 2) * display_image[1][2] * 1e-6
+            z_min = z_center - params["averaging_size"] * 1e-6
+            z_max = z_center + params["averaging_size"] * 1e-6
+
+            index = (z_min < mesh.nodes[:, 2]) & (mesh.nodes[:, 2] < z_max)
+
+            R = R[index]
+            field = field[index]
+            R, field = project_data(R, field, skip=skip)
+        else:
+            length = np.linalg.norm(field, axis=1)
+            angle = np.arctan2(field[:, 1], field[:, 0])
+            field = pd.DataFrame(np.hstack((length[:, None], angle[:, None])), columns=["length", "angle"])
         pil_image = add_quiver(pil_image, R, field.length, field.angle, max_length=max_length, cmap=colormap,
                                alpha=alpha,
                                scale=im_scale * aa_scale,
                                width=params["2D_arrows"]["width"],
                                headlength=params["2D_arrows"]["headlength"],
                                headheight=params["2D_arrows"]["headheight"])
+    if return_scale:
+        return pil_image, {"scale_max": scale_max, "colormap": colormap}
     return pil_image
 
 
 def render_2d_scalebar(params, result, pil_image, im_scale, aa_scale):
+    data = result.get_data_structure()
+
     def getBarParameters(pixtomu, scale=1):
         mu = 200 * pixtomu / scale
         values = [1, 5, 10, 25, 50, 75, 100, 150, 200, 250, 500, 1000, 1500, 2000, 2500, 5000, 10000]
         old_v = mu
         for v in values:
             if mu < v:
                 mu = old_v
                 break
             old_v = v
         pixel = mu / pixtomu * scale
         return pixel, mu
 
     if params["scalebar"]["length"] == 0:
-        pixel, mu = getBarParameters(result.stacks[0].voxel_size[0])
+        pixel, mu = getBarParameters(data["voxel_size"][0])
     else:
         mu = params["scalebar"]["length"]
-        pixel = mu / result.stacks[0].voxel_size[0]
+        pixel = mu / data["voxel_size"][0]
 
     pil_image = add_scalebar(pil_image, scale=1, image_scale=im_scale * aa_scale,
                              width=params["scalebar"]["width"] * aa_scale,
                              xpos=params["scalebar"]["xpos"] * aa_scale,
                              ypos=params["scalebar"]["ypos"] * aa_scale,
                              fontsize=params["scalebar"]["fontsize"] * aa_scale, pixel_width=pixel,
                              size_in_um=mu, color="w", unit="µm")
     return pil_image
 
+def render_2d_colorbar(params, result, pil_image, im_scale, aa_scale, colormap="viridis", scale_max=1):
+    pil_image = add_colorbar(pil_image, scale=1,
+                             colormap=colormap,#params["colorbar"]["colorbar"],
+                             #bar_width=params["colorbar"]["bar_width"] * aa_scale,
+                             #bar_height=params["colorbar"]["bar_height"] * aa_scale,
+                             #tick_height=params["colorbar"]["tick_height"] * aa_scale,
+                             #tick_count=params["colorbar"]["tick_count"],
+                             #min_v=params["scalebar"]["min_v"],
+                             max_v=scale_max,#params["colorbar"]["max_v"],
+                             #offset_x=params["colorbar"]["offset_x"] * aa_scale,
+                             #offset_y=params["colorbar"]["offset_y"] * aa_scale,
+                             #fontsize=params["colorbar"]["fontsize"] * aa_scale,
+                             )
+
+    return pil_image
+
 
 def render_2d_time(params, result, pil_image):
-    if result is not None and result.time_delta is not None and params["time"]["display"]:
+    data = result.get_data_structure()
+    if result is not None and data["time_delta"] is not None and params["time"]["display"]:
         pil_image = add_text(pil_image, get_time_text(params, result), position=(10, 10))
     return pil_image
 
 
 def render_2d_logo(params, result, pil_image, aa_scale):
     if params["image"]["logo_size"] >= 10:
         if params["theme"] == "dark":
@@ -206,28 +252,85 @@
     image = ImageDraw.ImageDraw(pil_image)
     font_size = int(round(fontsize * 4 / 3))  # the 4/3 appears to be a factor of "converting" screel dpi to image dpi
     try:
         font = ImageFont.truetype("arial", font_size)  # ImageFont.truetype("tahoma.ttf", font_size)
     except IOError:
         font = ImageFont.truetype("times", font_size)
 
-    length_number = image.textsize(text, font=font)
+    length_number = image.textlength(text, font=font)
     x, y = position
 
     if x < 0:
         x = pil_image.width + x - length_number[0]
     if y < 0:
         y = pil_image.height + y - length_number[1]
     color = tuple((matplotlib.colors.to_rgba_array("w")[0, :3] * 255).astype("uint8"))
     if pil_image.mode != "RGB":
         color = int(np.mean(color))
 
     image.text((x, y), text, color, font=font)
     return pil_image
 
+def add_colorbar(pil_image,
+                 colormap="viridis",
+                 bar_width=150,
+                 bar_height=10,
+                 tick_height=5,
+                 tick_count=3,
+                 min_v=0,
+                 max_v=10,
+                 offset_x=15,
+                 offset_y=-10,
+                 scale=1, fontsize=16, color="w"):
+    cmap = plt.get_cmap(colormap)
+    if offset_x < 0:
+        offset_x = pil_image.size[0] + offset_x
+    if offset_y < 0:
+        offset_y = pil_image.size[1] + offset_y
+
+    color = tuple((matplotlib.colors.to_rgba_array(color)[0, :3] * 255).astype("uint8"))
+    if pil_image.mode != "RGB":
+        color = int(np.mean(color))
+
+    colors = np.zeros((bar_height, bar_width, 3), dtype=np.uint8)
+    for i in range(bar_width):
+        c = plt.get_cmap(cmap)(int(i / bar_width * 255))
+        colors[:, i, :] = [c[0] * 255, c[1] * 255, c[2] * 255]
+    pil_image.paste(Image.fromarray(colors), (offset_x, offset_y - bar_height))
+
+    image = ImageDraw.ImageDraw(pil_image)
+    import matplotlib.ticker as ticker
+
+    font_size = int(
+        round(fontsize * scale * 4 / 3))  # the 4/3 appears to be a factor of "converting" screel dpi to image dpi
+    try:
+        font = ImageFont.truetype("arial", font_size)  # ImageFont.truetype("tahoma.ttf", font_size)
+    except IOError:
+        font = ImageFont.truetype("times", font_size)
+
+    locator = ticker.MaxNLocator(nbins=tick_count - 1)
+    #tick_positions = locator.tick_values(min_v, max_v)
+    tick_positions = np.linspace(min_v, max_v, tick_count)
+    for i, pos in enumerate(tick_positions):
+        x0 = offset_x + (bar_width - 2) / (tick_count - 1) * i
+        y0 = offset_y - bar_height - 1
+
+        image.rectangle([x0, y0-5, x0+1, y0])
+
+        text = "%d" % pos
+        length_number = image.textlength(text, font=font)
+        height_number = image.textbbox((0, 0), text, font=font)[3]
+
+        x = x0 - length_number * 0.5 + 1
+        y = y0 - height_number - tick_height - 3
+        # draw the text for the number and the unit
+        image.text((x, y), text, color, font=font)
+    #image.rectangle([pil_image.size[0]-10, 0, pil_image.size[0], 10], fill="w")
+    return pil_image
+
 def add_scalebar(pil_image, scale, image_scale, width, xpos, ypos, fontsize, pixel_width, size_in_um, color="w", unit="µm"):
     image = ImageDraw.ImageDraw(pil_image)
     pixel_height = width
     pixel_offset_x = xpos
     pixel_offset_y = ypos
     pixel_offset2 = 3
     font_size = int(round(fontsize*scale*4/3))  # the 4/3 appears to be a factor of "converting" screel dpi to image dpi
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender3D.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/exporter/ExporterRender3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
     crops = []
     for value in [params["crop"]["y"], params["crop"]["x"], params["crop"]["z"]]:
         crops.extend(value)
 
     t = params["time"]["t"]
     t_start = time.time()
     stack_data = None
+    if len(result.stacks) == 0:
+        return
     stack = result.stacks[t]
 
     if params["stack"]["use_reference_stack"]:
         stack = result.stack_reference
 
     if params["channel0"]["show"] and crops[0] != crops[1] and crops[2] != crops[3] and crops[4] != \
             crops[5]:
@@ -137,15 +139,15 @@
 
 def render_3d_arrows(params, result, plotter):
     used_values = [
         "use_nans",
         "arrows",
         ("time", "t"),
         ("deformation_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale")),
-        ("force_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale", "use_center")),
+        ("force_arrows", ("scale_max", "autoscale", "skip", "arrow_opacity", "colormap", "arrow_scale", "use_center", "use_log")),
     ]
     params, changed = filter_params(params, used_values, getattr(plotter, "previous_plot_params", {}))
 
     if not changed and result == getattr(plotter, "previous_plot_result", {}):
         return
 
     obj, field, params_arrows, name = get_mesh_arrows(params, result)
@@ -153,15 +155,15 @@
     if obj is None:
         plotter.remove_actor("arrows")
         plotter.remove_actor("nans")
         plotter.remove_actor("center")
         return
 
     show_nan = params["use_nans"]
-    scalebar_max = params_arrows["scale_max"] if params_arrows["autoscale"] else None
+    scalebar_max = params_arrows["scale_max"] if not params_arrows["autoscale"] else None
     colormap = params_arrows["colormap"]
     skip = params_arrows["skip"]
     arrow_opacity = params_arrows["arrow_opacity"]
 
     if field is not None:
         obj_R = obj.nodes * 1e6
 
@@ -182,15 +184,22 @@
         # convert to common units
         if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
             # scale deformations to µN
             point_cloud.point_data[name + "_mag2"] = 1e6*point_cloud.point_data[name + "_mag"].copy()
             factor = 0.1 * params_arrows["arrow_scale"]
         if name == "forces":
             # scale forces to pN
-            point_cloud.point_data[name + "_mag2"] = 1e12*point_cloud.point_data[name + "_mag"].copy()
+            if params_arrows["use_log"]:
+                if scalebar_max is not None:
+                    scalebar_max = np.log10(scalebar_max)
+                point_cloud.point_data[name + "_mag2"] = np.log10(1e12 * point_cloud.point_data[name + "_mag"].copy())
+                point_cloud.point_data[name + "_mag2"] *= (
+                        point_cloud.point_data[name + "_mag2"] > point_cloud.point_data[name + "_mag2"] * 0.1)
+            else:
+                point_cloud.point_data[name + "_mag2"] = 1e12*point_cloud.point_data[name + "_mag"].copy()
             factor = 0.15 * params_arrows["arrow_scale"]
         # hide nans
         point_cloud.point_data[name + "_mag2"][nan_values] = 0
 
         # scalebar scaling factor
         norm_stack_size = np.abs(np.max(obj_R) - np.min(obj_R))
         if scalebar_max is None:
@@ -231,15 +240,15 @@
         else:
             plotter.update_scalar_bar_range([0, scalebar_max])
     else:
         plotter.remove_actor("arrows")
 
     # plot center points if desired
     if params_arrows.get("use_center", False):
-        center = obj.get_center(mode="Force")
+        center = result.solvers[params["time"]["t"]].get_center(mode="Force")
         plotter.add_points(np.array([center])*1e6, color='m', point_size=10, render=False, name="center")
     else:
         plotter.remove_actor("center")
 
 
 def render_3d_image(params, result, plotter, exporter=None):
     used_values = [
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/FiberViewer.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/exporter/FiberViewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from matplotlib.colors import ListedColormap
 import matplotlib
 import time
 
 from saenopy.gui.common import QtShortCuts
 from saenopy import Result
 
-from saenopy.gui.solver.modules.PipelineModule import PipelineModule
-from saenopy.gui.solver.modules.QTimeSlider import QTimeSlider
+from saenopy.gui.common.PipelineModule import PipelineModule
+from saenopy.gui.common.QTimeSlider import QTimeSlider
 from saenopy.gui.solver.modules.VTK_Toolbar import VTK_Toolbar
 from saenopy.gui.solver.modules.DeformationDetector import CamPos
 from saenopy.gui.common.sigmoid_widget import SigmoidWidget
 
 
 caches = {}
 class Cache:
@@ -184,15 +184,15 @@
 
 class ChannelProperties(QtWidgets.QWidget):
     valueChanged = QtCore.Signal()
     def __init__(self, use_channel=False):
         super().__init__()
         self.setMaximumHeight(100)
         with QtShortCuts.QHBoxLayout(self) as layout:
-            QtShortCuts.current_layout.setContentsMargins(0, 0, 0, 0)
+            QtShortCuts.currentLayout().setContentsMargins(0, 0, 0, 0)
             with QtShortCuts.QVBoxLayout() as layout:
                 with QtShortCuts.QHBoxLayout() as layout:
                     self.input_show = QtShortCuts.QInputBool(None, "show", True)
                     self.input_show.valueChanged.connect(self.checkDisabled)
                     self.input_skip = QtShortCuts.QInputNumber(None, "skip", 1, min=1, max=10, float=False)
                     self.use_channel = use_channel
                     if use_channel:
@@ -206,15 +206,15 @@
                     #self.input_percentile1 = QtShortCuts.QInputNumber(None, "percentile_min", 0.01)
                     #self.input_percentile2 = QtShortCuts.QInputNumber(None, "percentile_max", 99.6)
                 with QtShortCuts.QHBoxLayout() as layout:
                     #self.input_alpha1 = QtShortCuts.QInputNumber(None, "alpha1", 0.065, min=0, max=0.3, step=0.01, decimals=3)
                     #self.input_alpha2 = QtShortCuts.QInputNumber(None, "alpha2", 0.2491, min=0, max=1, step=0.01)
                     #self.input_alpha3 = QtShortCuts.QInputNumber(None, "alpha3", 1, min=0, max=1, step=0.1)
                     self.input_cmap = QtShortCuts.QDragableColor("pink").addToLayout()
-                QtShortCuts.current_layout.addStretch()
+                QtShortCuts.currentLayout().addStretch()
 
             self.sigmoid = SigmoidWidget().addToLayout()
             self.input_cmap.valueChanged.connect(lambda x: self.sigmoid.p.set_cmap(x))
             #self.sigmoid.valueChanged.connect(lambda x1, x2, x3, *args: (self.input_alpha1.setValue(x1), self.input_alpha2.setValue(x2), self.input_alpha3.setValue(x3)))
         for widget in [self.input_sato, self.input_gauss, #self.input_percentile1, self.input_percentile2,
                        #self.input_alpha1, self.input_alpha2, self.input_alpha3,
                        self.input_cmap, self.input_show, self.input_skip]:
```

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/path_editor.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/path_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/gui/solver/modules/showVectorField.py` & `saenopy-1.0.4/saenopy/gui/solver/modules/showVectorField.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                     colormap=self.vtk_toolbar.colormap_chooser.value(),
                     colormap2=self.vtk_toolbar.colormap_chooser2.value(),
                     stack_shape=stack_shape)
 
 
 def showVectorField(plotter: QtInteractor, obj: Solver, field: np.ndarray, name: str, center=None, show_nan=True, stack_shape=None,
                     show_all_points=False, factor=.1, scalebar_max=None, display_image=None, show_grid=True,
-                    colormap="turbo", colormap2=None, stack_min_max=None, arrow_opacity=1, skip=1):
+                    colormap="turbo", colormap2=None, stack_min_max=None, arrow_opacity=1, skip=1, log_scale=False):
     # ensure that the image is either with color channels or no channels
     if (display_image is not None) and (display_image[0].shape[2] == 1):
         display_image[0] = display_image[0][:, :, 0]
 
     # force rendering to be disabled while updating content to prevent flickering
     render = plotter.render
     plotter.render = lambda *args: None
@@ -106,15 +106,19 @@
             point_cloud.point_data[name + "_mag"] = np.linalg.norm(field, axis=1)
             # convert to common units
             if name == "displacements_measured" or name == "displacements_target" or name == "displacements":
                   # scale deformations to µN
                   point_cloud.point_data[name + "_mag2"] = 1e6*point_cloud.point_data[name + "_mag"].copy()
             if name == "forces":
                   # scale forces to pN
-                  point_cloud.point_data[name + "_mag2"] = 1e12*point_cloud.point_data[name + "_mag"].copy()
+                  if log_scale:
+                      point_cloud.point_data[name + "_mag2"] = np.log10(1e12*point_cloud.point_data[name + "_mag"].copy())
+                      point_cloud.point_data[name + "_mag2"] *= (point_cloud.point_data[name + "_mag2"] > point_cloud.point_data[name + "_mag2"]*0.1)
+                  else:
+                      point_cloud.point_data[name + "_mag2"] = 1e12 * point_cloud.point_data[name + "_mag"].copy()
             # hide nans
             point_cloud.point_data[name + "_mag2"][nan_values] = 0
             # show nans
             if not show_all_points and show_nan:
                 R = obj_R[nan_values]
                 if R.shape[0]:
                     point_cloud2 = pv.PolyData(R)
```

### Comparing `saenopy-1.0.2/saenopy/img/Icon.ico` & `saenopy-1.0.4/saenopy/img/Icon.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/Logo.png` & `saenopy-1.0.4/saenopy/img/Logo.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/Logo.svg` & `saenopy-1.0.4/saenopy/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/Logo_black.png` & `saenopy-1.0.4/saenopy/img/Logo_black.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame00.png` & `saenopy-1.0.4/saenopy/img/animation/frame00.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame01.png` & `saenopy-1.0.4/saenopy/img/animation/frame01.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame02.png` & `saenopy-1.0.4/saenopy/img/animation/frame02.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame03.png` & `saenopy-1.0.4/saenopy/img/animation/frame03.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame04.png` & `saenopy-1.0.4/saenopy/img/animation/frame04.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame05.png` & `saenopy-1.0.4/saenopy/img/animation/frame05.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame06.png` & `saenopy-1.0.4/saenopy/img/animation/frame06.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame07.png` & `saenopy-1.0.4/saenopy/img/animation/frame07.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame08.png` & `saenopy-1.0.4/saenopy/img/animation/frame08.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame09.png` & `saenopy-1.0.4/saenopy/img/animation/frame09.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame10.png` & `saenopy-1.0.4/saenopy/img/animation/frame10.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame11.png` & `saenopy-1.0.4/saenopy/img/animation/frame11.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame12.png` & `saenopy-1.0.4/saenopy/img/animation/frame12.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/animation/frame13.png` & `saenopy-1.0.4/saenopy/img/animation/frame13.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/arrowscale.ico` & `saenopy-1.0.4/saenopy/img/arrowscale.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/autoscale0.ico` & `saenopy-1.0.4/saenopy/img/autoscale0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/autoscale1.ico` & `saenopy-1.0.4/saenopy/img/autoscale1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/buttons.svg` & `saenopy-1.0.4/saenopy/img/buttons.svg`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/center0.ico` & `saenopy-1.0.4/saenopy/img/center0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/center1.ico` & `saenopy-1.0.4/saenopy/img/center1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/contrast0.ico` & `saenopy-1.0.4/saenopy/img/contrast0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/contrast1.ico` & `saenopy-1.0.4/saenopy/img/contrast1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/grid.ico` & `saenopy-1.0.4/saenopy/img/grid.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/grid2.ico` & `saenopy-1.0.4/saenopy/img/grid2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/grid3.ico` & `saenopy-1.0.4/saenopy/img/grid3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/logo_splash.png` & `saenopy-1.0.4/saenopy/img/logo_splash.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/nan0.ico` & `saenopy-1.0.4/saenopy/img/nan0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/nan1.ico` & `saenopy-1.0.4/saenopy/img/nan1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/show_image.ico` & `saenopy-1.0.4/saenopy/img/show_image.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/show_image2.ico` & `saenopy-1.0.4/saenopy/img/show_image2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/show_image3.ico` & `saenopy-1.0.4/saenopy/img/show_image3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/slice0.ico` & `saenopy-1.0.4/saenopy/img/slice0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/slice1.ico` & `saenopy-1.0.4/saenopy/img/slice1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/slice2.ico` & `saenopy-1.0.4/saenopy/img/slice2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/slice_all.ico` & `saenopy-1.0.4/saenopy/img/slice_all.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/BFTFM.png` & `saenopy-1.0.4/saenopy/img/thumbnails/BFTFM.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/BFTFM_2.png` & `saenopy-1.0.4/saenopy/img/thumbnails/BFTFM_2.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/Bead_example_icon.png` & `saenopy-1.0.4/saenopy/img/thumbnails/Bead_example_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/Dynamic_icon.png` & `saenopy-1.0.4/saenopy/img/thumbnails/Dynamic_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/StainedOrganoid_icon.png` & `saenopy-1.0.4/saenopy/img/thumbnails/StainedOrganoid_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/thumbnails/liver_fibroblast_icon.png` & `saenopy-1.0.4/saenopy/img/thumbnails/liver_fibroblast_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/view_single.ico` & `saenopy-1.0.4/saenopy/img/view_single.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/img/view_two.ico` & `saenopy-1.0.4/saenopy/img/view_two.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/macro.py` & `saenopy-1.0.4/saenopy/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/materials.py` & `saenopy-1.0.4/saenopy/materials.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,14 +104,20 @@
     k: float = None
     d_0: float = None
     lambda_s: float = None
     d_s: float = None
 
     def __init__(self, k, d_0=None, lambda_s=None, d_s=None):
         super().__init__()
+        if d_0 == "None":
+            d_0 = None
+        if lambda_s == "None":
+            lambda_s = None
+        if d_s == "None":
+            d_s = None
         # parameters
         self.k = k
         self.d_0 = d_0 if d_0 is not None and d_0 >= 0 else None
         # buckling None (constant stiffness) and buckling zero (drop in stiffness) is not the same 
         if self.d_0 is not None and self.d_0 < 1e-30:  # approximate the zero case
             self.d_0 = 1e-30
         self.lambda_s = lambda_s if lambda_s is not None and lambda_s >= 0 else None
```

### Comparing `saenopy-1.0.2/saenopy/mesh.py` & `saenopy-1.0.4/saenopy/mesh.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/multigrid_helper.py` & `saenopy-1.0.4/saenopy/multigrid_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 
 def get_nodes_with_one_face(tetrahedra):
     # get the faces of the tetrahedrons
     faces = np.sort(np.array(tetrahedra[:, [[0, 1, 2], [0, 1, 3], [0, 2, 3], [1, 2, 3]]]).reshape(-1, 3), axis=1)
     # encode the faces as integers
     maxi = np.max(faces) + 1
+    assert maxi<=(np.iinfo(faces.dtype).max)**(1/3)
     face_index = faces[:, 0] * maxi ** 2 + faces[:, 1] * maxi ** 1 + faces[:, 2]
     # count how often each face is present
     face_counts = pd.Series(face_index).value_counts()
     # filter only faces that occur once
     single_faces = face_counts[face_counts == 1].index
     # get the nodes that belong to these faces
     return np.unique(np.array([single_faces % maxi, (single_faces // maxi) % maxi, (single_faces // maxi ** 2) % maxi]))
```

### Comparing `saenopy-1.0.2/saenopy/result_file.py` & `saenopy-1.0.4/saenopy/result_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import glob
 import re
 from pathlib import Path
+from pathlib import PurePath, PureWindowsPath
 import os
 import natsort
 from typing import List
 import tifffile
 from PIL import Image
 from saenopy.stack import Stack, format_glob
 from saenopy.saveable import Saveable
@@ -223,29 +224,53 @@
         start = values[0]
         while start:
             if all(value.startswith(start) for value in values):
                 return start
             start = start[:-1]
 
 
-def make_path_relative(template, output):
-    template = str(Path(template).absolute())
-    output = str(Path(output).absolute())
-    # relative and optionally go up to two folders up
+def is_relative_to(path, base):
+    """
+    Check if 'path' is relative to 'base'.
+    """
     try:
-        template = Path(template).relative_to(output)
+        path.relative_to(base)
+        return True
     except ValueError:
-        try:
-            template = Path("..") / Path(template).relative_to(Path(output).parent)
-        except ValueError:
-            try:
-                template = Path("../..") / Path(template).relative_to(Path(output).parent.parent)
-            except ValueError:
-                pass
-    return str(template)
+        return False
+
+def make_path_relative(filename, base):
+    """
+    Returns the relative path of `filename` with respect to the `base` directory,
+    working cross-platform for Windows paths on non-Windows systems.
+
+    :param filename: The path of the file.
+    :param base: The base directory to which the path should be relative.
+    :return: The relative path of the file.
+    """
+    # Convert to PurePath for cross-platform compatibility
+    base_path = PurePath(base)
+    file_path = PurePath(filename)
+
+    # Use PureWindowsPath if on a non-Windows system handling Windows paths
+    if not isinstance(base_path, PureWindowsPath) and '\\' in str(base):
+        base_path = PureWindowsPath(base)
+    if not isinstance(file_path, PureWindowsPath) and '\\' in str(filename):
+        file_path = PureWindowsPath(filename)
+
+    if not file_path.is_absolute():
+        return file_path
+
+    offset = ""
+    for i in range(3):
+        if is_relative_to(file_path,base_path):
+            return str(offset / file_path.relative_to(base_path))
+        base_path = base_path.parent
+        offset /= PurePath("..")
+    return file_path
 
 
 def make_path_absolute(template, output):
     if not Path(template).is_absolute():
         return str(Path(output).absolute() / template)
     return str(Path(template).absolute())
 
@@ -425,15 +450,15 @@
             ]
             apply_rename(data_dict, renames)
             apply_delete(data_dict, renames)
 
             data_dict["___save_version__"] = "1.4"
         return super().from_dict(data_dict)
 
-    def __init__(self, output=None, template=None, stack=None, time_delta=None, **kwargs):
+    def __init__(self, output=None, template="", stack=None, time_delta=None, **kwargs):
         if output is not None:
             self.output = str(Path(output).absolute())
 
         self.stacks = stack
         if stack is None:
             self.stacks = []
         self.stack_parameters = dict(z_project_name=None, z_project_range=0)
@@ -452,15 +477,15 @@
 
         # add a reference to this instance to the stacks, so they know the path
         if output is not None:
             for stack in self.stacks:
                 stack.paths_relative(self)
             if self.stack_reference is not None:
                 self.stack_reference.paths_relative(self)
-            self.template = make_path_relative(self.template, Path(self.output).parent)
+            self.template = str(make_path_relative(self.template, Path(self.output).parent))
 
 
         # if demo move parts to simulate empty result
         if os.environ.get("DEMO") == "true":  # pragma: no cover
             self.mesh_piv_demo = self.mesh_piv
             self.solver_demo = self.solvers
             if self.solvers[0] is not None and getattr(self.solvers[0], "regularisation_results", None):
@@ -513,14 +538,16 @@
             stack.parent = self
         if self.stack_reference is not None:
             self.stack_reference.parent = self
 
     def __repr__(self):
         folders = [str(Path(stack.template)) for stack in self.stacks]
         base_folder = common_start(folders)
+        if base_folder is None:
+            base_folder = " "
         base_folder = os.sep.join(base_folder.split(os.sep)[:-1])
         indent = "    "
         text = "Result(" + "\n"
         text += indent + "output = " + self.output + "\n"
         if self.template is not None:
             text += indent + "template = " + self.template + "\n"
         text += indent + "stacks = [" + "\n"
@@ -541,7 +568,81 @@
             text += indent + "mesh_parameters = " + str(self.mesh_parameters) + "\n"
         if self.material_parameters:
             text += indent + "material_parameters = " + str(self.material_parameters) + "\n"
         if self.solve_parameters:
             text += indent + "solve_parameters = " + str(self.solve_parameters) + "\n"
         text += ")" + "\n"
         return text
+
+    def get_data_structure(self):
+        return {
+            "dimensions": 3,
+            "time_point_count": len(self.stacks),
+            "has_reference": self.stack_reference is not None,
+            "z_slices_count": self.stacks[0].shape[2] if self.stacks else 0,
+            "im_shape": self.stacks[0].shape if self.stacks else (0,0,0),
+            "voxel_size": self.stacks[0].voxel_size if self.stacks else (0,0,0),
+            "time_delta": self.time_delta,
+            "channels": self.stacks[0].channels if self.stacks else [],
+            "fields": {
+                "piv": {
+                    "type": "vector",
+                    "measure": "deformation",
+                    "unit": "m",
+                    "name": "displacements_measured",
+                },
+                "target deformations": {
+                    "type": "vector",
+                    "measure": "deformation",
+                    "unit": "m",
+                    "name": "displacements_target",
+                },
+                "fitted deformations": {
+                    "type": "vector",
+                    "measure": "deformation",
+                    "unit": "m",
+                    "name": "displacements",
+                },
+                "fitted forces": {
+                    "type": "vector",
+                    "measure": "force",
+                    "unit": "N",
+                    "name": "forces",
+                }
+            }
+        }
+
+    def get_image_data(self, time_point, channel="default", use_reference=False):
+        if use_reference and self.stack_reference:
+            stack = self.stack_reference
+        else:
+            stack = self.stacks[time_point]
+        if isinstance(channel, str):
+            try:
+                channel = self.stacks[0].channels.index(channel)
+            except ValueError:
+                channel = 0
+        if channel >= len(stack.channels):
+            channel = 0
+        return stack[:, :, :, :, channel]
+
+    def get_field_data(result, name, time_point):
+        try:
+            if name == "piv":
+                mesh = result.mesh_piv[time_point]
+                if mesh is not None and mesh.displacements_measured is not None:
+                    return mesh, mesh.displacements_measured
+            elif name == "target deformations":
+                M = result.solvers[time_point]
+                if M is not None:
+                    return M.mesh, M.mesh.displacements_target
+            elif name == "fitted deformations":
+                M = result.solvers[time_point]
+                if M is not None:
+                    return M.mesh, M.mesh.displacements
+            elif name == "fitted forces":
+                M = result.solvers[time_point]
+                if M is not None:
+                    return M.mesh, -M.mesh.forces * M.mesh.regularisation_mask[:, None]
+        except IndexError:
+            return None, None         
+        return None, None
```

### Comparing `saenopy-1.0.2/saenopy/saveable.py` & `saenopy-1.0.4/saenopy/saveable.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,19 @@
         if file_format is None:
             file_format = Path(filename).suffix
 
         data = self.to_dict()
 
         if file_format == ".h5py" or file_format == ".h5":  # pragma: no cover
             return dict_to_h5(filename, flatten_dict(data))
-        elif file_format == ".npz" or file_format == ".saenopy":
+        elif file_format == ".npz" or file_format == ".saenopy" or file_format == ".saenopy2D" or file_format == ".saenopySpheroid":
             #np.savez(filename, **data)
             np.lib.npyio._savez(filename, [], flatten_dict(data), True, allow_pickle=False)
             import shutil
-            if file_format == ".saenopy":
+            if file_format == ".saenopy" or file_format == ".saenopy2D" or file_format == ".saenopySpheroid":
                 shutil.move(filename+".npz", filename)
         else:
             raise ValueError("format not supported")
 
     @classmethod
     def from_dict(cls, data_dict):
         types = typing.get_type_hints(cls)
@@ -83,15 +83,15 @@
         from pathlib import Path
         if file_format is None:
             file_format = Path(filename).suffix
         if file_format == ".h5py" or file_format == ".h5":  # pragma: no cover
             import h5py
             data = h5py.File(filename, "a")
             result = cls.from_dict(unflatten_dict_h5(data))
-        elif file_format == ".npz" or file_format == ".saenopy":
+        elif file_format == ".npz" or file_format == ".saenopy" or file_format == ".saenopy2D" or file_format == ".saenopySpheroid":
             data = np.load(filename, allow_pickle=False)
 
             result = cls.from_dict(unflatten_dict(data))
         else:
             raise ValueError("Unknown format")
         if getattr(result, 'on_load', None) is not None:
             getattr(result, 'on_load')(filename)
```

### Comparing `saenopy-1.0.2/saenopy/solver.py` & `saenopy-1.0.4/saenopy/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,15 @@
             else:
                 self.localweight *= 1.0
 
         index = self.localweight < 1e-10
         self.localweight[index & self.mesh.movable] = 1e-10
 
         if self.mesh.cell_boundary_mask is not None:
-            self.localweight[:] = 0.03
+            self.localweight[:] = 0.03*100
             self.localweight[self.mesh.cell_boundary_mask] = 0.003*0.001
 
         self.localweight[~self.mesh.regularisation_mask] = 0
 
         counter = np.sum(1.0 - self.localweight[self.mesh.movable])
         counterall = np.sum(self.mesh.movable)
 
@@ -996,14 +996,21 @@
 
 
 def load_solver(filename: str) -> Solver:
     return Solver.load(filename)
 
 
 def load(filename: str) -> Result:
+    from saenopy.gui.spheroid.modules.result import ResultSpheroid
+    from saenopy.gui.tfm2d.modules.result import Result2D
+
+    if filename.endswith(".saenopySpheroid"):
+        return ResultSpheroid.load(filename)
+    if filename.endswith(".saenopy2D"):
+        return Result2D.load(filename)
     return Result.load(filename)
 
 
 def load_results(filename: str) -> List[Result]:
     import glob
     return [Result.load(file) for file in glob.glob(filename, recursive=True)]
```

### Comparing `saenopy-1.0.2/saenopy/stack.py` & `saenopy-1.0.4/saenopy/stack.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/saenopy/unused/macro.py` & `saenopy-1.0.4/saenopy/unused/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.2/PKG-INFO` & `saenopy-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: saenopy
-Version: 1.0.2
+Version: 1.0.4
 Summary: Semi-elastic fiber optimisation in python.
 License: MIT
 Author: rgerum
 Author-email: 14153051+rgerum@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: black (>=24.4.0,<25.0.0)
 Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: imagecodecs (>=2022.9.26,<2023.0.0)
 Requires-Dist: jointforces (>=1.0.1,<2.0.0)
 Requires-Dist: natsort (>=8.2.0,<9.0.0)
-Requires-Dist: nbsphinx (>=0.8.10,<0.9.0) ; extra == "docs"
+Requires-Dist: nbsphinx (>=0.9.2,<0.10.0) ; extra == "docs"
 Requires-Dist: nptyping (>=2.4.1,<3.0.0)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: openpiv (>=0.24.2,<0.25.0)
 Requires-Dist: pyfields (>=1.7.0,<2.0.0)
-Requires-Dist: pyqt5 (>=5.15.7,<6.0.0)
+Requires-Dist: pyqt5 (==5.15.9)
+Requires-Dist: pyqt5-qt5 (==5.15.2)
 Requires-Dist: pyvista (>=0.37.0,<0.38.0)
 Requires-Dist: pyvistaqt (>=0.9.0,<0.10.0)
 Requires-Dist: qimage2ndarray (>=1.9.0,<2.0.0)
 Requires-Dist: qtawesome (>=1.2.1,<2.0.0)
 Requires-Dist: qtrangeslider (>=0.1.5,<0.2.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
-Requires-Dist: sphinx-gallery (>=0.11.1,<0.12.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
+Requires-Dist: solidspy
+Requires-Dist: sphinx (>=1.6,<7) ; extra == "docs"
+Requires-Dist: sphinx-gallery (>=0.13.0,<0.14.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.2.2,<2.0.0) ; extra == "docs"
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 SAENOPY
 =======
 
 [![DOC](https://readthedocs.org/projects/saenopy/badge/)](https://saenopy.readthedocs.io)
@@ -59,18 +62,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.3/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.3/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

