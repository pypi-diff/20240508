# Comparing `tmp/rad-0.19.3.tar.gz` & `tmp/rad-0.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.19.3.tar", last modified: Fri Apr 26 14:01:09 2024, max compression
+gzip compressed data, was "rad-0.19.4.tar", last modified: Wed May  8 20:40:30 2024, max compression
```

## Comparing `rad-0.19.3.tar` & `rad-0.19.4.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.142450 rad-0.19.3/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 14:00:57.000000 rad-0.19.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 14:00:57.000000 rad-0.19.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 14:00:57.000000 rad-0.19.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 14:00:57.000000 rad-0.19.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-26 14:00:57.000000 rad-0.19.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 14:00:57.000000 rad-0.19.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-26 14:00:57.000000 rad-0.19.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-26 14:00:57.000000 rad-0.19.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-26 14:00:57.000000 rad-0.19.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-26 14:00:57.000000 rad-0.19.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-26 14:00:57.000000 rad-0.19.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 14:01:09.142450 rad-0.19.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-26 14:00:57.000000 rad-0.19.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-04-26 14:00:57.000000 rad-0.19.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 14:00:57.000000 rad-0.19.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-26 14:00:57.000000 rad-0.19.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-26 14:00:57.000000 rad-0.19.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-26 14:00:57.000000 rad-0.19.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-04-26 14:00:57.000000 rad-0.19.3/docs/creating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 14:00:57.000000 rad-0.19.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-26 14:00:57.000000 rad-0.19.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 14:00:57.000000 rad-0.19.3/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-26 14:00:57.000000 rad-0.19.3/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-26 14:00:57.000000 rad-0.19.3/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-26 14:00:57.000000 rad-0.19.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.122450 rad-0.19.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-04-26 14:00:57.000000 rad-0.19.3/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-04-26 14:00:57.000000 rad-0.19.3/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:01:09.142450 rad-0.19.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.118450 rad-0.19.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.126450 rad-0.19.3/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.134450 rad-0.19.3/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/base_exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/fps-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ground_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/msos_stack-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/source_catalog-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tvac-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-26 14:00:57.000000 rad-0.19.3/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 14:01:09.000000 rad-0.19.3/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:01:09.138450 rad-0.19.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:00:57.000000 rad-0.19.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 14:00:57.000000 rad-0.19.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-26 14:00:57.000000 rad-0.19.3/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 14:00:57.000000 rad-0.19.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.926424 rad-0.19.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:40:20.000000 rad-0.19.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.902424 rad-0.19.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 20:40:20.000000 rad-0.19.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:40:20.000000 rad-0.19.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.902424 rad-0.19.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-08 20:40:20.000000 rad-0.19.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-08 20:40:20.000000 rad-0.19.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 20:40:20.000000 rad-0.19.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 20:40:20.000000 rad-0.19.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-08 20:40:20.000000 rad-0.19.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-08 20:40:20.000000 rad-0.19.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 20:40:20.000000 rad-0.19.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 20:40:20.000000 rad-0.19.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-08 20:40:30.926424 rad-0.19.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-08 20:40:20.000000 rad-0.19.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 20:40:20.000000 rad-0.19.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59966 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.898424 rad-0.19.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-08 20:40:20.000000 rad-0.19.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 20:40:20.000000 rad-0.19.4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-08 20:40:20.000000 rad-0.19.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 20:40:20.000000 rad-0.19.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20610 2024-05-08 20:40:20.000000 rad-0.19.4/docs/creating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 20:40:20.000000 rad-0.19.4/docs/ground_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-08 20:40:20.000000 rad-0.19.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-08 20:40:20.000000 rad-0.19.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 20:40:20.000000 rad-0.19.4/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 20:40:20.000000 rad-0.19.4/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-08 20:40:20.000000 rad-0.19.4/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-08 20:40:20.000000 rad-0.19.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-08 20:40:20.000000 rad-0.19.4/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      954 2024-05-08 20:40:20.000000 rad-0.19.4/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:40:30.926424 rad-0.19.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.898424 rad-0.19.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.906424 rad-0.19.4/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.910424 rad-0.19.4/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.910424 rad-0.19.4/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.918424 rad-0.19.4/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/base_exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/base_guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/fps-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ground_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/outlier_detection-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/segmentation_map-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/source_catalog-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tvac-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15054 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-08 20:40:20.000000 rad-0.19.4/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 20:40:30.000000 rad-0.19.4/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:30.922424 rad-0.19.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:40:20.000000 rad-0.19.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 20:40:20.000000 rad-0.19.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-08 20:40:20.000000 rad-0.19.4/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-08 20:40:20.000000 rad-0.19.4/tox.ini
```

### Comparing `rad-0.19.3/.github/pull_request_template.md` & `rad-0.19.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/.github/workflows/changelog.yml` & `rad-0.19.4/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/.github/workflows/ci_cron.yml` & `rad-0.19.4/.github/workflows/ci_cron.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/.github/workflows/release.yml` & `rad-0.19.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/.gitignore` & `rad-0.19.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/.pre-commit-config.yaml` & `rad-0.19.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/CHANGES.rst` & `rad-0.19.4/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-0.19.4 (unreleased)
+0.20.0 (unreleased)
 -------------------
 
+- 
 
+0.19.4 (2024-05-08)
+-------------------
+
+- Updated RTD with documentation for new data products. [#419]
 
 0.19.3 (2024-04-25)
 -------------------
 
 - Duplicated the keywords from groundtest to tvac_groundtest. [#409]
 
 
@@ -43,15 +48,15 @@
 - Create the flux step schema. [#395]
 
 - Create ``outlier_detection`` schema and add bit mask field to both it and ``resample``. [#401]
 
 - Add source_catalog and segmentation_map schemas for Level 2 and Level 3 files. [#393]
 
 
-  0.19.0 (2024-02-09)
+0.19.0 (2024-02-09)
 -------------------
 
 - Added streamlined Level 3 Mosaic metadata schemas. [#334]
 
 - Remove the unused ``variance-1.0.0`` schema. [#344]
 
 - Add wcs tag to wfi_image and wfi_mosaic schemas. [#351]
```

### Comparing `rad-0.19.3/CODE_OF_CONDUCT.md` & `rad-0.19.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/LICENSE` & `rad-0.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/PKG-INFO` & `rad-0.19.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.3
+Version: 0.19.4
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.3/README.md` & `rad-0.19.4/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/Makefile` & `rad-0.19.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/_static/custom.css` & `rad-0.19.4/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/_static/stsci_logo.png` & `rad-0.19.4/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/conf.py` & `rad-0.19.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/creating.rst` & `rad-0.19.4/docs/creating.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/index.rst` & `rad-0.19.4/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 .. toctree::
   :maxdepth: 1
 
   schemas.rst
   reference_files.rst
   manifests.rst
+  ground_tests.rst
 
 Developer Resources
 ===================
 
 .. toctree::
   :maxdepth: 1
```

### Comparing `rad-0.19.3/docs/make.bat` & `rad-0.19.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/reference_files.rst` & `rad-0.19.4/docs/reference_files.rst`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/docs/schemas.rst` & `rad-0.19.4/docs/schemas.rst`

 * *Files 23% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 Level 3 (resampled mosaic) File schema
 --------------------------------------
 
 .. asdf-autoschemas::
 
   wfi_mosaic-1.0.0
 
+Level 4 File schemas
+--------------------
+
+.. asdf-autoschemas::
+
+  source_catalog-1.0.0
+  segmentation_map-1.0.0
+  mosaic_source_catalog-1.0.0
+  mosaic_segmentation_map-1.0.0
+
+
 Tags
 ----
 
 .. asdf-autoschemas::
 
     aperture-1.0.0
     associations-1.0.0
@@ -61,7 +72,15 @@
     target-1.0.0
     velocity_aberration-1.0.0
     visit-1.0.0
     wcsinfo-1.0.0
     wfi_detector-1.0.0
     wfi_mode-1.0.0
     wfi_optical_element-1.0.0
+    tagged_scalars/file_date-1.0.0
+    tagged_scalars/calibration_software_version-1.0.0
+    tagged_scalars/filename-1.0.0
+    tagged_scalars/model_type-1.0.0
+    tagged_scalars/origin-1.0.0
+    tagged_scalars/prd_software_version-1.0.0
+    tagged_scalars/sdf_software_version-1.0.0
+    tagged_scalars/telescope-1.0.0
```

### Comparing `rad-0.19.3/pyproject.toml` & `rad-0.19.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/scripts/insert_next_release.py` & `rad-0.19.4/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/scripts/set_release_date.py` & `rad-0.19.4/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/integration.py` & `rad-0.19.4/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.19.4/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/base_exposure-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/base_exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/base_guidestar-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/base_guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/exposure_type-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/fps-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/fps-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/ground_common-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/ground_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/groundtest-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/groundtest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/individual_image_meta-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/l2_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/l3_cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/mosaic_basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/mosaic_segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/mosaic_source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/mosaic_wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/msos_stack-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/inverselinearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/segmentation_map-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/segmentation_map-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/source_catalog-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/source_catalog-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tvac-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tvac-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/tvac_groundtest-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.19.4/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/src/rad.egg-info/PKG-INFO` & `rad-0.19.4/src/rad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.19.3
+Version: 0.19.4
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.19.3/src/rad.egg-info/SOURCES.txt` & `rad-0.19.4/src/rad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .github/workflows/ci_cron.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/changes.rst
 docs/conf.py
 docs/contributing.rst
 docs/creating.rst
+docs/ground_tests.rst
 docs/index.rst
 docs/make.bat
 docs/manifests.rst
 docs/reference_files.rst
 docs/schemas.rst
 docs/_static/custom.css
 docs/_static/stsci_logo.png
```

### Comparing `rad-0.19.3/tests/test_integration.py` & `rad-0.19.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/tests/test_manifest.py` & `rad-0.19.4/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/tests/test_schemas.py` & `rad-0.19.4/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `rad-0.19.3/tox.ini` & `rad-0.19.4/tox.ini`

 * *Files identical despite different names*

